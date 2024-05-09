# Comparing `tmp/ptwebdiscover-1.0.5.tar.gz` & `tmp/ptwebdiscover-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptwebdiscover-1.0.5.tar", last modified: Thu Feb 22 23:57:32 2024, max compression
+gzip compressed data, was "ptwebdiscover-1.0.6.tar", last modified: Thu May  9 13:23:30 2024, max compression
```

## Comparing `ptwebdiscover-1.0.5.tar` & `ptwebdiscover-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 23:57:32.811788 ptwebdiscover-1.0.5/
--rw-rw-rw-   0        0        0    35823 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       40 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8194 2024-02-22 23:57:32.810786 ptwebdiscover-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7494 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 23:57:32.689244 ptwebdiscover-1.0.5/ptwebdiscover/
--rw-rw-rw-   0        0        0        0 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/__init__.py
--rw-rw-rw-   0        0        0       22 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/_version.py
--rw-rw-rw-   0        0        0      369 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/findings.py
--rw-rw-rw-   0        0        0      519 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/keyspace.py
-drwxrwxrwx   0        0        0        0 2024-02-22 23:57:32.766789 ptwebdiscover-1.0.5/ptwebdiscover/ptdataclasses/
--rw-rw-rw-   0        0        0        0 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/ptdataclasses/__init__.py
--rw-rw-rw-   0        0        0     1068 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/ptdataclasses/argumentoptions.py
--rw-rw-rw-   0        0        0      192 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/ptdataclasses/findingdetail.py
--rw-rw-rw-   0        0        0      343 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/ptdataclasses/processedargumentoptions.py
--rw-rw-rw-   0        0        0    48566 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/ptwebdiscover.py
--rw-rw-rw-   0        0        0    11506 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/responseprocessing.py
-drwxrwxrwx   0        0        0        0 2024-02-22 23:57:32.805784 ptwebdiscover-1.0.5/ptwebdiscover/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/utils/__init__.py
--rw-rw-rw-   0        0        0     9605 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/utils/cachefile.py
--rw-rw-rw-   0        0        0     2069 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/utils/treeshow.py
--rw-rw-rw-   0        0        0     1939 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/ptwebdiscover/utils/url.py
-drwxrwxrwx   0        0        0        0 2024-02-22 23:57:32.807785 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/
--rw-rw-rw-   0        0        0     8194 2024-02-22 23:57:32.000000 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-02-22 23:57:32.000000 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 23:57:32.000000 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-02-22 23:57:32.000000 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-02-22 23:57:32.000000 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-22 23:57:32.000000 ptwebdiscover-1.0.5/ptwebdiscover.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 23:57:32.812790 ptwebdiscover-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-02-22 23:56:06.000000 ptwebdiscover-1.0.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/LICENSE
+-rwxr-xr-x   0 kali      (1000) kali      (1000)       40 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     7626 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     7105 2024-05-09 13:20:59.000000 ptwebdiscover-1.0.6/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       22 2024-05-09 13:20:56.000000 ptwebdiscover-1.0.6/ptwebdiscover/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      369 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/findings.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      519 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/keyspace.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/__init__.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1068 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/argumentoptions.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      192 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/findingdetail.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      343 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/processedargumentoptions.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    48565 2024-04-30 07:58:41.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptwebdiscover.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    11506 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/responseprocessing.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/utils/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/
+-rw-r--r--   0 kali      (1000) kali      (1000)      182 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     4314 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     3949 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/url.cpython-311.pyc
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     9605 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/cachefile.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2069 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/treeshow.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1935 2024-05-09 13:16:29.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/url.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7626 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      911 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       67 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1043 2024-05-09 13:21:00.000000 ptwebdiscover-1.0.6/setup.py
```

### Comparing `ptwebdiscover-1.0.5/LICENSE` & `ptwebdiscover-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.5/PKG-INFO` & `ptwebdiscover-1.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,27 @@
-Metadata-Version: 2.1
-Name: ptwebdiscover
-Version: 1.0.5
-Summary: Web Source Discovery Tool
-Home-page: https://www.penterep.com/
-Author: Penterep
-Author-email: info@penterep.com
-License: GPLv3+
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Environment :: Console
-Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ptlibs<2,>=1.0.6
-Requires-Dist: requests
-Requires-Dist: appdirs
-Requires-Dist: treelib
-Requires-Dist: filelock
-
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTWEBDISCOVER
-> Web Source Discovery Tool
+## PTWEBDISCOVER - Web Source Discovery Tool
 
 ## Installation
-
 ```
 pip install ptwebdiscover
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
 source ~/.zshrc
 ```
 
 ## Usage examples
 ```
@@ -61,15 +37,15 @@
 ptwebdiscover -u https://www.example.com -E extensions.txt
 ptwebdiscover -u https://www.example.com -w -sn "Page Not Found"
 ```
 
 ## Options
 ```
 -u    --url                     <url>           URL for test (usage of a star character as anchor)
--ch   --charsets                <charsets>      Specify charset for brute force (example: lowercase,uppercase,numbers,[custom_chars])
+-ch   --charsets                <charsets>      Specify charset fro brute force (example: lowercase,uppercase,numbers,[custom_chars])
                                                 Modify wordlist (lowercase,uppercase,capitalize)
 -lm   --length-min              <length-min>    Minimal length of brute-force tested string (default 1)
 -lx   --length-max              <length-max>    Maximal length of brute-force tested string (default 6 bf / 99 wl
 -w    --wordlist                <filename>      Use specified wordlist(s)
 -pf   --prefix                  <string>        Use prefix before tested string
 -sf   --suffix                  <string>        Use suffix after tested string
 -bw   --begin-with              <string>        Use only words from wordlist that begin with the specified string
@@ -111,45 +87,25 @@
 -nr   --not-redirect                            Do not follow redirects
 -s    --silent                                  Do not show statistics in realtime
 -er   --errors                                  Show all errors
 -C    --cache                                   Cache each request response to temp file
 -v    --version                                 Show script version
 -h    --help                                    Show this help message
 -j    --json                                    Output in JSON format
-
 ```
 
 ## Dependencies
 ```
-requests
+ptlibs
 appdirs
 treelib
-ptlibs
+filelock
 ```
 
-## Version History
-```
-1.0.5
-    - Added custom tldparser
-1.0.1 - 1.0.4
-    - Added JSON support
-    - Removed deprecated SSL settings
-1.0.0
-    - Code improvements
-    - Updated for latest ptlibs
-0.0.5
-    - Updated prints for new ptlibs
-0.0.4
-    - Disabled availability check, when star in url
-0.0.3
-    - Fixed case sensitivity in wordlists
-    - Added .7z and .tgz extensions to backups search
-0.0.1 - 0.0.2
-    - Alpha releases
-```
+
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
 
 ptwebdiscover is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
```

### Comparing `ptwebdiscover-1.0.5/README.md` & `ptwebdiscover-1.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,144 +1,143 @@
-[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
-
-
-# PTWEBDISCOVER
-> Web Source Discovery Tool
-
-## Installation
-
-```
-pip install ptwebdiscover
-```
-
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
-
-> Add to PATH for Bash
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
-source ~/.bashrc
-```
-
-> Add to PATH for ZSH
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
-source ~/.zshrc
-```
-
-## Usage examples
-```
-ptwebdiscover -u https://www.example.com
-ptwebdiscover -u https://www.example.com -ch lowercase,numbers,123abcdEFG*
-ptwebdiscover -u https://www.example.com -lx 4
-ptwebdiscover -u https://www.example.com -w
-ptwebdiscover -u https://www.example.com -w wordlist.txt
-ptwebdiscover -u https://www.example.com -w wordlist.txt --begin_with admin
-ptwebdiscover -u https://*.example.com -w
-ptwebdiscover -u https://www.example.com/exam*.txt
-ptwebdiscover -u https://www.example.com -e "" bak old php~ php.bak
-ptwebdiscover -u https://www.example.com -E extensions.txt
-ptwebdiscover -u https://www.example.com -w -sn "Page Not Found"
-```
-
-## Options
-```
--u    --url                     <url>           URL for test (usage of a star character as anchor)
--ch   --charsets                <charsets>      Specify charset for brute force (example: lowercase,uppercase,numbers,[custom_chars])
-                                                Modify wordlist (lowercase,uppercase,capitalize)
--lm   --length-min              <length-min>    Minimal length of brute-force tested string (default 1)
--lx   --length-max              <length-max>    Maximal length of brute-force tested string (default 6 bf / 99 wl
--w    --wordlist                <filename>      Use specified wordlist(s)
--pf   --prefix                  <string>        Use prefix before tested string
--sf   --suffix                  <string>        Use suffix after tested string
--bw   --begin-with              <string>        Use only words from wordlist that begin with the specified string
--ci   --case-insensitive                        Case insensitive items from wordlist
--e    --extensions              <extensions>    Add extensions behind a tested string ("" for empty extension)
--E    --extension-file          <filename>      Add extensions from default or specified file behind a tested string.
--r    --recurse                                 Recursive browsing of found directories
--md   --max_depth               <integer>       Maximum depth during recursive browsing (default: 20)
--b    --backups                                 Find backups for db, all app and every discovered content
--bo   --backups-only                            Find backup of complete website only
--P    --parse                                   Parse HTML response for URLs discovery
--Po   --parse-only                              Brute force method is disabled, crawling started on specified url
--D    --directory                               Add a slash at the ends of the strings too
--nd   --not-directories         <directories>   Not include listed directories when recursive browse run
--sy   --string-in-response      <string>        Print findings only if string in response (GET method is used)
--sn   --string-not-in-response  <string>        Print findings only if string not in response (GET method is used)
--sc   --status-codes            <status codes>  Ignore response with status codes (default 404)
--m    --method                  <method>        Use said HTTP method (default: HEAD)
--se   --scheme                  <scheme>        Use scheme when missing (default: http)
--d    --delay                   <miliseconds>   Delay before each request in seconds
--p    --proxy                   <proxy>         Use proxy (e.g. http://127.0.0.1:8080)
--T    --timeout                 <miliseconds>   Manually set timeout (default 10000)
--cl   --content-length          <kilobytes>     Max content length to download and parse (default: 1000KB)
--H    --headers                 <headers>       Use custom headers
--ua   --user-agent              <agent>         Use custom value of User-Agent header
--c    --cookie                  <cookies>       Use cookie (-c "PHPSESSID=abc; any=123")
--rc   --refuse-cookies                          Do not use cookies sets by application
--a    --auth                    <name:pass>     Use HTTP authentication
--t    --threads                 <threads>       Number of threads (default 20)
--wd   --without-domain                          Output of discovered sources without domain
--wh   --with-headers                            Output of discovered sources with headers
--ip   --include-parameters                      Include GET parameters and anchors to output
--tr   --tree                                    Output as tree
--o    --output                  <filename>      Output to file
--S    --save                    <directory>     Save content localy
--wdc  --without_dns_cache                       Do not use DNS cache (example for /etc/hosts records)
--wa   --without_availability                    Do not use target availability check
--tg   --target                  <ip or host>    Use this target when * is in domain
--nr   --not-redirect                            Do not follow redirects
--s    --silent                                  Do not show statistics in realtime
--er   --errors                                  Show all errors
--C    --cache                                   Cache each request response to temp file
--v    --version                                 Show script version
--h    --help                                    Show this help message
--j    --json                                    Output in JSON format
-
-```
-
-## Dependencies
-```
-requests
-appdirs
-treelib
-ptlibs
-```
-
-## Version History
-```
-1.0.5
-    - Added custom tldparser
-1.0.1 - 1.0.4
-    - Added JSON support
-    - Removed deprecated SSL settings
-1.0.0
-    - Code improvements
-    - Updated for latest ptlibs
-0.0.5
-    - Updated prints for new ptlibs
-0.0.4
-    - Disabled availability check, when star in url
-0.0.3
-    - Fixed case sensitivity in wordlists
-    - Added .7z and .tgz extensions to backups search
-0.0.1 - 0.0.2
-    - Alpha releases
-```
-
-## License
-
-Copyright (c) 2024 Penterep Security s.r.o.
-
-ptwebdiscover is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-ptwebdiscover is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with ptwebdiscover. If not, see https://www.gnu.org/licenses/.
-
-## Warning
-
-You are only allowed to run the tool against the websites which
-you have been given permission to pentest. We do not accept any
-responsibility for any damage/harm that this application causes to your
-computer, or your network. Penterep is not responsible for any illegal
-or malicious use of this code. Be Ethical!
+Metadata-Version: 2.1
+Name: ptwebdiscover
+Version: 1.0.6
+Summary: Web Source Discovery Tool
+Home-page: https://www.penterep.com/
+Author: Penterep
+Author-email: info@penterep.com
+License: GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1.0.7
+Requires-Dist: appdirs
+Requires-Dist: treelib
+Requires-Dist: filelock
+
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
+
+## PTWEBDISCOVER - Web Source Discovery Tool
+
+## Installation
+```
+pip install ptwebdiscover
+```
+
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
+
+For Bash Users
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
+source ~/.bashrc
+```
+
+For ZSH Users
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
+```
+
+## Usage examples
+```
+ptwebdiscover -u https://www.example.com
+ptwebdiscover -u https://www.example.com -ch lowercase,numbers,123abcdEFG*
+ptwebdiscover -u https://www.example.com -lx 4
+ptwebdiscover -u https://www.example.com -w
+ptwebdiscover -u https://www.example.com -w wordlist.txt
+ptwebdiscover -u https://www.example.com -w wordlist.txt --begin_with admin
+ptwebdiscover -u https://*.example.com -w
+ptwebdiscover -u https://www.example.com/exam*.txt
+ptwebdiscover -u https://www.example.com -e "" bak old php~ php.bak
+ptwebdiscover -u https://www.example.com -E extensions.txt
+ptwebdiscover -u https://www.example.com -w -sn "Page Not Found"
+```
+
+## Options
+```
+-u    --url                     <url>           URL for test (usage of a star character as anchor)
+-ch   --charsets                <charsets>      Specify charset fro brute force (example: lowercase,uppercase,numbers,[custom_chars])
+                                                Modify wordlist (lowercase,uppercase,capitalize)
+-lm   --length-min              <length-min>    Minimal length of brute-force tested string (default 1)
+-lx   --length-max              <length-max>    Maximal length of brute-force tested string (default 6 bf / 99 wl
+-w    --wordlist                <filename>      Use specified wordlist(s)
+-pf   --prefix                  <string>        Use prefix before tested string
+-sf   --suffix                  <string>        Use suffix after tested string
+-bw   --begin-with              <string>        Use only words from wordlist that begin with the specified string
+-ci   --case-insensitive                        Case insensitive items from wordlist
+-e    --extensions              <extensions>    Add extensions behind a tested string ("" for empty extension)
+-E    --extension-file          <filename>      Add extensions from default or specified file behind a tested string.
+-r    --recurse                                 Recursive browsing of found directories
+-md   --max_depth               <integer>       Maximum depth during recursive browsing (default: 20)
+-b    --backups                                 Find backups for db, all app and every discovered content
+-bo   --backups-only                            Find backup of complete website only
+-P    --parse                                   Parse HTML response for URLs discovery
+-Po   --parse-only                              Brute force method is disabled, crawling started on specified url
+-D    --directory                               Add a slash at the ends of the strings too
+-nd   --not-directories         <directories>   Not include listed directories when recursive browse run
+-sy   --string-in-response      <string>        Print findings only if string in response (GET method is used)
+-sn   --string-not-in-response  <string>        Print findings only if string not in response (GET method is used)
+-sc   --status-codes            <status codes>  Ignore response with status codes (default 404)
+-m    --method                  <method>        Use said HTTP method (default: HEAD)
+-se   --scheme                  <scheme>        Use scheme when missing (default: http)
+-d    --delay                   <miliseconds>   Delay before each request in seconds
+-p    --proxy                   <proxy>         Use proxy (e.g. http://127.0.0.1:8080)
+-T    --timeout                 <miliseconds>   Manually set timeout (default 10000)
+-cl   --content-length          <kilobytes>     Max content length to download and parse (default: 1000KB)
+-H    --headers                 <headers>       Use custom headers
+-ua   --user-agent              <agent>         Use custom value of User-Agent header
+-c    --cookie                  <cookies>       Use cookie (-c "PHPSESSID=abc; any=123")
+-rc   --refuse-cookies                          Do not use cookies sets by application
+-a    --auth                    <name:pass>     Use HTTP authentication
+-t    --threads                 <threads>       Number of threads (default 20)
+-wd   --without-domain                          Output of discovered sources without domain
+-wh   --with-headers                            Output of discovered sources with headers
+-ip   --include-parameters                      Include GET parameters and anchors to output
+-tr   --tree                                    Output as tree
+-o    --output                  <filename>      Output to file
+-S    --save                    <directory>     Save content localy
+-wdc  --without_dns_cache                       Do not use DNS cache (example for /etc/hosts records)
+-wa   --without_availability                    Do not use target availability check
+-tg   --target                  <ip or host>    Use this target when * is in domain
+-nr   --not-redirect                            Do not follow redirects
+-s    --silent                                  Do not show statistics in realtime
+-er   --errors                                  Show all errors
+-C    --cache                                   Cache each request response to temp file
+-v    --version                                 Show script version
+-h    --help                                    Show this help message
+-j    --json                                    Output in JSON format
+```
+
+## Dependencies
+```
+ptlibs
+appdirs
+treelib
+filelock
+```
+
+
+
+## License
+
+Copyright (c) 2024 Penterep Security s.r.o.
+
+ptwebdiscover is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+ptwebdiscover is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with ptwebdiscover. If not, see https://www.gnu.org/licenses/.
+
+## Warning
+
+You are only allowed to run the tool against the websites which
+you have been given permission to pentest. We do not accept any
+responsibility for any damage/harm that this application causes to your
+computer, or your network. Penterep is not responsible for any illegal
+or malicious use of this code. Be Ethical!
```

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/keyspace.py` & `ptwebdiscover-1.0.6/ptwebdiscover/keyspace.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/ptdataclasses/argumentoptions.py` & `ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/argumentoptions.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/ptwebdiscover.py` & `ptwebdiscover-1.0.6/ptwebdiscover/ptwebdiscover.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from _version import __version__
 
 
 class PtWebDiscover():
     def __init__(self, args: ArgumentOptions) -> None:
         self.args: ProcessedArgumentOptions                         = args
         self.args.timeout                                           = args.timeout / 1000
-        self.args.content_length                                    = args.content_length * 1000 
+        self.args.content_length                                    = args.content_length * 1000
         self.args.delay                                             = args.delay / 1000
         self.args.is_star                                           = True if "*" in args.url else False
         self.args.nochanged_url                                     = self.args.url
         self.args.url                                               = ptnethelper.remove_slash_from_end_url(args.url) if not self.args.is_star else args.url
         self.args.url                                               = Url(args.url).add_missing_scheme(self.args.scheme)
         self.args.target                                            = Url(args.target).add_missing_scheme(self.args.scheme)
         self.args.position, self.args.url                           = self.get_star_position(self.args.url)
```

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/responseprocessing.py` & `ptwebdiscover-1.0.6/ptwebdiscover/responseprocessing.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/utils/cachefile.py` & `ptwebdiscover-1.0.6/ptwebdiscover/utils/cachefile.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/utils/treeshow.py` & `ptwebdiscover-1.0.6/ptwebdiscover/utils/treeshow.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover/utils/url.py` & `ptwebdiscover-1.0.6/ptwebdiscover/utils/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if not path.startswith("/"):
             path = "/"
         abs = os.path.abspath(path)+"/" if path.endswith("/") and path !="/" else os.path.abspath(path)
         return domain_with_protocol + abs
 
 
     def get_domain_from_url(self, level=True, with_protocol=True) -> str:
-        extract = tldparser.parse_url(self.url)
+        extract = tldparser.parse(self.url)
         if extract.subdomain:
             extract.subdomain += "."
         if with_protocol:
             protocol = extract.scheme + "://" if extract.scheme else "http://"
         else:
             protocol = ""
         if level:
```

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover.egg-info/PKG-INFO` & `ptwebdiscover-1.0.6/ptwebdiscover.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,166 +1,143 @@
-Metadata-Version: 2.1
-Name: ptwebdiscover
-Version: 1.0.5
-Summary: Web Source Discovery Tool
-Home-page: https://www.penterep.com/
-Author: Penterep
-Author-email: info@penterep.com
-License: GPLv3+
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Environment :: Console
-Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ptlibs<2,>=1.0.6
-Requires-Dist: requests
-Requires-Dist: appdirs
-Requires-Dist: treelib
-Requires-Dist: filelock
-
-[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
-
-
-# PTWEBDISCOVER
-> Web Source Discovery Tool
-
-## Installation
-
-```
-pip install ptwebdiscover
-```
-
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
-
-> Add to PATH for Bash
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
-source ~/.bashrc
-```
-
-> Add to PATH for ZSH
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
-source ~/.zshrc
-```
-
-## Usage examples
-```
-ptwebdiscover -u https://www.example.com
-ptwebdiscover -u https://www.example.com -ch lowercase,numbers,123abcdEFG*
-ptwebdiscover -u https://www.example.com -lx 4
-ptwebdiscover -u https://www.example.com -w
-ptwebdiscover -u https://www.example.com -w wordlist.txt
-ptwebdiscover -u https://www.example.com -w wordlist.txt --begin_with admin
-ptwebdiscover -u https://*.example.com -w
-ptwebdiscover -u https://www.example.com/exam*.txt
-ptwebdiscover -u https://www.example.com -e "" bak old php~ php.bak
-ptwebdiscover -u https://www.example.com -E extensions.txt
-ptwebdiscover -u https://www.example.com -w -sn "Page Not Found"
-```
-
-## Options
-```
--u    --url                     <url>           URL for test (usage of a star character as anchor)
--ch   --charsets                <charsets>      Specify charset for brute force (example: lowercase,uppercase,numbers,[custom_chars])
-                                                Modify wordlist (lowercase,uppercase,capitalize)
--lm   --length-min              <length-min>    Minimal length of brute-force tested string (default 1)
--lx   --length-max              <length-max>    Maximal length of brute-force tested string (default 6 bf / 99 wl
--w    --wordlist                <filename>      Use specified wordlist(s)
--pf   --prefix                  <string>        Use prefix before tested string
--sf   --suffix                  <string>        Use suffix after tested string
--bw   --begin-with              <string>        Use only words from wordlist that begin with the specified string
--ci   --case-insensitive                        Case insensitive items from wordlist
--e    --extensions              <extensions>    Add extensions behind a tested string ("" for empty extension)
--E    --extension-file          <filename>      Add extensions from default or specified file behind a tested string.
--r    --recurse                                 Recursive browsing of found directories
--md   --max_depth               <integer>       Maximum depth during recursive browsing (default: 20)
--b    --backups                                 Find backups for db, all app and every discovered content
--bo   --backups-only                            Find backup of complete website only
--P    --parse                                   Parse HTML response for URLs discovery
--Po   --parse-only                              Brute force method is disabled, crawling started on specified url
--D    --directory                               Add a slash at the ends of the strings too
--nd   --not-directories         <directories>   Not include listed directories when recursive browse run
--sy   --string-in-response      <string>        Print findings only if string in response (GET method is used)
--sn   --string-not-in-response  <string>        Print findings only if string not in response (GET method is used)
--sc   --status-codes            <status codes>  Ignore response with status codes (default 404)
--m    --method                  <method>        Use said HTTP method (default: HEAD)
--se   --scheme                  <scheme>        Use scheme when missing (default: http)
--d    --delay                   <miliseconds>   Delay before each request in seconds
--p    --proxy                   <proxy>         Use proxy (e.g. http://127.0.0.1:8080)
--T    --timeout                 <miliseconds>   Manually set timeout (default 10000)
--cl   --content-length          <kilobytes>     Max content length to download and parse (default: 1000KB)
--H    --headers                 <headers>       Use custom headers
--ua   --user-agent              <agent>         Use custom value of User-Agent header
--c    --cookie                  <cookies>       Use cookie (-c "PHPSESSID=abc; any=123")
--rc   --refuse-cookies                          Do not use cookies sets by application
--a    --auth                    <name:pass>     Use HTTP authentication
--t    --threads                 <threads>       Number of threads (default 20)
--wd   --without-domain                          Output of discovered sources without domain
--wh   --with-headers                            Output of discovered sources with headers
--ip   --include-parameters                      Include GET parameters and anchors to output
--tr   --tree                                    Output as tree
--o    --output                  <filename>      Output to file
--S    --save                    <directory>     Save content localy
--wdc  --without_dns_cache                       Do not use DNS cache (example for /etc/hosts records)
--wa   --without_availability                    Do not use target availability check
--tg   --target                  <ip or host>    Use this target when * is in domain
--nr   --not-redirect                            Do not follow redirects
--s    --silent                                  Do not show statistics in realtime
--er   --errors                                  Show all errors
--C    --cache                                   Cache each request response to temp file
--v    --version                                 Show script version
--h    --help                                    Show this help message
--j    --json                                    Output in JSON format
-
-```
-
-## Dependencies
-```
-requests
-appdirs
-treelib
-ptlibs
-```
-
-## Version History
-```
-1.0.5
-    - Added custom tldparser
-1.0.1 - 1.0.4
-    - Added JSON support
-    - Removed deprecated SSL settings
-1.0.0
-    - Code improvements
-    - Updated for latest ptlibs
-0.0.5
-    - Updated prints for new ptlibs
-0.0.4
-    - Disabled availability check, when star in url
-0.0.3
-    - Fixed case sensitivity in wordlists
-    - Added .7z and .tgz extensions to backups search
-0.0.1 - 0.0.2
-    - Alpha releases
-```
-
-## License
-
-Copyright (c) 2024 Penterep Security s.r.o.
-
-ptwebdiscover is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-ptwebdiscover is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with ptwebdiscover. If not, see https://www.gnu.org/licenses/.
-
-## Warning
-
-You are only allowed to run the tool against the websites which
-you have been given permission to pentest. We do not accept any
-responsibility for any damage/harm that this application causes to your
-computer, or your network. Penterep is not responsible for any illegal
-or malicious use of this code. Be Ethical!
+Metadata-Version: 2.1
+Name: ptwebdiscover
+Version: 1.0.6
+Summary: Web Source Discovery Tool
+Home-page: https://www.penterep.com/
+Author: Penterep
+Author-email: info@penterep.com
+License: GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1.0.7
+Requires-Dist: appdirs
+Requires-Dist: treelib
+Requires-Dist: filelock
+
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
+
+## PTWEBDISCOVER - Web Source Discovery Tool
+
+## Installation
+```
+pip install ptwebdiscover
+```
+
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
+
+For Bash Users
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
+source ~/.bashrc
+```
+
+For ZSH Users
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
+```
+
+## Usage examples
+```
+ptwebdiscover -u https://www.example.com
+ptwebdiscover -u https://www.example.com -ch lowercase,numbers,123abcdEFG*
+ptwebdiscover -u https://www.example.com -lx 4
+ptwebdiscover -u https://www.example.com -w
+ptwebdiscover -u https://www.example.com -w wordlist.txt
+ptwebdiscover -u https://www.example.com -w wordlist.txt --begin_with admin
+ptwebdiscover -u https://*.example.com -w
+ptwebdiscover -u https://www.example.com/exam*.txt
+ptwebdiscover -u https://www.example.com -e "" bak old php~ php.bak
+ptwebdiscover -u https://www.example.com -E extensions.txt
+ptwebdiscover -u https://www.example.com -w -sn "Page Not Found"
+```
+
+## Options
+```
+-u    --url                     <url>           URL for test (usage of a star character as anchor)
+-ch   --charsets                <charsets>      Specify charset fro brute force (example: lowercase,uppercase,numbers,[custom_chars])
+                                                Modify wordlist (lowercase,uppercase,capitalize)
+-lm   --length-min              <length-min>    Minimal length of brute-force tested string (default 1)
+-lx   --length-max              <length-max>    Maximal length of brute-force tested string (default 6 bf / 99 wl
+-w    --wordlist                <filename>      Use specified wordlist(s)
+-pf   --prefix                  <string>        Use prefix before tested string
+-sf   --suffix                  <string>        Use suffix after tested string
+-bw   --begin-with              <string>        Use only words from wordlist that begin with the specified string
+-ci   --case-insensitive                        Case insensitive items from wordlist
+-e    --extensions              <extensions>    Add extensions behind a tested string ("" for empty extension)
+-E    --extension-file          <filename>      Add extensions from default or specified file behind a tested string.
+-r    --recurse                                 Recursive browsing of found directories
+-md   --max_depth               <integer>       Maximum depth during recursive browsing (default: 20)
+-b    --backups                                 Find backups for db, all app and every discovered content
+-bo   --backups-only                            Find backup of complete website only
+-P    --parse                                   Parse HTML response for URLs discovery
+-Po   --parse-only                              Brute force method is disabled, crawling started on specified url
+-D    --directory                               Add a slash at the ends of the strings too
+-nd   --not-directories         <directories>   Not include listed directories when recursive browse run
+-sy   --string-in-response      <string>        Print findings only if string in response (GET method is used)
+-sn   --string-not-in-response  <string>        Print findings only if string not in response (GET method is used)
+-sc   --status-codes            <status codes>  Ignore response with status codes (default 404)
+-m    --method                  <method>        Use said HTTP method (default: HEAD)
+-se   --scheme                  <scheme>        Use scheme when missing (default: http)
+-d    --delay                   <miliseconds>   Delay before each request in seconds
+-p    --proxy                   <proxy>         Use proxy (e.g. http://127.0.0.1:8080)
+-T    --timeout                 <miliseconds>   Manually set timeout (default 10000)
+-cl   --content-length          <kilobytes>     Max content length to download and parse (default: 1000KB)
+-H    --headers                 <headers>       Use custom headers
+-ua   --user-agent              <agent>         Use custom value of User-Agent header
+-c    --cookie                  <cookies>       Use cookie (-c "PHPSESSID=abc; any=123")
+-rc   --refuse-cookies                          Do not use cookies sets by application
+-a    --auth                    <name:pass>     Use HTTP authentication
+-t    --threads                 <threads>       Number of threads (default 20)
+-wd   --without-domain                          Output of discovered sources without domain
+-wh   --with-headers                            Output of discovered sources with headers
+-ip   --include-parameters                      Include GET parameters and anchors to output
+-tr   --tree                                    Output as tree
+-o    --output                  <filename>      Output to file
+-S    --save                    <directory>     Save content localy
+-wdc  --without_dns_cache                       Do not use DNS cache (example for /etc/hosts records)
+-wa   --without_availability                    Do not use target availability check
+-tg   --target                  <ip or host>    Use this target when * is in domain
+-nr   --not-redirect                            Do not follow redirects
+-s    --silent                                  Do not show statistics in realtime
+-er   --errors                                  Show all errors
+-C    --cache                                   Cache each request response to temp file
+-v    --version                                 Show script version
+-h    --help                                    Show this help message
+-j    --json                                    Output in JSON format
+```
+
+## Dependencies
+```
+ptlibs
+appdirs
+treelib
+filelock
+```
+
+
+
+## License
+
+Copyright (c) 2024 Penterep Security s.r.o.
+
+ptwebdiscover is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+ptwebdiscover is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with ptwebdiscover. If not, see https://www.gnu.org/licenses/.
+
+## Warning
+
+You are only allowed to run the tool against the websites which
+you have been given permission to pentest. We do not accept any
+responsibility for any damage/harm that this application causes to your
+computer, or your network. Penterep is not responsible for any illegal
+or malicious use of this code. Be Ethical!
```

### Comparing `ptwebdiscover-1.0.5/ptwebdiscover.egg-info/SOURCES.txt` & `ptwebdiscover-1.0.6/ptwebdiscover.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 ptwebdiscover/ptdataclasses/__init__.py
 ptwebdiscover/ptdataclasses/argumentoptions.py
 ptwebdiscover/ptdataclasses/findingdetail.py
 ptwebdiscover/ptdataclasses/processedargumentoptions.py
 ptwebdiscover/utils/__init__.py
 ptwebdiscover/utils/cachefile.py
 ptwebdiscover/utils/treeshow.py
-ptwebdiscover/utils/url.py
+ptwebdiscover/utils/url.py
+ptwebdiscover/utils/__pycache__/__init__.cpython-311.pyc
+ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc
+ptwebdiscover/utils/__pycache__/url.cpython-311.pyc
```

### Comparing `ptwebdiscover-1.0.5/setup.py` & `ptwebdiscover-1.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 setuptools.setup(
     name="ptwebdiscover",
     description="Web Source Discovery Tool",
     url="https://www.penterep.com/",
     author="Penterep",
     author_email="info@penterep.com",
     version=__version__,
-    license="GPLv3+",
+    license="GPLv3",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Environment :: Console",
         "Topic :: Security",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     python_requires = '>=3.9',
-    install_requires=["ptlibs>=1.0.6,<2", "requests", "appdirs", "treelib", "filelock"],
+    install_requires=["ptlibs>=1.0.7,<2", "appdirs", "treelib", "filelock"],
     entry_points = {'console_scripts': ['ptwebdiscover = ptwebdiscover.ptwebdiscover:main']},
     include_package_data= True,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

