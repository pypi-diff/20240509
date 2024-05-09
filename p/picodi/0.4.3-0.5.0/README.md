# Comparing `tmp/picodi-0.4.3.tar.gz` & `tmp/picodi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.4.3.tar", max compression
+gzip compressed data, was "picodi-0.5.0.tar", max compression
```

## Comparing `picodi-0.4.3.tar` & `picodi-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-05-08 11:08:11.997047 picodi-0.4.3/LICENSE
--rw-r--r--   0        0        0     6904 2024-05-08 11:08:11.997047 picodi-0.4.3/README.md
--rw-r--r--   0        0        0      265 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/__init__.py
--rw-r--r--   0        0        0     9298 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/py.typed
--rw-r--r--   0        0        0     4253 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/scopes.py
--rw-r--r--   0        0        0     2604 2024-05-08 11:08:12.001047 picodi-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     7666 1970-01-01 00:00:00.000000 picodi-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-09 12:30:57.572187 picodi-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6904 2024-05-09 12:30:57.572187 picodi-0.5.0/README.md
+-rw-r--r--   0        0        0      265 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/__init__.py
+-rw-r--r--   0        0        0     9882 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/picodi.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/py.typed
+-rw-r--r--   0        0        0     2973 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/scopes.py
+-rw-r--r--   0        0        0     2604 2024-05-09 12:30:57.572187 picodi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7666 1970-01-01 00:00:00.000000 picodi-0.5.0/PKG-INFO
```

### Comparing `picodi-0.4.3/LICENSE` & `picodi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.4.3/README.md` & `picodi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `picodi-0.4.3/picodi/picodi.py` & `picodi-0.5.0/picodi/picodi.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,62 +2,52 @@
 
 import asyncio
 import functools
 import inspect
 import threading
 from collections.abc import Awaitable, Callable
 from contextlib import asynccontextmanager, contextmanager
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     ContextManager,
     ParamSpec,
     TypeVar,
     cast,
 )
 
-from picodi.scopes import ExitStack, NullScope, Scope, SingletonScope
+from picodi.scopes import GlobalScope, NullScope, Scope, SingletonScope
 
 if TYPE_CHECKING:
     from inspect import BoundArguments, Signature
 
-try:
-    import fastapi.params
-except ImportError:
-    fastapi = None  # type: ignore[assignment]
-
-
-Dependency = Callable[..., Any]
+DependencyCallable = Callable[..., Any]
 T = TypeVar("T")
 P = ParamSpec("P")
 TC = TypeVar("TC", bound=Callable)
 
 
 _unset = object()
-_resources: list[Depends] = []
 _lock = threading.RLock()
-_scopes: dict[str, Scope] = {
-    "null": NullScope(),
-    "singleton": SingletonScope(),
+_registry: dict[DependencyCallable, Provider] = {}
+_scopes: dict[type[Scope], Scope] = {
+    NullScope: NullScope(),
+    SingletonScope: SingletonScope(),
 }
 
 
-def _is_fastapi_dependency(value: Any) -> bool:
-    return bool(fastapi and isinstance(value, fastapi.params.Depends))
-
-
-def Provide(dependency: Dependency, /) -> Any:  # noqa: N802
+def Provide(dependency: DependencyCallable, /) -> Any:  # noqa: N802
     """
     Declare a provider.
     It takes a single "dependency" callable (like a function).
     Don't call it directly, picodi will call it for you.
-    Dependency can be a regular function or a generator with one yield.
+    DependencyCallable can be a regular function or a generator with one yield.
     If the dependency is a generator, it will be used as a context manager.
     Any generator that is valid for `contextlib.contextmanager`
     can be used as a dependency.
 
     Example:
     ```
     from picodi import Provide, inject
@@ -67,15 +57,21 @@
         print("closing db connection")
 
     @inject
     def my_service(db: str = Provide(get_db)):
         assert db == "db connection"
     ```
     """
-    return Depends.from_dependency(dependency)
+    with _lock:
+        if dependency not in _registry:
+            _registry[dependency] = Provider.from_dependency(dependency, in_use=True)
+        elif not _registry[dependency].in_use:
+            _registry[dependency] = _registry[dependency].replace(in_use=True)
+
+    return Dependency(dependency)
 
 
 def inject(fn: Callable[P, T]) -> Callable[P, T]:
     """
     Decorator to inject dependencies into a function.
     Use it in combination with `Provide` to declare dependencies.
     Should be placed first in the decorator chain (on bottom).
@@ -96,38 +92,37 @@
         async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             bound, dep_arguments = _arguments_to_getters(
                 args, kwargs, signature, is_async=True
             )
             for name, get_value in dep_arguments.items():
                 bound.arguments[name] = await get_value()
 
-            async with ExitStack() as stack:
-                for scope in _scopes.values():
-                    await stack.enter_context(scope)
-                result_or_gen = fn(*bound.args, **bound.kwargs)
-                if inspect.isasyncgen(result_or_gen):
-                    result = result_or_gen
-                else:
-                    result = await result_or_gen  # type: ignore[misc]
+            result_or_gen = fn(*bound.args, **bound.kwargs)
+            if inspect.isasyncgen(result_or_gen):
+                result = result_or_gen
+            else:
+                result = await result_or_gen  # type: ignore[misc]
+
+            for scope in _scopes.values():
+                await scope.close_local()
             return cast("T", result)
 
     else:
 
         @functools.wraps(fn)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             bound, dep_arguments = _arguments_to_getters(
                 args, kwargs, signature, is_async=False
             )
             for name, get_value in dep_arguments.items():
                 bound.arguments[name] = get_value()
 
-            with ExitStack() as stack:
-                for scope in _scopes.values():
-                    stack.enter_context(scope, sync_first=True)
-                result = fn(*bound.args, **bound.kwargs)
+            result = fn(*bound.args, **bound.kwargs)
+            for scope in _scopes.values():
+                scope.close_local()
             return result
 
     wrapper._picodi_inject_ = True  # type: ignore[attr-defined] # noqa: SF01
     return wrapper  # type: ignore[return-value]
 
 
 def resource(fn: TC) -> TC:
@@ -135,47 +130,48 @@
     Decorator to declare a resource. Resource is a dependency that should be
     called only once, cached and shared across the application.
     On shutdown, all resources will be closed
     (you need to call `shutdown_resources` manually).
     Use it with a dependency generator function to declare a resource.
     Should be placed last in the decorator chain (on top).
     """
-    fn._picodi_scope_ = "singleton"  # type: ignore[attr-defined] # noqa: SF01
     with _lock:
-        _resources.append(Depends.from_dependency(fn))
+        if fn in _registry:
+            provider = _registry[fn].replace(scope_class=SingletonScope)
+        else:
+            provider = Provider.from_dependency(
+                fn, scope_class=SingletonScope, in_use=False
+            )
+        _registry[fn] = provider
     return fn
 
 
 def init_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
     """
     async_resources = []
-    for depends in _resources:
-        if depends.is_async:
-            async_resources.append(_resolve_value_async(depends))
-        else:
-            _resolve_value(depends)
+    for provider in _registry.values():
+        if provider.in_use and issubclass(provider.scope_class, GlobalScope):
+            if provider.is_async:
+                async_resources.append(_resolve_value_async(provider))
+            else:
+                _resolve_value(provider)
 
     return asyncio.gather(*async_resources)
 
 
 def shutdown_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shut down.
     """
-    if _is_async_environment():
-        tasks = [scope.exit_stack.close() for scope in _scopes.values()]
-        return asyncio.gather(*tasks)  # type: ignore[arg-type]
-
-    for scope in _scopes.values():
-        scope.exit_stack.close(only_sync=True)
-    return asyncio.gather(*[])
+    tasks = [scope.close_global() for scope in _scopes.values()]
+    return asyncio.gather(*tasks)
 
 
 def make_dependency(fn: Callable[P, T], *args: Any, **kwargs: Any) -> Callable[..., T]:
     signature = inspect.signature(fn)
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
 
@@ -191,29 +187,60 @@
     return wrapper
 
 
 CallableManager = Callable[..., AsyncContextManager | ContextManager]
 
 
 @dataclass(frozen=True)
-class Depends:
-    dependency: Dependency
+class Dependency:
+    original: DependencyCallable
+
+    def __call__(self) -> Dependency:
+        return self
+
+    def get_provider(self) -> Provider:
+        return _registry[self.original]
+
+
+@dataclass(frozen=True)
+class Provider:
+    dependency: DependencyCallable
     is_async: bool = field(compare=False)
+    scope_class: type[Scope] = field(compare=False)
+    in_use: bool = field(compare=False)
 
     @classmethod
-    def from_dependency(cls, dependency: Dependency) -> Depends:
+    def from_dependency(
+        cls,
+        dependency: DependencyCallable,
+        scope_class: type[Scope] = NullScope,
+        in_use: bool = False,
+    ) -> Provider:
+        is_async = inspect.iscoroutinefunction(
+            dependency
+        ) or inspect.isasyncgenfunction(dependency)
         return cls(
-            dependency,
-            inspect.iscoroutinefunction(dependency)
-            or inspect.isasyncgenfunction(dependency),
+            dependency=dependency,
+            is_async=is_async,
+            scope_class=scope_class,
+            in_use=in_use,
         )
 
+    def replace(
+        self, scope_class: type[Scope] | None = None, in_use: bool | None = None
+    ) -> Provider:
+        kwargs = asdict(self)
+        if scope_class is not None:
+            kwargs["scope_class"] = scope_class
+        if in_use is not None:
+            kwargs["in_use"] = in_use
+        return Provider(**kwargs)
+
     def get_scope(self) -> Scope:
-        scope_name = getattr(self.dependency, "_picodi_scope_", "null")
-        return _scopes[scope_name]
+        return _scopes[self.scope_class]
 
     def resolve_value(self) -> Any:
         scope = self.get_scope()
         value_or_gen = self.dependency()
         if self.is_async:
 
             async def resolve_value_inner() -> Any:
@@ -230,73 +257,60 @@
             return resolve_value_inner()
 
         if inspect.isgenerator(value_or_gen):
             context_manager = contextmanager(lambda *args, **kwargs: value_or_gen)
             return scope.exit_stack.enter_context(context_manager())
         return value_or_gen
 
-    def __call__(self) -> Depends:
-        return self
-
 
 def _arguments_to_getters(
     args: P.args, kwargs: P.kwargs, signature: Signature, is_async: bool
 ) -> tuple[BoundArguments, dict[str, Callable[[], Any]]]:
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
-    dependencies: dict[Depends, list[str]] = {}
+    dependencies: dict[Provider, list[str]] = {}
     for name, value in bound.arguments.items():
-        if _is_fastapi_dependency(value):
-            value = value.dependency
-        if isinstance(value, Depends):
-            dependencies.setdefault(value, []).append(name)
+        if isinstance(value, Dependency):
+            dependencies.setdefault(value.get_provider(), []).append(name)
 
     get_val = _resolve_value_async if is_async else _resolve_value
 
     dep_arguments = {}
-    for depends, names in dependencies.items():
-        get_value: Callable = functools.partial(get_val, depends)
+    for provider, names in dependencies.items():
+        get_value: Callable = functools.partial(get_val, provider)
         for name in names:
             dep_arguments[name] = get_value
 
     return bound, dep_arguments
 
 
-def _resolve_value(depends: Depends) -> Any:
-    scope = depends.get_scope()
+def _resolve_value(provider: Provider) -> Any:
+    scope = provider.get_scope()
     try:
-        value = scope.get(depends.dependency)
+        value = scope.get(provider.dependency)
     except KeyError:
-        if depends.is_async:
-            value = depends.dependency()
+        if provider.is_async:
+            value = provider.dependency()
         else:
             with _lock:
                 try:
-                    value = scope.get(depends.dependency)
+                    value = scope.get(provider.dependency)
                 except KeyError:
-                    value = depends.resolve_value()
-                    scope.set(depends.dependency, value)
+                    value = provider.resolve_value()
+                    scope.set(provider.dependency, value)
     return value
 
 
-async def _resolve_value_async(depends: Depends) -> Any:
-    scope = depends.get_scope()
+async def _resolve_value_async(provider: Provider) -> Any:
+    scope = provider.get_scope()
     try:
-        value = scope.get(depends.dependency)
+        value = scope.get(provider.dependency)
     except KeyError:
         with _lock:
             try:
-                value = scope.get(depends.dependency)
+                value = scope.get(provider.dependency)
             except KeyError:
-                value = depends.resolve_value()
-                if depends.is_async:
+                value = provider.resolve_value()
+                if provider.is_async:
                     value = await value
-                scope.set(depends.dependency, value)
+                scope.set(provider.dependency, value)
     return value
-
-
-def _is_async_environment() -> bool:
-    try:
-        asyncio.get_running_loop()
-    except RuntimeError:
-        return False
-    return True
```

### Comparing `picodi-0.4.3/pyproject.toml` & `picodi-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.4.3"
+version = "0.5.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.4.3/PKG-INFO` & `picodi-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.4.3
+Version: 0.5.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```
