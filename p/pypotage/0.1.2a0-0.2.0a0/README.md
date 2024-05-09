# Comparing `tmp/pypotage-0.1.2a0.tar.gz` & `tmp/pypotage-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotage-0.1.2a0.tar", last modified: Mon Apr 15 14:49:47 2024, max compression
+gzip compressed data, was "pypotage-0.2.0a0.tar", last modified: Thu May  9 18:37:32 2024, max compression
```

## Comparing `pypotage-0.1.2a0.tar` & `pypotage-0.2.0a0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.586138 pypotage-0.1.2a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.586138 pypotage-0.1.2a0/src/pypotage/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/_chef.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/_ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/_pot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/src/pypotage/chefs/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/chefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/chefs/genericChef.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/chefs/listChef.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/src/pypotage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_abstract_ingredients.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_genericchef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_listchef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_nocall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_pot.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_preparechefline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:37:32.219123 pypotage-0.2.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-09 18:37:32.219123 pypotage-0.2.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-09 18:37:32.219123 pypotage-0.2.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:37:32.215123 pypotage-0.2.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:37:32.215123 pypotage-0.2.0a0/src/pypotage/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:37:32.215123 pypotage-0.2.0a0/src/pypotage/chefsImpl/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/chefsImpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/chefsImpl/genericChef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/chefsImpl/listChef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/kitchen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/pot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/src/pypotage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:37:32.219123 pypotage-0.2.0a0/src/pypotage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-09 18:37:32.000000 pypotage-0.2.0a0/src/pypotage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 18:37:32.000000 pypotage-0.2.0a0/src/pypotage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:37:32.000000 pypotage-0.2.0a0/src/pypotage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 18:37:32.000000 pypotage-0.2.0a0/src/pypotage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:37:32.219123 pypotage-0.2.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_abstract_ingredients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_chef_line_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_decorable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_genericchef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_kitchen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_listchef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_nocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_pot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_preparechefline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-09 18:37:25.000000 pypotage-0.2.0a0/tests/test_priorized.py
```

### Comparing `pypotage-0.1.2a0/src/pypotage/_pot.py` & `pypotage-0.2.0a0/src/pypotage/chefsImpl/genericChef.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,72 @@
-from typing import Callable, Type, TypeVar
-from functools import cache
-from math import inf
-
-from .chefs.listChef import ListChef
-from .chefs.genericChef import GenericChef
-from ._ingredient import (
-    Ingredient,
-    _OrderedIngredientProxy,
-    IngredientProxy,
-    IngredientData,
-    NoCallIngredient
-)
-from .utils import traverse_subclasses
-from ._chef import Chef
-
-
-_B = TypeVar("_B")
-
-
-class _Pot:
-
-    ingredients: dict[Type, list[Ingredient]]
-    chefs: list[Chef]
-
-    def __init__(self) -> None:
-        self.ingredients: dict[Type, list[Ingredient]] = {}
-        self.chefs: list[Chef] = [
-            ListChef(),
-            GenericChef()
-        ]
-
-    def create(self, func: Callable, /,
-               _ingredient: Type[Ingredient],
-               **kwargs) -> Ingredient:
-        ingredient = _ingredient(
-            _c=cache(func),
-            formula=IngredientData(**kwargs))
-        ingredient.formula._type = ingredient.type
-        return ingredient
-
-    def add(self, ingredient: Ingredient) -> Ingredient:
-        _l = self.ingredients.setdefault(
-            (ingredient.formula._type, ingredient.formula._id), [])
-        _l.insert(0, ingredient)
-        return ingredient
-
-    def get(self, formula: IngredientData) -> Ingredient:
-        classes = [formula._type]
-        classes.extend(traverse_subclasses(formula._type))
-
-        ingredients = []
-
-        for _type in classes:
-            ingredient = self.ingredients.get((_type, formula._id))
-            if ingredient is not None:
-                ingredients.extend(ingredient)
+from typing import Generic
 
-        return ingredients
+from ..kitchen import Chef
+from ..ingredient import IngredientProxy, IngredientData, Ingredient
 
-    def prepare(self, _f: _B = None, /,
-                lazy: bool = False, order: int = inf,
-                primary: bool = False, _id: str = None,
-                no_call: bool = False) -> _B:
-        def _wrapper(_f) -> Ingredient:
-            ingredient = self.create(
-                _f, lazy=lazy,
-                _ingredient=NoCallIngredient if no_call else Ingredient,
-                order=order, primary=primary,
-                _id=_id)
 
-            for chef in self.chefs:
-                ingredient = chef.prepare(ingredient)
-
-            self.add(ingredient)
-            return _f
-        return _wrapper(_f) if _f is not None else _wrapper
-
-    def cook(self, _type: _B, _id: str = None) -> IngredientProxy[_B]:
-        if not (_t := getattr(_type, "type", None)):
-            _t = _type
-
-        chef_line = _OrderedIngredientProxy(
-            _f=self.get,
-            formula=IngredientData(_type=_t, _id=_id))
-
-        for chef in self.chefs:
-            chef_line = chef.cook(chef_line)
-
-        return chef_line
+class _GenericIngredientProxy(IngredientProxy):
 
+    def _get_generic_type(self, formula: IngredientData) -> type:
+        return formula.extra.get("__generic_type__")
+
+    def __call__(self, formula: IngredientData) -> list[Ingredient]:
+        ingredients = super().__call__(formula)
+
+        if not ingredients:
+            return ingredients
+
+        _bases = self._get_generic_type(self.formula)
+
+        if _bases is None:
+            return ingredients
+
+        _matches = []
+        for ingredient in ingredients:
+            _ingredient_bases = self._get_generic_type(ingredient.formula)
+            for _ingredient_type, _ingredient_args in _ingredient_bases:
+                for _type, args in _bases:
+                    if not issubclass(_ingredient_type, _type):
+                        continue
+                    if args != _ingredient_args:
+                        continue
+                    _matches.append(ingredient)
+
+        return _matches
+
+
+class GenericChef(Chef):
+
+    @staticmethod
+    def _is_generic(_type: type) -> bool:
+        return isinstance(_type, type) and \
+            issubclass(_type, Generic) or \
+            hasattr(_type, "__origin__") and \
+            issubclass(_type.__origin__, Generic)
+
+    @staticmethod
+    def _get_bases(_type: type) -> list[tuple[type, tuple[type]]]:
+        if hasattr(_type, "__origin__"):
+            return [(_type.__origin__, _type.__args__)]
+        bases = _type.__orig_bases__
+        return [(base.__origin__, base.__args__) for base in bases]
+
+    @staticmethod
+    def _modify_formula(formula: IngredientData) -> IngredientData:
+        formula.extra["__generic_type__"] = \
+            GenericChef._get_bases(formula._type)
+        if hasattr(formula._type, "__origin__"):
+            formula._type = formula._type.__origin__
+        return formula
+
+    def prepare(self,
+                ingredient: Ingredient) -> Ingredient:
+        if not self._is_generic(ingredient.formula._type):
+            return ingredient
+        ingredient.formula = self._modify_formula(ingredient.formula)
+        return ingredient
 
-pot = _Pot()
+    def cook(self,
+             line: IngredientProxy) -> IngredientProxy:
+        if self._is_generic(line.formula._type):
+            line.formula = self._modify_formula(line.formula)
+        return _GenericIngredientProxy(_f=line, formula=line.formula)
```

### Comparing `pypotage-0.1.2a0/src/pypotage/chefs/listChef.py` & `pypotage-0.2.0a0/src/pypotage/pot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,34 @@
-from .._chef import Chef
-from .._ingredient import IngredientProxy, _B, Ingredient
+from typing import Type
 
+from .ingredient import (
+    Ingredient,
+    IngredientData
+)
+from .utils import traverse_subclasses
 
-class _ListIngredientProxy(IngredientProxy):
 
-    def take_out(self, __ingredients: list[Ingredient] = None) -> list[_B]:
-        if __ingredients is None:
-            __ingredients = self(self.formula)
+class Pot:
 
-        return [ingredient() for ingredient in __ingredients]
+    ingredients: dict[Type, list[Ingredient]]
 
+    def __init__(self) -> None:
+        self.ingredients: dict[Type, list[Ingredient]] = {}
 
-class ListChef(Chef):
+    def add(self, ingredient: Ingredient) -> Ingredient:
+        _l = self.ingredients.setdefault(
+            (ingredient.formula._type, ingredient.formula._id), [])
+        _l.insert(0, ingredient)
+        return ingredient
 
-    def prepare(self, ingredient: Ingredient) -> Ingredient:
-        return super().prepare(ingredient)
+    def get(self, formula: IngredientData) -> Ingredient:
+        classes = [formula._type]
+        classes.extend(traverse_subclasses(formula._type))
 
-    def cook(self, line: IngredientProxy) -> IngredientProxy[_B]:
-        if not getattr(line.formula._type, "__origin__", None) == list:
-            return line
-        line.formula._type = line.formula._type.__args__[0]
-        return _ListIngredientProxy(_f=line, formula=line.formula)
+        ingredients = []
+
+        for _type in classes:
+            ingredient = self.ingredients.get((_type, formula._id))
+            if ingredient is not None:
+                ingredients.extend(ingredient)
+
+        return ingredients
```

### Comparing `pypotage-0.1.2a0/src/pypotage.egg-info/SOURCES.txt` & `pypotage-0.2.0a0/src/pypotage.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/pypotage/__init__.py
-src/pypotage/_chef.py
-src/pypotage/_ingredient.py
-src/pypotage/_pot.py
+src/pypotage/decorators.py
+src/pypotage/ingredient.py
+src/pypotage/kitchen.py
+src/pypotage/pot.py
 src/pypotage/shared.py
 src/pypotage/utils.py
 src/pypotage.egg-info/PKG-INFO
 src/pypotage.egg-info/SOURCES.txt
 src/pypotage.egg-info/dependency_links.txt
 src/pypotage.egg-info/top_level.txt
-src/pypotage/chefs/__init__.py
-src/pypotage/chefs/genericChef.py
-src/pypotage/chefs/listChef.py
+src/pypotage/chefsImpl/__init__.py
+src/pypotage/chefsImpl/genericChef.py
+src/pypotage/chefsImpl/listChef.py
 tests/test_abstract_ingredients.py
+tests/test_base.py
 tests/test_build.py
+tests/test_chef_line_ordered.py
+tests/test_decorable.py
+tests/test_decorators.py
 tests/test_genericchef.py
+tests/test_kitchen.py
 tests/test_listchef.py
+tests/test_multiple_inheritance.py
 tests/test_nocall.py
 tests/test_pot.py
-tests/test_preparechefline.py
+tests/test_preparechefline.py
+tests/test_priorized.py
```

### Comparing `pypotage-0.1.2a0/tests/test_abstract_ingredients.py` & `pypotage-0.2.0a0/tests/test_abstract_ingredients.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 from src import pypotage
 
 
 @pytest.fixture(autouse=True)
 def reset():
-    pypotage.pot.ingredients.clear()
+    pypotage.kitchen_.pot.ingredients.clear()
 
 
 def test_take_out_abstract():
     class test(metaclass=abc.ABCMeta):
         @classmethod
         @abc.abstractmethod
         def test(self): ...
```

### Comparing `pypotage-0.1.2a0/tests/test_genericchef.py` & `pypotage-0.2.0a0/tests/test_genericchef.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class TestGeneric(typing.Generic[T]):
     ...
 
 
 @pytest.fixture(autouse=True)
 def reset():
-    pypotage.pot.ingredients.clear()
+    pypotage.kitchen_.pot.ingredients.clear()
 
 
 def test_generic_chef():
     pypotage.prepare(TestGeneric[int])
 
     pytest.raises(RuntimeError, pypotage.cook(TestGeneric).take_out)
 
@@ -94,7 +94,21 @@
     class MultipleGeneric(typing.Generic[T, K]):
         ...
 
     pypotage.prepare(MultipleGeneric[int, str])
     assert isinstance(
         pypotage.cook(MultipleGeneric[int, str]).take_out(),
         MultipleGeneric)
+
+
+def test_generic_chef_solo():
+    kitchen_ = pypotage.Kitchen(
+        pypotage.Pot(),
+        [pypotage.chefs.GenericChef()]
+    )
+
+    @kitchen_.prepare
+    class Bean(TestGeneric[int]):
+        ...
+
+    assert isinstance(kitchen_.cook(TestGeneric[int]).take_out(), Bean)
+    assert isinstance(kitchen_.cook(Bean).take_out(), Bean)
```

### Comparing `pypotage-0.1.2a0/tests/test_nocall.py` & `pypotage-0.2.0a0/tests/test_nocall.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,52 +3,56 @@
 from typing import Callable
 
 from src import pypotage
 
 
 @pytest.fixture(autouse=True)
 def reset():
-    pypotage.pot.ingredients.clear()
+    pypotage.kitchen_.pot.ingredients.clear()
 
 
 def test_no_call_ingredient():
-    @pypotage.prepare(no_call=True)
+    @pypotage.prepare
+    @pypotage.no_call
     def test_ingredient() -> Callable:
         raise Exception("Should be raised on take_out")
 
     func = pypotage.cook(Callable).take_out()
     pytest.raises(Exception, func)
 
     def test_ingredient2():
         ...
 
     pytest.raises(
-        RuntimeError, pypotage.prepare, test_ingredient2, no_call=True)
+        RuntimeError, pypotage.prepare, pypotage.no_call(test_ingredient2))
 
 
 def test_no_call_class_ingredient():
-    @pypotage.prepare(no_call=True)
+    @pypotage.prepare
+    @pypotage.no_call
     class TestClass:
         def __init__(self) -> None:
             raise Exception("Should be raised on take_out")
 
     func = pypotage.cook(TestClass).take_out()
     pytest.raises(Exception, func)
 
 
 def test_no_call_lazy_ingredient():
-    @pypotage.prepare(
-        no_call=True, lazy=True)
+    @pypotage.prepare
+    @pypotage.no_call
+    @pypotage.lazy
     class TestClass:
         def __init__(self) -> None:
             raise Exception("Should be raised on take_out")
 
     func = pypotage.cook(TestClass).take_out()
     pytest.raises(Exception, func)
 
-    @pypotage.prepare(
-        no_call=True, lazy=True)
+    @pypotage.prepare
+    @pypotage.lazy
+    @pypotage.no_call
     def test_ingredient() -> Callable:
         raise Exception("Should be raised on take_out")
 
     func = pypotage.cook(Callable).take_out()
     pytest.raises(Exception, func)
```

### Comparing `pypotage-0.1.2a0/tests/test_pot.py` & `pypotage-0.2.0a0/tests/test_pot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from src import pypotage
 
 
 @pytest.fixture(autouse=True)
 def reset():
-    pypotage.pot.ingredients.clear()
+    pypotage.kitchen_.pot.ingredients.clear()
 
 
 def test_prepare_normal_take_out_cases():
     @pypotage.prepare
     def bean1() -> str:
         return "bean1"
 
@@ -37,35 +37,38 @@
 def test_prepare_ordered_take_out_cases():
     @pypotage.prepare
     def bean1() -> str:
         return "bean1"
 
     assert pypotage.cook(str).take_out() == "bean1"
 
-    @pypotage.prepare(order=1)
+    @pypotage.prepare
+    @pypotage.order(1)
     def bean2() -> str:
         return "bean2"
 
     assert pypotage.cook(str).take_out() == "bean2"
 
-    @pypotage.prepare(order=999)
+    @pypotage.prepare
+    @pypotage.order(999)
     def bean3() -> str:
         return "bean3"
 
     assert pypotage.cook(str).take_out() == "bean2"
 
 
 def test_prepare_primary_take_out_cases():
     @pypotage.prepare
     def bean1() -> str:
         return "bean1"
 
     assert pypotage.cook(str).take_out() == "bean1"
 
-    @pypotage.prepare(primary=True)
+    @pypotage.prepare
+    @pypotage.primary
     def bean2() -> str:
         return "bean2"
 
     assert pypotage.cook(str).take_out() == "bean2"
 
     @pypotage.prepare
     def bean3() -> str:
@@ -120,13 +123,27 @@
             raise Exception("Should be called on take_out() (On lazy beans)")
 
     def bean():
         return Bean()
 
     pytest.raises(Exception, pypotage.prepare, bean)
 
-    @pypotage.prepare(lazy=True)
+    @pypotage.prepare
+    @pypotage.lazy
     def bean() -> Bean:
         return Bean()
 
     assert pypotage.cook(Bean).is_present()
     pytest.raises(Exception, pypotage.cook(Bean).take_out)
+
+
+def test_cook_lazy_not_annot():
+    def bean():
+        return 1
+
+    pytest.raises(RuntimeError, pypotage.prepare, pypotage.lazy(bean))
+
+    @pypotage.prepare
+    @pypotage.lazy
+    class Bean:
+        def __init__(self):
+            raise Exception("Should be called on take_out() (On lazy beans)")
```

### Comparing `pypotage-0.1.2a0/tests/test_preparechefline.py` & `pypotage-0.2.0a0/tests/test_preparechefline.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import pytest
 
 from src import pypotage
 
 
-class TestChef(pypotage.Chef):
+class _TestChef(pypotage.Chef):
     def prepare(self, ingredient):
         ingredient.formula._id = "test"
         ingredient.formula._type = str
         return ingredient
 
     def cook(self, line):
         line.formula._type = str
         return line
 
 
 @pytest.fixture(autouse=True)
 def reset():
-    pypotage.pot.ingredients.clear()
+    pypotage.kitchen_.pot.ingredients.clear()
 
 
 def test_preparechefline_works():
     @pypotage.prepare
     def bean_1():
         return 1
 
     assert pypotage.cook(int).take_out() == 1
 
-    pypotage.pot.chefs.append(TestChef())
+    pypotage.kitchen_.chef_line.add(_TestChef())
 
     @pypotage.prepare
     def bean_2():
         return 1
 
     assert pypotage.cook(int, "test").take_out() == 1
```

