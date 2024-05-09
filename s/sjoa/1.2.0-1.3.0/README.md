# Comparing `tmp/sjoa-1.2.0.tar.gz` & `tmp/sjoa-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sjoa-1.2.0.tar", last modified: Tue Dec  5 14:56:29 2023, max compression
+gzip compressed data, was "sjoa-1.3.0.tar", last modified: Thu May  9 17:30:56 2024, max compression
```

## Comparing `sjoa-1.2.0.tar` & `sjoa-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:56:29.836103 sjoa-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-05 14:56:22.000000 sjoa-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2023-12-05 14:56:29.836103 sjoa-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-12-05 14:56:22.000000 sjoa-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 14:56:29.836103 sjoa-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2023-12-05 14:56:22.000000 sjoa-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:56:29.836103 sjoa-1.2.0/sjoa/
--rwxr-xr-x   0 runner    (1001) docker     (127)      509 2023-12-05 14:56:22.000000 sjoa-1.2.0/sjoa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2023-12-05 14:56:22.000000 sjoa-1.2.0/sjoa/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3472 2023-12-05 14:56:22.000000 sjoa-1.2.0/sjoa/decoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1097 2023-12-05 14:56:22.000000 sjoa-1.2.0/sjoa/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2023-12-05 14:56:22.000000 sjoa-1.2.0/sjoa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 14:56:29.836103 sjoa-1.2.0/sjoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2023-12-05 14:56:29.000000 sjoa-1.2.0/sjoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-05 14:56:29.000000 sjoa-1.2.0/sjoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 14:56:29.000000 sjoa-1.2.0/sjoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-05 14:56:29.000000 sjoa-1.2.0/sjoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-05 14:56:29.000000 sjoa-1.2.0/sjoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-05 14:56:29.000000 sjoa-1.2.0/sjoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:56.877050 sjoa-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-09 17:30:53.000000 sjoa-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-09 17:30:56.873050 sjoa-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-09 17:30:53.000000 sjoa-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:30:56.877050 sjoa-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1305 2024-05-09 17:30:53.000000 sjoa-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:56.873050 sjoa-1.3.0/sjoa/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-09 17:30:53.000000 sjoa-1.3.0/sjoa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-05-09 17:30:53.000000 sjoa-1.3.0/sjoa/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3553 2024-05-09 17:30:53.000000 sjoa-1.3.0/sjoa/decoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1800 2024-05-09 17:30:53.000000 sjoa-1.3.0/sjoa/display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1097 2024-05-09 17:30:53.000000 sjoa-1.3.0/sjoa/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-09 17:30:53.000000 sjoa-1.3.0/sjoa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:56.873050 sjoa-1.3.0/sjoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-09 17:30:56.000000 sjoa-1.3.0/sjoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 17:30:56.000000 sjoa-1.3.0/sjoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:30:56.000000 sjoa-1.3.0/sjoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 17:30:56.000000 sjoa-1.3.0/sjoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 17:30:56.000000 sjoa-1.3.0/sjoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:56.000000 sjoa-1.3.0/sjoa.egg-info/top_level.txt
```

### Comparing `sjoa-1.2.0/LICENSE` & `sjoa-1.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Martin Simon
+   Copyright 2023-2024 Martin Simon
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sjoa-1.2.0/PKG-INFO` & `sjoa-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: sjoa
-Version: 1.2.0
+Version: 1.3.0
 Summary: Command-line tool to read metadata from torrent files or magnet URLs.
 Home-page: https://github.com/barnumbirr/sjoa
 Download-URL: https://github.com/barnumbirr/sjoa/archive/refs/heads/master.zip
 Author: Martin Simon
 Author-email: me@martinsimon.me
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bencodepy==0.9.5
-Requires-Dist: rich==13.7.0
+Requires-Dist: rich==13.7.1
 
 # sjoa
 
 `sjoa` is a powerful command-line tool designed to read metadata from torrent
 files or magnet URIs. It provides a simple and efficient way to extract
 information about torrents without the need to download the actual content.
 
@@ -75,15 +76,15 @@
  Tracker URL(s)  • https://torrent.ubuntu.com/announce
                  • https://ipv6.torrent.ubuntu.com/announce
 ```
 
 ## License
 
 ```
-Copyright 2023 Martin Simon
+Copyright 2023-2024 Martin Simon
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: sjoa Version: 1.2.0 Summary: Command-line tool to
+Metadata-Version: 2.1 Name: sjoa Version: 1.3.0 Summary: Command-line tool to
 read metadata from torrent files or magnet URLs. Home-page: https://github.com/
 barnumbirr/sjoa Download-URL: https://github.com/barnumbirr/sjoa/archive/refs/
 heads/master.zip Author: Martin Simon Author-email: me@martinsimon.me
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: End Users/Desktop Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: bencodepy==0.9.5 Requires-Dist: rich==13.7.0 # sjoa `sjoa` is a
-powerful command-line tool designed to read metadata from torrent files or
-magnet URIs. It provides a simple and efficient way to extract information
-about torrents without the need to download the actual content. > The Sjoa is a
-river in Innlandet county, Norway and is one of the best > whitewater rafting
-rivers in Europe renowned for its fast-moving, turbulent > waters with Class
-II-V rapids depending on the water level. > >
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+bencodepy==0.9.5 Requires-Dist: rich==13.7.1 # sjoa `sjoa` is a powerful
+command-line tool designed to read metadata from torrent files or magnet URIs.
+It provides a simple and efficient way to extract information about torrents
+without the need to download the actual content. > The Sjoa is a river in
+Innlandet county, Norway and is one of the best > whitewater rafting rivers in
+Europe renowned for its fast-moving, turbulent > waters with Class II-V rapids
+depending on the water level. > >
                                                > Source: _W_i_k_i_p_e_d_i_a > and _O_A_R_S >
 The word `sjoa` was chosen as a play on words: the term "torrent" is often used
 to describe a fast-flowing stream or river, typically characterized by strong
 currents and rapid water movement. ## Installation `sjoa` is implemented in
 Python and can be installed using pip, the Python package manager. To install
 `sjoa`, simply run: ```bash $ pip install sjoa ``` ## Usage Once installed, you
 can use `sjoa` from the command line. ``` $ sjoa -t examples/debian-12.2.0-
@@ -36,15 +37,15 @@
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ´ââââââââââââââââââââââ
 ``` ``` $ sjoa -m "magnet:?xt=urn:btih:
 2c6b6858d61da9543d4231a71db4b1c9264b0685&dn=ubuntu-22.04-desktop-
 amd64.iso&tr=https%3A%2F%2Ftorrent.ubuntu.com%2Fannounce&tr=https%3A%2F%2Fipv6.torrent.ubuntu.com%2Fannounce"
 Name ubuntu-22.04-desktop-amd64.iso Hash
 2c6b6858d61da9543d4231a71db4b1c9264b0685 Tracker URL(s) â¢ https://
 torrent.ubuntu.com/announce â¢ https://ipv6.torrent.ubuntu.com/announce ``` ##
-License ``` Copyright 2023 Martin Simon Licensed under the Apache License,
+License ``` Copyright 2023-2024 Martin Simon Licensed under the Apache License,
 Version 2.0 (the "License"); you may not use this file except in compliance
 with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
 limitations under the License. ``` ## Buy me a coffee? If you feel like buying
```

### Comparing `sjoa-1.2.0/README.md` & `sjoa-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
  Tracker URL(s)  • https://torrent.ubuntu.com/announce
                  • https://ipv6.torrent.ubuntu.com/announce
 ```
 
 ## License
 
 ```
-Copyright 2023 Martin Simon
+Copyright 2023-2024 Martin Simon
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ´ââââââââââââââââââââââ
 ``` ``` $ sjoa -m "magnet:?xt=urn:btih:
 2c6b6858d61da9543d4231a71db4b1c9264b0685&dn=ubuntu-22.04-desktop-
 amd64.iso&tr=https%3A%2F%2Ftorrent.ubuntu.com%2Fannounce&tr=https%3A%2F%2Fipv6.torrent.ubuntu.com%2Fannounce"
 Name ubuntu-22.04-desktop-amd64.iso Hash
 2c6b6858d61da9543d4231a71db4b1c9264b0685 Tracker URL(s) â¢ https://
 torrent.ubuntu.com/announce â¢ https://ipv6.torrent.ubuntu.com/announce ``` ##
-License ``` Copyright 2023 Martin Simon Licensed under the Apache License,
+License ``` Copyright 2023-2024 Martin Simon Licensed under the Apache License,
 Version 2.0 (the "License"); you may not use this file except in compliance
 with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
 limitations under the License. ``` ## Buy me a coffee? If you feel like buying
```

### Comparing `sjoa-1.2.0/setup.py` & `sjoa-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as fi:
     required = fi.read().splitlines()
 
 setup(
     name='sjoa',
-    version='1.2.0',
+    version='1.3.0',
     author='Martin Simon',
     author_email='me@martinsimon.me',
     description='Command-line tool to read metadata from torrent files or magnet URLs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/barnumbirr/sjoa',
     download_url='https://github.com/barnumbirr/sjoa/archive/refs/heads/master.zip',
@@ -30,9 +30,10 @@
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ]
 )
```

### Comparing `sjoa-1.2.0/sjoa/decoder.py` & `sjoa-1.3.0/sjoa/decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def _ps_torrent(file):
     metadata = {}
     decoded_data = bencodepy.decode(file)
     info = decoded_data.get(b'info', {})
 
     metadata['hash'] = hashlib.sha1(bencodepy.encode(info)).hexdigest() if info else None
     metadata['name'] = info.get(b'name').decode() if info.get(b'name') else None
+    metadata['private'] = info.get(b'private') if info.get(b'private') else None
 
     creation = {}
     creation['date'] = datetime.datetime.utcfromtimestamp(
         decoded_data.get(b"creation date")
     ).isoformat(' ')
     creation['tool'] = decoded_data.get(b'created by').decode()
     metadata['creation'] = creation
```

### Comparing `sjoa-1.2.0/sjoa/parser.py` & `sjoa-1.3.0/sjoa/parser.py`

 * *Files identical despite different names*

### Comparing `sjoa-1.2.0/sjoa/utils.py` & `sjoa-1.3.0/sjoa/utils.py`

 * *Files identical despite different names*

### Comparing `sjoa-1.2.0/sjoa.egg-info/PKG-INFO` & `sjoa-1.3.0/sjoa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: sjoa
-Version: 1.2.0
+Version: 1.3.0
 Summary: Command-line tool to read metadata from torrent files or magnet URLs.
 Home-page: https://github.com/barnumbirr/sjoa
 Download-URL: https://github.com/barnumbirr/sjoa/archive/refs/heads/master.zip
 Author: Martin Simon
 Author-email: me@martinsimon.me
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bencodepy==0.9.5
-Requires-Dist: rich==13.7.0
+Requires-Dist: rich==13.7.1
 
 # sjoa
 
 `sjoa` is a powerful command-line tool designed to read metadata from torrent
 files or magnet URIs. It provides a simple and efficient way to extract
 information about torrents without the need to download the actual content.
 
@@ -75,15 +76,15 @@
  Tracker URL(s)  • https://torrent.ubuntu.com/announce
                  • https://ipv6.torrent.ubuntu.com/announce
 ```
 
 ## License
 
 ```
-Copyright 2023 Martin Simon
+Copyright 2023-2024 Martin Simon
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: sjoa Version: 1.2.0 Summary: Command-line tool to
+Metadata-Version: 2.1 Name: sjoa Version: 1.3.0 Summary: Command-line tool to
 read metadata from torrent files or magnet URLs. Home-page: https://github.com/
 barnumbirr/sjoa Download-URL: https://github.com/barnumbirr/sjoa/archive/refs/
 heads/master.zip Author: Martin Simon Author-email: me@martinsimon.me
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: End Users/Desktop Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: bencodepy==0.9.5 Requires-Dist: rich==13.7.0 # sjoa `sjoa` is a
-powerful command-line tool designed to read metadata from torrent files or
-magnet URIs. It provides a simple and efficient way to extract information
-about torrents without the need to download the actual content. > The Sjoa is a
-river in Innlandet county, Norway and is one of the best > whitewater rafting
-rivers in Europe renowned for its fast-moving, turbulent > waters with Class
-II-V rapids depending on the water level. > >
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+bencodepy==0.9.5 Requires-Dist: rich==13.7.1 # sjoa `sjoa` is a powerful
+command-line tool designed to read metadata from torrent files or magnet URIs.
+It provides a simple and efficient way to extract information about torrents
+without the need to download the actual content. > The Sjoa is a river in
+Innlandet county, Norway and is one of the best > whitewater rafting rivers in
+Europe renowned for its fast-moving, turbulent > waters with Class II-V rapids
+depending on the water level. > >
                                                > Source: _W_i_k_i_p_e_d_i_a > and _O_A_R_S >
 The word `sjoa` was chosen as a play on words: the term "torrent" is often used
 to describe a fast-flowing stream or river, typically characterized by strong
 currents and rapid water movement. ## Installation `sjoa` is implemented in
 Python and can be installed using pip, the Python package manager. To install
 `sjoa`, simply run: ```bash $ pip install sjoa ``` ## Usage Once installed, you
 can use `sjoa` from the command line. ``` $ sjoa -t examples/debian-12.2.0-
@@ -36,15 +37,15 @@
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ´ââââââââââââââââââââââ
 ``` ``` $ sjoa -m "magnet:?xt=urn:btih:
 2c6b6858d61da9543d4231a71db4b1c9264b0685&dn=ubuntu-22.04-desktop-
 amd64.iso&tr=https%3A%2F%2Ftorrent.ubuntu.com%2Fannounce&tr=https%3A%2F%2Fipv6.torrent.ubuntu.com%2Fannounce"
 Name ubuntu-22.04-desktop-amd64.iso Hash
 2c6b6858d61da9543d4231a71db4b1c9264b0685 Tracker URL(s) â¢ https://
 torrent.ubuntu.com/announce â¢ https://ipv6.torrent.ubuntu.com/announce ``` ##
-License ``` Copyright 2023 Martin Simon Licensed under the Apache License,
+License ``` Copyright 2023-2024 Martin Simon Licensed under the Apache License,
 Version 2.0 (the "License"); you may not use this file except in compliance
 with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
 limitations under the License. ``` ## Buy me a coffee? If you feel like buying
```

