# Comparing `tmp/make_playlist-1.8.0.tar.gz` & `tmp/make_playlist-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_playlist-1.8.0.tar", last modified: Thu Aug  3 11:03:54 2023, max compression
+gzip compressed data, was "make_playlist-1.9.0.tar", last modified: Thu May  9 07:57:59 2024, max compression
```

## Comparing `make_playlist-1.8.0.tar` & `make_playlist-1.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gu        (1000) gu        (1000)        0 2023-08-03 11:03:54.299885 make_playlist-1.8.0/
--rwxrwxr-x   0 gu        (1000) gu        (1000)    34916 2022-10-24 16:51:45.000000 make_playlist-1.8.0/LICENSE.md
--rw-rw-r--   0 gu        (1000) gu        (1000)     9110 2023-08-03 11:03:54.299885 make_playlist-1.8.0/PKG-INFO
--rw-rw-r--   0 gu        (1000) gu        (1000)     8401 2023-08-03 11:01:53.000000 make_playlist-1.8.0/README.md
-drwxrwxr-x   0 gu        (1000) gu        (1000)        0 2023-08-03 11:03:54.299885 make_playlist-1.8.0/make_playlist.egg-info/
--rw-rw-r--   0 gu        (1000) gu        (1000)     9110 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/PKG-INFO
--rw-rw-r--   0 gu        (1000) gu        (1000)      267 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/SOURCES.txt
--rw-rw-r--   0 gu        (1000) gu        (1000)        1 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/dependency_links.txt
--rw-rw-r--   0 gu        (1000) gu        (1000)       61 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/entry_points.txt
--rw-rw-r--   0 gu        (1000) gu        (1000)        8 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/requires.txt
--rw-rw-r--   0 gu        (1000) gu        (1000)        5 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/top_level.txt
--rw-rw-r--   0 gu        (1000) gu        (1000)    18599 2023-08-03 11:01:53.000000 make_playlist-1.8.0/mkpl.py
--rw-rw-r--   0 gu        (1000) gu        (1000)      929 2023-08-03 11:01:53.000000 make_playlist-1.8.0/pyproject.toml
--rw-rw-r--   0 gu        (1000) gu        (1000)       38 2023-08-03 11:03:54.299885 make_playlist-1.8.0/setup.cfg
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-05-09 07:57:59.807156 make_playlist-1.9.0/
+-rwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)    34916 2022-09-09 08:34:13.000000 make_playlist-1.9.0/LICENSE.md
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    10218 2024-05-09 07:57:59.807156 make_playlist-1.9.0/PKG-INFO
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     9486 2024-05-09 07:54:51.000000 make_playlist-1.9.0/README.md
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-05-09 07:57:59.807156 make_playlist-1.9.0/make_playlist.egg-info/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    10218 2024-05-09 07:57:59.000000 make_playlist-1.9.0/make_playlist.egg-info/PKG-INFO
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      267 2024-05-09 07:57:59.000000 make_playlist-1.9.0/make_playlist.egg-info/SOURCES.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        1 2024-05-09 07:57:59.000000 make_playlist-1.9.0/make_playlist.egg-info/dependency_links.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       61 2024-05-09 07:57:59.000000 make_playlist-1.9.0/make_playlist.egg-info/entry_points.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        8 2024-05-09 07:57:59.000000 make_playlist-1.9.0/make_playlist.egg-info/requires.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        5 2024-05-09 07:57:59.000000 make_playlist-1.9.0/make_playlist.egg-info/top_level.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    20456 2024-05-09 07:54:51.000000 make_playlist-1.9.0/mkpl.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      929 2024-05-09 07:54:51.000000 make_playlist-1.9.0/pyproject.toml
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       38 2024-05-09 07:57:59.807156 make_playlist-1.9.0/setup.cfg
```

### Comparing `make_playlist-1.8.0/LICENSE.md` & `make_playlist-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `make_playlist-1.8.0/PKG-INFO` & `make_playlist-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: make_playlist
-Version: 1.8.0
+Version: 1.9.0
 Summary: Make M3U format playlist from command line.
 Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Project-URL: homepage, https://github.com/MatteoGuadrini/mkpl
 Project-URL: documentation, https://matteoguadrini.github.io/mkpl/
 Project-URL: changelog, https://github.com/MatteoGuadrini/mkpl/blob/master/CHANGES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: mutagen
 
 # ``make_playlist``: Playlist maker
 
 <img src="img/mkpl_logo.svg" alt="mkpl" title="mkpl" width="200" height="200" />
 
 ``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
@@ -34,40 +35,44 @@
 $ pip install .                           # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
-| short | long            | description                                   | args                      |
-|-------|-----------------|-----------------------------------------------|---------------------------|
-| -d    | --directories   | Directories that contains multimedia file     | Path of directories       |
-| -e    | --exclude-dirs  | Exclude directory paths                       | Path of directories       |
-| -i    | --include       | Include other file format                     | Format of file. ex. mp3   |
-| -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
-| -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
-| -s    | --size          | Start size in bytes                           | Bytes number              |
-| -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
-| -t    | --title         | Playlist title                                | Title string              |
-| -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
-| -I    | --image         | Playlist image                                | Image path                |
-| -l    | --link          | Add local or remote files                     | Files                     |
-| -j    | --join          | Join one or more other playlist files         | Playlist files            |
-| -r    | --recursive     | Recursive search                              |                           |
-| -a    | --absolute      | Absolute file name                            |                           |
-| -s    | --shuffle       | Casual order                                  |                           |
-| -u    | --unique        | The same files are not placed in the playlist |                           |
-| -c    | --append        | Continue playlist instead of override it      |                           |
-| -w    | --windows       | Windows style folder separator                |                           |
-| -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
-| -S    | --split         | Split playlist by directories                 |                           |
-| -o    | --orderby-name  | Order playlist files by name                  |                           |
-| -O    | --orderby-date  | Order playlist files by creation date         |                           |
-| -T    | --orderby-track | Order playlist files by track                 |                           |
-| -y    | --orderby-year  | Order playlist files by year                  |                           |
+| short | long             | description                                   | args                      |
+|-------|------------------|-----------------------------------------------|---------------------------|
+| -d    | --directories    | Directories that contains multimedia file     | Path of directories       |
+| -e    | --exclude-dirs   | Exclude directory paths                       | Path of directories       |
+| -i    | --include        | Include other file format                     | Format of file. ex. mp3   |
+| -p    | --pattern        | Regular expression inclusion pattern          | Regular expression string |
+| -f    | --format         | Select only a file format                     | Format of file. ex. mp3   |
+| -s    | --size           | Start size in bytes                           | Bytes number              |
+| -m    | --max-tracks     | Maximum number of tracks                      | Number                    |
+| -t    | --title          | Playlist title                                | Title string              |
+| -g    | --encoding       | Text encoding                                 | UTF-8,ASCII,UNICODE       |
+| -I    | --image          | Playlist image                                | Image path                |
+| -l    | --link           | Add local or remote files                     | Files                     |
+| -j    | --join           | Join one or more other playlist files         | Playlist files            |
+| -r    | --recursive      | Recursive search                              |                           |
+| -a    | --absolute       | Absolute file name                            |                           |
+| -s    | --shuffle        | Casual order                                  |                           |
+| -u    | --unique         | The same files are not placed in the playlist |                           |
+| -c    | --append         | Continue playlist instead of override it      |                           |
+| -w    | --windows        | Windows style folder separator                |                           |
+| -v    | --verbose        | Enable verbosity (debug mode)                 |                           |
+| -S    | --split          | Split playlist by directories                 |                           |
+| -R    | --interactive    | Asks each file for confirmation               |                           |
+| -C    | --count          | Count elements into playlist                  |                           |
+| -o    | --orderby-name   | Order playlist files by name                  |                           |
+| -O    | --orderby-date   | Order playlist files by creation date         |                           |
+| -T    | --orderby-track  | Order playlist files by track                 |                           |
+| -y    | --orderby-year   | Order playlist files by year                  |                           |
+| -Z    | --orderby-size   | Order playlist files by size                  |                           |
+| -L    | --orderby-length | Order playlist files by length                |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -158,27 +163,47 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`) or by year (`-y`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`), by year (`-y`), by size (`-Z`) or by length (`-L`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
     mkpl -d "new_collection" -r "my music.m3u" -T
     mkpl -d "new_collection" -r "my music.m3u" -y
+    mkpl -d "new_collection" -r "my music.m3u" -Z
+    mkpl -d "new_collection" -r "my music.m3u" -L
     ```
 
 16. Join the _"First playlist.m3u"_ and  _"Second playlist.m3u8"_ with new **"Third playlist.m3u"**:
 
     ```bash
     mkpl -d "new_collection" -r "Third playlist" -j "First playlist.m3u" "Second playlist.m3u8"
+    ```
+
+17. Counts the multimedia files:
+
+    ```console
+    mkpl -d "new_collection" -r "My new collection" -C
+    4023
+    ```
+
+18. Asks confirmation for every file into folders:
+
+    ```console
+    mkpl -d "new_collection" -r "My new collection" -R
+    Add file new_collection/sample1.mp3 to playlist? [Y/n]:y
+    Add file new_collection/sample2.mp3 to playlist? [Y/n]:Y
+    Add file new_collection/sample3.mp3 to playlist? [Y/n]:n
+    Add file new_collection/sample4.mp3 to playlist? [Y/n]:N
+    ```
 
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
 from make_playlist import *
```

### Comparing `make_playlist-1.8.0/README.md` & `make_playlist-1.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,40 +18,44 @@
 $ pip install .                           # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
-| short | long            | description                                   | args                      |
-|-------|-----------------|-----------------------------------------------|---------------------------|
-| -d    | --directories   | Directories that contains multimedia file     | Path of directories       |
-| -e    | --exclude-dirs  | Exclude directory paths                       | Path of directories       |
-| -i    | --include       | Include other file format                     | Format of file. ex. mp3   |
-| -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
-| -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
-| -s    | --size          | Start size in bytes                           | Bytes number              |
-| -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
-| -t    | --title         | Playlist title                                | Title string              |
-| -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
-| -I    | --image         | Playlist image                                | Image path                |
-| -l    | --link          | Add local or remote files                     | Files                     |
-| -j    | --join          | Join one or more other playlist files         | Playlist files            |
-| -r    | --recursive     | Recursive search                              |                           |
-| -a    | --absolute      | Absolute file name                            |                           |
-| -s    | --shuffle       | Casual order                                  |                           |
-| -u    | --unique        | The same files are not placed in the playlist |                           |
-| -c    | --append        | Continue playlist instead of override it      |                           |
-| -w    | --windows       | Windows style folder separator                |                           |
-| -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
-| -S    | --split         | Split playlist by directories                 |                           |
-| -o    | --orderby-name  | Order playlist files by name                  |                           |
-| -O    | --orderby-date  | Order playlist files by creation date         |                           |
-| -T    | --orderby-track | Order playlist files by track                 |                           |
-| -y    | --orderby-year  | Order playlist files by year                  |                           |
+| short | long             | description                                   | args                      |
+|-------|------------------|-----------------------------------------------|---------------------------|
+| -d    | --directories    | Directories that contains multimedia file     | Path of directories       |
+| -e    | --exclude-dirs   | Exclude directory paths                       | Path of directories       |
+| -i    | --include        | Include other file format                     | Format of file. ex. mp3   |
+| -p    | --pattern        | Regular expression inclusion pattern          | Regular expression string |
+| -f    | --format         | Select only a file format                     | Format of file. ex. mp3   |
+| -s    | --size           | Start size in bytes                           | Bytes number              |
+| -m    | --max-tracks     | Maximum number of tracks                      | Number                    |
+| -t    | --title          | Playlist title                                | Title string              |
+| -g    | --encoding       | Text encoding                                 | UTF-8,ASCII,UNICODE       |
+| -I    | --image          | Playlist image                                | Image path                |
+| -l    | --link           | Add local or remote files                     | Files                     |
+| -j    | --join           | Join one or more other playlist files         | Playlist files            |
+| -r    | --recursive      | Recursive search                              |                           |
+| -a    | --absolute       | Absolute file name                            |                           |
+| -s    | --shuffle        | Casual order                                  |                           |
+| -u    | --unique         | The same files are not placed in the playlist |                           |
+| -c    | --append         | Continue playlist instead of override it      |                           |
+| -w    | --windows        | Windows style folder separator                |                           |
+| -v    | --verbose        | Enable verbosity (debug mode)                 |                           |
+| -S    | --split          | Split playlist by directories                 |                           |
+| -R    | --interactive    | Asks each file for confirmation               |                           |
+| -C    | --count          | Count elements into playlist                  |                           |
+| -o    | --orderby-name   | Order playlist files by name                  |                           |
+| -O    | --orderby-date   | Order playlist files by creation date         |                           |
+| -T    | --orderby-track  | Order playlist files by track                 |                           |
+| -y    | --orderby-year   | Order playlist files by year                  |                           |
+| -Z    | --orderby-size   | Order playlist files by size                  |                           |
+| -L    | --orderby-length | Order playlist files by length                |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -142,27 +146,47 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`) or by year (`-y`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`), by year (`-y`), by size (`-Z`) or by length (`-L`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
     mkpl -d "new_collection" -r "my music.m3u" -T
     mkpl -d "new_collection" -r "my music.m3u" -y
+    mkpl -d "new_collection" -r "my music.m3u" -Z
+    mkpl -d "new_collection" -r "my music.m3u" -L
     ```
 
 16. Join the _"First playlist.m3u"_ and  _"Second playlist.m3u8"_ with new **"Third playlist.m3u"**:
 
     ```bash
     mkpl -d "new_collection" -r "Third playlist" -j "First playlist.m3u" "Second playlist.m3u8"
+    ```
+
+17. Counts the multimedia files:
+
+    ```console
+    mkpl -d "new_collection" -r "My new collection" -C
+    4023
+    ```
+
+18. Asks confirmation for every file into folders:
+
+    ```console
+    mkpl -d "new_collection" -r "My new collection" -R
+    Add file new_collection/sample1.mp3 to playlist? [Y/n]:y
+    Add file new_collection/sample2.mp3 to playlist? [Y/n]:Y
+    Add file new_collection/sample3.mp3 to playlist? [Y/n]:n
+    Add file new_collection/sample4.mp3 to playlist? [Y/n]:N
+    ```
 
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
 from make_playlist import *
```

### Comparing `make_playlist-1.8.0/make_playlist.egg-info/PKG-INFO` & `make_playlist-1.9.0/make_playlist.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: make-playlist
-Version: 1.8.0
+Name: make_playlist
+Version: 1.9.0
 Summary: Make M3U format playlist from command line.
 Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Project-URL: homepage, https://github.com/MatteoGuadrini/mkpl
 Project-URL: documentation, https://matteoguadrini.github.io/mkpl/
 Project-URL: changelog, https://github.com/MatteoGuadrini/mkpl/blob/master/CHANGES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: mutagen
 
 # ``make_playlist``: Playlist maker
 
 <img src="img/mkpl_logo.svg" alt="mkpl" title="mkpl" width="200" height="200" />
 
 ``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
@@ -34,40 +35,44 @@
 $ pip install .                           # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
-| short | long            | description                                   | args                      |
-|-------|-----------------|-----------------------------------------------|---------------------------|
-| -d    | --directories   | Directories that contains multimedia file     | Path of directories       |
-| -e    | --exclude-dirs  | Exclude directory paths                       | Path of directories       |
-| -i    | --include       | Include other file format                     | Format of file. ex. mp3   |
-| -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
-| -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
-| -s    | --size          | Start size in bytes                           | Bytes number              |
-| -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
-| -t    | --title         | Playlist title                                | Title string              |
-| -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
-| -I    | --image         | Playlist image                                | Image path                |
-| -l    | --link          | Add local or remote files                     | Files                     |
-| -j    | --join          | Join one or more other playlist files         | Playlist files            |
-| -r    | --recursive     | Recursive search                              |                           |
-| -a    | --absolute      | Absolute file name                            |                           |
-| -s    | --shuffle       | Casual order                                  |                           |
-| -u    | --unique        | The same files are not placed in the playlist |                           |
-| -c    | --append        | Continue playlist instead of override it      |                           |
-| -w    | --windows       | Windows style folder separator                |                           |
-| -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
-| -S    | --split         | Split playlist by directories                 |                           |
-| -o    | --orderby-name  | Order playlist files by name                  |                           |
-| -O    | --orderby-date  | Order playlist files by creation date         |                           |
-| -T    | --orderby-track | Order playlist files by track                 |                           |
-| -y    | --orderby-year  | Order playlist files by year                  |                           |
+| short | long             | description                                   | args                      |
+|-------|------------------|-----------------------------------------------|---------------------------|
+| -d    | --directories    | Directories that contains multimedia file     | Path of directories       |
+| -e    | --exclude-dirs   | Exclude directory paths                       | Path of directories       |
+| -i    | --include        | Include other file format                     | Format of file. ex. mp3   |
+| -p    | --pattern        | Regular expression inclusion pattern          | Regular expression string |
+| -f    | --format         | Select only a file format                     | Format of file. ex. mp3   |
+| -s    | --size           | Start size in bytes                           | Bytes number              |
+| -m    | --max-tracks     | Maximum number of tracks                      | Number                    |
+| -t    | --title          | Playlist title                                | Title string              |
+| -g    | --encoding       | Text encoding                                 | UTF-8,ASCII,UNICODE       |
+| -I    | --image          | Playlist image                                | Image path                |
+| -l    | --link           | Add local or remote files                     | Files                     |
+| -j    | --join           | Join one or more other playlist files         | Playlist files            |
+| -r    | --recursive      | Recursive search                              |                           |
+| -a    | --absolute       | Absolute file name                            |                           |
+| -s    | --shuffle        | Casual order                                  |                           |
+| -u    | --unique         | The same files are not placed in the playlist |                           |
+| -c    | --append         | Continue playlist instead of override it      |                           |
+| -w    | --windows        | Windows style folder separator                |                           |
+| -v    | --verbose        | Enable verbosity (debug mode)                 |                           |
+| -S    | --split          | Split playlist by directories                 |                           |
+| -R    | --interactive    | Asks each file for confirmation               |                           |
+| -C    | --count          | Count elements into playlist                  |                           |
+| -o    | --orderby-name   | Order playlist files by name                  |                           |
+| -O    | --orderby-date   | Order playlist files by creation date         |                           |
+| -T    | --orderby-track  | Order playlist files by track                 |                           |
+| -y    | --orderby-year   | Order playlist files by year                  |                           |
+| -Z    | --orderby-size   | Order playlist files by size                  |                           |
+| -L    | --orderby-length | Order playlist files by length                |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -158,27 +163,47 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`) or by year (`-y`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`), by year (`-y`), by size (`-Z`) or by length (`-L`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
     mkpl -d "new_collection" -r "my music.m3u" -T
     mkpl -d "new_collection" -r "my music.m3u" -y
+    mkpl -d "new_collection" -r "my music.m3u" -Z
+    mkpl -d "new_collection" -r "my music.m3u" -L
     ```
 
 16. Join the _"First playlist.m3u"_ and  _"Second playlist.m3u8"_ with new **"Third playlist.m3u"**:
 
     ```bash
     mkpl -d "new_collection" -r "Third playlist" -j "First playlist.m3u" "Second playlist.m3u8"
+    ```
+
+17. Counts the multimedia files:
+
+    ```console
+    mkpl -d "new_collection" -r "My new collection" -C
+    4023
+    ```
+
+18. Asks confirmation for every file into folders:
+
+    ```console
+    mkpl -d "new_collection" -r "My new collection" -R
+    Add file new_collection/sample1.mp3 to playlist? [Y/n]:y
+    Add file new_collection/sample2.mp3 to playlist? [Y/n]:Y
+    Add file new_collection/sample3.mp3 to playlist? [Y/n]:n
+    Add file new_collection/sample4.mp3 to playlist? [Y/n]:N
+    ```
 
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
 from make_playlist import *
```

### Comparing `make_playlist-1.8.0/mkpl.py` & `make_playlist-1.9.0/mkpl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # mkpl -- mkpl
 #
-#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2024 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -67,15 +67,15 @@
     "vob",
     "asf",
     "m4v",
     "3gp",
     "f4a",
 }
 FILE_FORMAT = AUDIO_FORMAT.union(VIDEO_FORMAT)
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 
 # endregion
 
 
 # region functions
 def get_args():
@@ -147,23 +147,23 @@
     )
     parser.add_argument("-I", "--image", help="Playlist image", default=None)
     parser.add_argument(
         "-l",
         "--link",
         help="Add local or remote file links",
         nargs=argparse.ONE_OR_MORE,
-        metavar='FILES',
+        metavar="FILES",
         default=[],
     )
     parser.add_argument(
         "-j",
         "--join",
         help="Join one or more other playlist files",
         nargs=argparse.ONE_OR_MORE,
-        metavar='PLAYLISTS',
+        metavar="PLAYLISTS",
         default=[],
     )
     parser.add_argument(
         "-r", "--recursive", help="Recursive search", action="store_true"
     )
     parser.add_argument(
         "-a", "--absolute", help="Absolute file name", action="store_true"
@@ -182,14 +182,23 @@
     )
     parser.add_argument(
         "-w", "--windows", help="Windows style folder separator", action="store_true"
     )
     parser.add_argument(
         "-S", "--split", help="Split playlist by directories", action="store_true"
     )
+    parser.add_argument(
+        "-R",
+        "--interactive",
+        help="Asks each file for confirmation",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-C", "--count", help="Count elements into playlist", action="store_true"
+    )
     orderby_group.add_argument(
         "-s", "--shuffle", help="Casual order", action="store_true"
     )
     orderby_group.add_argument(
         "-o", "--orderby-name", help="Order playlist files by name", action="store_true"
     )
     orderby_group.add_argument(
@@ -203,14 +212,26 @@
     )
     orderby_group.add_argument(
         "-y",
         "--orderby-year",
         help="Order playlist files by year",
         action="store_true",
     )
+    orderby_group.add_argument(
+        "-Z",
+        "--orderby-size",
+        help="Order playlist files by size",
+        action="store_true",
+    )
+    orderby_group.add_argument(
+        "-L",
+        "--orderby-length",
+        help="Order playlist files by length",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
     # Check extension of playlist file
     if not args.playlist.endswith(".m3u"):
         if args.encoding == "UNICODE":
             if not args.playlist.endswith(".m3u8"):
@@ -261,14 +282,36 @@
     # Select only one format
     if args.format:
         FILE_FORMAT = {args.format.strip("*").strip(".")}
 
     return args
 
 
+def confirm(file, default="y"):
+    """Ask user to enter Y or N (case-insensitive)
+
+    :file: file to add into playlist
+    :default: default answer
+    :return: True if the answer is Y.
+    :rtype: bool
+    """
+    while (
+        answer := input(
+            "Add file {0} to playlist? {1}:".format(
+                file, "[Y/n]" if default == "y" else "[y/N]"
+            )
+        ).lower()
+    ) not in ("y", "n"):
+        # Check if default
+        if not answer:
+            answer = default
+            break
+    return answer == "y"
+
+
 def file_in_playlist(playlist, file, root=None):
     """Check if file is in the playlist"""
     for f in playlist:
         # Skip extended tags
         if f.startswith("#"):
             continue
         # Check if absolute path in playlist
@@ -283,15 +326,17 @@
 
 def join_playlist(playlist, *others):
     """Join current playlist with others"""
     for file in others:
         try:
             # open playlist, remove extensions and extend current playlist file
             lines = open(file).readlines()
-            playlist.extend([line.rstrip() for line in lines if not line.startswith('#')])
+            playlist.extend(
+                [line.rstrip() for line in lines if not line.startswith("#")]
+            )
         except FileNotFoundError:
             print(f"warning: {file} file not found")
         except OSError as err:
             print(f"warning: {file} generated error: {err}")
 
 
 def report_issue(exc):
@@ -329,29 +374,36 @@
     """Get file by year for sort"""
     file = open_multimedia_file(file)
     if file and hasattr(file, "tags"):
         default = id3.TDOR(text="0")
         return file.tags.get("TDOR", default)[0]
 
 
+def get_length(file):
+    """Get file by length for sort"""
+    file = open_multimedia_file(file)
+    if file and hasattr(file, "info"):
+        return file.info.length if hasattr(file.info, "length") else 0.0
+
+
 def find_pattern(pattern, path):
     """Find patter in a file and tags"""
     global AUDIO_FORMAT
 
     # Create compiled pattern
     if not isinstance(pattern, re.Pattern):
         pattern = re.compile(pattern)
     # Check pattern into filename
     if pattern.findall(path):
         return True
     # Check type of file
-    ext = os.path.splitext(path)[1].replace('.', '').lower()
+    ext = os.path.splitext(path)[1].replace(".", "").lower()
     if ext in AUDIO_FORMAT:
         file = open_multimedia_file(path)
-        # Check supports of ID3 tagsadd compiled pattern
+        # Check supports of ID3 tags add compiled pattern
         if file and hasattr(file, "ID3"):
             # Check pattern into title
             if file.tags.get("TIT2"):
                 if pattern.findall(file.tags.get("TIT2")[0]):
                     return True
             # Check pattern into album
             if file.tags.get("TALB"):
@@ -377,31 +429,31 @@
     else:
         old_sep = "/"
         new_sep = r"\\"
     return sub(old_sep, new_sep, path)
 
 
 def write_playlist(
-        playlist,
-        open_mode,
-        files,
-        encoding,
-        enabled_extensions=False,
-        image=None,
-        ext_part=None,
-        max_tracks=None,
-        verbose=False,
+    playlist,
+    open_mode,
+    files,
+    encoding,
+    enabled_extensions=False,
+    image=None,
+    ext_part=None,
+    max_tracks=None,
+    verbose=False,
 ):
     """Write playlist into file"""
     if playlist:
         with open(
-                playlist,
-                mode=open_mode,
-                encoding="UTF-8" if encoding == "UNICODE" else encoding,
-                errors="ignore",
+            playlist,
+            mode=open_mode,
+            encoding="UTF-8" if encoding == "UNICODE" else encoding,
+            errors="ignore",
         ) as pl:
             if image and enabled_extensions:
                 vprint(verbose, f"set image {image}")
                 joined_string = f"\n#EXTIMG: {image}\n"
             else:
                 joined_string = "\n"
             end_file_string = "\n"
@@ -410,28 +462,31 @@
                 pl.write("\n".join(files[:ext_part]) + joined_string)
             # Write all multimedia files
             vprint(verbose, f"write playlist {pl.name}")
             pl.write(joined_string.join(files[ext_part:max_tracks]) + end_file_string)
 
 
 def make_playlist(
-        directory,
-        file_formats,
-        pattern=None,
-        sortby_name=False,
-        sortby_date=False,
-        sortby_track=False,
-        sortby_year=False,
-        recursive=False,
-        exclude_dirs=None,
-        unique=False,
-        absolute=False,
-        min_size=1,
-        windows=False,
-        verbose=False,
+    directory,
+    file_formats,
+    pattern=None,
+    sortby_name=False,
+    sortby_date=False,
+    sortby_track=False,
+    sortby_year=False,
+    sortby_size=False,
+    sortby_length=False,
+    recursive=False,
+    exclude_dirs=None,
+    unique=False,
+    absolute=False,
+    min_size=1,
+    windows=False,
+    interactive=False,
+    verbose=False,
 ):
     """Make playlist list"""
     filelist = list()
     # Check if directory exists
     if not exists(directory):
         print(f"warning: {directory} does not exists")
         return filelist
@@ -461,31 +516,38 @@
                     continue
             # Check if in exclude dirs
             if any([e_path in file for e_path in exclude_dirs]):
                 continue
             # Check if file is in playlist
             if unique:
                 if file_in_playlist(
-                        filelist, file, root=root if not absolute else None
+                    filelist, file, root=root if not absolute else None
                 ):
                     continue
             # Check file size
             if size <= min_size:
                 continue
+            if interactive:
+                if not confirm(file):
+                    continue
             vprint(verbose, f"add multimedia file {file}")
             filelist.append(unix_to_dos(file) if windows else file)
     # Check sort
     if sortby_name:
         filelist = sorted(filelist)
     elif sortby_date:
         filelist = sorted(filelist, key=getctime)
     elif sortby_track:
         filelist = sorted(filelist, key=get_track)
     elif sortby_year:
         filelist = sorted(filelist, key=get_year)
+    elif sortby_size:
+        filelist = sorted(filelist, key=os.path.getsize)
+    elif sortby_length:
+        filelist = sorted(filelist, key=get_length)
     return filelist
 
 
 def add_extension(filelist, cli_args, verbose=False):
     """Add extension to playlist list"""
     if not isinstance(filelist, list):
         raise ValueError(f"{filelist} is not a list object")
@@ -581,20 +643,23 @@
                 directory,
                 FILE_FORMAT,
                 args.pattern,
                 sortby_name=args.orderby_name,
                 sortby_date=args.orderby_date,
                 sortby_track=args.orderby_track,
                 sortby_year=args.orderby_year,
+                sortby_size=args.orderby_size,
+                sortby_length=args.orderby_length,
                 recursive=args.recursive,
                 exclude_dirs=args.exclude_dirs,
                 unique=args.unique,
                 absolute=args.absolute,
                 min_size=args.size,
                 windows=args.windows,
+                interactive=args.interactive,
                 verbose=args.verbose,
             )
 
             multimedia_files.extend(directory_files)
 
             # Check if you must split into directory playlist
             if args.split:
@@ -604,14 +669,18 @@
                     dirname(args.playlist), playlist_name + playlist_ext
                 )
                 _process_playlist(directory_files, args, playlist_path)
                 args.enabled_extensions = False
 
         _process_playlist(multimedia_files, args)
 
+        # Count files into playlist
+        if args.count:
+            print(len([file for file in multimedia_files if not file.startswith("#")]))
+
     except Exception as err:
         report_issue(err)
 
 
 # endregion
 
 # region main
```

### Comparing `make_playlist-1.8.0/pyproject.toml` & `make_playlist-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["mkpl"]
 
 [project]
 name = "make_playlist"
-version = "1.8.0"
+version = "1.9.0"
 readme = "README.md"
 
 authors = [{ name = "Matteo Guadrini", email = "matteo.guadrini@hotmail.it" }]
 maintainers = [
     { name = "Matteo Guadrini", email = "matteo.guadrini@hotmail.it" },
 ]
 
 description = "Make M3U format playlist from command line."
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = ["mutagen"]
```

