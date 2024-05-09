# Comparing `tmp/name_that_fucking_film-0.1.0.tar.gz` & `tmp/name_that_fucking_film-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_that_fucking_film-0.1.0.tar", max compression
+gzip compressed data, was "name_that_fucking_film-0.1.1.tar", max compression
```

## Comparing `name_that_fucking_film-0.1.0.tar` & `name_that_fucking_film-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.808015 name_that_fucking_film-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.0/name_that_fucking_film/__init__.py
--rw-r--r--   0        0        0     6715 2024-05-09 18:46:47.831312 name_that_fucking_film-0.1.0/name_that_fucking_film/main.py
--rw-r--r--   0        0        0      397 2024-05-09 18:24:18.078871 name_that_fucking_film-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1359 2024-05-09 19:08:20.531696 name_that_fucking_film-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.1/name_that_fucking_film/__init__.py
+-rw-r--r--   0        0        0     6745 2024-05-09 19:08:46.419175 name_that_fucking_film-0.1.1/name_that_fucking_film/main.py
+-rw-r--r--   0        0        0      397 2024-05-09 19:09:30.021043 name_that_fucking_film-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.1/PKG-INFO
```

### Comparing `name_that_fucking_film-0.1.0/name_that_fucking_film/main.py` & `name_that_fucking_film-0.1.1/name_that_fucking_film/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,26 +24,26 @@
     return distances[-1]
 
 
 def count_same_letters(s1, s2):
     return sum(min(s1.count(c), s2.count(c)) for c in set(s1 + s2))
 
 
-def read_swears_file(filepath="./combined_file.txt"):
+def read_swears_file(filepath="./resources/combined_file.txt"):
     with open(filepath, 'r') as file:
         return file.read().splitlines()
 
 
-def get_meta_data(imdb_id, filepath="./movie_meta_data.csv"):
+def get_meta_data(imdb_id, filepath="./resources/movie_meta_data.csv"):
     df = pd.read_csv(filepath)
     meta_data = df[df['imdbid'] == imdb_id]
     return meta_data
 
 
-def get_random_filepath(directory="./raw_texts"):
+def get_random_filepath(directory="./resources/raw_texts"):
     files = os.listdir(directory)
     return os.path.join(directory, choice(files))
 
 
 def count_words(file_path, swear_words):
     with open(file_path, 'r') as file:
         content = file.read().lower().split()
```

