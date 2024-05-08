# Comparing `tmp/py_common_fetch-0.352.tar.gz` & `tmp/py_common_fetch-0.354.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_common_fetch-0.352.tar", last modified: Wed Apr 26 16:56:15 2023, max compression
+gzip compressed data, was "py_common_fetch-0.354.tar", last modified: Wed May  8 19:29:29 2024, max compression
```

## Comparing `py_common_fetch-0.352.tar` & `py_common_fetch-0.354.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-26 16:56:15.548262 py_common_fetch-0.352/
--rw-r--r--   0 greg       (501) staff       (20)     1535 2023-04-26 16:56:15.548132 py_common_fetch-0.352/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     1200 2018-05-11 19:03:10.000000 py_common_fetch-0.352/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-26 16:56:15.544474 py_common_fetch-0.352/aniachi/
--rw-r--r--   0 greg       (501) staff       (20)        0 2017-03-03 18:42:55.000000 py_common_fetch-0.352/aniachi/__init__.py
--rw-r--r--   0 greg       (501) staff       (20)     4500 2023-04-26 16:55:23.000000 py_common_fetch-0.352/aniachi/stringUtils.py
--rw-r--r--   0 greg       (501) staff       (20)    10495 2022-12-28 14:08:55.000000 py_common_fetch-0.352/aniachi/systemUtils.py
--rw-r--r--   0 greg       (501) staff       (20)     1291 2022-12-28 13:57:20.000000 py_common_fetch-0.352/aniachi/timeUtils.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-26 16:56:15.547914 py_common_fetch-0.352/py_common_fetch.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)     1535 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      337 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2018-05-11 03:32:51.000000 py_common_fetch-0.352/py_common_fetch.egg-info/not-zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       64 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/requires.txt
--rw-r--r--   0 greg       (501) staff       (20)        8 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)       38 2023-04-26 16:56:15.548308 py_common_fetch-0.352/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      987 2023-04-26 16:55:44.000000 py_common_fetch-0.352/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2024-05-08 19:29:29.513921 py_common_fetch-0.354/
+-rw-r--r--   0 greg       (501) staff       (20)     1704 2024-05-08 19:29:29.513599 py_common_fetch-0.354/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     1200 2018-05-11 19:03:10.000000 py_common_fetch-0.354/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2024-05-08 19:29:29.510279 py_common_fetch-0.354/aniachi/
+-rw-r--r--   0 greg       (501) staff       (20)        0 2017-03-03 18:42:55.000000 py_common_fetch-0.354/aniachi/__init__.py
+-rw-r--r--   0 greg       (501) staff       (20)     4500 2023-04-26 16:55:23.000000 py_common_fetch-0.354/aniachi/stringUtils.py
+-rw-r--r--   0 greg       (501) staff       (20)    11165 2024-05-08 18:22:54.000000 py_common_fetch-0.354/aniachi/systemUtils.py
+-rw-r--r--   0 greg       (501) staff       (20)     1291 2022-12-28 13:57:20.000000 py_common_fetch-0.354/aniachi/timeUtils.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2024-05-08 19:29:29.513285 py_common_fetch-0.354/py_common_fetch.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)     1704 2024-05-08 19:29:29.000000 py_common_fetch-0.354/py_common_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      337 2024-05-08 19:29:29.000000 py_common_fetch-0.354/py_common_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2024-05-08 19:29:29.000000 py_common_fetch-0.354/py_common_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2018-05-11 03:32:51.000000 py_common_fetch-0.354/py_common_fetch.egg-info/not-zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       64 2024-05-08 19:29:29.000000 py_common_fetch-0.354/py_common_fetch.egg-info/requires.txt
+-rw-r--r--   0 greg       (501) staff       (20)        8 2024-05-08 19:29:29.000000 py_common_fetch-0.354/py_common_fetch.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)       38 2024-05-08 19:29:29.513985 py_common_fetch-0.354/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      984 2024-05-08 18:24:00.000000 py_common_fetch-0.354/setup.py
```

### Comparing `py_common_fetch-0.352/PKG-INFO` & `py_common_fetch-0.354/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: py_common_fetch
-Version: 0.352
+Version: 0.354
 Summary: A really simple to use Python fetch screen
 Home-page: https://github.com/bygregonline/py-common-fetch
 Author: Greg flores
 Author-email: bygregonline@yahoo.com
 License: MIT
 Keywords: noefetch common information welcome screen
 Description-Content-Type: text/markdown
+Requires-Dist: pip
+Requires-Dist: psutil>=5.4.5
+Requires-Dist: json2html
+Requires-Dist: py-cpuinfo
+Requires-Dist: termcolor
+Requires-Dist: numpy
+Requires-Dist: tabulate
 
 # How to USE
 
 ```
 
 from aniachi.systemUtils import Welcome as W
 W.printWelcome()
```

### Comparing `py_common_fetch-0.352/README.md` & `py_common_fetch-0.354/README.md`

 * *Files identical despite different names*

### Comparing `py_common_fetch-0.352/aniachi/stringUtils.py` & `py_common_fetch-0.354/aniachi/stringUtils.py`

 * *Files identical despite different names*

### Comparing `py_common_fetch-0.352/aniachi/systemUtils.py` & `py_common_fetch-0.354/aniachi/systemUtils.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,128 +19,145 @@
 from termcolor import colored
 from tabulate import tabulate
 from aniachi import stringUtils, timeUtils
 
 # from pip._internal.utils.misc import get_installed_distributions
 
 
-
 class Welcome:
 
-    __version__=.322
-
-
+    __version__ = .322
 
     @staticmethod
     def screen_resolution():
 
         return shutil.get_terminal_size()
 
-
-
     @staticmethod
     def _get_script():
         l = psutil.Process().cmdline()
-        if len(l)==1:
+        if len(l) == 1:
             return l[0]
         else:
             return l[1]
 
 #
 #
 #
 #
 # / ____/ / / / | / / ____/
 #  / /_  / / / /  |/ / /
 # / __/ / /_/ / /|  / /___
-#/_/    \____/_/ |_/\____/
+# /_/    \____/_/ |_/\____/
 #
     @staticmethod
-    def print_welcome(elapsed=timeUtils.elapsedtime(), version='beta',color_d='blue',color_out='magenta',attributes2=['bold']):
-        site_attribute=['bold','underline']
-        print(colored('+------------------------------------------+',color_out))
-        print(colored('Aniachi Technologies.',color_d,attrs=attributes2))
+    def print_welcome(elapsed=timeUtils.elapsedtime(), version='beta', color_d='blue', color_out='magenta', attributes2=['bold']):
+        site_attribute = ['bold', 'underline']
+        print(colored('+------------------------------------------+', color_out))
+        print(colored('Aniachi Technologies.', color_d, attrs=attributes2))
         s = getpass.getuser()+'@'+platform.node()
 
-
-        print(colored('Computer:            ',color_d,attrs=attributes2),colored(s,color_out))
-        print(colored('Script:              ',color_d,attrs=attributes2),colored(Welcome._get_script(),color_out))
-        print(colored('Api version:         ',color_d,attrs=attributes2),colored(sys.api_version,color_out))
-        print(colored('pip version          ',color_d,attrs=attributes2),colored(pip.__version__,color_out))
-        print(colored('site-packages         ',color_d,attrs=site_attribute))
-        for i,path in enumerate(site.getsitepackages()):
-            print(colored(f'   site-package[ {i} ] ',color_d,attrs=attributes2),colored(path,color_out))
-
-
-        print(colored('Path:                ',color_d,attrs=attributes2),colored(sys.executable,color_out))
-        print(colored('Installed Packages:  ',color_d,attrs=attributes2),colored(len(Welcome.get_installed_distributions()),color_out))
-
-
-        print(colored('Native Compiler:     ',color_d,attrs=attributes2),colored(platform.python_compiler(),color_out))
-        print(colored('Architecture:        ',color_d,attrs=attributes2),colored(platform.processor(),color_out))
-        s = platform.machine()+'  '+platform.system()+' Kernel version '+platform.release()
-        print(colored('Kernel:              ',color_d,attrs=attributes2),colored(s,color_out))
-
-
-        print(colored('CPU Info:            ',color_d,attrs=attributes2),colored(cpuinfo.get_cpu_info()['brand_raw'],color_out))
-        print(colored('Screen resolution:   ',color_d,attrs=attributes2),colored(Welcome.screen_resolution(),color_out))
-
-        print(colored('Python Version:      ',color_d,attrs=attributes2),colored(platform.python_version(),color_out))
-        print(colored('Processors:          ',color_d,attrs=attributes2),colored(psutil.cpu_count(logical=False),color_out))
-        print(colored('Terminal:            ',color_d,attrs=attributes2),colored(Welcome._get_terminal(),color_out))
-        print(colored('User:                ',color_d,attrs=attributes2),colored(getpass.getuser(),color_out))
-        print(colored('Current process:     ',color_d,attrs=attributes2),colored(psutil.Process().pid,color_out))
-        print(colored('Code version:        ',color_d,attrs=attributes2),colored(version,color_out))
+        print(colored('Computer:            ', color_d,
+              attrs=attributes2), colored(s, color_out))
+        print(colored('Script:              ', color_d, attrs=attributes2),
+              colored(Welcome._get_script(), color_out))
+        print(colored('Api version:         ', color_d, attrs=attributes2),
+              colored(sys.api_version, color_out))
+        print(colored('pip version          ', color_d, attrs=attributes2),
+              colored(pip.__version__, color_out))
+        print(colored('site-packages         ', color_d, attrs=site_attribute))
+        for i, path in enumerate(site.getsitepackages()):
+            print(colored(
+                f'   site-package[ {i} ] ', color_d, attrs=attributes2), colored(path, color_out))
+
+        print(colored('Path:                ', color_d,
+              attrs=attributes2), colored(sys.executable, color_out))
+        print(colored('Installed Packages:  ', color_d, attrs=attributes2),
+              colored(len(Welcome.get_installed_distributions()), color_out))
+
+        print(colored('Native Compiler:     ', color_d, attrs=attributes2),
+              colored(platform.python_compiler(), color_out))
+        print(colored('Architecture:        ', color_d, attrs=attributes2),
+              colored(platform.processor(), color_out))
+        s = platform.machine()+'  '+platform.system() + \
+            ' Kernel version '+platform.release()
+        print(colored('Kernel:              ', color_d,
+              attrs=attributes2), colored(s, color_out))
+
+        print(colored('CPU Info:            ', color_d, attrs=attributes2),
+              colored(cpuinfo.get_cpu_info()['brand_raw'], color_out))
+        print(colored('Screen resolution:   ', color_d, attrs=attributes2),
+              colored(Welcome.screen_resolution(), color_out))
+
+        print(colored('Python Version:      ', color_d, attrs=attributes2),
+              colored(platform.python_version(), color_out))
+        print(colored('Processors:          ', color_d, attrs=attributes2),
+              colored(psutil.cpu_count(logical=False), color_out))
+        print(colored('Terminal:            ', color_d, attrs=attributes2),
+              colored(Welcome._get_terminal(), color_out))
+        print(colored('User:                ', color_d, attrs=attributes2),
+              colored(getpass.getuser(), color_out))
+        print(colored('Current process:     ', color_d, attrs=attributes2),
+              colored(psutil.Process().pid, color_out))
+        print(colored('Code version:        ', color_d,
+              attrs=attributes2), colored(version, color_out))
         mem = psutil.virtual_memory()
 
-        print(colored('Total Memory:        ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.total),color_out))
+        print(colored('Total Memory:        ', color_d, attrs=attributes2),
+              colored(stringUtils.sizeof_fmt(mem.total), color_out))
 
-        print(colored('Available Memory:    ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.available),color_out))
-        print(colored('Free Memory:         ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.free),color_out))
-        print(colored('Used Memory:         ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.used),color_out))
-        print(colored('Active Memory:       ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.active),color_out))
-        print(colored('Inactive Memory:     ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.inactive),color_out))
+        print(colored('Available Memory:    ', color_d, attrs=attributes2),
+              colored(stringUtils.sizeof_fmt(mem.available), color_out))
+        print(colored('Free Memory:         ', color_d, attrs=attributes2),
+              colored(stringUtils.sizeof_fmt(mem.free), color_out))
+        print(colored('Used Memory:         ', color_d, attrs=attributes2),
+              colored(stringUtils.sizeof_fmt(mem.used), color_out))
+        print(colored('Active Memory:       ', color_d, attrs=attributes2),
+              colored(stringUtils.sizeof_fmt(mem.active), color_out))
+        print(colored('Inactive Memory:     ', color_d, attrs=attributes2),
+              colored(stringUtils.sizeof_fmt(mem.inactive), color_out))
         try:
-            print(colored('Wired Memory:        ',color_d,attrs=attributes2),colored(stringUtils.sizeof_fmt(mem.wired),color_out))
+            print(colored('Wired Memory:        ', color_d, attrs=attributes2), colored(
+                stringUtils.sizeof_fmt(mem.wired), color_out))
         except Exception as e:
             print(colored('Wired Memory:        ', color_d, attrs=attributes2),
                   colored('Not available', color_out))
 
-        print(colored('Current path:        ',color_d,attrs=attributes2),colored(os.getcwd(),color_out))
+        print(colored('Current path:        ', color_d,
+              attrs=attributes2), colored(os.getcwd(), color_out))
 
-
-        print(colored('Current date:        ',color_d,attrs=attributes2),colored(datetime.datetime.now(),color_out))
-        print(colored('Elapsed time:        ',color_d,attrs=attributes2),colored(elapsed.getElapsedTime(),color_out))
-        print(colored('+------------------------------------------+',color_out))
+        print(colored('Current date:        ', color_d, attrs=attributes2),
+              colored(datetime.datetime.now(), color_out))
+        print(colored('Elapsed time:        ', color_d, attrs=attributes2),
+              colored(elapsed.getElapsedTime(), color_out))
+        print(colored('+------------------------------------------+', color_out))
 
 #
 #
 #
 #
 # / ____/ / / / | / / ____/
 #  / /_  / / / /  |/ / /
 # / __/ / /_/ / /|  / /___
-#/_/    \____/_/ |_/\____/
+# /_/    \____/_/ |_/\____/
 #
 
-
     @staticmethod
     def _get_terminal():
         aux = 'Terminal not found'
         try:
             aux = os.ttyname(sys.stdout.fileno()).split(sep='/')[-1]
         except Exception as e:
             pass
 
         return aux
 
     @staticmethod
     def get_installed_distributions():
-         return list(freeze(skip=["pip", "setuptools", "distribute", "wheel"]))
-
+        return list(freeze(skip=["pip", "setuptools", "distribute", "wheel"]))
 
     @staticmethod
     def get_installed_distributions_as_dict(filter=None):
         if filter is None:
             data = Welcome.get_installed_distributions()
             d = dict()
             for i in data:
@@ -157,152 +174,138 @@
                     key = i.split(sep='==')[0]
                     if key in filter:
                         d[key] = i.split(sep='==')[1]
                 except Exception as e:
                     pass
             return collections.OrderedDict(sorted(d.items()))
 
-
-
     @staticmethod
     def get_all_libs(ft='json'):
         data = Welcome.get_installed_distributions_as_dict()
         if (ft == 'json'):
             return dict(data)
-        elif ft=='list':
-            return [{x:data.get(x,'NONE')} for x in sorted(data)]
+        elif ft == 'list':
+            return [{x: data.get(x, 'NONE')} for x in sorted(data)]
         elif (ft == 'html'):
-            return json2html.convert(json = json.dumps(data))
+            return json2html.convert(json=json.dumps(data))
         elif (ft == 'ascii_table'):
-            return tabulate([[x,data.get(x,'NONE')] for x in sorted(data)], ['module' , 'version'], tablefmt="presto")
-
-
+            return tabulate([[x, data.get(x, 'NONE')] for x in sorted(data)], ['module', 'version'], tablefmt="presto")
 
 
 #
 #
 #
 #
 # / ____/ / / / | / / ____/
 #  / /_  / / / /  |/ / /
 # / __/ / /_/ / /|  / /___
-#/_/    \____/_/ |_/\____/
+# /_/    \____/_/ |_/\____/
 #
+
     @staticmethod
-    def get_fetchdata(elapsed=timeUtils.elapsedtime(),format='dict'):
+    def get_fetchdata(elapsed=timeUtils.elapsedtime(), format='dict'):
         d = dict()
-        d['pip version']=pip.__version__
-        d['site-package']=site.getsitepackages()
-        d['Installed Packages']=len(Welcome.get_installed_distributions())
+        d['pip version'] = pip.__version__
+        d['site-package'] = site.getsitepackages()
+        d['Installed Packages'] = len(Welcome.get_installed_distributions())
 
-        d['Software']='Aniachi Technologies.'
+        d['Software'] = 'Aniachi Technologies.'
         s = getpass.getuser()+'@'+platform.node()
-        d['Computer']=s
-        d['Script']=Welcome._get_script()
-        d['Api version']=sys.api_version
-        d['Path']=sys.executable
-
-        d['Native Compiler']=platform.python_compiler()
-        d['Architecture']=platform.processor()
-        s = platform.machine()+'  '+platform.system()+' Kernel version '+platform.release()
-        d['Kernel']=s
-        d['CPU Info']=cpuinfo.get_cpu_info()['brand_raw']
-        d['Screen resolution']=Welcome.screen_resolution()
-        d['Python Version']=platform.python_version()
-        d['Processors']=psutil.cpu_count(logical=False)
-        d['Terminal']=Welcome._get_terminal()
-        d['User']=getpass.getuser()
-        d['Current process']=psutil.Process().pid
+        d['Computer'] = s
+        d['Script'] = Welcome._get_script()
+        d['Api version'] = sys.api_version
+        d['Path'] = sys.executable
+
+        d['Native Compiler'] = platform.python_compiler()
+        d['Architecture'] = platform.processor()
+        s = platform.machine()+'  '+platform.system() + \
+            ' Kernel version '+platform.release()
+        d['Kernel'] = s
+        d['CPU Info'] = cpuinfo.get_cpu_info().get('brand_raw', 'Not found')
+        d['Screen resolution'] = Welcome.screen_resolution()
+        d['Python Version'] = platform.python_version()
+        d['Processors'] = psutil.cpu_count(logical=False)
+        d['Terminal'] = Welcome._get_terminal()
+        d['User'] = getpass.getuser()
+        d['Current process'] = psutil.Process().pid
         mem = psutil.virtual_memory()
-        d['Code version']=Welcome.__version__
-        d['Total Memory']=stringUtils.sizeof_fmt(mem.total)
-        d['Available Memory']=stringUtils.sizeof_fmt(mem.available)
-        d['Free Memory']=stringUtils.sizeof_fmt(mem.free)
-        d['Used Memory']=stringUtils.sizeof_fmt(mem.used)
-        d['Active Memory']=stringUtils.sizeof_fmt(mem.active)
-        d['Inactive Memory']=stringUtils.sizeof_fmt(mem.inactive)
+        d['Code version'] = Welcome.__version__
+        d['Total Memory'] = stringUtils.sizeof_fmt(mem.total)
+        d['Available Memory'] = stringUtils.sizeof_fmt(mem.available)
+        d['Free Memory'] = stringUtils.sizeof_fmt(mem.free)
+        d['Used Memory'] = stringUtils.sizeof_fmt(mem.used)
+        d['Active Memory'] = stringUtils.sizeof_fmt(mem.active)
+        d['Inactive Memory'] = stringUtils.sizeof_fmt(mem.inactive)
         try:
-            d['Wired Memory']=stringUtils.sizeof_fmt(mem.wired)
+            d['Wired Memory'] = stringUtils.sizeof_fmt(mem.wired)
         except Exception as e:
-             d['Wired Memory']='Not available'
-
-        d['Current path']=os.getcwd()
-        d['Current date']=str(datetime.datetime.now())
-        d['Elapsed time']=elapsed.getElapsedTime()
-
+            d['Wired Memory'] = 'Not available'
 
+        d['Current path'] = os.getcwd()
+        d['Current date'] = str(datetime.datetime.now())
+        d['Elapsed time'] = elapsed.getElapsedTime()
 
         if format == 'json':
             return json.dumps(d)
-        elif format=='dict':
+        elif format == 'dict':
             return d
         else:
             return d
 
-
-
     @staticmethod
     def print_all_libs(color_d='green'):
         installed_packages = Welcome.get_all_libs(ft='ascii_table')
         print(installed_packages)
 
 
 #
 #
 #
 #
 # / ____/ / / / | / / ____/
 #  / /_  / / / /  |/ / /
 # / __/ / /_/ / /|  / /___
-#/_/    \____/_/ |_/\____/
+# /_/    \____/_/ |_/\____/
 #
+
     @staticmethod
-    def print_libs_version(libs,color_d='green'):
+    def print_libs_version(libs, color_d='green'):
         if libs is None:
             raise ValueError('libs is None')
         od = Welcome.get_installed_distributions_as_dict(filter=libs)
-   
 
-        maxLen=max(list(map(len,od)))+1
+        maxLen = max(list(map(len, od)))+1
 
-        if len(od) ==0:
-            print(colored('-'*maxLen,'magenta'))
-            print(colored('Modules not found',color_d))
-            print(colored('-'*maxLen,'magenta'))
+        if len(od) == 0:
+            print(colored('-'*maxLen, 'magenta'))
+            print(colored('Modules not found', color_d))
+            print(colored('-'*maxLen, 'magenta'))
         else:
-            print(colored('-'*(maxLen+8),'magenta'))
+            print(colored('-'*(maxLen+8), 'magenta'))
             for k, s in od.items():
-                print(colored(stringUtils.alingLeft(k,maxLen),color_d),colored(s,'magenta'))
-            print(colored('-'*(maxLen+8),'magenta'))
-            print(colored('Total modules ',color_d),colored(len(od.items()),'magenta'))
-
-
+                print(colored(stringUtils.alingLeft(k, maxLen),
+                      color_d), colored(s, 'magenta'))
+            print(colored('-'*(maxLen+8), 'magenta'))
+            print(colored('Total modules ', color_d),
+                  colored(len(od.items()), 'magenta'))
 
 
 #
 #
 #
 #
 # / ____/ / / / | / / ____/
 #  / /_  / / / /  |/ / /
 # / __/ / /_/ / /|  / /___
-#/_/    \____/_/ |_/\____/
+# /_/    \____/_/ |_/\____/
 #
 
 
-
-
-
 if __name__ == '__main__':
 
     # print('*'*30)
     # Welcome.print_libs_version(libs=['dicttoxml','visualise-spacy-tree','wasabi','numpy'])
     # print('*'*30)
     # Welcome.print_welcome()
     # Welcome.get_installed_distributions_as_dict()
     print('*'*30)
     pprint(Welcome.get_fetchdata())
-
-
-
-
-
```

### Comparing `py_common_fetch-0.352/aniachi/timeUtils.py` & `py_common_fetch-0.354/aniachi/timeUtils.py`

 * *Files identical despite different names*

### Comparing `py_common_fetch-0.352/py_common_fetch.egg-info/PKG-INFO` & `py_common_fetch-0.354/py_common_fetch.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
-Name: py-common-fetch
-Version: 0.352
+Name: py_common_fetch
+Version: 0.354
 Summary: A really simple to use Python fetch screen
 Home-page: https://github.com/bygregonline/py-common-fetch
 Author: Greg flores
 Author-email: bygregonline@yahoo.com
 License: MIT
 Keywords: noefetch common information welcome screen
 Description-Content-Type: text/markdown
+Requires-Dist: pip
+Requires-Dist: psutil>=5.4.5
+Requires-Dist: json2html
+Requires-Dist: py-cpuinfo
+Requires-Dist: termcolor
+Requires-Dist: numpy
+Requires-Dist: tabulate
 
 # How to USE
 
 ```
 
 from aniachi.systemUtils import Welcome as W
 W.printWelcome()
```

### Comparing `py_common_fetch-0.352/setup.py` & `py_common_fetch-0.354/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 setup(
     author='Greg flores',
     author_email='bygregonline@yahoo.com',
     license='MIT',
     zip_safe=False,
     packages=['aniachi'],
     name='py_common_fetch',    # This is the name of your PyPI-package.
-    version='0.352',                          # Update the version number for new releases
-    scripts=['aniachi/timeUtils.py', 'aniachi/stringUtils.py','aniachi/systemUtils.py'],   
+    version='0.354',                          # Update the version number for new releases
+    scripts=['aniachi/timeUtils.py', 'aniachi/stringUtils.py','aniachi/systemUtils.py'],
     keywords='noefetch common information welcome screen',
     install_requires=['pip', 'psutil>=5.4.5','json2html','py-cpuinfo','termcolor','numpy','tabulate'],
     url='https://github.com/bygregonline/py-common-fetch',
     description='A really simple to use Python fetch screen',
     long_description_content_type='text/markdown',
     long_description=long_description  # Optional
```

