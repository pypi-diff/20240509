# Comparing `tmp/animeflvV2-0.0.7.tar.gz` & `tmp/animeflvv2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animeflvV2-0.0.7.tar", last modified: Tue Feb 21 19:05:29 2023, max compression
+gzip compressed data, was "animeflvv2-0.0.8.tar", last modified: Wed May  8 22:28:45 2024, max compression
```

## Comparing `animeflvV2-0.0.7.tar` & `animeflvv2-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-02-21 19:05:29.444490 animeflvV2-0.0.7/
--rw-rw-r--   0 julian    (1000) julian    (1000)     1070 2023-02-14 22:53:39.000000 animeflvV2-0.0.7/LICENSE
--rw-rw-r--   0 julian    (1000) julian    (1000)     1544 2023-02-21 19:05:29.444490 animeflvV2-0.0.7/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      633 2023-02-20 19:03:17.000000 animeflvV2-0.0.7/README.md
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-02-21 19:05:29.440490 animeflvV2-0.0.7/animeflvV2/
--rw-rw-r--   0 julian    (1000) julian    (1000)      216 2023-02-21 19:04:17.000000 animeflvV2-0.0.7/animeflvV2/__init__.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    18358 2023-02-21 19:01:34.000000 animeflvV2-0.0.7/animeflvV2/animeflvV2.py
--rw-rw-r--   0 julian    (1000) julian    (1000)       46 2023-02-14 22:52:22.000000 animeflvV2-0.0.7/animeflvV2/exception.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-02-21 19:05:29.444490 animeflvV2-0.0.7/animeflvV2.egg-info/
--rw-rw-r--   0 julian    (1000) julian    (1000)     1544 2023-02-21 19:05:29.000000 animeflvV2-0.0.7/animeflvV2.egg-info/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      299 2023-02-21 19:05:29.000000 animeflvV2-0.0.7/animeflvV2.egg-info/SOURCES.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-02-21 19:05:29.000000 animeflvV2-0.0.7/animeflvV2.egg-info/dependency_links.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       33 2023-02-21 19:05:29.000000 animeflvV2-0.0.7/animeflvV2.egg-info/requires.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       11 2023-02-21 19:05:29.000000 animeflvV2-0.0.7/animeflvV2.egg-info/top_level.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)     1104 2023-02-14 23:09:17.000000 animeflvV2-0.0.7/pyproject.toml
--rw-rw-r--   0 julian    (1000) julian    (1000)       32 2023-02-14 22:52:22.000000 animeflvV2-0.0.7/requirements.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-02-21 19:05:29.444490 animeflvV2-0.0.7/setup.cfg
--rw-rw-r--   0 julian    (1000) julian    (1000)       86 2023-02-14 22:52:57.000000 animeflvV2-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:28:45.389245 animeflvv2-0.0.8/
+-rw-rw-rw-   0        0        0     1070 2023-02-14 22:53:39.000000 animeflvv2-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1159 2024-05-08 22:28:45.387241 animeflvv2-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2024-05-08 21:38:21.000000 animeflvv2-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 22:28:45.351258 animeflvv2-0.0.8/animeflvV2/
+-rw-rw-rw-   0        0        0      216 2024-05-08 21:39:47.000000 animeflvv2-0.0.8/animeflvV2/__init__.py
+-rw-rw-rw-   0        0        0    18394 2024-05-08 21:40:48.000000 animeflvv2-0.0.8/animeflvV2/animeflvV2.py
+-rw-rw-rw-   0        0        0       46 2023-02-14 22:52:22.000000 animeflvv2-0.0.8/animeflvV2/exception.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:28:45.386242 animeflvv2-0.0.8/animeflvV2.egg-info/
+-rw-rw-rw-   0        0        0     1159 2024-05-08 22:28:45.000000 animeflvv2-0.0.8/animeflvV2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-08 22:28:45.000000 animeflvv2-0.0.8/animeflvV2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 22:28:45.000000 animeflvv2-0.0.8/animeflvV2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 22:28:45.000000 animeflvv2-0.0.8/animeflvV2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 22:28:45.000000 animeflvv2-0.0.8/animeflvV2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 22:28:45.389245 animeflvv2-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2024-05-08 22:28:40.000000 animeflvv2-0.0.8/setup.py
```

### Comparing `animeflvV2-0.0.7/LICENSE` & `animeflvv2-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `animeflvV2-0.0.7/PKG-INFO` & `animeflvv2-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-Metadata-Version: 2.1
-Name: animeflvV2
-Version: 0.0.7
-Summary: AnimeFLV is a python custom API for https://animeflv.net website
-Author-email: Julian Morera <xxxx@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/JulianMorera07/anime-flv-api
-Keywords: animeflv,anime,manga
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AnimeFLV API
-
-
-> AnimeFLV is a python custom API for [animeflv.net](https://animeflv.net) a Spanish anime content website.
-
-## Installation
-For install with pip:
-```bash
-$ pip install animeflvV2
-```
-
-## API Documentation
-
-#### Create animeflv api instance:
-```python
->>> from animeflv import AnimeFLV
->>> with AnimeFLV() as api:
->>>     # Do anything with api object
->>>    ...
-```
-
-#### Features
-- [X] Get download links by episodes
-- [X] Search
-- [X] Get Video Servers
-- [X] Get Anime Info
-- [X] Get new releases (animes and episodes)
-
-## License
-[MIT](./LICENSE)
-
-## Authors
-+ [Julian Morera](https://github.com/JulianMorera07)
+Metadata-Version: 2.1
+Name: animeflvV2
+Version: 0.0.8
+Summary: Api para ver anime de AnimeFLV
+Home-page: 
+Author: 
+Author-email: 
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+# AnimeFLV API
+
+
+> AnimeFLV is a python custom API for [animeflv.net](https://animeflv.net) a Spanish anime content website.
+
+## Installation
+For install with pip:
+```bash
+$ pip install animeflvV2
+```
+
+## API Documentation
+
+#### Create animeflv api instance:
+```python
+>>> from animeflvV2 import AnimeFLV
+>>> with AnimeFLV() as api:
+>>>     # Do anything with api object
+>>>    ...
+```
+
+#### Features
+- [X] Get download links by episodes
+- [X] Search
+- [X] Get Video Servers
+- [X] Get Anime Info
+- [X] Get new releases (animes and episodes)
+
+## License
+[MIT](./LICENSE)
+
+## Authors
++ [Julian Morera](https://github.com/JulianMorera07)
```

### Comparing `animeflvV2-0.0.7/README.md` & `animeflvv2-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 $ pip install animeflvV2
 ```
 
 ## API Documentation
 
 #### Create animeflv api instance:
 ```python
->>> from animeflv import AnimeFLV
+>>> from animeflvV2 import AnimeFLV
 >>> with AnimeFLV() as api:
 >>>     # Do anything with api object
 >>>    ...
 ```
 
 #### Features
 - [X] Get download links by episodes
```

### Comparing `animeflvV2-0.0.7/animeflvV2/animeflvV2.py` & `animeflvv2-0.0.8/animeflvV2/animeflvV2.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                 videos = content.split("var videos = ")[1].split(";")[0]
                 data = json.loads(videos)
 
                 if "SUB" in data and EpisodeFormat.Subtitled in format:
                     servers.append(data["SUB"])
                 if "LAT" in data and EpisodeFormat.Dubbed in format:
                     servers.append(data["LAT"])
-
+                servers.append(data)
         return servers
 
     def chapters(self,id,format: EpisodeFormat = EpisodeFormat.Subtitled,**kwargs):
         response = self._scraper.get(f"{ANIME_VIDEO_URL}{id}")
         soup = BeautifulSoup(response.text, "lxml")
         elements = soup.select('div.CapNv')
         response = []
```

### Comparing `animeflvV2-0.0.7/animeflvV2.egg-info/PKG-INFO` & `animeflvv2-0.0.8/animeflvV2.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-Metadata-Version: 2.1
-Name: animeflvV2
-Version: 0.0.7
-Summary: AnimeFLV is a python custom API for https://animeflv.net website
-Author-email: Julian Morera <xxxx@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/JulianMorera07/anime-flv-api
-Keywords: animeflv,anime,manga
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AnimeFLV API
-
-
-> AnimeFLV is a python custom API for [animeflv.net](https://animeflv.net) a Spanish anime content website.
-
-## Installation
-For install with pip:
-```bash
-$ pip install animeflvV2
-```
-
-## API Documentation
-
-#### Create animeflv api instance:
-```python
->>> from animeflv import AnimeFLV
->>> with AnimeFLV() as api:
->>>     # Do anything with api object
->>>    ...
-```
-
-#### Features
-- [X] Get download links by episodes
-- [X] Search
-- [X] Get Video Servers
-- [X] Get Anime Info
-- [X] Get new releases (animes and episodes)
-
-## License
-[MIT](./LICENSE)
-
-## Authors
-+ [Julian Morera](https://github.com/JulianMorera07)
+Metadata-Version: 2.1
+Name: animeflvV2
+Version: 0.0.8
+Summary: Api para ver anime de AnimeFLV
+Home-page: 
+Author: 
+Author-email: 
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+# AnimeFLV API
+
+
+> AnimeFLV is a python custom API for [animeflv.net](https://animeflv.net) a Spanish anime content website.
+
+## Installation
+For install with pip:
+```bash
+$ pip install animeflvV2
+```
+
+## API Documentation
+
+#### Create animeflv api instance:
+```python
+>>> from animeflvV2 import AnimeFLV
+>>> with AnimeFLV() as api:
+>>>     # Do anything with api object
+>>>    ...
+```
+
+#### Features
+- [X] Get download links by episodes
+- [X] Search
+- [X] Get Video Servers
+- [X] Get Anime Info
+- [X] Get new releases (animes and episodes)
+
+## License
+[MIT](./LICENSE)
+
+## Authors
++ [Julian Morera](https://github.com/JulianMorera07)
```

