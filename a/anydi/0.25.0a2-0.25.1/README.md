# Comparing `tmp/anydi-0.25.0a2.tar.gz` & `tmp/anydi-0.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.25.0a2.tar", max compression
+gzip compressed data, was "anydi-0.25.1.tar", max compression
```

## Comparing `anydi-0.25.0a2.tar` & `anydi-0.25.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.0a2/LICENSE
--rw-r--r--   0        0        0     3414 2024-05-08 08:47:53.359541 anydi-0.25.0a2/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.0a2/anydi/__init__.py
--rw-r--r--   0        0        0    27978 2024-05-08 08:36:20.511875 anydi-0.25.0a2/anydi/_container.py
--rw-r--r--   0        0        0    10215 2024-05-08 08:36:20.512415 anydi-0.25.0a2/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.0a2/anydi/_logger.py
--rw-r--r--   0        0        0     3675 2024-05-08 08:27:43.981700 anydi-0.25.0a2/anydi/_module.py
--rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.25.0a2/anydi/_scanner.py
--rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.25.0a2/anydi/_types.py
--rw-r--r--   0        0        0     3439 2024-05-08 08:36:20.513338 anydi-0.25.0a2/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.0a2/anydi/ext/__init__.py
--rw-r--r--   0        0        0      223 2024-05-08 08:36:17.250672 anydi-0.25.0a2/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-08 08:36:17.250922 anydi-0.25.0a2/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      828 2024-05-08 08:36:17.251228 anydi-0.25.0a2/anydi/ext/django/_settings.py
--rw-r--r--   0        0        0     3491 2024-05-08 08:36:17.251589 anydi-0.25.0a2/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     2760 2024-05-08 08:36:17.251795 anydi-0.25.0a2/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      823 2024-05-08 08:36:17.252105 anydi-0.25.0a2/anydi/ext/django/middleware.py
--rw-r--r--   0        0        0      546 2024-05-08 08:36:17.252306 anydi-0.25.0a2/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 08:36:17.252503 anydi-0.25.0a2/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2213 2024-05-08 08:36:17.252796 anydi-0.25.0a2/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.25.0a2/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     3999 2024-05-08 06:51:25.864651 anydi-0.25.0a2/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.0a2/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.0a2/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.0a2/anydi/py.typed
--rw-r--r--   0        0        0     3109 2024-05-08 08:48:33.072752 anydi-0.25.0a2/pyproject.toml
--rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 anydi-0.25.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.1/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.25.1/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.1/anydi/__init__.py
+-rw-r--r--   0        0        0    27996 2024-05-09 08:20:34.172615 anydi-0.25.1/anydi/_container.py
+-rw-r--r--   0        0        0    10215 2024-05-08 12:47:28.300076 anydi-0.25.1/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.1/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-08 08:27:43.981700 anydi-0.25.1/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.25.1/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.25.1/anydi/_types.py
+-rw-r--r--   0        0        0     3692 2024-05-08 13:39:48.511132 anydi-0.25.1/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.1/anydi/ext/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.25.1/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.25.1/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.25.1/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.25.1/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.25.1/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.25.1/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.25.1/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.25.1/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.25.1/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.25.1/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     3999 2024-05-08 06:51:25.864651 anydi-0.25.1/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.1/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.1/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.1/anydi/py.typed
+-rw-r--r--   0        0        0     3107 2024-05-09 08:27:56.198682 anydi-0.25.1/pyproject.toml
+-rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 anydi-0.25.1/PKG-INFO
```

### Comparing `anydi-0.25.0a2/LICENSE` & `anydi-0.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/README.md` & `anydi-0.25.1/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/__init__.py` & `anydi-0.25.1/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/_container.py` & `anydi-0.25.1/anydi/_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from ._module import Module, ModuleRegistry
 from ._scanner import Scanner
 from ._types import AnyInterface, Interface, Provider, Scope, is_marker
 from ._utils import (
     get_full_qualname,
     get_typed_parameters,
     get_typed_return_annotation,
+    has_resource_origin,
     is_builtin_type,
 )
 
 T = TypeVar("T", bound=Any)
 P = ParamSpec("P")
 
 ALLOWED_SCOPES: dict[Scope, list[Scope]] = {
@@ -719,15 +720,17 @@
         annotation = get_typed_return_annotation(obj)
 
         if annotation is None:
             raise TypeError(
                 f"Missing `{get_full_qualname(obj)}` provider return annotation."
             )
 
-        if get_origin(annotation) in (get_origin(Iterator), get_origin(AsyncIterator)):
+        origin = get_origin(annotation)
+
+        if has_resource_origin(origin):
             args = get_args(annotation)
             if args:
                 return args[0]
             else:
                 raise TypeError(
                     f"Cannot use `{get_full_qualname(obj)}` resource type annotation "
                     "without actual type."
```

### Comparing `anydi-0.25.0a2/anydi/_context.py` & `anydi-0.25.1/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/_module.py` & `anydi-0.25.1/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/_scanner.py` & `anydi-0.25.1/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/_types.py` & `anydi-0.25.1/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/_utils.py` & `anydi-0.25.1/anydi/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import builtins
 import functools
 import inspect
 import sys
-from typing import Any, Callable, ForwardRef, TypeVar, cast
+from typing import Any, AsyncIterator, Callable, ForwardRef, Iterator, TypeVar, cast
 
 from typing_extensions import Annotated, ParamSpec, get_origin
 
 try:
     import anyio  # noqa
 except ImportError:
     anyio = None  # type: ignore[assignment]
@@ -92,14 +92,25 @@
         parameter.replace(
             annotation=get_typed_annotation(parameter.annotation, globalns)
         )
         for name, parameter in inspect.signature(obj).parameters.items()
     ]
 
 
+_resource_origins = (
+    get_origin(Iterator),
+    get_origin(AsyncIterator),
+)
+
+
+def has_resource_origin(origin: Any) -> bool:
+    """Check if the given origin is a resource origin."""
+    return origin in _resource_origins
+
+
 async def run_async(
     func: Callable[P, T],
     /,
     *args: P.args,
     **kwargs: P.kwargs,
 ) -> T:
     """Runs the given function asynchronously using the `anyio` library."""
```

### Comparing `anydi-0.25.0a2/anydi/ext/django/_settings.py` & `anydi-0.25.1/anydi/ext/django/_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Settings(TypedDict):
     CONTAINER_FACTORY: str | None
     STRICT_MODE: bool
     REGISTER_SETTINGS: bool
     REGISTER_COMPONENTS: bool
-    INJECT_URLCONF: str | None
+    INJECT_URLCONF: str | Sequence[str] | None
     MODULES: Sequence[str]
     SCAN_PACKAGES: Sequence[str]
     PATCH_NINJA: bool
 
 
 DEFAULTS = Settings(
     CONTAINER_FACTORY=None,
```

### Comparing `anydi-0.25.0a2/anydi/ext/django/_utils.py` & `anydi-0.25.1/anydi/ext/django/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,18 +90,22 @@
         )
 
 
 def inject_urlpatterns(container: anydi.Container, *, urlconf: str) -> None:
     """Auto-inject the container into views."""
     resolver = get_resolver(urlconf)
     for pattern in iter_urlpatterns(resolver.url_patterns):
+        # Skip already injected views
+        if hasattr(pattern.callback, "_injected"):
+            continue
         # Skip django-ninja views
         if pattern.lookup_str.startswith("ninja."):
             continue  # pragma: no cover
         pattern.callback = container.inject(pattern.callback)
+        pattern.callback._injected = True  # type: ignore[attr-defined]
 
 
 def iter_urlpatterns(
     urlpatterns: list[URLPattern | URLResolver],
 ) -> Iterator[URLPattern]:
     """Iterate over all views in urlpatterns."""
     for url_pattern in urlpatterns:
```

### Comparing `anydi-0.25.0a2/anydi/ext/django/apps.py` & `anydi-0.25.1/anydi/ext/django/apps.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if container_factory_path:
             try:
                 container_factory = cast(
                     Callable[[], anydi.Container], import_string(container_factory_path)
                 )
             except ImportError as exc:
                 raise ImproperlyConfigured(
-                    f"Cannot import container getter '{container_factory_path}'."
+                    f"Cannot import container factory '{container_factory_path}'."
                 ) from exc
             self.container = container_factory()
         else:
             self.container = anydi.Container(
                 strict=self.settings["STRICT_MODE"],
             )
 
@@ -71,12 +71,15 @@
         if self.settings["PATCH_NINJA"]:
             from .ninja import patch_ninja
 
             patch_ninja()
 
         # Auto-injecting the container into views
         if urlconf := self.settings["INJECT_URLCONF"]:
-            inject_urlpatterns(self.container, urlconf=urlconf)
+            if isinstance(urlconf, str):
+                urlconf = [urlconf]
+            for u in urlconf:
+                inject_urlpatterns(self.container, urlconf=u)
 
         # Scan packages
         for scan_package in self.settings["SCAN_PACKAGES"]:
             self.container.scan(scan_package)
```

### Comparing `anydi-0.25.0a2/anydi/ext/django/middleware.py` & `anydi-0.25.1/anydi/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/ext/django/ninja/__init__.py` & `anydi-0.25.1/anydi/ext/django/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/ext/django/ninja/_operation.py` & `anydi-0.25.1/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/ext/django/ninja/_signature.py` & `anydi-0.25.1/anydi/ext/django/ninja/_signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.http import HttpResponse
 from ninja.signature.details import (
     FuncParam,  # noqa
     ViewSignature as BaseViewSignature,
 )
 from ninja.signature.utils import get_path_param_names, get_typed_signature
 
-from anydi._types import Marker  # noqa
+from anydi._types import is_marker  # noqa
 
 
 class ViewSignature(BaseViewSignature):
     def __init__(self, path: str, view_func: Callable[..., Any]) -> None:
         self.view_func = view_func
         self.signature = get_typed_signature(self.view_func)
         self.path = path
@@ -42,15 +42,15 @@
                 continue
 
             if arg.annotation is HttpResponse:
                 self.response_arg = name
                 continue
 
             # Skip default values that are anydi dependency markers
-            if isinstance(arg.default, Marker):
+            if is_marker(arg.default):
                 self.dependencies.append((name, arg.annotation))
                 continue
 
             func_param = self._get_param_type(name, arg)
             self.params.append(func_param)
 
         if hasattr(view_func, "_ninja_contribute_args"):
```

### Comparing `anydi-0.25.0a2/anydi/ext/fastapi.py` & `anydi-0.25.1/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/ext/pytest_plugin.py` & `anydi-0.25.1/anydi/ext/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/anydi/ext/starlette/middleware.py` & `anydi-0.25.1/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a2/pyproject.toml` & `anydi-0.25.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.25.0a2"
+version = "0.25.1"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
```

### Comparing `anydi-0.25.0a2/PKG-INFO` & `anydi-0.25.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.25.0a2
+Version: 0.25.1
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
```

