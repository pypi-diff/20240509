# Comparing `tmp/sommify-0.8.9.tar.gz` & `tmp/sommify-0.9.0.tar.gz`

## Comparing `sommify-0.8.9.tar` & `sommify-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.9/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/__init__.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/regex.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/test.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/utils.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/countries/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/__init__.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/categories.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/constants.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/cuisine.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/embeddings.py
--rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_funnel.py
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredients.py
--rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/mean_ing_embedding_per_tag.csv
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/meat.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/modifiers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/vegetables.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/vulgar_fractions.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/cheeses.py
--rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/drinks.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/fruit.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/herbs.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/legumes.py
--rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/meats.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/nuts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/pasta.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/spices.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/data/ingredient_categories/vegetables.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/prompts/__init__.py
--rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/prompts/data/__init__.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/prompts/data/default.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/pygrape/__init__.py
--rw-r--r--   0        0        0   367147 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/pygrape/data.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/pynotesandhints/__init__.py
--rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/pynotesandhints/data.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/pyregion/__init__.py
--rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/pyregion/data.py
--rw-r--r--   0        0        0    67688 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/recipes/__init__.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/recipes/elastic.py
--rw-r--r--   0        0        0    15890 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/recipes/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/test_elastic.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/test_prompts.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/test_pygrape.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/test_pyregion.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/test_recipe_reader.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.9/sommify/tests/test_tag_reader.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.9/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.9/README.md
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 sommify-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.9.0/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/__init__.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/regex.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/test.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/utils.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/countries/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/__init__.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/categories.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/constants.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/cuisine.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/embeddings.py
+-rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_funnel.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredients.py
+-rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/mean_ing_embedding_per_tag.csv
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/meat.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/modifiers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/vegetables.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/vulgar_fractions.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/cheeses.py
+-rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/drinks.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/fruit.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/herbs.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/legumes.py
+-rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/meats.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/nuts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/pasta.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/spices.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/data/ingredient_categories/vegetables.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/prompts/__init__.py
+-rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/prompts/data/__init__.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/prompts/data/default.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/pygrape/__init__.py
+-rw-r--r--   0        0        0   529134 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/pygrape/data.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/pynotesandhints/__init__.py
+-rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/pynotesandhints/data.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/pyregion/__init__.py
+-rw-r--r--   0        0        0   223164 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/pyregion/data.py
+-rw-r--r--   0        0        0    67688 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/recipes/__init__.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/recipes/elastic.py
+-rw-r--r--   0        0        0    15890 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/recipes/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/test_elastic.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/test_prompts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/test_pygrape.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/test_pyregion.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/test_recipe_reader.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.9.0/sommify/tests/test_tag_reader.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sommify-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.9.0/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.9.0/README.md
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 sommify-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.9.0/PKG-INFO
```

### Comparing `sommify-0.8.9/sommify/regex.py` & `sommify-0.9.0/sommify/regex.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/test.py` & `sommify-0.9.0/sommify/test.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/utils.py` & `sommify-0.9.0/sommify/utils.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/countries/__init__.py` & `sommify-0.9.0/sommify/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/categories.py` & `sommify-0.9.0/sommify/data/categories.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/constants.py` & `sommify-0.9.0/sommify/data/constants.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/cuisine.py` & `sommify-0.9.0/sommify/data/cuisine.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/embeddings.py` & `sommify-0.9.0/sommify/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_funnel.py` & `sommify-0.9.0/sommify/data/ingredient_funnel.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredients.py` & `sommify-0.9.0/sommify/data/ingredients.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/mean_ing_embedding_per_tag.csv` & `sommify-0.9.0/sommify/data/mean_ing_embedding_per_tag.csv`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/meat.py` & `sommify-0.9.0/sommify/data/meat.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/modifiers.py` & `sommify-0.9.0/sommify/data/modifiers.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/vegetables.py` & `sommify-0.9.0/sommify/data/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/__init__.py` & `sommify-0.9.0/sommify/data/ingredient_categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/drinks.py` & `sommify-0.9.0/sommify/data/ingredient_categories/drinks.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/fruit.py` & `sommify-0.9.0/sommify/data/ingredient_categories/fruit.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/herbs.py` & `sommify-0.9.0/sommify/data/ingredient_categories/herbs.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/meats.py` & `sommify-0.9.0/sommify/data/ingredient_categories/meats.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/nuts.py` & `sommify-0.9.0/sommify/data/ingredient_categories/nuts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/spices.py` & `sommify-0.9.0/sommify/data/ingredient_categories/spices.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/data/ingredient_categories/vegetables.py` & `sommify-0.9.0/sommify/data/ingredient_categories/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/prompts/__init__.py` & `sommify-0.9.0/sommify/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/prompts/data/__init__.py` & `sommify-0.9.0/sommify/prompts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/prompts/data/default.py` & `sommify-0.9.0/sommify/prompts/data/default.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/pygrape/__init__.py` & `sommify-0.9.0/sommify/pygrape/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 import json
+import re
+from collections import namedtuple
+
+from thefuzz import fuzz, process
 
 from .data import grapes as data
 
 grape_to_object = {}
-format_name = lambda name: name.lower().replace("i̇", "i").title()
+
+
+def format_name(name: str) -> str:
+    return name.lower().replace("i̇", "i").title()
+
 
 for o in data:
     name = format_name(o["name"])
     grape_to_object[name] = {**o, "name": name}
 
 # named tuple
-import re
-from collections import namedtuple
 
-from thefuzz import fuzz, process
 
 Grape = namedtuple("Grape", ["name", "synonyms", "description", "color", "numeric"])
 
 
 # create a generator of grapes
 class ExistingGrapes:
     __slots__ = ["grapes", "_synonym_to_name"]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.grapes = []
         self._synonym_to_name = {}
-        for name in grape_to_object.keys():
+        for name in grape_to_object:
             grape = Grape(
                 name=name,
-                synonyms=grape_to_object[name].get("synonyms", []),
-                description=grape_to_object[name].get("description", None),
-                color=grape_to_object[name].get("color", None),
+                synonyms=(
+                    grape_to_object[name]["synonyms"]
+                    if "synonyms" in grape_to_object[name]
+                    else []
+                ),
+                description=grape_to_object[name]["description"],
+                color=grape_to_object[name]["color"],
                 numeric=list(grape_to_object.keys()).index(name),
             )
             self.grapes.append(grape)
             self._synonym_to_name[name] = name
             for synonym in grape.synonyms:
                 if re.search(r"\d", synonym) or re.search(r"×", synonym):
                     continue
                 self._synonym_to_name[synonym] = name
 
-    def __iter__(self):
+    def __iter__(self) -> Grape:
         yield from self.grapes
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> Grape:
         return self.grapes[index]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.grapes)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"ExistingGrapes({len(self.grapes)})"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"ExistingGrapes({len(self.grapes)})"
 
     def get(self, **kwargs):
         for grape in self.grapes:
             if all(getattr(grape, k) == v for k, v in kwargs.items()):
                 return grape
 
-    def search_fuzzy(self, grape, threshold=82):
+    def search_fuzzy(self, grape: str, threshold: int = 82) -> Grape:
         name, distance = process.extractOne(
             grape, self._synonym_to_name.keys(), scorer=fuzz.QRatio
         )
         if distance > threshold:
             return self.get(name=self._synonym_to_name[name])
         else:
             return None
```

### Comparing `sommify-0.8.9/sommify/pygrape/data.py` & `sommify-0.9.0/sommify/pygrape/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,152 @@
 grapes = [
     {
         "name": "Abbuoto",
-        "synonyms": ["Aboto", "Cecubo"],
-        "description": "Rare, central Italian variety producing plenty of alcohol, generally blended.",
-        "color": "black",
+        "synonyms": [
+            "Aboto",
+            "Cecubo"
+        ],
+        "description": {
+            "default": "Rare, central Italian variety producing plenty of alcohol, generally blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Abouriou",
         "synonyms": [
             "Beaujolais",
             "Early Burgundy",
             "Gamay Beaujolais",
             "Gamay-Saint-Laurent",
             "Loubéjac",
             "Malbec Argenté",
             "Plant Abouriou",
             "Précoce Naugé",
             "Précoce Noir",
-            "Pressac de Bourgogne",
+            "Pressac de Bourgogne"
         ],
-        "description": "Declining, early-ripening south-west French variety making tannic red.",
-        "color": "black",
+        "description": {
+            "default": "Declining, early-ripening south-west French variety making tannic red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Abrusco",
         "synonyms": [
             "Abrostalo",
             "Abrostine",
             "Abrostino",
             "Abrusco Nero",
             "Abrusio",
             "Colore",
             "Colorino",
             "Lambrusco",
-            "Raverusto",
+            "Raverusto"
         ],
-        "description": "Obscure and endangered late-ripening Italian red adding colour to blends.",
-        "color": "black",
+        "description": {
+            "default": "Obscure and endangered late-ripening Italian red adding colour to blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Acitana",
-        "synonyms": ["Citana Nera"],
-        "description": "Rare dark-skinned variety from north-east Sicilia used in blends.",
-        "color": "black",
+        "synonyms": [
+            "Citana Nera"
+        ],
+        "description": {
+            "default": "Rare dark-skinned variety from north-east Sicilia used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Acolon",
-        "synonyms": ["Weinsberg 71-816-102"],
-        "description": "Recently authorized German cross favoured for its colour and early ripening.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg 71-816-102"
+        ],
+        "description": {
+            "default": "Recently authorized German cross favoured for its colour and early ripening.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Adakarasi",
-        "synonyms": ["Ada Karası"],
-        "description": "Vine grown mainly on the Turkish island of Avşa, making soft, dark reds.",
-        "color": "black",
+        "synonyms": [
+            "Ada Karası"
+        ],
+        "description": {
+            "default": "Vine grown mainly on the Turkish island of Avşa, making soft, dark reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Adalmiina",
-        "synonyms": ["Aldemina", "ES 6-16-30"],
-        "description": "Minor but complex, cold-hardy American hybrid grown mostly in Québec.",
-        "color": "white",
+        "synonyms": [
+            "Aldemina",
+            "ES 6-16-30"
+        ],
+        "description": {
+            "default": "Minor but complex, cold-hardy American hybrid grown mostly in Québec.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Addoraca",
-        "synonyms": ["Odoacra"],
-        "description": "Extremely rare Calabrian white that contributes to an equally rare dessert wine.",
-        "color": "white",
+        "synonyms": [
+            "Odoacra"
+        ],
+        "description": {
+            "default": "Extremely rare Calabrian white that contributes to an equally rare dessert wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Affenthaler",
         "synonyms": [
             "Blauer Affenthaler",
             "Kleiner Trollinger",
-            "Säuerlicher Burgunder",
+            "Säuerlicher Burgunder"
         ],
-        "description": "Very rare old variety from southern Germany.",
-        "color": "black",
+        "description": {
+            "default": "Very rare old variety from southern Germany.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Agiorgitiko",
         "synonyms": [
             "Aghiorghitiko",
             "Mavro Nemeas",
             "Mavrostaphylo Mavraki",
             "Mavroudi Nemeas",
-            "Nemeas Mavro",
+            "Nemeas Mavro"
         ],
-        "description": "Greece’s most widely planted dark-skinned variety, capable of both high volumes and high quality as well as a wide range of styles.",
-        "color": "black",
+        "description": {
+            "default": "Greece’s most widely planted dark-skinned variety, capable of both high volumes and high quality as well as a wide range of styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aglianico",
         "synonyms": [
             "Aglianco di Puglia",
             "Aglianica",
             "Aglianichella",
@@ -126,68 +180,103 @@
             "Olivella di S. Cosmo",
             "Ruopolo",
             "Spriema",
             "Tringarulo",
             "Uva Catellaneta",
             "Uva dei Cani",
             "Uva di Castellaneta",
-            "Uva Nera",
+            "Uva Nera"
         ],
-        "description": "High-quality, late-ripening, tannic and ageworthy southern Italian red.",
-        "color": "black",
+        "description": {
+            "default": "High-quality, late-ripening, tannic and ageworthy southern Italian red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Agni",
-        "synonyms": ["PE-11/47"],
-        "description": "Recent Czech cross producing unusually aromatic reds.",
-        "color": "black",
+        "synonyms": [
+            "PE-11/47"
+        ],
+        "description": {
+            "default": "Recent Czech cross producing unusually aromatic reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aïdani",
         "synonyms": [
             "Adani",
             "Aedano Leyko",
             "Aïdani Aspro",
             "Aïdani Blanc",
             "Aïdani Lefko",
             "Aspaedano",
             "Aspraïdano",
-            "Moschaïdano",
+            "Moschaïdano"
         ],
-        "description": "Minor, aromatic Greek variety that plays a small but significant role in the wines of Santoríni.",
-        "color": "white",
+        "description": {
+            "default": "Minor, aromatic Greek variety that plays a small but significant role in the wines of Santoríni.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Airén",
         "synonyms": [
             "Aidén",
             "Blancón",
             "Burra Blanca",
             "Colgadera",
             "Forcallada",
             "Forcallat",
             "Forcallat Blanca",
             "Manchega",
             "Valdepeñera Blanca",
-            "Valdepeñas",
+            "Valdepeñas"
         ],
-        "description": "Spain’s most widely planted light-skinned variety making brandy and rather neutral, fresh white wines.",
-        "color": "white",
+        "description": {
+            "default": "Spain’s most widely planted light-skinned variety making brandy and rather neutral, fresh white wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Akhtanak",
-        "synonyms": ["2-18-23", "Akchtanak", "Haghtanak", "Hakhtanak"],
-        "description": "Versatile, late-ripening Armenian complex cross.",
-        "color": "black",
+        "synonyms": [
+            "2-18-23",
+            "Akchtanak",
+            "Haghtanak",
+            "Hakhtanak"
+        ],
+        "description": {
+            "default": "Versatile, late-ripening Armenian complex cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aladasturi",
-        "synonyms": ["Aladastouri", "Anadassaouli", "Anadastouri"],
-        "description": "Minor Georgian variety responsible for alcoholic reds.",
-        "color": "black",
+        "synonyms": [
+            "Aladastouri",
+            "Anadassaouli",
+            "Anadastouri"
+        ],
+        "description": {
+            "default": "Minor Georgian variety responsible for alcoholic reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Alarije",
         "synonyms": [
             "Acería",
             "Alarije Dorada",
             "Alarije Dorado",
@@ -201,121 +290,209 @@
             "Esclafacherri",
             "Malfar",
             "Malvasía",
             "Malvasía Riojana",
             "Pirulés Dorada  and Pirulés Verde",
             "Rojal",
             "Subirat",
-            "Subirat Parent",
+            "Subirat Parent"
         ],
-        "description": "Light-skinned variety from south-west Spain travelling under many aliases.",
-        "color": "white",
+        "description": {
+            "default": "Light-skinned variety from south-west Spain travelling under many aliases.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albalonga",
-        "synonyms": ["Würzburg B 51-2-1"],
-        "description": "Fresh and aromatically complex German cross planted and valued mainly in Rheinhessen.",
-        "color": "white",
+        "synonyms": [
+            "Würzburg B 51-2-1"
+        ],
+        "description": {
+            "default": "Fresh and aromatically complex German cross planted and valued mainly in Rheinhessen.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albana",
         "synonyms": [
             "Albana a Grappolo Fitto",
             "Albana a Grappolo Lungo",
             "Albana della Forcella",
             "Albana di Romagna",
             "Albana Gentile",
             "Albana Grossa",
             "Albanone",
             "Ribona",
             "Riminèse",
-            "Sforcella",
+            "Sforcella"
         ],
-        "description": "Ancient but inherently neutral Italian variety that can produce very good sweet wines.",
-        "color": "white",
+        "description": {
+            "default": "Ancient but inherently neutral Italian variety that can produce very good sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albanello",
-        "synonyms": ["Albanello di Siracusa"],
-        "description": "Disappearing Sicilian variety once used for sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Albanello di Siracusa"
+        ],
+        "description": {
+            "default": "Disappearing Sicilian variety once used for sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albaranzeuli Bianco",
-        "synonyms": ["Laconari", "Lacconargiu", "Lacconarzu"],
-        "description": "Virtually extinct white grape from Sardegna.",
-        "color": "white",
+        "synonyms": [
+            "Laconari",
+            "Lacconargiu",
+            "Lacconarzu"
+        ],
+        "description": {
+            "default": "Virtually extinct white grape from Sardegna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albaranzeuli Nero",
-        "synonyms": ["Albarenzelin Nero", "Uva Melone"],
-        "description": "A pinky-red-skinned Sardinian variety still very occasionally used in blends.",
-        "color": "red",
+        "synonyms": [
+            "Albarenzelin Nero",
+            "Uva Melone"
+        ],
+        "description": {
+            "default": "A pinky-red-skinned Sardinian variety still very occasionally used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Albarín Blanco",
         "synonyms": [
             "Blanco Legítimo",
             "Blanco País",
             "Blanco Verdín",
             "Branco Lexítimo",
             "Raposo",
-            "Tinta Fina",
+            "Tinta Fina"
         ],
-        "description": "Very minor variety from the far north of Spain.",
-        "color": "white",
+        "description": {
+            "default": "Very minor variety from the far north of Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albarola",
-        "synonyms": ["Bianchetta Genovese", "Calcatella"],
-        "description": "Neutral white grape of Liguria.",
-        "color": "white",
+        "synonyms": [
+            "Bianchetta Genovese",
+            "Calcatella"
+        ],
+        "description": {
+            "default": "Neutral white grape of Liguria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albarossa",
-        "synonyms": ["Incrocio Dalmasso XV/31"],
-        "description": "Minor Piemontese dark-skinned cross recently replanted by Michele Chiarlo.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso XV/31"
+        ],
+        "description": {
+            "default": "Minor Piemontese dark-skinned cross recently replanted by Michele Chiarlo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Albillo Mayor",
-        "synonyms": ["Albilla", "Pardina", "Turruntes", "Turruntés"],
-        "description": "Ribera del Duero variety used mostly in blends and now partly disentangled from the Albillo confusion.",
-        "color": "white",
+        "synonyms": [
+            "Albilla",
+            "Pardina",
+            "Turruntes",
+            "Turruntés"
+        ],
+        "description": {
+            "default": "Ribera del Duero variety used mostly in blends and now partly disentangled from the Albillo confusion.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Albillo Real",
-        "synonyms": ["Albillo", "Albillo de Cebreros", "Albillo de Madrid"],
-        "description": "Aromatic Spanish variety producing smooth wines that are used mostly in blends, both red and white.",
-        "color": "white",
+        "synonyms": [
+            "Albillo",
+            "Albillo de Cebreros",
+            "Albillo de Madrid"
+        ],
+        "description": {
+            "default": "Aromatic Spanish variety producing smooth wines that are used mostly in blends, both red and white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Alcañón",
-        "synonyms": ["Blanco Castellano", "Bobal Blanca"],
-        "description": "Rare variety producing light but characterful whites in Somontano.",
-        "color": "white",
+        "synonyms": [
+            "Blanco Castellano",
+            "Bobal Blanca"
+        ],
+        "description": {
+            "default": "Rare variety producing light but characterful whites in Somontano.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Aleatico",
         "synonyms": [
             "Aleaticu",
             "Halápi",
             "Moscatello Nero",
             "Moscato Nero",
             "Vernaccia di Pergola",
-            "Vernaccia Moscatella",
+            "Vernaccia Moscatella"
         ],
-        "description": "Unusually perfumed and Muscat-like Italian red.",
-        "color": "black",
+        "description": {
+            "default": "Unusually perfumed and Muscat-like Italian red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aleksandrouli",
-        "synonyms": ["Aleksandroouly", "Aleksandrouli Shavi", "Alexandrouli"],
-        "description": "Rare but highly promising Georgian variety often late harvested for violet-scented semi-sweet wines.",
-        "color": "black",
+        "synonyms": [
+            "Aleksandroouly",
+            "Aleksandrouli Shavi",
+            "Alexandrouli"
+        ],
+        "description": {
+            "default": "Rare but highly promising Georgian variety often late harvested for violet-scented semi-sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Alexander",
         "synonyms": [
             "Alexandria",
             "Black Cape",
             "Buck Grape",
@@ -332,50 +509,62 @@
             "Schuylkill Muscadel",
             "Schuylkill Muscadine",
             "Springmill Constantia",
             "Tasker’s Grape",
             "Vevay",
             "Vevay Winne",
             "Winne",
-            "York Lisbon",
+            "York Lisbon"
         ],
-        "description": "American hybrid of purely historical significance in the US.",
-        "color": "black",
+        "description": {
+            "default": "American hybrid of purely historical significance in the US.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Alfrocheiro",
         "synonyms": [
             "Albarín Negro",
             "Albarín Tinto",
             "Alfrocheiro Preto",
             "Alfrucheiro",
             "Baboso Negro",
             "Bastardo Negro",
             "Bruñal",
             "Caiño Gordo",
             "Tinta Bastardinha",
-            "Tinta Francesa de Viseu",
+            "Tinta Francesa de Viseu"
         ],
-        "description": "Portuguese variety with intense fruit aromas and high quality potential.",
-        "color": "black",
+        "description": {
+            "default": "Portuguese variety with intense fruit aromas and high quality potential.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Alicante Henri Bouschet",
         "synonyms": [
             "Alicante",
             "Alicante Bouschet",
             "Alicante Bouschet no. 2",
             "Dalmatinka",
             "Garnacha Tintorera",
             "Kambuša",
             "Sumo Tinto",
-            "Tintorera",
+            "Tintorera"
         ],
-        "description": "Productive, widely dispersed, red-fleshed southern French cross on the wane in France but waxing in southern Portugal.",
-        "color": "black",
+        "description": {
+            "default": "Productive, widely dispersed, red-fleshed southern French cross on the wane in France but waxing in southern Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aligoté",
         "synonyms": [
             "Aligotte",
             "Alligotay",
             "Alligoté",
@@ -387,54 +576,72 @@
             "Giboulot",
             "Giboudot",
             "Griset Blanc",
             "Mahranauli",
             "Plant de Trois",
             "Plant Gris",
             "Troyen Blanc",
-            "Vert Blanc",
+            "Vert Blanc"
         ],
-        "description": "Burgundy’s tart ‘other’ white wine grape, particularly popular in Eastern Europe.",
-        "color": "white",
+        "description": {
+            "default": "Burgundy’s tart ‘other’ white wine grape, particularly popular in Eastern Europe.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Alionza",
         "synonyms": [
             "Aleonza",
             "Alionga Bianca del Bolognese",
             "Allionza",
             "Glionza",
             "Leonza",
             "Uva Lonza",
-            "Uva Schiava",
+            "Uva Schiava"
         ],
-        "description": "Rare but ancient white on the verge of extinction.",
-        "color": "white",
+        "description": {
+            "default": "Rare but ancient white on the verge of extinction.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Allegro",
-        "synonyms": ["Geisenheim 8331-1"],
-        "description": "German hybrid with good disease resistance.",
-        "color": "black",
+        "synonyms": [
+            "Geisenheim 8331-1"
+        ],
+        "description": {
+            "default": "German hybrid with good disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Altesse",
         "synonyms": [
             "Anet",
             "Fusette d’Ambérieu",
             "Marestel",
             "Plant d’Altesse",
             "Prin Blanc",
             "Roussette",
             "Roussette de Montagnieu",
             "Roussette de Seyssel",
-            "Roussette Haute",
+            "Roussette Haute"
         ],
-        "description": "Savoie’s finest grape making delicate whites.",
-        "color": "white",
+        "description": {
+            "default": "Savoie’s finest grape making delicate whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Alvarelhão",
         "synonyms": [
             "Albarello",
             "Alvarelhao",
             "Alvarelho",
@@ -445,382 +652,610 @@
             "Locaia",
             "Pilongo",
             "Pirruivo",
             "Serradelo",
             "Serradillo",
             "Uva Gallega",
             "Varancelha",
-            "Verancelha",
+            "Verancelha"
         ],
-        "description": "Declining but potentially high-quality variety from northern Portugal.",
-        "color": "black",
+        "description": {
+            "default": "Declining but potentially high-quality variety from northern Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Alvarinho",
         "synonyms": [
             "Albariño",
             "Albelleiro",
             "Alvarin Blanco",
             "Azal Blanco",
             "Galego",
             "Galeguinho",
-            "Padernã",
+            "Padernã"
         ],
-        "description": "Fashionable, high-quality, fresh, aromatic variety straddling the Spanish–Portuguese border.",
-        "color": "white",
+        "description": {
+            "default": "Fashionable, high-quality, fresh, aromatic variety straddling the Spanish–Portuguese border.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Amaral",
         "synonyms": [
             "Azal Tinto",
             "Azar",
             "Cainho Bravo",
             "Cainho Miúdo",
             "Caíño Bravo",
-            "Cainzinho",
+            "Cainzinho"
         ],
-        "description": "High-acid Portuguese red found mainly in Vinho Verde.",
-        "color": "black",
+        "description": {
+            "default": "High-acid Portuguese red found mainly in Vinho Verde.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Amigne",
         "synonyms": [
             "Amigne Blanche",
             "Grande Amigne",
             "Grosse Amigne",
-            "Petite Amigne",
+            "Petite Amigne"
         ],
-        "description": "Ancient but minor Swiss variety making mainly sweeter styles of wine.",
-        "color": "white",
+        "description": {
+            "default": "Ancient but minor Swiss variety making mainly sweeter styles of wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ancellotta",
-        "synonyms": ["Ancellotta di Massenzatico", "Lancellotta"],
-        "description": "Useful, deeply coloured blending ingredient valued more for its colour, tannins and acidity than for its flavour.",
-        "color": "black",
+        "synonyms": [
+            "Ancellotta di Massenzatico",
+            "Lancellotta"
+        ],
+        "description": {
+            "default": "Useful, deeply coloured blending ingredient valued more for its colour, tannins and acidity than for its flavour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "André",
-        "synonyms": ["Andrea", "Semenac A 16-76"],
-        "description": "Late-ripening Czech cross producing well-structured reds if harvested fully ripe.",
-        "color": "black",
+        "synonyms": [
+            "Andrea",
+            "Semenac A 16-76"
+        ],
+        "description": {
+            "default": "Late-ripening Czech cross producing well-structured reds if harvested fully ripe.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Antão Vaz",
-        "synonyms": ["Antonio Vaz"],
-        "description": "High-quality Portuguese variety at home in the hot, dry south.",
-        "color": "white",
+        "synonyms": [
+            "Antonio Vaz"
+        ],
+        "description": {
+            "default": "High-quality Portuguese variety at home in the hot, dry south.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Antey Magarachsky",
-        "synonyms": ["Antei", "Antei Magarachskii", "Magarach 70-71-52"],
-        "description": "Ukrainian hybrid used to make sweet red wines.",
-        "color": "black",
+        "synonyms": [
+            "Antei",
+            "Antei Magarachskii",
+            "Magarach 70-71-52"
+        ],
+        "description": {
+            "default": "Ukrainian hybrid used to make sweet red wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Araklinos",
-        "synonyms": ["Araclinos", "Araklino", "Raklino"],
-        "description": "Rare Greek variety used mainly in red blends.",
-        "color": "black",
+        "synonyms": [
+            "Araclinos",
+            "Araklino",
+            "Raklino"
+        ],
+        "description": {
+            "default": "Rare Greek variety used mainly in red blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aramon Noir",
         "synonyms": [
             "Amor-Não-Me-Deixes",
             "Aramonen",
             "Gros Bouteillan",
             "Pisse-Vin",
             "Plant Riche",
             "Rabalaïré",
             "Ramonen",
             "Réballaïré",
-            "Ugni Noir",
+            "Ugni Noir"
         ],
-        "description": "Very productive vine once responsible for much of France’s least noble wine.",
-        "color": "black",
+        "description": {
+            "default": "Very productive vine once responsible for much of France’s least noble wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Arany Sárfehér",
         "synonyms": [
             "Fehér Kadarka",
             "Fehér Muskotály",
             "Huszár Szőlő",
             "Izsáki",
             "Izsáki Fehér",
             "Izsáki Sárfehér",
             "Német Dinka",
-            "Vékonyhéjú",
+            "Vékonyhéjú"
         ],
-        "description": "Hungarian variety making simple but useful, high-acid wines and fizz on the Alföld (Great Plain).",
-        "color": "white",
+        "description": {
+            "default": "Hungarian variety making simple but useful, high-acid wines and fizz on the Alföld (Great Plain).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arbane",
         "synonyms": [
             "Albane",
             "Arbanne",
             "Arbenne",
             "Arbone",
             "Crène",
             "Crénillat",
-            "Darbanne",
+            "Darbanne"
         ],
-        "description": "Old, aromatic but virtually extinct variety from southern Champagne.",
-        "color": "white",
+        "description": {
+            "default": "Old, aromatic but virtually extinct variety from southern Champagne.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Areni",
         "synonyms": [
             "Areni Chernyi",
             "Areni Noir",
             "Areny",
             "Areny Tcherny",
             "Malai Sev",
             "Malayi",
             "Sev Areni",
-            "Urza Sev",
+            "Urza Sev"
         ],
-        "description": "Armenia’s signature variety making top-quality dry and sweet reds.",
-        "color": "black",
+        "description": {
+            "default": "Armenia’s signature variety making top-quality dry and sweet reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Arilla",
-        "synonyms": ["Agrilla", "Arillo", "Rille", "Uva Rilla"],
-        "description": "Rare but productive island white from southern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Agrilla",
+            "Arillo",
+            "Rille",
+            "Uva Rilla"
+        ],
+        "description": {
+            "default": "Rare but productive island white from southern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arinto De Bucelas",
         "synonyms": [
             "Arinto",
             "Arinto Branco",
             "Arinto Cercial",
             "Arinto d’Anadia",
             "Arinto Galego",
             "Arintho",
             "Azal Espanhol",
             "Chapeludo",
             "Pedernã",
-            "Terrantez da Terceira",
+            "Terrantez da Terceira"
         ],
-        "description": "High-quality, high-acid, adaptable Portuguese variety from just north of Lisboa.",
-        "color": "white",
+        "description": {
+            "default": "High-quality, high-acid, adaptable Portuguese variety from just north of Lisboa.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arna-Grna",
-        "synonyms": ["Alagura", "Arha-Grna", "Khana Crna"],
-        "description": "Light-skinned Azeri variety found mainly in the Nakhchivan Autonomous Republic.",
-        "color": "white",
+        "synonyms": [
+            "Alagura",
+            "Arha-Grna",
+            "Khana Crna"
+        ],
+        "description": {
+            "default": "Light-skinned Azeri variety found mainly in the Nakhchivan Autonomous Republic.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arneis",
-        "synonyms": ["Bianchetta di Alba", "Bianchetto", "Nebbiolo Bianco"],
-        "description": "Piemonte’s scented and full-bodied signature dry white.",
-        "color": "white",
+        "synonyms": [
+            "Bianchetta di Alba",
+            "Bianchetto",
+            "Nebbiolo Bianco"
+        ],
+        "description": {
+            "default": "Piemonte’s scented and full-bodied signature dry white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arnsburger",
-        "synonyms": ["Geisenheim 22-74"],
-        "description": "Scarce German cross used to make base wines for inexpensive fizz.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 22-74"
+        ],
+        "description": {
+            "default": "Scarce German cross used to make base wines for inexpensive fizz.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arrouya",
-        "synonyms": ["Dourec Noir", "Eremachaoua", "Erematxahua"],
-        "description": "Virtually extinct old Jurançon vine.",
-        "color": "black",
+        "synonyms": [
+            "Dourec Noir",
+            "Eremachaoua",
+            "Erematxahua"
+        ],
+        "description": {
+            "default": "Virtually extinct old Jurançon vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Arrufiac",
         "synonyms": [
             "Arrefiat",
             "Arruffiac",
             "Arruffiat",
             "Arrufiat",
             "Bouisselet",
             "Raffiac",
             "Raffiat",
             "Réfiat",
             "Rufiat",
-            "Zurizerratia",
+            "Zurizerratia"
         ],
-        "description": "South-west France relic starting to regain a little local respect.",
-        "color": "white",
+        "description": {
+            "default": "South-west France relic starting to regain a little local respect.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arvesiniadu",
         "synonyms": [
             "Argu Ingianau",
             "Arvesimiadu Bianco",
             "Arvu Siniadu",
-            "Uva Oschirese",
+            "Uva Oschirese"
         ],
-        "description": "Rare Sardinian white that disappears into blends.",
-        "color": "white",
+        "description": {
+            "default": "Rare Sardinian white that disappears into blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Arvine",
-        "synonyms": ["Arvena", "Arvina", "Petite Arvine"],
-        "description": "The finest indigenous Valais variety making lively, sometimes intense, whites both dry and sweet.",
-        "color": "white",
+        "synonyms": [
+            "Arvena",
+            "Arvina",
+            "Petite Arvine"
+        ],
+        "description": {
+            "default": "The finest indigenous Valais variety making lively, sometimes intense, whites both dry and sweet.",
+            "julie": "",
+            "sommelier": "Arvine produces complex, nervous wines with aromas of citrus fruits, wisteria and rhubarb, with a voluptuous structure and a characteristic salinity on the finish. Traditional swiss pairings : Sweetbread, Crustaceans (langoustines, lobster), Cheese (fondue, raclette, cheese platter)"
+        },
+        "color": "white"
     },
     {
         "name": "Ashughaji",
-        "synonyms": ["Achougage", "Ashugazh"],
-        "description": "Minor Georgian variety producing fresh, aromatic reds.",
-        "color": "black",
+        "synonyms": [
+            "Achougage",
+            "Ashugazh"
+        ],
+        "description": {
+            "default": "Minor Georgian variety producing fresh, aromatic reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aspiran Bouschet",
-        "synonyms": ["Grand Noir de Laques"],
-        "description": "Deeply coloured but almost extinct.",
-        "color": "black",
+        "synonyms": [
+            "Grand Noir de Laques"
+        ],
+        "description": {
+            "default": "Deeply coloured but almost extinct.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Assyrtiko",
-        "synonyms": ["Assirtico", "Assyrtico", "Asyrtico", "Asyrtiko"],
-        "description": "Top-quality, intense, highly structured Greek island white that retains acidity even in the heat.",
-        "color": "white",
+        "synonyms": [
+            "Assirtico",
+            "Assyrtico",
+            "Asyrtico",
+            "Asyrtiko"
+        ],
+        "description": {
+            "default": "Top-quality, intense, highly structured Greek island white that retains acidity even in the heat.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Asuretuli Shavi",
-        "synonyms": ["Asuretuli", "Schalltraube", "Shadi Traube", "Shala"],
-        "description": "Minor Georgian variety once popular with German colonists.",
-        "color": "black",
+        "synonyms": [
+            "Asuretuli",
+            "Schalltraube",
+            "Shadi Traube",
+            "Shala"
+        ],
+        "description": {
+            "default": "Minor Georgian variety once popular with German colonists.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Athiri",
         "synonyms": [
             "Asprathiri",
             "Asprathiro",
             "Athiri Aspro",
             "Athiri Lefko",
-            "Athiri Leyko",
+            "Athiri Leyko"
         ],
-        "description": "An old, easy-to-grow Greek variety producing soft, dry, fruity whites.",
-        "color": "white",
+        "description": {
+            "default": "An old, easy-to-grow Greek variety producing soft, dry, fruity whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Aubin Blanc",
         "synonyms": [
             "Albin Blanc",
             "Aubain",
             "Aubier",
             "Aubin",
             "Blanc de Creuë",
             "Blanc de Magny",
-            "Gros Vert de Crenay",
+            "Gros Vert de Crenay"
         ],
-        "description": "Virtually extinct Lorraine speciality.",
-        "color": "white",
+        "description": {
+            "default": "Virtually extinct Lorraine speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Aubin Vert",
-        "synonyms": ["Blanc d’Euvézin", "Vert Blanc"],
-        "description": "Virtually extinct Lorraine variety.",
-        "color": "white",
+        "synonyms": [
+            "Blanc d’Euvézin",
+            "Vert Blanc"
+        ],
+        "description": {
+            "default": "Virtually extinct Lorraine variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Aubun",
         "synonyms": [
             "Carignan de Bédoin",
             "Carignan de Gigondas",
             "Grosse Rogettaz",
             "Morescola",
             "Murescola",
             "Moustardier",
-            "Moutardier",
+            "Moutardier"
         ],
-        "description": "Minor blending component from the southern Rhône.",
-        "color": "black",
+        "description": {
+            "default": "Minor blending component from the southern Rhône.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Aurore",
-        "synonyms": ["Aurora", "Feri Szölö", "Financ Szölö", "Redei", "Seibel 5279"],
-        "description": "Complex hybrid more successful in North America than in its homeland France.",
-        "color": "grey",
+        "synonyms": [
+            "Aurora",
+            "Feri Szölö",
+            "Financ Szölö",
+            "Redei",
+            "Seibel 5279"
+        ],
+        "description": {
+            "default": "Complex hybrid more successful in North America than in its homeland France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey"
     },
     {
         "name": "Auxerrois",
         "synonyms": [
             "Aucerot",
             "Auxera",
             "Auxerrois de Laquenexy",
             "Auxois",
             "Auzerrois Blanc",
             "Blanc de Kienzheim",
             "Ericey de la Montée",
             "Kleiner Heunisch",
             "Okseroa",
             "Pinot Auxerrois",
-            "Riesling Jaune de la Moselle",
+            "Riesling Jaune de la Moselle"
         ],
-        "description": "Low-acid variety useful in cool climates.",
-        "color": "white",
+        "description": {
+            "default": "Low-acid variety useful in cool climates.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Avanà",
         "synonyms": [
             "Avenà",
             "Avenai",
             "Avanale",
             "Avanas",
             "Avanato",
             "Avanè",
             "Hibou Noir",
-            "Vermaglio",
+            "Vermaglio"
         ],
-        "description": "Light, early-drinking Piemontese red, rarely made as a varietal.",
-        "color": "black",
+        "description": {
+            "default": "Light, early-drinking Piemontese red, rarely made as a varietal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Avarengo",
         "synonyms": [
             "Amarene",
             "Avarenc",
             "Avarena",
             "Mustèr",
             "Riondosca",
-            "Riundasca",
+            "Riundasca"
         ],
-        "description": "Low-yielding, perfumed Piemontese red.",
-        "color": "black",
+        "description": {
+            "default": "Low-yielding, perfumed Piemontese red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Avasirkhva",
-        "synonyms": ["Ajiche", "Ajishi", "Auasirkhva", "Avasarkhva", "Avassirkhva"],
-        "description": "Rare Georgian variety grown in Apkhazeti.",
-        "color": "white",
+        "synonyms": [
+            "Ajiche",
+            "Ajishi",
+            "Auasirkhva",
+            "Avasarkhva",
+            "Avassirkhva"
+        ],
+        "description": {
+            "default": "Rare Georgian variety grown in Apkhazeti.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Avesso",
-        "synonyms": ["Bornal", "Bornão", "Borral"],
-        "description": "Portuguese variety with more body than others making Vinho Verde.",
-        "color": "white",
+        "synonyms": [
+            "Bornal",
+            "Bornão",
+            "Borral"
+        ],
+        "description": {
+            "default": "Portuguese variety with more body than others making Vinho Verde.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Avgoustiatis",
-        "synonyms": ["Avgoustella", "Agoustiates"],
-        "description": "Minor Greek variety found mainly on the island of Zákynthos and in the western Pelopónnisos (Peloponnese).",
-        "color": "black",
+        "synonyms": [
+            "Avgoustella",
+            "Agoustiates"
+        ],
+        "description": {
+            "default": "Minor Greek variety found mainly on the island of Zákynthos and in the western Pelopónnisos (Peloponnese).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Azal",
         "synonyms": [
             "Asal",
             "Azal Branco",
             "Asal da Lixa",
             "Azal da Lixa",
             "Carvalha",
             "Carvalhal",
             "Gadelhudo",
-            "Pinheira",
+            "Pinheira"
         ],
-        "description": "High-acid variety losing ground but still widespread in northern Portugal.",
-        "color": "white",
+        "description": {
+            "default": "High-acid variety losing ground but still widespread in northern Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Băbească Neagră",
         "synonyms": [
             "Asîl Kara",
             "Băbească",
             "Căldăruşă",
@@ -830,107 +1265,184 @@
             "Poama Rară Neagră",
             "Rarăneagră",
             "Rară Neagră",
             "Răşchirată",
             "Rastriopa",
             "Serecsia Ciornaia",
             "Sereksia",
-            "Sereksiya",
+            "Sereksiya"
         ],
-        "description": "High-acid Romanian variety producing fairy light reds.",
-        "color": "black",
+        "description": {
+            "default": "High-acid Romanian variety producing fairy light reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Babić",
-        "synonyms": ["Babić Crni", "Rogoznička"],
-        "description": "Lively and potentially high-quality Croatian variety well suited to barrel ageing.",
-        "color": "black",
+        "synonyms": [
+            "Babić Crni",
+            "Rogoznička"
+        ],
+        "description": {
+            "default": "Lively and potentially high-quality Croatian variety well suited to barrel ageing.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Babica",
-        "synonyms": ["Kaštelanka"],
-        "description": "Rare variety from Croatia’s Adriatic coast.",
-        "color": "black",
+        "synonyms": [
+            "Kaštelanka"
+        ],
+        "description": {
+            "default": "Rare variety from Croatia’s Adriatic coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bacchus",
-        "synonyms": ["Bacchus Weiss", "Geilweilerhof 33-29-133"],
-        "description": "One of the most important German crosses producing highly aromatic whites, not least in England.",
-        "color": "white",
+        "synonyms": [
+            "Bacchus Weiss",
+            "Geilweilerhof 33-29-133"
+        ],
+        "description": {
+            "default": "One of the most important German crosses producing highly aromatic whites, not least in England.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bachet Noir",
-        "synonyms": ["Bachey", "François Noir", "Gris Bachet"],
-        "description": "Ancient and almost extinct.",
-        "color": "black",
+        "synonyms": [
+            "Bachey",
+            "François Noir",
+            "Gris Bachet"
+        ],
+        "description": {
+            "default": "Ancient and almost extinct.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Baco Blanc",
-        "synonyms": ["Baco 22 A", "Maurice Baco", "Piquepoul du Gers"],
-        "description": "Light-skinned French hybrid still allowed in Armagnac but declining.",
-        "color": "white",
+        "synonyms": [
+            "Baco 22 A",
+            "Maurice Baco",
+            "Piquepoul du Gers"
+        ],
+        "description": {
+            "default": "Light-skinned French hybrid still allowed in Armagnac but declining.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Baco Noir",
-        "synonyms": ["Baco 1", "Baco 24-23", "Bacoi", "Bago", "Bako Speiskii", "Bakon"],
-        "description": "Dark-skinned French hybrid faring better across the Atlantic than at home.",
-        "color": "black",
+        "synonyms": [
+            "Baco 1",
+            "Baco 24-23",
+            "Bacoi",
+            "Bago",
+            "Bako Speiskii",
+            "Bakon"
+        ],
+        "description": {
+            "default": "Dark-skinned French hybrid faring better across the Atlantic than at home.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Baga",
         "synonyms": [
             "Baga de Louro",
             "Carrasquenho",
             "Carrego Burros",
             "Poeirinho",
             "Tinta Bairrada",
             "Tinta da Bairrada",
-            "Tinta de Baga",
+            "Tinta de Baga"
         ],
-        "description": "Controversial, demanding northern Portuguese variety capable of making great, ageworthy wines.",
-        "color": "black",
+        "description": {
+            "default": "Controversial, demanding northern Portuguese variety capable of making great, ageworthy wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bagrina",
         "synonyms": [
             "Bagrina Crvena",
             "Bagrina Krajinska",
             "Bagrina Rošie",
             "Braghina",
             "Braghină",
             "Braghină de Drăgășani",
             "Bragina",
-            "Bragina Rara",
+            "Bragina Rara"
         ],
-        "description": "Pink-skinned Balkan variety making fresh and ageworthy whites.",
-        "color": "pink",
+        "description": {
+            "default": "Pink-skinned Balkan variety making fresh and ageworthy whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Balzac Blanc",
         "synonyms": [
             "Balzard Blanc",
             "Balzat",
             "Blanc Limousin",
             "Margnac Blanc",
-            "Ressière",
+            "Ressière"
         ],
-        "description": "Almost extinct variety from Cognac country.",
-        "color": "white",
+        "description": {
+            "default": "Almost extinct variety from Cognac country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Baratuciat",
-        "synonyms": ["Bertacuciàt"],
-        "description": "Rare but recovered Piemontese white that tastes a bit like Sauvignon Blanc.",
-        "color": "white",
+        "synonyms": [
+            "Bertacuciàt"
+        ],
+        "description": {
+            "default": "Rare but recovered Piemontese white that tastes a bit like Sauvignon Blanc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Barbaroux",
-        "synonyms": ["Barbarons", "Grec Rose", "Roussée"],
-        "description": "Almost extinct, relatively undistinguished pink-skinned Provençal variety.",
-        "color": "pink",
+        "synonyms": [
+            "Barbarons",
+            "Grec Rose",
+            "Roussée"
+        ],
+        "description": {
+            "default": "Almost extinct, relatively undistinguished pink-skinned Provençal variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Barbera",
         "synonyms": [
             "Barbera a Peduncolo Rosso",
             "Barbera a Raspo Verde",
             "Barbera Amaro",
@@ -940,143 +1452,204 @@
             "Barbera Grossa",
             "Barbera Nera",
             "Barbera Nostrana",
             "Barbera Vera",
             "Barberone",
             "Gaietto",
             "Lombardesca",
-            "Sciaa",
+            "Sciaa"
         ],
-        "description": "With origins still unknown, this versatile variety makes crisp, sweet Italian reds in a wide range of styles and locations.",
-        "color": "black",
+        "description": {
+            "default": "With origins still unknown, this versatile variety makes crisp, sweet Italian reds in a wide range of styles and locations.",
+            "julie": "Barbera is the most planted red grape varitety in the region of Piemonte, Italy. Barbera wines are deeply coloured, high in acidity, plump and with soft tannins. Famous DOC for production include Barbera d'Asti DOCG, Nizza DOCG and Barbera del Monferrato Superiore DOCG. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Barbera Bianca",
-        "synonyms": ["Bertolino", "Peisìn"],
-        "description": "Rare Piemontese variety unrelated to dark-skinned Barbera.",
-        "color": "white",
+        "synonyms": [
+            "Bertolino",
+            "Peisìn"
+        ],
+        "description": {
+            "default": "Rare Piemontese variety unrelated to dark-skinned Barbera.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Barbera Del Sannio",
-        "synonyms": ["Barbetta"],
-        "description": "Increasingly well-made central Italian variety unrelated to more northerly Barberas.",
-        "color": "black",
+        "synonyms": [
+            "Barbetta"
+        ],
+        "description": {
+            "default": "Increasingly well-made central Italian variety unrelated to more northerly Barberas.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Barcelo",
-        "synonyms": ["Barcello", "Barcelos"],
-        "description": "Minor Portuguese found in white Dão blends.",
-        "color": "white",
+        "synonyms": [
+            "Barcello",
+            "Barcelos"
+        ],
+        "description": {
+            "default": "Minor Portuguese found in white Dão blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bariadorgia",
         "synonyms": [
             "Bariadorgia Bianca",
             "Bariadorza",
             "Barria Dorgia",
             "Barriadorgia",
             "Carcaghjolu Biancu",
             "Carcajola",
             "Carcajola Bianco",
             "Carcajolo Blanc",
-            "Gregu Bianco",
+            "Gregu Bianco"
         ],
-        "description": "Virtually extinct Sardinian white, surviving on the French island of Corse as Carcajolo Blanc.",
-        "color": "white",
+        "description": {
+            "default": "Virtually extinct Sardinian white, surviving on the French island of Corse as Carcajolo Blanc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Baroque",
         "synonyms": [
             "Baroca",
             "Barroque",
             "Bordalès",
             "Bordelais Blanc",
-            "Bordeleza zuria",
+            "Bordeleza zuria"
         ],
-        "description": "South-west French variety given an injection of life from a renowned local chef.",
-        "color": "white",
+        "description": {
+            "default": "South-west French variety given an injection of life from a renowned local chef.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Barsaglina",
-        "synonyms": ["Barsullina", "Bersaglina", "Massareta", "Massaretta"],
-        "description": "Deeply coloured Tuscan red that has all but disappeared.",
-        "color": "black",
+        "synonyms": [
+            "Barsullina",
+            "Bersaglina",
+            "Massareta",
+            "Massaretta"
+        ],
+        "description": {
+            "default": "Deeply coloured Tuscan red that has all but disappeared.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bastardo Magarachsky",
         "synonyms": [
             "Bastard de Magaraci",
             "Bastardo Magarach",
             "Magaratch 217",
-            "Magarach Bastardo",
+            "Magarach Bastardo"
         ],
-        "description": "Versatile Ukrainian cross.",
-        "color": "black",
+        "description": {
+            "default": "Versatile Ukrainian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Batiki",
         "synonyms": [
             "Bantiki",
             "Dembatiki",
             "Deve Baliki",
             "Dimbatiki",
             "Dimi Batiki",
-            "Timbi Batiki",
+            "Timbi Batiki"
         ],
-        "description": "Variety grown mainly in central Greece making soft whites for blending, retsina and the table.",
-        "color": "white",
+        "description": {
+            "default": "Variety grown mainly in central Greece making soft whites for blending, retsina and the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Batoca",
         "synonyms": [
             "Alvadurao Portalegre",
             "Alvaraça",
             "Alvarça",
             "Alvaroça",
             "Alvaroco",
             "Asal Espanhol",
             "Batoco",
             "Blanca Mar",
             "Espadeiro Branco",
             "Sa Douro",
-            "Sedouro .",
+            "Sedouro ."
         ],
-        "description": "Minor, unexceptional white from Vinho Verde country.",
-        "color": "white",
+        "description": {
+            "default": "Minor, unexceptional white from Vinho Verde country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bayanshira",
         "synonyms": [
             "Ag Shirei",
             "Ag Üzüm",
             "Bahïan Chireï",
             "Bajac Shirei",
             "Banants",
             "Bayan Shirei",
             "Bayan Shirey",
             "Bayanshire",
             "Shirei",
-            "Spitak Khagog",
+            "Spitak Khagog"
         ],
-        "description": "Lacklustre Azeri variety with high acidity and generally low alcohol.",
-        "color": "white",
+        "description": {
+            "default": "Lacklustre Azeri variety with high acidity and generally low alcohol.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Beaunoir",
         "synonyms": [
             "Beaunoire",
             "Cep Gris",
             "Mourillon",
             "Pinot d’Aï",
             "Pinot d’Ailly",
             "Pinot d’Orléans",
-            "Sogris",
+            "Sogris"
         ],
-        "description": "Virtually extinct black-skinned variety with one illustrious and one promiscuous parent.",
-        "color": "black",
+        "description": {
+            "default": "Virtually extinct black-skinned variety with one illustrious and one promiscuous parent.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Beba",
         "synonyms": [
             "Beba de los Santos",
             "Beba Dorada de Jerez",
             "Blanca de Mesa",
@@ -1085,207 +1658,349 @@
             "Breval",
             "Calop Blanco",
             "Eva",
             "Malvoisie de la Chartreuse",
             "Malvoisie des Chartreux",
             "Teta de Vaca",
             "Uva de Planta",
-            "Valencí Blanco",
+            "Valencí Blanco"
         ],
-        "description": "Andalusian variety grown mainly in Extremadura today.",
-        "color": "white",
+        "description": {
+            "default": "Andalusian variety grown mainly in Extremadura today.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Béclan",
         "synonyms": [
             "Baclan",
             "Baclans",
             "Becclan",
             "Petit Béclan",
             "Petit Dureau",
             "Petit Margillin",
             "Roussette Noire",
-            "Saunoir",
+            "Saunoir"
         ],
-        "description": "Virtually extinct Jura vine.",
-        "color": "black",
+        "description": {
+            "default": "Virtually extinct Jura vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Beichun",
-        "synonyms": ["Bei Chun"],
-        "description": "Winter-hardy Chinese hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Bei Chun"
+        ],
+        "description": {
+            "default": "Winter-hardy Chinese hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bekari",
-        "synonyms": ["Bekaro", "Mbekari Mavro", "Mpekari Mavro", "Mbekaro", "Mpekaro"],
-        "description": "Minor variety local to Ípeiros (Epirus) in western Greece.",
-        "color": "black",
+        "synonyms": [
+            "Bekaro",
+            "Mbekari Mavro",
+            "Mpekari Mavro",
+            "Mbekaro",
+            "Mpekaro"
+        ],
+        "description": {
+            "default": "Minor variety local to Ípeiros (Epirus) in western Greece.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bellone",
-        "synonyms": ["Arciprete Bianco", "Cacchione", "Fagotto and many more"],
-        "description": "Vigorous Roman white that rarely appears solo.",
-        "color": "white",
+        "synonyms": [
+            "Arciprete Bianco",
+            "Cacchione",
+            "Fagotto and many more"
+        ],
+        "description": {
+            "default": "Vigorous Roman white that rarely appears solo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Béquignol Noir",
         "synonyms": [
             "Béquin Rouge",
             "Breton",
-            # "Cabernet",
+            "Cabernet",
             "Chalosse Noire",
             "Embalouzat",
-            "Mançais Noir",
+            "Mançais Noir"
         ],
-        "description": "Rare dark-skinned French variety much more common in Argentina.",
-        "color": "black",
+        "description": {
+            "default": "Rare dark-skinned French variety much more common in Argentina.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Berdomenel",
-        "synonyms": ["Berdanel"],
-        "description": "Virtually extinct Ariège variety recently replanted.",
-        "color": "white",
+        "synonyms": [
+            "Berdanel"
+        ],
+        "description": {
+            "default": "Virtually extinct Ariège variety recently replanted.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Besgano Bianco",
-        "synonyms": ["Colombana Bianca"],
-        "description": "Very rare northern Italian white once used to produce Vin Santo.",
-        "color": "white",
+        "synonyms": [
+            "Colombana Bianca"
+        ],
+        "description": {
+            "default": "Very rare northern Italian white once used to produce Vin Santo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bianca",
-        "synonyms": ["Bianka", "Ec 40", "Ecs 40", "Egri Csillagok 40", "May Rot"],
-        "description": "Hungarian hybrid producing generally unexciting wines, also in Russia.",
-        "color": "white",
+        "synonyms": [
+            "Bianka",
+            "Ec 40",
+            "Ecs 40",
+            "Egri Csillagok 40",
+            "May Rot"
+        ],
+        "description": {
+            "default": "Hungarian hybrid producing generally unexciting wines, also in Russia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bianchetta Trevigiana",
         "synonyms": [
             "Bianca Gentile di Fonzaso",
             "Bianchetta Gentile",
             "Bianchetta Semplice",
             "Senese",
             "Vernanzina",
-            "Vernassina",
+            "Vernassina"
         ],
-        "description": "Vigorous, thick-skinned northern Italian white producing rather ordinary, slightly astringent wines that are generally blended.",
-        "color": "white",
+        "description": {
+            "default": "Vigorous, thick-skinned northern Italian white producing rather ordinary, slightly astringent wines that are generally blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bianco D’Alessano",
         "synonyms": [
             "Acchiappapalmento",
             "Bianco di Lessame",
             "Iuvarello",
             "Verdurino",
-            "Vuiono",
+            "Vuiono"
         ],
-        "description": "Southern Italian white frequently blended with Verdeca, enjoying success in Australia.",
-        "color": "white",
+        "description": {
+            "default": "Southern Italian white frequently blended with Verdeca, enjoying success in Australia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Biancolella",
-        "synonyms": ["Bianculillo", "Jancolella", "San Nicola"],
-        "description": "Light white grape from Napoli and the neighbouring islands inspires some heroic production.",
-        "color": "white",
+        "synonyms": [
+            "Bianculillo",
+            "Jancolella",
+            "San Nicola"
+        ],
+        "description": {
+            "default": "Light white grape from Napoli and the neighbouring islands inspires some heroic production.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Biancone Di Portoferraio",
-        "synonyms": ["Biancone", "Pagadebiti di Porto S. Stefano"],
-        "description": "Ordinary white exclusive to Elba.",
-        "color": "white",
+        "synonyms": [
+            "Biancone",
+            "Pagadebiti di Porto S. Stefano"
+        ],
+        "description": {
+            "default": "Ordinary white exclusive to Elba.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Biancu Gentile",
-        "synonyms": ["Biancone Gentile"],
-        "description": "Rare, aromatic Corsican.",
-        "color": "white",
+        "synonyms": [
+            "Biancone Gentile"
+        ],
+        "description": {
+            "default": "Rare, aromatic Corsican.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bíborkadarka",
-        "synonyms": ["Bíbor Kadarka", "Biborkadarsa", "Cs 4"],
-        "description": "Minor red-fleshed Hungarian cross used mainly for colour.",
-        "color": "black",
+        "synonyms": [
+            "Bíbor Kadarka",
+            "Biborkadarsa",
+            "Cs 4"
+        ],
+        "description": {
+            "default": "Minor red-fleshed Hungarian cross used mainly for colour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bical",
         "synonyms": [
             "Arinto de Alcobaça",
             "Bical de Bairrada",
             "Borrado das Moscas",
             "Fernão Pires Galego",
             "Pintado das Moscas",
-            "Pintado dos Pardais",
+            "Pintado dos Pardais"
         ],
-        "description": "Aromatic, early-ripening variety widely planted in western central Portugal.",
-        "color": "white",
+        "description": {
+            "default": "Aromatic, early-ripening variety widely planted in western central Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bigolona",
         "synonyms": [
             "Bigolara",
             "Bigolona Bianca",
             "Bigolona Veronese",
             "Sampagna",
-            "Smarzirola",
+            "Smarzirola"
         ],
-        "description": "Rare white from the Valpolicella region of northern Italy used in sweet-wine blends.",
-        "color": "white",
+        "description": {
+            "default": "Rare white from the Valpolicella region of northern Italy used in sweet-wine blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Birstaler Muskat",
-        "synonyms": ["Birchstaler Muscat", "Muscat de la Birse", "VB 86-6"],
-        "description": "Light-skinned Swiss hybrid used mainly for the table.",
-        "color": "white",
+        "synonyms": [
+            "Birchstaler Muscat",
+            "Muscat de la Birse",
+            "VB 86-6"
+        ],
+        "description": {
+            "default": "Light-skinned Swiss hybrid used mainly for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Black Queen",
-        "synonyms": ["Pokdum", "Pok Dum"],
-        "description": "Japanese complex hybrid widely used for winemaking in Asia.",
-        "color": "black",
+        "synonyms": [
+            "Pokdum",
+            "Pok Dum"
+        ],
+        "description": {
+            "default": "Japanese complex hybrid widely used for winemaking in Asia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Blanc Dame",
         "synonyms": [
             "Blanc Madame",
             "Blanquette Grise",
             "Clairette de Gascogne",
             "Claret",
             "Claret de Gascogne",
-            "Plan de Dame",
+            "Plan de Dame"
         ],
-        "description": "Almost abandoned by south-west French vignerons but not quite by armagnac distillers.",
-        "color": "white",
+        "description": {
+            "default": "Almost abandoned by south-west French vignerons but not quite by armagnac distillers.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Blanc Du Bois",
-        "synonyms": ["Blanc DuBois", "Florida H18-37"],
-        "description": "Potentially high-quality, aromatic hybrid from Florida with useful resistance to Pierce’s disease.",
-        "color": "white",
+        "synonyms": [
+            "Blanc DuBois",
+            "Florida H18-37"
+        ],
+        "description": {
+            "default": "Potentially high-quality, aromatic hybrid from Florida with useful resistance to Pierce’s disease.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Blanqueiro",
-        "synonyms": ["Blanqueirol", "Blanqueiron", "Blanquerel", "Pignairon"],
-        "description": "Very minor Provençal variety.",
-        "color": "white",
+        "synonyms": [
+            "Blanqueirol",
+            "Blanqueiron",
+            "Blanquerel",
+            "Pignairon"
+        ],
+        "description": {
+            "default": "Very minor Provençal variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Blatina",
         "synonyms": [
             "Blathina",
             "Blatina Crna",
             "Blatina Hercegovacka",
             "Blatina Mala",
             "Blatina Velika",
             "Praznobačva",
-            "Zlorod",
+            "Zlorod"
         ],
-        "description": "Bosnia and Herzegovina’s most important red variety.",
-        "color": "black",
+        "description": {
+            "default": "Bosnia and Herzegovina’s most important red variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Blauer Portugieser",
         "synonyms": [
             "Autrichien",
             "Badner",
             "Early Burgundy",
@@ -1293,30 +2008,51 @@
             "Oporto",
             "Portugais Bleu",
             "Portugalkja",
             "Portugieser",
             "Portugieser Blau",
             "Portugizac Crni",
             "Português Azul",
-            "Vöslauer ; Kékoportó is no longer officially used in Hungary",
+            "Vöslauer ; Kékoportó is no longer officially used in Hungary"
         ],
-        "description": "Prolific Austrian red wine variety producing rather dull, low-acid wines.",
-        "color": "black",
+        "description": {
+            "default": "Prolific Austrian red wine variety producing rather dull, low-acid wines.",
+            "julie": "",
+            "sommelier": "Portugieser wines are uncomplicated, fruity, and fresh – easy drinking for everyday enjoyment. Medium-bodied and mild in tannins, they have restrained aromas of red currant, raspberry, sour cherry, or pepper. Portugieser is considered an uncomplicated, pleasant, full-bodied, drinkable and fresh wine. Without too much tannin, it develops quickly and is already a harmonious, easy-to-drink wine in spring. It can then also be served slightly cooler (rosé 9 - 13° C and red wine 14 - 16° C). This enhances the refreshing character of the light rosé or red wine, which usually has an invigorating acidity. In the restrained bouquet we find hints of berry flavours such as redcurrant, raspberry or strawberry, sometimes also sour cherry or a peppery note. The Portugieser can be a frugal accompaniment to many dishes. Flavour: red currant, strawberry, sour cherry, peppery note."
+        },
+        "color": "black"
     },
     {
         "name": "Blauer Urban",
-        "synonyms": ["Schwarzer Urban", "Urban", "Urban Blau", "Urban Blauer"],
-        "description": "Rarity just about surviving in southern Germany.",
-        "color": "black",
+        "synonyms": [
+            "Schwarzer Urban",
+            "Urban",
+            "Urban Blau",
+            "Urban Blauer"
+        ],
+        "description": {
+            "default": "Rarity just about surviving in southern Germany.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Blauer Wildbacher",
-        "synonyms": ["Schilcher", "Wildbacher", "Wildbacher Blau"],
-        "description": "Distinctively perfumed Austrian red wine grape producing eye-watering pinks.",
-        "color": "black",
+        "synonyms": [
+            "Schilcher",
+            "Wildbacher",
+            "Wildbacher Blau"
+        ],
+        "description": {
+            "default": "Distinctively perfumed Austrian red wine grape producing eye-watering pinks.",
+            "julie": "",
+            "sommelier": "The Blauer Wildbacher is a relative of Blaufränkisch and originates from a Gouais Blanc seedling. Despite the very small acreage of plantings in its native Weststeiermark (Styria), the Wildbacher is much better known as the Schilcher rosé wine. Racy acidity as well as a distinctive aroma and taste characterise the fruity-fresh, robust wine - which can be enjoyed also as an apéritif. In gneiss and slate soils, the variety achieves a grassy and spicy expression. Red wine is also made from Blauer Wildbacher, as is Prädikatswein (including Eiswein)."
+        },
+        "color": "black"
     },
     {
         "name": "Blaufränkisch",
         "synonyms": [
             "Blauer Limberger",
             "Borgonja",
             "Burgund Mare",
@@ -1326,18 +2062,22 @@
             "Frankovka Modrá",
             "Frankovna Crna",
             "Gamé",
             "Kékfrankos",
             "Limberger",
             "Lemberger",
             "Nagyburgundi",
-            "Sura Lisicina",
+            "Sura Lisicina"
         ],
-        "description": "Dark-skinned, dark-fruited Austro-Hungarian variety increasingly well grown and vinified, gaining ground.",
-        "color": "black",
+        "description": {
+            "default": "Dark-skinned, dark-fruited Austro-Hungarian variety increasingly well grown and vinified, gaining ground.",
+            "julie": "Blaufränkisch is Austria second most planted red grape variety. The variety produces a wide array of wine styles ranging from light, fresh and fruity to intensely flavoured, firmly structured and spicy. In Germany, the variety is called Lemberger and in Hungary it is known as Kékfrankos.",
+            "sommelier": "The Blaufränkisch is a thoroughly central European variety. This traditional Austrian variety is probably a cross between Sbulzina and Weißer Heunisch. Blaufränkisch was previously widely-planted throughout the Habsburg Monachy, and is the most important variety in Mittelburgenland, called Blaufränkischland. The typical bouquet of Blaufränkisch wines displays profound notes of wild berries or cherries, as well as a powerful acidity characteristic of this grape. Blaufränkisch can yield outstanding wines with dense structure and prominent tannins. The wines are often impetuous in their youth but develop velvety facets when sufficiently mature. Dense wines have very good ageing potential."
+        },
+        "color": "black"
     },
     {
         "name": "Bobal",
         "synonyms": [
             "Balau",
             "Benicarló",
             "Bobos",
@@ -1349,342 +2089,611 @@
             "Pobretón",
             "Provechón",
             "Rajeno",
             "Requena",
             "Terret d’Espagne",
             "Tinta Madrid",
             "Tonto de Zurra",
-            "Valenciana",
+            "Valenciana"
         ],
-        "description": "Important and increasingly respected variety producing velvety wines in Spain’s Levante.",
-        "color": "black",
+        "description": {
+            "default": "Important and increasingly respected variety producing velvety wines in Spain’s Levante.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Boğazkere",
-        "synonyms": ["Şaraplık Siyah"],
-        "description": "Tannic but potentially high-quality, quite common Turkish variety.",
-        "color": "black",
+        "synonyms": [
+            "Şaraplık Siyah"
+        ],
+        "description": {
+            "default": "Tannic but potentially high-quality, quite common Turkish variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bogdanuša",
         "synonyms": [
             "Bogdanjuša",
             "Bogdanuša Bijela",
             "Bojdanuša",
             "Hvarka",
-            "Vrbanjka",
+            "Vrbanjka"
         ],
-        "description": "Makes light, fresh white on the Croatian island of Hvar.",
-        "color": "white",
+        "description": {
+            "default": "Makes light, fresh white on the Croatian island of Hvar.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bombino Bianco",
         "synonyms": [
             "Bambino",
             "Buonvino",
             "Ottonese",
             "Pagadebit",
-            "Straccia Cambiale",
+            "Straccia Cambiale"
         ],
-        "description": "Productive Italian white found mainly in the south and only rarely distinguished.",
-        "color": "white",
+        "description": {
+            "default": "Productive Italian white found mainly in the south and only rarely distinguished.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bombino Nero",
-        "synonyms": ["Bambino", "Buonvino"],
-        "description": "Southern Italian dark-skinned variety much less common than its pale namesake.",
-        "color": "black",
+        "synonyms": [
+            "Bambino",
+            "Buonvino"
+        ],
+        "description": {
+            "default": "Southern Italian dark-skinned variety much less common than its pale namesake.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bonamico",
-        "synonyms": ["Giacomino", "Uva di Palaia"],
-        "description": "High-yielding Italian black variety hanging on in the Pisa region.",
-        "color": "black",
+        "synonyms": [
+            "Giacomino",
+            "Uva di Palaia"
+        ],
+        "description": {
+            "default": "High-yielding Italian black variety hanging on in the Pisa region.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bonarda Piemontese",
         "synonyms": [
             "Bonarda del Monferrato",
             "Bonarda dell’Astigiano",
-            "Bonarda di Chieri",
+            "Bonarda di Chieri"
         ],
-        "description": "Aromatic, well-coloured Italian red with small bunches and soft tannins.",
-        "color": "black",
+        "description": {
+            "default": "Aromatic, well-coloured Italian red with small bunches and soft tannins.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bondola",
-        "synonyms": ["Bondola Nera", "Briegler", "Brieger", "Bundula", "Longobardo"],
-        "description": "Old, rare Ticino variety that has been overwhelmed by Merlot.",
-        "color": "black",
+        "synonyms": [
+            "Bondola Nera",
+            "Briegler",
+            "Brieger",
+            "Bundula",
+            "Longobardo"
+        ],
+        "description": {
+            "default": "Old, rare Ticino variety that has been overwhelmed by Merlot.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bordô",
-        "synonyms": ["Grana d’Oro"],
-        "description": "American hybrid used to make cheap, sweetish reds and juices in Brazil.",
-        "color": "black",
+        "synonyms": [
+            "Grana d’Oro"
+        ],
+        "description": {
+            "default": "American hybrid used to make cheap, sweetish reds and juices in Brazil.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Borraçal",
         "synonyms": [
             "Azedo",
             "Bogalhal",
             "Caíño Tinto",
             "Espadeiro Redondo",
             "Olho de Sapo",
-            "Tinta Femia",
+            "Tinta Femia"
         ],
-        "description": "Makes potent, tart, sometimes tough wines in north-west Spain as well as in its native Vinho Verde.",
-        "color": "black",
+        "description": {
+            "default": "Makes potent, tart, sometimes tough wines in north-west Spain as well as in its native Vinho Verde.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bosco",
-        "synonyms": ["Bosco Bianco del Genovese", "Bosco Bianco di Savona"],
-        "description": "Ligurian white speciality making excellent sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Bosco Bianco del Genovese",
+            "Bosco Bianco di Savona"
+        ],
+        "description": {
+            "default": "Ligurian white speciality making excellent sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bouchalès",
         "synonyms": [
             "Bouchalets",
             "Bouissalet",
             "Gros Bouchalès",
             "Gros Boucharès",
             "Grappu",
             "Grapput",
             "Picardan Noir",
-            "Prolongeau",
+            "Prolongeau"
         ],
-        "description": "Declining dark-skinned variety surviving around Bordeaux.",
-        "color": "black",
+        "description": {
+            "default": "Declining dark-skinned variety surviving around Bordeaux.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bourboulenc",
         "synonyms": [
             "Blanquette",
             "Bourboulenco",
             "Bourbouleng",
             "Bourboulenque",
             "Bourbounenco",
             "Clairette à Grains Ronds",
             "Clairette Dorée",
             "Doucillon",
             "Malvoisie",
-            "Picardan",
+            "Picardan"
         ],
-        "description": "Useful vine making interesting white throughout the south of France.",
-        "color": "white",
+        "description": {
+            "default": "Useful vine making interesting white throughout the south of France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bourrisquou",
-        "synonyms": ["Bourriscou", "Mourrisquou de Romani", "Romanet"],
-        "description": "Very rarely makes wine; better known as the parent of various rootstocks.",
-        "color": "black",
+        "synonyms": [
+            "Bourriscou",
+            "Mourrisquou de Romani",
+            "Romanet"
+        ],
+        "description": {
+            "default": "Very rarely makes wine; better known as the parent of various rootstocks.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bouteillan Noir",
-        "synonyms": ["Fouiral", "Moulas", "Psalmodi Noir", "Sigoyer"],
-        "description": "Virtually extinct Provençal variety.",
-        "color": "black",
+        "synonyms": [
+            "Fouiral",
+            "Moulas",
+            "Psalmodi Noir",
+            "Sigoyer"
+        ],
+        "description": {
+            "default": "Virtually extinct Provençal variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bouvier",
         "synonyms": [
             "Bela Ranina",
             "Bouvier Blanc",
             "Bouvierovo Hrozno",
             "Bouviertraube",
             "Radgonska Ranina",
             "Ranina",
-            "Ranina Bela",
+            "Ranina Bela"
         ],
-        "description": "Low-acid Central European variety used for many styles of wine.",
-        "color": "white",
+        "description": {
+            "default": "Low-acid Central European variety used for many styles of wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bracciola Nera",
-        "synonyms": ["Bracciuola", "Braciola", "Braciuola", "Brassola"],
-        "description": "Obscure, high-yielding, late-ripening black Italian variety found in Toscana and Liguria.",
-        "color": "black",
+        "synonyms": [
+            "Bracciuola",
+            "Braciola",
+            "Braciuola",
+            "Brassola"
+        ],
+        "description": {
+            "default": "Obscure, high-yielding, late-ripening black Italian variety found in Toscana and Liguria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Brachetto Del Piemonte",
-        "synonyms": ["Bracchetto", "Brachetto d’Acqui"],
-        "description": "Rose-scented Piemontese variety making very light, sweet, frothy reds.",
-        "color": "black",
+        "synonyms": [
+            "Bracchetto",
+            "Brachetto d’Acqui"
+        ],
+        "description": {
+            "default": "Rose-scented Piemontese variety making very light, sweet, frothy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Braquet Noir",
-        "synonyms": ["Brachet"],
-        "description": "Very minor but historic, vine making aromatic light reds around Nice.",
-        "color": "black",
+        "synonyms": [
+            "Brachet"
+        ],
+        "description": {
+            "default": "Very minor but historic, vine making aromatic light reds around Nice.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bratkovina Bijela",
-        "synonyms": ["Brabkovica", "Mesnac"],
-        "description": "Rare Croatian island white adding freshness to Pošip blends.",
-        "color": "white",
+        "synonyms": [
+            "Brabkovica",
+            "Mesnac"
+        ],
+        "description": {
+            "default": "Rare Croatian island white adding freshness to Pošip blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Brauner Veltliner",
-        "synonyms": ["Todträger", "Veltliner Braun"],
-        "description": "Almost extinct Austrian, unrelated to Roter Veltliner.",
-        "color": "grey",
+        "synonyms": [
+            "Todträger",
+            "Veltliner Braun"
+        ],
+        "description": {
+            "default": "Almost extinct Austrian, unrelated to Roter Veltliner.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey"
     },
     {
         "name": "Breidecker",
-        "synonyms": ["Geisenheim 49-84"],
-        "description": "Relatively neutral German hybrid that has found limited favour in New Zealand.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 49-84"
+        ],
+        "description": {
+            "default": "Relatively neutral German hybrid that has found limited favour in New Zealand.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Breslava",
-        "synonyms": ["CHRTČ × St Dc ALC 10/28", "Chrtc × St M D#Alc 10/28"],
-        "description": "One of the earliest Slovakian crosses but little dispersed.",
-        "color": "white",
+        "synonyms": [
+            "CHRTČ × St Dc ALC 10/28",
+            "Chrtc × St M D#Alc 10/28"
+        ],
+        "description": {
+            "default": "One of the earliest Slovakian crosses but little dispersed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Brianna",
-        "synonyms": ["ES 7-4-76"],
-        "description": "Minor but usefully winter-hardy and increasingly popular American hybrid.",
-        "color": "white",
+        "synonyms": [
+            "ES 7-4-76"
+        ],
+        "description": {
+            "default": "Minor but usefully winter-hardy and increasingly popular American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bronner",
-        "synonyms": ["Freiburg 250-75"],
-        "description": "German hybrid bred for its disease resistance.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 250-75"
+        ],
+        "description": {
+            "default": "German hybrid bred for its disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Brun Argenté",
-        "synonyms": ["Camarèse", "Camarèze", "Vaccarèse", "Vacarèse", "Vaccarèze"],
-        "description": "Very minor southern Rhône variety.",
-        "color": "black",
+        "synonyms": [
+            "Camarèse",
+            "Camarèze",
+            "Vaccarèse",
+            "Vacarèse",
+            "Vaccarèze"
+        ],
+        "description": {
+            "default": "Very minor southern Rhône variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Brun Fourca",
         "synonyms": [
             "Brun d’Auriol",
             "Brun Fourcat",
             "Farnous",
             "Flouron",
             "Mançonnet",
             "Moulan",
             "Moureau",
             "Mouzeau",
-            "Mourrastel-Flourat",
+            "Mourrastel-Flourat"
         ],
-        "description": "Ancient but now virtually extinct western Provençal vine.",
-        "color": "black",
+        "description": {
+            "default": "Ancient but now virtually extinct western Provençal vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Brustiano Bianco",
-        "synonyms": ["Calitrano", "Colitrano", "Licronaxu Bianco"],
-        "description": "Scarce white variety found on the Italian island of Sardegna and reintroduced on the French island of Corse.",
-        "color": "white",
+        "synonyms": [
+            "Calitrano",
+            "Colitrano",
+            "Licronaxu Bianco"
+        ],
+        "description": {
+            "default": "Scarce white variety found on the Italian island of Sardegna and reintroduced on the French island of Corse.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Budai Zöld",
-        "synonyms": ["Budai", "Zöld Budai", "Zöld Szőlő", "Zöldfehér", "Zöldszőlő"],
-        "description": "Very minor Hungarian variety making fresh, simple whites.",
-        "color": "white",
+        "synonyms": [
+            "Budai",
+            "Zöld Budai",
+            "Zöld Szőlő",
+            "Zöldfehér",
+            "Zöldszőlő"
+        ],
+        "description": {
+            "default": "Very minor Hungarian variety making fresh, simple whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Budeshuri Tsiteli",
-        "synonyms": ["Budeshuri Saperavi", "Budeshuri Shavi", "Tsiteli Budeshuri"],
-        "description": "Very minor Georgian variety usually blended with Saperavi.",
-        "color": "pink",
+        "synonyms": [
+            "Budeshuri Saperavi",
+            "Budeshuri Shavi",
+            "Tsiteli Budeshuri"
+        ],
+        "description": {
+            "default": "Very minor Georgian variety usually blended with Saperavi.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Buket",
-        "synonyms": ["Bouquet"],
-        "description": "Relatively unknown Bulgarian cross with potential for well-structured, full-flavoured reds.",
-        "color": "black",
+        "synonyms": [
+            "Bouquet"
+        ],
+        "description": {
+            "default": "Relatively unknown Bulgarian cross with potential for well-structured, full-flavoured reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Bukettraube",
         "synonyms": [
             "Bocksbeutel",
             "Bouquettraube",
             "Buket",
             "Bukettrebe",
-            "Würzburger",
+            "Würzburger"
         ],
-        "description": "Aromatic cross bred in Germany but most widely planted in South Africa for sweet wines.",
-        "color": "white",
+        "description": {
+            "default": "Aromatic cross bred in Germany but most widely planted in South Africa for sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Bussanello",
-        "synonyms": ["Incrocio Dalmasso 12/37"],
-        "description": "Aromatic white Italian cross recommended in parts of Piemonte.",
-        "color": "white",
+        "synonyms": [
+            "Incrocio Dalmasso 12/37"
+        ],
+        "description": {
+            "default": "Aromatic white Italian cross recommended in parts of Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Busuioacă De Bohotin",
         "synonyms": [
             "Busuioacă Neagră",
             "Busuioacă Vânată de Bohotin",
             "Tămâioasă de Bohotin",
-            "Tămâioasă Violetă",
+            "Tămâioasă Violetă"
         ],
-        "description": "Aromatic pink-skinned Romanian variety making sweet, well-balanced Muscat-like wines.",
-        "color": "pink",
+        "description": {
+            "default": "Aromatic pink-skinned Romanian variety making sweet, well-balanced Muscat-like wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Caberinta",
-        "synonyms": ["CG 14892", "Gargiulo 14892"],
-        "description": "Productive but not very popular Argentine hybrid.",
-        "color": "black",
+        "synonyms": [
+            "CG 14892",
+            "Gargiulo 14892"
+        ],
+        "description": {
+            "default": "Productive but not very popular Argentine hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Blanc",
-        "synonyms": ["VB 91-26-1"],
-        "description": "Recent Swiss hybrid that combines fresh, clean flavours and good disease resistance.",
-        "color": "white",
+        "synonyms": [
+            "VB 91-26-1"
+        ],
+        "description": {
+            "default": "Recent Swiss hybrid that combines fresh, clean flavours and good disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cabernet Carbon",
-        "synonyms": ["Freiburg 377-83"],
-        "description": "Recent tannic German, very complex, hybrid bred for superior disease resistance.",
-        "color": "black",
+        "synonyms": [
+            "Freiburg 377-83"
+        ],
+        "description": {
+            "default": "Recent tannic German, very complex, hybrid bred for superior disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Carol",
-        "synonyms": ["Freiburg 428-82 R"],
-        "description": "Barely planted disease-resistant German hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Freiburg 428-82 R"
+        ],
+        "description": {
+            "default": "Barely planted disease-resistant German hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Colonjes",
-        "synonyms": ["VB 91-26-5", "VB 91-26-05"],
-        "description": "Minor dark-skinned Swiss hybrid found mainly in the Netherlands.",
-        "color": "black",
+        "synonyms": [
+            "VB 91-26-5",
+            "VB 91-26-05"
+        ],
+        "description": {
+            "default": "Minor dark-skinned Swiss hybrid found mainly in the Netherlands.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Cortis",
-        "synonyms": ["Freiburg 437-82 R"],
-        "description": "Recent tannic German hybrid bred for superior disease resistance.",
-        "color": "black",
+        "synonyms": [
+            "Freiburg 437-82 R"
+        ],
+        "description": {
+            "default": "Recent tannic German hybrid bred for superior disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Cubin",
-        "synonyms": ["Weinsberg 70-281-35"],
-        "description": "Deeply coloured, tannin-rich German cross that needs the best sites to ripen fully.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg 70-281-35"
+        ],
+        "description": {
+            "default": "Deeply coloured, tannin-rich German cross that needs the best sites to ripen fully.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Dorio",
-        "synonyms": ["Weinsberg 71-817-89"],
-        "description": "Recent German cross with a certain Cabernet likeness.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg 71-817-89"
+        ],
+        "description": {
+            "default": "Recent German cross with a certain Cabernet likeness.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Dorsa",
-        "synonyms": ["Weinsberg 71-817-92"],
-        "description": "The most successful of the new German Cabernets.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg 71-817-92"
+        ],
+        "description": {
+            "default": "The most successful of the new German Cabernets.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Franc",
         "synonyms": [
             "Achéria",
             "Ardounet",
             "Bidure",
@@ -1705,42 +2714,70 @@
             "Sable Rouge",
             "Trouchet",
             "Tsapournako",
             "Verdejilla Tinto",
             "Véron",
             "Vidure",
             "Vuidure",
-            "Grosse Vidure",
+            "Grosse Vidure"
         ],
-        "description": "Fragrant, well-structured parent of Cabernet Sauvignon that shines in the Loire and in Bordeaux blends.",
-        "color": "black",
+        "description": {
+            "default": "Fragrant, well-structured parent of Cabernet Sauvignon that shines in the Loire and in Bordeaux blends.",
+            "julie": "Cabernet franc is one of the most ancient grape varities found in the region of Bordeaux. Today it is also widely planted in the Loire Valley where it is often known as \"Breton\". Cabernet Franc produces wines that have a characteristic herbal aromas ranging from refreshing leafiness when ripe to full on green bell pepper (pyrazine) when underripe. In the Loire Valley, the wines can be supple, medium-bodied, with aromas of raspberries and pencil shavings or can show more structure and minerality in regions such as Saumur-Champigny. In Bordeaux, Cabernet Franc is most often blended with Merlot and Cabernet Sauvignon, howver, some producers in the region of Saint Emilion are using the grape variety as a solo player or as the main player. The grape is also found in many other countries around the world. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Jura",
-        "synonyms": ["VB 5-02"],
-        "description": "A recent dark-skinned, disease-resistant Swiss hybrid that has so far remained in its homeland.",
-        "color": "black",
+        "synonyms": [
+            "VB 5-02"
+        ],
+        "description": {
+            "default": "A recent dark-skinned, disease-resistant Swiss hybrid that has so far remained in its homeland.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Mitos",
-        "synonyms": ["Weinsberg 70-77-4F"],
-        "description": "Recent, deeply coloured German cross making wines useful in blends.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg 70-77-4F"
+        ],
+        "description": {
+            "default": "Recent, deeply coloured German cross making wines useful in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Moravia",
-        "synonyms": ["M-43"],
-        "description": "High-quality, late-ripening Czech cross producing Cabernet-like wines.",
-        "color": "black",
+        "synonyms": [
+            "M-43"
+        ],
+        "description": {
+            "default": "High-quality, late-ripening Czech cross producing Cabernet-like wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Pfeffer",
-        "synonyms": ["Pfeffer Cabernet"],
-        "description": "Rare, peppery California cross.",
-        "color": "black",
+        "synonyms": [
+            "Pfeffer Cabernet"
+        ],
+        "description": {
+            "default": "Rare, peppery California cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Sauvignon",
         "synonyms": [
             "Bidure",
             "Bordeaux",
             "Bordo",
@@ -1758,190 +2795,336 @@
             "Navarre",
             "Petit Cabernet",
             "Petit Cavernet Sauvignon",
             "Sauvignon",
             "Sauvignonne",
             "Vidure",
             "Vidure Sauvignonne",
-            "Petite Vidure",
+            "Petite Vidure"
         ],
-        "description": "The world’s best-travelled red wine variety making concentrated, tannic wines for particularly long ageing.",
-        "color": "black",
+        "description": {
+            "default": "The world’s best-travelled red wine variety making concentrated, tannic wines for particularly long ageing.",
+            "julie": "The number one red grape in the world is originally from the Gironde region in France. Cabernet Sauvignon has small, thick-skinned berries that contribute to deep colour, high tannins and relatively high acidity in the wine. Aronatically Cabernet is often associated with blackcurrant.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabernet Severny",
-        "synonyms": ["Cabernet Szevernuej", "Kaberne Severnyi"],
-        "description": "Winter-hardy hybrid with Asian not Cabernet genes but marked Cabernet colour and flavours.",
-        "color": "black",
+        "synonyms": [
+            "Cabernet Szevernuej",
+            "Kaberne Severnyi"
+        ],
+        "description": {
+            "default": "Winter-hardy hybrid with Asian not Cabernet genes but marked Cabernet colour and flavours.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cabertin",
-        "synonyms": ["VB 91-26-17"],
-        "description": "Recent disease-resistant Swiss hybrid with potential.",
-        "color": "black",
+        "synonyms": [
+            "VB 91-26-17"
+        ],
+        "description": {
+            "default": "Recent disease-resistant Swiss hybrid with potential.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cacaboué",
         "synonyms": [
             "Caca d’Oie",
             "Cacabois",
             "Cacabouet",
             "Persan Blanc",
-            "Saint-Péray",
+            "Saint-Péray"
         ],
-        "description": "Virtually extinct Savoie vine.",
-        "color": "white",
+        "description": {
+            "default": "Virtually extinct Savoie vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cacamosca",
-        "synonyms": ["Riciniello Bianco"],
-        "description": "Rare, low-yielding Campanian white.",
-        "color": "white",
+        "synonyms": [
+            "Riciniello Bianco"
+        ],
+        "description": {
+            "default": "Rare, low-yielding Campanian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Caddiu",
-        "synonyms": ["Caddeo", "Caddiu Nieddu", "Caddu", "Pàmpinu"],
-        "description": "Sardinian blending and sometimes table grape.",
-        "color": "black",
+        "synonyms": [
+            "Caddeo",
+            "Caddiu Nieddu",
+            "Caddu",
+            "Pàmpinu"
+        ],
+        "description": {
+            "default": "Sardinian blending and sometimes table grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Caíño Blanco",
-        "synonyms": ["Cainho de Moreira", "Caíño Branco"],
-        "description": "Rare Iberian white that ripens late but keeps its acidity.",
-        "color": "white",
+        "synonyms": [
+            "Cainho de Moreira",
+            "Caíño Branco"
+        ],
+        "description": {
+            "default": "Rare Iberian white that ripens late but keeps its acidity.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Caladoc",
-        "synonyms": ["Kaladok"],
-        "description": "Usefully reliable cross created in southern France but now well dispersed.",
-        "color": "black",
+        "synonyms": [
+            "Kaladok"
+        ],
+        "description": {
+            "default": "Usefully reliable cross created in southern France but now well dispersed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Calagraño",
-        "synonyms": ["Calagraña", "Navès"],
-        "description": "Virtually extinct Rioja vine making coarse, uninteresting wine.",
-        "color": "white",
+        "synonyms": [
+            "Calagraña",
+            "Navès"
+        ],
+        "description": {
+            "default": "Virtually extinct Rioja vine making coarse, uninteresting wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Calandro",
-        "synonyms": ["Geilweilerhof 84-58-1233"],
-        "description": "Recent German hybrid awaiting official recognition.",
-        "color": "black",
+        "synonyms": [
+            "Geilweilerhof 84-58-1233"
+        ],
+        "description": {
+            "default": "Recent German hybrid awaiting official recognition.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Calitor Noir",
         "synonyms": [
             "Col Tor",
             "Colitor",
             "Coytor",
             "Garriga",
             "Pécoui-Touar",
-            "Picpoul de Fronton",
+            "Picpoul de Fronton"
         ],
-        "description": "Declining, low-quality Provençal variety with more synonyms than hectares under vine.",
-        "color": "black",
+        "description": {
+            "default": "Declining, low-quality Provençal variety with more synonyms than hectares under vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Çalkarasi",
-        "synonyms": ["Çal Karası"],
-        "description": "Produces light, fresh reds and rosés in south-west Turkey.",
-        "color": "black",
+        "synonyms": [
+            "Çal Karası"
+        ],
+        "description": {
+            "default": "Produces light, fresh reds and rosés in south-west Turkey.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Camaralet De Lasseube",
         "synonyms": [
             "Camaralet",
             "Camaralet Blanc",
             "Camaralet de la Seube",
             "Camarau Blanc",
             "Kamarau",
             "Gentil Aromatique",
             "Moustardet",
-            "Petit Camarau",
+            "Petit Camarau"
         ],
-        "description": "Low fertility threatens this south-west France vine that can produce full-bodied, aromatic whites.",
-        "color": "white",
+        "description": {
+            "default": "Low fertility threatens this south-west France vine that can produce full-bodied, aromatic whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Camaraou Noir",
-        "synonyms": ["Caíño Redondo", "Camarau", "Kamarau", "Moustardet"],
-        "description": "Vigorous south-west French vine makes basic wine, mainly in Galicia.",
-        "color": "black",
+        "synonyms": [
+            "Caíño Redondo",
+            "Camarau",
+            "Kamarau",
+            "Moustardet"
+        ],
+        "description": {
+            "default": "Vigorous south-west French vine makes basic wine, mainly in Galicia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Camarate",
         "synonyms": [
             "Camarate Tinto",
             "Castelão da Bairrada",
             "Castelão do Nosso",
             "Castelão Nacional",
             "Moreto do Douro",
             "Moreto de Soure",
             "Mortágua",
             "Mortagua de Vide Preta",
             "Negro Mouro",
-            "Vide Preta",
+            "Vide Preta"
         ],
-        "description": "Sun-loving Portuguese variety making soft, easy-drinking reds.",
-        "color": "black",
+        "description": {
+            "default": "Sun-loving Portuguese variety making soft, easy-drinking reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Campbell Early",
-        "synonyms": ["Campbell", "Campbell’s Early", "Island Belle"],
-        "description": "North American hybrid now more widely grown in Asia, often for the table.",
-        "color": "black",
+        "synonyms": [
+            "Campbell",
+            "Campbell’s Early",
+            "Island Belle"
+        ],
+        "description": {
+            "default": "North American hybrid now more widely grown in Asia, often for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Canada Muscat",
-        "synonyms": ["NY 17806"],
-        "description": "Grapey hybrid just about surviving in Australia.",
-        "color": "white",
+        "synonyms": [
+            "NY 17806"
+        ],
+        "description": {
+            "default": "Grapey hybrid just about surviving in Australia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Canaiolo Nero",
-        "synonyms": ["Cannaiola di Marta", "Cannaiola Macchie di Marta"],
-        "description": "Soft, full-bodied, central Italian red used mainly to complement Sangiovese.",
-        "color": "black",
+        "synonyms": [
+            "Cannaiola di Marta",
+            "Cannaiola Macchie di Marta"
+        ],
+        "description": {
+            "default": "Soft, full-bodied, central Italian red used mainly to complement Sangiovese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Canari Noir",
-        "synonyms": ["Batista", "Canaril", "Canarill", "Carcassès", "Luverdon"],
-        "description": "Hanging on by a thread in the Ariège.",
-        "color": "black",
+        "synonyms": [
+            "Batista",
+            "Canaril",
+            "Canarill",
+            "Carcassès",
+            "Luverdon"
+        ],
+        "description": {
+            "default": "Hanging on by a thread in the Ariège.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cañocazo",
-        "synonyms": ["False Pedro", "Hardskin Pedro", "Mollar Blanco", "Pedro"],
-        "description": "Virtually extinct variety once popular in sherry country.",
-        "color": "white",
+        "synonyms": [
+            "False Pedro",
+            "Hardskin Pedro",
+            "Mollar Blanco",
+            "Pedro"
+        ],
+        "description": {
+            "default": "Virtually extinct variety once popular in sherry country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Caracol",
-        "synonyms": ["Olho de Pargo", "Uva das Eiras"],
-        "description": "Very minor variety found on the Portuguese island of Porto Santo.",
-        "color": "white",
+        "synonyms": [
+            "Olho de Pargo",
+            "Uva das Eiras"
+        ],
+        "description": {
+            "default": "Very minor variety found on the Portuguese island of Porto Santo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cardinal",
         "synonyms": [
             "Apostoliatiko",
             "Francesa",
             "G 10-30",
             "Karaburnu Rannii",
             "Kardinal",
-            "Rannii Carabournu",
+            "Rannii Carabournu"
         ],
-        "description": "Red-skinned North American table grape occasionally used to make wine in parts of Asia.",
-        "color": "red",
+        "description": {
+            "default": "Red-skinned North American table grape occasionally used to make wine in parts of Asia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Cargarello",
-        "synonyms": ["Cargarèl"],
-        "description": "White variety on the verge of extinction in the Rimini area of northern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Cargarèl"
+        ],
+        "description": {
+            "default": "White variety on the verge of extinction in the Rimini area of northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Carmenère",
         "synonyms": [
             "Bordo",
             "Cabernelle",
             "Cabernet Gernicht",
@@ -1950,110 +3133,182 @@
             "Cabernet Shelongzhu",
             "Carbonet",
             "Carbouet",
             "Caremenelle",
             "Carménègre",
             "Carménère",
             "Carmeneyre",
-            "Grosse Vidure",
+            "Grosse Vidure"
         ],
-        "description": "Produces deeply coloured, sometimes herbaceous wines, in Chile far more than in its native Bordeaux.",
-        "color": "black",
+        "description": {
+            "default": "Produces deeply coloured, sometimes herbaceous wines, in Chile far more than in its native Bordeaux.",
+            "julie": "Carménère is an old grape varierty from the Gironde region, in France. It was widely planted in Bordeaux until the Phylloxera crisis but nearly disappeared since. Carménère has built a new reputation in Chile, where it was at first mistaken for Merlot. If harvested before being fully ripe, Carménère produces wines which are are in pyrazine (herbaceous, green bell pepper aromas). When made from fully ripe grapes, the wines are full bodied and display aromas of black and blue fruits, chocolate and soy sauce. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Carricante",
-        "synonyms": ["Catanese Bianco"],
-        "description": "Potentially very fine, crisp and distinctive Sicilian white variety.",
-        "color": "white",
+        "synonyms": [
+            "Catanese Bianco"
+        ],
+        "description": {
+            "default": "Potentially very fine, crisp and distinctive Sicilian white variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cascarolo Bianco",
-        "synonyms": ["Cascarala", "Cascarecul", "Cascarelbo"],
-        "description": "Ancient and barely surviving white variety from Piemonte.",
-        "color": "white",
+        "synonyms": [
+            "Cascarala",
+            "Cascarecul",
+            "Cascarelbo"
+        ],
+        "description": {
+            "default": "Ancient and barely surviving white variety from Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Casculho",
-        "synonyms": ["Cascudo"],
-        "description": "Minor northern Portuguese variety generally found in blends.",
-        "color": "black",
+        "synonyms": [
+            "Cascudo"
+        ],
+        "description": {
+            "default": "Minor northern Portuguese variety generally found in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Casetta",
-        "synonyms": ["Lambrusco a Foglia Tonda", "Lambrusco Casetta", "Maranela"],
-        "description": "Northern Italian dark-skinned variety snatched from the jaws of extinction and making highly structured and distinctive wines.",
-        "color": "black",
+        "synonyms": [
+            "Lambrusco a Foglia Tonda",
+            "Lambrusco Casetta",
+            "Maranela"
+        ],
+        "description": {
+            "default": "Northern Italian dark-skinned variety snatched from the jaws of extinction and making highly structured and distinctive wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Castagnara",
-        "synonyms": ["Santa Maria Nera", "Sarnese"],
-        "description": "Low-acid Italian red wine variety improved by blending.",
-        "color": "black",
+        "synonyms": [
+            "Santa Maria Nera",
+            "Sarnese"
+        ],
+        "description": {
+            "default": "Low-acid Italian red wine variety improved by blending.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Castelão",
         "synonyms": [
             "Bastardo Castico",
             "Bastardo Espanhol",
             "Castelão Francês",
             "Castellao Portugues",
             "Castico",
             "João Santarém",
             "João de Santarém",
             "Periquita",
             "Piriquita",
-            "Piriquito",
+            "Piriquito"
         ],
-        "description": "Portugal’s most common variety: hardy, adaptable and widely grown under many different aliases.",
-        "color": "black",
+        "description": {
+            "default": "Portugal’s most common variety: hardy, adaptable and widely grown under many different aliases.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Castets",
-        "synonyms": ["Engrunat", "Machouquet", "Nicouleau"],
-        "description": "Very minor western Pyreneen variety clinging on in France; a parent in Slovakia.",
-        "color": "black",
+        "synonyms": [
+            "Engrunat",
+            "Machouquet",
+            "Nicouleau"
+        ],
+        "description": {
+            "default": "Very minor western Pyreneen variety clinging on in France; a parent in Slovakia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Castiglione",
         "synonyms": [
             "Castigliono",
             "Mantonico Nero",
             "Marchesana",
             "Zagarese",
-            "Zagarolese",
+            "Zagarolese"
         ],
-        "description": "Dark-skinned Italian variety almost exclusive to Calabria and usually blended.",
-        "color": "black",
+        "description": {
+            "default": "Dark-skinned Italian variety almost exclusive to Calabria and usually blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Catalanesca",
-        "synonyms": ["Catalana", "Uva Catalana"],
-        "description": "Very old, high-acid white Italian variety suited to both table and glass and exclusive to Campania.",
-        "color": "white",
+        "synonyms": [
+            "Catalana",
+            "Uva Catalana"
+        ],
+        "description": {
+            "default": "Very old, high-acid white Italian variety suited to both table and glass and exclusive to Campania.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Catanese Nero",
-        "synonyms": ["Vesparola"],
-        "description": "Minor Sicilian red variety.",
-        "color": "black",
+        "synonyms": [
+            "Vesparola"
+        ],
+        "description": {
+            "default": "Minor Sicilian red variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Catarratto Bianco",
         "synonyms": [
             "Catarratteddu",
             "Catarratto Bertolaro",
             "Catarratto Bianco Comune",
             "Catarratto Bianco Lucido",
             "Catarratto Bianco Lucido Serrato",
             "Catarratto Corteddaro",
             "Catarratto Latino",
-            "Catarrattu Lu Nostrum.",
+            "Catarrattu Lu Nostrum."
         ],
-        "description": "Widely planted and variously named Sicilian white with potential for quality in the right hands.",
-        "color": "white",
+        "description": {
+            "default": "Widely planted and variously named Sicilian white with potential for quality in the right hands.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Catawba",
         "synonyms": [
             "Arkansas",
             "Catawba Rosa",
             "Cherokee",
@@ -2066,29 +3321,37 @@
             "Michigan",
             "Munipale Red",
             "Omega",
             "Rose of Tennessee",
             "Saratoga",
             "Singleton",
             "Tekomah",
-            "Tokay",
+            "Tokay"
         ],
-        "description": "Historically important American or part-American variety that was very popular in the nineteenth century but ripens inconveniently late and is now in decline.",
-        "color": "red",
+        "description": {
+            "default": "Historically important American or part-American variety that was very popular in the nineteenth century but ripens inconveniently late and is now in decline.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Cavrara",
         "synonyms": [
             "Bassanese dal Peduncolo Rosso",
             "Caprara",
             "Cavarada",
-            "Cavarara",
+            "Cavarara"
         ],
-        "description": "Virtually extinct red of the Veneto.",
-        "color": "black",
+        "description": {
+            "default": "Virtually extinct red of the Veneto.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Çavuş",
         "synonyms": [
             "Čauš Beli",
             "Čauš Bijeli",
             "Ceaus Alb",
@@ -2096,18 +3359,22 @@
             "Damascenka",
             "Feher Tökszölö",
             "Panse de Constantinople",
             "Parc de Versailles",
             "Tchaouch",
             "Tsaousi",
             "Tsaoussi",
-            "Turceasca",
+            "Turceasca"
         ],
-        "description": "Eastern table grape showing potential for citrus-flavoured wines in Turkey and Greece.",
-        "color": "white",
+        "description": {
+            "default": "Eastern table grape showing potential for citrus-flavoured wines in Turkey and Greece.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cayetana Blanca",
         "synonyms": [
             "Amor Blanco",
             "Aujubi",
             "Baladi",
@@ -2163,108 +3430,184 @@
             "Padero",
             "Parda",
             "Pardina",
             "Pirulet",
             "Plateadillo",
             "Robal",
             "Sarigo",
-            "Tierra de Barros",
+            "Tierra de Barros"
         ],
-        "description": "Lesser-quality Iberian variety known in Portugal as Mourisco Branco but more common in Spain under various synonyms.",
-        "color": "white",
+        "description": {
+            "default": "Lesser-quality Iberian variety known in Portugal as Mourisco Branco but more common in Spain under various synonyms.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cayuga White",
-        "synonyms": ["Geneva White 3", "GW 3", "New York 33403", "NY 33403"],
-        "description": "Versatile New York hybrid.",
-        "color": "white",
+        "synonyms": [
+            "Geneva White 3",
+            "GW 3",
+            "New York 33403",
+            "NY 33403"
+        ],
+        "description": {
+            "default": "Versatile New York hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Centesimino",
-        "synonyms": ["Alicante del Faentino", "Savignon Rosso", "Savignôn Rosso"],
-        "description": "Red variety resurrected in a garden in Emilia-Romagna in the mid twentieth century.",
-        "color": "black",
+        "synonyms": [
+            "Alicante del Faentino",
+            "Savignon Rosso",
+            "Savignôn Rosso"
+        ],
+        "description": {
+            "default": "Red variety resurrected in a garden in Emilia-Romagna in the mid twentieth century.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Centurian",
-        "synonyms": ["Centurion"],
-        "description": "California cross as unsuccessful as its sibling Carnelian.",
-        "color": "black",
+        "synonyms": [
+            "Centurion"
+        ],
+        "description": {
+            "default": "California cross as unsuccessful as its sibling Carnelian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cerceal Branco",
-        "synonyms": ["Cercial", "Cercial do Douro"],
-        "description": "Fresh Douro variety not to be confused with Madeira’s Sercial.",
-        "color": "white",
+        "synonyms": [
+            "Cercial",
+            "Cercial do Douro"
+        ],
+        "description": {
+            "default": "Fresh Douro variety not to be confused with Madeira’s Sercial.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cesanese",
         "synonyms": [
             "Bonvino Nero",
             "Cesanese Comune",
             "Cesanese di Affile",
             "Cesanese Nostrano",
             "Nero Ferrigno",
             "Sanguinella",
-            "Uva di Affile",
+            "Uva di Affile"
         ],
-        "description": "Lazio’s prime red wine grape, aromatic and difficult to ripen.",
-        "color": "black",
+        "description": {
+            "default": "Lazio’s prime red wine grape, aromatic and difficult to ripen.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "César",
-        "synonyms": ["Céear", "Céelar", "Célar", "Picarniau", "Romain", "Römer"],
-        "description": "Tannic variety playing a very minor and local role in northern Burgundy.",
-        "color": "black",
+        "synonyms": [
+            "Céear",
+            "Céelar",
+            "Célar",
+            "Picarniau",
+            "Romain",
+            "Römer"
+        ],
+        "description": {
+            "default": "Tannic variety playing a very minor and local role in northern Burgundy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cetinka",
         "synonyms": [
             "Blajka",
             "Blatinka",
             "Blatka",
             "Blatska",
             "Cetinjka",
             "Cetinjka Bijela",
             "Cetinka Bijela",
             "Poserača",
-            "Potomkinja",
+            "Potomkinja"
         ],
-        "description": "Extremely rare Croatian island white.",
-        "color": "white",
+        "description": {
+            "default": "Extremely rare Croatian island white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cevat Kara",
         "synonyms": [
             "Djevat Kara",
             "Dshevat-Kara",
             "Dzhevat Kara",
             "Jewath",
-            "Polkovnik Kara",
+            "Polkovnik Kara"
         ],
-        "description": "Southern Ukrainian variety used in fortified blends.",
-        "color": "black",
+        "description": {
+            "default": "Southern Ukrainian variety used in fortified blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chambourcin",
-        "synonyms": ["Joannes Seyve 26-205"],
-        "description": "French humidity-tolerant hybrid popular in the US and Australia but on the decline in its homeland.",
-        "color": "black",
+        "synonyms": [
+            "Joannes Seyve 26-205"
+        ],
+        "description": {
+            "default": "French humidity-tolerant hybrid popular in the US and Australia but on the decline in its homeland.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chancellor",
-        "synonyms": ["Seibel 7053"],
-        "description": "Minor French-American hybrid now more widely planted in North America than in France.",
-        "color": "black",
+        "synonyms": [
+            "Seibel 7053"
+        ],
+        "description": {
+            "default": "Minor French-American hybrid now more widely planted in North America than in France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chardonel",
-        "synonyms": ["GW 9", "NY 45010"],
-        "description": "New York hybrid that is more hardy and productive than its Chardonnay parent, adopted in some northern US states.",
-        "color": "white",
+        "synonyms": [
+            "GW 9",
+            "NY 45010"
+        ],
+        "description": {
+            "default": "New York hybrid that is more hardy and productive than its Chardonnay parent, adopted in some northern US states.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Chardonnay",
         "synonyms": [
             "Aubaine",
             "Auvernat",
             "Auxerrois",
@@ -2276,30 +3619,46 @@
             "Gamay Blanc",
             "Luisant",
             "Melon à Queue Rouge",
             "Melon d’Arbois",
             "Obaideh",
             "Pinot Blanc Chardonnay",
             "Wais Edler",
-            "Waiser Clevner",
+            "Waiser Clevner"
         ],
-        "description": "Hugely popular, versatile and widely planted international white variety equally capable of extreme mediocrity and regal splendour.",
-        "color": "white",
+        "description": {
+            "default": "Hugely popular, versatile and widely planted international white variety equally capable of extreme mediocrity and regal splendour.",
+            "julie": "",
+            "sommelier": "A multifaceted grape varieties highly influenced by where it is grown and how it is made into wine. From racy, lean and citrucy to creamy, buttery and tropical, its personality is full of surprises."
+        },
+        "color": "white"
     },
     {
         "name": "Charentsi",
-        "synonyms": ["Charentzi"],
-        "description": "Cold-hardy Armenian hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Charentzi"
+        ],
+        "description": {
+            "default": "Cold-hardy Armenian hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chasan",
-        "synonyms": ["INRA 1527-78"],
-        "description": "Low-acid French cross grown mainly in the Languedoc.",
-        "color": "white",
+        "synonyms": [
+            "INRA 1527-78"
+        ],
+        "description": {
+            "default": "Low-acid French cross grown mainly in the Languedoc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Chasselas",
         "synonyms": [
             "Amber Chasselas",
             "Bar-sur-Aube",
             "Bassiraube",
@@ -2362,18 +3721,22 @@
             "Temprana Tardía",
             "Tempranillo de Nav",
             "Temprano",
             "Temprano Blanco",
             "Viviser",
             "Wälsche",
             "Weisser Gutedel",
-            "Weisser Krachgutedel",
+            "Weisser Krachgutedel"
         ],
-        "description": "French Switzerland’s characteristic variety producing soft, occasionally distinguished but often pretty ordinary, whites. Widely grown for juice and the table.",
-        "color": "white",
+        "description": {
+            "default": "French Switzerland’s characteristic variety producing soft, occasionally distinguished but often pretty ordinary, whites. Widely grown for juice and the table.",
+            "julie": "",
+            "sommelier": "The Chasselas is the typical white vine variety of French-speaking Switzerland and the identity of Switzerland wine culture. It makes a fruity, fresh and delicate wine. The Chasselas is marvellously advisable for the aperitif and in the accompaniment of meals. To eat cheese fondue, raclette, vacherin Mont-d’Or cheese, trout, fera or fillets of perch without Chasselas is unthinkable. According to regions it can be fruity, floral, slightly mild. In great vintages, after five or ten years, it has aromas of honey, scents of walnut and a smooth texture which give it a remarkable personality. Despite its low natural acidity, Chasselas can acquire, with aging, aromas of honey, elderflower, chamomile, with a creamy texture, almost oily, as opposed to the friskiness of its youth with notes of white flowers, flint , butter or lemon. Swiss pairings : Lake fish, fish with white flesh, fondue, raclette, cheese crust dishes, vacherin Mont-d’Or, Malakoff cheese, Vully green asparagus or when catching a trout from one of the Swiss Lakes on August 1st for the National Day."
+        },
+        "color": "white"
     },
     {
         "name": "Chatus",
         "synonyms": [
             "Bolgnino",
             "Bourgnin",
             "Brachet",
@@ -2395,24 +3758,34 @@
             "Nebbiolo Pairolè",
             "Neiret",
             "Neiret Pinerolese",
             "Neretto",
             "Ouron",
             "Houron",
             "Persagne-Gamay",
-            "Scarlattin",
+            "Scarlattin"
         ],
-        "description": "Ancient, rare tannic Ardèche variety also found in Piemonte.",
-        "color": "black",
+        "description": {
+            "default": "Ancient, rare tannic Ardèche variety also found in Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chelois",
-        "synonyms": ["Seibel 10878"],
-        "description": "French-American hybrid found in Canada and the north-eastern US; wine is rather rustic on its own.",
-        "color": "black",
+        "synonyms": [
+            "Seibel 10878"
+        ],
+        "description": {
+            "default": "French-American hybrid found in Canada and the north-eastern US; wine is rather rustic on its own.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chelva",
         "synonyms": [
             "Chelva de Cebreros",
             "Chelva de Guareña",
             "Eva",
@@ -2423,24 +3796,34 @@
             "Mantúo de Pilas",
             "Montúa",
             "Montúo de Villanueva",
             "Montúo Gordo",
             "Uva Rey",
             "Uva del Rey",
             "Uva de Puerto Real",
-            "Villanueva",
+            "Villanueva"
         ],
-        "description": "Spanish variety more popular for the table than for wine.",
-        "color": "white",
+        "description": {
+            "default": "Spanish variety more popular for the table than for wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Chenanson",
-        "synonyms": ["Chenançon"],
-        "description": "Montpellier cross planted to a limited extent around the Mediterranean.",
-        "color": "black",
+        "synonyms": [
+            "Chenançon"
+        ],
+        "description": {
+            "default": "Montpellier cross planted to a limited extent around the Mediterranean.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chenin Blanc",
         "synonyms": [
             "Agudelo",
             "Agudillo",
             "Anjou",
@@ -2451,88 +3834,140 @@
             "Gros Pineau",
             "Pineau d’Anjou",
             "Pineau de la Loire",
             "Plant d’Anjou",
             "Ronchalin",
             "Rouchelein",
             "Rouchelin",
-            "Steen",
+            "Steen"
         ],
-        "description": "Loire, and South African, speciality making crisp, sometimes long-lived, wines with varying degrees of sweetness that deserve more recognition.",
-        "color": "white",
+        "description": {
+            "default": "Loire, and South African, speciality making crisp, sometimes long-lived, wines with varying degrees of sweetness that deserve more recognition.",
+            "julie": "Chenin blanc is mostly planted into two areas : France's Loire Valley and South Africa. In the Loire Valley it produces a multitude of styles - sparkling wines, dry, off-dry and sweet wines. Chenin blanc is a very versatile grape variety highly influences by the soil it grows on. Aromatically, it can displays aromas of white flowers, quince, stone fruits and honey. South Africa has the most plantings of Chenin Blanc in the world and the styles and quality of the wines produced with the grapes can varry greatly too. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Chichaud",
-        "synonyms": ["Brunet", "Tsintsào"],
-        "description": "Ardèche variety that can still, just, be found in southern France.",
-        "color": "black",
+        "synonyms": [
+            "Brunet",
+            "Tsintsào"
+        ],
+        "description": {
+            "default": "Ardèche variety that can still, just, be found in southern France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chidiriotiko",
-        "synonyms": ["Kalloniatiko"],
-        "description": "Greek variety revived by one producer on the island of Lésvos (Lesbos).",
-        "color": "black",
+        "synonyms": [
+            "Kalloniatiko"
+        ],
+        "description": {
+            "default": "Greek variety revived by one producer on the island of Lésvos (Lesbos).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chinuri",
-        "synonyms": ["Chinabuli", "Kaspura", "Kaspuri Tetri", "Okroula", "Tchinouri"],
-        "description": "High-acid Georgian variety used for both still and sparkling wines.",
-        "color": "white",
+        "synonyms": [
+            "Chinabuli",
+            "Kaspura",
+            "Kaspuri Tetri",
+            "Okroula",
+            "Tchinouri"
+        ],
+        "description": {
+            "default": "High-acid Georgian variety used for both still and sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Chkhaveri",
-        "synonyms": ["Tchkhaveri", "Vanis Chkhaveri"],
-        "description": "Minor but versatile pink-skinned Georgian variety.",
-        "color": "pink",
+        "synonyms": [
+            "Tchkhaveri",
+            "Vanis Chkhaveri"
+        ],
+        "description": {
+            "default": "Minor but versatile pink-skinned Georgian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Chondromavro",
         "synonyms": [
             "Chondromavrouda",
             "Chondromavroudi",
             "Chondromavroudo",
-            "Khondromavroud",
+            "Khondromavroud"
         ],
-        "description": "Very rare Greek variety planted in Makedonía.",
-        "color": "black",
+        "description": {
+            "default": "Very rare Greek variety planted in Makedonía.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Chouchillon",
-        "synonyms": ["Faux Viognier"],
-        "description": "Light-skinned variety recently rescued in central France.",
-        "color": "white",
+        "synonyms": [
+            "Faux Viognier"
+        ],
+        "description": {
+            "default": "Light-skinned variety recently rescued in central France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cianorie",
         "synonyms": [
             "Canore",
             "Canorie",
             "Chianorie",
             "Cianoria",
             "Cjanorie",
             "Rossarie",
-            "Vinosa",
+            "Vinosa"
         ],
-        "description": "Old and very minor dark-skinned variety from Friuli, north-east Italy.",
-        "color": "black",
+        "description": {
+            "default": "Old and very minor dark-skinned variety from Friuli, north-east Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ciliegiolo",
         "synonyms": [
             "Albana Nera",
             "Brunellone",
             "Canaiolo Romano",
             "Ciliegino",
             "Ciliegiolo di Spagna",
             "Mazzèse",
             "Riminese Nero",
-            "Sangiovese Polveroso",
+            "Sangiovese Polveroso"
         ],
-        "description": "Cherry-flavoured Italian red with untapped potential, especially in Toscana. Parent of Sangiovese.",
-        "color": "black",
+        "description": {
+            "default": "Cherry-flavoured Italian red with untapped potential, especially in Toscana. Parent of Sangiovese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cinsaut",
         "synonyms": [
             "Black Malvoisie",
             "Black Prince",
             "Blue Imperial",
@@ -2549,30 +3984,47 @@
             "Piquepoul d’Uzès",
             "Prunelat",
             "Prunellas",
             "Samsó",
             "Sinsó",
             "Sinsón",
             "Sinseur",
-            "Uva Spina",
+            "Uva Spina"
         ],
-        "description": "Underrated Mediterranean-loving variety making characterful rosés and flirtatious reds.",
-        "color": "black",
+        "description": {
+            "default": "Underrated Mediterranean-loving variety making characterful rosés and flirtatious reds.",
+            "julie": "Cinsault thrives in mediterranean climates and produces red wines that are soft, elegant, fruity and aromatic as well as fersh and perfumed rosé wines.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ciurlese",
-        "synonyms": ["Ciurlès"],
-        "description": "Virtually extinct white from around Rimini in northern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Ciurlès"
+        ],
+        "description": {
+            "default": "Virtually extinct white from around Rimini in northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Cividin",
-        "synonyms": ["Cividin Bianco", "Cividino"],
-        "description": "Ancient, rare white from Friuli, north-east Italy.",
-        "color": "white",
+        "synonyms": [
+            "Cividin Bianco",
+            "Cividino"
+        ],
+        "description": {
+            "default": "Ancient, rare white from Friuli, north-east Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Clairette",
         "synonyms": [
             "Blanc Laffite",
             "Blanquette",
             "Clairet",
@@ -2584,114 +4036,195 @@
             "Muscade",
             "Oeillade Blanche",
             "Osianka",
             "Ovsyanka",
             "Petit Blanc",
             "Petit Kleret",
             "Uva Gijona",
-            "Vivsyanka",
+            "Vivsyanka"
         ],
-        "description": "Once very popular and now useful, crisp southern French white.",
-        "color": "white",
+        "description": {
+            "default": "Once very popular and now useful, crisp southern French white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Claverie",
         "synonyms": [
             "Bouguieu",
             "Chalosse Blanche",
             "Chaloussenc",
             "Clabarien",
             "Clabérieu",
             "Claverie Blanc",
             "Claverie Verte",
-            "Galia Zuria",
+            "Galia Zuria"
         ],
-        "description": "Virtually extinct, disease-prone white from south-west France.",
-        "color": "white",
+        "description": {
+            "default": "Virtually extinct, disease-prone white from south-west France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Clinton",
         "synonyms": [
             "Bacchus",
             "Clinton Rose",
             "Klinton",
             "Plant des Carmes",
             "Plant Pouzin",
             "Vorthington",
             "Worthington",
-            "Zephirin",
+            "Zephirin"
         ],
-        "description": "Pre-Civil War natural American hybrid of historical interest only.",
-        "color": "black",
+        "description": {
+            "default": "Pre-Civil War natural American hybrid of historical interest only.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cococciola",
-        "synonyms": ["Cacciola", "Cocacciara"],
-        "description": "Fruity, herbal white from Abruzzo and Puglia.",
-        "color": "white",
+        "synonyms": [
+            "Cacciola",
+            "Cocacciara"
+        ],
+        "description": {
+            "default": "Fruity, herbal white from Abruzzo and Puglia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Coda Di Cavallo Bianca",
-        "synonyms": ["Cavalla", "Codacavallo", "Latina"],
-        "description": "Barely cultivated and generally blended white variety from Campania, southern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Cavalla",
+            "Codacavallo",
+            "Latina"
+        ],
+        "description": {
+            "default": "Barely cultivated and generally blended white variety from Campania, southern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Coda Di Volpe Bianca",
-        "synonyms": ["Durante", "Falerno", "Guarnaccia Bianca"],
-        "description": "Ancient, full-bodied white from southern Italy coming into its own as a varietal wine.",
-        "color": "white",
+        "synonyms": [
+            "Durante",
+            "Falerno",
+            "Guarnaccia Bianca"
+        ],
+        "description": {
+            "default": "Ancient, full-bodied white from southern Italy coming into its own as a varietal wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Côdega De Larinho",
-        "synonyms": ["Côdega do Larinho"],
-        "description": "Very fruity but soft variety from north-east Portugal.",
-        "color": "white",
+        "synonyms": [
+            "Côdega do Larinho"
+        ],
+        "description": {
+            "default": "Very fruity but soft variety from north-east Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Codivarta",
-        "synonyms": ["Codivarte Blanc", "Codivertola Blanc", "Cudiverta"],
-        "description": "Soft northern Corsican.",
-        "color": "white",
+        "synonyms": [
+            "Codivarte Blanc",
+            "Codivertola Blanc",
+            "Cudiverta"
+        ],
+        "description": {
+            "default": "Soft northern Corsican.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Colobel",
-        "synonyms": ["Seibel 8357"],
-        "description": "Almost extinct French hybrid that can make very dark but astringent reds.",
-        "color": "black",
+        "synonyms": [
+            "Seibel 8357"
+        ],
+        "description": {
+            "default": "Almost extinct French hybrid that can make very dark but astringent reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Colombard",
         "synonyms": [
             "Colombar",
             "Colombier",
             "French Colombard",
             "Queue Tendre",
-            "Tourterelle",
+            "Tourterelle"
         ],
-        "description": "Productive workhorse variety now more valued for easy-drinking blended whites than for brandy.",
-        "color": "white",
+        "description": {
+            "default": "Productive workhorse variety now more valued for easy-drinking blended whites than for brandy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Colombaud",
-        "synonyms": ["Aubié", "Colombaud du Var"],
-        "description": "Ancient but virtually extinct white related to the Swiss variety Humagne.",
-        "color": "white",
+        "synonyms": [
+            "Aubié",
+            "Colombaud du Var"
+        ],
+        "description": {
+            "default": "Ancient but virtually extinct white related to the Swiss variety Humagne.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Colorino Del Valdarno",
-        "synonyms": ["Colore", "Colorino"],
-        "description": "Rare, dark-skinned Tuscan variety often confused with others called Colorino Something and especially useful for adding colour to blends.",
-        "color": "black",
+        "synonyms": [
+            "Colore",
+            "Colorino"
+        ],
+        "description": {
+            "default": "Rare, dark-skinned Tuscan variety often confused with others called Colorino Something and especially useful for adding colour to blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Completer",
-        "synonyms": ["Lindauer", "Malanstraube", "Zürirebe"],
-        "description": "Rare Swiss variety making very distinctive, ageworthy whites.",
-        "color": "white",
+        "synonyms": [
+            "Lindauer",
+            "Malanstraube",
+            "Zürirebe"
+        ],
+        "description": {
+            "default": "Rare Swiss variety making very distinctive, ageworthy whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Concord",
         "synonyms": [
             "Bergerac",
             "Bull’s Seedling",
             "Corin",
@@ -2703,87 +4236,137 @@
             "Gorin",
             "Gurin",
             "Kek Olasz",
             "Konkordi",
             "Konkordia",
             "Nyarfalevelue",
             "Nyarlevelue",
-            "Olasz Kek",
+            "Olasz Kek"
         ],
-        "description": "America’s own grape. Winter-hardy, Massachusetts hybrid planted more for jelly and juice than for wine.",
-        "color": "black",
+        "description": {
+            "default": "America’s own grape. Winter-hardy, Massachusetts hybrid planted more for jelly and juice than for wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cordenossa",
-        "synonyms": ["Cordenos"],
-        "description": "Recently rescued and still rare Friulian red.",
-        "color": "black",
+        "synonyms": [
+            "Cordenos"
+        ],
+        "description": {
+            "default": "Recently rescued and still rare Friulian red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cornalin",
         "synonyms": [
             "Broblanc",
             "Cargnola",
             "Cornalin d’Aoste",
             "Cornalino",
             "Cornallin",
             "Corniola",
-            "Humagne Rouge",
+            "Humagne Rouge"
         ],
-        "description": "Ancient red from the Valle d’Aosta in northern Italy, widespread in the Valais in Switzerland as Humagne Rouge.",
-        "color": "black",
+        "description": {
+            "default": "Ancient red from the Valle d’Aosta in northern Italy, widespread in the Valais in Switzerland as Humagne Rouge.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cornarea",
-        "synonyms": ["Incrocio Dalmasso IV/28"],
-        "description": "Obscure dark-skinned Italian cross whose true parentage has only recently been revealed.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso IV/28"
+        ],
+        "description": {
+            "default": "Obscure dark-skinned Italian cross whose true parentage has only recently been revealed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cornifesto",
         "synonyms": [
             "Cornifeito",
             "Cornifesta",
             "Cornifesto no Dao",
             "Cornifesto Tinto",
             "Cornifresco",
-            "Tinta Bastardeira",
+            "Tinta Bastardeira"
         ],
-        "description": "Minor Douro variety used for both port and unfortified wines.",
-        "color": "black",
+        "description": {
+            "default": "Minor Douro variety used for both port and unfortified wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Corot Noir",
-        "synonyms": ["NY 70.0809.10"],
-        "description": "Minor hybrid bred in upstate New York for the eastern US.",
-        "color": "black",
+        "synonyms": [
+            "NY 70.0809.10"
+        ],
+        "description": {
+            "default": "Minor hybrid bred in upstate New York for the eastern US.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cortese",
-        "synonyms": ["Corteis", "Courteis", "Courtesia"],
-        "description": "Generally rather bland northern-Italian white that shows its best varietal face in Gavi.",
-        "color": "white",
+        "synonyms": [
+            "Corteis",
+            "Courteis",
+            "Courtesia"
+        ],
+        "description": {
+            "default": "Generally rather bland northern-Italian white that shows its best varietal face in Gavi.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Corvina Veronese",
         "synonyms": [
             "Corvina Comune",
             "Corvina Gentile",
             "Corvina Nostrana",
             "Corvina Reale",
             "Cruina",
+            "Corvina"
         ],
-        "description": "Bright, fresh, cherry-scented red encountered most often in Valpolicella and Bardolino.",
-        "color": "black",
+        "description": {
+            "default": "Bright, fresh, cherry-scented red encountered most often in Valpolicella and Bardolino.",
+            "julie": "Corvina is a grape variety found in the Veneto region of Italy and which is typically blended with Rondinella and Molinara to producer Valpolicella, Bardolino and Amarone wines. When not blended, Corvina gives wines which are light-bodied, with fresh acidity, moderate tannins and sour cherry flavours. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Corvinone",
-        "synonyms": ["Corvinon", "Cruinon"],
-        "description": "A dark-skinned variety with fresh acidity that contributes to Veneto blends.",
-        "color": "black",
+        "synonyms": [
+            "Corvinon",
+            "Cruinon"
+        ],
+        "description": {
+            "default": "A dark-skinned variety with fresh acidity that contributes to Veneto blends.",
+            "julie": "Corvinone is a red grape variety, with bright acidity, that contributes to blends in the region of Veneto. It can replace a percentage of the Corvina grape for Valpolicella and Amaron wines.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Cot",
         "synonyms": [
             "Agreste",
             "Auxerrois",
             "Bouyssales",
@@ -2803,110 +4386,165 @@
             "Malbech",
             "Mancin",
             "Nuar de Presac",
             "Pied de Perdrix",
             "Pressac",
             "Noir de Pressac",
             "Prunelat",
-            "Quercy",
+            "Quercy"
         ],
-        "description": "Makes dark, flavoursome, well-structured reds more celebrated as Argentine Malbec than in its home Cahors.",
-        "color": "black",
+        "description": {
+            "default": "Makes dark, flavoursome, well-structured reds more celebrated as Argentine Malbec than in its home Cahors.",
+            "julie": "Better known as Malbec, Cot is originally from the region of Cahors in Southwest France. Today, modern Cahors can be incredible pure, bright and mineral balancing structure and fruit yumminess. The biggest success of Malbec however, resides in Argentina, especially in the region of Mendoza where Malbec has become a super-star variety. There, the wines produces are full-bodied, smooth and packed with blue fruits and spiciness. The grape particularly stives in the high alitude vineyards of sub-regions such as the Uco Valley where it can express more elegance and minerality. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Couderc Noir",
-        "synonyms": ["Contassot 20", "Couderc 7120", "Plant Verni"],
-        "description": "Undistinguished French hybrid with few remaining fans.",
-        "color": "black",
+        "synonyms": [
+            "Contassot 20",
+            "Couderc 7120",
+            "Plant Verni"
+        ],
+        "description": {
+            "default": "Undistinguished French hybrid with few remaining fans.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Counoise",
         "synonyms": [
             "Coneze",
             "Connoges",
             "Connoise",
             "Counèse",
             "Counoïse",
             "Counoïso",
             "Counoueiso",
             "Guénoise",
             "Quenoise",
-            "Rivier",
+            "Rivier"
         ],
-        "description": "Minor but valued southern Rhône ingredient, occasional varietal.",
-        "color": "black",
+        "description": {
+            "default": "Minor but valued southern Rhône ingredient, occasional varietal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Courbu Blanc",
         "synonyms": [
             "Courbeau",
             "Courbi",
             "Courbis Blanc",
             "Courbu",
             "Courbut Blanc",
             "Courtoisie",
-            "Vieux Pacherenc",
+            "Vieux Pacherenc"
         ],
-        "description": "Minor variety often consorting with the Mansengs in French Basque Country.",
-        "color": "white",
+        "description": {
+            "default": "Minor variety often consorting with the Mansengs in French Basque Country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Courbu Noir",
-        "synonyms": ["Courbu Rouge", "Courbut", "Dolceolo", "Noir du Pays"],
-        "description": "Virtually extinct speciality of Béarn, south-west France, unrelated to Courbu Blanc.",
-        "color": "black",
+        "synonyms": [
+            "Courbu Rouge",
+            "Courbut",
+            "Dolceolo",
+            "Noir du Pays"
+        ],
+        "description": {
+            "default": "Virtually extinct speciality of Béarn, south-west France, unrelated to Courbu Blanc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Crâmpoșie Selecţionată",
-        "synonyms": ["Crîmpoșie Selecţionată"],
-        "description": "High-quality, high-acid Romanian variety producing zesty, mineral-laden whites.",
-        "color": "white",
+        "synonyms": [
+            "Crîmpoșie Selecţionată"
+        ],
+        "description": {
+            "default": "High-quality, high-acid Romanian variety producing zesty, mineral-laden whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Criolla Grande",
-        "synonyms": ["Criolla Grande Sanjuanina"],
-        "description": "Declining but still very widely planted Argentine pink-skinned variety making humdrum wine.",
-        "color": "red",
+        "synonyms": [
+            "Criolla Grande Sanjuanina"
+        ],
+        "description": {
+            "default": "Declining but still very widely planted Argentine pink-skinned variety making humdrum wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Croatina",
         "synonyms": [
             "Bonarda",
             "Bonarda di Rovescala",
             "Crovattina",
             "Nebbiolo di Gattinara",
             "Neretto",
             "Spanna-Nebbiolo",
             "Uga del Zio",
-            "Uva Vermiglia",
+            "Uva Vermiglia"
         ],
-        "description": "A fruity dark-skinned variety grown in many different areas of northern Italy and used both solo and in blends.",
-        "color": "black",
+        "description": {
+            "default": "A fruity dark-skinned variety grown in many different areas of northern Italy and used both solo and in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Crouchen",
         "synonyms": [
             "Cape Riesling",
             "Clare Riesling",
             "Cougnet",
             "Cruchen Blanc",
             "Cruchenta",
             "Messanges Blanc",
             "Paarl Riesling",
             "Sable Blanc",
-            "Trouchet Blanc",
+            "Trouchet Blanc"
         ],
-        "description": "Widely travelled neutral French variety from the western Pyrenees that for long benefited from naming confusion.",
-        "color": "white",
+        "description": {
+            "default": "Widely travelled neutral French variety from the western Pyrenees that for long benefited from naming confusion.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Crovassa",
-        "synonyms": ["Croassa"],
-        "description": "Very minor red variety in the Valle d’Aosta.",
-        "color": "black",
+        "synonyms": [
+            "Croassa"
+        ],
+        "description": {
+            "default": "Very minor red variety in the Valle d’Aosta.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Csaba Gyöngye",
         "synonyms": [
             "Cabski Biser",
             "Csabagyöngye",
             "Julski Muskat",
@@ -2914,138 +4552,243 @@
             "Perl do Saba",
             "Perla Czabanska",
             "Perla di Csaba",
             "Perle de Csaba",
             "Perle von Csaba",
             "Rindunicaz Strugurilor",
             "Vengerskii Muskatnii Rannüj",
-            "Zemcug Saba",
+            "Zemcug Saba"
         ],
-        "description": "Hungarian table grape occasionally turned into light, grapey whites.",
-        "color": "white",
+        "description": {
+            "default": "Hungarian table grape occasionally turned into light, grapey whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Csókaszőlő",
         "synonyms": [
             "Csóka Szőlő",
             "Csóka",
             "Fekete Magyarka",
             "Kleinhungar Blauer",
             "Magyarka Neagra",
             "Rácfekete",
-            "Vadfekete",
+            "Vadfekete"
         ],
-        "description": "Old Hungarian variety in the throes of rediscovery.",
-        "color": "black",
+        "description": {
+            "default": "Old Hungarian variety in the throes of rediscovery.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dafni",
-        "synonyms": ["Dafnia", "Daphni", "Daphnia"],
-        "description": "Distinctively laurel-scented variety from Kríti (Crete) recently rescued from oblivion.",
-        "color": "white",
+        "synonyms": [
+            "Dafnia",
+            "Daphni",
+            "Daphnia"
+        ],
+        "description": {
+            "default": "Distinctively laurel-scented variety from Kríti (Crete) recently rescued from oblivion.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dakapo",
-        "synonyms": ["Geisenheim 7225-8"],
-        "description": "Red-fleshed German cross adds colour to blends.",
-        "color": "black",
+        "synonyms": [
+            "Geisenheim 7225-8"
+        ],
+        "description": {
+            "default": "Red-fleshed German cross adds colour to blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dalkauer",
-        "synonyms": ["Beutelrebe"],
-        "description": "Rare German offspring of Riesling and A N Other.",
-        "color": "white",
+        "synonyms": [
+            "Beutelrebe"
+        ],
+        "description": {
+            "default": "Rare German offspring of Riesling and A N Other.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Damaschino",
         "synonyms": [
             "Alicante Branco",
             "Beldi",
             "Damaschena",
             "Farana  orFaranah",
             "Farranah",
             "Mayorquin",
             "Planta Fina",
             "Planta Fina de Pedralba",
-            "Planta Pedralba",
+            "Planta Pedralba"
         ],
-        "description": "Ancient but neutral white included in blends around the Mediterranean and in Portugal.",
-        "color": "white",
+        "description": {
+            "default": "Ancient but neutral white included in blends around the Mediterranean and in Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "De Chaunac",
-        "synonyms": ["Cameo", "Seibel 9549"],
-        "description": "French hybrid now at home in Canada and New York State.",
-        "color": "black",
+        "synonyms": [
+            "Cameo",
+            "Seibel 9549"
+        ],
+        "description": {
+            "default": "French hybrid now at home in Canada and New York State.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Debina",
-        "synonyms": ["Debina Metsovou", "Debina Palea", "Dempina", "Ntempina", "Zítsa"],
-        "description": "Highly localized, high-acid Greek variety making light, fresh and digestible wines.",
-        "color": "white",
+        "synonyms": [
+            "Debina Metsovou",
+            "Debina Palea",
+            "Dempina",
+            "Ntempina",
+            "Zítsa"
+        ],
+        "description": {
+            "default": "Highly localized, high-acid Greek variety making light, fresh and digestible wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Debine E Bardhë",
-        "synonyms": ["Debin"],
-        "description": "Declining Albanian of mysterious origin.",
-        "color": "white",
+        "synonyms": [
+            "Debin"
+        ],
+        "description": {
+            "default": "Declining Albanian of mysterious origin.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Debit",
-        "synonyms": ["Belan", "Čarapar", "Debit Bijeli", "Puljižanac"],
-        "description": "Vine producing alcoholic wine throughout Dalmacija (Dalmatia).",
-        "color": "white",
+        "synonyms": [
+            "Belan",
+            "Čarapar",
+            "Debit Bijeli",
+            "Puljižanac"
+        ],
+        "description": {
+            "default": "Vine producing alcoholic wine throughout Dalmacija (Dalmatia).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Deckrot",
-        "synonyms": ["Freiburg 71-119-39"],
-        "description": "Red-fleshed German cross bred for colour.",
-        "color": "black",
+        "synonyms": [
+            "Freiburg 71-119-39"
+        ],
+        "description": {
+            "default": "Red-fleshed German cross bred for colour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Delaware",
-        "synonyms": ["Delavar", "Heath Grape", "Ladies Choice", "Powell", "Ruff Heath"],
-        "description": "Historic variety of obscure origin once popular in the Midwest and in the eastern US states.",
-        "color": "pink",
+        "synonyms": [
+            "Delavar",
+            "Heath Grape",
+            "Ladies Choice",
+            "Powell",
+            "Ruff Heath"
+        ],
+        "description": {
+            "default": "Historic variety of obscure origin once popular in the Midwest and in the eastern US states.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Delisle",
-        "synonyms": ["ES 7-5-41"],
-        "description": "Very minor, cold-hardy North American hybrid with marked petrol-like aromas.",
-        "color": "white",
+        "synonyms": [
+            "ES 7-5-41"
+        ],
+        "description": {
+            "default": "Very minor, cold-hardy North American hybrid with marked petrol-like aromas.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Devín",
-        "synonyms": ["Děvín", "TCVCB 15/4"],
-        "description": "Slovakian cross producing full-bodied, spicy whites in Slovakia and the Czech Republic.",
-        "color": "white",
+        "synonyms": [
+            "Děvín",
+            "TCVCB 15/4"
+        ],
+        "description": {
+            "default": "Slovakian cross producing full-bodied, spicy whites in Slovakia and the Czech Republic.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Diagalves",
         "synonyms": [
             "Carnal",
             "Dependura",
             "Diego Alves",
             "Diogalves",
             "Fernan Fer",
             "Formosa",
             "Formosa Dourada",
             "Formosa Portalegre",
             "Pendura",
             "Pendura Amarela",
-            "Villanueva",
+            "Villanueva"
         ],
-        "description": "Southern Portuguese variety generally used in blends or eaten fresh.",
-        "color": "white",
+        "description": {
+            "default": "Southern Portuguese variety generally used in blends or eaten fresh.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dimrit",
-        "synonyms": ["Dimlit", "Dimrit Kara", "Dirmit Kara"],
-        "description": "Poor-quality, dark-skinned Turkish variety little used for wine so far.",
-        "color": "black",
+        "synonyms": [
+            "Dimlit",
+            "Dimrit Kara",
+            "Dirmit Kara"
+        ],
+        "description": {
+            "default": "Poor-quality, dark-skinned Turkish variety little used for wine so far.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dimyat",
         "synonyms": [
             "Ahorntraube",
             "Bekaszőlő",
             "Dertonia",
@@ -3058,100 +4801,180 @@
             "Smederevka",
             "Smederevka Bianca",
             "Szemendriai Fehér",
             "Töröklugas",
             "Yapalaki",
             "Zoumiatiko",
             "Zumiatico",
-            "Zumyat",
+            "Zumyat"
         ],
-        "description": "Productive, everyday Bulgarian white.",
-        "color": "white",
+        "description": {
+            "default": "Productive, everyday Bulgarian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dindarella",
-        "synonyms": ["Dindarella Rizza", "Pelada", "Pelara"],
-        "description": "Rare, dark-skinned Veneto variety well suited to dried-grape wine styles.",
-        "color": "black",
+        "synonyms": [
+            "Dindarella Rizza",
+            "Pelada",
+            "Pelara"
+        ],
+        "description": {
+            "default": "Rare, dark-skinned Veneto variety well suited to dried-grape wine styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dišeća Ranina",
-        "synonyms": ["Dišeća Ranina Bijela", "Petrinjska Ranina", "Petrinjska Bijela"],
-        "description": "Rare and very localized Croatian variety from south of Zagreb.",
-        "color": "white",
+        "synonyms": [
+            "Dišeća Ranina Bijela",
+            "Petrinjska Ranina",
+            "Petrinjska Bijela"
+        ],
+        "description": {
+            "default": "Rare and very localized Croatian variety from south of Zagreb.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dobričić",
         "synonyms": [
             "Čihovac",
             "Crljenak Slatinski",
             "Dobričić Crni",
             "Dobrovoljac",
             "Krucalin",
             "Okručanac",
             "Sholtanats",
             "Slatinjac",
-            "Slatinski",
+            "Slatinski"
         ],
-        "description": "Rare Croatian variety high in sugar, rich in colour and used mainly in red blends on the island of Šolta.",
-        "color": "black",
+        "description": {
+            "default": "Rare Croatian variety high in sugar, rich in colour and used mainly in red blends on the island of Šolta.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dolcetto",
-        "synonyms": ["Dolcetto Nero", "Nibièu", "Nibiò", "Ormeasco"],
-        "description": "Deeply coloured, low-acid, fragrant Piemontese red.",
-        "color": "black",
+        "synonyms": [
+            "Dolcetto Nero",
+            "Nibièu",
+            "Nibiò",
+            "Ormeasco"
+        ],
+        "description": {
+            "default": "Deeply coloured, low-acid, fragrant Piemontese red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dolciame",
-        "synonyms": ["Malfiore", "Parlano", "Uva delle Vecchie"],
-        "description": "Virtually extinct Umbrian white.",
-        "color": "white",
+        "synonyms": [
+            "Malfiore",
+            "Parlano",
+            "Uva delle Vecchie"
+        ],
+        "description": {
+            "default": "Virtually extinct Umbrian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Domina",
-        "synonyms": ["Geilweilerhof 4-25-7"],
-        "description": "Modern red German cross planted mainly in Franken.",
-        "color": "black",
+        "synonyms": [
+            "Geilweilerhof 4-25-7"
+        ],
+        "description": {
+            "default": "Modern red German cross planted mainly in Franken.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Donzelinho Tinto",
-        "synonyms": ["Donzelinho do Castello", "Donzelynho", "Tinta do Minho"],
-        "description": "Old, rare Douro variety playing a very small, inglorious part in blended wines, fortified and unfortified.",
-        "color": "black",
+        "synonyms": [
+            "Donzelinho do Castello",
+            "Donzelynho",
+            "Tinta do Minho"
+        ],
+        "description": {
+            "default": "Old, rare Douro variety playing a very small, inglorious part in blended wines, fortified and unfortified.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Doradilla",
-        "synonyms": ["Forastera Blanca", "Plateado"],
-        "description": "Very minor variety from Málaga in Andalucía frequently confused with other varieties.",
-        "color": "white",
+        "synonyms": [
+            "Forastera Blanca",
+            "Plateado"
+        ],
+        "description": {
+            "default": "Very minor variety from Málaga in Andalucía frequently confused with other varieties.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dorinto",
         "synonyms": [
             "Arinto Branco",
             "Arinto do Douro",
             "Arinto do Interior",
             "Arinto no Douro",
-            "Arinto de Trás-os-Montes",
+            "Arinto de Trás-os-Montes"
         ],
-        "description": "Recently renamed Portuguese white.",
-        "color": "white",
+        "description": {
+            "default": "Recently renamed Portuguese white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dornfelder",
-        "synonyms": ["Weinsberg S 341"],
-        "description": "The most successful of the modern red German crosses, making dark, velvety wines.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg S 341"
+        ],
+        "description": {
+            "default": "The most successful of the modern red German crosses, making dark, velvety wines.",
+            "julie": "",
+            "sommelier": "Dornfelder is vinified in all styles, but primarily as a dry wine. One distinctive style is a very fruity Dornfelder that brings forth the grape’s intense aromas of sour cherry, blackberry, and elder. Other growers ferment and/or age their Dornfelders in casks or barriques, focus on tannins and structure, and create rich, smooth, and harmonious deep color. All styles have an unmistakably deep color. The deep red-coloured Dornfelder red wines are ideal for the cool season and go well with hearty roasts, game or cheese. Fruity versions from the last harvest are also a pleasure to drink, even slightly chilled in summer. Aroma: sour cherry, blackberry and elderberry. Flavour: tannic, full-bodied, smooth, harmonious."
+        },
+        "color": "black"
     },
     {
         "name": "Dorona Di Venezia",
-        "synonyms": ["Dorona", "Dorona Veneziana", "Uva d’Oro"],
-        "description": "Recently rescued but not especially ancient Venetian white.",
-        "color": "white",
+        "synonyms": [
+            "Dorona",
+            "Dorona Veneziana",
+            "Uva d’Oro"
+        ],
+        "description": {
+            "default": "Recently rescued but not especially ancient Venetian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Douce Noire",
         "synonyms": [
             "Bathiolin",
             "Bonarda",
             "Charbonneau",
@@ -3159,155 +4982,288 @@
             "Corbeau",
             "Corbeau Noir",
             "Mauvais Noir",
             "Plant de Montmélian",
             "Plant de Turin",
             "Plant Noir",
             "Turca",
-            "Turin",
+            "Turin"
         ],
-        "description": "Savoie variety with several aliases causing considerable confusion, most widely planted in Argentina.",
-        "color": "black",
+        "description": {
+            "default": "Savoie variety with several aliases causing considerable confusion, most widely planted in Argentina.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Doux D’Henry",
-        "synonyms": ["Doux d’Enry", "Gros d’Henry"],
-        "description": "Rare, light-bodied red exclusive to the Pinerolese region of Piemonte.",
-        "color": "black",
+        "synonyms": [
+            "Doux d’Enry",
+            "Gros d’Henry"
+        ],
+        "description": {
+            "default": "Rare, light-bodied red exclusive to the Pinerolese region of Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Drnekuša",
-        "synonyms": ["Darnekuša", "Darnekuša Mala", "Darnekuša Vela", "Dernakuša"],
-        "description": "Rare vine from the Croatian island of Hvar.",
-        "color": "black",
+        "synonyms": [
+            "Darnekuša",
+            "Darnekuša Mala",
+            "Darnekuša Vela",
+            "Dernakuša"
+        ],
+        "description": {
+            "default": "Rare vine from the Croatian island of Hvar.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Drupeggio",
         "synonyms": [
             "Bottaio Bianco",
             "Cacinello",
             "Cacciumo",
             "Canaiolo Bianco",
             "Canajola",
             "Canina",
             "Uva dei Cani",
             "Drupeccio",
             "Lupeccio",
             "Trupeccio",
-            "Volpicchio",
+            "Volpicchio"
         ],
-        "description": "Neutral, central Italian white also known as Canaiolo Bianco.",
-        "color": "white",
+        "description": {
+            "default": "Neutral, central Italian white also known as Canaiolo Bianco.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dunaj",
-        "synonyms": ["MBOP × SV 6/10"],
-        "description": "Minor but potentially high-quality Slovak cross responsible for soft, full-bodied reds.",
-        "color": "black",
+        "synonyms": [
+            "MBOP × SV 6/10"
+        ],
+        "description": {
+            "default": "Minor but potentially high-quality Slovak cross responsible for soft, full-bodied reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dunkelfelder",
-        "synonyms": ["Fröhlich V. 4.4", "Fröhlich V 4", "Purpur"],
-        "description": "Dark-skinned German cross usefully adding colour and body to blends.",
-        "color": "black",
+        "synonyms": [
+            "Fröhlich V. 4.4",
+            "Fröhlich V 4",
+            "Purpur"
+        ],
+        "description": {
+            "default": "Dark-skinned German cross usefully adding colour and body to blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Duranija",
-        "synonyms": ["Brajdenica", "Duranija Bijela", "Duronija"],
-        "description": "Almost extinct Croatian variety from the Istrian peninsula.",
-        "color": "white",
+        "synonyms": [
+            "Brajdenica",
+            "Duranija Bijela",
+            "Duronija"
+        ],
+        "description": {
+            "default": "Almost extinct Croatian variety from the Istrian peninsula.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Duras",
-        "synonyms": ["Durade", "Duras Rouge", "Durazé"],
-        "description": "Structured and peppery variety playing a minor role in the Gaillac appellation.",
-        "color": "black",
+        "synonyms": [
+            "Durade",
+            "Duras Rouge",
+            "Durazé"
+        ],
+        "description": {
+            "default": "Structured and peppery variety playing a minor role in the Gaillac appellation.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Durella",
-        "synonyms": ["Cagnina", "Caina", "Durella Gentile", "Rabiosa"],
-        "description": "Makes crisp, light-bodied Veneto whites.",
-        "color": "white",
+        "synonyms": [
+            "Cagnina",
+            "Caina",
+            "Durella Gentile",
+            "Rabiosa"
+        ],
+        "description": {
+            "default": "Makes crisp, light-bodied Veneto whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dureza",
-        "synonyms": ["Duré", "Duret", "Durezza", "Petit Duret", "Serène", "Serine"],
-        "description": "Virtually extinct Ardèche variety most famous as a parent of Syrah.",
-        "color": "black",
+        "synonyms": [
+            "Duré",
+            "Duret",
+            "Durezza",
+            "Petit Duret",
+            "Serène",
+            "Serine"
+        ],
+        "description": {
+            "default": "Virtually extinct Ardèche variety most famous as a parent of Syrah.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Durif",
         "synonyms": [
             "Dure",
             "Duret",
             "Gros Noir",
             "Petite Sirah",
             "Petite Syrah",
             "Pinot de l’Hermitage",
             "Pinot de Romans",
             "Plant Durif",
             "Serine des Mauves",
-            "Sirane Fourchue",
+            "Sirane Fourchue"
         ],
-        "description": "Originally French but particularly famous, as Petite Sirah, in California.",
-        "color": "black",
+        "description": {
+            "default": "Originally French but particularly famous, as Petite Sirah, in California.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Dutchess",
-        "synonyms": ["Duchess"],
-        "description": "Disappearing, low-yielding, sensitive North American hybrid also found in Brazil.",
-        "color": "white",
+        "synonyms": [
+            "Duchess"
+        ],
+        "description": {
+            "default": "Disappearing, low-yielding, sensitive North American hybrid also found in Brazil.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Dzvelshavi Obchuri",
-        "synonyms": ["Zelscavi"],
-        "description": "Mediocre Georgian variety producing intensely coloured reds.",
-        "color": "black",
+        "synonyms": [
+            "Zelscavi"
+        ],
+        "description": {
+            "default": "Mediocre Georgian variety producing intensely coloured reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Early Muscat",
-        "synonyms": ["California K 4-19"],
-        "description": "California cross bred for the table but also producing aromatic wines in Oregon.",
-        "color": "white",
+        "synonyms": [
+            "California K 4-19"
+        ],
+        "description": {
+            "default": "California cross bred for the table but also producing aromatic wines in Oregon.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Edelweiss",
-        "synonyms": ["Elmer Swenson", "ES 40"],
-        "description": "Minor, usefully disease-resistant and winter-hardy, not too foxy American hybrid.",
-        "color": "white",
+        "synonyms": [
+            "Elmer Swenson",
+            "ES 40"
+        ],
+        "description": {
+            "default": "Minor, usefully disease-resistant and winter-hardy, not too foxy American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ederena",
-        "synonyms": ["Édéréna"],
-        "description": "Bordeaux cross being trialled in California.",
-        "color": "black",
+        "synonyms": [
+            "Édéréna"
+        ],
+        "description": {
+            "default": "Bordeaux cross being trialled in California.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Egiodola",
-        "synonyms": ["Égiodola"],
-        "description": "Recent productive Bordeaux cross starting to show some potential at home and abroad. Quite tannic.",
-        "color": "black",
+        "synonyms": [
+            "Égiodola"
+        ],
+        "description": {
+            "default": "Recent productive Bordeaux cross starting to show some potential at home and abroad. Quite tannic.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ehrenfelser",
-        "synonyms": ["Geisenheim 9-93"],
-        "description": "Frost-resistant German cross bred as an alternative to Riesling.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 9-93"
+        ],
+        "description": {
+            "default": "Frost-resistant German cross bred as an alternative to Riesling.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ekigaïna",
-        "synonyms": ["Ékigaïna"],
-        "description": "Recent Bordeaux cross yet to make inroads in the vineyard.",
-        "color": "black",
+        "synonyms": [
+            "Ékigaïna"
+        ],
+        "description": {
+            "default": "Recent Bordeaux cross yet to make inroads in the vineyard.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ekim Kara",
-        "synonyms": ["Echim Kara"],
-        "description": "Late-ripening Ukrainian variety making fortified red dessert wines.",
-        "color": "black",
+        "synonyms": [
+            "Echim Kara"
+        ],
+        "description": {
+            "default": "Late-ripening Ukrainian variety making fortified red dessert wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Elbling",
         "synonyms": [
             "Aelbinen",
             "Albich",
             "Burger",
@@ -3315,154 +5271,278 @@
             "Elsässer",
             "Grobriesling",
             "Grossriesling",
             "Haussard",
             "Raisin Blanc des Allemands",
             "Rheinelbe",
             "Weisser Silvaner",
-            "Ysèle .",
+            "Ysèle ."
         ],
-        "description": "Ancient, once ubiquitous, now unfashionable German variety used mainly as a base wine for fizz.",
-        "color": "white",
+        "description": {
+            "default": "Ancient, once ubiquitous, now unfashionable German variety used mainly as a base wine for fizz.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Emerald Riesling",
-        "synonyms": ["California 1139E29", "Emerald Rizling"],
-        "description": "California cross that has travelled widely but not gloriously and turns out to be no Riesling.",
-        "color": "white",
+        "synonyms": [
+            "California 1139E29",
+            "Emerald Rizling"
+        ],
+        "description": {
+            "default": "California cross that has travelled widely but not gloriously and turns out to be no Riesling.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Enantio",
         "synonyms": [
             "Foja Tonda",
             "Lambrusco a Foglia Frastagliata",
-            "Lambrusco Nostrano",
+            "Lambrusco Nostrano"
         ],
-        "description": "Fairly recent official name for a Trentino variety once called Lambrusco a Foglia Frastagliata.",
-        "color": "black",
+        "description": {
+            "default": "Fairly recent official name for a Trentino variety once called Lambrusco a Foglia Frastagliata.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Encruzado",
-        "synonyms": ["Salgueirinho"],
-        "description": "High-quality, well-structured Portuguese variety with the potential to produce ageworthy wines.",
-        "color": "white",
+        "synonyms": [
+            "Salgueirinho"
+        ],
+        "description": {
+            "default": "High-quality, well-structured Portuguese variety with the potential to produce ageworthy wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Enfariné Noir",
-        "synonyms": ["Enfariné du Jura", "Gaillard", "Gouais Noir", "Grison"],
-        "description": "Ancient and virtually extinct variety that survives in the Jura.",
-        "color": "black",
+        "synonyms": [
+            "Enfariné du Jura",
+            "Gaillard",
+            "Gouais Noir",
+            "Grison"
+        ],
+        "description": {
+            "default": "Ancient and virtually extinct variety that survives in the Jura.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Eona",
-        "synonyms": ["Éona"],
-        "description": "South Dakotan hybrid just about surviving in Québec.",
-        "color": "white",
+        "synonyms": [
+            "Éona"
+        ],
+        "description": {
+            "default": "South Dakotan hybrid just about surviving in Québec.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Erbaluce",
         "synonyms": [
             "Albaluce",
             "Bian Roustì",
             "Bianchera",
             "Greco Bianco di Novara",
-            "Uva Rustìa",
+            "Uva Rustìa"
         ],
-        "description": "Minor white Piemontese variety, occasionally making distinctive sweet wines.",
-        "color": "white",
+        "description": {
+            "default": "Minor white Piemontese variety, occasionally making distinctive sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Erbamat",
-        "synonyms": ["Albamatto", "Erbamatto", "Verdealbara"],
-        "description": "Virtually extinct local white from Brescia, northern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Albamatto",
+            "Erbamatto",
+            "Verdealbara"
+        ],
+        "description": {
+            "default": "Virtually extinct local white from Brescia, northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ervi",
-        "synonyms": ["Barbera × Bonarda 108", "Incrocio Fregoni 108"],
-        "description": "Minor and relatively recent dark-skinned cross from Emilia-Romagna.",
-        "color": "black",
+        "synonyms": [
+            "Barbera × Bonarda 108",
+            "Incrocio Fregoni 108"
+        ],
+        "description": {
+            "default": "Minor and relatively recent dark-skinned cross from Emilia-Romagna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Escursac",
-        "synonyms": ["Corçac", "Cursach", "Escorçac", "Escursag", "Excursach"],
-        "description": "Recently rescued Mallorcan making promising reds.",
-        "color": "black",
+        "synonyms": [
+            "Corçac",
+            "Cursach",
+            "Escorçac",
+            "Escursag",
+            "Excursach"
+        ],
+        "description": {
+            "default": "Recently rescued Mallorcan making promising reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Espadeiro",
-        "synonyms": ["Espadeiro Tinto", "Padeiro Tinto"],
-        "description": "Minho vine producing rosé.",
-        "color": "black",
+        "synonyms": [
+            "Espadeiro Tinto",
+            "Padeiro Tinto"
+        ],
+        "description": {
+            "default": "Minho vine producing rosé.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Espirit",
-        "synonyms": ["ES 422", "Esprit"],
-        "description": "Very minor but cold-hardy American hybrid producing mild, fruity wines.",
-        "color": "white",
+        "synonyms": [
+            "ES 422",
+            "Esprit"
+        ],
+        "description": {
+            "default": "Very minor but cold-hardy American hybrid producing mild, fruity wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Etraire De L’Aduï",
         "synonyms": [
             "Beccu de l’Aduï",
             "Betu",
             "Etraire de la Dot",
             "Etraire de la Dû",
             "Due",
             "Etraire de la Duï",
             "Etraire de la Duy",
-            "Grosse Etraire",
+            "Grosse Etraire"
         ],
-        "description": "Isère speciality still cultivated to a limited extent in Savoie.",
-        "color": "black",
+        "description": {
+            "default": "Isère speciality still cultivated to a limited extent in Savoie.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Evmolpia",
-        "synonyms": ["Evmolpiya", "Thracian Mavrud"],
-        "description": "Recent Bulgarian cross valued for its productivity and early ripening as well as for its easy-drinking reds.",
-        "color": "black",
+        "synonyms": [
+            "Evmolpiya",
+            "Thracian Mavrud"
+        ],
+        "description": {
+            "default": "Recent Bulgarian cross valued for its productivity and early ripening as well as for its easy-drinking reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Eyholzer Rote",
-        "synonyms": ["Eyholzer Roter", "Gross Roth", "Grossroter"],
-        "description": "Ancient and extremely rare variety vinified by just one southern Swiss producer.",
-        "color": "red",
+        "synonyms": [
+            "Eyholzer Roter",
+            "Gross Roth",
+            "Grossroter"
+        ],
+        "description": {
+            "default": "Ancient and extremely rare variety vinified by just one southern Swiss producer.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Ezerfürtű",
-        "synonyms": ["Kecskemét 5", "Miklóstelepi 5"],
-        "description": "Neutral Hungarian white cross generally hidden in blends.",
-        "color": "white",
+        "synonyms": [
+            "Kecskemét 5",
+            "Miklóstelepi 5"
+        ],
+        "description": {
+            "default": "Neutral Hungarian white cross generally hidden in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ezerjó",
         "synonyms": [
             "Budai Fehér",
             "Fehér Bakator",
             "Kolmreifler",
             "Korponai",
             "Tausendgute",
             "Tausent Güte",
             "Trummertraube",
-            "Zátoki",
+            "Zátoki"
         ],
-        "description": "Once widely planted Hungarian variety making high-acid whites from dry to sweet.",
-        "color": "white",
+        "description": {
+            "default": "Once widely planted Hungarian variety making high-acid whites from dry to sweet.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Faberrebe",
-        "synonyms": ["Alzey 10375", "Faber"],
-        "description": "High-yielding, lightly aromatic German cross losing ground.",
-        "color": "white",
+        "synonyms": [
+            "Alzey 10375",
+            "Faber"
+        ],
+        "description": {
+            "default": "High-yielding, lightly aromatic German cross losing ground.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Falanghina Flegrea",
-        "synonyms": ["Falanghina Pigna Piccola", "Falernina", "Uva Falerna"],
-        "description": "Campania’s signature white wine grape.",
-        "color": "white",
+        "synonyms": [
+            "Falanghina Pigna Piccola",
+            "Falernina",
+            "Uva Falerna"
+        ],
+        "description": {
+            "default": "Campania’s signature white wine grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fer",
         "synonyms": [
             "Braucol",
             "Caillaba",
             "Camaralet Noir",
@@ -3471,160 +5551,253 @@
             "Fer Servadou",
             "Gragnelut",
             "Hère",
             "Mansois",
             "Samençois",
             "Mourac",
             "Pinenc",
-            "Servadou",
+            "Servadou"
         ],
-        "description": "The untamed, tannic variety of Marcillac, south-west France.",
-        "color": "black",
+        "description": {
+            "default": "The untamed, tannic variety of Marcillac, south-west France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fernão Pires",
         "synonyms": [
             "Fernao Pirao",
             "Fernão Pires de Beco",
             "Gaeiro",
             "Gaieiro",
             "Maria Gomes",
             "Molinha",
-            "Torrontés",
+            "Torrontés"
         ],
-        "description": "Most common light-skinned grape in Portugal. Adaptable, high-yielding, making aromatic whites.",
-        "color": "white",
+        "description": {
+            "default": "Most common light-skinned grape in Portugal. Adaptable, high-yielding, making aromatic whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fertilia",
-        "synonyms": ["Incrocio Cosmo", "Merlot × Raboso Veronese 108"],
-        "description": "Very minor red blending component in Treviso, northern Italy.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Cosmo",
+            "Merlot × Raboso Veronese 108"
+        ],
+        "description": {
+            "default": "Very minor red blending component in Treviso, northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fetească Albă",
         "synonyms": [
             "Dievcie Hrozno",
             "Fetiasca Belii",
             "Fetișoară",
             "Fetyaska Alba",
             "Mädchentraube",
             "Păsărească Albă",
             "Poamă Fetei Albă",
-            "Văratic",
+            "Văratic"
         ],
-        "description": "Second most planted Fetească and is even more important in Romania than in its Moldovan birthplace.",
-        "color": "white",
+        "description": {
+            "default": "Second most planted Fetească and is even more important in Romania than in its Moldovan birthplace.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fetească Neagră",
         "synonyms": [
             "Coada Rândunicii",
             "Fetyaska Chernaya",
             "Păsărească Neagră",
             "Poamă Fetei Neagră",
-            "Schwarze Mädchentraube",
+            "Schwarze Mädchentraube"
         ],
-        "description": "The red-wine Fetească, a resurgent Moldovan producing good-quality wine mainly in Romania.",
-        "color": "black",
+        "description": {
+            "default": "The red-wine Fetească, a resurgent Moldovan producing good-quality wine mainly in Romania.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fetească Regală",
         "synonyms": [
             "Dănăşană",
             "Danesana",
             "Dunesdörfer Königsast",
             "Galbenă de Ardeal",
             "Königliche Mädchentraube",
-            "Pesecká Leánka .",
+            "Pesecká Leánka ."
         ],
-        "description": "The most planted Fetească, responsible for fresh, aromatic whites in Romania.",
-        "color": "white",
+        "description": {
+            "default": "The most planted Fetească, responsible for fresh, aromatic whites in Romania.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fiano",
-        "synonyms": ["Fiano di Avellino"],
-        "description": "Rich, waxy, strongly flavoured, fashionable southern Italian.",
-        "color": "white",
+        "synonyms": [
+            "Fiano di Avellino"
+        ],
+        "description": {
+            "default": "Rich, waxy, strongly flavoured, fashionable southern Italian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fioletovy Ranny",
-        "synonyms": ["Filetovyi Ranii"],
-        "description": "Russian variety used for the table, grape juice and nutmeg-flavoured red wine.",
-        "color": "black",
+        "synonyms": [
+            "Filetovyi Ranii"
+        ],
+        "description": {
+            "default": "Russian variety used for the table, grape juice and nutmeg-flavoured red wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Flavis",
-        "synonyms": ["Incrocio Cosmo 76"],
-        "description": "Minor white northern Italian cross.",
-        "color": "white",
+        "synonyms": [
+            "Incrocio Cosmo 76"
+        ],
+        "description": {
+            "default": "Minor white northern Italian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Flora",
-        "synonyms": ["California H59-90"],
-        "description": "Minor, pink-skinned California cross capable of producing aromatic, full-bodied, sometimes flabby wines.",
-        "color": "pink",
+        "synonyms": [
+            "California H59-90"
+        ],
+        "description": {
+            "default": "Minor, pink-skinned California cross capable of producing aromatic, full-bodied, sometimes flabby wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Florental",
-        "synonyms": ["Burdin 7705"],
-        "description": "Minor eastern French hybrid widely recommended but apparently hardly grown.",
-        "color": "black",
+        "synonyms": [
+            "Burdin 7705"
+        ],
+        "description": {
+            "default": "Minor eastern French hybrid widely recommended but apparently hardly grown.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Foça Karasi",
-        "synonyms": ["Bilgi Yok", "Foça", "Foçakarası"],
-        "description": "Almost-extinct variety from Turkey’s Aegean coast.",
-        "color": "black",
+        "synonyms": [
+            "Bilgi Yok",
+            "Foça",
+            "Foçakarası"
+        ],
+        "description": {
+            "default": "Almost-extinct variety from Turkey’s Aegean coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fogarina",
-        "synonyms": ["Fogarina di Gualtieri", "Fugarina"],
-        "description": "Mysterious, twice-rescued northern Italian red that adds colour and acidity in blends.",
-        "color": "black",
+        "synonyms": [
+            "Fogarina di Gualtieri",
+            "Fugarina"
+        ],
+        "description": {
+            "default": "Mysterious, twice-rescued northern Italian red that adds colour and acidity in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fogoneu",
         "synonyms": [
             "Fogoneau",
             "Fogonet",
             "Fogonetxo",
             "Fogoneu Frances",
-            "Fogoneu Mallorquí",
+            "Fogoneu Mallorquí"
         ],
-        "description": "Minor Mallorcan, usually blended.",
-        "color": "black",
+        "description": {
+            "default": "Minor Mallorcan, usually blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fokiano",
         "synonyms": [
             "Damaskino",
             "Fokiana",
             "Fokiano Kokkino",
             "Fokiano Mavro",
             "Giouroukiko",
             "Ghiouroukiko",
             "Phokiano",
             "Phokiano Kokkineli",
-            "Phokiano Mavro",
+            "Phokiano Mavro"
         ],
-        "description": "Rare Greek variety almost lost in the confusion over its name and synonyms.",
-        "color": "black",
+        "description": {
+            "default": "Rare Greek variety almost lost in the confusion over its name and synonyms.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Folgasão",
-        "synonyms": ["Cagarrizo", "Silveiriña"],
-        "description": "Robust Iberian variety with complex origins.",
-        "color": "white",
+        "synonyms": [
+            "Cagarrizo",
+            "Silveiriña"
+        ],
+        "description": {
+            "default": "Robust Iberian variety with complex origins.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Folignan",
-        "synonyms": ["INRA 8476"],
-        "description": "Recent Bordeaux cross authorized for the production of cognac.",
-        "color": "white",
+        "synonyms": [
+            "INRA 8476"
+        ],
+        "description": {
+            "default": "Recent Bordeaux cross authorized for the production of cognac.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Folle Blanche",
         "synonyms": [
             "Chalosse Blanche",
             "Dame Blanche",
             "Enrageat",
@@ -3632,50 +5805,83 @@
             "Folle",
             "Gros Plant",
             "Matza Zuri",
             "Mune Mahatsa",
             "Piquepoul",
             "Piquepoul du Gers",
             "Picpoul",
-            "Picpoule",
+            "Picpoule"
         ],
-        "description": "Productive but rot-prone and very acidic white variety.",
-        "color": "white",
+        "description": {
+            "default": "Productive but rot-prone and very acidic white variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fonte Cal",
-        "synonyms": ["Fonte de Cal"],
-        "description": "Minor Portuguese variety that rarely takes a leading role.",
-        "color": "white",
+        "synonyms": [
+            "Fonte de Cal"
+        ],
+        "description": {
+            "default": "Minor Portuguese variety that rarely takes a leading role.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Forastera",
-        "synonyms": ["Forastiera", "Forestiera", "Frastera", "Uva dell’Isola"],
-        "description": "Ischian speciality.",
-        "color": "white",
+        "synonyms": [
+            "Forastiera",
+            "Forestiera",
+            "Frastera",
+            "Uva dell’Isola"
+        ],
+        "description": {
+            "default": "Ischian speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Forcallat Tinta",
         "synonyms": [
             "Alcabril di Gualadin",
             "Forcalla",
             "Forcalla Negra",
             "Forcalla Prieta",
             "Verdal",
             "Verdalejo",
-            "Verdalla",
+            "Verdalla"
         ],
-        "description": "Late-ripening central Spanish variety used in blends.",
-        "color": "black",
+        "description": {
+            "default": "Late-ripening central Spanish variety used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Forsellina",
-        "synonyms": ["Forcelina", "Forselina", "Forsella", "Forsellana", "Forzelina"],
-        "description": "Rarity occasionally blended into Valpolicella or Bardolino.",
-        "color": "black",
+        "synonyms": [
+            "Forcelina",
+            "Forselina",
+            "Forsella",
+            "Forsellana",
+            "Forzelina"
+        ],
+        "description": {
+            "default": "Rarity occasionally blended into Valpolicella or Bardolino.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fortana",
         "synonyms": [
             "Canèna",
             "Canina Nera",
             "Cannina",
@@ -3683,123 +5889,185 @@
             "Oliva",
             "Rapa",
             "Uva Canina",
             "Uva Cornetta",
             "Uva d’Oro",
             "Uva d’Oro di Comacchio",
             "Uva Francese Nera",
-            "Uva Vecchia",
+            "Uva Vecchia"
         ],
-        "description": "Late-ripening, declining Italian red prized for its high yields.",
-        "color": "black",
+        "description": {
+            "default": "Late-ripening, declining Italian red prized for its high yields.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Francavidda",
-        "synonyms": ["Francavilla"],
-        "description": "Minor and dwindling vine found in Brindisi, generally blended.",
-        "color": "white",
+        "synonyms": [
+            "Francavilla"
+        ],
+        "description": {
+            "default": "Minor and dwindling vine found in Brindisi, generally blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Frâncuşă",
         "synonyms": [
             "Frâncuşe",
             "Frîncuşă",
             "Mustoasă",
             "Mustoasă de Moldova",
             "Poamă Creaţă",
             "Poamă Franchie",
             "Poamă Muştei",
             "Târţără",
-            "Vinoasă",
+            "Vinoasă"
         ],
-        "description": "North-east Romanian variety producing fresh and relatively light, dry whites for early drinking.",
-        "color": "white",
+        "description": {
+            "default": "North-east Romanian variety producing fresh and relatively light, dry whites for early drinking.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Frappato",
         "synonyms": [
             "Frappato di Vittoria",
             "Frappato Nero",
             "Frappatu",
             "Nero Capitano",
-            "Surra",
+            "Surra"
         ],
-        "description": "Fruity, fresh and floral Sicilian often blended with Nero d’Avola.",
-        "color": "black",
+        "description": {
+            "default": "Fruity, fresh and floral Sicilian often blended with Nero d’Avola.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Fraueler",
-        "synonyms": ["Frauler", "Vezzaner"],
-        "description": "Rare, high-yielding and acidic Tyrolean white.",
-        "color": "white",
+        "synonyms": [
+            "Frauler",
+            "Vezzaner"
+        ],
+        "description": {
+            "default": "Rare, high-yielding and acidic Tyrolean white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fredonia",
-        "synonyms": ["Early Concord"],
-        "description": "New York hybrid found mainly in Pennsylvania.",
-        "color": "black",
+        "synonyms": [
+            "Early Concord"
+        ],
+        "description": {
+            "default": "New York hybrid found mainly in Pennsylvania.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Freisa",
         "synonyms": [
             "Freisa di Chieri",
             "Freisa Piccola",
             "Freisetta",
             "Fresia",
             "Monferrina",
             "Mounfrina",
-            "Spannina",
+            "Spannina"
         ],
-        "description": "Light, fragrant, unusual Nebbiolo relative, made in a wide range of styles, including frothy.",
-        "color": "black",
+        "description": {
+            "default": "Light, fragrant, unusual Nebbiolo relative, made in a wide range of styles, including frothy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Freisamer",
-        "synonyms": ["Freiburg 25-1", "Freiburger"],
-        "description": "Early-twentieth-century German cross in severe decline.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 25-1",
+            "Freiburger"
+        ],
+        "description": {
+            "default": "Early-twentieth-century German cross in severe decline.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Frontenac",
-        "synonyms": ["MN 1047"],
-        "description": "Successfully cold-hardy American hybrid thriving particularly in its home state of Minnesota.",
-        "color": "black",
+        "synonyms": [
+            "MN 1047"
+        ],
+        "description": {
+            "default": "Successfully cold-hardy American hybrid thriving particularly in its home state of Minnesota.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Frühroter Veltliner",
         "synonyms": [
             "Früher Roter Malvasier",
             "Korai Piros Veltelini",
             "Malvasier",
             "Malvoisie Rouge d’Italie",
             "Velteliner Rouge Précoce",
             "Veltlínské Červené Rané",
-            "Veltlínske Červené Skoré",
+            "Veltlínske Červené Skoré"
         ],
-        "description": "Tentacular in its relations but Grüner Veltliner is not one of them.",
-        "color": "red",
+        "description": {
+            "default": "Tentacular in its relations but Grüner Veltliner is not one of them.",
+            "julie": "",
+            "sommelier": "This very old variety is a crossing of Roter Veltliner x Sylvaner, and is regarded as being typically Austrian. In recent years, it has lost significance, and is mostly sold as table grapes, as a young wine, or as a simple house wine, particularly in the Thermenregion, Weinviertel and Wagram (Lower Austria). The early-drinking wines that are relatively low in acidity are also low in alcohol and usually present a bouquet somewhat evocative of flowers and bitter almonds."
+        },
+        "color": "red"
     },
     {
         "name": "Fubiano",
-        "synonyms": ["Incrocio Dalmasso II/32"],
-        "description": "Barely significant white cross from northern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Incrocio Dalmasso II/32"
+        ],
+        "description": {
+            "default": "Barely significant white cross from northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Fuella Nera",
         "synonyms": [
             "Dame Noire",
             "Folle de Nice",
             "Folle Noire",
             "Fuella",
             "Fuola",
-            "Jurançon Rouge",
+            "Jurançon Rouge"
         ],
-        "description": "Minor but aromatic variety at home on the French Riviera.",
-        "color": "black",
+        "description": {
+            "default": "Minor but aromatic variety at home on the French Riviera.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Furmint",
         "synonyms": [
             "Fehér Furmint",
             "Lazafürtű Furmint",
             "Moslavac",
@@ -3807,88 +6075,129 @@
             "Mosler",
             "Šipon",
             "Som",
             "Szigeti",
             "Tokay",
             "Változó Furmint",
             "Zapfner",
-            "Zopfner",
+            "Zopfner"
         ],
-        "description": "The principal variety of the fiery, high-acid wines of Tokaj in Hungary.",
-        "color": "white",
+        "description": {
+            "default": "The principal variety of the fiery, high-acid wines of Tokaj in Hungary.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gaglioppo",
         "synonyms": [
             "Arvino Nero",
             "Cirotana",
             "Gaglioppo di Cirò",
             "Galloppo",
             "Morellino Pizzuto",
-            "Navarna",
+            "Navarna"
         ],
-        "description": "The characterful red wine grape of Calabria.",
-        "color": "black",
+        "description": {
+            "default": "The characterful red wine grape of Calabria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gaidouria",
-        "synonyms": ["Gaidouricha", "Gaidouriha", "Gaydura", "Guydourina"],
-        "description": "Very rare variety just surviving on the Greek island of Santoríni.",
-        "color": "white",
+        "synonyms": [
+            "Gaidouricha",
+            "Gaidouriha",
+            "Gaydura",
+            "Guydourina"
+        ],
+        "description": {
+            "default": "Very rare variety just surviving on the Greek island of Santoríni.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Galbenă De Odobești",
         "synonyms": [
             "Bucium de Poamă Galbenă",
             "Galbenă di Căpătanu",
             "Galbenă Grasă",
             "Galbenă Uriașă",
-            "Poamă Galbenă",
+            "Poamă Galbenă"
         ],
-        "description": "Gradually declining Romanian variety producing everyday whites.",
-        "color": "white",
+        "description": {
+            "default": "Gradually declining Romanian variety producing everyday whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Galego Dourado",
         "synonyms": [
             "Dourado",
             "False Pedro",
             "Gallego",
             "Moscato Galego Dourado",
             "Olho de Lebre",
             "Pedro Luis",
-            "Rutherglen Pedro",
+            "Rutherglen Pedro"
         ],
-        "description": "Rare Portuguese clings on.",
-        "color": "white",
+        "description": {
+            "default": "Rare Portuguese clings on.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gallioppo Delle Marche",
         "synonyms": [
             "Balsamina Galloppa",
             "Balsamina Grossa",
             "Gaglioppa",
             "Galloppa",
             "Lancianese Nero",
-            "Moretta",
+            "Moretta"
         ],
-        "description": "Recently rescued and replanted central Italian vine that may be related to Sangiovese.",
-        "color": "black",
+        "description": {
+            "default": "Recently rescued and replanted central Italian vine that may be related to Sangiovese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gallizzone",
-        "synonyms": ["Gallazzone"],
-        "description": "Tuscan red on the verge of extinction.",
-        "color": "black",
+        "synonyms": [
+            "Gallazzone"
+        ],
+        "description": {
+            "default": "Tuscan red on the verge of extinction.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gamaret",
-        "synonyms": ["Pully B-13"],
-        "description": "Increasingly popular Swiss cross valued for its early ripening and resistance to rot.",
-        "color": "black",
+        "synonyms": [
+            "Pully B-13"
+        ],
+        "description": {
+            "default": "Increasingly popular Swiss cross valued for its early ripening and resistance to rot.",
+            "julie": "",
+            "sommelier": "Gamaret produces wines with a beautiful purple robe, spicy aromas and powerful tannins. It is often used as a blend component. When it is vinified as a monovarietal wine, it is, most of the time, aged in barrels."
+        },
+        "color": "black"
     },
     {
         "name": "Gamay Noir",
         "synonyms": [
             "Beaujolais",
             "Bourguignon Noir",
             "Gamai",
@@ -3911,74 +6220,123 @@
             "Gamay Précoce",
             "Gamé",
             "Gammé",
             "Grosse Dôle",
             "Liverdun Grand",
             "Lyonnais",
             "Petit Gamay",
-            "Plant Robert",
+            "Plant Robert"
         ],
-        "description": "Greater Burgundian refresher making wines generally but not always for early consumption.",
-        "color": "black",
+        "description": {
+            "default": "Greater Burgundian refresher making wines generally but not always for early consumption.",
+            "julie": "",
+            "sommelier": "In Switzerland, Gamay is one of the most widely planted grape varieties Although Gamay has a dark skin, its flesh is almost white. Wine made from Gamay is refreshing with low alcohol and tannins. Its aroma is characterized by fruity notes of raspberries and cherries. Gamay in general should be drunk young. Some top wines aged in wooden barrels can be long-lived, however. Gamay produces wines with notes of red fruits (strawberry, raspberry, cherry). It has soft tannins and sustained acidity. Color: dark-red color. Nose: intense aroma. Aromas: seductive and charming."
+        },
+        "color": "black"
     },
     {
         "name": "Gamay Teinturier De Bouze",
         "synonyms": [
             ": Gamay de Bouze",
             "Moureau",
             "Mourot",
             "Plant de Bouze",
-            "Rouge de Bouze",
+            "Rouge de Bouze"
         ],
-        "description": "Red-fleshed variety possibly related to the more common Gamay Noir but much less widely planted.",
-        "color": "black",
+        "description": {
+            "default": "Red-fleshed variety possibly related to the more common Gamay Noir but much less widely planted.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gamba Di Pernice",
-        "synonyms": ["Neretto degli Alteni", "Pernice"],
-        "description": "Rare, aromatic and spicy Piemontese.",
-        "color": "black",
+        "synonyms": [
+            "Neretto degli Alteni",
+            "Pernice"
+        ],
+        "description": {
+            "default": "Rare, aromatic and spicy Piemontese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gänsfüsser",
         "synonyms": [
             "Argan",
             "Argant",
             "Bockshorn",
             "Buchser",
             "Espagnol",
             "Gros Margillien",
-            "Margillien",
+            "Margillien"
         ],
-        "description": "Barely surviving ancient variety, probably German.",
-        "color": "black",
+        "description": {
+            "default": "Barely surviving ancient variety, probably German.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gara Ikeni",
-        "synonyms": ["Gara Lkeni", "Qara Lkeni", "Lkeny Tchernyi"],
-        "description": "Azeri grape used for both dry and sweet reds.",
-        "color": "black",
+        "synonyms": [
+            "Gara Lkeni",
+            "Qara Lkeni",
+            "Lkeny Tchernyi"
+        ],
+        "description": {
+            "default": "Azeri grape used for both dry and sweet reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Garandmak",
-        "synonyms": ["Alani Chagog", "Alivoruk", "Dik Chardji", "Garan Dmak"],
-        "description": "Old, popular and multi-purpose Armenian variety.",
-        "color": "white",
+        "synonyms": [
+            "Alani Chagog",
+            "Alivoruk",
+            "Dik Chardji",
+            "Garan Dmak"
+        ],
+        "description": {
+            "default": "Old, popular and multi-purpose Armenian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Garanoir",
-        "synonyms": ["Pully B-28"],
-        "description": "Swiss cross producing fruity but low-acid wines.",
-        "color": "black",
+        "synonyms": [
+            "Pully B-28"
+        ],
+        "description": {
+            "default": "Swiss cross producing fruity but low-acid wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Garganega",
-        "synonyms": ["Grecanico Dorato", "Malvasía de Manresa"],
-        "description": "A delicate white closely associated with Soave whose vigour and yields need strict control.",
-        "color": "white",
+        "synonyms": [
+            "Grecanico Dorato",
+            "Malvasía de Manresa"
+        ],
+        "description": {
+            "default": "A delicate white closely associated with Soave whose vigour and yields need strict control.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Garnacha Tinta",
         "synonyms": [
             ": Abundante",
             "Alicante",
             "Licante",
@@ -4001,18 +6359,22 @@
             "Lladoner",
             "Redondal",
             "Ranaccio",
             "Roussillon",
             "Sans Pareil",
             "Tinto Basto",
             "Tocai Rosso",
-            "Vernaccia Nera",
+            "Vernaccia Nera"
         ],
-        "description": "Very widely planted, long-lived vine making strong, sweetish reds and some successful rosés.",
-        "color": "black",
+        "description": {
+            "default": "Very widely planted, long-lived vine making strong, sweetish reds and some successful rosés.",
+            "julie": "One of the world's most planted grape variety that can thrive in hot and dry climate. Also known as Garnacha in Spain, it is often blended with Syrah and Mourvèdre - sometimes labelled then at GSM. In France, it thrives in the Southern Rhône and the Languedoc Roussillon. In the Rhône Valley, Grenache Noir has made the reputation of wines such as Châteauneuf-du-Pape, Gigondas and Vacqueyras where it is usually blended with Syrah and Mourvèdre. In the Roussillon, it produces some delicious fortified wines (Vins Doux Naturels) sold under the names Banyuls and Maury. In Spain, a new wave of perfumed, digest and elegant grenache have appeared in the regions of Gredos and Mentrida, near Madrid. In Catalonia, producers in the region of Priorat are making big, powerful wines grown on llicorella schist. Grenacge is also planted in Australia, California, Sardinia, etc. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Garnacha Blanca",
         "synonyms": [
             "Alicant Belyi",
             "Alicante Blanca",
             "Belan",
@@ -4027,148 +6389,226 @@
             "Grenache Blanc",
             "Grenash Beli",
             "Grenash Belyi",
             "Grenash Bjal",
             "Lladanor Blanca",
             "Rool Grenache",
             "Silla Blanc",
-            "Sillina Lanc",
+            "Sillina Lanc"
         ],
-        "description": "Full-bodied whites, pale version of the reds.",
-        "color": "white",
+        "description": {
+            "default": "Full-bodied whites, pale version of the reds.",
+            "julie": "Garnacha Blanca is mostly found in the Roussillon region in France but also in Catalonia and Aragon in Spain. Traditionnaly grown for the production of Vin Doux Naturel in France, it is more often blended than sold as a single grape variety for the production of table wine. It can produce however some outstading white wines with great subtance, texture and fragrance. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Garnacha Roja (Gris)",
         "synonyms": [
             "Garnacha Gris",
             "Garnacha Rioja",
             "Garnacho Rojo",
             "Garnatxa Gris",
             "Grenache Gris",
             "Grenache Rouge",
             "Grey Grenache",
             "Piros Grenache",
             "Rosco dos Pinheiro",
-            "Szuerke Grenache",
+            "Szuerke Grenache"
         ],
-        "description": "Perfumed and full-bodied.",
-        "color": "grey and pink",
+        "description": {
+            "default": "Perfumed and full-bodied.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey and pink"
     },
     {
         "name": "Garnacha Peluda",
         "synonyms": [
             "Garnatxa Pelud",
             "Garnatxa Peluda",
             "Grenache d’Afrique",
             "Grenache Noir Tomenteux",
             "Grenache Poilu",
             "Grenache Velu",
             "Lladoner Pelud",
-            "Lledoner Pelut",
+            "Lledoner Pelut"
         ],
-        "description": "Downy-leaved variant of Garnacha Tinta.",
-        "color": "black",
+        "description": {
+            "default": "Downy-leaved variant of Garnacha Tinta.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Garrido Fino",
         "synonyms": [
             "Charrido Fino",
             "Garrido",
             "Garrido Fino de Villanueva",
             "Garrio Fino",
-            "Palomino Garrio",
+            "Palomino Garrio"
         ],
-        "description": "Very minor, acidic variety from Huelva in southern Spain.",
-        "color": "white",
+        "description": {
+            "default": "Very minor, acidic variety from Huelva in southern Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gascon",
         "synonyms": [
             "Franc Noir de l’Yonne",
             "Franc Noir du Gâtinais",
             "Noirien",
-            "Plant de Moret",
+            "Plant de Moret"
         ],
-        "description": "Rare Touraine vine.",
-        "color": "black",
+        "description": {
+            "default": "Rare Touraine vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gegić",
         "synonyms": [
             "Debejan",
             "Debljan",
             "Gegić Bijeli",
             "Paška",
             "Paškinja",
-            "Žutina",
+            "Žutina"
         ],
-        "description": "Speciality of the Croatian island of Pag.",
-        "color": "white",
+        "description": {
+            "default": "Speciality of the Croatian island of Pag.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ġellewża",
-        "synonyms": ["Gelleuza"],
-        "description": "Second most planted Maltese variety but being edged out by international invaders.",
-        "color": "black",
+        "synonyms": [
+            "Gelleuza"
+        ],
+        "description": {
+            "default": "Second most planted Maltese variety but being edged out by international invaders.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Genouillet",
-        "synonyms": ["Genouilleret", "Genouillet Noir", "Moret Noir"],
-        "description": "Recently rescued central French vine.",
-        "color": "black",
+        "synonyms": [
+            "Genouilleret",
+            "Genouillet Noir",
+            "Moret Noir"
+        ],
+        "description": {
+            "default": "Recently rescued central French vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gibi",
         "synonyms": [
             "Alzibib",
             "Aparia",
             "Augibi",
             "Jubi Blanc",
             "Maccabeu à Gros Grains",
             "Panse Blanche",
             "Passerille Blanche",
-            "Tercia Blanc",
+            "Tercia Blanc"
         ],
-        "description": "Ancient Spanish table grape still planted in Argentina with significant offspring.",
-        "color": "white",
+        "description": {
+            "default": "Ancient Spanish table grape still planted in Argentina with significant offspring.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ginestra",
-        "synonyms": ["Biancatenera", "Biancazita", "Ginestro", "Nocella"],
-        "description": "Minor but interesting and refreshing Campanian.",
-        "color": "white",
+        "synonyms": [
+            "Biancatenera",
+            "Biancazita",
+            "Ginestro",
+            "Nocella"
+        ],
+        "description": {
+            "default": "Minor but interesting and refreshing Campanian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Girgentina",
-        "synonyms": ["Ghirghentina", "Insolja Tal-Girgenti"],
-        "description": "The most planted Maltese variety, producing soft, light whites but under threat from Chardonnay.",
-        "color": "white",
+        "synonyms": [
+            "Ghirghentina",
+            "Insolja Tal-Girgenti"
+        ],
+        "description": {
+            "default": "The most planted Maltese variety, producing soft, light whites but under threat from Chardonnay.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Girò",
         "synonyms": [
             "Girò Comune",
             "Girò Rosso di Spagna",
             "Girone di Spagna",
-            "Zirone",
+            "Zirone"
         ],
-        "description": "Cherry-flavoured Sardinian red used to make dry, sweet and fortified wines.",
-        "color": "black",
+        "description": {
+            "default": "Cherry-flavoured Sardinian red used to make dry, sweet and fortified wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Giró Blanc",
-        "synonyms": ["Girò Roz"],
-        "description": "Recently rescued, high-quality, aromatic, full-bodied Mallorcan.",
-        "color": "pink",
+        "synonyms": [
+            "Girò Roz"
+        ],
+        "description": {
+            "default": "Recently rescued, high-quality, aromatic, full-bodied Mallorcan.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Glavinuša",
-        "synonyms": ["Carnjenak", "Glavanjuša", "Glavinka", "Okatac", "Okatac Crni"],
-        "description": "Very rare Croatian variety sometimes useful for the Dalmatian sweet wine Prošek.",
-        "color": "black",
+        "synonyms": [
+            "Carnjenak",
+            "Glavanjuša",
+            "Glavinka",
+            "Okatac",
+            "Okatac Crni"
+        ],
+        "description": {
+            "default": "Very rare Croatian variety sometimes useful for the Dalmatian sweet wine Prošek.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Godello",
         "synonyms": [
             "Agodello",
             "Agodenho",
             "Agudanho",
@@ -4182,68 +6622,107 @@
             "Godella",
             "Godenho",
             "Gouveio",
             "Ojo de Gallo",
             "Prieto Picudo Blanco",
             "Trincadente",
             "Verdelho",
-            "Verdelho do Dão",
+            "Verdelho do Dão"
         ],
-        "description": "Very high-quality variety undergoing a revival, under several names, in north-western Iberia.",
-        "color": "white",
+        "description": {
+            "default": "Very high-quality variety undergoing a revival, under several names, in north-western Iberia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Goldburger",
-        "synonyms": ["Klosterneuburg 16-8", "Orangeriesling"],
-        "description": "Generally unexciting pale Austrian cross used mainly for sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Klosterneuburg 16-8",
+            "Orangeriesling"
+        ],
+        "description": {
+            "default": "Generally unexciting pale Austrian cross used mainly for sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Golden Muscat",
-        "synonyms": ["New York 10303"],
-        "description": "Minor American hybrid producing grapey dessert wines.",
-        "color": "white",
+        "synonyms": [
+            "New York 10303"
+        ],
+        "description": {
+            "default": "Minor American hybrid producing grapey dessert wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Goldriesling",
         "synonyms": [
             "Franzosentraube",
             "Gelbriesling",
             "Goldmuskat",
             "Riesling Doré",
             "Risling Khativ",
-            "Risling Zolotistyi",
+            "Risling Zolotistyi"
         ],
-        "description": "Alsace cross producing light, white quaffing wine, now a speciality of Sachsen in eastern Germany.",
-        "color": "white",
+        "description": {
+            "default": "Alsace cross producing light, white quaffing wine, now a speciality of Sachsen in eastern Germany.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Golubok",
-        "synonyms": ["Golubuk"],
-        "description": "Red-fleshed Ukrainian hybrid also found in Russia.",
-        "color": "black",
+        "synonyms": [
+            "Golubuk"
+        ],
+        "description": {
+            "default": "Red-fleshed Ukrainian hybrid also found in Russia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gorgollasa",
-        "synonyms": ["Gargollasa", "Gargollosa", "Gorgollosa"],
-        "description": "Recently resurrected, high-quality, red-fruited Mallorcan.",
-        "color": "black",
+        "synonyms": [
+            "Gargollasa",
+            "Gargollosa",
+            "Gorgollosa"
+        ],
+        "description": {
+            "default": "Recently resurrected, high-quality, red-fruited Mallorcan.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Goruli Mtsvane",
         "synonyms": [
             "Goruli Mcvané",
             "Kvishkhuri",
             "Mtsvane",
             "Mtsvané",
             "Suramula",
-            "Tetrpotola",
+            "Tetrpotola"
         ],
-        "description": "Fresh, fruity, light-skinned Georgian variety used to make both still and sparkling wines.",
-        "color": "white",
+        "description": {
+            "default": "Fresh, fruity, light-skinned Georgian variety used to make both still and sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gouais Blanc",
         "synonyms": [
             "Belina",
             "Belina Drobna",
             "Best’s no 4",
@@ -4264,55 +6743,74 @@
             "Krapinska Belina",
             "Liseiret",
             "Plant de Séchex",
             "Président",
             "Preveiral",
             "Provereau Blanc",
             "Weisser Heunisch",
-            "Wippacher",
+            "Wippacher"
         ],
-        "description": "Extremely important progenitor (with Pinot) even if almost extinct.",
-        "color": "white",
+        "description": {
+            "default": "Extremely important progenitor (with Pinot) even if almost extinct.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gouget Noir",
         "synonyms": [
             "Gouge Noir",
             "Gouget",
             "Goujet",
             "Lyonnais",
             "Nérou",
             "Neyran",
-            "Neyrou",
+            "Neyrou"
         ],
-        "description": "Rare and disappearing central French vine.",
-        "color": "black",
+        "description": {
+            "default": "Rare and disappearing central French vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Goustolidi",
         "synonyms": [
             "Augoustelidi",
             "Augoustelli",
             "Avgoustolidi",
             "Bostilidas",
             "Goustoulidi",
             "Goystolidi",
             "Rompola",
             "Vostilidi",
             "Vostilida",
-            "Voustolidi",
+            "Voustolidi"
         ],
-        "description": "Traditional, rustic Greek variety.",
-        "color": "white",
+        "description": {
+            "default": "Traditional, rustic Greek variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gr 7",
-        "synonyms": ["Geneva Red 7", "NY 34791"],
-        "description": "Minor but sturdy, winter-hardy complex American hybrid used mostly in blends.",
-        "color": "black",
+        "synonyms": [
+            "Geneva Red 7",
+            "NY 34791"
+        ],
+        "description": {
+            "default": "Minor but sturdy, winter-hardy complex American hybrid used mostly in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Graciano",
         "synonyms": [
             "Bovale",
             "Bovale Sardo",
             "Bovaleddu",
@@ -4329,58 +6827,74 @@
             "Morastell",
             "Morrastel",
             "Moristell",
             "Muristellu",
             "Tinta Miúda",
             "Tintilla de Rota",
             "Xeres",
-            "and many more",
+            "and many more"
         ],
-        "description": "Low-yielding, richly coloured, perfumed variety that retains acidity and is regaining favour in Rioja.",
-        "color": "black",
+        "description": {
+            "default": "Low-yielding, richly coloured, perfumed variety that retains acidity and is regaining favour in Rioja.",
+            "julie": "Graciano is a fragrant, fresh and sometimes spicy grape variety that is most often blended with other grape varieties to add brightness and perfume. It is regularly used in the region of Rioja. Graciano is also fashionable in Sardinia where it is called Bovale Sardo or Cagnulari.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Graisse",
         "synonyms": [
             "Blanquette Grise",
             "Chalosse",
             "Gras",
             "Gras Blanc",
             "Grèce Blanche",
             "Plant de Graisse",
             "Plant de Grèce",
             "Président",
             "Ramassou Blanc",
-            "Tizourine Bou-Afrara",
+            "Tizourine Bou-Afrara"
         ],
-        "description": "Minor south-west French variety used mostly for armagnac.",
-        "color": "white",
+        "description": {
+            "default": "Minor south-west French variety used mostly for armagnac.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Grand Noir",
         "synonyms": [
             "Gran Negro",
             "Grand Bouschet",
             "Grand Noir de la Calmette",
             "Gros Noir",
-            "Sumo Tinto",
+            "Sumo Tinto"
         ],
-        "description": "Pale red-fleshed nineteenth-century French cross with potential. Still found around the world.",
-        "color": "black",
+        "description": {
+            "default": "Pale red-fleshed nineteenth-century French cross with potential. Still found around the world.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Grapariol",
         "synonyms": [
             "Grappariol",
             "Rabosa Bianca",
             "Rabosina Bianca",
-            "Rabosino Grappariol",
+            "Rabosino Grappariol"
         ],
-        "description": "Veneto variety recently rescued from extinction.",
-        "color": "white",
+        "description": {
+            "default": "Veneto variety recently rescued from extinction.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Grasă De Cotnari",
         "synonyms": [
             "Bajor",
             "Fehér Kövérszőlő",
             "Fejérszőlő",
@@ -4389,18 +6903,22 @@
             "Grasă de Cotnar",
             "Grasă Mare",
             "Grasă Mică",
             "Grasi",
             "Grassa",
             "Kövérszőlő",
             "Poamă Grasă",
-            "Resertraube",
+            "Resertraube"
         ],
-        "description": "Rare Romanian variety once famous for its sweet Cotnari wines, occasionally found in those of Tokaj in Hungary.",
-        "color": "white",
+        "description": {
+            "default": "Rare Romanian variety once famous for its sweet Cotnari wines, occasionally found in those of Tokaj in Hungary.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Graševina",
         "synonyms": [
             "Borba",
             "Graševina Bijela",
             "Italian Riesling",
@@ -4412,93 +6930,152 @@
             "Rismi",
             "Rismi",
             "Risli",
             "Rizling Vlašský",
             "Ryzlink Vlašský",
             "Taljanska Graševina",
             "Wälschriesling",
-            "Welschriesling",
+            "Welschriesling"
         ],
-        "description": "Unfairly maligned variety widely planted in Central Europe that has in its time suffered in comparison to Riesling.",
-        "color": "white",
+        "description": {
+            "default": "Unfairly maligned variety widely planted in Central Europe that has in its time suffered in comparison to Riesling.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Grechetto Di Orvieto",
-        "synonyms": ["Grechetto", "Grechetto Bianco", "Grechetto Spoletino"],
-        "description": "Characterful and versatile Umbrian.",
-        "color": "white",
+        "synonyms": [
+            "Grechetto",
+            "Grechetto Bianco",
+            "Grechetto Spoletino"
+        ],
+        "description": {
+            "default": "Characterful and versatile Umbrian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Greco",
         "synonyms": [
             "Asprinio",
             "Greco del Vesuvio",
             "Greco della Torre",
             "Greco di Napoli",
             "Greco di Tufo",
-            "Grieco di Castelvenere",
+            "Grieco di Castelvenere"
         ],
-        "description": "Potentially fine, aromatic but notably firm Campanian.",
-        "color": "white",
+        "description": {
+            "default": "Potentially fine, aromatic but notably firm Campanian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Greco Bianco",
         "synonyms": [
             "Greco Bianco di Cosenza",
             "Greco Bianco di Rogliano",
-            "Pecorello Bianco",
+            "Pecorello Bianco"
         ],
-        "description": "Rare Calabrian used to make dessert wines.",
-        "color": "white",
+        "description": {
+            "default": "Rare Calabrian used to make dessert wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Greco Nero",
         "synonyms": [
             "Collective name for different varieties",
-            "so synonyms are misleading.",
+            "so synonyms are misleading."
         ],
-        "description": "A group of different Calabrians confusingly sharing one name.",
-        "color": "black",
+        "description": {
+            "default": "A group of different Calabrians confusingly sharing one name.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Grignolino",
-        "synonyms": ["Barbesino", "Barbisino", "Berbesino"],
-        "description": "Waning, distinctively pale, light, local (ancient) Monferrato speciality.",
-        "color": "black",
+        "synonyms": [
+            "Barbesino",
+            "Barbisino",
+            "Berbesino"
+        ],
+        "description": {
+            "default": "Waning, distinctively pale, light, local (ancient) Monferrato speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Grillo",
-        "synonyms": ["Ariddu", "Riddu", "Rossese Bianco"],
-        "description": "Increasingly popular high-quality, full-bodied western Sicilian white.",
-        "color": "white",
+        "synonyms": [
+            "Ariddu",
+            "Riddu",
+            "Rossese Bianco"
+        ],
+        "description": {
+            "default": "Increasingly popular high-quality, full-bodied western Sicilian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gringet",
-        "synonyms": ["Gringet Gras", "Gros Gringet", "Petit Gringet"],
-        "description": "Rare, lightly floral and high-quality variety exclusive to Savoie.",
-        "color": "white",
+        "synonyms": [
+            "Gringet Gras",
+            "Gros Gringet",
+            "Petit Gringet"
+        ],
+        "description": {
+            "default": "Rare, lightly floral and high-quality variety exclusive to Savoie.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Grisa Nera",
-        "synonyms": ["Grisa", "Grisa di Cumiana"],
-        "description": "Old and rare Piemontese.",
-        "color": "black",
+        "synonyms": [
+            "Grisa",
+            "Grisa di Cumiana"
+        ],
+        "description": {
+            "default": "Old and rare Piemontese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Grk",
         "synonyms": [
             "Gark",
             "Grk Bijeli",
             "Grk Korčulanski",
             "Grk Mali",
             "Grk Veli",
-            "Lumbarajski Grk",
+            "Lumbarajski Grk"
         ],
-        "description": "Rare, high-quality and highly localized island white from Croatia.",
-        "color": "white",
+        "description": {
+            "default": "Rare, high-quality and highly localized island white from Croatia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Grolleau Noir",
         "synonyms": [
             "Bourdalès",
             "Gamay de Châtillon",
             "Gamay Groslot",
@@ -4507,153 +7084,258 @@
             "Grolleau des Mahé",
             "Grolleau de Tours",
             "Groslot",
             "Gros-Lot",
             "Groslot de Vallères",
             "Groslot Noir",
             "Moinard",
-            "Pineau de Saumur",
+            "Pineau de Saumur"
         ],
-        "description": "Widely planted though little recognized dark-skinned Loire variety that makes a lot of rosé and some supple reds.",
-        "color": "black",
+        "description": {
+            "default": "Widely planted though little recognized dark-skinned Loire variety that makes a lot of rosé and some supple reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Groppello Di Mocasina",
-        "synonyms": ["Groppello di San Stefano", "Groppello Moliner"],
-        "description": "Minor northern Italian whose wine is generally blended.",
-        "color": "black",
+        "synonyms": [
+            "Groppello di San Stefano",
+            "Groppello Moliner"
+        ],
+        "description": {
+            "default": "Minor northern Italian whose wine is generally blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Groppello Di Revò",
-        "synonyms": ["Gropel", "Gropel Nones", "Groppello Anaune"],
-        "description": "Very minor northern Italian that was far more popular in the eighteenth and nineteenth centuries.",
-        "color": "black",
+        "synonyms": [
+            "Gropel",
+            "Gropel Nones",
+            "Groppello Anaune"
+        ],
+        "description": {
+            "default": "Very minor northern Italian that was far more popular in the eighteenth and nineteenth centuries.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Groppello Gentile",
-        "synonyms": ["Groppella", "Groppello Comune", "Groppellone"],
-        "description": "Ancient, usually blended, northern Italian red.",
-        "color": "black",
+        "synonyms": [
+            "Groppella",
+            "Groppello Comune",
+            "Groppellone"
+        ],
+        "description": {
+            "default": "Ancient, usually blended, northern Italian red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gros Manseng",
         "synonyms": [
             "Gros Mansenc",
             "Izkiriot Haundi",
             "Iskiriota Zuri Handia",
-            "Manseng Gros Blanc",
+            "Manseng Gros Blanc"
         ],
-        "description": "Full-flavoured, thick-skinned white speciality of the far south west of France.",
-        "color": "white",
+        "description": {
+            "default": "Full-flavoured, thick-skinned white speciality of the far south west of France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gros Verdot",
-        "synonyms": ["Hère", "Plant des Palus", "Verdot Colon"],
-        "description": "Very minor dark-skinned variety inferior to Petit Verdot.",
-        "color": "black",
+        "synonyms": [
+            "Hère",
+            "Plant des Palus",
+            "Verdot Colon"
+        ],
+        "description": {
+            "default": "Very minor dark-skinned variety inferior to Petit Verdot.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Grossa",
-        "synonyms": ["Tinta Grossa"],
-        "description": "Alentejo variety used to improve red blends.",
-        "color": "black",
+        "synonyms": [
+            "Tinta Grossa"
+        ],
+        "description": {
+            "default": "Alentejo variety used to improve red blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gruaja",
         "synonyms": [
             "Crovaja",
             "Cruaia",
             "Cruara",
             "Cruvaio",
             "Gruaia",
             "Gruaio",
-            "Gruajo",
+            "Gruajo"
         ],
-        "description": "Rescued from extinction in northern Italy in the early 1990s but still very rare.",
-        "color": "black",
+        "description": {
+            "default": "Rescued from extinction in northern Italy in the early 1990s but still very rare.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Grüner Veltliner",
         "synonyms": [
             "Grauer Veltliner",
             "Grün Muskateller",
             "Veltliner",
             "Veltliner Grau",
             "Veltliner Grün",
             "Veltlinske Zelené",
             "Veltlinské Zelené",
             "Weissgipfler",
             "Zeleni Veltinec",
-            "Zöld Veltlini",
+            "Zöld Veltlini"
         ],
-        "description": "Fashionable, versatile, top-quality Austrian white wine variety.",
-        "color": "white",
+        "description": {
+            "default": "Fashionable, versatile, top-quality Austrian white wine variety.",
+            "julie": "Grüner Veltliner is the most planted grape variety of Austria. The variety can produce wines that range from light, crisp and fruity to full-bodied, complex, mineral and textural with a fabulous ageing potential. ",
+            "sommelier": """Austria's most significant white wine variety is Grüner Veltliner, which most probably derives from a crossing with Traminer. The second parent remains unconfirmed, but it is thought to be a Century old variety discovered in St. Georgen in Burgenland. Grüner Veltliner is not genetically related to Roter Veltliner or Frühroter Veltliner. Grüner Veltliner delivers all quality levels – from light, more acidic wines, through to Prädikatswein with a high degree of ripeness. Quality is highly dependent upon the vineyard and the yield. Winegrowers strive for spicy, peppery wines, or wines with notes of stone fruit."""
+        },
+        "color": "white"
     },
     {
         "name": "Guardavalle",
         "synonyms": [
             "Greco Bianco di Cirò",
             "Greco del Cirotano",
             "Montonico di Rogliano",
             "Uva da Passito",
             "Uva Greca",
-            "Vardavalli",
+            "Vardavalli"
         ],
-        "description": "Makes a minor, nutty white in Italy’s deep south.",
-        "color": "white",
+        "description": {
+            "default": "Makes a minor, nutty white in Italy’s deep south.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Gueuche Noir",
-        "synonyms": ["Foirard", "Foirard Noir", "Plant d’Arlay", "Plant de Treffort"],
-        "description": "Virtually extinct, late-ripening variety from eastern France, related to Gouais Blanc.",
-        "color": "black",
+        "synonyms": [
+            "Foirard",
+            "Foirard Noir",
+            "Plant d’Arlay",
+            "Plant de Treffort"
+        ],
+        "description": {
+            "default": "Virtually extinct, late-ripening variety from eastern France, related to Gouais Blanc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Gutenborner",
-        "synonyms": ["Geisenheim 17-52"],
-        "description": "Minor German cross with very limited plantings in the UK.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 17-52"
+        ],
+        "description": {
+            "default": "Minor German cross with very limited plantings in the UK.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Hamashara",
-        "synonyms": ["Aronova Boroda", "Gamashara"],
-        "description": "Early-ripening Azeri red wine grape.",
-        "color": "black",
+        "synonyms": [
+            "Aronova Boroda",
+            "Gamashara"
+        ],
+        "description": {
+            "default": "Early-ripening Azeri red wine grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Hárslevelű",
         "synonyms": [
             "Budai Féher",
             "Feuille de Tilleul",
             "Harslevleue",
             "Harzevelu",
             "Lindenblättrige",
             "Lipolist",
-            "Lipovina",
+            "Lipovina"
         ],
-        "description": "Aromatic, descriptively named Hungarian variety used for both sweet and dry whites.",
-        "color": "white",
+        "description": {
+            "default": "Aromatic, descriptively named Hungarian variety used for both sweet and dry whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Hasandede",
-        "synonyms": ["Ahmet Bey", "Aşeri", "Hasan Dede", "Hasandede Beyazi"],
-        "description": "Humdrum Turkish variety found east of the capital, Ankara.",
-        "color": "white",
+        "synonyms": [
+            "Ahmet Bey",
+            "Aşeri",
+            "Hasan Dede",
+            "Hasandede Beyazi"
+        ],
+        "description": {
+            "default": "Humdrum Turkish variety found east of the capital, Ankara.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Helfensteiner",
-        "synonyms": ["Blauer Weinsberger", "Weinsberg S 5332"],
-        "description": "German cross eclipsed by its offspring Dornfelder.",
-        "color": "red",
+        "synonyms": [
+            "Blauer Weinsberger",
+            "Weinsberg S 5332"
+        ],
+        "description": {
+            "default": "German cross eclipsed by its offspring Dornfelder.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Helios",
-        "synonyms": ["Freiburg 242-73"],
-        "description": "Little-known, very complex, disease-resistant German hybrid.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 242-73"
+        ],
+        "description": {
+            "default": "Little-known, very complex, disease-resistant German hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Herbemont",
         "synonyms": [
             "Black Herbemont",
             "Bottsi",
             "Brown French",
@@ -4664,169 +7346,285 @@
             "Kay’s Seedling",
             "Madeira",
             "Mcknee",
             "Neal Grape",
             "Neil Grape",
             "Warren",
             "Warrenton",
-            "White Herbemont",
+            "White Herbemont"
         ],
-        "description": "Almost extinct American hybrid with a complex and disputed parentage.",
-        "color": "black",
+        "description": {
+            "default": "Almost extinct American hybrid with a complex and disputed parentage.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Heroldrebe",
-        "synonyms": ["Weinsberg S 130"],
-        "description": "Unexceptional, productive but inconveniently late-ripening German cross.",
-        "color": "black",
+        "synonyms": [
+            "Weinsberg S 130"
+        ],
+        "description": {
+            "default": "Unexceptional, productive but inconveniently late-ripening German cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Hetera",
-        "synonyms": ["HTCVCB 4/13"],
-        "description": "Recently authorized Slovakian cross making promising sweet wines.",
-        "color": "red",
+        "synonyms": [
+            "HTCVCB 4/13"
+        ],
+        "description": {
+            "default": "Recently authorized Slovakian cross making promising sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Hibernal",
-        "synonyms": ["Geisenheim 322-58"],
-        "description": "German hybrid planted more widely in the Czech Republic than at home.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 322-58"
+        ],
+        "description": {
+            "default": "German hybrid planted more widely in the Czech Republic than at home.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Hitzkircher",
-        "synonyms": ["Grosse Blaue Mörsch", "Hitzkirchener", "Hitzkirchler"],
-        "description": "Swiss rarity found only in the village after which it was named.",
-        "color": "black",
+        "synonyms": [
+            "Grosse Blaue Mörsch",
+            "Hitzkirchener",
+            "Hitzkirchler"
+        ],
+        "description": {
+            "default": "Swiss rarity found only in the village after which it was named.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Hölder",
-        "synonyms": ["Hoelder", "Weinsberg S 397"],
-        "description": "Very minor, distinctly ordinary German cross.",
-        "color": "white",
+        "synonyms": [
+            "Hoelder",
+            "Weinsberg S 397"
+        ],
+        "description": {
+            "default": "Very minor, distinctly ordinary German cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Hondarribi Beltza",
         "synonyms": [
             "Chacolí",
             "Cruchen Nègre",
             "Hondarrabi Beltza",
             "Kurixketu Beltza",
             "Ondarrabi Beltza",
             "Txakoli",
             "Verde Matza",
-            "Xerratu Beltza",
+            "Xerratu Beltza"
         ],
-        "description": "Rare speciality of northern Spain’s Basque Country related to, and sometimes reminiscent of, Cabernet Franc.",
-        "color": "black",
+        "description": {
+            "default": "Rare speciality of northern Spain’s Basque Country related to, and sometimes reminiscent of, Cabernet Franc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Horozkarasi",
-        "synonyms": ["Horoz Karası"],
-        "description": "A stay-at-home variety used more for the table than for wine.",
-        "color": "black",
+        "synonyms": [
+            "Horoz Karası"
+        ],
+        "description": {
+            "default": "A stay-at-home variety used more for the table than for wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Hron",
-        "synonyms": ["CAAB 3/22"],
-        "description": "Recent but promising Slovakian cross producing full-bodied, ageworthy reds.",
-        "color": "black",
+        "synonyms": [
+            "CAAB 3/22"
+        ],
+        "description": {
+            "default": "Recent but promising Slovakian cross producing full-bodied, ageworthy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Hrvatica",
         "synonyms": [
             "Hrvatica Crna",
             "Jarbola",
             "Karbonera",
             "Markolina",
             "Negrara",
-            "Negrona",
+            "Negrona"
         ],
-        "description": "Recently rescued Croatian variety making pale reds.",
-        "color": "black",
+        "description": {
+            "default": "Recently rescued Croatian variety making pale reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Humagne",
         "synonyms": [
             "Humagne Blanc",
             "Humagne Blanche",
             "Miousat",
             "Miousap",
-            "Mioussat",
+            "Mioussat"
         ],
-        "description": "Ancient, tangy Swiss variety recently revived in the Valais.",
-        "color": "white",
+        "description": {
+            "default": "Ancient, tangy Swiss variety recently revived in the Valais.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Huxelrebe",
-        "synonyms": ["Alzey S. 3962"],
-        "description": "German cross scores highly for yields, ripeness, aroma and acidity but not for subtlety.",
-        "color": "white",
+        "synonyms": [
+            "Alzey S. 3962"
+        ],
+        "description": {
+            "default": "German cross scores highly for yields, ripeness, aroma and acidity but not for subtlety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Incrocio Bianco Fedit 51",
-        "synonyms": ["Fedit 51"],
-        "description": "Rare Veneto 1950s white cross good for passito wines.",
-        "color": "white",
+        "synonyms": [
+            "Fedit 51"
+        ],
+        "description": {
+            "default": "Rare Veneto 1950s white cross good for passito wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Incrocio Bruni 54",
-        "synonyms": ["Dorico", "Sauvignon × Verdicchio"],
-        "description": "Minor but high-yielding central Italian white cross that generally disappears into blends.",
-        "color": "white",
+        "synonyms": [
+            "Dorico",
+            "Sauvignon × Verdicchio"
+        ],
+        "description": {
+            "default": "Minor but high-yielding central Italian white cross that generally disappears into blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Incrocio Manzoni 2.15",
-        "synonyms": ["Manzoni Nero", "Prosecco × Cabernet Sauvignon 2-15"],
-        "description": "Very minor black-skinned cross confined to the Veneto in northern Italy.",
-        "color": "black",
+        "synonyms": [
+            "Manzoni Nero",
+            "Prosecco × Cabernet Sauvignon 2-15"
+        ],
+        "description": {
+            "default": "Very minor black-skinned cross confined to the Veneto in northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Incrocio Terzi 1",
-        "synonyms": ["Barbera × Cabernet Franc 1"],
-        "description": "Minor Lombardia crossing that disappears into blends.",
-        "color": "black",
+        "synonyms": [
+            "Barbera × Cabernet Franc 1"
+        ],
+        "description": {
+            "default": "Minor Lombardia crossing that disappears into blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Invernenga",
-        "synonyms": ["Invernesca", "Ua’mbrunesca"],
-        "description": "Old and rare Brescia white, ideal for drying off the vine.",
-        "color": "white",
+        "synonyms": [
+            "Invernesca",
+            "Ua’mbrunesca"
+        ],
+        "description": {
+            "default": "Old and rare Brescia white, ideal for drying off the vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Inzolia",
         "synonyms": [
             "Ansolica",
             "Ansonica",
             "Ansora",
             "Anzonica",
             "Insolia",
             "Insolia di Palermo",
             "Insora",
             "’Nzolia",
-            "Zolia Bianca",
+            "Zolia Bianca"
         ],
-        "description": "Nutty Sicilian white.",
-        "color": "white",
+        "description": {
+            "default": "Nutty Sicilian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Iri Kara",
-        "synonyms": ["Arikaras", "Focea", "Fodja"],
-        "description": "Very minor, mediocre, pink-skinned Turkish variety.",
-        "color": "pink",
+        "synonyms": [
+            "Arikaras",
+            "Focea",
+            "Fodja"
+        ],
+        "description": {
+            "default": "Very minor, mediocre, pink-skinned Turkish variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Irsai Olivér",
         "synonyms": [
             "Irsay Oliver",
             "Irsay Oliver Muskotaly",
             "Muscat Oliver",
-            "Oliver Irsay",
+            "Oliver Irsay"
         ],
-        "description": "Hungarian table grape promoted to making soft, aromatic white wines.",
-        "color": "white",
+        "description": {
+            "default": "Hungarian table grape promoted to making soft, aromatic white wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Isabella",
         "synonyms": [
             "Americano",
             "Ananas",
             "Bangalore Blue",
@@ -4871,122 +7669,183 @@
             "Tzortzidika Chakidike",
             "Tzortzines",
             "Utkopro",
             "Uva Cimice",
             "Uva Fragola",
             "Vernet",
             "Woodward",
-            "Zampela",
+            "Zampela"
         ],
-        "description": "Once widely planted, old American variety now found mostly in Brazil and India.",
-        "color": "black",
+        "description": {
+            "default": "Once widely planted, old American variety now found mostly in Brazil and India.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Italia",
-        "synonyms": ["Moscatel Italia", "Moscatel Italiano", "Muscat d’Italie"],
-        "description": "Important, extremely large-berried table grape only very rarely used to make wine.",
-        "color": "white",
+        "synonyms": [
+            "Moscatel Italia",
+            "Moscatel Italiano",
+            "Muscat d’Italie"
+        ],
+        "description": {
+            "default": "Important, extremely large-berried table grape only very rarely used to make wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Italica",
-        "synonyms": ["103", "Incrocio Cosmo 103", "Verdiso × Riesling Italico 103"],
-        "description": "A 1950s white Italian cross of interest only in the province of Treviso.",
-        "color": "white",
+        "synonyms": [
+            "103",
+            "Incrocio Cosmo 103",
+            "Verdiso × Riesling Italico 103"
+        ],
+        "description": {
+            "default": "A 1950s white Italian cross of interest only in the province of Treviso.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ives",
         "synonyms": [
             "Black Ives",
             "Bôrdo",
             "Ives Madeira",
             "Ives’ Madeira Seedling",
             "Ives Seedling",
-            "Kittredge",
+            "Kittredge"
         ],
-        "description": "American hybrid that needs fresh air.",
-        "color": "black",
+        "description": {
+            "default": "American hybrid that needs fresh air.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Jacquère",
         "synonyms": [
             "Cugnette",
             "Jacquerre",
             "Jaquère",
             "Martin-Cot",
             "Molette de Montmélian",
             "Plant des Abîmes",
             "Plant des Abymes de Myans",
             "Raisin des Abîmes",
             "Redin",
             "Robinet",
-            "Roussette",
+            "Roussette"
         ],
-        "description": "Savoie speciality producing fresh, light, mountain whites.",
-        "color": "white",
+        "description": {
+            "default": "Savoie speciality producing fresh, light, mountain whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Jacquez",
         "synonyms": [
             "Black Spanish",
             "Cigar Box",
             "French Grape",
             "Jacquet",
             "Lenoir",
             "Longworth’s Ohio",
-            "Troya",
+            "Troya"
         ],
-        "description": "Once-popular American hybrid with good resistance to Pierce’s disease and now surviving mainly in Brazil and Texas.",
-        "color": "black",
+        "description": {
+            "default": "Once-popular American hybrid with good resistance to Pierce’s disease and now surviving mainly in Brazil and Texas.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Jampal",
-        "synonyms": ["Cercial", "Jampaulo", "João Paolo", "Pinheira Branca"],
-        "description": "Minor Portuguese vine recognized for its quality but not widely planted.",
-        "color": "white",
+        "synonyms": [
+            "Cercial",
+            "Jampaulo",
+            "João Paolo",
+            "Pinheira Branca"
+        ],
+        "description": {
+            "default": "Minor Portuguese vine recognized for its quality but not widely planted.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Johanniter",
-        "synonyms": ["Freiburg 177-68"],
-        "description": "Recent German hybrid with very good disease resistance.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 177-68"
+        ],
+        "description": {
+            "default": "Recent German hybrid with very good disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Juan García",
         "synonyms": [
             "Gorda",
             "Malvasía  Negra",
             "Mouratón",
             "Negrera",
             "Negrón de Aldán",
             "Nepada",
             "Tinta Gorda",
-            "Villarino",
+            "Villarino"
         ],
-        "description": "Intriguing, perfumed speciality of north-western Spain.",
-        "color": "black",
+        "description": {
+            "default": "Intriguing, perfumed speciality of north-western Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Juhfark",
-        "synonyms": ["Lämmerschwanz"],
-        "description": "Minor Hungarian variety that needs ageing and aeration to swap asperity for elegance.",
-        "color": "white",
+        "synonyms": [
+            "Lämmerschwanz"
+        ],
+        "description": {
+            "default": "Minor Hungarian variety that needs ageing and aeration to swap asperity for elegance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Jurançon Blanc",
         "synonyms": [
             "Braquet",
             "Dame Blanc",
             "Plant de Dame",
             "Plant Debout",
             "Quillat",
             "Quillard",
-            "Secal",
+            "Secal"
         ],
-        "description": "Inferior and increasingly neglected variety traditionally used as a base for spirits.",
-        "color": "white",
+        "description": {
+            "default": "Inferior and increasingly neglected variety traditionally used as a base for spirits.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Jurançon Noir",
         "synonyms": [
             "Chalosse Noire",
             "Dame Noire",
             "Plant de Dame",
@@ -4996,36 +7855,62 @@
             "Folle Rouge",
             "Gouni",
             "Jurançon Rouge",
             "Luxuriant",
             "Piquepout Rouge",
             "Quillat",
             "Quillard",
-            "Vidiella",
+            "Vidiella"
         ],
-        "description": "South-west French variety producing light wines but rapidly losing ground.",
-        "color": "black",
+        "description": {
+            "default": "South-west French variety producing light wines but rapidly losing ground.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Juwel",
-        "synonyms": ["Jewel", "Weinsberg S 378"],
-        "description": "Modern German cross with patchy disease resistance.",
-        "color": "white",
+        "synonyms": [
+            "Jewel",
+            "Weinsberg S 378"
+        ],
+        "description": {
+            "default": "Modern German cross with patchy disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kabar",
-        "synonyms": ["Tarcal 10"],
-        "description": "Recent Hungarian cross designed for Tokaj.",
-        "color": "white",
+        "synonyms": [
+            "Tarcal 10"
+        ],
+        "description": {
+            "default": "Recent Hungarian cross designed for Tokaj.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kachichi",
-        "synonyms": ["Abkhazouri", "Kagigi", "Katchitchi", "Katcitci"],
-        "description": "Minor variety producing deep red wines in north-western Georgia.",
-        "color": "black",
+        "synonyms": [
+            "Abkhazouri",
+            "Kagigi",
+            "Katchitchi",
+            "Katcitci"
+        ],
+        "description": {
+            "default": "Minor variety producing deep red wines in north-western Georgia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kadarka",
         "synonyms": [
             "Branicevka",
             "Cadarcă",
             "Cadarcă Neagră",
@@ -5037,249 +7922,422 @@
             "Gumza",
             "Gymza",
             "Kadarka Kék",
             "Kallmet",
             "Lugojană",
             "Skadarka",
             "Törökszőlő",
-            "Varnenska Gimza",
+            "Varnenska Gimza"
         ],
-        "description": "Variety of uncertain origin producing gentle, fresh reds in Eastern Europe.",
-        "color": "black",
+        "description": {
+            "default": "Variety of uncertain origin producing gentle, fresh reds in Eastern Europe.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kakhet",
-        "synonyms": ["Cakhete", "Kachet", "Kakheti"],
-        "description": "Possibly Georgian grape best known for the sweet Kagor reds in Armenia.",
-        "color": "black",
+        "synonyms": [
+            "Cakhete",
+            "Kachet",
+            "Kakheti"
+        ],
+        "description": {
+            "default": "Possibly Georgian grape best known for the sweet Kagor reds in Armenia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kakotrygis",
-        "synonyms": ["Kako Tryghi", "Kakotriguis", "Kakotriki", "Kakotryghis"],
-        "description": "Very minor variety found on the Greek island of Kérkyra (Corfu).",
-        "color": "white",
+        "synonyms": [
+            "Kako Tryghi",
+            "Kakotriguis",
+            "Kakotriki",
+            "Kakotryghis"
+        ],
+        "description": {
+            "default": "Very minor variety found on the Greek island of Kérkyra (Corfu).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kangun",
-        "synonyms": ["2-17-22", "Cangoune", "Kangoon", "Kangoun"],
-        "description": "Armenian complex hybrid used to produce brandy and sweet, fortified whites.",
-        "color": "white",
+        "synonyms": [
+            "2-17-22",
+            "Cangoune",
+            "Kangoon",
+            "Kangoun"
+        ],
+        "description": {
+            "default": "Armenian complex hybrid used to produce brandy and sweet, fortified whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kanzler",
-        "synonyms": ["Alzey S 3983"],
-        "description": "Low-yielding and declining German cross.",
-        "color": "white",
+        "synonyms": [
+            "Alzey S 3983"
+        ],
+        "description": {
+            "default": "Low-yielding and declining German cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kapistoni Tetri",
         "synonyms": [
             "Capistoni Tetri",
             "Kabistoni Tetri",
             "Kapistona",
             "Kapistoni",
-            "Zekroula Kapistoni",
+            "Zekroula Kapistoni"
         ],
-        "description": "Ancient Georgian variety responsible for still and sparkling wines.",
-        "color": "white",
+        "description": {
+            "default": "Ancient Georgian variety responsible for still and sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kapitan Jani Kara",
         "synonyms": [
             "Adzhi Ibram Kara",
             "Agii Ibram",
             "Capitan Kara",
             "Chaban Khalil Kara",
             "Kapitan Yani Kara",
-            "Ridzhaga",
+            "Ridzhaga"
         ],
-        "description": "Minor Ukrainian component in sweet red blends.",
-        "color": "black",
+        "description": {
+            "default": "Minor Ukrainian component in sweet red blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kapselsky",
         "synonyms": [
             "Kapsel Skii",
             "Kapselski",
             "Kapselskii",
             "Matvienkovsky",
-            "SD-62",
+            "SD-62"
         ],
-        "description": "Minor Ukrainian white.",
-        "color": "white",
+        "description": {
+            "default": "Minor Ukrainian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Karalahna",
-        "synonyms": ["Kara Lahna", "Lahna Kara"],
-        "description": "Found mainly on the Turkish island of Bozcaada in the Aegean, makes tannic but fresh reds.",
-        "color": "black",
+        "synonyms": [
+            "Kara Lahna",
+            "Lahna Kara"
+        ],
+        "description": {
+            "default": "Found mainly on the Turkish island of Bozcaada in the Aegean, makes tannic but fresh reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Karasakiz",
         "synonyms": [
             "Kara Sakız",
             "Karakız",
             "Karassakýz",
             "Kuntra",
             "Makbule",
             "Mavrupalya",
-            "Sakız Kara",
+            "Sakız Kara"
         ],
-        "description": "Turkish variety making soft, light reds and being overtaken by the likes of Cabernet and Merlot.",
-        "color": "black",
+        "description": {
+            "default": "Turkish variety making soft, light reds and being overtaken by the likes of Cabernet and Merlot.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Karmrahyut",
-        "synonyms": ["Karmrahiut", "Karmraiute"],
-        "description": "Dark-skinned, red-fleshed Armenian hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Karmrahiut",
+            "Karmraiute"
+        ],
+        "description": {
+            "default": "Dark-skinned, red-fleshed Armenian hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Karnachalades",
-        "synonyms": ["Karnachalas"],
-        "description": "Very rare variety from north-eastern Greece.",
-        "color": "black",
+        "synonyms": [
+            "Karnachalas"
+        ],
+        "description": {
+            "default": "Very rare variety from north-eastern Greece.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Katsakoulias",
         "synonyms": [
             "Gyftokoritho",
             "Kaltsakouli",
             "Kartsakouli",
             "Katsacoul",
             "Katsakouli",
-            "Katsakoulia",
+            "Katsakoulia"
         ],
-        "description": "Rare Greek variety almost exclusive to the island of Zákynthos.",
-        "color": "black",
+        "description": {
+            "default": "Rare Greek variety almost exclusive to the island of Zákynthos.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Katsano",
-        "synonyms": ["Katsamon"],
-        "description": "Rare variety just surviving on Santoríni.",
-        "color": "white",
+        "synonyms": [
+            "Katsamon"
+        ],
+        "description": {
+            "default": "Rare variety just surviving on Santoríni.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kay Gray",
-        "synonyms": ["Elmer Swenson 1-63", "ES 1-63"],
-        "description": "Minor and not terribly successful American hybrid.",
-        "color": "white",
+        "synonyms": [
+            "Elmer Swenson 1-63",
+            "ES 1-63"
+        ],
+        "description": {
+            "default": "Minor and not terribly successful American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kefessiya",
         "synonyms": [
             "Cefecia",
             "Cefesia",
             "Doktorsky Chernyi",
             "Kefe Izyum",
             "Kefesia",
             "Kefesiya",
-            "Kethessia",
+            "Kethessia"
         ],
-        "description": "Late-ripening variety from southern Ukraine that needs help to reproduce.",
-        "color": "black",
+        "description": {
+            "default": "Late-ripening variety from southern Ukraine that needs help to reproduce.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kéknyelű",
-        "synonyms": ["Blaustängler"],
-        "description": "Rare, potentially high-quality western Hungarian variety producing fragrant, high-acid whites.",
-        "color": "white",
+        "synonyms": [
+            "Blaustängler"
+        ],
+        "description": {
+            "default": "Rare, potentially high-quality western Hungarian variety producing fragrant, high-acid whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Keratsuda",
         "synonyms": [
             "Breza",
             "Breznik",
             "Govedina",
             "Keratsouda",
             "Keratuda",
             "Mirizlivka",
-            "Tsarevitsa",
+            "Tsarevitsa"
         ],
-        "description": "Minor Bulgarian variety making simple whites in the Struma Valley.",
-        "color": "white",
+        "description": {
+            "default": "Minor Bulgarian variety making simple whites in the Struma Valley.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kerner",
-        "synonyms": ["Weinsberg S 2530"],
-        "description": "Qualitatively the most successful modern German cross, versatile, producing Riesling-like wines.",
-        "color": "white",
+        "synonyms": [
+            "Weinsberg S 2530"
+        ],
+        "description": {
+            "default": "Qualitatively the most successful modern German cross, versatile, producing Riesling-like wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Khikhvi",
-        "synonyms": ["Chichvi", "Djananura", "Janaani", "Jananura", "Khichvi"],
-        "description": "Rare Georgian variety used for both dry and sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Chichvi",
+            "Djananura",
+            "Janaani",
+            "Jananura",
+            "Khichvi"
+        ],
+        "description": {
+            "default": "Rare Georgian variety used for both dry and sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Khindogni",
         "synonyms": [
             "Chindogni",
             "Khendorni",
             "Khindogny",
             "Khndogni",
             "Scireni",
-            "Sveni",
+            "Sveni"
         ],
-        "description": "Versatile grape from the southern Caucasus used to make just about every style of red wine.",
-        "color": "black",
+        "description": {
+            "default": "Versatile grape from the southern Caucasus used to make just about every style of red wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Királyleányka",
-        "synonyms": ["Dánosi Leányka"],
-        "description": "Hungarian variety producing light, aromatic whites.",
-        "color": "white",
+        "synonyms": [
+            "Dánosi Leányka"
+        ],
+        "description": {
+            "default": "Hungarian variety producing light, aromatic whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kisi",
-        "synonyms": ["Kissi", "Maghranuli"],
-        "description": "Floral-scented Georgian variety made in both modern and traditional styles.",
-        "color": "white",
+        "synonyms": [
+            "Kissi",
+            "Maghranuli"
+        ],
+        "description": {
+            "default": "Floral-scented Georgian variety made in both modern and traditional styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Klarnica",
-        "synonyms": ["Klarna Mieja", "Klarnca", "Klarnitza", "Mejina"],
-        "description": "Minor but characterful Slovenian variety making sweet-smelling whites.",
-        "color": "white",
+        "synonyms": [
+            "Klarna Mieja",
+            "Klarnca",
+            "Klarnitza",
+            "Mejina"
+        ],
+        "description": {
+            "default": "Minor but characterful Slovenian variety making sweet-smelling whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Knipperlé",
         "synonyms": [
             "Ettlinger",
             "Gelber Ortlieber",
             "Kleiner Räuschling",
             "Kniperlé",
             "Ortlieber",
             "Petit Mielleux",
             "Petit Räuschling",
             "Reichenweiherer",
             "Strassburger",
             "Türckheimer",
-            "Wesser Ortlieber",
+            "Wesser Ortlieber"
         ],
-        "description": "Light-skinned, rot-prone Alsace variety on the way out.",
-        "color": "white",
+        "description": {
+            "default": "Light-skinned, rot-prone Alsace variety on the way out.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kok Pandas",
-        "synonyms": ["Coc Pandas", "Kok Pandasse", "Pandas Kok", "Tken Izyum"],
-        "description": "Vine making full-bodied whites in southern Ukraine.",
-        "color": "white",
+        "synonyms": [
+            "Coc Pandas",
+            "Kok Pandasse",
+            "Pandas Kok",
+            "Tken Izyum"
+        ],
+        "description": {
+            "default": "Vine making full-bodied whites in southern Ukraine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kokur Bely",
-        "synonyms": ["Belji Dolgi", "Dolgi", "Kokour Blanc", "Kokuri Belji"],
-        "description": "Multi-purpose Ukrainian variety with possible Greek origins.",
-        "color": "white",
+        "synonyms": [
+            "Belji Dolgi",
+            "Dolgi",
+            "Kokour Blanc",
+            "Kokuri Belji"
+        ],
+        "description": {
+            "default": "Multi-purpose Ukrainian variety with possible Greek origins.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kolindrino",
-        "synonyms": ["Kolindros"],
-        "description": "Rare Greek variety named after its place of origin.",
-        "color": "black",
+        "synonyms": [
+            "Kolindros"
+        ],
+        "description": {
+            "default": "Rare Greek variety named after its place of origin.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Korinthiaki",
         "synonyms": [
             "Alga Passera",
             "Black Corinth",
             "Corinthe Noir",
@@ -5293,373 +8351,689 @@
             "Lianorogi",
             "Mavri Stafis",
             "Passerilla",
             "Passula di Corinto",
             "Raisin de Corinthe",
             "Stafida",
             "Stafidambelo",
-            "Zante Currant",
+            "Zante Currant"
         ],
-        "description": "The currant grape.",
-        "color": "black",
+        "description": {
+            "default": "The currant grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Koriostafylo",
-        "synonyms": ["Koriostaphylo"],
-        "description": "Very rare Greek variety that seems to be exclusive to the island of Ikaría.",
-        "color": "black",
+        "synonyms": [
+            "Koriostaphylo"
+        ],
+        "description": {
+            "default": "Very rare Greek variety that seems to be exclusive to the island of Ikaría.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kotsifali",
-        "synonyms": ["Kotrifali", "Kotsiphali", "Kotzifali"],
-        "description": "Oft-maligned variety widely planted on Kríti (Crete), producing soft, pale, alcoholic but potentially aromatic and distinctive reds.",
-        "color": "black",
+        "synonyms": [
+            "Kotrifali",
+            "Kotsiphali",
+            "Kotzifali"
+        ],
+        "description": {
+            "default": "Oft-maligned variety widely planted on Kríti (Crete), producing soft, pale, alcoholic but potentially aromatic and distinctive reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Koutsoumpeli",
         "synonyms": [
             "Koutsoubeli",
             "Koutsoumbeli",
             "Koutsoumbeli Kokkino",
-            "Koutsoumpeli Kokkino",
+            "Koutsoumpeli Kokkino"
         ],
-        "description": "Rare Greek pink-skinned variety.",
-        "color": "pink",
+        "description": {
+            "default": "Rare Greek pink-skinned variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Kövidinka",
         "synonyms": [
             "Dinka Alba",
             "Dinka Fehér",
             "Kevedinka",
             "Kevidinka",
             "Kövidinka Rose",
             "Rosentraube",
             "Ruzsitza",
-            "Steinschiller",
+            "Steinschiller"
         ],
-        "description": "Common pink-skinned Hungarian variety making commonplace whites.",
-        "color": "pink",
+        "description": {
+            "default": "Common pink-skinned Hungarian variety making commonplace whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Krakhuna",
-        "synonyms": ["Chkovra", "Krakhuna Shavi"],
-        "description": "Minor but well-established Georgian variety producing fresh, fruity whites.",
-        "color": "white",
+        "synonyms": [
+            "Chkovra",
+            "Krakhuna Shavi"
+        ],
+        "description": {
+            "default": "Minor but well-established Georgian variety producing fresh, fruity whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kraljevina",
-        "synonyms": ["Imbrina", "Kraljevina Crvena", "Moravina"],
-        "description": "Old Croatian variety producing simple, refreshing everyday whites.",
-        "color": "white",
+        "synonyms": [
+            "Imbrina",
+            "Kraljevina Crvena",
+            "Moravina"
+        ],
+        "description": {
+            "default": "Old Croatian variety producing simple, refreshing everyday whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Krasnostop Zolotovsky",
-        "synonyms": ["Krasnostop", "Krasnostop Anapsky"],
-        "description": "Russian variety making full-bodied dry reds as well as sweet fizz.",
-        "color": "black",
+        "synonyms": [
+            "Krasnostop",
+            "Krasnostop Anapsky"
+        ],
+        "description": {
+            "default": "Russian variety making full-bodied dry reds as well as sweet fizz.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Krassato",
-        "synonyms": ["Krasata", "Krasato"],
-        "description": "Greek variety integral to the Rapsáni appellation.",
-        "color": "black",
+        "synonyms": [
+            "Krasata",
+            "Krasato"
+        ],
+        "description": {
+            "default": "Greek variety integral to the Rapsáni appellation.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kreaca",
         "synonyms": [
             "Banat Riesling",
             "Bánáti Rizling",
             "Banatski Rizling",
             "Creaţă",
             "Creaţă de Banat",
             "Franchie",
             "Kreáca",
             "Kreatza",
             "Kriaca",
             "Riesling Banatsky",
-            "Zakkelweiss",
+            "Zakkelweiss"
         ],
-        "description": "Rare Balkan pale-skinned vine now found mainly in Serbia.",
-        "color": "white",
+        "description": {
+            "default": "Rare Balkan pale-skinned vine now found mainly in Serbia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Krkošija",
-        "synonyms": ["Krkochia", "Krkoshia", "Kyrkochia"],
-        "description": "Minor blending partner for Žilavka in Bosnia and Herzegovina.",
-        "color": "white",
+        "synonyms": [
+            "Krkochia",
+            "Krkoshia",
+            "Kyrkochia"
+        ],
+        "description": {
+            "default": "Minor blending partner for Žilavka in Bosnia and Herzegovina.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Krstač",
         "synonyms": [
             "Bijeli Krstač",
             "Krata Bijela",
             "Krstač Bijela",
             "Loza Bijela",
-            "Vinogradarska Bijela",
+            "Vinogradarska Bijela"
         ],
-        "description": "Old Montenegrin variety producing light, summery whites.",
-        "color": "white",
+        "description": {
+            "default": "Old Montenegrin variety producing light, summery whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kujundžuša",
-        "synonyms": ["Kojundžuša", "Kujundžuša Bijela", "Tvrdac", "Žutac", "Žutka"],
-        "description": "Rare Dalmatian variety.",
-        "color": "white",
+        "synonyms": [
+            "Kojundžuša",
+            "Kujundžuša Bijela",
+            "Tvrdac",
+            "Žutac",
+            "Žutka"
+        ],
+        "description": {
+            "default": "Rare Dalmatian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Kupusar",
-        "synonyms": ["Plavac Kupusar"],
-        "description": "Very rare, tannic variety from coastal Croatia.",
-        "color": "black",
+        "synonyms": [
+            "Plavac Kupusar"
+        ],
+        "description": {
+            "default": "Very rare, tannic variety from coastal Croatia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Kydonitsa",
-        "synonyms": ["Kidonitsa"],
-        "description": "Promising but still very minor variety producing aromatic, finely textured wines near Monemvasia.",
-        "color": "white",
+        "synonyms": [
+            "Kidonitsa"
+        ],
+        "description": {
+            "default": "Promising but still very minor variety producing aromatic, finely textured wines near Monemvasia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "L’Acadie Blanc",
-        "synonyms": ["Acadie", "L’Acadie", "V 53261"],
-        "description": "1950s Canadian very complex hybrid performing well in the chilly climes of Nova Scotia and Québec.",
-        "color": "white",
+        "synonyms": [
+            "Acadie",
+            "L’Acadie",
+            "V 53261"
+        ],
+        "description": {
+            "default": "1950s Canadian very complex hybrid performing well in the chilly climes of Nova Scotia and Québec.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "La Crescent",
-        "synonyms": ["MN 1166"],
-        "description": "Promising and increasingly popular cold-hardy American hybrid.",
-        "color": "white",
+        "synonyms": [
+            "MN 1166"
+        ],
+        "description": {
+            "default": "Promising and increasingly popular cold-hardy American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "La Crosse",
-        "synonyms": ["ES 294", "LaCrosse"],
-        "description": "Complex American hybrid starting to achieve some success in the US Midwest.",
-        "color": "white",
+        "synonyms": [
+            "ES 294",
+            "LaCrosse"
+        ],
+        "description": {
+            "default": "Complex American hybrid starting to achieve some success in the US Midwest.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lacrima Di Morro D’Alba",
-        "synonyms": ["Lacrima"],
-        "description": "Recovered, very local Marche speciality used for both dry and sweet early-maturing reds",
-        "color": "black",
+        "synonyms": [
+            "Lacrima"
+        ],
+        "description": {
+            "default": "Recovered, very local Marche speciality used for both dry and sweet early-maturing reds",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lafnetscha",
-        "synonyms": ["Laffnetscha", "Lafnätscha", "Lavenetsch"],
-        "description": "Old but quantitively unimportant Swiss variety producing well-structured, ageworthy whites.",
-        "color": "white",
+        "synonyms": [
+            "Laffnetscha",
+            "Lafnätscha",
+            "Lavenetsch"
+        ],
+        "description": {
+            "default": "Old but quantitively unimportant Swiss variety producing well-structured, ageworthy whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lagarino Bianco",
-        "synonyms": ["Chegarèl", "Sghittarella"],
-        "description": "Old but only recently registered crisp Trentino white wine grape.",
-        "color": "white",
+        "synonyms": [
+            "Chegarèl",
+            "Sghittarella"
+        ],
+        "description": {
+            "default": "Old but only recently registered crisp Trentino white wine grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lagrein",
-        "synonyms": ["Lagrain"],
-        "description": "Very well-connected, distinctively fruity but sometimes rustic feature of the Alto Adige.",
-        "color": "black",
+        "synonyms": [
+            "Lagrain"
+        ],
+        "description": {
+            "default": "Very well-connected, distinctively fruity but sometimes rustic feature of the Alto Adige.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lairén",
         "synonyms": [
             "Laeren del Rey",
             "Layrenes",
             "Malvar",
             "Mantuo Laéren",
             "Mantuo Layrenes",
-            "Temprana Agosteña",
+            "Temprana Agosteña"
         ],
-        "description": "Very minor Andalusian variety often mistaken for the much more common Airén.",
-        "color": "white",
+        "description": {
+            "default": "Very minor Andalusian variety often mistaken for the much more common Airén.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lalvari",
-        "synonyms": ["Burra", "Dana Bouroun", "Dana Burnu", "Dana Burun", "Glglan"],
-        "description": "Versatile Armenian white wine grape.",
-        "color": "white",
+        "synonyms": [
+            "Burra",
+            "Dana Bouroun",
+            "Dana Burnu",
+            "Dana Burun",
+            "Glglan"
+        ],
+        "description": {
+            "default": "Versatile Armenian white wine grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lambrusca Di Alessandria",
         "synonyms": [
             "Anrè",
             "Caruét",
             "Croetto",
             "Crova",
             "Crovet",
             "Crovìn",
             "Moretto",
             "Lambrusco di Alessandria",
             "Neretto di Alessandria",
-            "Stupèt",
+            "Stupèt"
         ],
-        "description": "Adaptable but minor dark-skinned variety grown in parts of Piemonte, north-west Italy, and generally blended.",
-        "color": "black",
+        "description": {
+            "default": "Adaptable but minor dark-skinned variety grown in parts of Piemonte, north-west Italy, and generally blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusca Vittona",
-        "synonyms": ["Vittona"],
-        "description": "Very minor Piemontese variety.",
-        "color": "black",
+        "synonyms": [
+            "Vittona"
+        ],
+        "description": {
+            "default": "Very minor Piemontese variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambruschetto",
-        "synonyms": ["Crovino", "Lambruschetta", "Malaga"],
-        "description": "Old and very localized variety arousing current interest in Piemonte.",
-        "color": "black",
+        "synonyms": [
+            "Crovino",
+            "Lambruschetta",
+            "Malaga"
+        ],
+        "description": {
+            "default": "Old and very localized variety arousing current interest in Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Barghi",
-        "synonyms": ["Lambrusco Bardi", "Lambrusco Corbelli", "Lambrusco di Rivalta"],
-        "description": "Very minor, recently recognized, dark-skinned blending component in Reggio.",
-        "color": "black",
+        "synonyms": [
+            "Lambrusco Bardi",
+            "Lambrusco Corbelli",
+            "Lambrusco di Rivalta"
+        ],
+        "description": {
+            "default": "Very minor, recently recognized, dark-skinned blending component in Reggio.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Di Fiorano",
-        "synonyms": ["Lambruscone"],
-        "description": "Obscure, highly localized Emilia-Romagna variety unrelated to other Lambruscos.",
-        "color": "black",
+        "synonyms": [
+            "Lambruscone"
+        ],
+        "description": {
+            "default": "Obscure, highly localized Emilia-Romagna variety unrelated to other Lambruscos.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Di Sorbara",
-        "synonyms": ["Lambruschetta di Sorbara", "Lambrusco Sorbarese"],
-        "description": "Perhaps the most respected of the varieties responsible for Lambrusco, Emilia-Romagna’s potentially refreshing, lightly frothy, food-friendly red.",
-        "color": "black",
+        "synonyms": [
+            "Lambruschetta di Sorbara",
+            "Lambrusco Sorbarese"
+        ],
+        "description": {
+            "default": "Perhaps the most respected of the varieties responsible for Lambrusco, Emilia-Romagna’s potentially refreshing, lightly frothy, food-friendly red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Grasparossa",
-        "synonyms": ["Lambrusco di Castelvetro", "Scorzamara"],
-        "description": "Makes fuller, more tannic Lambrusco than most, both dry and medium sweet.",
-        "color": "black",
+        "synonyms": [
+            "Lambrusco di Castelvetro",
+            "Scorzamara"
+        ],
+        "description": {
+            "default": "Makes fuller, more tannic Lambrusco than most, both dry and medium sweet.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Maestri",
-        "synonyms": ["Grappello Maestri", "Lambrusco di Spagna"],
-        "description": "One of the lesser Lambruscos, from Parma, and making rather rustic wines.",
-        "color": "black",
+        "synonyms": [
+            "Grappello Maestri",
+            "Lambrusco di Spagna"
+        ],
+        "description": {
+            "default": "One of the lesser Lambruscos, from Parma, and making rather rustic wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Oliva",
-        "synonyms": ["Lambrusco Mazzone", "Olivone"],
-        "description": "Relatively minor, occasionally bitter Lambrusco variety.",
-        "color": "black",
+        "synonyms": [
+            "Lambrusco Mazzone",
+            "Olivone"
+        ],
+        "description": {
+            "default": "Relatively minor, occasionally bitter Lambrusco variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Salamino",
-        "synonyms": ["Lambrusco Galassi", "Lambrusco di Santa Croce"],
-        "description": "The most widely planted of the Lambrusco varieties, making the most substantial wines.",
-        "color": "black",
+        "synonyms": [
+            "Lambrusco Galassi",
+            "Lambrusco di Santa Croce"
+        ],
+        "description": {
+            "default": "The most widely planted of the Lambrusco varieties, making the most substantial wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lambrusco Viadanese",
-        "synonyms": ["Grappello Ruperti", "Mantovano", "Montecchio", "Viadanese"],
-        "description": "Minor but characterful Lambrusco variety.",
-        "color": "black",
+        "synonyms": [
+            "Grappello Ruperti",
+            "Mantovano",
+            "Montecchio",
+            "Viadanese"
+        ],
+        "description": {
+            "default": "Minor but characterful Lambrusco variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Landal",
-        "synonyms": ["Landot 244"],
-        "description": "Disease-resistant, waning French hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Landot 244"
+        ],
+        "description": {
+            "default": "Disease-resistant, waning French hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Landot Noir",
-        "synonyms": ["Landot 4511"],
-        "description": "Minor French hybrid, son of Landal, also found in a few pockets in the US and Canada.",
-        "color": "black",
+        "synonyms": [
+            "Landot 4511"
+        ],
+        "description": {
+            "default": "Minor French hybrid, son of Landal, also found in a few pockets in the US and Canada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lanzesa",
-        "synonyms": ["Lanzés", "Lanzesca"],
-        "description": "Very rare white wine speciality of Ravenna in northern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Lanzés",
+            "Lanzesca"
+        ],
+        "description": {
+            "default": "Very rare white wine speciality of Ravenna in northern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lasina",
-        "synonyms": ["Krapljenica", "Kutlarica", "Lasin", "Lasina Crna", "Vlasina"],
-        "description": "Very rare vine found only in Dalmacija (Dalmatia) and generally used in blends.",
-        "color": "black",
+        "synonyms": [
+            "Krapljenica",
+            "Kutlarica",
+            "Lasin",
+            "Lasina Crna",
+            "Vlasina"
+        ],
+        "description": {
+            "default": "Very rare vine found only in Dalmacija (Dalmatia) and generally used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Laurot",
-        "synonyms": ["MI 5-106"],
-        "description": "Recently bred and privately owned disease-resistant Czech dark-skinned hybrid.",
-        "color": "black",
+        "synonyms": [
+            "MI 5-106"
+        ],
+        "description": {
+            "default": "Recently bred and privately owned disease-resistant Czech dark-skinned hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Lauzet",
-        "synonyms": ["Laouset", "Lauzet Blanc"],
-        "description": "Almost extinct variety in Jurançon, south-west France.",
-        "color": "white",
+        "synonyms": [
+            "Laouset",
+            "Lauzet Blanc"
+        ],
+        "description": {
+            "default": "Almost extinct variety in Jurançon, south-west France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Len De L’El",
         "synonyms": [
             "Cavaillès",
             "Cavalier",
             "Len-de-Lel",
             "Len de l’Elh",
             "Lenc dé l’El",
-            "Loin de l’Oeil",
+            "Loin de l’Oeil"
         ],
-        "description": "Highly localized and well suited to the production of sweet wines in its native Gaillac.",
-        "color": "black",
+        "description": {
+            "default": "Highly localized and well suited to the production of sweet wines in its native Gaillac.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Léon Millot",
-        "synonyms": ["Frühe Schwarze", "Kuhlmann 194-2", "Millot"],
-        "description": "French hybrid producing deeply coloured reds. Popular in regions with short growing seasons.",
-        "color": "black",
+        "synonyms": [
+            "Frühe Schwarze",
+            "Kuhlmann 194-2",
+            "Millot"
+        ],
+        "description": {
+            "default": "French hybrid producing deeply coloured reds. Popular in regions with short growing seasons.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Liatiko",
-        "synonyms": ["Aleatiko", "Liatico", "Liatis", "Stafili Tu Louliou"],
-        "description": "Idiosyncratic and underrated dark-skinned Cretan variety making aromatic dry and sweet wines.",
-        "color": "black",
+        "synonyms": [
+            "Aleatiko",
+            "Liatico",
+            "Liatis",
+            "Stafili Tu Louliou"
+        ],
+        "description": {
+            "default": "Idiosyncratic and underrated dark-skinned Cretan variety making aromatic dry and sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Limnio",
         "synonyms": [
             "Kalabaki",
             "Kalambaki",
             "Kalampaki",
             "Lembiotiko",
             "Lemnia",
-            "Lemnio",
+            "Lemnio"
         ],
-        "description": "Ancient Greek variety that has successfully travelled from the island of Límnos to the mainland and is often a minor partner to Cabernets Sauvignon and Franc.",
-        "color": "black",
+        "description": {
+            "default": "Ancient Greek variety that has successfully travelled from the island of Límnos to the mainland and is often a minor partner to Cabernets Sauvignon and Franc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Limniona",
-        "synonyms": ["Lemniona"],
-        "description": "Recently resurrected and promising Greek variety from Thessalía.",
-        "color": "black",
+        "synonyms": [
+            "Lemniona"
+        ],
+        "description": {
+            "default": "Recently resurrected and promising Greek variety from Thessalía.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Listán De Huelva",
         "synonyms": [
             "Listán",
             "Listán Blanca",
             "Malvasia Rasteiro",
             "Manteúdo",
             "Manteúdo Branco",
             "Mantheudo",
             "Manteúdo do Algarve",
-            "Vale Grosso",
+            "Vale Grosso"
         ],
-        "description": "Minor variety used mostly for fino-like wines in western Andalucía.",
-        "color": "white",
+        "description": {
+            "default": "Minor variety used mostly for fino-like wines in western Andalucía.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Listán Negro",
-        "synonyms": ["Almuñeco", "Listán Morado", "Negra Commún"],
-        "description": "The red wine grape of Spain’s Islas Canarias. Potentially aromatic wines.",
-        "color": "black",
+        "synonyms": [
+            "Almuñeco",
+            "Listán Morado",
+            "Negra Commún"
+        ],
+        "description": {
+            "default": "The red wine grape of Spain’s Islas Canarias. Potentially aromatic wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Listán Prieto",
         "synonyms": [
             "Criolla Chica",
             "El Paso",
             "Hariri",
@@ -5675,141 +9049,214 @@
             "Palomina Negra",
             "Rosa del Perú",
             "Uva Chica Negra",
             "Uva Negra",
             "Uva Negra Vino",
             "Uva Tinta",
             "Viña Blanca",
-            "Viña Negra",
+            "Viña Negra"
         ],
-        "description": "Historically important, well-travelled, dark-skinned Spanish variety now more common in the Americas but generally in retreat and, with some recent exceptions, producing inferior wines.",
-        "color": "black",
+        "description": {
+            "default": "Historically important, well-travelled, dark-skinned Spanish variety now more common in the Americas but generally in retreat and, with some recent exceptions, producing inferior wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ljutun",
-        "synonyms": ["Ljutac", "Plavac", "Plavac Bedalovac"],
-        "description": "Rare, tart Croatian variety exclusive to the area just north west of Split on the Dalmatian coast.",
-        "color": "black",
+        "synonyms": [
+            "Ljutac",
+            "Plavac",
+            "Plavac Bedalovac"
+        ],
+        "description": {
+            "default": "Rare, tart Croatian variety exclusive to the area just north west of Split on the Dalmatian coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Longyan",
-        "synonyms": ["Czhi-Pu-Tao", "Hun-Juan-Sin", "Long Yan", "Lungyen"],
-        "description": "Old and widely planted red-skinned Chinese variety used for the table and for white wine.",
-        "color": "red",
+        "synonyms": [
+            "Czhi-Pu-Tao",
+            "Hun-Juan-Sin",
+            "Long Yan",
+            "Lungyen"
+        ],
+        "description": {
+            "default": "Old and widely planted red-skinned Chinese variety used for the table and for white wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Louise Swenson",
-        "synonyms": ["ES 4-8-33"],
-        "description": "Complex American hybrid with a significant degree of cold hardiness.",
-        "color": "white",
+        "synonyms": [
+            "ES 4-8-33"
+        ],
+        "description": {
+            "default": "Complex American hybrid with a significant degree of cold hardiness.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Loureiro",
         "synonyms": [
             "Branco Redondos",
             "Loureira",
             "Loureiro Blanco",
             "Marqués",
-            "Marquez",
+            "Marquez"
         ],
-        "description": "High-quality, aromatic Vinho Verde variety.",
-        "color": "white",
+        "description": {
+            "default": "High-quality, aromatic Vinho Verde variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lucie Kuhlmann",
-        "synonyms": ["Kuhlmann 149-3", "Lucy-Kuhlman"],
-        "description": "Minor French hybrid grown mainly in Canada.",
-        "color": "black",
+        "synonyms": [
+            "Kuhlmann 149-3",
+            "Lucy-Kuhlman"
+        ],
+        "description": {
+            "default": "Minor French hybrid grown mainly in Canada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Luglienga",
         "synonyms": [
             "Agostenga",
             "Bona in Ca",
             "Guštana",
             "Jouanenc",
             "Lignan Blanc",
             "Lignenga",
             "Lugliatica",
             "Luglienga Blanca",
             "Luigese",
             "Seidentraube",
-            "Uva di Sant’Anna",
+            "Uva di Sant’Anna"
         ],
-        "description": "Historic, widespread but mainly table grape.",
-        "color": "white",
+        "description": {
+            "default": "Historic, widespread but mainly table grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Lumassina",
         "synonyms": [
             "Acerbina",
             "Buzzetto",
             "Garella",
             "Mataòsso",
             "Mataòssu",
-            "Uga Matta",
+            "Uga Matta"
         ],
-        "description": "Rare, light, crisp white exclusive to Liguria in north-west Italy.",
-        "color": "white",
+        "description": {
+            "default": "Rare, light, crisp white exclusive to Liguria in north-west Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Macabeo",
         "synonyms": [
             "Charas Blanc",
             "Lardot",
             "Macabeu",
             "Maccabéo",
             "Maccabeu",
             "Viura",
-            "Vuera",
+            "Vuera"
         ],
-        "description": "Often underestimated, widely grown variety that can make ageworthy whites as Viura in Rioja and Maccabeu in Roussillon.",
-        "color": "white",
+        "description": {
+            "default": "Often underestimated, widely grown variety that can make ageworthy whites as Viura in Rioja and Maccabeu in Roussillon.",
+            "julie": "Macabeo, also known as Viura, is northern spain most planted white grape variety. It plays a key role in the production of Cava wines in Catalonia where it is generally blended with Parellada and Xarello. Maccabeo wines tends to be delicately aromatic with nuances of white flowers and almonds and low in acidity. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Maceratino",
         "synonyms": [
             "Bianchetta Montecchiese",
             "Greco delle Marche",
             "Greco Maceratino",
             "Maceratese",
             "Matelicano",
             "Montecchiese",
             "Ribona",
             "Uva Stretta",
             "Verdicchio Marino",
-            "Verdicchio Tirolese",
+            "Verdicchio Tirolese"
         ],
-        "description": "Rare white found in the Marche on Italy’s Adriatic coast.",
-        "color": "white",
+        "description": {
+            "default": "Rare white found in the Marche on Italy’s Adriatic coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Madeleine Angevine",
-        "synonyms": ["Äugstler Weiss", "Maddalena Angevina", "Madlen Anževin"],
-        "description": "Minor, fresh, citrusy French variety found mainly in Canada and very cool parts of Europe, sometimes grown for table grapes.",
-        "color": "white",
+        "synonyms": [
+            "Äugstler Weiss",
+            "Maddalena Angevina",
+            "Madlen Anževin"
+        ],
+        "description": {
+            "default": "Minor, fresh, citrusy French variety found mainly in Canada and very cool parts of Europe, sometimes grown for table grapes.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Madrasa",
         "synonyms": [
             "Kara Shirei",
             "Qara Shira",
             "Matrasa",
             "Matrassa",
             "Medrese",
-            "Sevi Shirai",
+            "Sevi Shirai"
         ],
-        "description": "Widely planted Azeri variety producing full-bodied and well-structured wines.",
-        "color": "black",
+        "description": {
+            "default": "Widely planted Azeri variety producing full-bodied and well-structured wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Magliocco Canino",
-        "synonyms": ["Magliocco Ovale", "Maglioccolone"],
-        "description": "Makes tannic wines mainly for blends in Calabria.",
-        "color": "black",
+        "synonyms": [
+            "Magliocco Ovale",
+            "Maglioccolone"
+        ],
+        "description": {
+            "default": "Makes tannic wines mainly for blends in Calabria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Magliocco Dolce",
         "synonyms": [
             "Arvino",
             "Catanzarese",
             "Gaddrica",
@@ -5819,112 +9266,174 @@
             "Magliocco Tondo",
             "Maglioccuni",
             "Mangiaguerra",
             "Marcigliana",
             "Marsigliana Nera",
             "Merigallo",
             "Nera di Scilla",
-            "Petroniere",
+            "Petroniere"
         ],
-        "description": "Widely planted Calabrian and the more common of the two Maglioccos.",
-        "color": "black",
+        "description": {
+            "default": "Widely planted Calabrian and the more common of the two Maglioccos.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Magnolia",
-        "synonyms": ["North Carolina 60-60"],
-        "description": "Minor Muscadine variety that ripens unevenly.",
-        "color": "grey",
+        "synonyms": [
+            "North Carolina 60-60"
+        ],
+        "description": {
+            "default": "Minor Muscadine variety that ripens unevenly.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey"
     },
     {
         "name": "Magyarfrankos",
-        "synonyms": ["Magyar Frankos"],
-        "description": "Dark-skinned escapee from experimental plantings during Hungary’s Communist era.",
-        "color": "black",
+        "synonyms": [
+            "Magyar Frankos"
+        ],
+        "description": {
+            "default": "Dark-skinned escapee from experimental plantings during Hungary’s Communist era.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Maiolica",
-        "synonyms": ["Gaglioppa", "Ortonese"],
-        "description": "Minor dark-skinned Abruzzo variety, usually blended with Montepulciano.",
-        "color": "black",
+        "synonyms": [
+            "Gaglioppa",
+            "Ortonese"
+        ],
+        "description": {
+            "default": "Minor dark-skinned Abruzzo variety, usually blended with Montepulciano.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Maiolina",
-        "synonyms": ["Majolina"],
-        "description": "Rare, productive, northern Italian red rescued from extinction in the 1980s.",
-        "color": "black",
+        "synonyms": [
+            "Majolina"
+        ],
+        "description": {
+            "default": "Rare, productive, northern Italian red rescued from extinction in the 1980s.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Malagousia",
-        "synonyms": ["Malagouzia", "Malagoyzia", "Malaouzia", "Melaouzia"],
-        "description": "Aromatic, high-quality Greek recently rescued from oblivion.",
-        "color": "white",
+        "synonyms": [
+            "Malagouzia",
+            "Malagoyzia",
+            "Malaouzia",
+            "Melaouzia"
+        ],
+        "description": {
+            "default": "Aromatic, high-quality Greek recently rescued from oblivion.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malbo Gentile",
-        "synonyms": ["Amabile di Genova", "Tubino", "Turbino"],
-        "description": "Minor Italian red exclusive to Modena.",
-        "color": "black",
+        "synonyms": [
+            "Amabile di Genova",
+            "Tubino",
+            "Turbino"
+        ],
+        "description": {
+            "default": "Minor Italian red exclusive to Modena.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Maligia",
         "synonyms": [
             "Malese",
             "Malige",
             "Maligia Omalise",
             "Malis",
             "Malisa",
             "Malise",
             "Malisia",
             "Malixa",
             "Malixe",
-            "Malixia",
+            "Malixia"
         ],
-        "description": "Rare vine makes alcoholic white in Emilia-Romagna.",
-        "color": "white",
+        "description": {
+            "default": "Rare vine makes alcoholic white in Emilia-Romagna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia",
         "synonyms": [
             "These are basically translations of Malvasia",
             "rather than synonyms",
             "since the name Malvasia is used for so many different varieties",
             "as explained below: Malmsey",
             "Malvagia",
             "Malvasier",
             "Malvasijie",
             "Malvelzevec",
-            "Malvoisie",
+            "Malvoisie"
         ],
-        "description": "MALVASIA",
-        "color": "",
+        "description": {
+            "default": "MALVASIA",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": ""
     },
     {
         "name": "Malvasia Bianca Di Candia",
         "synonyms": [
             "Malvasia Bianca",
             "Malvasia Candia",
             "Malvasia di Candia",
-            "Malvasia Rossa",
+            "Malvasia Rossa"
         ],
-        "description": "Most planted Malvasia, making neutral white. In decline but still quite widely planted and blended in central Italy.",
-        "color": "white",
+        "description": {
+            "default": "Most planted Malvasia, making neutral white. In decline but still quite widely planted and blended in central Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Bianca Di Piemonte",
         "synonyms": [
             "Caccarella",
             "Greco",
             "Malvasia Bianca",
             "Malvasia Greca",
             "Moscatella",
             "Moscato Greco",
-            "Mosella",
+            "Mosella"
         ],
-        "description": "California’s Malvasia. Aromatic, tough-skinned, originally Italian.",
-        "color": "white",
+        "description": {
+            "default": "California’s Malvasia. Aromatic, tough-skinned, originally Italian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Bianca Lunga",
         "synonyms": [
             "Krizol",
             "Malvasia Bianca",
             "Malvasia Bianca Siciliana",
@@ -5941,44 +9450,66 @@
             "Mareština",
             "Menuetta",
             "Pavlos",
             "Prosecco Nostrano",
             "Racina du Monacu Bianca",
             "Rukatac",
             "Tundulillu Bianco",
-            "Višana",
+            "Višana"
         ],
-        "description": "Widely distributed neutral Tuscan variety used in blends for both dry wines and Vin Santo.",
-        "color": "white",
+        "description": {
+            "default": "Widely distributed neutral Tuscan variety used in blends for both dry wines and Vin Santo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Branca De São Jorge",
-        "synonyms": ["Malvasia Branca de S Jorge"],
-        "description": "Portuguese variety of unknown parentage but high quality used in the production of Madeira.",
-        "color": "white",
+        "synonyms": [
+            "Malvasia Branca de S Jorge"
+        ],
+        "description": {
+            "default": "Portuguese variety of unknown parentage but high quality used in the production of Madeira.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasía De Lanzarote",
         "synonyms": [
             "Málaga",
             "Malvasía",
             "Malvasía Portuguesa",
             "Malvasía Volcánica",
             "Peregil",
             "Perejil",
-            "Sebastián García",
+            "Sebastián García"
         ],
-        "description": "Recently identified variety found on the Islas Canarias, easily confused with other Malvasía Somethings.",
-        "color": "white",
+        "description": {
+            "default": "Recently identified variety found on the Islas Canarias, easily confused with other Malvasía Somethings.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Del Lazio",
-        "synonyms": ["Malvasia col Puntino", "Malvasia Gentile", "Malvasia Puntinata"],
-        "description": "Muscat of Hamburg sibling, grapey wines.",
-        "color": "white",
+        "synonyms": [
+            "Malvasia col Puntino",
+            "Malvasia Gentile",
+            "Malvasia Puntinata"
+        ],
+        "description": {
+            "default": "Muscat of Hamburg sibling, grapey wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Di Lipari",
         "synonyms": [
             "Greco Bianco di Gerace",
             "Greco di Gerace",
             "Malmsey",
@@ -5986,24 +9517,35 @@
             "Malvasia Cândida",
             "Malvasía de la Palma",
             "Malvasía de Sitges",
             "Malvasía de Tenerife",
             "Malvasia delle Lipari",
             "Malvasia di Cagliari",
             "Malvasia di Sardegna",
-            "Malvasija Dubrovačka",
+            "Malvasija Dubrovačka"
         ],
-        "description": "Very widespread variety used for a wide array of generally sweet, often dried-grape, wines.",
-        "color": "white",
+        "description": {
+            "default": "Very widespread variety used for a wide array of generally sweet, often dried-grape, wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Di Schierano",
-        "synonyms": ["Malvasia a Grappolo Corto", "Malvasia di Castelnuovo Don Bosco"],
-        "description": "Minor, dark-skinned Malvasia from Piemonte that produces lightly aromatic sweet reds.",
-        "color": "black",
+        "synonyms": [
+            "Malvasia a Grappolo Corto",
+            "Malvasia di Castelnuovo Don Bosco"
+        ],
+        "description": {
+            "default": "Minor, dark-skinned Malvasia from Piemonte that produces lightly aromatic sweet reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Malvasia Fina",
         "synonyms": [
             "Arinto do Dão",
             "Assario",
             "Assario Branco",
@@ -6012,85 +9554,127 @@
             "Boal Cachudo",
             "Boal da Graciosa",
             "Boal da Madeira",
             "Cachudo",
             "Galego",
             "Gual",
             "Terrantez do Pico",
-            "Torrontés",
+            "Torrontés"
         ],
-        "description": "High-quality Portuguese variety that goes by many names, notably Boal on Madeira, and produces many styles of wine.",
-        "color": "white",
+        "description": {
+            "default": "High-quality Portuguese variety that goes by many names, notably Boal on Madeira, and produces many styles of wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malvasia Nera Di Basilicata",
-        "synonyms": ["Malvasia Nera"],
-        "description": "The less common of the two dark-skinned Malvasias of southern Italy.",
-        "color": "black",
+        "synonyms": [
+            "Malvasia Nera"
+        ],
+        "description": {
+            "default": "The less common of the two dark-skinned Malvasias of southern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Malvasia Nera Di Brindisi",
         "synonyms": [
             "Malvasia Negra",
             "Malvasia Nera",
             "Malvasia Nera di Bari",
             "Malvasia Nera di Bitonto",
             "Malvasia Nera di Lecce",
             "Malvasia Nera di Trani",
-            "Malvasia Niura",
+            "Malvasia Niura"
         ],
-        "description": "The most common of the two dark-skinned Malvasias of southern Italy, commonly blended with Negroamaro, one of its parents.",
-        "color": "black",
+        "description": {
+            "default": "The most common of the two dark-skinned Malvasias of southern Italy, commonly blended with Negroamaro, one of its parents.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Malvasia Nera Lunga",
-        "synonyms": ["Moscatella"],
-        "description": "Rare, dark-skinned Malvasia exclusive to the province of Asti.",
-        "color": "black",
+        "synonyms": [
+            "Moscatella"
+        ],
+        "description": {
+            "default": "Rare, dark-skinned Malvasia exclusive to the province of Asti.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Malvasia Preta",
-        "synonyms": ["Moreto", "Mureto", "Pinheira Roxa"],
-        "description": "Douro variety used for port and table wines.",
-        "color": "black",
+        "synonyms": [
+            "Moreto",
+            "Mureto",
+            "Pinheira Roxa"
+        ],
+        "description": {
+            "default": "Douro variety used for port and table wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Malvazija Istarska",
         "synonyms": [
             "Istrska Malvazija",
             "Malvasia del Carso",
             "Malvasia Friulana",
             "Malvasia Istriana",
             "Malvazija",
             "Malvazija Istarska Bijela",
-            "Polijšakica Drnovk",
+            "Polijšakica Drnovk"
         ],
-        "description": "The emphatic white wine grape of Croatia’s Istra (Istria) peninsula.",
-        "color": "white",
+        "description": {
+            "default": "The emphatic white wine grape of Croatia’s Istra (Istria) peninsula.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Malverina",
-        "synonyms": ["BV-19-143"],
-        "description": "Recent, late-ripening, disease-resistant Czech hybrid producing aromatic whites.",
-        "color": "pink",
+        "synonyms": [
+            "BV-19-143"
+        ],
+        "description": {
+            "default": "Recent, late-ripening, disease-resistant Czech hybrid producing aromatic whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Mammolo",
         "synonyms": [
             "Broumest",
             "Malvasia Montanaccio",
             "Mammolo Toscano",
             "Mammolone di Lucca",
             "Muntanaccia",
             "Schiorello",
             "Sciaccarello",
-            "Sciaccarellu",
+            "Sciaccarellu"
         ],
-        "description": "Minor but historically significant perfumed central Italian Sangiovese blending partner, more important on the French island of Corse, as Sciaccarello.",
-        "color": "black",
+        "description": {
+            "default": "Minor but historically significant perfumed central Italian Sangiovese blending partner, more important on the French island of Corse, as Sciaccarello.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mandilaria",
         "synonyms": [
             "Amorghiano",
             "Amorgiano",
             "Dombrena Mavri",
@@ -6101,82 +9685,145 @@
             "Kountoura",
             "Koundoura",
             "Kountoura Mavri",
             "Mandelaria",
             "Mandilaria",
             "Mantilari",
             "Mantilaria",
-            "Montoyra",
+            "Montoyra"
         ],
-        "description": "Greek island variety producing intensely coloured, tannic wines that tend to lack body.",
-        "color": "black",
+        "description": {
+            "default": "Greek island variety producing intensely coloured, tannic wines that tend to lack body.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mandón",
-        "synonyms": ["Galmeta", "Galmete", "Mandó", "Valenciana Tinta"],
-        "description": "Virtually extinct variety from Bierzo, north-west Spain.",
-        "color": "black",
+        "synonyms": [
+            "Galmeta",
+            "Galmete",
+            "Mandó",
+            "Valenciana Tinta"
+        ],
+        "description": {
+            "default": "Virtually extinct variety from Bierzo, north-west Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mandrègue",
-        "synonyms": ["Manrègue", "Néral"],
-        "description": "Ancient and recently rescued Ariège variety.",
-        "color": "black",
+        "synonyms": [
+            "Manrègue",
+            "Néral"
+        ],
+        "description": {
+            "default": "Ancient and recently rescued Ariège variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Manseng Noir",
         "synonyms": [
             "Caíño do Freixo",
             "Ferrón",
             "Ferrol",
             "Mansenc Noir",
-            "Noir du Pays",
+            "Noir du Pays"
         ],
-        "description": "Rare but characterful red wine grape from south-west France, also found in north-west Spain.",
-        "color": "black",
+        "description": {
+            "default": "Rare but characterful red wine grape from south-west France, also found in north-west Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Manto Negro",
-        "synonyms": ["Cabelis", "Mantonegro", "Mantuo Negro"],
-        "description": "Principal dark-skinned variety on the Spanish island of Mallorca, producing pale, fruity, high-alcohol wines.",
-        "color": "black",
+        "synonyms": [
+            "Cabelis",
+            "Mantonegro",
+            "Mantuo Negro"
+        ],
+        "description": {
+            "default": "Principal dark-skinned variety on the Spanish island of Mallorca, producing pale, fruity, high-alcohol wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mantonico Bianco",
         "synonyms": [
             "Mantonico Pizzutella",
             "Mantonacu Viru della Locride",
-            "Mantonico Vero",
+            "Mantonico Vero"
         ],
-        "description": "Minor light-skinned Calabrian.",
-        "color": "white",
+        "description": {
+            "default": "Minor light-skinned Calabrian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Manzoni Bianco",
-        "synonyms": ["I M 6.0.13", "Incrocio Manzoni 6.0.13", "Manzoni"],
-        "description": "Potentially high-quality northern Italian white cross which has inherited the positive qualities of its parents.",
-        "color": "black",
+        "synonyms": [
+            "I M 6.0.13",
+            "Incrocio Manzoni 6.0.13",
+            "Manzoni"
+        ],
+        "description": {
+            "default": "Potentially high-quality northern Italian white cross which has inherited the positive qualities of its parents.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Manzoni Moscato",
-        "synonyms": ["Incrocio Manzoni 13.0.25"],
-        "description": "One of the least planted of Manzoni’s crosses, this dark-skinned version is used to make sweet, sparkling rosé in Trentino.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Manzoni 13.0.25"
+        ],
+        "description": {
+            "default": "One of the least planted of Manzoni’s crosses, this dark-skinned version is used to make sweet, sparkling rosé in Trentino.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Manzoni Rosa",
-        "synonyms": ["Incrocio Manzoni 1-50"],
-        "description": "Very rare Veneto pink-berried cross.",
-        "color": "pink",
+        "synonyms": [
+            "Incrocio Manzoni 1-50"
+        ],
+        "description": {
+            "default": "Very rare Veneto pink-berried cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Mara",
-        "synonyms": ["C41", "C41"],
-        "description": "Recent, promising, early-ripening Swiss cross.",
-        "color": "black",
+        "synonyms": [
+            "C41",
+            "C41"
+        ],
+        "description": {
+            "default": "Recent, promising, early-ripening Swiss cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Maratheftiko",
         "synonyms": [
             "Aloupostaphylo",
             "Bambakada",
             "Bambakina",
@@ -6185,55 +9832,92 @@
             "Marathophiko",
             "Mavrospourtiko",
             "Pambakada",
             "Pambakina",
             "Pampakia",
             "Vambakadha",
             "Vambakina",
-            "Vamvakada",
+            "Vamvakada"
         ],
-        "description": "Rare, high-quality dark-skinned Cyprus variety that is starting to gain in popularity despite difficulties in the vineyard.",
-        "color": "black",
+        "description": {
+            "default": "Rare, high-quality dark-skinned Cyprus variety that is starting to gain in popularity despite difficulties in the vineyard.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Maréchal Foch",
-        "synonyms": ["Foch", "Kuhlmann 188-2", "Marechal Foch", "Marshal Fosh"],
-        "description": "French hybrid that has been very successful in the colder climes of the US and Canada.",
-        "color": "black",
+        "synonyms": [
+            "Foch",
+            "Kuhlmann 188-2",
+            "Marechal Foch",
+            "Marshal Fosh"
+        ],
+        "description": {
+            "default": "French hybrid that has been very successful in the colder climes of the US and Canada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Marmajuelo",
-        "synonyms": ["Bermejuela", "Marmajuela", "Vermejuelo"],
-        "description": "Rare variety from Spain’s Islas Canarias producing crisp, aromatic and potentially high-quality whites.",
-        "color": "white",
+        "synonyms": [
+            "Bermejuela",
+            "Marmajuela",
+            "Vermejuelo"
+        ],
+        "description": {
+            "default": "Rare variety from Spain’s Islas Canarias producing crisp, aromatic and potentially high-quality whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Marquette",
-        "synonyms": ["MN 1211"],
-        "description": "Promising, increasingly popular, cold-hardy complex American hybrid.",
-        "color": "black",
+        "synonyms": [
+            "MN 1211"
+        ],
+        "description": {
+            "default": "Promising, increasingly popular, cold-hardy complex American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Marsanne",
         "synonyms": [
             "Avilleran",
             "Ermitage",
             "Hermitage",
             "Grosse Roussette",
             "Marsanne Blanche",
-            "Roussette de Saint-Péray",
+            "Roussette de Saint-Péray"
         ],
-        "description": "Flavourful and potentially very high-quality light-skinned Rhône variety with notable outposts in Australia and the US.",
-        "color": "white",
+        "description": {
+            "default": "Flavourful and potentially very high-quality light-skinned Rhône variety with notable outposts in Australia and the US.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Marselan",
-        "synonyms": ["INRA 1810-68"],
-        "description": "One of the most successful relatively recent French crosses.",
-        "color": "black",
+        "synonyms": [
+            "INRA 1810-68"
+        ],
+        "description": {
+            "default": "One of the most successful relatively recent French crosses.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Marufo",
         "synonyms": [
             "Brujidera",
             "Brujidero",
             "Brujigero",
@@ -6243,143 +9927,220 @@
             "Moravia Dulce",
             "Mourisco",
             "Mourisco du Douro",
             "Mourisco Preto",
             "Mourisco Tinto",
             "Rucial",
             "Trujidera",
-            "Vigorosa",
+            "Vigorosa"
         ],
-        "description": "Iberian variety that goes by many names and whose light wine is used mainly in blends.",
-        "color": "black",
+        "description": {
+            "default": "Iberian variety that goes by many names and whose light wine is used mainly in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Marzemina Bianca",
-        "synonyms": ["Berzemina di Breganze", "Sciampagna"],
-        "description": "Rare Veneto variety usually found as an ingredient in sweet blended wines.",
-        "color": "white",
+        "synonyms": [
+            "Berzemina di Breganze",
+            "Sciampagna"
+        ],
+        "description": {
+            "default": "Rare Veneto variety usually found as an ingredient in sweet blended wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Marzemino",
         "synonyms": [
             "Balsamina",
             "Barzemin",
             "Berzamino",
             "Marzemina Cenerenta",
             "Marzemina Nera",
             "Marzemino Comune",
-            "Marzemino Gentile",
+            "Marzemino Gentile"
         ],
-        "description": "Makes fruity, perfumed reds often sweet or sparkling or both.",
-        "color": "black",
+        "description": {
+            "default": "Makes fruity, perfumed reds often sweet or sparkling or both.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mátrai Muskotály",
-        "synonyms": ["Mátrai Muskatály"],
-        "description": "Recently registered, grapey Hungarian cross.",
-        "color": "white",
+        "synonyms": [
+            "Mátrai Muskatály"
+        ],
+        "description": {
+            "default": "Recently registered, grapey Hungarian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Maturana Blanca",
-        "synonyms": ["Maturano", "Ribadavia"],
-        "description": "Rare and recently rescued Rioja variety with real potential.",
-        "color": "white",
+        "synonyms": [
+            "Maturano",
+            "Ribadavia"
+        ],
+        "description": {
+            "default": "Rare and recently rescued Rioja variety with real potential.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mauzac Blanc",
         "synonyms": [
             "Blanc Laffite",
             "Gaillac",
             "Plant de Gaillac",
             "Gamet Blanc",
-            "Mausat",
+            "Mausat"
         ],
-        "description": "Characterful, apple-skin-flavoured Gaillac and Limoux variety used in dry, sweet and sparkling wines.",
-        "color": "white",
+        "description": {
+            "default": "Characterful, apple-skin-flavoured Gaillac and Limoux variety used in dry, sweet and sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mauzac Noir",
-        "synonyms": ["Mauzac Rouge"],
-        "description": "Rare variety from south-west France unrelated to its white-wine namesake.",
-        "color": "black",
+        "synonyms": [
+            "Mauzac Rouge"
+        ],
+        "description": {
+            "default": "Rare variety from south-west France unrelated to its white-wine namesake.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mavro",
         "synonyms": [
             "Cipro Nero",
             "Cyperntraube Blaue",
             "Cypro Nero",
             "Korithi Mavro",
             "Kritiko Mavro",
             "Kypreico Mavro",
             "Kypreiko Mavro",
             "Kypriotiko",
             "Mavro Kyproy",
             "Skuro Mavro",
-            "Staphili-Mavro",
+            "Staphili-Mavro"
         ],
-        "description": "The dominant Cyprus variety, makes undistinguished wine.",
-        "color": "black",
+        "description": {
+            "default": "The dominant Cyprus variety, makes undistinguished wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mavro Kalavritino",
-        "synonyms": ["Kalavritino Mavro", "Mavro Kalavrytiko", "Psilomavro Kalavryton"],
-        "description": "Very minor Greek variety from the northern Pelopónnisos (Peloponnese).",
-        "color": "black",
+        "synonyms": [
+            "Kalavritino Mavro",
+            "Mavro Kalavrytiko",
+            "Psilomavro Kalavryton"
+        ],
+        "description": {
+            "default": "Very minor Greek variety from the northern Pelopónnisos (Peloponnese).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mavro Messenikola",
-        "synonyms": ["Mavro de Messenicolas", "Mavro Mesenikola", "Messenikola Mavro"],
-        "description": "Variety exclusive to the Greek region of Thessalía that benefits greatly from its partnership with Syrah.",
-        "color": "black",
+        "synonyms": [
+            "Mavro de Messenicolas",
+            "Mavro Mesenikola",
+            "Messenikola Mavro"
+        ],
+        "description": {
+            "default": "Variety exclusive to the Greek region of Thessalía that benefits greatly from its partnership with Syrah.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mavrodafni",
         "synonyms": [
             "Ahmar Mechtras",
             "Fraoula Kokkini",
             "Mavrodafnitsa",
             "Mavrodaphne",
             "Mavrodaphni",
             "Mavrodrami",
-            "Thiniatiko",
+            "Thiniatiko"
         ],
-        "description": "Deeply coloured, tannic yet aromatic Greek variety famous for producing ageworthy, sweet, fortified wines.",
-        "color": "black",
+        "description": {
+            "default": "Deeply coloured, tannic yet aromatic Greek variety famous for producing ageworthy, sweet, fortified wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mavroudi Arachovis",
         "synonyms": [
             "Arachovis",
             "Arachovitiko Mavro",
             "Arahovitikos",
             "Mavro Arachovitiko",
-            "Mavroudi of Arachova",
+            "Mavroudi of Arachova"
         ],
-        "description": "Rare variety from central Greece.",
-        "color": "black",
+        "description": {
+            "default": "Rare variety from central Greece.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mavrud",
         "synonyms": [
             "Kachivela",
             "Mavro",
             "Mavroud",
             "Mavroudi",
             "Mavroudi Boulgarias",
-            "Tsiganka",
+            "Tsiganka"
         ],
-        "description": "Indigenous Bulgarian variety producing sturdy reds that can improve with age.",
-        "color": "black",
+        "description": {
+            "default": "Indigenous Bulgarian variety producing sturdy reds that can improve with age.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mayolet",
-        "synonyms": ["Maïolet", "Majolet"],
-        "description": "Extremely rare Aosta variety gradually recovering from near-extinction.",
-        "color": "black",
+        "synonyms": [
+            "Maïolet",
+            "Majolet"
+        ],
+        "description": {
+            "default": "Extremely rare Aosta variety gradually recovering from near-extinction.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mazuelo",
         "synonyms": [
             "Bovale di Spagna",
             "Bovale Grande",
             "Bovale Mannu",
@@ -6387,155 +10148,251 @@
             "Carignane",
             "Carignano",
             "Cariñano",
             "Cariñena",
             "Crujillón",
             "Mazuela",
             "Mollard",
-            "Samsó  and many more",
+            "Samsó  and many more"
         ],
-        "description": "Black variety from north-east Spain high in tannins and acidity that can make fine wine from old vines but has in its time, as Carignan, blighted Languedoc-Roussillon.",
-        "color": "black",
+        "description": {
+            "default": "Black variety from north-east Spain high in tannins and acidity that can make fine wine from old vines but has in its time, as Carignan, blighted Languedoc-Roussillon.",
+            "julie": "Mazuelo, also known as Carignan, has been a controversial grape variety for its ability to give super high yields and many regions, such as Languedoc, have uprooted many of its vineyards. However, the grape has recently been cherised by new producers that have saved old bush vines and a trend of carbonic maceration Carignan is born in the last few years. The best examples are supple and fruit forward with a touch of umami.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mazzese",
         "synonyms": [
             "Massase",
             "Mazzese di Parlascio",
             "Orzese",
             "Rinaldesca",
             "Uva Mazzese",
-            "Vajano",
+            "Vajano"
         ],
-        "description": "Very minor variety used as a minor component in blends.",
-        "color": "black",
+        "description": {
+            "default": "Very minor variety used as a minor component in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mècle De Bourgoin",
-        "synonyms": ["Mescle de Bourgoin"],
-        "description": "Neglected eastern French variety now receiving some attention.",
-        "color": "black",
+        "synonyms": [
+            "Mescle de Bourgoin"
+        ],
+        "description": {
+            "default": "Neglected eastern French variety now receiving some attention.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Medna",
-        "synonyms": ["Buboj", "Bumba", "Medna Bijala", "Medva", "Rizavac", "Zložder"],
-        "description": "Rare Dalmatian variety, often with a honey aroma.",
-        "color": "white",
+        "synonyms": [
+            "Buboj",
+            "Bumba",
+            "Medna Bijala",
+            "Medva",
+            "Rizavac",
+            "Zložder"
+        ],
+        "description": {
+            "default": "Rare Dalmatian variety, often with a honey aroma.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Megrabuir",
-        "synonyms": ["Meghrabuyr", "Megrabouir", "Megrabuyr"],
-        "description": "Productive and cold-hardy Armenian hybrid used mainly to produce pink dessert wines.",
-        "color": "black",
+        "synonyms": [
+            "Meghrabuyr",
+            "Megrabouir",
+            "Megrabuyr"
+        ],
+        "description": {
+            "default": "Productive and cold-hardy Armenian hybrid used mainly to produce pink dessert wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Melara",
-        "synonyms": ["Merlara"],
-        "description": "Rare, used as a component in Vin Santo di Vigoleno.",
-        "color": "white",
+        "synonyms": [
+            "Merlara"
+        ],
+        "description": {
+            "default": "Rare, used as a component in Vin Santo di Vigoleno.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Melnik 82",
-        "synonyms": ["Melnik"],
-        "description": "Result of crossing the variety commonly called Melnik, Shiroka Melnishka, with a variety from south-west France.",
-        "color": "black",
+        "synonyms": [
+            "Melnik"
+        ],
+        "description": {
+            "default": "Result of crossing the variety commonly called Melnik, Shiroka Melnishka, with a variety from south-west France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Melon",
         "synonyms": [
             "Gamay Blanc",
             "Latran",
             "Melon de Bourgogne",
             "Muscadet",
             "Plant de Bourgogne",
-            "Petit Bourgogne",
+            "Petit Bourgogne"
         ],
-        "description": "Old Burgundian variety well suited to the western, Atlantic-dominated mouth of the Loire.",
-        "color": "white",
+        "description": {
+            "default": "Old Burgundian variety well suited to the western, Atlantic-dominated mouth of the Loire.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mencía",
-        "synonyms": ["Jaen", "Jaen du Dão", "Loureiro Tinto", "Mencía Pajaral"],
-        "description": "Increasingly appreciated aromatic variety found in both Spain and Portugal.",
-        "color": "black",
+        "synonyms": [
+            "Jaen",
+            "Jaen du Dão",
+            "Loureiro Tinto",
+            "Mencía Pajaral"
+        ],
+        "description": {
+            "default": "Increasingly appreciated aromatic variety found in both Spain and Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Menoir",
-        "synonyms": ["Kékmedoc", "Medoc Noir", "Menoire"],
-        "description": "Minor, recently renamed Hungarian variety making reds with Muscat aromas.",
-        "color": "black",
+        "synonyms": [
+            "Kékmedoc",
+            "Medoc Noir",
+            "Menoire"
+        ],
+        "description": {
+            "default": "Minor, recently renamed Hungarian variety making reds with Muscat aromas.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Menu Pineau",
         "synonyms": [
             "Arbois Blanc",
             "Herbois",
             "Menu",
             "Menu Pinot",
             "Orbois",
             "Petit Pineau",
-            "Verdet",
+            "Verdet"
         ],
-        "description": "Well-connected and once important Blois speciality with a handful of advocates.",
-        "color": "white",
+        "description": {
+            "default": "Well-connected and once important Blois speciality with a handful of advocates.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mérille",
         "synonyms": [
             "Bordelais",
             "Bordelais Noir",
             "Bourdalès",
             "Bouchalès",
             "Grand Vesparo",
             "Vesparo à Queue Verte",
-            "Périgord",
+            "Périgord"
         ],
-        "description": "Virtually extinct variety found occasionally in Fronton blends in south-west France.",
-        "color": "black",
+        "description": {
+            "default": "Virtually extinct variety found occasionally in Fronton blends in south-west France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Merlot",
         "synonyms": [
             "Bigney",
             "Crabutet",
             "Langon",
             "Médoc Noir",
             "Merlau",
             "Merlot Noir",
             "Picard",
             "Sémillon Rouge",
-            "Vitraille",
+            "Vitraille"
         ],
-        "description": "Fleshy, widely planted, relatively early ripening member of the Bordeaux family.",
-        "color": "black",
+        "description": {
+            "default": "Fleshy, widely planted, relatively early ripening member of the Bordeaux family.",
+            "julie": "",
+            "sommelier": "Merlot can be a bit of a chameleon; ranging from fruity, smooth and easy-going to age-worthy, full-bodied, and sophisticated. Merlot offers wines with notes of roasted coffee, burnt cherry, wild berries and chocolate. It has supple tannins and a dark robe with purplish highlights."
+        },
+        "color": "black"
     },
     {
         "name": "Merseguera",
-        "synonyms": ["Exquitsagos", "Esquitxagos", "Verdosilla"],
-        "description": "Uninspiring variety widely planted in eastern central Spain.",
-        "color": "white",
+        "synonyms": [
+            "Exquitsagos",
+            "Esquitxagos",
+            "Verdosilla"
+        ],
+        "description": {
+            "default": "Uninspiring variety widely planted in eastern central Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Merzling",
-        "synonyms": ["Freiburg 993-60"],
-        "description": "Very minor, disease-resistant German hybrid.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 993-60"
+        ],
+        "description": {
+            "default": "Very minor, disease-resistant German hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Meslier Saint-François",
         "synonyms": [
             "Blanc Ramé",
             "Gaillac",
             "Gros Meslier",
             "Meslier",
             "Purgarie",
-            "Pelegarie",
+            "Pelegarie"
         ],
-        "description": "Almost extinct, historic French variety.",
-        "color": "white",
+        "description": {
+            "default": "Almost extinct, historic French variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mézes Fehér",
         "synonyms": [
             "Alföldi Fehér",
             "Aranyka",
             "Aranyka Sarga",
@@ -6548,121 +10405,209 @@
             "Honigtraube",
             "Margit",
             "Mézédes",
             "Mézes",
             "Sarféjer",
             "Sárga Margit",
             "Sárga Szőlő",
-            "Zsige",
+            "Zsige"
         ],
-        "description": "Ancient but almost extinct Hungarian variety making rich, aromatic whites.",
-        "color": "white",
+        "description": {
+            "default": "Ancient but almost extinct Hungarian variety making rich, aromatic whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mézy",
-        "synonyms": ["Mési", "Meslier Noir", "Petit Mesi"],
-        "description": "Franche-Comté variety known only as a minor ingredient in a blend.",
-        "color": "black",
+        "synonyms": [
+            "Mési",
+            "Meslier Noir",
+            "Petit Mesi"
+        ],
+        "description": {
+            "default": "Franche-Comté variety known only as a minor ingredient in a blend.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Milgranet",
-        "synonyms": ["Périgord Noir", "Petite Mérille"],
-        "description": "Recently snatched from virtual extinction by researchers in southern France.",
-        "color": "black",
+        "synonyms": [
+            "Périgord Noir",
+            "Petite Mérille"
+        ],
+        "description": {
+            "default": "Recently snatched from virtual extinction by researchers in southern France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Millot-Foch",
-        "synonyms": ["VB 85-1"],
-        "description": "Rare, disease-resistant Swiss hybrid producing deeply coloured, fruity wines.",
-        "color": "black",
+        "synonyms": [
+            "VB 85-1"
+        ],
+        "description": {
+            "default": "Rare, disease-resistant Swiss hybrid producing deeply coloured, fruity wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Minella Bianca",
-        "synonyms": ["Eppula", "Minedda Bianca", "Minnella"],
-        "description": "Minor Sicilian white rarely made as a varietal.",
-        "color": "white",
+        "synonyms": [
+            "Eppula",
+            "Minedda Bianca",
+            "Minnella"
+        ],
+        "description": {
+            "default": "Minor Sicilian white rarely made as a varietal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Minutolo",
         "synonyms": [
             "Fiano Aromatico",
             "Fiano della Valle d’Itria",
             "Fiano di Puglia",
             "Fiano di Salento",
             "Fiano Minutolo",
             "Fiore Mendillo",
             "Greco Aromatico",
             "Minutola",
-            "Moscatellina",
+            "Moscatellina"
         ],
-        "description": "Opulently grapey Puglian once known as Fiano Aromatico.",
-        "color": "white",
+        "description": {
+            "default": "Opulently grapey Puglian once known as Fiano Aromatico.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Misket Cherven",
         "synonyms": [
             "Karlovski Misket",
             "Kimionka",
             "Misket Siv",
             "Misket Starozagorski",
             "Misket Sungurlarski",
             "Sinja Temenuga",
             "Songurlarski Misket",
-            "Yuzhnobalgarski Cherven Misket",
+            "Yuzhnobalgarski Cherven Misket"
         ],
-        "description": "Old, pink-skinned Bulgarian variety used to make dry, scented whites.",
-        "color": "pink",
+        "description": {
+            "default": "Old, pink-skinned Bulgarian variety used to make dry, scented whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Misket Varnenski",
-        "synonyms": ["Muscat de Varna", "Muscat Varnenski"],
-        "description": "Minor Bulgarian cross from Varna.",
-        "color": "white",
+        "synonyms": [
+            "Muscat de Varna",
+            "Muscat Varnenski"
+        ],
+        "description": {
+            "default": "Minor Bulgarian cross from Varna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Misket Vrachanski",
         "synonyms": [
             "Mirizlivka",
             "Misket Vratchanski",
             "Tvarda Vrazhda Misket",
             "Wrat Chanskii Musket",
-            "Wratchanski Misket",
+            "Wratchanski Misket"
         ],
-        "description": "Minor Bulgarian cross planted mostly in the far east and west. The most aromatic of the Bulgarian Miskets.",
-        "color": "white",
+        "description": {
+            "default": "Minor Bulgarian cross planted mostly in the far east and west. The most aromatic of the Bulgarian Miskets.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mladinka",
-        "synonyms": ["Mladenka"],
-        "description": "Very rare variety from the Croatian coast generally used in blends.",
-        "color": "white",
+        "synonyms": [
+            "Mladenka"
+        ],
+        "description": {
+            "default": "Very rare variety from the Croatian coast generally used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Molette",
-        "synonyms": ["Molette Blanche", "Molette de Seyssel"],
-        "description": "Minor and rather neutral vine used mainly for sparkling wines in Savoie, eastern France.",
-        "color": "white",
+        "synonyms": [
+            "Molette Blanche",
+            "Molette de Seyssel"
+        ],
+        "description": {
+            "default": "Minor and rather neutral vine used mainly for sparkling wines in Savoie, eastern France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Molinara",
-        "synonyms": ["Brepon", "Mulinara", "Uva del Mulino", "Uva Salà"],
-        "description": "Now plays distinctly third fiddle to Corvina Veronese and Rondinella in wines such as Valpolicella.",
-        "color": "black",
+        "synonyms": [
+            "Brepon",
+            "Mulinara",
+            "Uva del Mulino",
+            "Uva Salà"
+        ],
+        "description": {
+            "default": "Now plays distinctly third fiddle to Corvina Veronese and Rondinella in wines such as Valpolicella.",
+            "julie": "Molinara is planted mainly in the region of Veneto in Italy. The wines are generally pale in colour, high in acidity and prone to oxidation. They play a minor role, blending with Rondinella and Corvina to producer the wines of Valpolicella, Amarone and Bardolino.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mollard",
-        "synonyms": ["Molard", "Petit Mollard", "Tallardier"],
-        "description": "Very minor variety making fresh, light reds in south-east France.",
-        "color": "black",
+        "synonyms": [
+            "Molard",
+            "Petit Mollard",
+            "Tallardier"
+        ],
+        "description": {
+            "default": "Very minor variety making fresh, light reds in south-east France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Monarch",
-        "synonyms": ["Freiburg 487-88"],
-        "description": "Dark, powerful recent German hybrid giving fruity and full-bodied wines.",
-        "color": "black",
+        "synonyms": [
+            "Freiburg 487-88"
+        ],
+        "description": {
+            "default": "Dark, powerful recent German hybrid giving fruity and full-bodied wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Monastrell",
         "synonyms": [
             "Alcayata",
             "Balzac Noir",
             "Catalan",
@@ -6672,309 +10617,520 @@
             "Gayata",
             "Mataro",
             "Mataró",
             "Mourvede",
             "Mourvedon",
             "Mourvèdre",
             "Negria",
-            "Ros",
+            "Ros"
         ],
-        "description": "High-quality, heat-loving dark-skinned variety most valued for its heady, structured contribution to blends.",
-        "color": "black",
+        "description": {
+            "default": "High-quality, heat-loving dark-skinned variety most valued for its heady, structured contribution to blends.",
+            "julie": "The name monastrell derives from the Latin \"mosnateriellu\" meaning \"monastery\" and suggesting that the grape was first cultivated by monks. Kown as Mourvèdre in France and Mataro in Australia and USA, this grape thrives in Mediterrean climate. Spain has a lot of vineyard acreage dedicated to the variety and most of the plantings are located in centre and South East Spain. In France, Bandol is the most famous wine region for the production of Mourvèdre where it produces structures wines that needs time to soften and reveal their full aromatic potential. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Monbadon",
-        "synonyms": ["Burger", "Frontignan des Charentes"],
-        "description": "Productive, dull western French variety that once thrived in California’s Central Valley.",
-        "color": "white",
+        "synonyms": [
+            "Burger",
+            "Frontignan des Charentes"
+        ],
+        "description": {
+            "default": "Productive, dull western French variety that once thrived in California’s Central Valley.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mondeuse Blanche",
-        "synonyms": ["Dongine", "Jongin", "Savouette"],
-        "description": "Savoie variety more famous as Syrah’s parent than for its wines.",
-        "color": "white",
+        "synonyms": [
+            "Dongine",
+            "Jongin",
+            "Savouette"
+        ],
+        "description": {
+            "default": "Savoie variety more famous as Syrah’s parent than for its wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mondeuse Noire",
         "synonyms": [
             "Gros Rouge",
             "Grosse Syrah",
             "Maldoux",
             "Persagne",
             "Petite Persaigne",
             "Plant Maldoux",
-            "Savoyan",
+            "Savoyan"
         ],
-        "description": "Aromatic Savoie variety regaining recognition for its well-structured reds.",
-        "color": "black",
+        "description": {
+            "default": "Aromatic Savoie variety regaining recognition for its well-structured reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Monemvassia",
         "synonyms": [
             "Artemissi",
             "Klossaria",
             "Monemvasia",
             "Monemvassitiko",
-            "Monovassia",
+            "Monovassia"
         ],
-        "description": "Powerful, historic variety widely planted on Páros but receiving renewed attention in the southern Pelopónnisos (Peloponnese).",
-        "color": "white",
+        "description": {
+            "default": "Powerful, historic variety widely planted on Páros but receiving renewed attention in the southern Pelopónnisos (Peloponnese).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Monerac",
-        "synonyms": ["Monérac"],
-        "description": "Fairly recent Montpellier cross yet to win favour.",
-        "color": "black",
+        "synonyms": [
+            "Monérac"
+        ],
+        "description": {
+            "default": "Fairly recent Montpellier cross yet to win favour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Monica Nera",
         "synonyms": [
             "Manzesu",
             "Monaca",
             "Monica di Sardegna",
             "Niedda de Ispagna",
             "Niedda Mora",
             "Nieddera Manna",
-            "Pascale Sardu",
+            "Pascale Sardu"
         ],
-        "description": "Generally undistinguished dark-skinned variety widely planted on the Italian island of Sardegna and made in a variety of styles.",
-        "color": "black",
+        "description": {
+            "default": "Generally undistinguished dark-skinned variety widely planted on the Italian island of Sardegna and made in a variety of styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Montepulciano",
         "synonyms": [
             "Africano",
             "Angolano",
             "Montepulciano Cordisco",
             "Montepulciano Spargolo",
             "Morellone",
             "Sangiovese Cordisco",
-            "Uva Abruzzese",
+            "Uva Abruzzese"
         ],
-        "description": "Productive, deeply coloured, firmly structured and widely planted.",
-        "color": "black",
+        "description": {
+            "default": "Productive, deeply coloured, firmly structured and widely planted.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Montils",
-        "synonyms": ["Chalosse"],
-        "description": "Charentais variety used in the production of cognac.",
-        "color": "white",
+        "synonyms": [
+            "Chalosse"
+        ],
+        "description": {
+            "default": "Charentais variety used in the production of cognac.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Montonico Bianco",
         "synonyms": [
             "Chiapparù",
             "Ciapparone",
             "Greco Bianco del Pollino",
             "Greco del Pollino",
             "Mantonico Bianco Italico",
             "Montonico",
             "Pagadebit",
             "Racciapaluta",
             "Uva della Scala",
-            "Uva Regno",
+            "Uva Regno"
         ],
-        "description": "Minor southern Italian white used mainly in blends.",
-        "color": "white",
+        "description": {
+            "default": "Minor southern Italian white used mainly in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Montù",
-        "synonyms": ["Bianchetto Faentino", "Bianchino", "Montuni", "Montuno"],
-        "description": "Very late ripening Bolognese variety.",
-        "color": "white",
+        "synonyms": [
+            "Bianchetto Faentino",
+            "Bianchino",
+            "Montuni",
+            "Montuno"
+        ],
+        "description": {
+            "default": "Very late ripening Bolognese variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Monvedro",
-        "synonyms": ["Bastardo", "Monvedro Dão"],
-        "description": "Minor, late-budding Portuguese variety causing confusion by its synonyms.",
-        "color": "white",
+        "synonyms": [
+            "Bastardo",
+            "Monvedro Dão"
+        ],
+        "description": {
+            "default": "Minor, late-budding Portuguese variety causing confusion by its synonyms.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Moore’S Diamond",
-        "synonyms": ["Diamond"],
-        "description": "Minor American hybrid similar to, but less successful than, Concord and Niagara.",
-        "color": "white",
+        "synonyms": [
+            "Diamond"
+        ],
+        "description": {
+            "default": "Minor American hybrid similar to, but less successful than, Concord and Niagara.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Moradella",
-        "synonyms": ["Croà", "Moranzana", "Vermiglio"],
-        "description": "Prized by growers but not recognized by officialdom.",
-        "color": "black",
+        "synonyms": [
+            "Croà",
+            "Moranzana",
+            "Vermiglio"
+        ],
+        "description": {
+            "default": "Prized by growers but not recognized by officialdom.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Moravia Agria",
-        "synonyms": ["Maravia Agria", "Moravia", "Moravio"],
-        "description": "Hitherto neglected Spanish variety contributing to at least one distinctively fresh, tannic red in the heat of Manchuela.",
-        "color": "black",
+        "synonyms": [
+            "Maravia Agria",
+            "Moravia",
+            "Moravio"
+        ],
+        "description": {
+            "default": "Hitherto neglected Spanish variety contributing to at least one distinctively fresh, tannic red in the heat of Manchuela.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Moreto Do Alentejo",
-        "synonyms": ["Morito"],
-        "description": "Popular but generally light and lacklustre red in southern Portugal more commonly but ambiguously known as Moreto.",
-        "color": "black",
+        "synonyms": [
+            "Morito"
+        ],
+        "description": {
+            "default": "Popular but generally light and lacklustre red in southern Portugal more commonly but ambiguously known as Moreto.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Morio-Muskat",
-        "synonyms": ["Geilweilerhof I-28-30"],
-        "description": "Intensely grapey but rather flabby German cross that has had its day.",
-        "color": "white",
+        "synonyms": [
+            "Geilweilerhof I-28-30"
+        ],
+        "description": {
+            "default": "Intensely grapey but rather flabby German cross that has had its day.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Moristel",
-        "synonyms": ["Concejón", "Juan Ibáñez", "Moristell"],
-        "description": "Makes light but distinctive reds in Somontano, north-east Spain.",
-        "color": "black",
+        "synonyms": [
+            "Concejón",
+            "Juan Ibáñez",
+            "Moristell"
+        ],
+        "description": {
+            "default": "Makes light but distinctive reds in Somontano, north-east Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mornen Noir",
-        "synonyms": ["Chasselas Noir", "Montruchon", "Mornant", "Mornerain Noir"],
-        "description": "Chasselas relative that might just be rescued from extinction.",
-        "color": "black",
+        "synonyms": [
+            "Chasselas Noir",
+            "Montruchon",
+            "Mornant",
+            "Mornerain Noir"
+        ],
+        "description": {
+            "default": "Chasselas relative that might just be rescued from extinction.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Morone",
         "synonyms": [
             "Morone Farinaccio",
             "Mostaiola del Lapi",
             "Uva Moro",
-            "Uva Morone Nera",
+            "Uva Morone Nera"
         ],
-        "description": "Very minor Tuscan occasionally used to add colour to blends.",
-        "color": "black",
+        "description": {
+            "default": "Very minor Tuscan occasionally used to add colour to blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Morrastel Bouschet",
-        "synonyms": ["Garnacho", "Morrastel Bouschet à Gros Grains"],
-        "description": "Nineteenth-century southern French cross now making tiny amounts of deep red wine.",
-        "color": "black",
+        "synonyms": [
+            "Garnacho",
+            "Morrastel Bouschet à Gros Grains"
+        ],
+        "description": {
+            "default": "Nineteenth-century southern French cross now making tiny amounts of deep red wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Moscatello Selvatico",
-        "synonyms": ["Moscato di Barletta"],
-        "description": "Rare, aromatic white for sweet wines usually from southern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Moscato di Barletta"
+        ],
+        "description": {
+            "default": "Rare, aromatic white for sweet wines usually from southern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Moscato Di Scanzo",
-        "synonyms": ["Moscatino di Scanzo"],
-        "description": "Rare, aromatic red exclusive to Bergamo used to make sweet passito wines and basking in the creation of its new DOCG.",
-        "color": "black",
+        "synonyms": [
+            "Moscatino di Scanzo"
+        ],
+        "description": {
+            "default": "Rare, aromatic red exclusive to Bergamo used to make sweet passito wines and basking in the creation of its new DOCG.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Moscato Di Terracina",
-        "synonyms": ["Moscato di Maccarese"],
-        "description": "Recently rescued aromatic white from central Italy making a wide range of styles.",
-        "color": "white",
+        "synonyms": [
+            "Moscato di Maccarese"
+        ],
+        "description": {
+            "default": "Recently rescued aromatic white from central Italy making a wide range of styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Moscato Giallo",
         "synonyms": [
             "Fior d’Arancio",
             "Goldenmuskateller",
             "Goldmuskateller",
             "Moscatel",
             "Moscato dalla Siria",
             "Moscato Sirio",
             "Muscat du Pays",
             "Muscat Vert",
-            "Muscatedda",
+            "Muscatedda"
         ],
-        "description": "Golden-berried Muscat variety of northern Italy making mainly passito-style wines.",
-        "color": "white",
+        "description": {
+            "default": "Golden-berried Muscat variety of northern Italy making mainly passito-style wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Moscato Rosa Del Trentino",
-        "synonyms": ["Muškat Ruža Porečki", "Rosenmuskateller"],
-        "description": "A minor, red-skinned northern Italian that produces rose-scented sweet wines.",
-        "color": "red",
+        "synonyms": [
+            "Muškat Ruža Porečki",
+            "Rosenmuskateller"
+        ],
+        "description": {
+            "default": "A minor, red-skinned northern Italian that produces rose-scented sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Moschofilero",
-        "synonyms": ["Fileri", "Fileri Mantineias", "Moschophilero"],
-        "description": "Aromatic, high-acid Greek variety that has seen a surge in popularity and plantings in the last twenty years.",
-        "color": "pink",
+        "synonyms": [
+            "Fileri",
+            "Fileri Mantineias",
+            "Moschophilero"
+        ],
+        "description": {
+            "default": "Aromatic, high-acid Greek variety that has seen a surge in popularity and plantings in the last twenty years.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Moschomavro",
-        "synonyms": ["Moschato Mavro", "Moschogaltso", "Xinogaltso"],
-        "description": "Minor Greek variety with good potential for rosés.",
-        "color": "black",
+        "synonyms": [
+            "Moschato Mavro",
+            "Moschogaltso",
+            "Xinogaltso"
+        ],
+        "description": {
+            "default": "Minor Greek variety with good potential for rosés.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mostosa",
-        "synonyms": ["Empibotte Bianco", "Pagadebit", "Pagadebito"],
-        "description": "Minor white variety found on the Adriatic coast, occasionally made as a varietal wine under its synonym Pagadebit.",
-        "color": "white",
+        "synonyms": [
+            "Empibotte Bianco",
+            "Pagadebit",
+            "Pagadebito"
+        ],
+        "description": {
+            "default": "Minor white variety found on the Adriatic coast, occasionally made as a varietal wine under its synonym Pagadebit.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mouyssaguès",
-        "synonyms": ["Négret", "Plant du Pauvre"],
-        "description": "Virtually extinct variety once producing astringent reds in southern central France.",
-        "color": "black",
+        "synonyms": [
+            "Négret",
+            "Plant du Pauvre"
+        ],
+        "description": {
+            "default": "Virtually extinct variety once producing astringent reds in southern central France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Mskhali",
         "synonyms": [
             "Ararati",
             "At Uzyum",
             "Mashali",
             "Messchaly",
             "Mishali",
             "Msali",
             "Mschali",
             "Musrali",
-            "Spitak Khagog",
+            "Spitak Khagog"
         ],
-        "description": "Armenia’s most planted variety, used mainly for brandy.",
-        "color": "white",
+        "description": {
+            "default": "Armenia’s most planted variety, used mainly for brandy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mtsvane Kakhuri",
         "synonyms": [
             "Dedali Mtsvane",
             "Mamali Mtsvane",
             "Mcknara",
             "Mtsvane",
             "Mtsvane Kachuri",
             "Mtsvani",
-            "Mtzvané",
+            "Mtzvané"
         ],
-        "description": "The more widespread of the Mtsvanes makes high-quality Georgian whites in both traditional and European styles.",
-        "color": "white",
+        "description": {
+            "default": "The more widespread of the Mtsvanes makes high-quality Georgian whites in both traditional and European styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mujuretuli",
-        "synonyms": ["Keduretuli"],
-        "description": "Georgian variety used to produce dry and semi-sweet wines.",
-        "color": "black",
+        "synonyms": [
+            "Keduretuli"
+        ],
+        "description": {
+            "default": "Georgian variety used to produce dry and semi-sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Müller-Thurgau",
         "synonyms": [
             "Findling",
             "Riesling-Silvaner",
             "Riesling × Silvaner",
             "Rivaner",
             "Rizlingszilváni",
-            "Rizvanec",
+            "Rizvanec"
         ],
-        "description": "Prolific German invader of the world’s vineyards producing soft, semi-aromatic whites in over-abundance.",
-        "color": "white",
+        "description": {
+            "default": "Prolific German invader of the world’s vineyards producing soft, semi-aromatic whites in over-abundance.",
+            "julie": "",
+            "sommelier": "Created in 1882 in Geisenheim from a cross of Riesling x Madeleine royale, Müller-Thurgau is now the second most important white grape variety in German viticulture after Riesling. Aroma: delicately fruity-floral, delicate herbs, apples or pears. The grape variety ripens early and produces drinkable, sometimes flowery wines with a delicately fruity muscat aroma. The acidity tends to be mild. The wine is usually matured in stainless steel tanks, which are good for preserving the freshness and varietal aroma. Most of the wines are dry or residually sweet quality wines. With some exceptions, Müller-Thurgau is not a storable wine and tastes best in the first few years after harvesting. The wines are easily accessible in taste and are popular because of their harmonious character. They are pale yellow to light yellow in colour and have a medium body. If they bear the designation Rivaner on the label, one can assume that it is a dry, rather youthful, light and fresh wine. Müller-Thurgau wines are usually uncomplicated everyday wines that harmonise well with delicately aromatic dishes."
+        },
+        "color": "white"
     },
     {
         "name": "Muscadelle",
         "synonyms": [
             "Bouillenc",
             "Guinlhan Musqué",
             "Muscat Fou",
             "Sauvignon Vert",
-            "Tokay",
+            "Tokay"
         ],
-        "description": "Significant in Monbazillac, less so in sweet white bordeaux and very important in north-east Victoria.",
-        "color": "white",
+        "description": {
+            "default": "Significant in Monbazillac, less so in sweet white bordeaux and very important in north-east Victoria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Muscat",
         "synonyms": [
             "These are basically translations of Muscat",
             "rather than synonyms",
             "since the name Muscat is used for so many different varieties",
@@ -6984,36 +11140,59 @@
             "Moscato",
             "Moscatello",
             "Moschato",
             "Moschoudia",
             "Muskat",
             "Muskateller",
             "Muskatoly",
-            "Muskotály",
+            "Muskotály"
         ],
-        "description": "MUSCAT",
-        "color": "",
+        "description": {
+            "default": "MUSCAT",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": ""
     },
     {
         "name": "Muscat Bailey A",
-        "synonyms": ["Muscat Bailey"],
-        "description": "Japanese hybrid with many an American gene, good disease resistance but producing candy-flavoured wines.",
-        "color": "black",
+        "synonyms": [
+            "Muscat Bailey"
+        ],
+        "description": {
+            "default": "Japanese hybrid with many an American gene, good disease resistance but producing candy-flavoured wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Muscat Blanc À Petits Grains",
-        "synonyms": [""],
-        "description": "The classic Muscat, the small-berried one that is widely dispersed around the world.",
-        "color": "white",
+        "synonyms": [
+            "Muscat Blanc a Petits Grains"
+        ],
+        "description": {
+            "default": "The classic Muscat, the small-berried one that is widely dispersed around the world.",
+            "julie": "Muscat Blanc à Petits Grains is a very old white grape variety from the Mediterranéen area. The grape is used to produce dry, sweet and fortified wines. It is characterised by its perfumed aromatic reminescent or rose petals, orange blossom and spices. Its main areas of cultivation are the Roussillon and the island of Corsica in France,  the Piemonte region of Italy, the Douro Valley in Portugal, some parts of Spain, Greece and South Africa. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Muscat Bleu",
-        "synonyms": ["Garnier 83/2", "Muscat Bleu Garnier"],
-        "description": "Minor Swiss hybrid valued particularly by organic growers for its Muscat-like aroma and disease resistance but more commonly grown for the table.",
-        "color": "black",
+        "synonyms": [
+            "Garnier 83/2",
+            "Muscat Bleu Garnier"
+        ],
+        "description": {
+            "default": "Minor Swiss hybrid valued particularly by organic growers for its Muscat-like aroma and disease resistance but more commonly grown for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Muscat Fleur D’Oranger",
         "synonyms": [
             "Chasselas Fleur d’Orange",
             "Cranford Muscat",
             "Madarski Muskat",
@@ -7028,18 +11207,22 @@
             "Muscat Regnier",
             "Muscat Vengerskii",
             "Orange Muscat",
             "Orange Muskat",
             "Primavis Muscat",
             "Raisin Vanille",
             "Vanilia Muskotaly",
-            "Weisse Vanillentraube",
+            "Weisse Vanillentraube"
         ],
-        "description": "Highly aromatic, orange-flavoured variety of unknown geographical origin but definitely related to Muscat Blanc à Petits Grains.",
-        "color": "white",
+        "description": {
+            "default": "Highly aromatic, orange-flavoured variety of unknown geographical origin but definitely related to Muscat Blanc à Petits Grains.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Muscat Of Alexandria",
         "synonyms": [
             "Acherfields Early Muscat",
             "Albillo di Toro",
             "Aleksandrijski Muskat",
@@ -7084,18 +11267,22 @@
             "Muscat Romain",
             "Salamanca",
             "Seralamanna",
             "Tămaîioasă de Alexandria",
             "White Hanepoot",
             "Zibbibo",
             "Zibibo",
-            "Zibibbo",
+            "Zibibbo"
         ],
-        "description": "Light-skinned Mediterranean variety generally considered inferior to Muscat Blanc à Petits Grains, used mostly to produce very sweet wines.",
-        "color": "white",
+        "description": {
+            "default": "Light-skinned Mediterranean variety generally considered inferior to Muscat Blanc à Petits Grains, used mostly to produce very sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Muscat Of Hamburg",
         "synonyms": [
             "Black Muscat",
             "Black Muscat of Alexandria",
             "Hamburg Musqué",
@@ -7115,107 +11302,183 @@
             "Muscat Hamburg Crni",
             "Oeillade Musquée",
             "Snow’s Muscat Hamburgh",
             "Tămîioasă Hamburg",
             "Tămîioasă Neagra",
             "Venn’s Seedling",
             "Venn’s Seedling Black Muscat",
-            "Zibibbo Nero",
+            "Zibibbo Nero"
         ],
-        "description": "Genetic conundrum associated most readily with table grapes grown intermittently in England and widely elsewhere.",
-        "color": "black",
+        "description": {
+            "default": "Genetic conundrum associated most readily with table grapes grown intermittently in England and widely elsewhere.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Muscat Ottonel",
         "synonyms": [
             "Muscadel Ottonel",
             "Muskat Otonel",
             "Muskat Ottonel",
             "Muskotály",
             "Ottonel Muskotály",
-            "Tămîioasă Ottonel",
+            "Tămîioasă Ottonel"
         ],
-        "description": "Soft, grapey French variety used for both dry and sweet wines, particularly in Alsace and Eastern Europe.",
-        "color": "white",
+        "description": {
+            "default": "Soft, grapey French variety used for both dry and sweet wines, particularly in Alsace and Eastern Europe.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Muscat Swenson",
-        "synonyms": ["ES 8-2-43", "Muscat de Swenson"],
-        "description": "Muscat-like hardy American hybrid.",
-        "color": "white",
+        "synonyms": [
+            "ES 8-2-43",
+            "Muscat de Swenson"
+        ],
+        "description": {
+            "default": "Muscat-like hardy American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Muškát Moravský",
-        "synonyms": ["Mopr", "Moravian Muscat", "Moravsky Muskat"],
-        "description": "The Czech Republic’s very own Muscat. Widely planted.",
-        "color": "white",
+        "synonyms": [
+            "Mopr",
+            "Moravian Muscat",
+            "Moravsky Muskat"
+        ],
+        "description": {
+            "default": "The Czech Republic’s very own Muscat. Widely planted.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Mustoasă De Măderat",
-        "synonyms": ["Lampor", "Mustafer", "Mustosfehér"],
-        "description": "Productive, high-acid variety from western Romania making light, fresh, locally popular whites.",
-        "color": "white",
+        "synonyms": [
+            "Lampor",
+            "Mustafer",
+            "Mustosfehér"
+        ],
+        "description": {
+            "default": "Productive, high-acid variety from western Romania making light, fresh, locally popular whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Narince",
-        "synonyms": ["Güzül Üzüm", "Kazova", "Narance", "Nerince"],
-        "description": "Turkey’s best-known white wine variety, also grown for the table.",
-        "color": "white",
+        "synonyms": [
+            "Güzül Üzüm",
+            "Kazova",
+            "Narance",
+            "Nerince"
+        ],
+        "description": {
+            "default": "Turkey’s best-known white wine variety, also grown for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Nascetta",
-        "synonyms": ["Anascetta", "Nas-cëtta"],
-        "description": "Renascent semi-aromatic Piemontese made increasingly as a varietal wine.",
-        "color": "white",
+        "synonyms": [
+            "Anascetta",
+            "Nas-cëtta"
+        ],
+        "description": {
+            "default": "Renascent semi-aromatic Piemontese made increasingly as a varietal wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Nasco",
-        "synonyms": ["Nascu", "Nusco"],
-        "description": "Possibly ancient light-berried variety making soft white, mostly dessert, wines on Sardegna.",
-        "color": "white",
+        "synonyms": [
+            "Nascu",
+            "Nusco"
+        ],
+        "description": {
+            "default": "Possibly ancient light-berried variety making soft white, mostly dessert, wines on Sardegna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Nebbiera",
-        "synonyms": ["Incrocio Dalmasso XV/29"],
-        "description": "Very minor northern Italian dark-skinned cross whose true parentage has only recently been revealed.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso XV/29"
+        ],
+        "description": {
+            "default": "Very minor northern Italian dark-skinned cross whose true parentage has only recently been revealed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nebbiolo",
         "synonyms": [
             "Chiavennasca",
             "Picotendro",
             "Picoutener",
             "Picotèner",
             "Prunent",
             "Prünent",
-            "Spanna",
+            "Spanna"
         ],
-        "description": "Piemonte’s, arguably Italy’s, most revered wine grape; very old variety capable of producing perfumed, expressive, ageworthy wines of great beauty.",
-        "color": "black",
+        "description": {
+            "default": "Piemonte’s, arguably Italy’s, most revered wine grape; very old variety capable of producing perfumed, expressive, ageworthy wines of great beauty.",
+            "julie": "Iconic red grape of the Piemonte region of Italy where it produces world class wines in regions such as Barolo DOCG and Barbaresco DOCG. Fragrant, offering a perfect balance between elegance and structure, Barolo wines are high in acidity and tannins and the best of them need a lot of time to fully develop and reveal themselves. There are the true definition of an iron fist in a velvelt glove.",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nebbiolo Rosé",
-        "synonyms": ["Chiavennasca Piccola", "Chiavennaschino", "Nebiol Matiné"],
-        "description": "Piemontese similar to but genetically distinct from Nebbiolo.",
-        "color": "black",
+        "synonyms": [
+            "Chiavennasca Piccola",
+            "Chiavennaschino",
+            "Nebiol Matiné"
+        ],
+        "description": {
+            "default": "Piemontese similar to but genetically distinct from Nebbiolo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Negoska",
         "synonyms": [
             "Goumenissas Mavro",
             "Mavro Goumenissas",
             "Neghotska",
             "Negkoska",
             "Negoska Popolka",
             "Negotska",
-            "Popolka Naoussis",
+            "Popolka Naoussis"
         ],
-        "description": "Northern Greek variety making soft, full-bodied wines that are often blended with Xinomavro.",
-        "color": "black",
+        "description": {
+            "default": "Northern Greek variety making soft, full-bodied wines that are often blended with Xinomavro.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Negramoll",
         "synonyms": [
             "Molar",
             "Mollar",
             "Mollar Cano",
@@ -7228,37 +11491,51 @@
             "Negra Criolla",
             "Negra Mole",
             "Negramolle",
             "Rabo de Ovelha Tinto",
             "Saborinho",
             "Tinta de Madeira",
             "Tinta Negra",
-            "Tinta Negra Mole",
+            "Tinta Negra Mole"
         ],
-        "description": "The dark-skinned grape of Iberia’s Atlantic islands.",
-        "color": "black",
+        "description": {
+            "default": "The dark-skinned grape of Iberia’s Atlantic islands.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Negrara Trentina",
         "synonyms": [
             "Doleara",
             "Doveana",
             "Dovenzana",
             "Edeleschwarze",
             "Keltertraube",
-            "Zoveana",
+            "Zoveana"
         ],
-        "description": "Trentino variety that lost significant ground post-phylloxera in the early twentieth century.",
-        "color": "black",
+        "description": {
+            "default": "Trentino variety that lost significant ground post-phylloxera in the early twentieth century.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Negrara Veronese",
-        "synonyms": ["Terodola"],
-        "description": "Minor Veneto blending component, useful for colour.",
-        "color": "black",
+        "synonyms": [
+            "Terodola"
+        ],
+        "description": {
+            "default": "Minor Veneto blending component, useful for colour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Négrette",
         "synonyms": [
             "Cap de More",
             "Dégoûtant",
             "Morelet",
@@ -7267,416 +11544,636 @@
             "Négralet",
             "Négret",
             "Négret de Gaillac",
             "Négret du Tarn",
             "Négrette de Fronton",
             "Noirien",
             "Pinot St George",
-            "Vesparo Noir",
+            "Vesparo Noir"
         ],
-        "description": "Supple, fruity and distinctive variety that has thrived for centuries just north of Toulouse.",
-        "color": "black",
+        "description": {
+            "default": "Supple, fruity and distinctive variety that has thrived for centuries just north of Toulouse.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Negretto",
         "synonyms": [
             "Negretta",
             "Negrettino",
             "Negrettino Bolognese",
-            "Negrettino Erioli",
+            "Negrettino Erioli"
         ],
-        "description": "Ancient but now minor Emilia-Romagna variety for the table or early-drinking wines.",
-        "color": "black",
+        "description": {
+            "default": "Ancient but now minor Emilia-Romagna variety for the table or early-drinking wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Negroamaro",
         "synonyms": [
             "Abruzzese",
             "Albese",
             "Jonico",
             "Lacrima",
             "Negro Amaro",
             "Nigroamaro",
             "Purcinara",
-            "Uva Olivella",
+            "Uva Olivella"
         ],
-        "description": "Makes sweet-tasting, early-drinking reds and some good rosés on the heel of Italy.",
-        "color": "black",
+        "description": {
+            "default": "Makes sweet-tasting, early-drinking reds and some good rosés on the heel of Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ner D’Ala",
         "synonyms": [
             "Barau",
             "Durás",
             "Fiori",
             "Gros Vien",
             "Neirét dal Picul Rus",
             "Provinè",
             "Pruinè",
             "Uva di Biella",
             "Verdés",
-            "Vernassa",
+            "Vernassa"
         ],
-        "description": "Virtually extinct vine now known to come from Piemonte.",
-        "color": "black",
+        "description": {
+            "default": "Virtually extinct vine now known to come from Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nerello Cappuccio",
         "synonyms": [
             "Mantiddatu Niuru",
             "Nerello Mantellato",
             "Nirello Cappucio",
             "Niureddu",
             "Niureddu Ammatiddatu",
-            "Niureddu Capucciu",
+            "Niureddu Capucciu"
         ],
-        "description": "The lesser, softer of Sicily’s Nerellos, frequently planted with other, as yet unknown, varieties.",
-        "color": "black",
+        "description": {
+            "default": "The lesser, softer of Sicily’s Nerellos, frequently planted with other, as yet unknown, varieties.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nerello Mascalese",
         "synonyms": [
             "Mascalese Nera",
             "Mascalisi",
             "Nerello Calabrese",
             "Nerello Carbunaru",
             "Nerello di Mascali",
             "Nerello Nostrale",
             "Nerello Paesano",
             "Niureddu",
-            "Niureddu Mascalese",
+            "Niureddu Mascalese"
         ],
-        "description": "Important, noble Sicilian of particular significance around Etna. The firmer, longer-lived Nerello.",
-        "color": "black",
+        "description": {
+            "default": "Important, noble Sicilian of particular significance around Etna. The firmer, longer-lived Nerello.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neret Di Saint-Vincent",
-        "synonyms": ["Neiret", "Neret", "Neretto", "Neyret"],
-        "description": "Obscure, recently identified, burly Aostan.",
-        "color": "black",
+        "synonyms": [
+            "Neiret",
+            "Neret",
+            "Neretto",
+            "Neyret"
+        ],
+        "description": {
+            "default": "Obscure, recently identified, burly Aostan.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neretta Cuneese",
         "synonyms": [
             "Freisa di Nizza",
             "Freisa Grossa",
             "Freisa Mora",
             "Neretta",
             "Neretto",
-            "Neretto di Cavaglià",
+            "Neretto di Cavaglià"
         ],
-        "description": "Minor Piemontese that disappears into blends.",
-        "color": "black",
+        "description": {
+            "default": "Minor Piemontese that disappears into blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neretto Di Bairo",
-        "synonyms": ["Nerét", "Nerét Gros", "Neretto", "Neretto di San Giorgio"],
-        "description": "Minor Piemontese used in blends.",
-        "color": "black",
+        "synonyms": [
+            "Nerét",
+            "Nerét Gros",
+            "Neretto",
+            "Neretto di San Giorgio"
+        ],
+        "description": {
+            "default": "Minor Piemontese used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neretto Duro",
         "synonyms": [
             "Balò",
             "Balau",
             "Barbera Rotonda",
             "Bonarda",
             "Bonarda ‘d Macoun",
             "Dolcetto di Boca",
             "Durasa",
             "Freisone",
             "Peilavert",
-            "Uva ′d Galvan",
+            "Uva ′d Galvan"
         ],
-        "description": "Rare Piemontese with a disproportionate number of synonyms.",
-        "color": "black",
+        "description": {
+            "default": "Rare Piemontese with a disproportionate number of synonyms.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neretto Gentile",
         "synonyms": [
             "Nerét Cit",
             "Neretìn",
             "Neretto",
             "Neretto di Cavaglià",
-            "Vermiglia",
+            "Vermiglia"
         ],
-        "description": "Fragile, minor Piemontese.",
-        "color": "black",
+        "description": {
+            "default": "Fragile, minor Piemontese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neretto Nostrano",
         "synonyms": [
             "Freisa Blu",
             "Nebbiulìn",
             "Nerét ‘d Rean",
             "Nerét dal Busc Bianc",
             "Nerét di Romano",
             "Nerét Gentil",
-            "Neretto della Valchiusella",
+            "Neretto della Valchiusella"
         ],
-        "description": "Minor Piemontese also known in the south of the Valle d’Aosta.",
-        "color": "black",
+        "description": {
+            "default": "Minor Piemontese also known in the south of the Valle d’Aosta.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nerkarat",
-        "synonyms": ["Nerkarata"],
-        "description": "Cold-hardy Armenian hybrid used mainly for sweet reds.",
-        "color": "black",
+        "synonyms": [
+            "Nerkarata"
+        ],
+        "description": {
+            "default": "Cold-hardy Armenian hybrid used mainly for sweet reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nero Buono Di Cori",
-        "synonyms": ["Nero Buono", "Nero di Cori"],
-        "description": "Minor central Italian generally blended with Montepulciano or Cesanese.",
-        "color": "black",
+        "synonyms": [
+            "Nero Buono",
+            "Nero di Cori"
+        ],
+        "description": {
+            "default": "Minor central Italian generally blended with Montepulciano or Cesanese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nero D’Avola",
         "synonyms": [
             "Calabrese",
             "Calabrese d’Avola",
             "Calabrese di Vittoria",
             "Calabrese Dolce",
-            "Niureddu Calavrisi",
+            "Niureddu Calavrisi"
         ],
-        "description": "Sicilia’s most widely planted red wine variety valued for its colour, full body and ageing potential.",
-        "color": "black",
+        "description": {
+            "default": "Sicilia’s most widely planted red wine variety valued for its colour, full body and ageing potential.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nero Di Troia",
         "synonyms": [
             "Sommarrello",
             "Sumarello",
             "Summariello",
             "Tranese",
             "Troiano",
             "Uva della Marina",
             "Uva di Barletta",
             "Uva di Canosa",
-            "Uva di Troia",
+            "Uva di Troia"
         ],
-        "description": "High-quality, flavourful, firm northern Puglian that has declined considerably in the last 40 years.",
-        "color": "black",
+        "description": {
+            "default": "High-quality, flavourful, firm northern Puglian that has declined considerably in the last 40 years.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Neuburger",
-        "synonyms": ["Brubler", "Neuburské"],
-        "description": "Nutty, full-bodied but soft Austrian white.",
-        "color": "white",
+        "synonyms": [
+            "Brubler",
+            "Neuburské"
+        ],
+        "description": {
+            "default": "Nutty, full-bodied but soft Austrian white.",
+            "julie": "",
+            "sommelier": "Neuburger is particularly found in drier areas such as the Thermenregion (Lower Austria). In Burgenland it may be used alongside Pinot Blanc, Chardonnay and Grüner Veltliner for white Leithaberg DAC (Burgenland). It's a natural crossing of Roter Veltliner and Sylvaner. Neuburger delivers mostly dense, full-bodied yet mild wines with a subtle flavour. Young wines are spicy and flowery, with a nutty flavour developing with age. This variety is very well suited for Qualitätswein and Prädikatswein."
+        },
+        "color": "white"
     },
     {
         "name": "New York Muscat",
-        "synonyms": ["New York 12997", "NY 12997", "NY Muscat"],
-        "description": "American hybrid with pronounced Muscat flavours grown mainly in Canada.",
-        "color": "black",
+        "synonyms": [
+            "New York 12997",
+            "NY 12997",
+            "NY Muscat"
+        ],
+        "description": {
+            "default": "American hybrid with pronounced Muscat flavours grown mainly in Canada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Niagara",
-        "synonyms": ["Niagara White", "White Concord"],
-        "description": "The foxiest American hybrid of them all.",
-        "color": "white",
+        "synonyms": [
+            "Niagara White",
+            "White Concord"
+        ],
+        "description": {
+            "default": "The foxiest American hybrid of them all.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Nieddera",
-        "synonyms": ["Nieddaera", "Nireddie"],
-        "description": "Recently revived and promising Sardinian.",
-        "color": "black",
+        "synonyms": [
+            "Nieddaera",
+            "Nireddie"
+        ],
+        "description": {
+            "default": "Recently revived and promising Sardinian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nigra",
-        "synonyms": ["Incrocio Cosmo 96"],
-        "description": "Very minor, little-planted, dark-skinned Veneto cross.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Cosmo 96"
+        ],
+        "description": {
+            "default": "Very minor, little-planted, dark-skinned Veneto cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ninčuša",
-        "synonyms": ["Lincuša", "Mlinčevac", "Vincuša"],
-        "description": "Now virtually extinct, rather ordinary variety from the region of Split, on Croatia’s Adriatic coast.",
-        "color": "black",
+        "synonyms": [
+            "Lincuša",
+            "Mlinčevac",
+            "Vincuša"
+        ],
+        "description": {
+            "default": "Now virtually extinct, rather ordinary variety from the region of Split, on Croatia’s Adriatic coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nitranka",
-        "synonyms": ["CAAB 3/22"],
-        "description": "Recently authorized and increasingly popular Slovakian cross.",
-        "color": "black",
+        "synonyms": [
+            "CAAB 3/22"
+        ],
+        "description": {
+            "default": "Recently authorized and increasingly popular Slovakian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Noah",
         "synonyms": [
             "Belo Otelo",
             "Charvat",
             "Flaga Alba",
             "Fraga",
             "Noa",
             "Noé",
             "Noka",
             "Nova",
-            "Tatar Rizling",
+            "Tatar Rizling"
         ],
-        "description": "American hybrid once popular in Europe, notably Spanish Basque Country, but now almost extinct.",
-        "color": "white",
+        "description": {
+            "default": "American hybrid once popular in Europe, notably Spanish Basque Country, but now almost extinct.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Noble",
-        "synonyms": ["North Carolina 20-119"],
-        "description": "Productive Muscadine variety widely grown in North Carolina for juice and wine.",
-        "color": "black",
+        "synonyms": [
+            "North Carolina 20-119"
+        ],
+        "description": {
+            "default": "Productive Muscadine variety widely grown in North Carolina for juice and wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nobling",
-        "synonyms": ["Freiburg 128-40"],
-        "description": "Demanding German cross making neutral wines.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 128-40"
+        ],
+        "description": {
+            "default": "Demanding German cross making neutral wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Nocera",
         "synonyms": [
             "Nocera di Catania",
             "Nocera Mantonico",
             "Nocera Nera di Milazzo",
             "Nucera",
-            "Nucera Niura",
+            "Nucera Niura"
         ],
-        "description": "Minor blending ingredient in Calabria and Sicilia.",
-        "color": "black",
+        "description": {
+            "default": "Minor blending ingredient in Calabria and Sicilia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Noir Fleurien",
         "synonyms": [
             "Damas Rouge",
             "Fleurien Noir",
             "Mire-Fleurien",
             "Mirefleurien",
-            "Noir-Fleurien",
+            "Noir-Fleurien"
         ],
-        "description": "Ancient and very rare Auvergne vine.",
-        "color": "black",
+        "description": {
+            "default": "Ancient and very rare Auvergne vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Noiret",
-        "synonyms": ["NY 73.0136.17"],
-        "description": "Promising new American hybrid producing peppery, well-structured dry reds.",
-        "color": "black",
+        "synonyms": [
+            "NY 73.0136.17"
+        ],
+        "description": {
+            "default": "Promising new American hybrid producing peppery, well-structured dry reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Norton",
         "synonyms": [
             "Arkansas",
             "Cynthiana",
             "Norton Virginia",
             "Norton’s Seedling",
             "Norton’s Virginia Seedling",
             "Red River",
             "Virginia",
-            "Vitis Nortoni",
+            "Vitis Nortoni"
         ],
-        "description": "Old, very successful American hybrid making rich, vinifera-like reds in a wide range of US states.",
-        "color": "black",
+        "description": {
+            "default": "Old, very successful American hybrid making rich, vinifera-like reds in a wide range of US states.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nosiola",
         "synonyms": [
             "Groppello Bianco",
             "Nosellara",
             "Nosiola Gentile",
             "Nusiola",
-            "Spargelen",
+            "Spargelen"
         ],
-        "description": "Trentino-Alto Adige variety long appreciated for Vino Santo but now making waves for its characterful dry wine.",
-        "color": "white",
+        "description": {
+            "default": "Trentino-Alto Adige variety long appreciated for Vino Santo but now making waves for its characterful dry wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Notardomenico",
-        "synonyms": ["Notar Domenico"],
-        "description": "Minor variety of unknown origin found in Puglia today.",
-        "color": "black",
+        "synonyms": [
+            "Notar Domenico"
+        ],
+        "description": {
+            "default": "Minor variety of unknown origin found in Puglia today.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Nuragus",
         "synonyms": [
             "Abbondosa",
             "Axina ’e Pòberus",
             "Axina Scacciadèppidus",
-            "Preni Tineddus",
+            "Preni Tineddus"
         ],
-        "description": "Ancient, fertile and generally unremarkable Sardinian.",
-        "color": "white",
+        "description": {
+            "default": "Ancient, fertile and generally unremarkable Sardinian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Odessky Cherny",
         "synonyms": [
             "Alibernet",
             "Oděskij Čornyj",
             "Odessa Black",
             "Odesskii Chernyi",
-            "Semenac 1-17-4",
+            "Semenac 1-17-4"
         ],
-        "description": "Red-fleshed, versatile Ukrainian cross that reveals its Cabernet parentage.",
-        "color": "black",
+        "description": {
+            "default": "Red-fleshed, versatile Ukrainian cross that reveals its Cabernet parentage.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Oeillade Noire",
         "synonyms": [
             "Aragnan Noir",
             "Ouillade",
             "Ouillard",
             "Ouliade",
-            "Passerille Noire",
+            "Passerille Noire"
         ],
-        "description": "Disappearing, dark-skinned, southern French variety more popular as a table grape.",
-        "color": "black",
+        "description": {
+            "default": "Disappearing, dark-skinned, southern French variety more popular as a table grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ofthalmo",
         "synonyms": [
             "Oftalmo",
             "Ophtalmo",
             "Ophtalmon",
             "Optalmo",
             "Pephtalmo",
-            "Pophtalmo",
+            "Pophtalmo"
         ],
-        "description": "Rare Cypriot variety whose soft, light reds are generally hidden in blends.",
-        "color": "red",
+        "description": {
+            "default": "Rare Cypriot variety whose soft, light reds are generally hidden in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Ohridsko Crno",
-        "synonyms": ["Prespanka"],
-        "description": "Macedonian variety that was a casualty of phylloxera.",
-        "color": "black",
+        "synonyms": [
+            "Prespanka"
+        ],
+        "description": {
+            "default": "Macedonian variety that was a casualty of phylloxera.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ojaleshi",
-        "synonyms": ["Chonouri", "Odjaleshi", "Odzhaleshi", "Sconuri", "Svanuri"],
-        "description": "Georgian variety suspected of Turkish origins.",
-        "color": "black",
+        "synonyms": [
+            "Chonouri",
+            "Odjaleshi",
+            "Odzhaleshi",
+            "Sconuri",
+            "Svanuri"
+        ],
+        "description": {
+            "default": "Georgian variety suspected of Turkish origins.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Öküzgözü",
-        "synonyms": ["Kara Erik"],
-        "description": "Turkish variety with an increasing reputation for its juicy, fresh, aromatic reds.",
-        "color": "black",
+        "synonyms": [
+            "Kara Erik"
+        ],
+        "description": {
+            "default": "Turkish variety with an increasing reputation for its juicy, fresh, aromatic reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Onchette",
-        "synonyms": ["Ouchette"],
-        "description": "Recently rescued Isère variety.",
-        "color": "black",
+        "synonyms": [
+            "Ouchette"
+        ],
+        "description": {
+            "default": "Recently rescued Isère variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ondenc",
         "synonyms": [
             "Blanquette",
             "Irvine’s White",
             "Oundenc",
             "Oundenq",
             "Piquepout de Moissac",
-            "Plant de Gaillac",
+            "Plant de Gaillac"
         ],
-        "description": "Neglected variety persists in south-west France and in isolated spots in Australia.",
-        "color": "white",
+        "description": {
+            "default": "Neglected variety persists in south-west France and in isolated spots in Australia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Opsimo Edessis",
         "synonyms": [
             "Agriostaphylo",
             "Chimoniatiko",
             "Dopio",
@@ -7691,130 +12188,225 @@
             "Paschalino",
             "Raisin de Foustani",
             "Raisin de Karatzova",
             "Staphyli Edessis",
             "Staphyli Karatzovas",
             "Valandovski Drenak",
             "Zimsko Belo",
-            "Belo Zimsko",
+            "Belo Zimsko"
         ],
-        "description": "Inferior northern Greek variety also grown for the table.",
-        "color": "white",
+        "description": {
+            "default": "Inferior northern Greek variety also grown for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Optima",
-        "synonyms": ["Optima 113"],
-        "description": "German cross designed to reach stupendous sugar levels even on poor sites.",
-        "color": "white",
+        "synonyms": [
+            "Optima 113"
+        ],
+        "description": {
+            "default": "German cross designed to reach stupendous sugar levels even on poor sites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Orangetraube",
-        "synonyms": ["Gelbe Orangetraube", "Narancsszőlő", "Orangentraube"],
-        "description": "Variety with a much-discussed history but now strictly limited geography.",
-        "color": "white",
+        "synonyms": [
+            "Gelbe Orangetraube",
+            "Narancsszőlő",
+            "Orangentraube"
+        ],
+        "description": {
+            "default": "Variety with a much-discussed history but now strictly limited geography.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Oraniensteiner",
-        "synonyms": ["Geisenheim 11-34", "Hochkroner"],
-        "description": "German cross that seems to have a found a niche in Canada.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 11-34",
+            "Hochkroner"
+        ],
+        "description": {
+            "default": "German cross that seems to have a found a niche in Canada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Orion",
-        "synonyms": ["Geilweilerhof GA-58-30"],
-        "description": "Little-planted cool-climate German hybrid similar to Müller-Thurgau.",
-        "color": "white",
+        "synonyms": [
+            "Geilweilerhof GA-58-30"
+        ],
+        "description": {
+            "default": "Little-planted cool-climate German hybrid similar to Müller-Thurgau.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Orleans Gelb",
         "synonyms": [
             "Gelber Orleans",
             "Hart-Heunscht",
             "Hartheinisch",
             "Harthengst",
             "Hart-Hängst",
             "Harthinsch",
             "Orleaner",
             "Orléans Jaune",
             "Orleanser",
             "Orleanstraube",
-            "Weisser Orleans",
+            "Weisser Orleans"
         ],
-        "description": "Ancient but now very minor, high-acid German vine replaced by Riesling. The oldest vines in Germany may be Orleans Gelb.",
-        "color": "white",
+        "description": {
+            "default": "Ancient but now very minor, high-acid German vine replaced by Riesling. The oldest vines in Germany may be Orleans Gelb.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ortega",
-        "synonyms": ["Würzburg 48-21-4"],
-        "description": "Early-ripening Gerrman cross that can achieve impressive sugar levels if not acidity.",
-        "color": "white",
+        "synonyms": [
+            "Würzburg 48-21-4"
+        ],
+        "description": {
+            "default": "Early-ripening Gerrman cross that can achieve impressive sugar levels if not acidity.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ortrugo",
-        "synonyms": ["Altruga", "Altrugo", "Artrugo"],
-        "description": "Emilia-Romagnan often blended with the most aromatic Malvasia.",
-        "color": "white",
+        "synonyms": [
+            "Altruga",
+            "Altrugo",
+            "Artrugo"
+        ],
+        "description": {
+            "default": "Emilia-Romagnan often blended with the most aromatic Malvasia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Oseleta",
-        "synonyms": ["Oselina"],
-        "description": "Revived and rather fashionable in Valpolicella country.",
-        "color": "black",
+        "synonyms": [
+            "Oselina"
+        ],
+        "description": {
+            "default": "Revived and rather fashionable in Valpolicella country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Osteiner",
-        "synonyms": ["Geisenheim 9-97"],
-        "description": "Very minor German cross with a successful outpost in New Zealand.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 9-97"
+        ],
+        "description": {
+            "default": "Very minor German cross with a successful outpost in New Zealand.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Österreichisch Weiss",
-        "synonyms": ["Kahlenberger Weisse"],
-        "description": "Rare light-skinned Viennese variety with a well-known offspring.",
-        "color": "white",
+        "synonyms": [
+            "Kahlenberger Weisse"
+        ],
+        "description": {
+            "default": "Rare light-skinned Viennese variety with a well-known offspring.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Otskhanuri Sapere",
-        "synonyms": ["Argvetuli Sapere"],
-        "description": "Minor Georgian variety responsible for deeply coloured, ageworthy reds.",
-        "color": "black",
+        "synonyms": [
+            "Argvetuli Sapere"
+        ],
+        "description": {
+            "default": "Minor Georgian variety responsible for deeply coloured, ageworthy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Padeiro",
-        "synonyms": ["Padeiro de Basto", "Tinto Matias"],
-        "description": "Productive but good-quality Portuguese variety makes rosé and light-red wines.",
-        "color": "black",
+        "synonyms": [
+            "Padeiro de Basto",
+            "Tinto Matias"
+        ],
+        "description": {
+            "default": "Productive but good-quality Portuguese variety makes rosé and light-red wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pálava",
-        "synonyms": ["Nema", "Veverka"],
-        "description": "Pink-skinned Czech cross producing full-bodied yet fresh, spicy whites.",
-        "color": "pink",
+        "synonyms": [
+            "Nema",
+            "Veverka"
+        ],
+        "description": {
+            "default": "Pink-skinned Czech cross producing full-bodied yet fresh, spicy whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Pallagrello Bianco",
         "synonyms": [
             "Pallagrella Bianca",
             "Pallagrello di Avellino",
             "Pallarella",
-            "Piedimonte Bianco",
+            "Piedimonte Bianco"
         ],
-        "description": "Old, rare Campanian, not unlike Viognier.",
-        "color": "white",
+        "description": {
+            "default": "Old, rare Campanian, not unlike Viognier.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pallagrello Nero",
         "synonyms": [
             "Coda di Volpe Nera",
             "Pallagrella Nera",
             "Piedilungo",
-            "Piedimonte Rosso",
+            "Piedimonte Rosso"
         ],
-        "description": "Rare dark-skinned variety from Campania, unrelated to Pallagrello Bianco.",
-        "color": "black",
+        "description": {
+            "default": "Rare dark-skinned variety from Campania, unrelated to Pallagrello Bianco.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Palomino Fino",
         "synonyms": [
             "Albán",
             "Albar",
             "Albillo de Lucena",
@@ -7834,75 +12426,106 @@
             "Ojo de Liebre",
             "Palomina Blanca",
             "Palomino",
             "Palomino Macho",
             "Palomino Pelusón",
             "Temprana",
             "Tempranilla",
-            "Xeres",
+            "Xeres"
         ],
-        "description": "The sherry grape.",
-        "color": "white",
+        "description": {
+            "default": "The sherry grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pamid",
         "synonyms": [
             "Grechesky Rosovy",
             "Manaluki",
             "Pamidi",
             "Pamitis",
             "Piros Szlanka",
             "Plovdina",
             "Roşioar",
             "Saratchoubouk",
-            "Slankamenka Crvena",
+            "Slankamenka Crvena"
         ],
-        "description": "Old, widely planted but uninspiring Bulgarian red wine grape.",
-        "color": "pink, red and black",
+        "description": {
+            "default": "Old, widely planted but uninspiring Bulgarian red wine grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink, red and black"
     },
     {
         "name": "Pampanuto",
-        "synonyms": ["Pampanino", "Pampanuta", "Rizzulo"],
-        "description": "Minor and largely unexciting Puglian.",
-        "color": "white",
+        "synonyms": [
+            "Pampanino",
+            "Pampanuta",
+            "Rizzulo"
+        ],
+        "description": {
+            "default": "Minor and largely unexciting Puglian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Papazkarasi",
-        "synonyms": ["Papaskara", "Papaz Karası"],
-        "description": "Turkish variety found mainly in Trakya (Thrace) with a very local purpose.",
-        "color": "black",
+        "synonyms": [
+            "Papaskara",
+            "Papaz Karası"
+        ],
+        "description": {
+            "default": "Turkish variety found mainly in Trakya (Thrace) with a very local purpose.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pardillo",
         "synonyms": [
             "Blanca Pequeña",
             "Marisancho",
             "Parda",
             "Pardilla",
             "Pardillo de Madrid",
             "Parill Blanco",
-            "Temprana Media",
+            "Temprana Media"
         ],
-        "description": "Local La Mancha variety producing well-structured, non-aromatic wines.",
-        "color": "white",
+        "description": {
+            "default": "Local La Mancha variety producing well-structured, non-aromatic wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Parellada",
         "synonyms": [
             "Martorella",
             "Moltonach",
             "Montañesa",
             "Montona",
             "Montònec",
             "Montónega",
             "Montonench",
-            "Verda Grossa",
+            "Verda Grossa"
         ],
-        "description": "Aromatic variety with high quality potential used mainly in the production of Cava.",
-        "color": "white",
+        "description": {
+            "default": "Aromatic variety with high quality potential used mainly in the production of Cava.",
+            "julie": "Parellada is a white grape variety mostly used for the production of Cava wines. It produces aromatic wines with a moderate level of alcohol and a juicy acidity.",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Parraleta",
         "synonyms": [
             "Bonifaccencu",
             "Bonifacienco",
             "Bonvedro",
@@ -7926,24 +12549,36 @@
             "Preto Foz",
             "Preto João Mendes",
             "Salceño Negro",
             "Tinta Caiada",
             "Tinta Grossa",
             "Tinta Lameira",
             "Tintorro",
-            "Torres de Algarve",
+            "Torres de Algarve"
         ],
-        "description": "Distinctive Somontano variety producing dark, aromatic wines in several countries and under many different names.",
-        "color": "black",
+        "description": {
+            "default": "Distinctive Somontano variety producing dark, aromatic wines in several countries and under many different names.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pascal Blanc",
-        "synonyms": ["Pascal", "Pascaou", "Pascau"],
-        "description": "Historic variety barely surviving in Provence.",
-        "color": "white",
+        "synonyms": [
+            "Pascal",
+            "Pascaou",
+            "Pascau"
+        ],
+        "description": {
+            "default": "Historic variety barely surviving in Provence.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pascale",
         "synonyms": [
             "Barberone",
             "Falso Gregu",
             "Giacomino",
@@ -7951,164 +12586,231 @@
             "Nera Tomentosa",
             "Nieddu Mannu",
             "Nieddu Pedra Serra",
             "Pascale di Cagliari",
             "Pascale Nero",
             "Pasquale",
             "Picciolo Rosso",
-            "Primidivu Nieddu",
+            "Primidivu Nieddu"
         ],
-        "description": "Dark-skinned Sardinian rarely bottled on its own.",
-        "color": "black",
+        "description": {
+            "default": "Dark-skinned Sardinian rarely bottled on its own.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Passau",
-        "synonyms": ["Incrocio Dalmasso 17/25"],
-        "description": "Very minor Veneto cross whose correct parentage has only recently been identified.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso 17/25"
+        ],
+        "description": {
+            "default": "Very minor Veneto cross whose correct parentage has only recently been identified.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Passerina",
         "synonyms": [
             "Cacciadebiti",
             "Caccione",
             "Camplese",
             "Pagadebito",
             "Scacciadebito",
             "Trebbiano di Teramo",
             "Uva d’Oro",
-            "Uva Fermana",
+            "Uva Fermana"
         ],
-        "description": "Old variety from Italy’s Adriatic coast made in a variety of styles.",
-        "color": "white",
+        "description": {
+            "default": "Old variety from Italy’s Adriatic coast made in a variety of styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pavana",
         "synonyms": [
             "Nera Gentile di Fonzaso",
             "Nostrana Nera",
             "Pelosetta",
             "Ussulara",
             "Vicentina",
-            "Visentina",
+            "Visentina"
         ],
-        "description": "Much diminished, now highly localized, northern Italian.",
-        "color": "black",
+        "description": {
+            "default": "Much diminished, now highly localized, northern Italian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pecorino",
         "synonyms": [
             "Arquitano",
             "Norcino",
             "Pecorina Arquatanella",
             "Pecorino di Osimo",
             "Promotico",
             "Uva delle Pecore",
             "Uva Pecorina",
-            "Vissanello",
+            "Vissanello"
         ],
-        "description": "Marche speciality enjoying a certain modishness. Mineral or herbal dry whites.",
-        "color": "white",
+        "description": {
+            "default": "Marche speciality enjoying a certain modishness. Mineral or herbal dry whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pedral",
         "synonyms": [
             "Alvarinho Tinto",
             "Cainho dos Milagres",
             "Cainho Espanhol",
             "Dozal",
             "Padral",
             "Pardal",
             "Pedrol",
             "Pégudo",
             "Perna de Perdiz",
-            "Verdejo Colorado",
+            "Verdejo Colorado"
         ],
-        "description": "Rare Minho variety, now more common (just) over the border in Spain and found in blends.",
-        "color": "black",
+        "description": {
+            "default": "Rare Minho variety, now more common (just) over the border in Spain and found in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pedro Giménez",
-        "synonyms": ["Pedro Jiménez"],
-        "description": "Quantitatively if not qualitatively important Argentine white unrelated to Spain’s Pedro Ximénez.",
-        "color": "white",
+        "synonyms": [
+            "Pedro Jiménez"
+        ],
+        "description": {
+            "default": "Quantitatively if not qualitatively important Argentine white unrelated to Spain’s Pedro Ximénez.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pedro Ximénez",
         "synonyms": [
             "Corinto Bianco",
             "Don Bueno",
             "Pedro Jimenez",
             "Pedro Ximenes",
             "Perrum",
             "PX",
             "Verdello",
-            "Ximenes",
+            "Ximenes"
         ],
-        "description": "Andalucía’s variety used mainly for some of the darkest, stickiest wines made anywhere.",
-        "color": "white",
+        "description": {
+            "default": "Andalucía’s variety used mainly for some of the darkest, stickiest wines made anywhere.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pelaverga",
         "synonyms": [
             "Cari",
             "Pelaverga di Pagno",
             "Pelaverga Grosso",
             "Uva Coussa",
-            "Uva delle Zucche",
+            "Uva delle Zucche"
         ],
-        "description": "The more commonly planted, big-berried Pelaverga, often blended with Nebbiolo and/or Barbera in Piemonte.",
-        "color": "black",
+        "description": {
+            "default": "The more commonly planted, big-berried Pelaverga, often blended with Nebbiolo and/or Barbera in Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pelaverga Piccolo",
-        "synonyms": ["Pelaverga di Verduno"],
-        "description": "Fashionable if relatively minor Piemontese making light, fruity, spicy varietal reds.",
-        "color": "black",
+        "synonyms": [
+            "Pelaverga di Verduno"
+        ],
+        "description": {
+            "default": "Fashionable if relatively minor Piemontese making light, fruity, spicy varietal reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Peloursin",
         "synonyms": [
             "Corsin",
             "Fumette",
             "Feunette",
             "Gros Béclan",
             "Pelossard",
             "Péloursin",
             "Pourret",
-            "Pourrot",
+            "Pourrot"
         ],
-        "description": "From Isère, now mostly of historical and genetic significance.",
-        "color": "black",
+        "description": {
+            "default": "From Isère, now mostly of historical and genetic significance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Perera",
-        "synonyms": ["Perera Gialla", "Pevarise"],
-        "description": "Old variety of the Veneto used to perfume passito and sparkling wines in Prosecco country.",
-        "color": "white",
+        "synonyms": [
+            "Perera Gialla",
+            "Pevarise"
+        ],
+        "description": {
+            "default": "Old variety of the Veneto used to perfume passito and sparkling wines in Prosecco country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Perle",
-        "synonyms": ["Perle von Alzey"],
-        "description": "Pink-berried German cross with a hint of its rose-like parental perfume but short on freshness.",
-        "color": "pink",
+        "synonyms": [
+            "Perle von Alzey"
+        ],
+        "description": {
+            "default": "Pink-berried German cross with a hint of its rose-like parental perfume but short on freshness.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Perricone",
         "synonyms": [
             "Catarratto Rouge",
             "Niuru",
             "Perricone Nero",
             "Pignateddu",
             "Pignatello",
             "Pirricuni",
-            "Tuccarinu",
+            "Tuccarinu"
         ],
-        "description": "Dark-skinned, relatively tannic Sicilian, often blended with Nero d’Avola.",
-        "color": "black",
+        "description": {
+            "default": "Dark-skinned, relatively tannic Sicilian, often blended with Nero d’Avola.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Perruno",
         "synonyms": [
             "Casta de Montúo",
             "Firmissima",
             "Getibi",
@@ -8118,18 +12820,22 @@
             "Perruna",
             "Perruno Común",
             "Perruno de Arcos",
             "Perruno de la Sierra",
             "Perruno Duro",
             "Perruno Fino",
             "Perruno Tierno",
-            "Vidueño",
+            "Vidueño"
         ],
-        "description": "Old Extremaduran variety with a lone supporter in Andalucía.",
-        "color": "white",
+        "description": {
+            "default": "Old Extremaduran variety with a lone supporter in Andalucía.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Persan",
         "synonyms": [
             "Beccu",
             "Bécuet",
             "Becuét",
@@ -8137,219 +12843,357 @@
             "Berla‘d Crava Cita",
             "Berlo Citto",
             "Etraire",
             "Etris",
             "Princens",
             "Prinsens",
             "Serine",
-            "Siranne",
+            "Siranne"
         ],
-        "description": "Rare but high-quality Savoie variety on a voyage of rediscovery.",
-        "color": "black",
+        "description": {
+            "default": "Rare but high-quality Savoie variety on a voyage of rediscovery.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pervenets Magaracha",
-        "synonyms": ["Pervenec Magaraca", "Pervenyec Magaracsa"],
-        "description": "Recent Ukrainian cross notably resistant to downy mildew and used for dry and sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Pervenec Magaraca",
+            "Pervenyec Magaracsa"
+        ],
+        "description": {
+            "default": "Recent Ukrainian cross notably resistant to downy mildew and used for dry and sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petit Bouschet",
         "synonyms": [
             "Aramon-Teinturier",
             "Bouschet Petit",
             "Negrón de Aldán",
-            "Tintinha",
+            "Tintinha"
         ],
-        "description": "Disappearing red-juiced nineteenth-century southern French cross.",
-        "color": "black",
+        "description": {
+            "default": "Disappearing red-juiced nineteenth-century southern French cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Petit Courbu",
         "synonyms": [
             "Courbis",
             "Courbu Petit",
             "Petit Courbu Blanc",
             "Vieux Pacherenc",
-            "Xuri Zerratu",
+            "Xuri Zerratu"
         ],
-        "description": "Minor but high-quality, aromatic Jurançon speciality.",
-        "color": "white",
+        "description": {
+            "default": "Minor but high-quality, aromatic Jurançon speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petit Manseng",
         "synonyms": [
             "Izkiriot Ttipi",
             "Iskiriota Zuri Tipia",
             "Ichiriota Zuria Tipia",
             "Manseng Petit Blanc",
-            "Mansengou",
+            "Mansengou"
         ],
-        "description": "High-quality variety making superb sweet wines in south-western France.",
-        "color": "white",
+        "description": {
+            "default": "High-quality variety making superb sweet wines in south-western France.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petit Meslier",
-        "synonyms": ["Melié Blanc", "Meslier Doré", "Meslier Jaune", "Meslier Petit"],
-        "description": "Extremely rare, light-berried potential champagne ingredient with significant relatives and a lone outpost in Australia.",
-        "color": "white",
+        "synonyms": [
+            "Melié Blanc",
+            "Meslier Doré",
+            "Meslier Jaune",
+            "Meslier Petit"
+        ],
+        "description": {
+            "default": "Extremely rare, light-berried potential champagne ingredient with significant relatives and a lone outpost in Australia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petit Rouge",
-        "synonyms": ["Oriou", "Picciourouzo"],
-        "description": "Old, dark-skinned Aostan producing spicy, redcurrant-flavoured wines.",
-        "color": "black",
+        "synonyms": [
+            "Oriou",
+            "Picciourouzo"
+        ],
+        "description": {
+            "default": "Old, dark-skinned Aostan producing spicy, redcurrant-flavoured wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Petit Verdot",
-        "synonyms": ["Lambrusquet", "Verdau", "Verdot", "Verdot Petit"],
-        "description": "High-quality, late-ripening Bordeaux variety adding colour and spice to blends there but making an increasing number of solo appearances elsewhere.",
-        "color": "black",
+        "synonyms": [
+            "Lambrusquet",
+            "Verdau",
+            "Verdot",
+            "Verdot Petit"
+        ],
+        "description": {
+            "default": "High-quality, late-ripening Bordeaux variety adding colour and spice to blends there but making an increasing number of solo appearances elsewhere.",
+            "julie": "Petit Verdot produces wines which are powerful, rich, deeply coloured, tannic and ageworthy. Small plantings are found in the region of Bordeaux, where it originates, and where it is still used in blends. The grape is also planted in various countries such as USA (California), Argentina and Australia. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Petite Amie",
-        "synonyms": ["DM 8313.1"],
-        "description": "Recent and promisingly aromatic American hybrid planted in Nebraska.",
-        "color": "white",
+        "synonyms": [
+            "DM 8313.1"
+        ],
+        "description": {
+            "default": "Recent and promisingly aromatic American hybrid planted in Nebraska.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petite Pearl",
-        "synonyms": ["TP 2-1-24"],
-        "description": "Promising new cold-hardy American hybrid.",
-        "color": "black",
+        "synonyms": [
+            "TP 2-1-24"
+        ],
+        "description": {
+            "default": "Promising new cold-hardy American hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Petra",
-        "synonyms": ["Petka"],
-        "description": "Serbian hybrid producing full-bodied, aromatic whites.",
-        "color": "white",
+        "synonyms": [
+            "Petka"
+        ],
+        "description": {
+            "default": "Serbian hybrid producing full-bodied, aromatic whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petrokoritho",
-        "synonyms": ["Petrocoritho", "Pietro Corinto"],
-        "description": "Greek island variety of which the white mutation is the stronger survivor.",
-        "color": "white",
+        "synonyms": [
+            "Petrocoritho",
+            "Pietro Corinto"
+        ],
+        "description": {
+            "default": "Greek island variety of which the white mutation is the stronger survivor.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Petroulianos",
-        "synonyms": ["Petrolianos"],
-        "description": "Rare but promising vine from the southern tip of Greece’s Pelopónnisos (Peloponnese).",
-        "color": "white",
+        "synonyms": [
+            "Petrolianos"
+        ],
+        "description": {
+            "default": "Rare but promising vine from the southern tip of Greece’s Pelopónnisos (Peloponnese).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Phoenix",
-        "synonyms": ["Geilweilerhof GA-49-22"],
-        "description": "Disease-resistant German hybrid producing fresh and lightly aromatic wines in the UK.",
-        "color": "white",
+        "synonyms": [
+            "Geilweilerhof GA-49-22"
+        ],
+        "description": {
+            "default": "Disease-resistant German hybrid producing fresh and lightly aromatic wines in the UK.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Picapoll Blanco",
         "synonyms": [
             "Blanca Extra",
             "Clairette Blanche",
             "Picapoll",
-            "Picapolla Blanca",
+            "Picapolla Blanca"
         ],
-        "description": "Minor Catalan that may be the same as France’s Clairette Blanche.",
-        "color": "white",
+        "description": {
+            "default": "Minor Catalan that may be the same as France’s Clairette Blanche.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Picardan",
         "synonyms": [
             "Aragnan",
             "Aragnan Blanc",
             "Araignan Blanc",
             "Gallet",
             "Gallet Blanc",
             "Grosse Clairette",
             "Milhaud Blanc",
             "Papadoux",
             "Oeillade Blanche",
-            "Picardan Blanc",
+            "Picardan Blanc"
         ],
-        "description": "Occasionally adds acidity to Châteauneuf.",
-        "color": "white",
+        "description": {
+            "default": "Occasionally adds acidity to Châteauneuf.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Piccola Nera",
-        "synonyms": ["Mala Cerna", "Nera Tenera"],
-        "description": "Makes very pale reds in the hinterland of Trieste.",
-        "color": "pink",
+        "synonyms": [
+            "Mala Cerna",
+            "Nera Tenera"
+        ],
+        "description": {
+            "default": "Makes very pale reds in the hinterland of Trieste.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Picolit",
-        "synonyms": ["Pikolit"],
-        "description": "Ancient Friulian producing small quantities of highly regarded sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Pikolit"
+        ],
+        "description": {
+            "default": "Ancient Friulian producing small quantities of highly regarded sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Piculit Neri",
-        "synonyms": ["Picolit Neri", "Picolit Nero"],
-        "description": "Old, rare, small-berried red wine variety unrelated to Picolit.",
-        "color": "black",
+        "synonyms": [
+            "Picolit Neri",
+            "Picolit Nero"
+        ],
+        "description": {
+            "default": "Old, rare, small-berried red wine variety unrelated to Picolit.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Piedirosso",
         "synonyms": [
             "Palombina",
             "Palumbina",
             "Palumbo",
             "Palummina",
             "Per’e Palummo",
-            "Streppa Verde",
+            "Streppa Verde"
         ],
-        "description": "Fresh, aromatic Campanian that makes an ideal blending partner for Aglianico but can also shine as a varietal.",
-        "color": "black",
+        "description": {
+            "default": "Fresh, aromatic Campanian that makes an ideal blending partner for Aglianico but can also shine as a varietal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pignola Valtellinese",
         "synonyms": [
             "Groppello di Breganze",
             "Pignola",
             "Pignola Spanna",
-            "Pignolo Spano",
+            "Pignolo Spano"
         ],
-        "description": "Minor red wine grape grown in Lombardia and Piemonte, and in the Veneto as the recently rescued Groppello di Breganze.",
-        "color": "black",
+        "description": {
+            "default": "Minor red wine grape grown in Lombardia and Piemonte, and in the Veneto as the recently rescued Groppello di Breganze.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pignoletto",
         "synonyms": [
             "Grechetto di Todi",
             "Grechetto Gentile",
             "Occhietto",
             "Pallagrello di Caserta",
             "Pignoletto Bolognese",
             "Pignolino",
             "Pulcinculo",
             "Rébola",
             "Ribolla Riminese",
-            "Strozzavolpe",
+            "Strozzavolpe"
         ],
-        "description": "Light, refreshing variety quite widely planted in the Bologna hills and in Umbria.",
-        "color": "white",
+        "description": {
+            "default": "Light, refreshing variety quite widely planted in the Bologna hills and in Umbria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pineau D’Aunis",
         "synonyms": [
             "Aunis",
             "Chenin Noir",
             "Gros Pineau",
             "Gros-Véronais",
             "Plant d’Aunis",
-            "Plant de Mayet",
+            "Plant de Mayet"
         ],
-        "description": "Ancient, light and underrated Loire variety, often used for rosé but capable of interesting reds.",
-        "color": "black",
+        "description": {
+            "default": "Ancient, light and underrated Loire variety, often used for rosé but capable of interesting reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pinella",
-        "synonyms": ["Mattozza", "Pinela", "Pinjela", "Pinola"],
-        "description": "Minor variety from the hills south of Padova, also grown in neighbouring Slovenia.",
-        "color": "white",
+        "synonyms": [
+            "Mattozza",
+            "Pinela",
+            "Pinjela",
+            "Pinola"
+        ],
+        "description": {
+            "default": "Minor variety from the hills south of Padova, also grown in neighbouring Slovenia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pinot Noir",
         "synonyms": [
             "Auvernat",
             "Auvernas",
             "Black Burgundy",
@@ -8379,32 +13223,40 @@
             "Pinot Nero",
             "Plant Doré",
             "Rulandské Modré",
             "Savagnin Noir",
             "Salvagnin Noir",
             "Servagnin",
             "Spätburgunder",
-            "Vert Doré",
+            "Vert Doré"
         ],
-        "description": "Finicky Burgundian vine produces wildly variable, relatively delicate, potentially haunting essences of place.",
-        "color": "black",
+        "description": {
+            "default": "Finicky Burgundian vine produces wildly variable, relatively delicate, potentially haunting essences of place.",
+            "julie": "An incredibly elegant red grape variety thay thrives in cool climate area. King variety of red Burgundy wines, it also produces excellent wines in Germany under the name späburgunder, Austria, New Zealand, Tasmania, Oregon, etc. It is also the major components in many traditional method sparkling wines. ",
+            "sommelier": "Ranging from ruby to garnet red, Pinot Noir wines are slightly tannic, mild in acidity, and have a long finish with aromas reminiscent of blackberry and cherry. Pinot Noir wines taste full-bodied and velvety, with a fruity flavour and hints of almond. The typical Pinot Noir has a slightly sweetish aroma of red fruit, from strawberry to cherry and blackberry to blackcurrant. Barrique wines also have hints of vanilla and cinnamon. A distinction is made between the classic and the modern type. Traditionally, the best Pinot Noirs were made from very ripe grapes, were not very colourful, mild, low in tannins and reddish-red in colour. In addition to this classic type, the modern Pinot Noir with a strong red colour, more tannin, less acidity and often a short ageing period in small oak barrels is becoming increasingly important. Aroma: blackberries, cherries, strawberries, elderberries, pepper. Flavour: classic vinification: mild, low in tannins. Modern vinification: full-bodied and rich in tannins, full-bodied."
+        },
+        "color": "black"
     },
     {
         "name": "Pinot Meunier",
         "synonyms": [
             "Auvernat Blanc",
             "Gris Meunier",
             "Meunier",
             "Morillon Taconné",
             "Müllerrebe",
             "Samtrot",
-            "Schwarzriesling",
+            "Schwarzriesling"
         ],
-        "description": "Fruity blending ingredient for top-quality sparkling wine.",
-        "color": "black",
+        "description": {
+            "default": "Fruity blending ingredient for top-quality sparkling wine.",
+            "julie": "Pinot Meunier is a key player in the production of Champagne. The grapes contributes to adding softeness, juiciness and yellow fruit aromas and flavours to the wines. 100% Pinot Meunier Champagne are more commonly seen than in the past but the grape is rarely sold as a still wine. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pinot Gris",
         "synonyms": [
             "Auvernat Gris",
             "Beurot",
             "Burgunder Roter",
@@ -8423,18 +13275,22 @@
             "Râjik",
             "Ruländer",
             "Rulandské Šedé",
             "Rulandské Sivé",
             "Sivi Pinot",
             "Speyeren",
             "Szürkebarát",
-            "Tokay",
+            "Tokay"
         ],
-        "description": "Full-bodied and aromatic at its best but much more usually encountered enjoying international fame if not glory as anodyne Pinot Grigio.",
-        "color": "pink",
+        "description": {
+            "default": "Full-bodied and aromatic at its best but much more usually encountered enjoying international fame if not glory as anodyne Pinot Grigio.",
+            "julie": "Wines labelled as Pinot Gris tend to have body, texture a good aromatic intensity reminescent of stone fruits, flowers and spices. Wines labelled as Pinot Grigio, however made from the same grape variety, are generarlly light, crisp and farily neutral. ",
+            "sommelier": "Although it is a mutation of Pinot Noir and has pinkish skin, Grauburgunder is a white wine grape. It produces pale to golden yellow wines reminiscent of mango, nuts, almonds, and quince. It is vinified in stainless steel or oak, and typically denotes a dry, medium-bodied wine with fairly lively acidity. A young, light, dry to semi-dry Pinot Gris is well suited as a summer wine. Dry Kabinett wines and Spätlese wines harmonise well with seafood, strong sea fish, pasta, lamb, wild fowl and young game as well as ripe soft cheeses. Barrique wines go well with intense-tasting lamb dishes and light game dishes, such as wild fowl or venison. Fruity-sweet Spätlese or noble sweet Auslese wines go particularly well with fatty blue cheese and desserts with honey, almonds or marzipan. Depending on the vinification method and quality level, the colour is pale yellow, golden yellow or even amber. Pinot gris is associated in particular with aromas of green nuts, almonds and fresh butter, as well as fruity aromas reminiscent of pears, dried fruit and sultanas, pineapple and citrus fruits. Vegetative notes of green beans or peppers also appear."
+        },
+        "color": "pink"
     },
     {
         "name": "Pinot Blanc",
         "synonyms": [
             "Auvernat Blanc",
             "Beli Pinot",
             "Burgunder Veisser",
@@ -8448,24 +13304,35 @@
             "Pinot Bijeli",
             "Pinot Blanc Vrai",
             "Pinot Branco",
             "Rulandské Biele",
             "Rulandské Bílé",
             "Weissburgunder",
             "Weisser Burgunder",
-            "Burgunder Weiss",
+            "Burgunder Weiss"
         ],
-        "description": "Possibly underrated producer of friendly, medium-bodied, confident whites. Easy to ripen.",
-        "color": "white",
+        "description": {
+            "default": "Possibly underrated producer of friendly, medium-bodied, confident whites. Easy to ripen.",
+            "julie": "For years Pinot Blanc has been mistaken for Chardonnay as the grapes look very similar..Pinot Blanc, however is a colour mutation of Pinot Noir and is mostly found in Alsace where it is used for the production of Crémants but also for the production of elegant, fresh and moderatly complex white wines. The variety is known as Pinot Bianco in Italy and Weissburgunder in Austria and Germany, two countries that produces some exceptionnally good examples of the variety. ",
+            "sommelier": "Pinot Blanc presents itself as pale to light yellow in the glass, delicate and restrained on the nose. Its slightly nutty aroma is typical. When dry, its medium to full body and fine acidity make it suitable for many dishes. Aroma: discreet, reminiscent of apples, pears, mangos, nuts, quinces. Not overly rich in alcohol, Pinot Blanc has a discreet aroma, often reminiscent of green nuts, apple, pear, quince, apricot, citrus fruit or fresh pineapple. Moderate body and a pleasantly refreshing acidity characterise it as a versatile menu wine. It is therefore well suited to seafood, fish, veal, pork and poultry, or simply as a well-chilled terrace wine."
+        },
+        "color": "white"
     },
     {
         "name": "Pinot Teinturier",
-        "synonyms": ["Farbclevner", "Pinot Fin Teinturier"],
-        "description": "Red-fleshed Pinot mutation.",
-        "color": "black",
+        "synonyms": [
+            "Farbclevner",
+            "Pinot Fin Teinturier"
+        ],
+        "description": {
+            "default": "Red-fleshed Pinot mutation.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pinot Noir Précoce",
         "synonyms": [
             "Augustclevner",
             "Augusttraube",
             "Blauer Frühburgunder",
@@ -8478,447 +13345,776 @@
             "Madeleine Noire",
             "Möhrchen",
             "Morillon Noir Hâtif",
             "Pinot Hâtif de Rilly",
             "Pinot Madeleine",
             "Pinot Précoce",
             "Pinot Précoce Noir",
-            "Raisin de la Madeleine",
+            "Raisin de la Madeleine"
         ],
-        "description": "Early-ripening mutation of Pinot Noir that is currently popular in Germany as Frühburgunder.",
-        "color": "black",
+        "description": {
+            "default": "Early-ripening mutation of Pinot Noir that is currently popular in Germany as Frühburgunder.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pinotage",
-        "synonyms": ["Perold’s Hermitage × Pinot"],
-        "description": "South Africa’s very own cross, both loved and despised.",
-        "color": "black",
+        "synonyms": [
+            "Perold’s Hermitage × Pinot"
+        ],
+        "description": {
+            "default": "South Africa’s very own cross, both loved and despised.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pinotin",
-        "synonyms": ["VB 91-26-19"],
-        "description": "Recent, obscure Swiss hybrid.",
-        "color": "black",
+        "synonyms": [
+            "VB 91-26-19"
+        ],
+        "description": {
+            "default": "Recent, obscure Swiss hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pionnier",
-        "synonyms": ["ES 4-7-25"],
-        "description": "Minor but complex, cold-hardy American hybrid used in blends in Québec.",
-        "color": "black",
+        "synonyms": [
+            "ES 4-7-25"
+        ],
+        "description": {
+            "default": "Minor but complex, cold-hardy American hybrid used in blends in Québec.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Piquepoul Noir",
-        "synonyms": ["Picapoll Negro", "Picapoll Tinta"],
-        "description": "DNA profiling has recently shown that PICAPOLL BLANCO, a white variety from Pla de Bages in Catalunya, north-east Spain, already mentioned in the sixteenth century and long considered identical to the French Piquepoul Blanc, is in fact a distinct variety that is much more closely related to CLAIRETTE, possibly a clone (Puig et al. 2006). However, Picapoll Negro has been shown to be identical to Piqupoul Noir (Galet 2000). Piquepoul belongs to the Piquepoul ampelographic group (see p XXVII; Bisson 2009).",
-        "color": "black",
+        "synonyms": [
+            "Picapoll Negro",
+            "Picapoll Tinta"
+        ],
+        "description": {
+            "default": "DNA profiling has recently shown that PICAPOLL BLANCO, a white variety from Pla de Bages in Catalunya, north-east Spain, already mentioned in the sixteenth century and long considered identical to the French Piquepoul Blanc, is in fact a distinct variety that is much more closely related to CLAIRETTE, possibly a clone (Puig et al. 2006). However, Picapoll Negro has been shown to be identical to Piqupoul Noir (Galet 2000). Piquepoul belongs to the Piquepoul ampelographic group (see p XXVII; Bisson 2009).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Piquepoul Blanc",
         "synonyms": [
             "Avillo",
             "Languedocien",
             "Picpoul de Pinet",
-            "Piquepoul de Pinet",
+            "Piquepoul de Pinet"
         ],
-        "description": "Piquepoul Noir produces pale, alcoholic but aromatic and nervy wines well suited to rosé production and is much less widely planted than the white version – there were just 73 ha (180 acres) in southern France in 2008. Although it is recommended in most French wine-growing départements, and is a permitted variety in Châteauneuf-du-Pape and Côtes du Rhône, it is generally a very minor component in blends, unlike its more successful white mutation. A rare example of a Piquepoul Noir-dominant red wine is Minervois producer Clos Centeille’s C de Centeilles, which is 90% Piquepoul Noir and 10% RIVAIRENC; Domaine La Grangette just south of Pézenas bottle a varietal rosé.",
-        "color": "white",
+        "description": {
+            "default": "Piquepoul Noir produces pale, alcoholic but aromatic and nervy wines well suited to rosé production and is much less widely planted than the white version – there were just 73 ha (180 acres) in southern France in 2008. Although it is recommended in most French wine-growing départements, and is a permitted variety in Châteauneuf-du-Pape and Côtes du Rhône, it is generally a very minor component in blends, unlike its more successful white mutation. A rare example of a Piquepoul Noir-dominant red wine is Minervois producer Clos Centeille’s C de Centeilles, which is 90% Piquepoul Noir and 10% RIVAIRENC; Domaine La Grangette just south of Pézenas bottle a varietal rosé.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Plant Droit",
-        "synonyms": ["Cinsaut Droit", "Espanenc", "Garnacha Francesa", "Plant Dressé"],
-        "description": "Minor and diminishing southern Rhône variety producing rather pale reds.",
-        "color": "black",
+        "synonyms": [
+            "Cinsaut Droit",
+            "Espanenc",
+            "Garnacha Francesa",
+            "Plant Dressé"
+        ],
+        "description": {
+            "default": "Minor and diminishing southern Rhône variety producing rather pale reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Planta Nova",
-        "synonyms": ["Coma", "Malvasia", "Tardana", "Tortozon", "Tortozón"],
-        "description": "Actually very old but generally undistinguished variety grown mainly in Valencia today.",
-        "color": "white",
+        "synonyms": [
+            "Coma",
+            "Malvasia",
+            "Tardana",
+            "Tortozon",
+            "Tortozón"
+        ],
+        "description": {
+            "default": "Actually very old but generally undistinguished variety grown mainly in Valencia today.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Plantet",
-        "synonyms": ["Seibel 5455"],
-        "description": "Hybrid once popular in the Loire, now producing slightly odd, raspberry-flavoured wines.",
-        "color": "black",
+        "synonyms": [
+            "Seibel 5455"
+        ],
+        "description": {
+            "default": "Hybrid once popular in the Loire, now producing slightly odd, raspberry-flavoured wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Plantscher",
-        "synonyms": ["Bordeaux Blanc", "Bourgogne Blanc", "Gros Bourgogne"],
-        "description": "Very rare Swiss or possibly Hungarian variety just surviving in the Haut-Valais.",
-        "color": "white",
+        "synonyms": [
+            "Bordeaux Blanc",
+            "Bourgogne Blanc",
+            "Gros Bourgogne"
+        ],
+        "description": {
+            "default": "Very rare Swiss or possibly Hungarian variety just surviving in the Haut-Valais.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Plassa",
-        "synonyms": ["Scarlattino"],
-        "description": "Thick-skinned red making tannic wines south west of Torino.",
-        "color": "black",
+        "synonyms": [
+            "Scarlattino"
+        ],
+        "description": {
+            "default": "Thick-skinned red making tannic wines south west of Torino.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Platani",
-        "synonyms": ["Platania", "Platanos"],
-        "description": "Minor blending component on the Greek island of Santoríni.",
-        "color": "white",
+        "synonyms": [
+            "Platania",
+            "Platanos"
+        ],
+        "description": {
+            "default": "Minor blending component on the Greek island of Santoríni.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Plavac Mali",
         "synonyms": [
             "Crljenak",
             "Kasteljanak",
             "Pagadebit Crni",
             "Pagadebit Mali",
             "Plavac Mali Crni",
             "Plavac Veliki",
             "Plavec Mal",
-            "Zelenak",
+            "Zelenak"
         ],
-        "description": "Ancient and leading Croatian variety making powerful reds, genetically close but not identical to Tribidrag (Zinfandel).",
-        "color": "black",
+        "description": {
+            "default": "Ancient and leading Croatian variety making powerful reds, genetically close but not identical to Tribidrag (Zinfandel).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Plavec Žuti",
-        "synonyms": ["Debeli Klešec", "Plavac Žuti", "Plavec Rumeni", "Rumeni Plavec"],
-        "description": "Minor variety producing light, tart whites in Croatia and Slovenia.",
-        "color": "white",
+        "synonyms": [
+            "Debeli Klešec",
+            "Plavac Žuti",
+            "Plavec Rumeni",
+            "Rumeni Plavec"
+        ],
+        "description": {
+            "default": "Minor variety producing light, tart whites in Croatia and Slovenia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Plavina",
-        "synonyms": ["Brajda", "Brajdica", "Plavina Crna", "Plavka", "Plajka"],
-        "description": "Dark-skinned offspring of Tribidrag (Zinfandel) producing light reds the length of the Dalmatian coast.",
-        "color": "black",
+        "synonyms": [
+            "Brajda",
+            "Brajdica",
+            "Plavina Crna",
+            "Plavka",
+            "Plajka"
+        ],
+        "description": {
+            "default": "Dark-skinned offspring of Tribidrag (Zinfandel) producing light reds the length of the Dalmatian coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Plechistik",
         "synonyms": [
             "Bogata Kist",
             "Goryun",
             "Khreshchatinskii",
             "Letun",
             "Osipnijak",
             "Petoun",
             "Plechistik Tsimlyansky",
             "Plecistik",
-            "Rogataia Kisty",
+            "Rogataia Kisty"
         ],
-        "description": "Viticulturally difficult Russian variety used in sweet red sparkling wine.",
-        "color": "black",
+        "description": {
+            "default": "Viticulturally difficult Russian variety used in sweet red sparkling wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Plyto",
-        "synonyms": [": Plito", "Ploto", "Pluto", "Plytó"],
-        "description": "Rare, ancient, herbal-scented Cretan variety with great promise.",
-        "color": "white",
+        "synonyms": [
+            ": Plito",
+            "Ploto",
+            "Pluto",
+            "Plytó"
+        ],
+        "description": {
+            "default": "Rare, ancient, herbal-scented Cretan variety with great promise.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pollera Nera",
-        "synonyms": ["Corlaga", "Pollora Nera"],
-        "description": "Old dark-skinned variety grown in Liguria and north-west Toscana.",
-        "color": "black",
+        "synonyms": [
+            "Corlaga",
+            "Pollora Nera"
+        ],
+        "description": {
+            "default": "Old dark-skinned variety grown in Liguria and north-west Toscana.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pošip Bijeli",
-        "synonyms": ["Pošip", "Pošip Veliki", "Pošipak", "Vgorski Bijeli"],
-        "description": "High-quality vine from the Croatian island of Korčula making full-bodied whites.",
-        "color": "white",
+        "synonyms": [
+            "Pošip",
+            "Pošip Veliki",
+            "Pošipak",
+            "Vgorski Bijeli"
+        ],
+        "description": {
+            "default": "High-quality vine from the Croatian island of Korčula making full-bodied whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Potamissi",
         "synonyms": [
             "Aspropotamisio",
             "Aspropotamissi",
             "Potamisi",
             "Potamisiès",
             "Potamisio",
             "Potamisio Lefko",
-            "Potamissio Lefko",
+            "Potamissio Lefko"
         ],
-        "description": "Minor Greek island white hidden mainly in blends.",
-        "color": "white",
+        "description": {
+            "default": "Minor Greek island white hidden mainly in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Poulsard",
         "synonyms": [
             "Mècle",
             "Pelossard",
             "Peloussard",
             "Plant d’Arbois",
             "Pleusart",
             "Ploussard",
             "Plussart",
             "Poulsard Noir",
             "Pulceau",
-            "Pulsard",
+            "Pulsard"
         ],
-        "description": "Ancient, perfumed Jura speciality.",
-        "color": "black",
+        "description": {
+            "default": "Ancient, perfumed Jura speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Prairie Star",
-        "synonyms": ["ES 3-24-7"],
-        "description": "Cold-hardy American hybrid producing neutral, full whites for blending.",
-        "color": "white",
+        "synonyms": [
+            "ES 3-24-7"
+        ],
+        "description": {
+            "default": "Cold-hardy American hybrid producing neutral, full whites for blending.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Prč",
-        "synonyms": ["Čimavica", "Parč", "Prč Bijeli"],
-        "description": "Unusually scented Croatian variety being recuperated on the island of Hvar.",
-        "color": "white",
+        "synonyms": [
+            "Čimavica",
+            "Parč",
+            "Prč Bijeli"
+        ],
+        "description": {
+            "default": "Unusually scented Croatian variety being recuperated on the island of Hvar.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Précoce De Malingre",
         "synonyms": [
             "Blanc Précoce de Malingre",
             "Early Malingre",
             "Madeleine Blanche de Malingre",
             "Malinger",
-            "Malingre Précoce",
+            "Malingre Précoce"
         ],
-        "description": "Obscure Parisian cross still found in one old vineyard in the Ahr in Germany.",
-        "color": "white",
+        "description": {
+            "default": "Obscure Parisian cross still found in one old vineyard in the Ahr in Germany.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Prensal",
         "synonyms": [
             "Moll",
             "Pensal Blanca",
             "Premsal",
             "Premsal Blanca",
-            "Prensal Blanc",
+            "Prensal Blanc"
         ],
-        "description": "Robust Mallorcan speciality.",
-        "color": "white",
+        "description": {
+            "default": "Robust Mallorcan speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Preto Martinho",
-        "synonyms": ["Amostrinha", "Preto Martinho do Oeste"],
-        "description": "Portuguese variety often confused with Trincadeira.",
-        "color": "black",
+        "synonyms": [
+            "Amostrinha",
+            "Preto Martinho do Oeste"
+        ],
+        "description": {
+            "default": "Portuguese variety often confused with Trincadeira.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Prié",
         "synonyms": [
             "Bernarde",
             "Blanc de Morgex",
             "Blanc du Valdigne",
             "Legiruela",
             "Plant de la Salle",
-            "Prié Blanc",
+            "Prié Blanc"
         ],
-        "description": "Hugely significant Aostan variety with links to Spain and Switzerland.",
-        "color": "white",
+        "description": {
+            "default": "Hugely significant Aostan variety with links to Spain and Switzerland.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Prieto Picudo",
-        "synonyms": ["Prieto Picudo Oval", "Prieto Picudo Tinto"],
-        "description": "Crisp, perfumed speciality of León, north-west Spain.",
-        "color": "black",
+        "synonyms": [
+            "Prieto Picudo Oval",
+            "Prieto Picudo Tinto"
+        ],
+        "description": {
+            "default": "Crisp, perfumed speciality of León, north-west Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Priknadi",
         "synonyms": [
             "Prekiadi",
             "Prekna",
             "Preknadi",
             "Preknari",
             "Preknari Lefko",
             "Prekniariko",
-            "Prekno",
+            "Prekno"
         ],
-        "description": "Rare, and puzzling, variety from eastern Makedonía.",
-        "color": "white",
+        "description": {
+            "default": "Rare, and puzzling, variety from eastern Makedonía.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Primetta",
-        "synonyms": ["Neblou", "Premetta", "Prëmetta", "Prié Rouge", "Prometta"],
-        "description": "Recuperated Aostan pink wine speciality.",
-        "color": "pink",
+        "synonyms": [
+            "Neblou",
+            "Premetta",
+            "Prëmetta",
+            "Prié Rouge",
+            "Prometta"
+        ],
+        "description": {
+            "default": "Recuperated Aostan pink wine speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Prinzipal",
-        "synonyms": ["Geisenheim 7116-26"],
-        "description": "Recent disease-resistant German hybrid with marked Riesling influence.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 7116-26"
+        ],
+        "description": {
+            "default": "Recent disease-resistant German hybrid with marked Riesling influence.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Prior",
-        "synonyms": ["Freiburg 484-87 R"],
-        "description": "German hybrid bred for disease resistance.",
-        "color": "black",
+        "synonyms": [
+            "Freiburg 484-87 R"
+        ],
+        "description": {
+            "default": "German hybrid bred for disease resistance.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Prodest",
-        "synonyms": ["Incrocio Cosmo 109"],
-        "description": "Conegliano cross; attempt at fresher Merlot.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Cosmo 109"
+        ],
+        "description": {
+            "default": "Conegliano cross; attempt at fresher Merlot.",
+            "julie": "Second most planted wine grape in the world, Merlot produces wines that range from inexpensive to super premium in the region of Pomerol. Its profile is highly influence by the winemaking techniques used to vinify it. Its plumpness and smoothness make it a great ally to other grapes such as Cabernet Sauvignon to which it is often blended with. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Prokupac",
         "synonyms": [
             "Kameničarka",
             "Kamenilarka",
             "Majski Čornii",
             "Nikodimka",
             "Niševka",
             "Prokupec",
             "Prokupka",
             "Rskavac",
             "Skopsko Crno",
-            "Zarčin",
+            "Zarčin"
         ],
-        "description": "Balkan variety making early-drinking reds and deeply coloured rosé.",
-        "color": "black",
+        "description": {
+            "default": "Balkan variety making early-drinking reds and deeply coloured rosé.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Prosecco",
         "synonyms": [
             "Briška Glera",
             "Glera",
             "Prosecco Tondo",
             "Serpina",
             "Serprina",
             "Serprino",
             "Števerjana",
-            "Teran Bijeli",
+            "Teran Bijeli"
         ],
-        "description": "The dominant, rather neutral grape for Prosecco sparkling wine, probably Istrian. Misleadingly renamed Glera for commercially protective reasons.",
-        "color": "white",
+        "description": {
+            "default": "The dominant, rather neutral grape for Prosecco sparkling wine, probably Istrian. Misleadingly renamed Glera for commercially protective reasons.",
+            "julie": "Glera, also known as Prosecco, is one of the most planted varieties in the region of Veneto in Northern Italy. It is mostly cultivated for the production of Prosecco sparkling wines. The grapes translates into simple wines which are light and floral with nuances of pear and lemon. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Prosecco Lungo",
-        "synonyms": ["Glera", "Ribolla Spizade", "Tocai Nostrano"],
-        "description": "The spicier, less common Prosecco grape.",
-        "color": "white",
+        "synonyms": [
+            "Glera Lungo",
+            "Ribolla Spizade",
+            "Tocai Nostrano"
+        ],
+        "description": {
+            "default": "The spicier, less common Prosecco grape.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Prunelard",
-        "synonyms": ["Prunelart"],
-        "description": "Old, rare, recently rescued, south-west French variety, parent of Cot (Malbec).",
-        "color": "black",
+        "synonyms": [
+            "Prunelart"
+        ],
+        "description": {
+            "default": "Old, rare, recently rescued, south-west French variety, parent of Cot (Malbec).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Prunesta",
-        "synonyms": ["Prunesta Nera"],
-        "description": "Minor Calabrian used mainly in blends.",
-        "color": "black",
+        "synonyms": [
+            "Prunesta Nera"
+        ],
+        "description": {
+            "default": "Minor Calabrian used mainly in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Pukhliakovsky",
         "synonyms": [
             "Coarna Alba",
             "Kecskecsecsu",
             "Korna Belaja",
             "Majorka Belaja",
-            "Puchljakovski",
+            "Puchljakovski"
         ],
-        "description": "Russian variety with erratic yields producing light wines.",
-        "color": "white",
+        "description": {
+            "default": "Russian variety with erratic yields producing light wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Pules",
-        "synonyms": ["Pulës", "Puls"],
-        "description": "Minor Albanian white.",
-        "color": "white",
+        "synonyms": [
+            "Pulës",
+            "Puls"
+        ],
+        "description": {
+            "default": "Minor Albanian white.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rabigato",
         "synonyms": [
             "Baldsena",
             "Carrega Besta",
             "Estreito",
             "Muscatel Bravo",
             "Não Há",
             "Puesta en Cruz",
             "Rabigato Respigueiro",
             "Rabo de Asno",
             "Rabo de Carneiro",
             "Rabo de Gato",
-            "Rodrigo Affonso",
+            "Rodrigo Affonso"
         ],
-        "description": "Potentially high-quality, high-acid Douro variety.",
-        "color": "white",
+        "description": {
+            "default": "Potentially high-quality, high-acid Douro variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rabo De Ovelha",
-        "synonyms": ["Fernan Piriz", "Rabo de Ovella"],
-        "description": "Undemonstrative Portuguese variety making whites for early drinking.",
-        "color": "white",
+        "synonyms": [
+            "Fernan Piriz",
+            "Rabo de Ovella"
+        ],
+        "description": {
+            "default": "Undemonstrative Portuguese variety making whites for early drinking.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Raboso Piave",
         "synonyms": [
             "Friulara di Bagnoli",
             "Friularo",
             "Raboso del Piave",
-            "Raboso Nostrano",
+            "Raboso Nostrano"
         ],
-        "description": "Often tough Veneto variety needing careful handling and long ageing to produce high-quality wine. Parent of Raboso Veronese.",
-        "color": "black",
+        "description": {
+            "default": "Often tough Veneto variety needing careful handling and long ageing to produce high-quality wine. Parent of Raboso Veronese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Raboso Veronese",
-        "synonyms": ["Rabosa", "Raboso di Verona", "Raboso Friularo"],
-        "description": "Makes tannic Veneto red, often used for sparkling wines, and often confused with its parent, the more common Raboso Piave.",
-        "color": "black",
+        "synonyms": [
+            "Rabosa",
+            "Raboso di Verona",
+            "Raboso Friularo"
+        ],
+        "description": {
+            "default": "Makes tannic Veneto red, often used for sparkling wines, and often confused with its parent, the more common Raboso Piave.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Radisson",
-        "synonyms": ["ES 5-17"],
-        "description": "Another dark-skinned American hybrid that has found its way to Québec, although its exact identity is unclear.",
-        "color": "black",
+        "synonyms": [
+            "ES 5-17"
+        ],
+        "description": {
+            "default": "Another dark-skinned American hybrid that has found its way to Québec, although its exact identity is unclear.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Raffiat De Moncade",
-        "synonyms": ["Arréfiat", "Arrufiat", "Raffiat", "Refiat", "Ruffiac"],
-        "description": "Rare south-west French vine often confused with Arrufiac.",
-        "color": "white",
+        "synonyms": [
+            "Arréfiat",
+            "Arrufiat",
+            "Raffiat",
+            "Refiat",
+            "Ruffiac"
+        ],
+        "description": {
+            "default": "Rare south-west French vine often confused with Arrufiac.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ramisco",
-        "synonyms": ["Rasmisco nos Açores"],
-        "description": "Demanding and endangered Portuguese variety that produces wines aggressive in youth but elegant after considerable time in bottle.",
-        "color": "black",
+        "synonyms": [
+            "Rasmisco nos Açores"
+        ],
+        "description": {
+            "default": "Demanding and endangered Portuguese variety that produces wines aggressive in youth but elegant after considerable time in bottle.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ranac Bijeli",
-        "synonyms": ["Ranac Silbijanski Bijeli", "Silbijanac Bijeli"],
-        "description": "Almost extinct, intensely flavoured Croatian island variety.",
-        "color": "white",
+        "synonyms": [
+            "Ranac Silbijanski Bijeli",
+            "Silbijanac Bijeli"
+        ],
+        "description": {
+            "default": "Almost extinct, intensely flavoured Croatian island variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ranfol",
         "synonyms": [
             "Belina Pleterje",
             "Plavis",
             "Praskava Belina",
             "Ranfol Beli",
             "Ranfol Bijeli",
             "Sremska Lipovina",
             "Štajerska Belina",
             "Urbanka",
-            "Vrbanka",
+            "Vrbanka"
         ],
-        "description": "Variety with Slovenian origins making humdrum whites there and in Croatia.",
-        "color": "white",
+        "description": {
+            "default": "Variety with Slovenian origins making humdrum whites there and in Croatia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ranna Melnishka Loza",
-        "synonyms": ["Early Melnik", "Melnik 55", "Melnishka Ranna", "Ranna Melnishka"],
-        "description": "Bulgarian cross with good potential but lacking recognition.",
-        "color": "black",
+        "synonyms": [
+            "Early Melnik",
+            "Melnik 55",
+            "Melnishka Ranna",
+            "Ranna Melnishka"
+        ],
+        "description": {
+            "default": "Bulgarian cross with good potential but lacking recognition.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rastajola",
-        "synonyms": ["Durera", "Restajola"],
-        "description": "Minor variety from northern Piemonte encountered in blends.",
-        "color": "black",
+        "synonyms": [
+            "Durera",
+            "Restajola"
+        ],
+        "description": {
+            "default": "Minor variety from northern Piemonte encountered in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ráthay",
-        "synonyms": ["Klosterneuburg 1355-3-33", "Ráthay Noir"],
-        "description": "Rare, disease-resistant Austrian hybrid making wines for early drinking.",
-        "color": "black",
+        "synonyms": [
+            "Klosterneuburg 1355-3-33",
+            "Ráthay Noir"
+        ],
+        "description": {
+            "default": "Rare, disease-resistant Austrian hybrid making wines for early drinking.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Räuschling",
         "synonyms": [
             "Dretsch",
             "Drutsch",
             "Drutscht",
@@ -8926,90 +14122,166 @@
             "Klöpfer",
             "Offenburger",
             "Räuschling Weiss",
             "Reuschling",
             "Ruchelin",
             "Weisser Räuschling",
             "Zürirebe",
-            "Züriwiss",
+            "Züriwiss"
         ],
-        "description": "Historic, rare German variety experiencing a small revival in Switzerland.",
-        "color": "white",
+        "description": {
+            "default": "Historic, rare German variety experiencing a small revival in Switzerland.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ravat Blanc",
-        "synonyms": ["Rava 6", "Ravat 6", "Ravat Chardonnay 6", "Ravat Chardonnay B"],
-        "description": "Mediocre light-skinned Mâconnais hybrid on its way out.",
-        "color": "white",
+        "synonyms": [
+            "Rava 6",
+            "Ravat 6",
+            "Ravat Chardonnay 6",
+            "Ravat Chardonnay B"
+        ],
+        "description": {
+            "default": "Mediocre light-skinned Mâconnais hybrid on its way out.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rayon D’Or",
         "synonyms": [
             "Feherek Kiralya",
             "Roi des Blancs",
             "Seibel 4986",
             "Zlatni Luc",
-            "Zokoy Loloutch",
+            "Zokoy Loloutch"
         ],
-        "description": "Minor but relatively successful French hybrid once popular in the Loire. Begat Seyval Blanc and Vidal.",
-        "color": "white",
+        "description": {
+            "default": "Minor but relatively successful French hybrid once popular in the Loire. Begat Seyval Blanc and Vidal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Reberger",
-        "synonyms": ["Geilweilerhof 86-2-60"],
-        "description": "Recent, disease-resistant German hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Geilweilerhof 86-2-60"
+        ],
+        "description": {
+            "default": "Recent, disease-resistant German hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rebo",
-        "synonyms": ["Incrocio Rigotti 107-3"],
-        "description": "Rather promising red cross made in Trentino.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Rigotti 107-3"
+        ],
+        "description": {
+            "default": "Rather promising red cross made in Trentino.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Refosco",
-        "synonyms": ["Refoschin", "Refošk", "Rifòsc", "Rifosco"],
-        "description": "REFOSCO",
-        "color": "black",
+        "synonyms": [
+            "Refoschin",
+            "Refošk",
+            "Rifòsc",
+            "Rifosco"
+        ],
+        "description": {
+            "default": "REFOSCO",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Refosco Dal Peduncolo Rosso",
-        "synonyms": ["Rifòsc dal Pecòl Ròss"],
-        "description": "Most widely planted Refosco with complex family history making tart but potentially interesting reds in Friuli and Slovenia.",
-        "color": "black",
+        "synonyms": [
+            "Rifòsc dal Pecòl Ròss"
+        ],
+        "description": {
+            "default": "Most widely planted Refosco with complex family history making tart but potentially interesting reds in Friuli and Slovenia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Refosco Di Faedis",
-        "synonyms": ["Refosco di Ronchis", "Refosco Nostrano", "Refoscone"],
-        "description": "A relatively minor but perfumed Friuli Refosco enthusiastically supported by a local growers’ association.",
-        "color": "black",
+        "synonyms": [
+            "Refosco di Ronchis",
+            "Refosco Nostrano",
+            "Refoscone"
+        ],
+        "description": {
+            "default": "A relatively minor but perfumed Friuli Refosco enthusiastically supported by a local growers’ association.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Regent",
-        "synonyms": ["Geilweilerhof 67-198-3"],
-        "description": "Highly successful and increasingly popular German hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Geilweilerhof 67-198-3"
+        ],
+        "description": {
+            "default": "Highly successful and increasingly popular German hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Regner",
-        "synonyms": ["Alzey 10378"],
-        "description": "Declining, light-skinned German cross with little to recommend it.",
-        "color": "white",
+        "synonyms": [
+            "Alzey 10378"
+        ],
+        "description": {
+            "default": "Declining, light-skinned German cross with little to recommend it.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Reichensteiner",
-        "synonyms": ["Geisenheim 18-92"],
-        "description": "Cool-climate, productive, relatively soft German cross of pan-European descent.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 18-92"
+        ],
+        "description": {
+            "default": "Cool-climate, productive, relatively soft German cross of pan-European descent.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Réselle",
-        "synonyms": ["VB 86-3"],
-        "description": "Very minor disease-resistant Swiss hybrid.",
-        "color": "white",
+        "synonyms": [
+            "VB 86-3"
+        ],
+        "description": {
+            "default": "Very minor disease-resistant Swiss hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Retagliado Bianco",
         "synonyms": [
             "Arba Luxi",
             "Arretallau",
             "Arrotelas",
@@ -9018,49 +14290,79 @@
             "Coa de Brebèi",
             "Erbaluxi",
             "Mara Bianca",
             "Rechiliau",
             "Redaglàdu",
             "Retagladu",
             "Retellau",
-            "Ritelau",
+            "Ritelau"
         ],
-        "description": "Rare Sardinian with almost more synonyms than vines.",
-        "color": "white",
+        "description": {
+            "default": "Rare Sardinian with almost more synonyms than vines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rèze",
-        "synonyms": ["Blanc de Maurienne", "Resi", "Rèze Jaune", "Rèze Verte"],
-        "description": "Rare, very old, well-connected Swiss variety worthy of greater attention.",
-        "color": "white",
+        "synonyms": [
+            "Blanc de Maurienne",
+            "Resi",
+            "Rèze Jaune",
+            "Rèze Verte"
+        ],
+        "description": {
+            "default": "Rare, very old, well-connected Swiss variety worthy of greater attention.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ribolla Gialla",
         "synonyms": [
             "Rabola",
             "Rabiola",
             "Rebolla",
             "Rebula",
             "Ribolla di Rosazzo",
-            "Ribuèle",
+            "Ribuèle"
         ],
-        "description": "Ancient white from the Italy–Slovenia border.",
-        "color": "white",
+        "description": {
+            "default": "Ancient white from the Italy–Slovenia border.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Riesel",
-        "synonyms": ["VB 11-11-89-12"],
-        "description": "Minor Swiss hybrid bred mainly for its disease resistance that has found a home in the Netherlands.",
-        "color": "white",
+        "synonyms": [
+            "VB 11-11-89-12"
+        ],
+        "description": {
+            "default": "Minor Swiss hybrid bred mainly for its disease resistance that has found a home in the Netherlands.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rieslaner",
-        "synonyms": ["Mainriesling", "Würzburg N 1-11-17"],
-        "description": "Rare, undervalued but demanding Riesling-like German cross making stunning botrytis-influenced sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Mainriesling",
+            "Würzburg N 1-11-17"
+        ],
+        "description": {
+            "default": "Rare, undervalued but demanding Riesling-like German cross making stunning botrytis-influenced sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Riesling",
         "synonyms": [
             "Beyaz Riesling",
             "Johannisberg",
             "Kleinriesling",
@@ -9081,42 +14383,78 @@
             "Riesling Weisser",
             "Rislinoc",
             "Risling",
             "Rizling Rajnski",
             "Ryzlink Rýnský",
             "Starovetski",
             "Weisser Riesling",
-            "White Riesling",
+            "White Riesling"
         ],
-        "description": "One of the world’s greatest white wine grapes, capable of making particularly geographically expressive and long-lived wines at all sweetness levels.",
-        "color": "white",
+        "description": {
+            "default": "One of the world’s greatest white wine grapes, capable of making particularly geographically expressive and long-lived wines at all sweetness levels.",
+            "julie": "Riesling is an ancient grape variety originally from Germany where it is still producing world class wines today. Riesling expresses terroir like very few other grape varieties and for this reason it can be floral, fruity, spicy and/or mineral. Style range from bone dry to very sweet but its laser like natural acidity always keep wines in balance. Today, the variety thrives in many regions outside of Germany including Austria, Alsace in France, Central Europe, Washington state, New Zealand and some parts of Australia. ",
+            "sommelier": "While Riesling is incredibly versatile, you can expect German Riesling to be a light to medium bodied white wine with pronounced acidity, lower alcohol, and flavors and aromas of citrus, orchard, or stone fruits. Germany is where late-ripening Riesling best exhibits its trademark acidity and unique minerality, which add balance and complexity to its fruity tones and make it utterly mouthwatering. Color: Greenish yellow to light golden yellow. Aroma: Reminiscent of apple, peach, apricot. Taste: Delicately fruity, marked acidity. Body: Light to medium-bodied. Style: Dry to off-dry to sweet, still and sparkling."
+        },
+        "color": "white"
     },
     {
         "name": "Riesus",
-        "synonyms": ["Risus", "Risys", "Rysus"],
-        "description": "Recent and relatively robust Ukrainian hybrid with Riesling-like aromas.",
-        "color": "",
+        "synonyms": [
+            "Risus",
+            "Risys",
+            "Rysus"
+        ],
+        "description": {
+            "default": "Recent and relatively robust Ukrainian hybrid with Riesling-like aromas.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": ""
     },
     {
         "name": "Rimava",
-        "synonyms": ["CAAB 3/12"],
-        "description": "Recently authorized, promising Slovakian cross.",
-        "color": "black",
+        "synonyms": [
+            "CAAB 3/12"
+        ],
+        "description": {
+            "default": "Recently authorized, promising Slovakian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ripolo",
-        "synonyms": ["Ripala", "Ripoli", "Uva Ripola"],
-        "description": "Makes ageworthy whites on the Amalfi coast in southern Italy.",
-        "color": "white",
+        "synonyms": [
+            "Ripala",
+            "Ripoli",
+            "Uva Ripola"
+        ],
+        "description": {
+            "default": "Makes ageworthy whites on the Amalfi coast in southern Italy.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ritino",
-        "synonyms": ["Aretino", "Reteno", "Retina", "Retino", "Ripno"],
-        "description": "Very minor Greek variety used in local blends.",
-        "color": "black",
+        "synonyms": [
+            "Aretino",
+            "Reteno",
+            "Retina",
+            "Retino",
+            "Ripno"
+        ],
+        "description": {
+            "default": "Very minor Greek variety used in local blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rivairenc",
         "synonyms": [
             "Aspiran",
             "Aspiran Noir",
             "Épiran",
@@ -9128,32 +14466,40 @@
             "Ribeyrenc",
             "Riverain",
             "Riveirenc Noir",
             "Riveyrenc",
             "Riveyrene",
             "Spiran",
             "Verdai",
-            "Verdal",
+            "Verdal"
         ],
-        "description": "Ancient, once widespread, nearly extinct southern French vine. Better known as Aspiran Noir.",
-        "color": "black",
+        "description": {
+            "default": "Ancient, once widespread, nearly extinct southern French vine. Better known as Aspiran Noir.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rkatsiteli",
         "synonyms": [
             "Baiyu",
             "Corolioc",
             "Dedali Rcatiteli",
             "Mamali Rcatiteli",
             "Rkatiteli",
             "Rkatziteli",
-            "Topolioc",
+            "Topolioc"
         ],
-        "description": "Extremely useful, versatile, widely planted, originally Georgian variety.",
-        "color": "white",
+        "description": {
+            "default": "Extremely useful, versatile, widely planted, originally Georgian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Robola",
         "synonyms": [
             "Asporombola",
             "Asprorobola",
             "Asprorompola",
@@ -9161,18 +14507,22 @@
             "Robola Aspri",
             "Robola Aspro",
             "Robola Kerini",
             "Robolla",
             "Rombola",
             "Rombola Aspri",
             "Rompola",
-            "Rompola Kerine",
+            "Rompola Kerine"
         ],
-        "description": "High-quality Greek island white producing elegant, sometimes powerful, dry lemony wines.",
-        "color": "white",
+        "description": {
+            "default": "High-quality Greek island white producing elegant, sometimes powerful, dry lemony wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Roditis",
         "synonyms": [
             "Alepou Roditis",
             "Arilogos Roditis",
             "Arsenikos Roditis",
@@ -9194,326 +14544,628 @@
             "Rogditis",
             "Roidites",
             "Roiditis",
             "Roïdo",
             "Roigditis",
             "Sourviotes",
             "Sourviotis",
-            "Thilikos Roditis",
+            "Thilikos Roditis"
         ],
-        "description": "Very widely planted Greek variety with many clonal variations and generally low ambitions.",
-        "color": "pink",
+        "description": {
+            "default": "Very widely planted Greek variety with many clonal variations and generally low ambitions.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Rollo",
         "synonyms": [
             "Bruciapagliaio",
             "Capello",
             "Livornese Bianca",
             "Occhiana",
             "Pagadebiti",
-            "Rollo Genovese",
+            "Rollo Genovese"
         ],
-        "description": "Rare, old Ligurian (possibly Tuscan?) with a confusing array of synonyms.",
-        "color": "white",
+        "description": {
+            "default": "Rare, old Ligurian (possibly Tuscan?) with a confusing array of synonyms.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Romé",
-        "synonyms": ["Romé de Motril", "Romé Negro"],
-        "description": "Rare local Málaga speciality, possibly better at rosés than reds.",
-        "color": "black",
+        "synonyms": [
+            "Romé de Motril",
+            "Romé Negro"
+        ],
+        "description": {
+            "default": "Rare local Málaga speciality, possibly better at rosés than reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Romeiko",
-        "synonyms": ["Loïssima", "Romeico", "Romeiko Mavro", "Tsardana"],
-        "description": "Greek island variety that has been important on Kríti (Crete).",
-        "color": "black",
+        "synonyms": [
+            "Loïssima",
+            "Romeico",
+            "Romeiko Mavro",
+            "Tsardana"
+        ],
+        "description": {
+            "default": "Greek island variety that has been important on Kríti (Crete).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Romero De Híjar",
-        "synonyms": ["Romero"],
-        "description": "Potentially interesting but very rare Aragonese speciality.",
-        "color": "black",
+        "synonyms": [
+            "Romero"
+        ],
+        "description": {
+            "default": "Potentially interesting but very rare Aragonese speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Romorantin",
         "synonyms": [
             "Bury",
             "Dameret Blanc",
             "Damery",
             "Dannery",
             "Dannezy",
             "Maclon",
-            "Petit Dannezy",
+            "Petit Dannezy"
         ],
-        "description": "Minor and difficult to ripen Burgundian variety now exclusive to Cour-Cheverny in the Loire.",
-        "color": "white",
+        "description": {
+            "default": "Minor and difficult to ripen Burgundian variety now exclusive to Cour-Cheverny in the Loire.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rondo",
-        "synonyms": ["Geisenheim 6494-5"],
-        "description": "German red-fleshed hybrid with a complicated genealogy well suited to cool climes makes light, fruity reds.",
-        "color": "black",
+        "synonyms": [
+            "Geisenheim 6494-5"
+        ],
+        "description": {
+            "default": "German red-fleshed hybrid with a complicated genealogy well suited to cool climes makes light, fruity reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rosé Du Var",
-        "synonyms": ["Barbaroux", "Grec Rose", "Roussanne du Var"],
-        "description": "Dull and understandably declining pink-skinned Provençal variety.",
-        "color": "pink",
+        "synonyms": [
+            "Barbaroux",
+            "Grec Rose",
+            "Roussanne du Var"
+        ],
+        "description": {
+            "default": "Dull and understandably declining pink-skinned Provençal variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Rose Honey",
-        # "synonyms": ["Honey", "Red"],
-        "description": "As yet unidentified minor variety found in China’s Yunnan province.",
-        "color": "pink",
+        "description": {
+            "default": "As yet unidentified minor variety found in China’s Yunnan province.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Rosetta",
-        "synonyms": ["Freiburg 991-60"],
-        "description": "Red-skinned German hybrid used mainly for the table.",
-        "color": "red",
+        "synonyms": [
+            "Freiburg 991-60"
+        ],
+        "description": {
+            "default": "Red-skinned German hybrid used mainly for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Rosette",
-        "synonyms": ["Francuz Seibel", "Seibel 1000"],
-        "description": "Ardèche hybrid still planted in New York State.",
-        "color": "black",
+        "synonyms": [
+            "Francuz Seibel",
+            "Seibel 1000"
+        ],
+        "description": {
+            "default": "Ardèche hybrid still planted in New York State.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rossara Trentina",
-        "synonyms": ["Geschlafene", "Ross Ciàr", "Rossar", "Rossera", "Varenzasca"],
-        "description": "Trentino interrelated rarity.",
-        "color": "red",
+        "synonyms": [
+            "Geschlafene",
+            "Ross Ciàr",
+            "Rossar",
+            "Rossera",
+            "Varenzasca"
+        ],
+        "description": {
+            "default": "Trentino interrelated rarity.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Rossetto",
-        "synonyms": ["Greco di Velletri", "Greco Giallo", "Greco Verde", "Roscetto"],
-        "description": "Rare Lazio vine only recently showing its potential for quality.",
-        "color": "white",
+        "synonyms": [
+            "Greco di Velletri",
+            "Greco Giallo",
+            "Greco Verde",
+            "Roscetto"
+        ],
+        "description": {
+            "default": "Rare Lazio vine only recently showing its potential for quality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Rossignola",
-        "synonyms": ["Rossetta", "Rossetta di Montagna", "Rossola"],
-        "description": "Minor and rather tart variety used to a limited extent in Veneto blends.",
-        "color": "black",
+        "synonyms": [
+            "Rossetta",
+            "Rossetta di Montagna",
+            "Rossola"
+        ],
+        "description": {
+            "default": "Minor and rather tart variety used to a limited extent in Veneto blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rossola Nera",
-        "synonyms": ["Rossera", "Rossola", "Rossolo"],
-        "description": "Minor, high-acid Valtellina vine.",
-        "color": "red",
+        "synonyms": [
+            "Rossera",
+            "Rossola",
+            "Rossolo"
+        ],
+        "description": {
+            "default": "Minor, high-acid Valtellina vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Rossolino Nero",
-        "synonyms": ["Rossolino Rosa"],
-        "description": "Minor variety in Valtellina in Italy’s cool far north, probably progeny of Rossola Nera.",
-        "color": "black",
+        "synonyms": [
+            "Rossolino Rosa"
+        ],
+        "description": {
+            "default": "Minor variety in Valtellina in Italy’s cool far north, probably progeny of Rossola Nera.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rotberger",
-        "synonyms": ["Geisenheim 3-37", "Redberger"],
-        "description": "German cross that takes after its parent Schiava Grossa (aka Trollinger).",
-        "color": "black",
+        "synonyms": [
+            "Geisenheim 3-37",
+            "Redberger"
+        ],
+        "description": {
+            "default": "German cross that takes after its parent Schiava Grossa (aka Trollinger).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Roter Veltliner",
         "synonyms": [
             "Piros Veltelini",
             "Rote Fleischtraube",
             "Roter Veltliner Baldig",
             "Rotmuskateller",
             "Rotreifler",
             "Ryvola Cervena",
-            "Veltlínske Červené",
+            "Veltlínske Červené"
         ],
-        "description": "Ancient Austrian variety that makes powerful white wine, whatever its name suggests.",
-        "color": "pink",
+        "description": {
+            "default": "Ancient Austrian variety that makes powerful white wine, whatever its name suggests.",
+            "julie": "",
+            "sommelier": "The indigenous Roter Veltliner plays a vital role within the Veltliner Family, and is the parent variety of Neuburger, Zierfandler and Rotgipfler. The Roter Veltliner is predominantly in Wagram (Lower Austria). Roter Veltliner is a high-yielding variety, which is why yield management is necessary to achieve high quality. Restricting the yield enables the production of very original, elegant, extract-rich wines with fine, spicy aromas and great ageing potential. Without yield management, the wines are somewhat thin and lacking in complexity."
+        },
+        "color": "pink"
     },
     {
         "name": "Rotgipfler",
-        "synonyms": ["Reifler", "Slatzki Zelenac", "Zelenac Slatki"],
-        "description": "Thermenregion speciality makes powerful whites usually blended with Zierfandler.",
-        "color": "white",
+        "synonyms": [
+            "Reifler",
+            "Slatzki Zelenac",
+            "Zelenac Slatki"
+        ],
+        "description": {
+            "default": "Thermenregion speciality makes powerful whites usually blended with Zierfandler.",
+            "julie": "",
+            "sommelier": "Rotgipfler is a crossing of Traminer and Roter Veltliner. Likewise with Zierfandler, Rotgipfler is a speciality found virtually only in the Thermenregion (Lower Austria). When the yield is sufficiently restricted, wines are characterised by a high extract content, pleasant acidity and a fine bouquet. Rotgipler tends to mature slowly and is mostly produced as a monovarietal wine, but is also blended with Zierfandler."
+        },
+        "color": "white"
     },
     {
         "name": "Rouge De Fully",
-        "synonyms": ["Durize"],
-        "description": "Swiss, or possibly Italian, variety making rustic reds.",
-        "color": "black",
+        "synonyms": [
+            "Durize"
+        ],
+        "description": {
+            "default": "Swiss, or possibly Italian, variety making rustic reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rouge Du Pays",
-        "synonyms": ["Cornalin", "Cornalin du Valais", "Landroter", "Rouge du Valais"],
-        "description": "Variety exclusive to southern Switzerland also known as Cornalin but distinct from the Italian Cornalin in the Valle d’Aosta.",
-        "color": "black",
+        "synonyms": [
+            "Cornalin",
+            "Cornalin du Valais",
+            "Landroter",
+            "Rouge du Valais"
+        ],
+        "description": {
+            "default": "Variety exclusive to southern Switzerland also known as Cornalin but distinct from the Italian Cornalin in the Valle d’Aosta.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Roussanne",
         "synonyms": [
             "Barbin",
             "Bergeron",
             "Fromental",
             "Fromenteau",
             "Martin Cot",
             "Petite Roussette",
-            "Roussanne Blanc",
+            "Roussanne Blanc"
         ],
-        "description": "Scented, high-quality Rhône white often blended with Marsanne. Not easy to grow.",
-        "color": "white",
+        "description": {
+            "default": "Scented, high-quality Rhône white often blended with Marsanne. Not easy to grow.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Roussette D’Ayze",
         "synonyms": [
             "Bonne Roussette d’Ayze",
             "Grosse Roussette",
             "Riusse",
-            "Riussette",
+            "Riussette"
         ],
-        "description": "Virtually extinct and rather inferior Savoie variety used occasionally in sparkling wines.",
-        "color": "white",
+        "description": {
+            "default": "Virtually extinct and rather inferior Savoie variety used occasionally in sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Roussin",
-        "synonyms": ["Gros Roussin", "Picciou Roussin", "Rossé"],
-        "description": "Almost extinct Aostan.",
-        "color": "black",
+        "synonyms": [
+            "Gros Roussin",
+            "Picciou Roussin",
+            "Rossé"
+        ],
+        "description": {
+            "default": "Almost extinct Aostan.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Royal De Alloza",
-        "synonyms": ["Alloza", "Derechero de Muniesa"],
-        "description": "Recuperated and very limited Aragonese speciality.",
-        "color": "black",
+        "synonyms": [
+            "Alloza",
+            "Derechero de Muniesa"
+        ],
+        "description": {
+            "default": "Recuperated and very limited Aragonese speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Royalty",
-        "synonyms": ["Calif 526", "California S 26", "Royalti", "Royalty 1390"],
-        "description": "Red-fleshed American hybrid on the wane in California.",
-        "color": "black",
+        "synonyms": [
+            "Calif 526",
+            "California S 26",
+            "Royalti",
+            "Royalty 1390"
+        ],
+        "description": {
+            "default": "Red-fleshed American hybrid on the wane in California.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rubin",
-        "synonyms": ["Rubin Bolgarskii"],
-        "description": "Intriguing, successful but not widely planted Bulgarian cross used for both dry and sweet reds.",
-        "color": "black",
+        "synonyms": [
+            "Rubin Bolgarskii"
+        ],
+        "description": {
+            "default": "Intriguing, successful but not widely planted Bulgarian cross used for both dry and sweet reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rubin Golodrigi",
-        "synonyms": ["Magarach 15-74-29", "Ruby of Golodryga"],
-        "description": "Recent and usefully disease-resistant Ukrainian hybrid producing deeply coloured reds.",
-        "color": "red",
+        "synonyms": [
+            "Magarach 15-74-29",
+            "Ruby of Golodryga"
+        ],
+        "description": {
+            "default": "Recent and usefully disease-resistant Ukrainian hybrid producing deeply coloured reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Rubinet",
-        "synonyms": ["R – 27", "Tintet"],
-        "description": "Very minor red-fleshed Czech cross producing usefully dark, rich wines.",
-        "color": "black",
+        "synonyms": [
+            "R – 27",
+            "Tintet"
+        ],
+        "description": {
+            "default": "Very minor red-fleshed Czech cross producing usefully dark, rich wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rubinovy Magaracha",
-        "synonyms": ["Crossing 56", "Magarach 56", "Magarach Ruby", "Ruby Magaracha"],
-        "description": "Robust but awkwardly late-ripening Ukrainian cross.",
-        "color": "black",
+        "synonyms": [
+            "Crossing 56",
+            "Magarach 56",
+            "Magarach Ruby",
+            "Ruby Magaracha"
+        ],
+        "description": {
+            "default": "Robust but awkwardly late-ripening Ukrainian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rubired",
-        "synonyms": ["California S 8", "Tintoria"],
-        "description": "Winemakers’ secret weapon. Productive, red-fleshed American hybrid valued for juice and for adding colour.",
-        "color": "black",
+        "synonyms": [
+            "California S 8",
+            "Tintoria"
+        ],
+        "description": {
+            "default": "Winemakers’ secret weapon. Productive, red-fleshed American hybrid valued for juice and for adding colour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ruby Cabernet",
-        "synonyms": ["California 234 F 2"],
-        "description": "Productive California cross with sweet-fruit flavours, generally used to bolster blends.",
-        "color": "black",
+        "synonyms": [
+            "California 234 F 2"
+        ],
+        "description": {
+            "default": "Productive California cross with sweet-fruit flavours, generally used to bolster blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ruchè",
-        "synonyms": ["Moscatellina", "Roché", "Romitagi", "Rouchet"],
-        "description": "Rare, perfumed red wine grape with its own Piemonte DOC.",
-        "color": "black",
+        "synonyms": [
+            "Moscatellina",
+            "Roché",
+            "Romitagi",
+            "Rouchet"
+        ],
+        "description": {
+            "default": "Rare, perfumed red wine grape with its own Piemonte DOC.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rudava",
-        "synonyms": ["CATAP 6/28"],
-        "description": "Recently authorized Slovakian cross with good potential for everyday reds.",
-        "color": "black",
+        "synonyms": [
+            "CATAP 6/28"
+        ],
+        "description": {
+            "default": "Recently authorized Slovakian cross with good potential for everyday reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Rufete",
         "synonyms": [
             "Castellana",
             "Penamacor",
             "Preto Rifete",
             "Rifete",
             "Rosette",
             "Rufeta",
-            "Tinta Pinheira",
+            "Tinta Pinheira"
         ],
-        "description": "Late-ripening Portuguese variety that can occasionally yield fine, ageworthy, light reds.",
-        "color": "black",
+        "description": {
+            "default": "Late-ripening Portuguese variety that can occasionally yield fine, ageworthy, light reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Ruggine",
-        "synonyms": ["Rugginosa", "Ruzninteina"],
-        "description": "Recuperated Emilia-Romagnan.",
-        "color": "white",
+        "synonyms": [
+            "Rugginosa",
+            "Ruzninteina"
+        ],
+        "description": {
+            "default": "Recuperated Emilia-Romagnan.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Ruzzese",
-        "synonyms": ["Rossese Bianco"],
-        "description": "Rare Ligurian rescued from extinction but so far authorized only for table wines.",
-        "color": "white",
+        "synonyms": [
+            "Rossese Bianco"
+        ],
+        "description": {
+            "default": "Rare Ligurian rescued from extinction but so far authorized only for table wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sabato",
-        "synonyms": ["Gigante"],
-        "description": "Minor Campanian vine associated with the Sorrento coast.",
-        "color": "black",
+        "synonyms": [
+            "Gigante"
+        ],
+        "description": {
+            "default": "Minor Campanian vine associated with the Sorrento coast.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sabrevois",
-        "synonyms": ["ES 2-1-9"],
-        "description": "Insubstantial US hybrid prospering in Québec.",
-        "color": "black",
+        "synonyms": [
+            "ES 2-1-9"
+        ],
+        "description": {
+            "default": "Insubstantial US hybrid prospering in Québec.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sacy",
-        "synonyms": ["Aligoté Vert", "Plant d’Essert", "Plant de Sacy", "Tressallier"],
-        "description": "Light, nether Bugundian, losing ground.",
-        "color": "white",
+        "synonyms": [
+            "Aligoté Vert",
+            "Plant d’Essert",
+            "Plant de Sacy",
+            "Tressallier"
+        ],
+        "description": {
+            "default": "Light, nether Bugundian, losing ground.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Saint-Macaire",
-        "synonyms": ["Bouton Blanc", "Moustère", "Moustouzère"],
-        "description": "Obscure Bordeaux variety found to a very limited extent in California and Australia.",
-        "color": "black",
+        "synonyms": [
+            "Bouton Blanc",
+            "Moustère",
+            "Moustouzère"
+        ],
+        "description": {
+            "default": "Obscure Bordeaux variety found to a very limited extent in California and Australia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Salvador",
-        "synonyms": ["Pate Noir", "Salvadore", "Seibel 128"],
-        "description": "Red-fleshed French hybrid now largely superseded by Rubired in California’s San Joaquin Valley.",
-        "color": "black",
+        "synonyms": [
+            "Pate Noir",
+            "Salvadore",
+            "Seibel 128"
+        ],
+        "description": {
+            "default": "Red-fleshed French hybrid now largely superseded by Rubired in California’s San Joaquin Valley.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "San Lunardo",
-        "synonyms": ["Bianca", "Don Lunardo", "Lunardo"],
-        "description": "Rare Ischian white wine variety.",
-        "color": "white",
+        "synonyms": [
+            "Bianca",
+            "Don Lunardo",
+            "Lunardo"
+        ],
+        "description": {
+            "default": "Rare Ischian white wine variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "San Martino",
-        "synonyms": ["Incrocio Dalmasso 7/21"],
-        "description": "Very minor cross made at Conegliano in the Veneto but apparently grown only in Piemonte.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso 7/21"
+        ],
+        "description": {
+            "default": "Very minor cross made at Conegliano in the Veneto but apparently grown only in Piemonte.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "San Michele",
-        "synonyms": ["Incrocio Dalmasso 15/34"],
-        "description": "Obscure Conegliano cross whose true parentage has only recently been revealed.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso 15/34"
+        ],
+        "description": {
+            "default": "Obscure Conegliano cross whose true parentage has only recently been revealed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sangiovese",
         "synonyms": [
             "Brunelletto",
             "Brunello",
             "Cacchiano",
@@ -9539,52 +15191,80 @@
             "Sangiovese Grosso",
             "Sangiovese Piccolo",
             "Sangioveto",
             "Tabernello",
             "Toustain",
             "Tuccanese",
             "Vigna del Conte",
-            "Vigna Maggio",
+            "Vigna Maggio"
         ],
-        "description": "Hugely important and wildly variable central Italian variety with many a name and surprising origins.",
-        "color": "black",
+        "description": {
+            "default": "Hugely important and wildly variable central Italian variety with many a name and surprising origins.",
+            "julie": "Sangiovese is the main red grape variety in Tuscany and the key player in the regions of Chianti, Vino Nobile di Montepulciano and many of the Supertuscans. It gives wines which are high in acidity and tannins and can be deliciously savoury and with great ageing potential. In Corsica, the grape is known as Nielluccio and is the most planted grape on the island. The variety is also increasingly growing in other parts of the world such as Australia. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sankt Laurent",
         "synonyms": [
             "Laurenzitraube",
             "Lorenztraube",
             "Saint Laurent",
             "Saint-Laurent",
             "Saint-Lorentz",
             "Schwarzer",
             "Svatovavřinecké",
             "Svätovavrinecké",
-            "Vavřinecké",
+            "Vavřinecké"
         ],
-        "description": "Middle European variety of uncertain origin producing velvety reds.",
-        "color": "black",
+        "description": {
+            "default": "Middle European variety of uncertain origin producing velvety reds.",
+            "julie": "",
+            "sommelier": "The high quality St. Laurent variety belongs to the Pinot family, and the synonym Pinot St. Laurent suggests a pinot seedling. In the course of a more quality orientated thinking in recent years, the variety has experienced a revival in all wine-producing regions. Sankt Laurent delivers dark, dense and fruity red wines with aromas of morello cherry. These wines are high quality and store well."
+        },
+        "color": "black"
     },
     {
         "name": "Saperavi",
-        "synonyms": ["Atenuri Saperavi", "Meskhuri Saperavi", "Obchuri Saperavi"],
-        "description": "Quintessential Georgian variety producing deeply coloured, firm, initially tart but ageworthy reds.",
-        "color": "black",
+        "synonyms": [
+            "Atenuri Saperavi",
+            "Meskhuri Saperavi",
+            "Obchuri Saperavi"
+        ],
+        "description": {
+            "default": "Quintessential Georgian variety producing deeply coloured, firm, initially tart but ageworthy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Saphira",
-        "synonyms": ["Geisenheim 7815-1"],
-        "description": "New German hybrid with moderate disease resistance making rather neutral whites.",
-        "color": "white",
+        "synonyms": [
+            "Geisenheim 7815-1"
+        ],
+        "description": {
+            "default": "New German hybrid with moderate disease resistance making rather neutral whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sary Pandas",
-        "synonyms": ["Sarah Pandas"],
-        "description": "Old Ukrainian variety planted mainly in the south of the country for dessert wines.",
-        "color": "white",
+        "synonyms": [
+            "Sarah Pandas"
+        ],
+        "description": {
+            "default": "Old Ukrainian variety planted mainly in the south of the country for dessert wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sauvignon Blanc",
         "synonyms": [
             "Blanc Fumé",
             "Blanc Fumet",
             "Fié",
@@ -9596,36 +15276,44 @@
             "Sauternes",
             "Sauvignon Fumé",
             "Sauvignon Musqué",
             "Sauvignon Blanc Musqué",
             "Savagnou",
             "Sotern Mărunt",
             "Surin",
-            "Verdo Belîi",
+            "Verdo Belîi"
         ],
-        "description": "Parent of Cabernet Sauvignon producing increasingly appreciated aromatic, zesty, crisp whites.",
-        "color": "white",
+        "description": {
+            "default": "Parent of Cabernet Sauvignon producing increasingly appreciated aromatic, zesty, crisp whites.",
+            "julie": "Possibly, the most recognisable grape varitety when made into wine. Sauvignon blanc, especially from New Zealand, can have intense aromas of exotic fruits, citrus and netlle. The grape is highly impacted by the climate it grows in - cool climate Sauvignon blanc tend to develop more herbaceous aromas than wines made in a more temperate climate. In France, Sauvignon blanc is is thriving in the Loire Valley where it is produced as a single grape variety in appellations such as Sancerre, Pouilly Fumé et Quincy. In this part of France, the grape tends to express a little less its varietal characters and a little more the terroir it is grown on - mostly marl, limestone and flint. In the region of Bordeaux and in Margaret Valley in Western Australia, Sauvignon blanc is generally blended with Sémillon. Sauvignon blanc is planted all over the wine world and has a hugh fan base. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sauvignonasse",
         "synonyms": [
             "Friulano",
             "Occhio di Gatto",
             "Sauvignon de la Corrèze",
             "Sauvignon Gros Grain",
             "Sauvignon Vert",
             "Tai Bianco",
             "Tocai",
             "Tocai Friulano",
             "Tocai Italico",
             "Tocai Italico Friulano",
-            "Zeleni Sauvignon",
+            "Zeleni Sauvignon"
         ],
-        "description": "Lightly aromatic variety now called Friulano in Italy and for long confused with Sauvignon Blanc in Chile.",
-        "color": "white",
+        "description": {
+            "default": "Lightly aromatic variety now called Friulano in Italy and for long confused with Sauvignon Blanc in Chile.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Savagnin Blanc",
         "synonyms": [
             "Brynšt",
             "Edler Weiss",
             "Weissedler",
@@ -9646,18 +15334,22 @@
             "Prynč",
             "Sauvagnin",
             "Savagnin Jaune",
             "Savagnin Vert",
             "Tramín Bílý",
             "Traminec",
             "Traminer",
-            "Weisser Traminer",
+            "Weisser Traminer"
         ],
-        "description": "Full-bodied, firm, ageworthy wines, sometimes called Traminer.",
-        "color": "",
+        "description": {
+            "default": "Full-bodied, firm, ageworthy wines, sometimes called Traminer.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": ""
     },
     {
         "name": "Savagnin Rose",
         "synonyms": [
             "Clevener",
             "Clevner",
             "Fromenteau Rouge",
@@ -9669,18 +15361,22 @@
             "Roter Traminer",
             "Rotfrenschen",
             "Savagnin Rose Non Musqué",
             "Savagnin Rouge",
             "Traminac Crveni",
             "Traminer Rot",
             "Traminer Rother",
-            "simply Traminer",
+            "simply Traminer"
         ],
-        "description": "The non-aromatic version of the much more famous Gewürztraminer.",
-        "color": "",
+        "description": {
+            "default": "The non-aromatic version of the much more famous Gewürztraminer.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": ""
     },
     {
         "name": "Gewürztraminer",
         "synonyms": [
             "Dišeči Traminec",
             "Gentil Aromatique",
             "Gentil Rose Aromatique",
@@ -9695,52 +15391,85 @@
             "Traminer Rose",
             "Traminer Rot",
             "Traminer Rother",
             "Traminer Roz",
             "Tramini",
             "Fűsyeres Tramini",
             "Piros Tramini",
+            "Gewurztraminer"
         ],
-        "description": "One of the most headily and distinctively aromatic varietals of all with strong lychee flavours and high alcohol levels.",
-        "color": "",
+        "description": {
+            "default": "One of the most headily and distinctively aromatic varietals of all with strong lychee flavours and high alcohol levels.",
+            "julie": "Highly aromatic pink grape varieties distcintive for its aromas and flavours of rose, litchi and spices. Gewürztraminer wines are full bodied, often high in alcohol and rarely bone dry. It is mostly planted in Alsace (France), in Alto Adige (Italy) and Germany as well as in New Wolrd countries.",
+            "sommelier": "The aromatic bouquet, complemented by a tart, spicy fruit flavour, makes Gewürztraminer a variety for lovers of aromatic wines. When matured dry to semi-dry, it goes well with game pâtés, poultry with aromatic sauces, snails and spicy-aromatic ragouts. Well matured and noble sweet, it is appreciated as an aperitif. Sweet Spätlesen and edelsüße Auslesen go very well with aromatic desserts prepared with marzipan, chocolate or brandies. The combination of Gewürztraminer and Munster cheese or high-fat blue cheese is particularly appreciated. Ordinary, but also highly refined wines can be produced from this very aromatic and spicy variety. Depending on the soil and yield, the wines are more elegant or heavier - sometimes with considerable alcohol content. What they all have in common is a relatively mild acidity. Depending on the quality level, typical Gewürztraminers have a straw-yellow to golden-yellow colour and exude a fragrance, sometimes subtle, sometimes lush, reminiscent of roses in bloom; sometimes one also finds the scent of acacia blossoms, violets, honey, marzipan, quince jelly, bitter oranges or passion fruit. Noble sweet selections are suitable for many years of storage. Aroma: fading roses, sultanas, quince"
+        },
+        "color": "white"
     },
     {
         "name": "Savatiano",
         "synonyms": [
             "Dobraina Aspri",
             "Doubraina Aspri",
             "Doumpraina Lefki",
             "Kountoura Aspri",
             "Perahoritiko",
             "Sakeiko",
             "Savathiano",
             "Savvatiano",
             "Stamatiano",
-            "Tsoumprena",
+            "Tsoumprena"
         ],
-        "description": "Greece’s most widely planted variety, used to make retsina but capable of a good deal more.",
-        "color": "white",
+        "description": {
+            "default": "Greece’s most widely planted variety, used to make retsina but capable of a good deal more.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Scheurebe",
-        "synonyms": ["Alzey S 88", "Dr Wagnerrebe", "Sämling 88", "Scheu 88"],
-        "description": "Underrated and declining early-twentieth-century German cross capable of producing intense, refreshing, dry and sweet wines.",
-        "color": "white",
+        "synonyms": [
+            "Alzey S 88",
+            "Dr Wagnerrebe",
+            "Sämling 88",
+            "Scheu 88"
+        ],
+        "description": {
+            "default": "Underrated and declining early-twentieth-century German cross capable of producing intense, refreshing, dry and sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Schiava Gentile",
-        "synonyms": ["Edelvernatsch", "Rothervernatsch"],
-        "description": "Small-berried vine making soft, fruity reds in the Alto Adige.",
-        "color": "black",
+        "synonyms": [
+            "Edelvernatsch",
+            "Rothervernatsch"
+        ],
+        "description": {
+            "default": "Small-berried vine making soft, fruity reds in the Alto Adige.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Schiava Grigia",
-        "synonyms": ["Cenerina", "Grauervernatsch", "Grauvernatsch"],
-        "description": "Particularly blueish-berried member of the Alto Adige’s Schiava group of varieties.",
-        "color": "black",
+        "synonyms": [
+            "Cenerina",
+            "Grauervernatsch",
+            "Grauvernatsch"
+        ],
+        "description": {
+            "default": "Particularly blueish-berried member of the Alto Adige’s Schiava group of varieties.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Schiava Grossa",
         "synonyms": [
             "Black Hamburg",
             "Black Hamburgh",
             "Blauer Trollinger",
@@ -9749,72 +15478,114 @@
             "Frankenthaler",
             "Grossvernatsch",
             "Kleinvernatsch",
             "Meraner Kurtraube",
             "Schiavone",
             "Trollinger",
             "Tschaggele",
-            "Uva Meranese",
+            "Uva Meranese"
         ],
-        "description": "The most common Schiava, from the Tirol. Well connected and more widely planted, as Trollinger, in Germany than in Italy. Also a table grape.",
-        "color": "black",
+        "description": {
+            "default": "The most common Schiava, from the Tirol. Well connected and more widely planted, as Trollinger, in Germany than in Italy. Also a table grape.",
+            "julie": "",
+            "sommelier": "The majority of Trollinger wines are light and fruity with a delicate scent reminiscent of strawberry or cherry. Usually light brick red to pale ruby red, Trollinger is meant to be enjoyed young, and can be used to produce Rosé. It is a classic, lighter, German drinking wine with a certain residual sweetness. The light wines do not need to be stored for several years, but are ready to drink the year after the harvest. Their fine floral aroma reveals a delicate muscat tone or a wild cherry flavour. The wines are usually a light red colour in the glass, in good years also ruby red. Trollinger is often enjoyed with a hearty snack, but also goes well with a piece of white meat or neutral cream cheese. Flavour: strawberries, currants, cherries."
+        },
+        "color": "black"
     },
     {
         "name": "Schiava Lombarda",
-        "synonyms": ["Schiava Nera"],
-        "description": "Lombardia’s Schiava produces soft, fruity red.",
-        "color": "black",
+        "synonyms": [
+            "Schiava Nera"
+        ],
+        "description": {
+            "default": "Lombardia’s Schiava produces soft, fruity red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Schioppettino",
-        "synonyms": ["Pocalza", "Poçalza", "Pokalca", "Pokalza", "Ribolla Nera"],
-        "description": "Perfumed and fruity Friulian rescued in the 1970s and now thriving.",
-        "color": "black",
+        "synonyms": [
+            "Pocalza",
+            "Poçalza",
+            "Pokalca",
+            "Pokalza",
+            "Ribolla Nera"
+        ],
+        "description": {
+            "default": "Perfumed and fruity Friulian rescued in the 1970s and now thriving.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Schönburger",
-        "synonyms": ["Geisenheim 15-114", "Schönberger", "Schönburger Rose"],
-        "description": "A pink-skinned German cross making white wines with light Muscat aromas, mainly in England.",
-        "color": "pink",
+        "synonyms": [
+            "Geisenheim 15-114",
+            "Schönberger",
+            "Schönburger Rose"
+        ],
+        "description": {
+            "default": "A pink-skinned German cross making white wines with light Muscat aromas, mainly in England.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Sciaglìn",
-        "synonyms": ["Scjaglìn"],
-        "description": "Ancient and rare Friulian.",
-        "color": "white",
+        "synonyms": [
+            "Scjaglìn"
+        ],
+        "description": {
+            "default": "Ancient and rare Friulian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sciascinoso",
         "synonyms": [
             "Crovina",
             "Livella di Battipaglia",
             "Livella Nera",
             "Olivella Nera",
             "Olivella Nostrana",
             "Sanginoso",
             "Uva Olivella",
             "Uva Olivella Verace",
-            "Vulivella",
+            "Vulivella"
         ],
-        "description": "Unusual Campanian making light reds.",
-        "color": "black",
+        "description": {
+            "default": "Unusual Campanian making light reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Scimiscià",
         "synonyms": [
             "Çimixâ",
             "Frate Pelato",
             "Genovese",
             "Genovèse",
             "Raisin Génois",
             "Rossala Bianca",
-            "Simixà",
+            "Simixà"
         ],
-        "description": "Old and very minor Genoese variety also found on the French island of Corse.",
-        "color": "white",
+        "description": {
+            "default": "Old and very minor Genoese variety also found on the French island of Corse.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Scuppernong",
         "synonyms": [
             "American Muscadine",
             "Big White Grape",
             "Bull",
@@ -9823,180 +15594,339 @@
             "Green Muscadine",
             "Green Scuppernong",
             "Hickman’s Grape",
             "Pedee",
             "Roanoke",
             "White Muscadine",
             "White Scuppernong",
-            "Yellow Muscadine",
+            "Yellow Muscadine"
         ],
-        "description": "Bronze-berried native American variety producing distinctive sweet wines said to have health benefits.",
-        "color": "grey",
+        "description": {
+            "default": "Bronze-berried native American variety producing distinctive sweet wines said to have health benefits.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey"
     },
     {
         "name": "Seara Nova",
-        "synonyms": ["H-8-51-29"],
-        "description": "Cross quite widely planted in western Portugal and on the Açores.",
-        "color": "white",
+        "synonyms": [
+            "H-8-51-29"
+        ],
+        "description": {
+            "default": "Cross quite widely planted in western Portugal and on the Açores.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sefka",
-        "synonyms": ["Mavrouti", "Nichevka", "Sefka Nichevka", "Sefko"],
-        "description": "Undistinguished variety of Balkan origin found only in Greece.",
-        "color": "black",
+        "synonyms": [
+            "Mavrouti",
+            "Nichevka",
+            "Sefka Nichevka",
+            "Sefko"
+        ],
+        "description": {
+            "default": "Undistinguished variety of Balkan origin found only in Greece.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Segalin",
-        "synonyms": ["Ségalin"],
-        "description": "Minor Montpellier cross useful for stiffening blends in Cahors country.",
-        "color": "black",
+        "synonyms": [
+            "Ségalin"
+        ],
+        "description": {
+            "default": "Minor Montpellier cross useful for stiffening blends in Cahors country.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Seibel 10868",
-        "synonyms": ["Soleil Blanc"],
-        "description": "Ardèche hybrid found only (rarely) in Michigan today.",
-        "color": "grey",
+        "synonyms": [
+            "Soleil Blanc"
+        ],
+        "description": {
+            "default": "Ardèche hybrid found only (rarely) in Michigan today.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey"
     },
     {
         "name": "Semidano",
-        "synonyms": ["Arvusiniagu", "Laconarzu", "Migiu", "Semidamu", "Semidanu"],
-        "description": "Minor white variety exclusive to the Italian island of Sardegna.",
-        "color": "white",
+        "synonyms": [
+            "Arvusiniagu",
+            "Laconarzu",
+            "Migiu",
+            "Semidamu",
+            "Semidanu"
+        ],
+        "description": {
+            "default": "Minor white variety exclusive to the Italian island of Sardegna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sémillon",
         "synonyms": [
             "Barnawartha Pinot",
             "Blanc Doux",
             "Chevrier",
             "Greengrape",
             "Hunter River Riesling",
             "Merwah",
             "Saint-Émilion",
             "Semilion",
             "Semillon",
             "Sémillon Blanc",
-            "Sémillon Muscat",
+            "Sémillon Muscat"
         ],
-        "description": "The grape variety of sweet white bordeaux and a natural blending partner of Sauvignon Blanc in dry whites too.",
-        "color": "white",
+        "description": {
+            "default": "The grape variety of sweet white bordeaux and a natural blending partner of Sauvignon Blanc in dry whites too.",
+            "julie": "Sémillon is rarely found as a solo grape variety and is generally blended with Sauvignon Blanc. When fully ripe, Sémillon gives wines which are soft and waxy in texture with aromas of citrus fruits, lanolin and sometimes smokiness. In Bordeaux, Sémillon is used for the production of both white and sweet wines and is a key player in the production of botrytised wines in Sauternes and Barsac. In Australia, it is often blended with Sauvignon blanc in the Margaret River to produce high quality white wines that can age gracefully. The Hunter Valley, Australia, has build its reputation on the production of Semillon varietal wines which are bone dry, low in alcohol, lean and high in acidity and requires years in bottle to develop fully. Semillon is also showing some interesting results in Argentina. ",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sercial",
-        "synonyms": ["Arinto dos Açores", "Esgana", "Esgana Cão", "Esganoso"],
-        "description": "Exceptionally acid Portuguese variety most famous for its role in the driest of Madeiras.",
-        "color": "white",
+        "synonyms": [
+            "Arinto dos Açores",
+            "Esgana",
+            "Esgana Cão",
+            "Esganoso"
+        ],
+        "description": {
+            "default": "Exceptionally acid Portuguese variety most famous for its role in the driest of Madeiras.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sercialinho",
-        "synonyms": ["Cercealinho", "Sercealinho"],
-        "description": "Rare, high-acid Portuguese cross adding freshness and aroma.",
-        "color": "white",
+        "synonyms": [
+            "Cercealinho",
+            "Sercealinho"
+        ],
+        "description": {
+            "default": "Rare, high-acid Portuguese cross adding freshness and aroma.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Servant",
-        "synonyms": ["Nonay", "Raisin Blanc", "Servan"],
-        "description": "Minor variety in both France and South Africa, used mainly for the table.",
-        "color": "white",
+        "synonyms": [
+            "Nonay",
+            "Raisin Blanc",
+            "Servan"
+        ],
+        "description": {
+            "default": "Minor variety in both France and South Africa, used mainly for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Severny",
-        "synonyms": ["Severnyi Muskat"],
-        "description": "Russian variety valued mainly for its cold hardiness.",
-        "color": "black",
+        "synonyms": [
+            "Severnyi Muskat"
+        ],
+        "description": {
+            "default": "Russian variety valued mainly for its cold hardiness.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Seyval Blanc",
-        "synonyms": ["Seyval", "Seyve-Villard", "Seyve-Villard 5276"],
-        "description": "One of the more successful pale-skinned French hybrids, popular in marginal climates, especially England.",
-        "color": "white",
+        "synonyms": [
+            "Seyval",
+            "Seyve-Villard",
+            "Seyve-Villard 5276"
+        ],
+        "description": {
+            "default": "One of the more successful pale-skinned French hybrids, popular in marginal climates, especially England.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Seyval Noir",
-        "synonyms": ["Seyve-Villard 5247"],
-        "description": "Isère hybrid that is less successful than its white sibling but still found in Québec.",
-        "color": "black",
+        "synonyms": [
+            "Seyve-Villard 5247"
+        ],
+        "description": {
+            "default": "Isère hybrid that is less successful than its white sibling but still found in Québec.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sgavetta",
-        "synonyms": ["Sganetta", "Sgavetta a Graspo Rosso"],
-        "description": "Emilia-Romagna rarity, generally playing only a small, colouring part in blends.",
-        "color": "black",
+        "synonyms": [
+            "Sganetta",
+            "Sgavetta a Graspo Rosso"
+        ],
+        "description": {
+            "default": "Emilia-Romagna rarity, generally playing only a small, colouring part in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Shavkapito",
-        "synonyms": ["Chavkapito"],
-        "description": "Rediscovered and promising dark-skinned Georgian variety.",
-        "color": "black",
+        "synonyms": [
+            "Chavkapito"
+        ],
+        "description": {
+            "default": "Rediscovered and promising dark-skinned Georgian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Shesh I Bardhë",
-        "synonyms": ["Pucalla"],
-        "description": "Albania’s most planted, late-ripening, light-skinned indigenous variety.",
-        "color": "white",
+        "synonyms": [
+            "Pucalla"
+        ],
+        "description": {
+            "default": "Albania’s most planted, late-ripening, light-skinned indigenous variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Shesh I Zi",
-        "synonyms": ["Seshi Zi", "Shesh"],
-        "description": "Albania’s most planted indigenous dark-skinned variety.",
-        "color": "black",
+        "synonyms": [
+            "Seshi Zi",
+            "Shesh"
+        ],
+        "description": {
+            "default": "Albania’s most planted indigenous dark-skinned variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Shevka",
-        "synonyms": ["Chevka"],
-        "description": "Bulgarian making bland, low-alcohol, low-acid reds.",
-        "color": "black",
+        "synonyms": [
+            "Chevka"
+        ],
+        "description": {
+            "default": "Bulgarian making bland, low-alcohol, low-acid reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Shiroka Melnishka",
         "synonyms": [
             "Chiroka Melnichka",
             "Melnik",
             "Shiroka Melnishka Loza",
-            "Siroka Melniska",
+            "Siroka Melniska"
         ],
-        "description": "Very old, late-ripening, top-quality variety associated with Melnik in the far south west of Bulgaria producing powerful, ageworthy reds.",
-        "color": "black",
+        "description": {
+            "default": "Very old, late-ripening, top-quality variety associated with Melnik in the far south west of Bulgaria producing powerful, ageworthy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Shirvanshahy",
-        "synonyms": ["Shirvan Schahi", "Shirvanshakhi", "Shirvan Shakhi"],
-        "description": "Powerful, Azeri variety used to make fortified, semi-sweet as well as dry reds.",
-        "color": "black",
+        "synonyms": [
+            "Shirvan Schahi",
+            "Shirvanshakhi",
+            "Shirvan Shakhi"
+        ],
+        "description": {
+            "default": "Powerful, Azeri variety used to make fortified, semi-sweet as well as dry reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sibirkovy",
-        "synonyms": ["Efremovsky", "Sibirek", "Sibir’kovy"],
-        "description": "Very minor Russian variety making aromatic whites on the banks of the Don.",
-        "color": "white",
+        "synonyms": [
+            "Efremovsky",
+            "Sibirek",
+            "Sibir’kovy"
+        ],
+        "description": {
+            "default": "Very minor Russian variety making aromatic whites on the banks of the Don.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sidalan",
-        "synonyms": ["Sidalak"],
-        "description": "Rare Turkish variety grown mainly on the Aegean island of Bozcaada.",
-        "color": "white",
+        "synonyms": [
+            "Sidalak"
+        ],
+        "description": {
+            "default": "Rare Turkish variety grown mainly on the Aegean island of Bozcaada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sideritis",
         "synonyms": [
             "Akaki",
             "Chimoniatiko",
             "Siderites",
             "Sideritis Scopelan",
             "Sideritis Scopelou",
-            "Sidiritis",
+            "Sidiritis"
         ],
-        "description": "Pink-skinned Greek variety grown mainly for the table but now showing potential for crisp, peppery whites.",
-        "color": "pink",
+        "description": {
+            "default": "Pink-skinned Greek variety grown mainly for the table but now showing potential for crisp, peppery whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Siegerrebe",
-        "synonyms": ["Alzey 7957", "Scheu 7957", "Sieger"],
-        "description": "Overpoweringly Muscat-scented, low-acid German cross.",
-        "color": "pink",
+        "synonyms": [
+            "Alzey 7957",
+            "Scheu 7957",
+            "Sieger"
+        ],
+        "description": {
+            "default": "Overpoweringly Muscat-scented, low-acid German cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Silvaner",
         "synonyms": [
             "Bálint",
             "Gros Rhin",
             "Grüner Silvaner",
@@ -10010,24 +15940,34 @@
             "Silvain Vert",
             "Silvanac Zeleni",
             "Silvánske Zelené",
             "Sylvaner",
             "Sylvaner Verde",
             "Sylvanske Zelené",
             "Zeleni Silvanec",
-            "Zöld Szilváni",
+            "Zöld Szilváni"
         ],
-        "description": "Austrian variety making relatively neutral wines with impressively racy firmness and staying power in Germany and Alsace.",
-        "color": "white",
+        "description": {
+            "default": "Austrian variety making relatively neutral wines with impressively racy firmness and staying power in Germany and Alsace.",
+            "julie": "",
+            "sommelier": "Silvaner is diversity. An uncomplicated summer wine, a soft, creamy barrique wine, a well-developed, elegant and lively Großes Gewächs or an intense, long-lasting noble sweetness. Everything is possible. The grape variety perfectly reflects its terroir and combines earthy tones with delicate fruity aromas and mild acidity. Characteristic of Silvaner wines is a fine fragrance reminiscent of herbs or gooseberries, sometimes accompanied by the aroma of fresh hay. As a rule, these are light wines with a discreet, fragrant aroma that are highly appreciated, not least because of their mild acidity. Quality Silvaner will harmonise very well not only with asparagus and fish. On heavy soils, Silvaner can develop into a full-bodied wine with a certain opulence and a distinct aroma of ripe pears and artichokes, making it a welcome accompaniment to more substantial dishes. Subtle in aroma and mild in acidity, hearty, fairly neutral Silvaner is an excellent food pairing wine. The wines are sometimes earthy and powerful, and are prized for being juicy and mouth-filling. Aroma: discreetly fragrant, reminiscent of herbs or gooseberries."
+        },
+        "color": "white"
     },
     {
         "name": "Siramé",
-        "synonyms": ["Salomé"],
-        "description": "Very minor Swiss hybrid that adapts well to marginal climates.",
-        "color": "black",
+        "synonyms": [
+            "Salomé"
+        ],
+        "description": {
+            "default": "Very minor Swiss hybrid that adapts well to marginal climates.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Síria",
         "synonyms": [
             "Alva",
             "Alvadurão",
             "Alvaro de Soire",
@@ -10047,226 +15987,415 @@
             "Malvasía Castellana",
             "Malvasía Grosso",
             "Moza Fresca",
             "Posto Branco",
             "Roupeiro",
             "Sabro",
             "Valenciana",
-            "Verdegudillo",
+            "Verdegudillo"
         ],
-        "description": "Aromatic, light-skinned variety widely planted in Portugal under various names, with as many names but fewer vines in Spain.",
-        "color": "white",
+        "description": {
+            "default": "Aromatic, light-skinned variety widely planted in Portugal under various names, with as many names but fewer vines in Spain.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sklava",
-        "synonyms": ["Sklaba", "Sklabes", "Sklabos", "Sklaves", "Sklavos"],
-        "description": "Greek variety producing lightweight wines used in blends.",
-        "color": "white",
+        "synonyms": [
+            "Sklaba",
+            "Sklabes",
+            "Sklabos",
+            "Sklaves",
+            "Sklavos"
+        ],
+        "description": {
+            "default": "Greek variety producing lightweight wines used in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Skopelitiko",
-        "synonyms": ["Scopelitico", "Skopelitis"],
-        "description": "Speciality of the island of Kérkyra (Corfu).",
-        "color": "black",
+        "synonyms": [
+            "Scopelitico",
+            "Skopelitis"
+        ],
+        "description": {
+            "default": "Speciality of the island of Kérkyra (Corfu).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Škrlet",
-        "synonyms": ["Ovnek Slatki", "Ovnek Žuti", "Škrlet Tusti", "Škrtec"],
-        "description": "Delicate, fresh Croatian variety enjoying a new lease of life.",
-        "color": "white",
+        "synonyms": [
+            "Ovnek Slatki",
+            "Ovnek Žuti",
+            "Škrlet Tusti",
+            "Škrtec"
+        ],
+        "description": {
+            "default": "Delicate, fresh Croatian variety enjoying a new lease of life.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Skylopnichtis",
         "synonyms": [
             "Kasteliotiko",
             "Mavros Arkadias",
             "Skylopnichtis Kokkino",
             "Skylopnichtra",
-            "Skylopnihti",
+            "Skylopnihti"
         ],
-        "description": "Rare Greek variety used in traditional local blends.",
-        "color": "black",
+        "description": {
+            "default": "Rare Greek variety used in traditional local blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Slankamenka",
         "synonyms": [
             "Mađaruša",
             "Maghiarca",
             "Magyarica",
             "Magyarkă",
             "Majarcă Albă",
             "Slankamenka Béla",
-            "Szlanka Fehér",
+            "Szlanka Fehér"
         ],
-        "description": "Ancient Balkan variety producing generally uninspiring whites.",
-        "color": "white",
+        "description": {
+            "default": "Ancient Balkan variety producing generally uninspiring whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Solaris",
-        "synonyms": ["Freiburg 240-75"],
-        "description": "Modern, disease-resistant and early-ripening German hybrid that produces tooth-rottingly high sugar levels.",
-        "color": "white",
+        "synonyms": [
+            "Freiburg 240-75"
+        ],
+        "description": {
+            "default": "Modern, disease-resistant and early-ripening German hybrid that produces tooth-rottingly high sugar levels.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Soldaia",
-        "synonyms": ["SD-56", "Soldaiya"],
-        "description": "Old, late-ripening Ukrainian variety found occasionally in blends.",
-        "color": "white",
+        "synonyms": [
+            "SD-56",
+            "Soldaiya"
+        ],
+        "description": {
+            "default": "Old, late-ripening Ukrainian variety found occasionally in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Solnechnodolinsky",
-        "synonyms": ["DM-63", "SD-2"],
-        "description": "Productive Ukrainian pale-skinned variety.",
-        "color": "white",
+        "synonyms": [
+            "DM-63",
+            "SD-2"
+        ],
+        "description": {
+            "default": "Productive Ukrainian pale-skinned variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Soperga",
-        "synonyms": ["Incrocio Dalmasso IV/31", "Superga"],
-        "description": "Rare Conegliano cross whose true parentage has only recently been revealed.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso IV/31",
+            "Superga"
+        ],
+        "description": {
+            "default": "Rare Conegliano cross whose true parentage has only recently been revealed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sorbigno",
-        "synonyms": ["Sorbino", "Sorvegna", "Sorvigno"],
-        "description": "A minor Ischian speciality.",
-        "color": "white",
+        "synonyms": [
+            "Sorbino",
+            "Sorvegna",
+            "Sorvigno"
+        ],
+        "description": {
+            "default": "A minor Ischian speciality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Spergola",
-        "synonyms": ["Spargoletta Bianca", "Spergolà", "Spergolina", "Spergolinàis"],
-        "description": "Tart Emilia-Romagnan thought until very recently to be Sauvignon Blanc.",
-        "color": "white",
+        "synonyms": [
+            "Spargoletta Bianca",
+            "Spergolà",
+            "Spergolina",
+            "Spergolinàis"
+        ],
+        "description": {
+            "default": "Tart Emilia-Romagnan thought until very recently to be Sauvignon Blanc.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Spourtiko",
-        "synonyms": ["Spourtico"],
-        "description": "Rare Cypriot variety producing light, zesty whites.",
-        "color": "white",
+        "synonyms": [
+            "Spourtico"
+        ],
+        "description": {
+            "default": "Rare Cypriot variety producing light, zesty whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "St Croix",
-        "synonyms": ["ES 2-3-21", "Sainte-Croix", "Ste-Croix"],
-        "description": "Very cold-hardy, complex American hybrid gaining ground in Québec and the Midwest.",
-        "color": "black",
+        "synonyms": [
+            "ES 2-3-21",
+            "Sainte-Croix",
+            "Ste-Croix"
+        ],
+        "description": {
+            "default": "Very cold-hardy, complex American hybrid gaining ground in Québec and the Midwest.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "St Pepin",
-        "synonyms": ["Elmer Swenson 282", "ES 282", "Saint-Pépin"],
-        "description": "Fruity, low-acid American hybrid that often has a hint of foxiness.",
-        "color": "white",
+        "synonyms": [
+            "Elmer Swenson 282",
+            "ES 282",
+            "Saint-Pépin"
+        ],
+        "description": {
+            "default": "Fruity, low-acid American hybrid that often has a hint of foxiness.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Stanušina Crna",
-        "synonyms": ["Gradesh", "Stanušhina Crna", "Strnušina", "Tikvesko"],
-        "description": "Macedonian variety in dire need of vineyard selection to improve quality.",
-        "color": "black",
+        "synonyms": [
+            "Gradesh",
+            "Stanušhina Crna",
+            "Strnušina",
+            "Tikvesko"
+        ],
+        "description": {
+            "default": "Macedonian variety in dire need of vineyard selection to improve quality.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Stavroto",
-        "synonyms": ["Ampelakiotiko", "Ampelakiotiko Mavro", "Stavromavro"],
-        "description": "Greek variety required in and virtually exclusive to the Rapsáni appellation.",
-        "color": "black",
+        "synonyms": [
+            "Ampelakiotiko",
+            "Ampelakiotiko Mavro",
+            "Stavromavro"
+        ],
+        "description": {
+            "default": "Greek variety required in and virtually exclusive to the Rapsáni appellation.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Steuben",
-        "synonyms": ["New York 12696"],
-        "description": "Minor but successful American hybrid used for the table and for wine.",
-        "color": "black",
+        "synonyms": [
+            "New York 12696"
+        ],
+        "description": {
+            "default": "Minor but successful American hybrid used for the table and for wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Storgozia",
-        "synonyms": ["Storgoziya"],
-        "description": "Recent, usefully disease-resistant Bulgarian hybrid.",
-        "color": "black",
+        "synonyms": [
+            "Storgoziya"
+        ],
+        "description": {
+            "default": "Recent, usefully disease-resistant Bulgarian hybrid.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sultaniye",
         "synonyms": [
             "Banati",
             "Kishmish",
             "Kis Mis Alb",
             "Kişmiş",
             "Soultanina",
             "Sultana",
             "Sultani Çekirdeksiz",
             "Sultanina",
             "Sultanina Blanche",
             "Sultanine",
-            "Thompson Seedless",
+            "Thompson Seedless"
         ],
-        "description": "The world’s most widely planted light-skinned variety. The sultana grape is only rarely used for wine, fortunately.",
-        "color": "white",
+        "description": {
+            "default": "The world’s most widely planted light-skinned variety. The sultana grape is only rarely used for wine, fortunately.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sumoll",
         "synonyms": [
             "Sumoi",
             "Sumoll Negro",
             "Sumoll Tinto",
             "Sunier",
             "Verijariego Negra",
             "Vigiriega",
             "Vigiriega Negra",
             "Vigiriego Negro",
             "Vijariego Negra",
             "Vijariego Negro",
-            "Vijiriego Negro",
+            "Vijiriego Negro"
         ],
-        "description": "Minor Catalan found mainly in red blends, and also now on the Islas Canarias.",
-        "color": "black",
+        "description": {
+            "default": "Minor Catalan found mainly in red blends, and also now on the Islas Canarias.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Sumoll Blanc",
-        "synonyms": ["Sumoi Blanc", "Sumoll Blanco"],
-        "description": "Very rare but promising, refreshing Catalan variety that is unrelated to the dark-berried Sumoll.",
-        "color": "white",
+        "synonyms": [
+            "Sumoi Blanc",
+            "Sumoll Blanco"
+        ],
+        "description": {
+            "default": "Very rare but promising, refreshing Catalan variety that is unrelated to the dark-berried Sumoll.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sušćan",
-        "synonyms": ["Brajda Velika Crna", "Sansigot", "Susac", "Sušćan Crni"],
-        "description": "Minor Croatian variety found on just a few islands in the Adriatic but gaining in popularity.",
-        "color": "black",
+        "synonyms": [
+            "Brajda Velika Crna",
+            "Sansigot",
+            "Susac",
+            "Sušćan Crni"
+        ],
+        "description": {
+            "default": "Minor Croatian variety found on just a few islands in the Adriatic but gaining in popularity.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Susumaniello",
         "synonyms": [
             "Cozzomaniello",
             "Grismaniello",
             "Somarello Nero",
             "Susomaniello",
             "Susumaniello Nero",
             "Zingariello",
-            "Zuzomaniello",
+            "Zuzomaniello"
         ],
-        "description": "Minor, deeply coloured Puglian.",
-        "color": "black",
+        "description": {
+            "default": "Minor, deeply coloured Puglian.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Swenson Red",
-        "synonyms": ["Elmer Swenson 439"],
-        "description": "Minor red-berried American hybrid bred for the chill of the Northwest.",
-        "color": "red",
+        "synonyms": [
+            "Elmer Swenson 439"
+        ],
+        "description": {
+            "default": "Minor red-berried American hybrid bred for the chill of the Northwest.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Swenson White",
-        "synonyms": ["ES 6-1-43"],
-        "description": "Minor but very complex, cold-hardy American hybrid better suited to the table than to wine.",
-        "color": "white",
+        "synonyms": [
+            "ES 6-1-43"
+        ],
+        "description": {
+            "default": "Minor but very complex, cold-hardy American hybrid better suited to the table than to wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Sykiotis",
-        "synonyms": ["Chiotis", "Kiotes", "Skiotes", "Skiotis", "Sykioti"],
-        "description": "Greek variety used mainly for distillation.",
-        "color": "black",
+        "synonyms": [
+            "Chiotis",
+            "Kiotes",
+            "Skiotes",
+            "Skiotis",
+            "Sykioti"
+        ],
+        "description": {
+            "default": "Greek variety used mainly for distillation.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Symphony",
-        "synonyms": ["Davis S15-58"],
-        "description": "Rare and highly aromatic Muscat-flavoured California cross.",
-        "color": "white",
+        "synonyms": [
+            "Davis S15-58"
+        ],
+        "description": {
+            "default": "Rare and highly aromatic Muscat-flavoured California cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Syrah",
         "synonyms": [
             "Candive",
             "Hermitage",
             "Marsanne Noire",
@@ -10276,102 +16405,141 @@
             "Sérine",
             "Serinne",
             "Shiraz",
             "Sira",
             "Sirac",
             "Sirah",
             "Syra",
-            "Syrac",
+            "Syrac"
         ],
-        "description": "Generally fashionable alternative to Cabernet Sauvignon with a complex and surprising family background.",
-        "color": "black",
+        "description": {
+            "default": "Generally fashionable alternative to Cabernet Sauvignon with a complex and surprising family background.",
+            "julie": "Syrah is originally from the Northern Rhône Valley where it is still today producing some world class red wines under appellations such as Hermitage, Côte Rôtie and Cornas. The wines are perfumed with aromas of violet, black fruits, black pepper citrus peels, juniper berries, etc.  and have the potential to age for decades for many of them. In Australia, Syrah is called Shiraz but that names can also be found in other countries such as South Africa. Wines labeled as Shiraz tend to be big, bold and oaky as a reference to the Barossa Shiraz style from Australia but this is not always the case anymore. Syrah is also often found blended with Grenache noir and Mourvèdre for its ability to bring structure, acidity and perfume. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Syriki",
         "synonyms": [
             "Cserichi",
             "Kserikhi",
             "Kseriki",
             "Kserukhti",
             "Seriki",
             "Syrike",
             "Xerichi",
             "Xerichi Mavro",
             "Xeruchti",
-            "Xirichi",
+            "Xirichi"
         ],
-        "description": "Vine variety grown spottily around Greece but rarely seen on labels.",
-        "color": "black",
+        "description": {
+            "default": "Vine variety grown spottily around Greece but rarely seen on labels.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tamarez",
-        "synonyms": ["Arinto Gordo", "Boal Prior", "Tamares", "Tamarez Branco"],
-        "description": "Old southern Portuguese variety authorized in many wine regions but usually distilled or blended.",
-        "color": "white",
+        "synonyms": [
+            "Arinto Gordo",
+            "Boal Prior",
+            "Tamares",
+            "Tamarez Branco"
+        ],
+        "description": {
+            "default": "Old southern Portuguese variety authorized in many wine regions but usually distilled or blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Tamurro",
-        "synonyms": ["Coll d’Tammurr"],
-        "description": "Virtually extinct, thick-skinned Basilicata variety.",
-        "color": "black",
+        "synonyms": [
+            "Coll d’Tammurr"
+        ],
+        "description": {
+            "default": "Virtually extinct, thick-skinned Basilicata variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tannat",
         "synonyms": [
             "Bordelez Beltza",
             "Harriague",
             "Madiran",
             "Moustrou",
             "Moustroun",
-            "Tanat",
+            "Tanat"
         ],
-        "description": "Powerful, characterful, often tannic variety at home in south-west France and Uruguay but becoming global.",
-        "color": "black",
+        "description": {
+            "default": "Powerful, characterful, often tannic variety at home in south-west France and Uruguay but becoming global.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tauberschwarz",
         "synonyms": [
             "Blaue Hartwegstraube",
             "Blauer Hängling",
             "Elsässer",
             "Frankentraube",
             "Grobrot",
             "Grobschwarze",
             "Häusler",
-            "Süssrot",
+            "Süssrot"
         ],
-        "description": "Old, unidentified cross used to produce light reds in southern Germany.",
-        "color": "black",
+        "description": {
+            "default": "Old, unidentified cross used to produce light reds in southern Germany.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tavkveri",
         "synonyms": [
             "Takweri",
             "Tarkveri",
             "Tavaveri",
             "Tavkeri Kartalinsky",
             "Tavkeri Kartlis",
-            "Tavkveri Didmartsvala",
+            "Tavkveri Didmartsvala"
         ],
-        "description": "Georgian variety producing very small amounts of light, tangy reds.",
-        "color": "black",
+        "description": {
+            "default": "Georgian variety producing very small amounts of light, tangy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tazzelenghe",
         "synonyms": [
             "Refosco del Botton",
             "Tacelenghe",
             "Tassalinghe",
             "Taze Lunghe",
             "Tazzalenghe Nera",
             "Tazzalenghe Nera Friulana",
-            "Tazzalingua",
+            "Tazzalingua"
         ],
-        "description": "High-acid and potentially astringent red Friulian, rescued from extinction in the 1980s.",
-        "color": "black",
+        "description": {
+            "default": "High-acid and potentially astringent red Friulian, rescued from extinction in the 1980s.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Teinturier",
         "synonyms": [
             "Auvernat Teint",
             "Bourguignon Noir",
             "Gros Noir",
@@ -10380,18 +16548,22 @@
             "Noir d’Orléans",
             "Plant d’Espagne",
             "Pontac",
             "Tachard",
             "Teint-Vin",
             "Teinturier du Cher",
             "Teinturier Mâle",
-            "Tintewein",
+            "Tintewein"
         ],
-        "description": "Red-fleshed French variety still found (just) in Portugal and South Africa.",
-        "color": "black",
+        "description": {
+            "default": "Red-fleshed French variety still found (just) in Portugal and South Africa.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tempranillo",
         "synonyms": [
             "Aragón",
             "Aragones",
             "Aragonez",
@@ -10418,313 +16590,534 @@
             "Tinto Aragónez",
             "Tinto de Madrid",
             "Tinto del País",
             "Tinto Fino",
             "Ull de Llebre",
             "Valdepeñas",
             "Verdiell",
-            "Vid de Aranda",
+            "Vid de Aranda"
         ],
-        "description": "Spain’s most famous grape, responsible for the majority of its most famous reds.",
-        "color": "black",
+        "description": {
+            "default": "Spain’s most famous grape, responsible for the majority of its most famous reds.",
+            "julie": "Tempranillo is Spain most planted red grape variety and is found under various names such as tinto del pais and cencibel. The wines produced have marked acidity and tannins and flavours of ripe red fruits, tobacco and cocoa often seasoned by American oak bringing aromas of sweet spices and coconut. Tempranillo is widely found in the region of Castilla y Leon and is the key variety in Ribera del Duero DO, Rioja DOCa, Toro DO where it produces world class wines with long ageing potential. In Portugal is known as Tinta Roriz. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Téoulier Noir",
-        "synonyms": ["Manosquin", "Plant de Manosque", "Plant Dufour", "Thuillier"],
-        "description": "Almost extinct Provençal variety.",
-        "color": "black",
+        "synonyms": [
+            "Manosquin",
+            "Plant de Manosque",
+            "Plant Dufour",
+            "Thuillier"
+        ],
+        "description": {
+            "default": "Almost extinct Provençal variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Terbash",
-        "synonyms": ["Irtik Iaprak", "Irtuk Yaprak"],
-        "description": "Widely planted, multi-purpose Turkmen variety.",
-        "color": "white",
+        "synonyms": [
+            "Irtik Iaprak",
+            "Irtuk Yaprak"
+        ],
+        "description": {
+            "default": "Widely planted, multi-purpose Turkmen variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Termarina Rossa",
-        "synonyms": ["Oltremarina", "Tramarina"],
-        "description": "Unusual Emilia-Romagna seedless pink-skinned variety used in cooking as well as for wine.",
-        "color": "pink",
+        "synonyms": [
+            "Oltremarina",
+            "Tramarina"
+        ],
+        "description": {
+            "default": "Unusual Emilia-Romagna seedless pink-skinned variety used in cooking as well as for wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Teroldego",
         "synonyms": [
             "Merlina",
             "Teroldega",
             "Teroldeghe",
             "Teroldico",
             "Teroldigo",
             "Tiraldega",
             "Tirodola",
             "Tiroldegho",
-            "Tiroldigo",
+            "Tiroldigo"
         ],
-        "description": "Well-connected, revived Trentino speciality whose acidity needs careful handling.",
-        "color": "black",
+        "description": {
+            "default": "Well-connected, revived Trentino speciality whose acidity needs careful handling.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Terrano",
         "synonyms": [
             "Cagnina",
             "Crodarina",
             "Rabiosa Nera",
             "Refosco del Carso",
             "Refosco d’Istria",
             "Refosco Terrano",
             "Refošk",
             "Teran",
             "Terran",
             "Terrano del Carso",
-            "Terrano d’Istria",
+            "Terrano d’Istria"
         ],
-        "description": "Significant variety making fresh, aromatic red from the Italy–Slovenia border and Croatia; often confused with the best-known Refosco.",
-        "color": "black",
+        "description": {
+            "default": "Significant variety making fresh, aromatic red from the Italy–Slovenia border and Croatia; often confused with the best-known Refosco.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Terrantez",
-        "synonyms": ["Terrantez da Madeira"],
-        "description": "Historic Madeira variety that has virtually disappeared from the island.",
-        "color": "white",
+        "synonyms": [
+            "Terrantez da Madeira"
+        ],
+        "description": {
+            "default": "Historic Madeira variety that has virtually disappeared from the island.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Terret",
-        "synonyms": ["Bourret", "Tarret"],
-        "description": "Old Languedoc variety found in three colours, all in quantitative decline.",
-        "color": "white, grey and black",
+        "synonyms": [
+            "Bourret",
+            "Tarret"
+        ],
+        "description": {
+            "default": "Old Languedoc variety found in three colours, all in quantitative decline.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white, grey and black"
     },
     {
         "name": "Thrapsathiri",
-        "synonyms": ["Begleri", "Beghleri", "Dafnato"],
-        "description": "Distinctive Greek island variety, travelling under two names and producing richly fruited wines.",
-        "color": "white",
+        "synonyms": [
+            "Begleri",
+            "Beghleri",
+            "Dafnato"
+        ],
+        "description": {
+            "default": "Distinctive Greek island variety, travelling under two names and producing richly fruited wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Tibouren",
         "synonyms": [
             "Antiboulen",
             "Rossese",
             "Rossese di Dolceacqua",
             "Rossese Nericcio",
             "Rossese di Ventimiglia",
-            "Tiboulen",
+            "Tiboulen"
         ],
-        "description": "Ancient variety making fine rosé wines in Provence and light reds over the border in Italy’s Liguria.",
-        "color": "black",
+        "description": {
+            "default": "Ancient variety making fine rosé wines in Provence and light reds over the border in Italy’s Liguria.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tigrani",
-        "synonyms": ["1452/75"],
-        "description": "Armenian all-vinifera cross used for reds dry and sweet.",
-        "color": "black",
+        "synonyms": [
+            "1452/75"
+        ],
+        "description": {
+            "default": "Armenian all-vinifera cross used for reds dry and sweet.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Timorasso",
-        "synonyms": ["Morasso", "Timoraccio", "Timuassa"],
-        "description": "Rare, high-quality Piemontese earning renewed recognition.",
-        "color": "white",
+        "synonyms": [
+            "Morasso",
+            "Timoraccio",
+            "Timuassa"
+        ],
+        "description": {
+            "default": "Rare, high-quality Piemontese earning renewed recognition.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Tinta Barroca",
-        "synonyms": ["Boca de Mina", "Tinta Barocca", "Tinta das Baroccas"],
-        "description": "Rustic, dark-skinned, early-ripening port variety.",
-        "color": "black",
+        "synonyms": [
+            "Boca de Mina",
+            "Tinta Barocca",
+            "Tinta das Baroccas"
+        ],
+        "description": {
+            "default": "Rustic, dark-skinned, early-ripening port variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tinta Carvalha",
-        "synonyms": ["Lobão", "Preto Gordo", "Tinta Carvalha du Douro"],
-        "description": "Portuguese variety that is light in every way.",
-        "color": "black",
+        "synonyms": [
+            "Lobão",
+            "Preto Gordo",
+            "Tinta Carvalha du Douro"
+        ],
+        "description": {
+            "default": "Portuguese variety that is light in every way.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tinta Castañal",
-        "synonyms": ["Castañal", "Rabo de Cordeiro"],
-        "description": "Recently resurrected Galician of unknown origin.",
-        "color": "black",
+        "synonyms": [
+            "Castañal",
+            "Rabo de Cordeiro"
+        ],
+        "description": {
+            "default": "Recently resurrected Galician of unknown origin.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tinta Francisca",
-        "synonyms": ["Tinta de França", "Tinta Francesca", "Tinta Franceza"],
-        "description": "Lesser but not insignificant port variety.",
-        "color": "black",
+        "synonyms": [
+            "Tinta de França",
+            "Tinta Francesca",
+            "Tinta Franceza"
+        ],
+        "description": {
+            "default": "Lesser but not insignificant port variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tintilia Del Molise",
-        "synonyms": ["Tintilia"],
-        "description": "Minor Molise variety until recently confused with Bovale Grande (ie Mazuelo/Carignan).",
-        "color": "black",
+        "synonyms": [
+            "Tintilia"
+        ],
+        "description": {
+            "default": "Minor Molise variety until recently confused with Bovale Grande (ie Mazuelo/Carignan).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tinto Cão",
-        "synonyms": ["Farmento", "Tinta Cão"],
-        "description": "High-quality port variety that occasionally shines in Dão.",
-        "color": "black",
+        "synonyms": [
+            "Farmento",
+            "Tinta Cão"
+        ],
+        "description": {
+            "default": "High-quality port variety that occasionally shines in Dão.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tinto Velasco",
         "synonyms": [
             "Benitillo",
             "Blasco",
             "Frasco",
             "Granadera",
             "Tinto de la Pámpana Blanca",
-            "Tinto Velasco Peludo",
+            "Tinto Velasco Peludo"
         ],
-        "description": "Unexciting La Mancha variety.",
-        "color": "black",
+        "description": {
+            "default": "Unexciting La Mancha variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tintore Di Tramonti",
-        "synonyms": ["Cannamelu", "Guarnaccia", "Tintora", "Tintore"],
-        "description": "Rare, deeply coloured Campanian with excellent potential for fine reds.",
-        "color": "black",
+        "synonyms": [
+            "Cannamelu",
+            "Guarnaccia",
+            "Tintora",
+            "Tintore"
+        ],
+        "description": {
+            "default": "Rare, deeply coloured Campanian with excellent potential for fine reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Torbato",
         "synonyms": [
             "Malvoisie du Roussillon",
             "Malvoisie des Pyrénées Orientales",
             "Torbat",
             "Tourbat",
             "Turbat",
-            "Uva Catalana",
+            "Uva Catalana"
         ],
-        "description": "Pale-berried variety found on the Italian island of Sardegna and in southern France, recovering from virtual extinction.",
-        "color": "white",
+        "description": {
+            "default": "Pale-berried variety found on the Italian island of Sardegna and in southern France, recovering from virtual extinction.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Torrontés Mendocino",
-        "synonyms": ["Chichera", "Loca Blanca", "Palet"],
-        "description": "A lesser Argentine Torrontés.",
-        "color": "white",
+        "synonyms": [
+            "Chichera",
+            "Loca Blanca",
+            "Palet"
+        ],
+        "description": {
+            "default": "A lesser Argentine Torrontés.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Torrontés Riojano",
-        "synonyms": ["Malvasia"],
-        "description": "The most important of the three Argentine Torrontés Somethings, responsible for the country’s highly aromatic signature white wine.",
-        "color": "white",
+        "synonyms": [
+            "Malvasia"
+        ],
+        "description": {
+            "default": "The most important of the three Argentine Torrontés Somethings, responsible for the country’s highly aromatic signature white wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Torrontés Sanjuanino",
-        "synonyms": ["Moscatel de Austria", "Moscatel Romano"],
-        "description": "One of the two lesser-known Torrontés Somethings in Argentina.",
-        "color": "white",
+        "synonyms": [
+            "Moscatel de Austria",
+            "Moscatel Romano"
+        ],
+        "description": {
+            "default": "One of the two lesser-known Torrontés Somethings in Argentina.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Torysa",
-        "synonyms": ["CATAP 9/17"],
-        "description": "Recently authorized red-fleshed Slovakian cross.",
-        "color": "black",
+        "synonyms": [
+            "CATAP 9/17"
+        ],
+        "description": {
+            "default": "Recently authorized red-fleshed Slovakian cross.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Touriga Fêmea",
-        "synonyms": ["Tinta Coimbra", "Touriga Brasileira"],
-        "description": "Minor Touriga from northern Portugal.",
-        "color": "black",
+        "synonyms": [
+            "Tinta Coimbra",
+            "Touriga Brasileira"
+        ],
+        "description": {
+            "default": "Minor Touriga from northern Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Touriga Franca",
         "synonyms": [
             "Albino de Souza",
             "Touriga Frances",
             "Touriga Francesa",
-            "Tourigo Francês",
+            "Tourigo Francês"
         ],
-        "description": "High-quality, widely planted Douro variety qualitatively in the shadow of Touriga Nacional.",
-        "color": "black",
+        "description": {
+            "default": "High-quality, widely planted Douro variety qualitatively in the shadow of Touriga Nacional.",
+            "julie": "Touriga Franca is the most widely planted red grape variety in the Douro Valley in Portugal. The grape is used for the production of Port wines and Table wines mostly as part of a blend to which it brings finesse, good depth of colour, and a beautiful perfume of red fruits and wild flowers and herbs. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Touriga Nacional",
         "synonyms": [
             "Azal Espanhol",
             "Carabuñeira",
             "Mortagua",
             "Mortagua Preto",
             "Touriga",
             "Touriga Fina",
             "Tourigo",
             "Tourigo Antiguo",
-            "Tourigo do Dão",
+            "Tourigo do Dão"
         ],
-        "description": "High-quality, concentrated, tannic and perfumed dark-skinned Portuguese variety increasingly cast in a starring role.",
-        "color": "black",
+        "description": {
+            "default": "High-quality, concentrated, tannic and perfumed dark-skinned Portuguese variety increasingly cast in a starring role.",
+            "julie": "Touriga Nacional is an iconic red grape variety from Portugal, especially highly praised for the production of Port wines in the Douro valley. The grapes gives wines which are deeply coloured, concentrated, tannic and beautifully fragrant - rose flowers, violet, blue and black fruits, tea, etc. Despite their structure however, the wines made from Touriga Nacional display a charisma and elegance very specific to the grape. ",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tourkopoula",
-        "synonyms": ["Rhoditis Kokkinos", "Roditis Kokkinos"],
-        "description": "Rare, pinky-red-skinned Greek variety that should not be confused with Roditis.",
-        "color": "pink",
+        "synonyms": [
+            "Rhoditis Kokkinos",
+            "Roditis Kokkinos"
+        ],
+        "description": {
+            "default": "Rare, pinky-red-skinned Greek variety that should not be confused with Roditis.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Trajadura",
-        "synonyms": ["Treixadura"],
-        "description": "High-quality variety best in blends in the north-western corner of both Spain and Portugal.",
-        "color": "white",
+        "synonyms": [
+            "Treixadura"
+        ],
+        "description": {
+            "default": "High-quality variety best in blends in the north-western corner of both Spain and Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trbljan",
         "synonyms": [
             "Dobrogoština",
             "Grban",
             "Kuč",
             "Pljuskavac",
             "Rukavina",
             "Šampanjol",
-            "Trbljan Bijeli",
+            "Trbljan Bijeli"
         ],
-        "description": "Variety widely planted in coastal Croatia for long thought to be a Trebbiano.",
-        "color": "white",
+        "description": {
+            "default": "Variety widely planted in coastal Croatia for long thought to be a Trebbiano.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trebbiano D’Abruzzo",
         "synonyms": [
             "Sbagagnina",
             "Sbagarina",
             "Svagadia",
             "Trebbiano Abruzzese",
             "Trebbiano Campolese",
-            "Trebbiano di Teramo",
+            "Trebbiano di Teramo"
         ],
-        "description": "Light-skinned variety from east-central Italy unrelated to other Trebbianos but whose identity is still unclear.",
-        "color": "white",
+        "description": {
+            "default": "Light-skinned variety from east-central Italy unrelated to other Trebbianos but whose identity is still unclear.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trebbiano Giallo",
         "synonyms": [
             "Greco di Velletri",
             "Trebbiano dei Castelli",
             "Trebbiano di Spagna",
-            "Trebbiano Giallo di Velletri",
+            "Trebbiano Giallo di Velletri"
         ],
-        "description": "Another Trebbiano, grown and blended mainly around Roma.",
-        "color": "white",
+        "description": {
+            "default": "Another Trebbiano, grown and blended mainly around Roma.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trebbiano Modenese",
         "synonyms": [
             "Terbiàn Moscatlè",
             "Terbianella",
             "Trebbiano Comune",
             "Trebbiano di Collina",
             "Trebbiano di Modena",
-            "Trebbiano Montanaro",
+            "Trebbiano Montanaro"
         ],
-        "description": "Emilia-Romagnan used more for balsamic vinegar than for wine.",
-        "color": "white",
+        "description": {
+            "default": "Emilia-Romagnan used more for balsamic vinegar than for wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trebbiano Romagnolo",
-        "synonyms": ["Trebbiano della Fiamma", "Trebbiano di Romagna"],
-        "description": "The widely planted but not especially distinguished Emilia-Romagnan Trebbiano.",
-        "color": "white",
+        "synonyms": [
+            "Trebbiano della Fiamma",
+            "Trebbiano di Romagna"
+        ],
+        "description": {
+            "default": "The widely planted but not especially distinguished Emilia-Romagnan Trebbiano.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trebbiano Spoletino",
-        "synonyms": ["Spoletino", "Trebbiano di Avezzano", "Trebbiano di Spoleto"],
-        "description": "Recently rescued Umbrian capable of better quality, and more body, than most Trebbiano Somethings.",
-        "color": "white",
+        "synonyms": [
+            "Spoletino",
+            "Trebbiano di Avezzano",
+            "Trebbiano di Spoleto"
+        ],
+        "description": {
+            "default": "Recently rescued Umbrian capable of better quality, and more body, than most Trebbiano Somethings.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trebbiano Toscano",
         "synonyms": [
             "Alfrocheiro Branco",
             "Armenian",
             "Bianca di Poviglio",
@@ -10736,33 +17129,41 @@
             "Rossola Brandisca",
             "Roussan",
             "Saint-Émilion",
             "St Emilion",
             "Šijaka",
             "Tália",
             "Thalia",
-            "Ugni Blanc",
+            "Ugni Blanc"
         ],
-        "description": "Tuscan variety also known as Ugni Blanc that probably produces more (typically tart and neutral) wine than any other vine in the world.",
-        "color": "white",
+        "description": {
+            "default": "Tuscan variety also known as Ugni Blanc that probably produces more (typically tart and neutral) wine than any other vine in the world.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Trepat",
         "synonyms": [
             "Bonicaire",
             "Carlina",
             "Embolicaire",
             "Negra Blana",
             "Parrel",
             "Parrel-Verdal",
             "Trepat Negre",
-            "Traput",
+            "Traput"
         ],
-        "description": "Red-skinned Catalan traditionally used for still and sparkling rosés.",
-        "color": "red",
+        "description": {
+            "default": "Red-skinned Catalan traditionally used for still and sparkling rosés.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Tressot",
         "synonyms": [
             "Bourguignon",
             "Bourguignon Noir",
             "Morillon Noir",
@@ -10770,24 +17171,36 @@
             "Nairien",
             "Resseau",
             "Treceaux",
             "Tresseau",
             "Tressiot",
             "Tressot Noir",
             "Vérot",
-            "Petit Verrot",
+            "Petit Verrot"
         ],
-        "description": "Ancient but virtually extinct, struggling variety from Chablis country of intriguing parentage.",
-        "color": "black",
+        "description": {
+            "default": "Ancient but virtually extinct, struggling variety from Chablis country of intriguing parentage.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Trevisana Nera",
-        "synonyms": ["Borgogna", "Gattera", "Refosco di Guarnieri"],
-        "description": "Minor Veneto vine of mysterious origin.",
-        "color": "black",
+        "synonyms": [
+            "Borgogna",
+            "Gattera",
+            "Refosco di Guarnieri"
+        ],
+        "description": {
+            "default": "Minor Veneto vine of mysterious origin.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tribidrag",
         "synonyms": [
             "Crljenak Kaštelanski",
             "Kratošija",
             "Morellone",
@@ -10795,65 +17208,98 @@
             "Primaticcio",
             "Primitivo",
             "Primitivo di Goia",
             "Primativo",
             "Trebidrag",
             "Uva di Corato",
             "Zagarese",
-            "Zinfandel",
+            "Zinfandel"
         ],
-        "description": "Croatian variety making full-bodied reds, much better known as Primitivo or Zinfandel.",
-        "color": "black",
+        "description": {
+            "default": "Croatian variety making full-bodied reds, much better known as Primitivo or Zinfandel.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Trincadeira",
         "synonyms": [
             "Black Alicante",
             "Black Portugal",
             "Crato Preto",
             "Mortagua",
             "Mortagua Preto",
             "Rosete Espalhado",
             "Tinta Amarela",
             "Tinta Amarelha",
             "Tinta Manuola",
             "Torneiro",
-            "Trincadeira Preta",
+            "Trincadeira Preta"
         ],
-        "description": "The dark-skinned, widely planted Trincadeira goes under many aliases throughout Portugal. Potentially high-quality reds but not easy to grow.",
-        "color": "black",
+        "description": {
+            "default": "The dark-skinned, widely planted Trincadeira goes under many aliases throughout Portugal. Potentially high-quality reds but not easy to grow.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Trincadeira Das Pratas",
-        "synonyms": ["Arinto Gordo", "Boal Prior"],
-        "description": "Underrated aromatic variety from central Portugal.",
-        "color": "white",
+        "synonyms": [
+            "Arinto Gordo",
+            "Boal Prior"
+        ],
+        "description": {
+            "default": "Underrated aromatic variety from central Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Triomphe",
         "synonyms": [
             "Kuhlmann 319-1",
             "Triomphe d’Alsace",
             "Triumpf vom Elsass",
-            "Triumph d’Alsace",
+            "Triumph d’Alsace"
         ],
-        "description": "Slightly foxy-tasting red hybrid planted mainly in the UK.",
-        "color": "black",
+        "description": {
+            "default": "Slightly foxy-tasting red hybrid planted mainly in the UK.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Trnjak",
-        "synonyms": ["Rudežuša", "Trnjak Crni"],
-        "description": "Minor variety found in both Croatia and Bosnia-Herzegovina.",
-        "color": "black",
+        "synonyms": [
+            "Rudežuša",
+            "Trnjak Crni"
+        ],
+        "description": {
+            "default": "Minor variety found in both Croatia and Bosnia-Herzegovina.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tronto",
-        "synonyms": ["Aglianico di Napoli", "Tronta"],
-        "description": "Possibly an Aglianico relative from around Amalfi in Campania.",
-        "color": "black",
+        "synonyms": [
+            "Aglianico di Napoli",
+            "Tronta"
+        ],
+        "description": {
+            "default": "Possibly an Aglianico relative from around Amalfi in Campania.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Trousseau",
         "synonyms": [
             "Bastardo",
             "Bastardo",
             "Bastardhino",
@@ -10868,198 +17314,361 @@
             "Tintilla",
             "Tinta Lisboa",
             "Troussé",
             "Trousseau Noir",
             "Troussot",
             "Verdejo",
             "Verdejo Negro",
-            "Verdejo Tinto",
+            "Verdejo Tinto"
         ],
-        "description": "Demanding variety making powerful, ageworthy wines and having a complex geographical distribution and many aliases, including Bastardo.",
-        "color": "black",
+        "description": {
+            "default": "Demanding variety making powerful, ageworthy wines and having a complex geographical distribution and many aliases, including Bastardo.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tsimlyansky Cherny",
-        "synonyms": ["Tsimlyansky"],
-        "description": "Convincing, if rather tannic, Russian variety used to make various styles of red.",
-        "color": "black",
+        "synonyms": [
+            "Tsimlyansky"
+        ],
+        "description": {
+            "default": "Convincing, if rather tannic, Russian variety used to make various styles of red.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Tsitska",
-        "synonyms": ["Shanti", "Tsitsiko"],
-        "description": "High-acid Georgian variety used to make still and sparkling wines.",
-        "color": "white",
+        "synonyms": [
+            "Shanti",
+            "Tsitsiko"
+        ],
+        "description": {
+            "default": "High-acid Georgian variety used to make still and sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Tsolikouri",
-        "synonyms": ["Melqos Tsolikouri", "Obchuri Tsolikouri", "Tsolikoouri"],
-        "description": "Versatile, widely planted Georgian variety.",
-        "color": "white",
+        "synonyms": [
+            "Melqos Tsolikouri",
+            "Obchuri Tsolikouri",
+            "Tsolikoouri"
+        ],
+        "description": {
+            "default": "Versatile, widely planted Georgian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Tsulukidzis Tetra",
-        "synonyms": ["Rachuli Tetra", "Racthuli Tetri", "Tsulukidze Tetra"],
-        "description": "Minor but productive Georgian variety making both dry and sweet whites.",
-        "color": "white",
+        "synonyms": [
+            "Rachuli Tetra",
+            "Racthuli Tetri",
+            "Tsulukidze Tetra"
+        ],
+        "description": {
+            "default": "Minor but productive Georgian variety making both dry and sweet whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Turán",
-        "synonyms": ["Agria", "Bikavér 13", "Eger 208"],
-        "description": "Dark-skinned, red-fleshed Hungarian variety valued mainly for its colour.",
-        "color": "black",
+        "synonyms": [
+            "Agria",
+            "Bikavér 13",
+            "Eger 208"
+        ],
+        "description": {
+            "default": "Dark-skinned, red-fleshed Hungarian variety valued mainly for its colour.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Usakhelouri",
-        "synonyms": ["Okhureshuli", "Okourechouli"],
-        "description": "Georgian variety producing semi-sweet, aromatic reds.",
-        "color": "black",
+        "synonyms": [
+            "Okhureshuli",
+            "Okourechouli"
+        ],
+        "description": {
+            "default": "Georgian variety producing semi-sweet, aromatic reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Uva Della Cascina",
-        "synonyms": ["Uva Cascina"],
-        "description": "Rare, perfumed, recently rescued Oltrepò Pavese variety.",
-        "color": "black",
+        "synonyms": [
+            "Uva Cascina"
+        ],
+        "description": {
+            "default": "Rare, perfumed, recently rescued Oltrepò Pavese variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Uva Longanesi",
-        "synonyms": ["Bursôn", "Longanesi", "Negretto Longanesi"],
-        "description": "Hardy Emilia-Romagnan named after the family that rescued it.",
-        "color": "black",
+        "synonyms": [
+            "Bursôn",
+            "Longanesi",
+            "Negretto Longanesi"
+        ],
+        "description": {
+            "default": "Hardy Emilia-Romagnan named after the family that rescued it.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Uva Tosca",
-        "synonyms": ["Montanara"],
-        "description": "Minor Emilia-Romagnan variety that has moved downhill.",
-        "color": "black",
+        "synonyms": [
+            "Montanara"
+        ],
+        "description": {
+            "default": "Minor Emilia-Romagnan variety that has moved downhill.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Uvalino",
-        "synonyms": ["Cunaiola", "Freisone", "Lambrusca", "Lambruschino"],
-        "description": "Recently resurrected Piemontese.",
-        "color": "black",
+        "synonyms": [
+            "Cunaiola",
+            "Freisone",
+            "Lambrusca",
+            "Lambruschino"
+        ],
+        "description": {
+            "default": "Recently resurrected Piemontese.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Váh",
-        "synonyms": ["CAAB 3/13"],
-        "description": "Recently authorized Slovakian cross that needs a good site to prosper.",
-        "color": "black",
+        "synonyms": [
+            "CAAB 3/13"
+        ],
+        "description": {
+            "default": "Recently authorized Slovakian cross that needs a good site to prosper.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Valdiguié",
-        "synonyms": ["Cot de Cheragas", "Gros Auxerrois", "Valdiguier"],
-        "description": "High-yielding rather ordinary variety from south-west France once popular in southern France and California but now in continuing decline.",
-        "color": "black",
+        "synonyms": [
+            "Cot de Cheragas",
+            "Gros Auxerrois",
+            "Valdiguier"
+        ],
+        "description": {
+            "default": "High-yielding rather ordinary variety from south-west France once popular in southern France and California but now in continuing decline.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Valentino Nero",
-        "synonyms": ["Incrocio Dalmasso 16/8"],
-        "description": "Very minor Veneto cross whose true parentage has only recently been revealed.",
-        "color": "black",
+        "synonyms": [
+            "Incrocio Dalmasso 16/8"
+        ],
+        "description": {
+            "default": "Very minor Veneto cross whose true parentage has only recently been revealed.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Valiant",
         "synonyms": [
             "South Dakota 72S15",
             "South Dakota NF7-121",
-            "South Dakota SD7-121",
+            "South Dakota SD7-121"
         ],
-        "description": "Very winter-hardy, foxy American hybrid best suited to juice, jelly and the table.",
-        "color": "black",
+        "description": {
+            "default": "Very winter-hardy, foxy American hybrid best suited to juice, jelly and the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Van Buren",
-        "synonyms": ["Gladwin 3000"],
-        "description": "Old, low-acid American hybrid used mostly for the table.",
-        "color": "black",
+        "synonyms": [
+            "Gladwin 3000"
+        ],
+        "description": {
+            "default": "Old, low-acid American hybrid used mostly for the table.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vandal-Cliche",
         "synonyms": [
             "Cliche",
             "Cliche 8414",
             "Cliche Blanc",
             "Vandal 84-14",
             "Vandal Blanc",
-            "Vandal Cliche",
+            "Vandal Cliche"
         ],
-        "description": "Hardy Canadian complex hybrid used for a wide range of wine styles.",
-        "color": "white",
+        "description": {
+            "default": "Hardy Canadian complex hybrid used for a wide range of wine styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vasilaki",
-        "synonyms": ["Altıntaş"],
-        "description": "Low-acid but potentially high-quality white wine grape from the Turkish island of Bozcaada.",
-        "color": "white",
+        "synonyms": [
+            "Altıntaş"
+        ],
+        "description": {
+            "default": "Low-acid but potentially high-quality white wine grape from the Turkish island of Bozcaada.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vb 91-26-4",
-        "synonyms": ["VB 91-26-04"],
-        "description": "Minor and usefully disease-resistant Swiss hybrid found to a very limited extent in northern Europe.",
-        "color": "black",
+        "synonyms": [
+            "VB 91-26-04"
+        ],
+        "description": {
+            "default": "Minor and usefully disease-resistant Swiss hybrid found to a very limited extent in northern Europe.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Verdea",
-        "synonyms": ["Colombana Bianca", "Colombana di Peccioli"],
-        "description": "Ancient Tuscan white, now a Lombardia speciality, used to make a range of wine styles.",
-        "color": "white",
+        "synonyms": [
+            "Colombana Bianca",
+            "Colombana di Peccioli"
+        ],
+        "description": {
+            "default": "Ancient Tuscan white, now a Lombardia speciality, used to make a range of wine styles.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdeca",
         "synonyms": [
             "Alvino Verde",
             "Lagorthi",
             "Verdera",
             "Verdicchio Femmina",
             "Verdisco Bianco",
             "Verdone",
-            "Vino Verde",
+            "Vino Verde"
         ],
-        "description": "Regarded as light, neutral and declining in Puglia but, as Lagorthi, in tantalizingly short supply in Greece.",
-        "color": "white",
+        "description": {
+            "default": "Regarded as light, neutral and declining in Puglia but, as Lagorthi, in tantalizingly short supply in Greece.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdejo",
         "synonyms": [
             "Albillo de Nava",
             "Botón de Gallo Blanco",
             "Verdeja",
-            "Verdejo Blanco",
+            "Verdejo Blanco"
         ],
-        "description": "High-quality, aromatic, rich, nutty variety most at home in Spain’s Rueda region.",
-        "color": "white",
+        "description": {
+            "default": "High-quality, aromatic, rich, nutty variety most at home in Spain’s Rueda region.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdejo Serrano",
-        "synonyms": ["Rufete Blanca"],
-        "description": "Almost extinct variety from the mountains of Salamanca province.",
-        "color": "white",
+        "synonyms": [
+            "Rufete Blanca"
+        ],
+        "description": {
+            "default": "Almost extinct variety from the mountains of Salamanca province.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdelho",
         "synonyms": [
             "Verdelho Branco",
             "Verdelho da Madeira",
             "Verdelho dos Açores",
             "Verdelho Pico",
-            "Verdello no Peluda Finca Natero",
+            "Verdello no Peluda Finca Natero"
         ],
-        "description": "Portuguese variety making fine, medium-dry wines on Madeira and full-bodied table wines in Australia and the Loire.",
-        "color": "white",
+        "description": {
+            "default": "Portuguese variety making fine, medium-dry wines on Madeira and full-bodied table wines in Australia and the Loire.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdello",
-        "synonyms": ["Verdetto"],
-        "description": "Waning high-acid Umbrian blending ingredient.",
-        "color": "white",
+        "synonyms": [
+            "Verdetto"
+        ],
+        "description": {
+            "default": "Waning high-acid Umbrian blending ingredient.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdesse",
-        "synonyms": ["Bian Ver", "Verdasse", "Verdèche", "Verdesse Musquée"],
-        "description": "Potentially high-quality, aromatic variety being replanted in Savoie.",
-        "color": "white",
+        "synonyms": [
+            "Bian Ver",
+            "Verdasse",
+            "Verdèche",
+            "Verdesse Musquée"
+        ],
+        "description": {
+            "default": "Potentially high-quality, aromatic variety being replanted in Savoie.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdicchio Bianco",
         "synonyms": [
             "Angelica",
             "Boschera",
             "Boschera Bianca",
@@ -11082,44 +17691,70 @@
             "Turbiano",
             "Turviana",
             "Verdetto",
             "Verdicchio Giallo",
             "Verdicchio Marchigiano",
             "Verdicchio Peloso",
             "Verdicchio Verde",
-            "Verdone",
+            "Verdone"
         ],
-        "description": "Famously associated with the Marche’s best-known dry white, this is probably originally from the Veneto, where it is also found, as Trebbiano di Soave. Wines can age.",
-        "color": "white",
+        "description": {
+            "default": "Famously associated with the Marche’s best-known dry white, this is probably originally from the Veneto, where it is also found, as Trebbiano di Soave. Wines can age.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verdiso",
-        "synonyms": ["Pedevenda", "Peverenda", "Pexerenda", "Verdino", "Verdise"],
-        "description": "Recuperated minor variety from the Colli Euganei in the Veneto makes wines from fizz to passito.",
-        "color": "white",
+        "synonyms": [
+            "Pedevenda",
+            "Peverenda",
+            "Pexerenda",
+            "Verdino",
+            "Verdise"
+        ],
+        "description": {
+            "default": "Recuperated minor variety from the Colli Euganei in the Veneto makes wines from fizz to passito.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verduzzo Friulano",
         "synonyms": [
             "Ramandolo",
             "Ramandolo Dorato",
             "Verdùç",
             "Verdùz",
             "Verdùzz",
             "Verduzzo di Ramandolo",
-            "Verduzzo Giallo",
+            "Verduzzo Giallo"
         ],
-        "description": "Ancient, characterful, sometimes astringent, Friulian; good sweet wines.",
-        "color": "white",
+        "description": {
+            "default": "Ancient, characterful, sometimes astringent, Friulian; good sweet wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Verduzzo Trevigiano",
-        "synonyms": ["Verduc", "Verduz", "Verduzzo di Motta"],
-        "description": "The other Verduzzo, generally inferior to and often blended with Verduzzo Friulano. Waning.",
-        "color": "white",
+        "synonyms": [
+            "Verduc",
+            "Verduz",
+            "Verduzzo di Motta"
+        ],
+        "description": {
+            "default": "The other Verduzzo, generally inferior to and often blended with Verduzzo Friulano. Waning.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vermentino",
         "synonyms": [
             "Favorita",
             "Furmentin",
             "Garbesso",
@@ -11132,130 +17767,226 @@
             "Rollé",
             "Sapaiola",
             "Verlantin",
             "Varlantin",
             "Verlentin",
             "Varlentin",
             "Vermentino di Gallura",
-            "Vermentinu",
+            "Vermentinu"
         ],
-        "description": "Aromatic, crisp high-quality variety flourishing near the sea in northern Italy, southern France and on the islands of Corse and Sardegna.",
-        "color": "white",
+        "description": {
+            "default": "Aromatic, crisp high-quality variety flourishing near the sea in northern Italy, southern France and on the islands of Corse and Sardegna.",
+            "julie": "Known as Rolle in the region of Provence and Corsica in France, Vermentino is an aromatic variety widely grown in Liguria and Sardinia in Italy. Vermentino displays aromas of white flowers, citrus and mediterranean herbs as well as a characteristic bitter almond aftertaste.",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vernaccia Di Oristano",
         "synonyms": [
             "Aregu Biancu",
             "Aregu Seulu",
             "Cranaccia",
             "Garnaccia",
             "Granaccia",
             "Granazza",
             "Varnaccia",
             "Vernaccia",
             "Vernaccia Austera",
             "Vernaccia Orosei",
-            "Vernaccia S. Rosalia",
+            "Vernaccia S. Rosalia"
         ],
-        "description": "Makes complex sherry-like wines on Sardegna.",
-        "color": "white",
+        "description": {
+            "default": "Makes complex sherry-like wines on Sardegna.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vernaccia Di San Gimignano",
-        "synonyms": ["Bervedino", "Piccabòn", "Vernaccia"],
-        "description": "Refreshing and generally light variety from the Tuscan town with the towers. Potential for high-quality wine.",
-        "color": "white",
+        "synonyms": [
+            "Bervedino",
+            "Piccabòn",
+            "Vernaccia"
+        ],
+        "description": {
+            "default": "Refreshing and generally light variety from the Tuscan town with the towers. Potential for high-quality wine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Versoaln",
-        "synonyms": ["Versailler", "Weiss Versoalen", "Weisser Versailler"],
-        "description": "Recent burgeoning based on a single, ancient Alto Adige giant vine.",
-        "color": "white",
+        "synonyms": [
+            "Versailler",
+            "Weiss Versoalen",
+            "Weisser Versailler"
+        ],
+        "description": {
+            "default": "Recent burgeoning based on a single, ancient Alto Adige giant vine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vertzami",
         "synonyms": [
             "Deykaditiko",
             "Lefkada",
             "Lefkaditiko",
             "Lefkas",
             "Marzavi",
-            "Vartzami",
+            "Vartzami"
         ],
-        "description": "Promising Greek variety that produces deeply coloured, powerful, very tannic wines.",
-        "color": "black",
+        "description": {
+            "default": "Promising Greek variety that produces deeply coloured, powerful, very tannic wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vespaiola",
-        "synonyms": ["Bresparola"],
-        "description": "Speciality of Vicenza, associated with sweet whites.",
-        "color": "white",
+        "synonyms": [
+            "Bresparola"
+        ],
+        "description": {
+            "default": "Speciality of Vicenza, associated with sweet whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vespolina",
-        "synonyms": ["Ughetta", "Uvetta di Canneto"],
-        "description": "Low-yielding, minor Nebbiolo relative of Gattinara that is currently losing ground.",
-        "color": "black",
+        "synonyms": [
+            "Ughetta",
+            "Uvetta di Canneto"
+        ],
+        "description": {
+            "default": "Low-yielding, minor Nebbiolo relative of Gattinara that is currently losing ground.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vidal",
-        "synonyms": ["Vidal Blanc", "Vidal 256"],
-        "description": "French hybrid ideally suited to the production of sweet Canadian icewine.",
-        "color": "white",
+        "synonyms": [
+            "Vidal Blanc",
+            "Vidal 256"
+        ],
+        "description": {
+            "default": "French hybrid ideally suited to the production of sweet Canadian icewine.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vidiano",
-        "synonyms": ["Abidano", "Abidiano", "Abudiano", "Avidiano", "Bidiano"],
-        "description": "Old Greek variety showing signs of a revival on Kríti (Crete).",
-        "color": "white",
+        "synonyms": [
+            "Abidano",
+            "Abidiano",
+            "Abudiano",
+            "Avidiano",
+            "Bidiano"
+        ],
+        "description": {
+            "default": "Old Greek variety showing signs of a revival on Kríti (Crete).",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vien De Nus",
-        "synonyms": ["Gros Rouge", "Gros Vien", "Oriou Gros"],
-        "description": "Minor Aostan with relatives elsewhere. Wine is always blended.",
-        "color": "black",
+        "synonyms": [
+            "Gros Rouge",
+            "Gros Vien",
+            "Oriou Gros"
+        ],
+        "description": {
+            "default": "Minor Aostan with relatives elsewhere. Wine is always blended.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vignoles",
-        "synonyms": ["Ravat 51"],
-        "description": "French hybrid better known in the United States, mostly for sweeter wines.",
-        "color": "white",
+        "synonyms": [
+            "Ravat 51"
+        ],
+        "description": {
+            "default": "French hybrid better known in the United States, mostly for sweeter wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vijariego",
         "synonyms": [
             "Bujariego",
             "Diego",
             "Verijadiego Blanco",
             "Vijariego Blanco",
             "Vijiriega Blanca",
             "Vijiriega Común",
             "Vijiriego",
-            "Vujariego",
+            "Vujariego"
         ],
-        "description": "Minor variety found mainly on the Islas Canarias, used for both still and sparkling wines.",
-        "color": "white",
+        "description": {
+            "default": "Minor variety found mainly on the Islas Canarias, used for both still and sparkling wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vilana",
-        "synonyms": ["Velana"],
-        "description": "The grape of Kríti (Crete) produces fresh, lightly floral whites.",
-        "color": "white",
+        "synonyms": [
+            "Velana"
+        ],
+        "description": {
+            "default": "The grape of Kríti (Crete) produces fresh, lightly floral whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Villard Blanc",
-        "synonyms": ["Seyve-Villard 12-375", "SV 12-375"],
-        "description": "Light-skinned French hybrid in decline but still quite widely scattered round the globe.",
-        "color": "white",
+        "synonyms": [
+            "Seyve-Villard 12-375",
+            "SV 12-375"
+        ],
+        "description": {
+            "default": "Light-skinned French hybrid in decline but still quite widely scattered round the globe.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vincent",
-        "synonyms": ["Vineland 49431", "V 49431"],
-        "description": "Hardy North American hybrid bred in Canada for cold climates.",
-        "color": "black",
+        "synonyms": [
+            "Vineland 49431",
+            "V 49431"
+        ],
+        "description": {
+            "default": "Hardy North American hybrid bred in Canada for cold climates.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vinhão",
         "synonyms": [
             "Espadeiro Basto",
             "Espadeiro da Tinta",
             "Espadeiro Preto",
@@ -11267,124 +17998,217 @@
             "Sousão Forte",
             "Sousón",
             "Souzao",
             "Souzão",
             "Tinta Nacional",
             "Tinta País",
             "Tinto de Parada",
-            "Tinto Nacional",
+            "Tinto Nacional"
         ],
-        "description": "High-acid, highly distinctive Portuguese variety making rustic, deeply coloured wines in north-west Iberia.",
-        "color": "black",
+        "description": {
+            "default": "High-acid, highly distinctive Portuguese variety making rustic, deeply coloured wines in north-west Iberia.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Viognier",
-        "synonyms": ["Viogné", "Vionnier", "Viognier Jaune", "Viognier Vert"],
-        "description": "Headily aromatic variety making particularly full-bodied whites – all over the world now.",
-        "color": "white",
+        "synonyms": [
+            "Viogné",
+            "Vionnier",
+            "Viognier Jaune",
+            "Viognier Vert"
+        ],
+        "description": {
+            "default": "Headily aromatic variety making particularly full-bodied whites – all over the world now.",
+            "julie": "Aromatic grape varieties from the Northern Rhône which was nearly extinct in the 1960s but is now planted all over the globe. Viognier wines tend to be full bodied, smooth, with aromas of apricot, violet and candied citrus. The best examples come from Condrieu AOC and the tiny, monopole AOC of Château Grillet. Viognier is also blended in small amounts with the Syrah grape, in Côte Rôtie AOC to add perfume to the wine and stabilise its colour. The grape is also found in the Southern Rhône, Languedoc-Roussillon, the Valais in Switzerland and most New World countries.",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Violento",
-        "synonyms": ["Violenti"],
-        "description": "Pink-skinned variety from the Greek island of Zákynthos used mostly in blends.",
-        "color": "pink",
+        "synonyms": [
+            "Violenti"
+        ],
+        "description": {
+            "default": "Pink-skinned variety from the Greek island of Zákynthos used mostly in blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "pink"
     },
     {
         "name": "Vital",
-        "synonyms": ["Boal Bonifacio", "Malvasia Corada", "Malvasia Fina do Douro"],
-        "description": "Low-acid variety grown mainly in central Portugal.",
-        "color": "white",
+        "synonyms": [
+            "Boal Bonifacio",
+            "Malvasia Corada",
+            "Malvasia Fina do Douro"
+        ],
+        "description": {
+            "default": "Low-acid variety grown mainly in central Portugal.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vitovska",
-        "synonyms": ["Vitouska"],
-        "description": "Makes rare but high-quality white in the Italy–Slovenia border region around Trieste.",
-        "color": "white",
+        "synonyms": [
+            "Vitouska"
+        ],
+        "description": {
+            "default": "Makes rare but high-quality white in the Italy–Slovenia border region around Trieste.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vitovska Grganja",
-        "synonyms": ["Grganka", "Racuk", "Vitovska Garganija"],
-        "description": "Rare Slovenian white attracting increasing recognition.",
-        "color": "white",
+        "synonyms": [
+            "Grganka",
+            "Racuk",
+            "Vitovska Garganija"
+        ],
+        "description": {
+            "default": "Rare Slovenian white attracting increasing recognition.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vlachiko",
         "synonyms": [
             "Blachiko",
             "Blachos",
             "Vlachico de Jannina",
             "Vlachos",
             "Vlachs",
             "Vlacos",
             "Vlahico",
-            "Vlahos",
+            "Vlahos"
         ],
-        "description": "Greek variety that makes svelte, dark-fruited wines and deserves more attention.",
-        "color": "black",
+        "description": {
+            "default": "Greek variety that makes svelte, dark-fruited wines and deserves more attention.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vlaška",
-        "synonyms": ["Maraškina Velog Zrna", "Prejica", "Vezuljka", "Žutuja"],
-        "description": "Rare, low-acid Croatian variety found only in the area around Split.",
-        "color": "white",
+        "synonyms": [
+            "Maraškina Velog Zrna",
+            "Prejica",
+            "Vezuljka",
+            "Žutuja"
+        ],
+        "description": {
+            "default": "Rare, low-acid Croatian variety found only in the area around Split.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vlosh",
-        "synonyms": ["Vloshi", "Vlosk"],
-        "description": "Dark-skinned Albanian variety in decline.",
-        "color": "black",
+        "synonyms": [
+            "Vloshi",
+            "Vlosk"
+        ],
+        "description": {
+            "default": "Dark-skinned Albanian variety in decline.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Voskeat",
         "synonyms": [
             "Hardzhi",
             "Kanacicheni",
             "Katviacik",
             "Khardji",
             "Kharji",
             "Pishik Gezi",
             "Pscigi",
             "Voskeate",
             "Voskehat",
-            "Xardji",
+            "Xardji"
         ],
-        "description": "Productive old Armenian variety used mostly for fortified whites.",
-        "color": "white",
+        "description": {
+            "default": "Productive old Armenian variety used mostly for fortified whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Vranac",
-        "synonyms": ["Vranac Crmnichki", "Vranac Crni", "Vranac Prhljavac", "Vranec"],
-        "description": "Balkan variety capable of producing powerful, high-quality, ageworthy reds.",
-        "color": "black",
+        "synonyms": [
+            "Vranac Crmnichki",
+            "Vranac Crni",
+            "Vranac Prhljavac",
+            "Vranec"
+        ],
+        "description": {
+            "default": "Balkan variety capable of producing powerful, high-quality, ageworthy reds.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Vugava",
-        "synonyms": ["Bugava", "Ugava", "Viškulja", "Vugava Bijela"],
-        "description": "High-quality, aromatic variety found on the Croatian island of Vis.",
-        "color": "white",
+        "synonyms": [
+            "Bugava",
+            "Ugava",
+            "Viškulja",
+            "Vugava Bijela"
+        ],
+        "description": {
+            "default": "High-quality, aromatic variety found on the Croatian island of Vis.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Würzer",
-        "synonyms": ["Alzey 10487"],
-        "description": "Declining, perfumed German cross best in small doses.",
-        "color": "white",
+        "synonyms": [
+            "Alzey 10487"
+        ],
+        "description": {
+            "default": "Declining, perfumed German cross best in small doses.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Xarello",
         "synonyms": [
             "Cartoixà",
             "Pansa Blanca",
             "Pansal",
             "Premsal Blanca",
             "Xarel-lo",
             "Xarel·lo",
-            "Xerello",
+            "Xerello"
         ],
-        "description": "High-quality Catalan with a strong personality making firm wines both still and sparkling.",
-        "color": "white",
+        "description": {
+            "default": "High-quality Catalan with a strong personality making firm wines both still and sparkling.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Xinomavro",
         "synonyms": [
             "Csinomavro",
             "Mavro",
             "Mavro Naoussis",
@@ -11402,18 +18226,22 @@
             "Popolka",
             "Xinogaltso",
             "Xynomavro Bolgar",
             "Xynomavro Naoussis",
             "Xynomavro of Náoussa",
             "Xynomavron",
             "Zinomavro",
-            "Zynomavro",
+            "Zynomavro"
         ],
-        "description": "Top-quality, widely planted but pernickety, high-acid Greek variety.",
-        "color": "black",
+        "description": {
+            "default": "Top-quality, widely planted but pernickety, high-acid Greek variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Xynisteri",
         "synonyms": [
             "Aspro Kyprou",
             "Cipro Bianco",
             "Hebron Blanc",
@@ -11421,157 +18249,281 @@
             "Hibron Blanc",
             "Koumantaria",
             "Lefko Kyprou",
             "Lefko Kyproy",
             "Topiko Aspro",
             "Xinisteri",
             "Xynistera",
-            "Xynisteri Aspro Kyprou",
+            "Xynisteri Aspro Kyprou"
         ],
-        "description": "Widely planted Cypriot variety capable of making fresh, citrusy whites.",
-        "color": "white",
+        "description": {
+            "default": "Widely planted Cypriot variety capable of making fresh, citrusy whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Yamabudo",
-        "synonyms": ["Crimson Glory Vine", "Meoru"],
-        "description": "Member of an Asian vine species producing fresh, leafy wines in Japan.",
-        "color": "red",
+        "synonyms": [
+            "Crimson Glory Vine",
+            "Meoru"
+        ],
+        "description": {
+            "default": "Member of an Asian vine species producing fresh, leafy wines in Japan.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "red"
     },
     {
         "name": "Yapincak",
-        "synonyms": ["Erkek Yapıncak", "Kınalı Yapıncak", "Yapakak", "Yapındjac"],
-        "description": "Minor Turkish variety grown on the north coast of the Sea of Marmara.",
-        "color": "white",
+        "synonyms": [
+            "Erkek Yapıncak",
+            "Kınalı Yapıncak",
+            "Yapakak",
+            "Yapındjac"
+        ],
+        "description": {
+            "default": "Minor Turkish variety grown on the north coast of the Sea of Marmara.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Začinak",
-        "synonyms": ["Krajinsko Crno", "Negotinsko Crno", "Zachinak", "Zazinak"],
-        "description": "Serbian variety contributing colour to red blends.",
-        "color": "black",
+        "synonyms": [
+            "Krajinsko Crno",
+            "Negotinsko Crno",
+            "Zachinak",
+            "Zazinak"
+        ],
+        "description": {
+            "default": "Serbian variety contributing colour to red blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Zakynthino",
-        "synonyms": ["Zachara", "Zacharo", "Zakinthino"],
-        "description": "Ancient Greek island variety being modestly revived.",
-        "color": "white",
+        "synonyms": [
+            "Zachara",
+            "Zacharo",
+            "Zakinthino"
+        ],
+        "description": {
+            "default": "Ancient Greek island variety being modestly revived.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zalagyöngye",
         "synonyms": [
             "Ecs-24",
             "Egri Csillagok 24",
             "Pearl of Zala",
             "Zala Dende",
-            "Zhemchug Zala",
+            "Zhemchug Zala"
         ],
-        "description": "High-yielding, widely planted Hungarian hybrid producing generally inferior wines.",
-        "color": "white",
+        "description": {
+            "default": "High-yielding, widely planted Hungarian hybrid producing generally inferior wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zalema",
-        "synonyms": ["Del Pipajo", "Rebazo", "Salemo", "Zalemo"],
-        "description": "Southern Spanish variety that is light in every way and used to make fortified wines.",
-        "color": "white",
+        "synonyms": [
+            "Del Pipajo",
+            "Rebazo",
+            "Salemo",
+            "Zalemo"
+        ],
+        "description": {
+            "default": "Southern Spanish variety that is light in every way and used to make fortified wines.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Žametovka",
         "synonyms": [
             "Bettlertraube",
             "Blauer Hainer",
             "Blauer Kölner",
             "Kapcina",
             "Kavčina Crna",
             "Kölner Blau",
             "Modra Kavčina",
             "Plava Velica",
             "Žametasta Črnina",
-            "Žametna Črnina",
+            "Žametna Črnina"
         ],
-        "description": "Ancient dark-skinned Slovenian variety traditionally goes into the tart local Cviček but also has a claim as oldest vine in the world.",
-        "color": "black",
+        "description": {
+            "default": "Ancient dark-skinned Slovenian variety traditionally goes into the tart local Cviček but also has a claim as oldest vine in the world.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "black"
     },
     {
         "name": "Zefír",
-        "synonyms": ["Badacsony 2", "Zephyr"],
-        "description": "Recent Hungarian cross of uncertain parentage yet to establish a track record.",
-        "color": "grey",
+        "synonyms": [
+            "Badacsony 2",
+            "Zephyr"
+        ],
+        "description": {
+            "default": "Recent Hungarian cross of uncertain parentage yet to establish a track record.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "grey"
     },
     {
         "name": "Zengő",
-        "synonyms": ["Badachon 8", "Badacsony 8"],
-        "description": "Hungarian cross making full-bodied, high-quality whites if handled carefully.",
-        "color": "white",
+        "synonyms": [
+            "Badachon 8",
+            "Badacsony 8"
+        ],
+        "description": {
+            "default": "Hungarian cross making full-bodied, high-quality whites if handled carefully.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zéta",
-        "synonyms": ["Oremus"],
-        "description": "Renamed daughter of Furmint used mainly in sweet Tokaji blends.",
-        "color": "white",
+        "synonyms": [
+            "Oremus"
+        ],
+        "description": {
+            "default": "Renamed daughter of Furmint used mainly in sweet Tokaji blends.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zeusz",
-        "synonyms": ["Badacsony 10"],
-        "description": "Hungarian cross making full-bodied but well-balanced late-harvest whites.",
-        "color": "white",
+        "synonyms": [
+            "Badacsony 10"
+        ],
+        "description": {
+            "default": "Hungarian cross making full-bodied but well-balanced late-harvest whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zghihară De Huşi",
         "synonyms": [
             "Ghihară",
             "Poamă Zosănească",
             "Sghigardă Galbenă",
             "Zghihară",
             "Zghihară Galbenă",
-            "Zghihară Verde Bătută",
+            "Zghihară Verde Bătută"
         ],
-        "description": "Old Romanian variety producing crisp, easy-drinking whites.",
-        "color": "white",
+        "description": {
+            "default": "Old Romanian variety producing crisp, easy-drinking whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zierfandler",
         "synonyms": [
             "Cirfandli",
             "Gumpoldskirchner",
             "Roter Zierfandler",
             "Rubiner",
             "Spätrot",
-            "Zierfandler Rot",
+            "Zierfandler Rot"
         ],
-        "description": "Thermenregion speciality making powerful, aromatic and highly distinctive wines, typically in partnership with Rotgipfler.",
-        "color": "pink",
+        "description": {
+            "default": "Thermenregion speciality making powerful, aromatic and highly distinctive wines, typically in partnership with Rotgipfler.",
+            "julie": "",
+            "sommelier": "The indigenous Zierfandler is a curiosity found in the Thermenregion (Lower Austria), and derives from Roter Veltliner and a second, unknown parentage, that is thought to liken Traminer. Zierfandler is traditionally blended with Rotgipfler, and vinified as 'Spätrot-Rotgipfler', either as a blend of the two varieties after fermentation, or if planted together in the vineyard, as a mixture. When the grapes are well ripened, the wines are characterised by extract, a pleasant acidity and delicate floral notes. Trockenbeeren-auslese displays a honey-like bouquet that can be complemented by mineral notes. Prädikatswein from this variety has excellent storage potential."
+        },
+        "color": "pink"
     },
     {
         "name": "Žilavka",
-        "synonyms": ["Jilavka", "Mostarska", "Mostarska Zilavka"],
-        "description": "Herzegovina’s most famous variety, producing full-bodied but nutty, well-balanced, high-quality whites.",
-        "color": "white",
+        "synonyms": [
+            "Jilavka",
+            "Mostarska",
+            "Mostarska Zilavka"
+        ],
+        "description": {
+            "default": "Herzegovina’s most famous variety, producing full-bodied but nutty, well-balanced, high-quality whites.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Žlahtina",
         "synonyms": [
             "Vrbnička Žlahtina",
             "Žlahtina Bijela",
             "Žlahtina Toljani",
-            "Žlajtina",
+            "Žlajtina"
         ],
-        "description": "High-yielding, minor Croatian variety currently being re-evaluated and benefiting from an enthusiastic local market.",
-        "color": "white",
+        "description": {
+            "default": "High-yielding, minor Croatian variety currently being re-evaluated and benefiting from an enthusiastic local market.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zlatarica Vrgorska",
         "synonyms": [
             "Bila loza",
             "Dračkinja",
             "Plavka",
             "Zlatarica",
-            "Zlatarica Bijela",
+            "Zlatarica Bijela"
         ],
-        "description": "Very rare Croatian variety.",
-        "color": "white",
+        "description": {
+            "default": "Very rare Croatian variety.",
+            "julie": "",
+            "sommelier": ""
+        },
+        "color": "white"
     },
     {
         "name": "Zweigelt",
-        "synonyms": ["Blauer Zweigelt", "Rotburger", "Zweigeltrebe"],
-        "description": "Most common red wine grape in Austria producing firm, full-bodied wines if yields are controlled.",
-        "color": "black",
-    },
-]
+        "synonyms": [
+            "Blauer Zweigelt",
+            "Rotburger",
+            "Zweigeltrebe"
+        ],
+        "description": {
+            "default": "Most common red wine grape in Austria producing firm, full-bodied wines if yields are controlled.",
+            "julie": "Zweigelt is the most planted red grape variety in Austria. It was obtained in 1922 by Fritz Zweigelt by crossing two other grape varieties : Blaufränkisch and Sankt Laurent. Zweigelt produces wines which are violet red when young and express aromas of purple berries. If yields are kept low, the wines can be full-bodied and long-lived. ",
+            "sommelier": ""
+        },
+        "color": "red"
+    },
+    {
+        "name": "Rondinella",
+        "synonyms": [
+            "Rondinela"
+        ],
+        "description": {
+            "default": "Rondinella is an Italian red-wine grape variety that most commonly appears in the blended wines of Valpolicella and Bardolino. Rarely grown outside the Veneto region, Rondinella's key attribute is its prolific and reliable yields. However, this attribute rarely equates to good quality and, consequently, Rondinella is hardly ever produced as a varietal wine. Rather, it is used to add herbal flavors to Corvina-based wines and to flesh out the blend.",
+            "julie": "Rondinella is mostly grown in the Veneto region of Italy for the production of of Bardolino and Valpolicella wines. Rondinella produces fruity, cherry flavoured wines but is never sold as a single varietal and always blended with Corvina and Molinara.",
+            "sommelier": ""
+        },
+        "color": "red"
+    }
+]
```

### Comparing `sommify-0.8.9/sommify/pynotesandhints/__init__.py` & `sommify-0.9.0/sommify/pynotesandhints/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/pynotesandhints/data.py` & `sommify-0.9.0/sommify/pynotesandhints/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/pyregion/__init__.py` & `sommify-0.9.0/sommify/pyregion/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from collections import namedtuple
 
 from thefuzz import fuzz, process
 
 from .data import regions as data
 
-flatten = lambda l: [item for sublist in l for item in sublist]
+
+def flatten(l : list) -> list:
+    return [item for sublist in l for item in sublist]
 
 # create a namedtuple
 Region = namedtuple(
     "Region",
     [
         "name",
         "synonyms",
         "parent",
         "subregions",
         "country",
+        "description"
     ],
 )
 
 
-def get_subregions(branch):
+def get_subregions(branch : dict) -> list:
     obj = Region(
         name=branch["name"],
         synonyms=branch.get("synonyms", []),
         parent=branch.get("parent", None),
-        subregions=list(map(lambda x: x["name"], branch.get("subregions", []))),
+        subregions=[x["name"] for x in branch.get("subregions", [])],
         country=branch["country"],
+        description=branch.get("description", None),
     )
 
     return [
         obj,
         *flatten(
             [
                 get_subregions(
@@ -44,91 +48,91 @@
         ),
     ]
 
 
 class ExistingRegions:
     __slots__ = ["regions", "region_tree", "_synonym_to_name"]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.regions = sorted(
             flatten([get_subregions(branch) for branch in data]),
             key=lambda x: x.name,
         )
         self.region_tree = data
         self._synonym_to_name = {}
         for region in self.regions:
             self._synonym_to_name[region.name] = region.name
             for synonym in region.synonyms:
                 self._synonym_to_name[synonym] = region.name
 
-    def __getitem__(self, key):
+    def __getitem__(self, key : str) -> Region:
         return self.regions[key]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.regions)
 
-    def __iter__(self):
+    def __iter__(self) -> Region:
         yield from self.regions
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"ExistingRegions({self.regions})"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"ExistingRegions({self.regions})"
 
     def get(self, **kwargs):
         for region in self.regions:
             if all(getattr(region, key) == value for key, value in kwargs.items()):
                 return region
 
-    def flatten_branch(self, branch):
+    def flatten_branch(self, branch : dict) -> list:
         return [
             self.get(name=branch["name"]),
             *flatten(
                 [
                     self.flatten_branch(subregion)
                     for subregion in branch.get("subregions", [])
                 ]
             ),
         ]
 
-    def find_branch(self, name, branch=None):
+    def find_branch(self, name : str, branch : object = None) -> object:
         if branch == None:
             branch = self.region_tree
 
         for region in branch:
             if region["name"] == name:
                 return region
 
             res = self.find_branch(name, region.get("subregions", []))
 
             if res != None:
                 return res
 
         return None
 
-    def get_descendants(self, region):
+    def get_descendants(self, region : object) -> list:
         branch = self.find_branch(region if isinstance(region, str) else region.name)
 
         if branch == None:
             return []
 
         return self.flatten_branch(branch)[1:]
 
-    def search_fuzzy(self, name, threshold=82):
+    def search_fuzzy(self, name : str, threshold: int =82) -> Region:
         name, distance = process.extractOne(
             name, self._synonym_to_name.keys(), scorer=fuzz.QRatio
         )
 
         if distance < threshold:
             return None
 
         return self.get(name=self._synonym_to_name[name])
 
-    def find_closest_geo(self, region, subset=None):
+    def find_closest_geo(self, region : str, subset: object=None) -> list:
         """Find geographically closest region to name in subset. Ordering of closeness is:
         0. regions that are children of name
         1. regions that are siblings of name (same parent)
         2. regions that are cousins of name (same grandparent)
         ...
         N. same country
         """
```

### Comparing `sommify-0.8.9/sommify/recipes/__init__.py` & `sommify-0.9.0/sommify/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/recipes/elastic.py` & `sommify-0.9.0/sommify/recipes/elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/recipes/reader.py` & `sommify-0.9.0/sommify/recipes/reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/tests/test_elastic.py` & `sommify-0.9.0/sommify/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/tests/test_prompts.py` & `sommify-0.9.0/sommify/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/sommify/tests/test_recipe_reader.py` & `sommify-0.9.0/sommify/tests/test_recipe_reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/.gitignore` & `sommify-0.9.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 *.DS_Store*
 token
+sommify/pygrape/data_backup.py
+sommify/pyregion/data_backup.py
 # C extensions
 *.so
 *test.ipynb
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `sommify-0.8.9/LICENSE` & `sommify-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sommify-0.8.9/pyproject.toml` & `sommify-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "sommify"
-version = "0.8.9"
+version = "0.9.0"
 authors = [
   { name="William Brach", email="william@sommify.ai" },
   { name="Tomas Bedej", email="tomas@sommify.ai" },
 ]
 description = "A package for recipe parsing"
 dependencies = [
   "inflect==7.0.0",
```

### Comparing `sommify-0.8.9/PKG-INFO` & `sommify-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sommify
-Version: 0.8.9
+Version: 0.9.0
 Summary: A package for recipe parsing
 Author-email: William Brach <william@sommify.ai>, Tomas Bedej <tomas@sommify.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

