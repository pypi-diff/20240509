# Comparing `tmp/name_that_fucking_film-0.1.3.tar.gz` & `tmp/name_that_fucking_film-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_that_fucking_film-0.1.3.tar", max compression
+gzip compressed data, was "name_that_fucking_film-0.1.4.tar", max compression
```

## Comparing `name_that_fucking_film-0.1.3.tar` & `name_that_fucking_film-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1359 2024-05-09 19:08:20.531696 name_that_fucking_film-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.3/name_that_fucking_film/__init__.py
--rw-r--r--   0        0        0     6836 2024-05-09 19:30:55.679529 name_that_fucking_film-0.1.3/name_that_fucking_film/main.py
--rw-r--r--   0        0        0      397 2024-05-09 19:31:42.566200 name_that_fucking_film-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1359 2024-05-09 19:08:20.531696 name_that_fucking_film-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.4/name_that_fucking_film/__init__.py
+-rw-r--r--   0        0        0     6833 2024-05-09 19:34:21.600252 name_that_fucking_film-0.1.4/name_that_fucking_film/main.py
+-rw-r--r--   0        0        0      397 2024-05-09 19:33:55.274307 name_that_fucking_film-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.4/PKG-INFO
```

### Comparing `name_that_fucking_film-0.1.3/README.md` & `name_that_fucking_film-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `name_that_fucking_film-0.1.3/name_that_fucking_film/main.py` & `name_that_fucking_film-0.1.4/name_that_fucking_film/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     return distances[-1]
 
 
 def count_same_letters(s1, s2):
     return sum(min(s1.count(c), s2.count(c)) for c in set(s1 + s2))
 
 
-def read_swears_file(filepath=resources_path + "./resources/combined_file.txt"):
+def read_swears_file(filepath=resources_path + "/resources/combined_file.txt"):
     with open(filepath, 'r') as file:
         return file.read().splitlines()
 
 
-def get_meta_data(imdb_id, filepath=resources_path + "./resources/movie_meta_data.csv"):
+def get_meta_data(imdb_id, filepath=resources_path + "/resources/movie_meta_data.csv"):
     df = pd.read_csv(filepath)
     meta_data = df[df['imdbid'] == imdb_id]
     return meta_data
 
 
-def get_random_filepath(directory=resources_path + "./resources/raw_texts"):
+def get_random_filepath(directory=resources_path + "/resources/raw_texts"):
     files = os.listdir(directory)
     return os.path.join(directory, choice(files))
 
 
 def count_words(file_path, swear_words):
     with open(file_path, 'r') as file:
         content = file.read().lower().split()
```

### Comparing `name_that_fucking_film-0.1.3/PKG-INFO` & `name_that_fucking_film-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-that-fucking-film
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: jkarenko
 Author-email: juho.karenko@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

