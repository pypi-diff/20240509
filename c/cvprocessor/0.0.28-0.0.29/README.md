# Comparing `tmp/cvprocessor-0.0.28.tar.gz` & `tmp/cvprocessor-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.28.tar", last modified: Thu May  9 01:34:46 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.29.tar", last modified: Thu May  9 01:45:05 2024, max compression
```

## Comparing `cvprocessor-0.0.28.tar` & `cvprocessor-0.0.29.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:34:46.597425 cvprocessor-0.0.28/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.28/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-09 01:34:46.596799 cvprocessor-0.0.28/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.0.28/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-09 01:34:17.000000 cvprocessor-0.0.28/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-09 01:34:46.597572 cvprocessor-0.0.28/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:34:46.575302 cvprocessor-0.0.28/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:34:46.591873 cvprocessor-0.0.28/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.28/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.0.28/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.28/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     3974 2024-05-09 01:17:24.000000 cvprocessor-0.0.28/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.0.28/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.0.28/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.0.28/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3795 2024-05-08 07:11:28.000000 cvprocessor-0.0.28/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.0.28/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.0.28/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.0.28/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.0.28/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.0.28/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.0.28/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.0.28/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5799 2024-05-08 07:22:45.000000 cvprocessor-0.0.28/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:34:46.596179 cvprocessor-0.0.28/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-09 01:34:46.000000 cvprocessor-0.0.28/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      683 2024-05-09 01:34:46.000000 cvprocessor-0.0.28/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-09 01:34:46.000000 cvprocessor-0.0.28/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-09 01:34:46.000000 cvprocessor-0.0.28/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-09 01:34:46.000000 cvprocessor-0.0.28/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:45:05.717064 cvprocessor-0.0.29/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.29/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-09 01:45:05.716443 cvprocessor-0.0.29/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.0.29/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-09 01:44:37.000000 cvprocessor-0.0.29/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-09 01:45:05.717213 cvprocessor-0.0.29/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:45:05.693382 cvprocessor-0.0.29/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:45:05.711220 cvprocessor-0.0.29/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.29/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.0.29/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.29/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4205 2024-05-09 01:44:26.000000 cvprocessor-0.0.29/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.0.29/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.0.29/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.0.29/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3795 2024-05-08 07:11:28.000000 cvprocessor-0.0.29/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.0.29/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.0.29/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.0.29/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.0.29/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1980 2024-05-09 01:44:15.000000 cvprocessor-0.0.29/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.0.29/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.0.29/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.0.29/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5799 2024-05-08 07:22:45.000000 cvprocessor-0.0.29/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 01:45:05.715698 cvprocessor-0.0.29/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-09 01:45:05.000000 cvprocessor-0.0.29/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      710 2024-05-09 01:45:05.000000 cvprocessor-0.0.29/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-09 01:45:05.000000 cvprocessor-0.0.29/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-09 01:45:05.000000 cvprocessor-0.0.29/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-09 01:45:05.000000 cvprocessor-0.0.29/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.28/LICENSE` & `cvprocessor-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/PKG-INFO` & `cvprocessor-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.28
+Version: 0.0.29
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.28/README.md` & `cvprocessor-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/pyproject.toml` & `cvprocessor-0.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.28"
+version = "0.0.29"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.28/src/cvprocessor/authors.py` & `cvprocessor-0.0.29/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/cv.py` & `cvprocessor-0.0.29/src/cvprocessor/cv.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from cvprocessor.news import News
 from cvprocessor.research_interests import ResearchInterests
 from cvprocessor.grants_awards import GrantsAwards
 from cvprocessor.teaching import Teaching
 from cvprocessor.supervision import Supervision
 from cvprocessor.experience import Experience
 from cvprocessor.skills import Skills
+from cvprocessor.service import Services
 
 
 class CV:
     def __init__(self, filename):
         self._filename = filename
         self._education = Education(self.filename)
         self._institutes = Institutes(self.filename)
@@ -30,14 +31,15 @@
         self._publications = Publications(self.filename, self)
         self._research_interests = ResearchInterests(self.filename)
         self._grants_awards = GrantsAwards(self.filename)
         self._teaching = Teaching(self.filename)
         self._supervision = Supervision(self.filename, self)
         self._experience = Experience(self.filename, self)
         self._skills = Skills(self.filename)
+        self._service = Services(self.filename)
 
     @property
     def filename(self):
         return self._filename
 
     @property
     def intro(self):
@@ -90,14 +92,18 @@
     @property
     def experience(self):
         return self._experience
 
     @property
     def skills(self):
         return self._skills
+    
+    @property
+    def service(self):
+        return self._service
 
     def __str__(self):
         string = f"Education: {self.education}\n"
         string += f"Institutes: {self.institutes}\n"
         string += f"Software: {self.software}\n"
         string += f"Intro: {self.intro}\n"
         string += f"Authors: {self.authors}\n"
@@ -105,18 +111,19 @@
         string += f"Publications: {self.publications}\n"
         string += f"Research Interests: {self.research_interests}\n"
         string += f"Grants and Awards: {self.grants_awards}\n"
         string += f"Teaching: {self.teaching}\n"
         string += f"Supervision: {self.supervision}\n"
         string += f"Experience: {self.experience}\n"
         string += f"Skills: {self.skills}\n"
+        string += f"Service: {self.service}\n"
         return string
 
     def __repr__(self):
-        repr = f"CV(filename={self.filename}, education={self.education}, institutes={self.institutes}, software={self.software}, intro={self.intro}, authors={self.authors}, news={self.news}, publications={self.publications}, research_interests={self.research_interests}, grants_awards={self.grants_awards}, teaching={self.teaching}, supervision={self.supervision}, experience={self.experience}, skills={self.skills})"
+        repr = f"CV(filename={self.filename}, education={self.education}, institutes={self.institutes}, software={self.software}, intro={self.intro}, authors={self.authors}, news={self.news}, publications={self.publications}, research_interests={self.research_interests}, grants_awards={self.grants_awards}, teaching={self.teaching}, supervision={self.supervision}, experience={self.experience}, skills={self.skills}, service={self.service})"
         return repr
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    print(repr(cv.skills))
+    print(str(cv.service))
     sys.exit(0)
```

### Comparing `cvprocessor-0.0.28/src/cvprocessor/education.py` & `cvprocessor-0.0.29/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/experience.py` & `cvprocessor-0.0.29/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/grants_awards.py` & `cvprocessor-0.0.29/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/institutes.py` & `cvprocessor-0.0.29/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/intro.py` & `cvprocessor-0.0.29/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/news.py` & `cvprocessor-0.0.29/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/publications.py` & `cvprocessor-0.0.29/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.29/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/skills.py` & `cvprocessor-0.0.29/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/software.py` & `cvprocessor-0.0.29/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/supervision.py` & `cvprocessor-0.0.29/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor/teaching.py` & `cvprocessor-0.0.29/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.28/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.29/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.28
+Version: 0.0.29
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.28/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.29/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/cvprocessor/experience.py
 src/cvprocessor/grants_awards.py
 src/cvprocessor/institutes.py
 src/cvprocessor/intro.py
 src/cvprocessor/news.py
 src/cvprocessor/publications.py
 src/cvprocessor/research_interests.py
+src/cvprocessor/service.py
 src/cvprocessor/skills.py
 src/cvprocessor/software.py
 src/cvprocessor/supervision.py
 src/cvprocessor/teaching.py
 src/cvprocessor.egg-info/PKG-INFO
 src/cvprocessor.egg-info/SOURCES.txt
 src/cvprocessor.egg-info/dependency_links.txt
```

