# Comparing `tmp/cvprocessor-0.0.26.tar.gz` & `tmp/cvprocessor-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.26.tar", last modified: Wed May  8 07:53:12 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.27.tar", last modified: Wed May  8 08:20:37 2024, max compression
```

## Comparing `cvprocessor-0.0.26.tar` & `cvprocessor-0.0.27.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:53:12.319484 cvprocessor-0.0.26/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.26/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-08 07:53:12.319069 cvprocessor-0.0.26/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.0.26/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 07:52:49.000000 cvprocessor-0.0.26/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 07:53:12.319560 cvprocessor-0.0.26/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:53:12.307947 cvprocessor-0.0.26/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:53:12.316301 cvprocessor-0.0.26/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.26/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.0.26/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.26/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     3503 2024-05-08 07:47:34.000000 cvprocessor-0.0.26/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.0.26/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.26/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.0.26/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3795 2024-05-08 07:11:28.000000 cvprocessor-0.0.26/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.0.26/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.0.26/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.0.26/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.0.26/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.0.26/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.0.26/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5799 2024-05-08 07:22:45.000000 cvprocessor-0.0.26/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:53:12.318639 cvprocessor-0.0.26/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-08 07:53:12.000000 cvprocessor-0.0.26/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      657 2024-05-08 07:53:12.000000 cvprocessor-0.0.26/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 07:53:12.000000 cvprocessor-0.0.26/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 07:53:12.000000 cvprocessor-0.0.26/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 07:53:12.000000 cvprocessor-0.0.26/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 08:20:37.188547 cvprocessor-0.0.27/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.27/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-08 08:20:37.187851 cvprocessor-0.0.27/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.0.27/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 08:19:52.000000 cvprocessor-0.0.27/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 08:20:37.188665 cvprocessor-0.0.27/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 08:20:37.170797 cvprocessor-0.0.27/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 08:20:37.183184 cvprocessor-0.0.27/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.27/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.0.27/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.27/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3761 2024-05-08 08:18:00.000000 cvprocessor-0.0.27/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.0.27/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4628 2024-05-08 08:19:15.000000 cvprocessor-0.0.27/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.0.27/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3795 2024-05-08 07:11:28.000000 cvprocessor-0.0.27/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.0.27/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.0.27/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.0.27/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.0.27/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.0.27/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.0.27/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5799 2024-05-08 07:22:45.000000 cvprocessor-0.0.27/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 08:20:37.187090 cvprocessor-0.0.27/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-08 08:20:37.000000 cvprocessor-0.0.27/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      657 2024-05-08 08:20:37.000000 cvprocessor-0.0.27/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 08:20:37.000000 cvprocessor-0.0.27/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 08:20:37.000000 cvprocessor-0.0.27/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 08:20:37.000000 cvprocessor-0.0.27/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.26/LICENSE` & `cvprocessor-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/PKG-INFO` & `cvprocessor-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.26
+Version: 0.0.27
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.26/README.md` & `cvprocessor-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/pyproject.toml` & `cvprocessor-0.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.26"
+version = "0.0.27"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.26/src/cvprocessor/authors.py` & `cvprocessor-0.0.27/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/cv.py` & `cvprocessor-0.0.27/src/cvprocessor/cv.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cvprocessor.software import Software
 from cvprocessor.institutes import Institutes
 from cvprocessor.news import News
 from cvprocessor.research_interests import ResearchInterests
 from cvprocessor.grants_awards import GrantsAwards
 from cvprocessor.teaching import Teaching
 from cvprocessor.supervision import Supervision
+from cvprocessor.experience import Experience
 
 
 class CV:
     def __init__(self, filename):
         self._filename = filename
         self._education = Education(self.filename)
         self._institutes = Institutes(self.filename)
@@ -26,14 +27,15 @@
         self._authors = Authors(self.filename, self)
         self._news = News(self.filename)
         self._publications = Publications(self.filename, self)
         self._research_interests = ResearchInterests(self.filename)
         self._grants_awards = GrantsAwards(self.filename)
         self._teaching = Teaching(self.filename)
         self._supervision = Supervision(self.filename, self)
+        self._experience = Experience(self.filename, self)
 
     @property
     def filename(self):
         return self._filename
 
     @property
     def intro(self):
@@ -78,31 +80,36 @@
     @property
     def teaching(self):
         return self._teaching
 
     @property
     def supervision(self):
         return self._supervision
+    
+    @property
+    def experience(self):
+        return self._experience
 
     def __str__(self):
         string = f"Education: {self.education}\n"
         string += f"Institutes: {self.institutes}\n"
         string += f"Software: {self.software}\n"
         string += f"Intro: {self.intro}\n"
         string += f"Authors: {self.authors}\n"
         string += f"News: {self.news}\n"
         string += f"Publications: {self.publications}\n"
         string += f"Research Interests: {self.research_interests}\n"
         string += f"Grants and Awards: {self.grants_awards}\n"
         string += f"Teaching: {self.teaching}\n"
         string += f"Supervision: {self.supervision}\n"
+        string += f"Experience: {self.experience}\n"
         return string
 
     def __repr__(self):
-        repr = f"CV(filename={self.filename}, education={self.education}, institutes={self.institutes}, software={self.software}, intro={self.intro}, authors={self.authors}, news={self.news}, publications={self.publications}, research_interests={self.research_interests}, grants_awards={self.grants_awards}, teaching={self.teaching}, supervision={self.supervision})"
+        repr = f"CV(filename={self.filename}, education={self.education}, institutes={self.institutes}, software={self.software}, intro={self.intro}, authors={self.authors}, news={self.news}, publications={self.publications}, research_interests={self.research_interests}, grants_awards={self.grants_awards}, teaching={self.teaching}, supervision={self.supervision}, experience={self.experience})"
         return repr
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    print(repr(cv.supervision))
+    print(cv.experience)
     sys.exit(0)
```

### Comparing `cvprocessor-0.0.26/src/cvprocessor/education.py` & `cvprocessor-0.0.27/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/grants_awards.py` & `cvprocessor-0.0.27/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/institutes.py` & `cvprocessor-0.0.27/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/intro.py` & `cvprocessor-0.0.27/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/news.py` & `cvprocessor-0.0.27/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/publications.py` & `cvprocessor-0.0.27/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.27/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/software.py` & `cvprocessor-0.0.27/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/supervision.py` & `cvprocessor-0.0.27/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor/teaching.py` & `cvprocessor-0.0.27/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.26/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.27/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.26
+Version: 0.0.27
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.26/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.27/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

