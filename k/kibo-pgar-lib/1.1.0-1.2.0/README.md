# Comparing `tmp/kibo_pgar_lib-1.1.0.tar.gz` & `tmp/kibo_pgar_lib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibo_pgar_lib-1.1.0.tar", last modified: Wed May  8 07:34:29 2024, max compression
+gzip compressed data, was "kibo_pgar_lib-1.2.0.tar", last modified: Thu May  9 15:31:56 2024, max compression
```

## Comparing `kibo_pgar_lib-1.1.0.tar` & `kibo_pgar_lib-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:29.136705 kibo_pgar_lib-1.1.0/
--rw-rw-rw-   0        0        0     1093 2024-05-02 08:31:50.000000 kibo_pgar_lib-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3903 2024-05-08 07:34:29.133700 kibo_pgar_lib-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1661 2024-05-03 07:55:51.000000 kibo_pgar_lib-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:29.117623 kibo_pgar_lib-1.1.0/kibo_pgar_lib/
--rw-rw-rw-   0        0        0      346 2024-05-03 07:57:27.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/__init__.py
--rw-rw-rw-   0        0        0     4213 2024-05-02 13:48:32.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/ansi_colors.py
--rw-rw-rw-   0        0        0     2208 2024-05-03 07:57:34.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/file_service.py
--rw-rw-rw-   0        0        0    12321 2024-05-03 07:59:55.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/input_data.py
--rw-rw-rw-   0        0        0     3836 2024-05-02 13:47:29.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/known_problems.py
--rw-rw-rw-   0        0        0     4939 2024-05-03 07:57:57.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/menu.py
--rw-rw-rw-   0        0        0     5924 2024-05-02 13:50:01.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/pretty_strings.py
--rw-rw-rw-   0        0        0     2987 2024-05-02 13:46:20.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib/random_draws.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:29.131703 kibo_pgar_lib-1.1.0/kibo_pgar_lib.egg-info/
--rw-rw-rw-   0        0        0     3903 2024-05-08 07:34:29.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-05-08 07:34:29.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:34:29.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 07:34:29.000000 kibo_pgar_lib-1.1.0/kibo_pgar_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      953 2024-05-08 07:33:10.000000 kibo_pgar_lib-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 07:34:29.136705 kibo_pgar_lib-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      428 2024-05-08 07:32:28.000000 kibo_pgar_lib-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:56.852158 kibo_pgar_lib-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-09 15:31:56.852158 kibo_pgar_lib-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:56.852158 kibo_pgar_lib-1.2.0/kibo_pgar_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/known_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/pretty_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib/random_draws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:56.852158 kibo_pgar_lib-1.2.0/kibo_pgar_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-09 15:31:56.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 15:31:56.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:31:56.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 15:31:56.000000 kibo_pgar_lib-1.2.0/kibo_pgar_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:31:56.852158 kibo_pgar_lib-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-09 15:31:27.000000 kibo_pgar_lib-1.2.0/setup.py
```

### Comparing `kibo_pgar_lib-1.1.0/LICENSE.txt` & `kibo_pgar_lib-1.2.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Alessandro Muscio
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 Alessandro Muscio
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `kibo_pgar_lib-1.1.0/PKG-INFO` & `kibo_pgar_lib-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 2.1
-Name: kibo_pgar_lib
-Version: 1.1.0
-Summary: KiboPgArLib modified, documented and converted in python.
-Home-page: https://github.com/AlessandroMuscio/kibo_pgar_lib
-Author: Alessandro Muscio
-Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
-License: MIT License
-        
-        Copyright (c) 2024 Alessandro Muscio
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: source, https://github.com/AlessandroMuscio/kibo_pgar_lib
-Project-URL: download, https://pypi.org/project/kibo-unibs-fp-lib/#files
-Project-URL: tracker, https://github.com/AlessandroMuscio/kibo_pgar_lib/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Typing :: Typed
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# kibo_pgar_lib
-
-This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
-
-## Installation
-
-This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
-
-```bash
-pip install kibo-unibs-fp-lib
-```
-
-## Usage
-
-For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/wiki) (**WIP!!**).
-
-*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
-
-## Reason for Rename
-
-This library is been renamed from `kibo_unibs_fp_lib` to `kibo_pgar_lib`, basically, just for one main reason. \
-Even thought its Java counterpart `KiboUniBSFpLib` used the already established `UniBSFpLib` as its starting point, hence the name, with the two main goal being:
-
-- Refactoring the code to make it more readable and work with IntelliJ Idea.
-- Adding documentation.
-
-I can already see that this library its evolving into something pretty different from where it started and the changes are just gonna keep coming.
-
-That was the main reason, there is also a second small reason, being that this library is meant to be used for the projects of the course "*Programma Arnaldo*". That does not mean it can only be exclusively used for that (because how the hell can I know what you are using it for?) but I also wanted a way to symbolize the fact that this library was created for that purpose.
+Metadata-Version: 2.1
+Name: kibo_pgar_lib
+Version: 1.2.0
+Summary: KiboUniBSFpLib modified, documented and converted in python.
+Home-page: https://github.com/AlessandroMuscio/kibo_pgar_lib
+Author: Alessandro Muscio
+Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
+License: MIT License
+        
+        Copyright (c) 2024 Alessandro Muscio
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: source, https://github.com/AlessandroMuscio/kibo_pgar_lib
+Project-URL: download, https://pypi.org/project/kibo-unibs-fp-lib/#files
+Project-URL: tracker, https://github.com/AlessandroMuscio/kibo_pgar_lib/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# kibo_pgar_lib
+
+This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
+
+## Installation
+
+This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
+
+```bash
+pip install kibo-pgar-lib
+```
+
+## Usage
+
+For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_pgar_lib/wiki) (**WIP!!**).
+
+*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
+
+## Reason for Rename
+
+This library has been renamed from `kibo_unibs_fp_lib` to `kibo_pgar_lib`, basically, just for one main reason. \
+Even thought its Java counterpart `KiboPgArLib` used the already established `UniBSFpLib` as its starting point, hence the name, with the two main goal being:
+
+- Refactoring the code to make it more readable and work with *IntelliJ Idea*.
+- Adding documentation.
+
+I can already see that this library its evolving into something pretty different from where it started and the changes are just gonna keep coming.
+
+That was the main reason, there is also a second small reason. The main purpose of this library is being used for the projects of the course "*Programma Arnaldo*". That **does not** mean it can only be exclusively used for that (because how the hell can I know what you are using it for?) but I also wanted a way to symbolize the fact that this library was created for that purpose.
```

### Comparing `kibo_pgar_lib-1.1.0/README.md` & `kibo_pgar_lib-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# kibo_pgar_lib
-
-This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
-
-## Installation
-
-This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
-
-```bash
-pip install kibo-unibs-fp-lib
-```
-
-## Usage
-
-For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/wiki) (**WIP!!**).
-
-*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
-
-## Reason for Rename
-
-This library is been renamed from `kibo_unibs_fp_lib` to `kibo_pgar_lib`, basically, just for one main reason. \
-Even thought its Java counterpart `KiboUniBSFpLib` used the already established `UniBSFpLib` as its starting point, hence the name, with the two main goal being:
-
-- Refactoring the code to make it more readable and work with IntelliJ Idea.
-- Adding documentation.
-
-I can already see that this library its evolving into something pretty different from where it started and the changes are just gonna keep coming.
-
-That was the main reason, there is also a second small reason, being that this library is meant to be used for the projects of the course "*Programma Arnaldo*". That does not mean it can only be exclusively used for that (because how the hell can I know what you are using it for?) but I also wanted a way to symbolize the fact that this library was created for that purpose.
+# kibo_pgar_lib
+
+This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
+
+## Installation
+
+This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
+
+```bash
+pip install kibo-pgar-lib
+```
+
+## Usage
+
+For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_pgar_lib/wiki) (**WIP!!**).
+
+*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
+
+## Reason for Rename
+
+This library has been renamed from `kibo_unibs_fp_lib` to `kibo_pgar_lib`, basically, just for one main reason. \
+Even thought its Java counterpart `KiboPgArLib` used the already established `UniBSFpLib` as its starting point, hence the name, with the two main goal being:
+
+- Refactoring the code to make it more readable and work with *IntelliJ Idea*.
+- Adding documentation.
+
+I can already see that this library its evolving into something pretty different from where it started and the changes are just gonna keep coming.
+
+That was the main reason, there is also a second small reason. The main purpose of this library is being used for the projects of the course "*Programma Arnaldo*". That **does not** mean it can only be exclusively used for that (because how the hell can I know what you are using it for?) but I also wanted a way to symbolize the fact that this library was created for that purpose.
```

### Comparing `kibo_pgar_lib-1.1.0/kibo_pgar_lib/input_data.py` & `kibo_pgar_lib-1.2.0/kibo_pgar_lib/input_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-"""Module for the InputData class"""
-
-# Internal Libraries
-from kibo_pgar_lib.ansi_colors import (
-    RESET,
-    AnsiFontColors,
-    AnsiFontDecorations,
-    AnsiFontWeights,
-)
-
-
-class InputData:
-    """
-    This class can read a specific data type inserted in input by the user, while also allowing to
-    make controls on the data inserted and printing errors to the user.
-    """
-
-    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
-    _RED_ERROR: str = f"\n{AnsiFontColors.RED}{AnsiFontWeights.BOLD}Error!{RESET}"
-
-    _ALPHANUMERIC_CHARACTERS_ERROR: str = (
-        f"Only {AnsiFontWeights.BOLD}alphanumeric{RESET} characters are allowed.\n"
-    )
-    _EMPTY_STRING_ERROR: str = (
-        f"No {AnsiFontWeights.BOLD}characters{RESET} or only \
-            {AnsiFontWeights.BOLD}whitespaces{RESET} were inserted.\n"
-    )
-    _ALLOWED_CHARACTERS_ERROR: str = "The only allowed characters are: %s\n"
-    _YES_ANSWERS: str = "yY"
-    _NO_ANSWERS: str = "nN"
-    _INTEGER_FORMAT_ERROR: str = (
-        f"The inserted data is in an {AnsiFontWeights.BOLD}incorrect{RESET} format. An \
-            {AnsiFontDecorations.UNDERLINE}integer{RESET} is required.\n"
-    )
-    _MINIMUM_ERROR: str = "A value greater than or equal to %.2f is required.\n"
-    _MAXIMUM_ERROR: str = "A value less than or equal to %.2f is required.\n"
-    _FLOAT_FORMAT_ERROR: str = (
-        f"The inserted data is in an {AnsiFontWeights.BOLD}incorrect{RESET} format. A \
-            {AnsiFontDecorations.UNDERLINE}float{RESET} is required.\n"
-    )
-
-    def __init__(self) -> None:
-        """Prevents the instantiation of this class.
-
-        Raises
-        ------
-        - NotImplementedError
-        """
-        raise NotImplementedError(InputData._CONSTRUCTOR_ERROR)
-
-    @staticmethod
-    def read_string(message: str, alphanumeric: bool = False) -> str:
-        """Prints message in the terminal and reads the text inserted by the user. It's also
-        possible to select if the inserted text needs to be alphanumeric or not via the
-        alphanumeric variable.
-
-        Params
-        ------
-        - message -> The message to print.
-        - alphanumeric -> If the input needs to be alphanumeric or not, defaulted to False.
-
-        Returns
-        -------
-        A string representing the user input.
-        """
-        if not alphanumeric:
-            return input(message)
-
-        is_alphanumeric: bool = False
-        while not is_alphanumeric:
-            read: str = input(message)
-
-            is_alphanumeric = read.isalnum()
-
-            if not is_alphanumeric:
-                print(InputData._RED_ERROR)
-                print(InputData._ALPHANUMERIC_CHARACTERS_ERROR)
-
-        return read
-
-    @staticmethod
-    def read_non_empty_string(message: str, alphanumeric: bool = False) -> str:
-        """Prints message in the terminal and reads the text inserted by the user, given that it
-        isn't empty. It's also possible to select if the inserted text needs to be alphanumeric or
-        not via the alphanumeric variable.
-
-        Params
-        ------
-        - message -> The message to print.
-        - alphanumeric -> If the input needs to be alphanumeric or not.
-
-        Returns
-        -------
-        A string representing the user input.
-        """
-        is_empty: bool = True
-
-        while is_empty:
-            read: str = InputData.read_string(message, alphanumeric).strip()
-
-            is_empty = not read
-            if is_empty:
-                print(InputData._RED_ERROR)
-                print(InputData._EMPTY_STRING_ERROR)
-
-        return read
-
-    @staticmethod
-    def read_char(message: str, allowed: str = None) -> str:
-        """Read a single character input from the user. It's also possible to give a list, in the
-        form of a string, of the possible allowed characters.
-
-        Params
-        ------
-        - message -> The message to display to the user.
-        - allowed -> Contains the allowed characters, defaulted to None.
-
-        Returns
-        -------
-        The single character input by the user.
-        """
-        if not allowed:
-            return InputData.read_non_empty_string(message, False)[0]
-
-        is_allowed = False
-
-        while not is_allowed:
-            read = InputData.read_non_empty_string(message, False)[0]
-
-            if read in allowed:
-                is_allowed = True
-            else:
-                print(InputData._RED_ERROR)
-                print(InputData._ALLOWED_CHARACTERS_ERROR % list(allowed))
-
-        return read
-
-    @staticmethod
-    def read_yes_or_no(question: str) -> bool:
-        """Prompts the user with a question and expects a yes or no response.
-
-        The idea is to give the question the usual unix terminal aspects, where the question is
-        followed by square brackets and the two possible answers, the upper case one is the default
-        if no answer is given.
-
-        Params
-        ------
-        - question -> The question to display the user without question mark.
-
-        Returns
-        -------
-        True if the user respond with 'y' or 'Y', False otherwise.
-        """
-        question = (
-            f"{question}? [{InputData._YES_ANSWERS[1]}/{InputData._NO_ANSWERS[0]}] "
-        )
-        response = InputData.read_string(question)
-
-        if not response:
-            return True
-
-        return response[0] in InputData._YES_ANSWERS
-
-    @staticmethod
-    def read_integer(message: str) -> int:
-        """Reads an integer input from the user.
-
-        Params
-        ------
-        - message -> The message to display the user.
-
-        Returns
-        -------
-        The integer input by the user.
-        """
-        is_integer: bool = False
-
-        while not is_integer:
-            try:
-                read: int = int(input(message))
-                is_integer = True
-            except ValueError:
-                print(InputData._RED_ERROR)
-                print(InputData._INTEGER_FORMAT_ERROR)
-
-        return read
-
-    @staticmethod
-    def read_integer_with_minimum(message: str, min_value: int) -> int:
-        """Reads an integer input from the user with a minimum value constraint.
-
-        Params
-        ------
-        - message -> The message to display the user.
-        - min_value -> The minimum allowed value for the input.
-
-        Returns
-        -------
-        The integer input by the user that is greater than or equal to min_value.
-        """
-        is_input_out_of_range: bool = True
-
-        while is_input_out_of_range:
-            read: int = InputData.read_integer(message)
-
-            if read >= min_value:
-                is_input_out_of_range = False
-            else:
-                print(InputData._RED_ERROR)
-                print(InputData._MINIMUM_ERROR % min_value)
-
-        return read
-
-    @staticmethod
-    def read_integer_with_maximum(message: str, max_value: int) -> int:
-        """Reads an integer input from the user with a maximum value constraint.
-
-        Params
-        ------
-        - message -> The message to display the user.
-        - max_value -> The maximum allowed value for the input.
-
-        Returns
-        -------
-        The integer input by the user that is less than or equal to max_value.
-        """
-        is_input_out_of_range: bool = True
-
-        while is_input_out_of_range:
-            read: int = InputData.read_integer(message)
-
-            if read <= max_value:
-                is_input_out_of_range = False
-            else:
-                print(InputData._RED_ERROR)
-                print(InputData._MAXIMUM_ERROR % max_value)
-
-        return read
-
-    @staticmethod
-    def read_integer_between(message: str, min_value: int, max_value: int) -> int:
-        """Reads an integer input from the user with a minimum and maximum value constraint.
-
-        Params
-        ------
-        - message -> The message to display the user.
-        - min_value -> The minimum allowed value for the input.
-        - max_value -> The maximum allowed value for the input.
-
-        Returns
-        -------
-        The integer input by the user that is greater than or equal to min_value and less than or
-        equal to max_value.
-        """
-        is_input_out_of_range: bool = True
-
-        while is_input_out_of_range:
-            read: int = InputData.read_integer(message)
-
-            if read < min_value:
-                print(InputData._RED_ERROR)
-                print(InputData._MINIMUM_ERROR % min_value)
-            elif read > max_value:
-                print(InputData._RED_ERROR)
-                print(InputData._MAXIMUM_ERROR % max_value)
-            else:
-                is_input_out_of_range = False
-
-        return read
-
-    @staticmethod
-    def read_float(message: str) -> float:
-        """Reads a float input from the user.
-
-        Params
-        ------
-        - message -> The message to display the user.
-
-        Returns
-        -------
-        The float input by the user.
-        """
-        is_float: bool = False
-
-        while not is_float:
-            try:
-                read = float(input(message))
-                is_float = True
-            except ValueError:
-                print(InputData._RED_ERROR)
-                print(InputData._FLOAT_FORMAT_ERROR)
-
-        return read
-
-    @staticmethod
-    def read_float_with_minimum(message: str, min_value: float) -> float:
-        """Reads a float input from the user with a minimum value constraint.
-
-        Params
-        ------
-        - message -> The message to display the user.
-        - min_value -> The minimum allowed value for the input.
-
-        Returns
-        -------
-        The float input by the user that is greater than or equal to min_value.
-        """
-        is_input_out_of_range: bool = True
-
-        while is_input_out_of_range:
-            read: float = InputData.read_float(message)
-
-            if read >= min_value:
-                is_input_out_of_range = False
-            else:
-                print(InputData._RED_ERROR)
-                print(InputData._MINIMUM_ERROR % min_value)
-
-        return read
-
-    @staticmethod
-    def read_float_with_maximum(message: str, max_value: float) -> float:
-        """Reads a float input from the user with a maximum value constraint.
-
-        Params
-        ------
-        - message -> The message to display the user.
-        - max_value -> The maximum allowed value for the input.
-
-        Returns
-        -------
-        The float input by the user that is less than or equal to max_value.
-        """
-        is_input_out_of_range: bool = True
-
-        while is_input_out_of_range:
-            read: float = InputData.read_float(message)
-
-            if read <= max_value:
-                is_input_out_of_range = False
-            else:
-                print(InputData._RED_ERROR)
-                print(InputData._MAXIMUM_ERROR % max_value)
-
-        return read
-
-    @staticmethod
-    def read_float_between(message: str, min_value: float, max_value: float) -> float:
-        """Reads a float input from the user with a minimum and maximum value constraint.
-
-        Params
-        ------
-        - message -> The message to display the user.
-        - min_value -> The minimum allowed value for the input.
-        - max_value -> The maximum allowed value for the input.
-
-        Returns
-        -------
-        The float input by the user that is greater than or equal to min_value and less than or
-        equal to max_value.
-        """
-        is_input_out_of_range: bool = True
-
-        while is_input_out_of_range:
-            read: float = InputData.read_float(message)
-
-            if read < min_value:
-                print(InputData._RED_ERROR)
-                print(InputData._MINIMUM_ERROR % min_value)
-            elif read > max_value:
-                print(InputData._RED_ERROR)
-                print(InputData._MAXIMUM_ERROR % max_value)
-            else:
-                is_input_out_of_range = False
-
-        return read
+"""Module for the InputData class"""
+
+# Internal Libraries
+from kibo_pgar_lib.ansi_colors import (
+    RESET,
+    AnsiFontColors,
+    AnsiFontDecorations,
+    AnsiFontWeights,
+)
+
+
+class InputData:
+    """
+    This class can read a specific data type inserted in input by the user, while also allowing to
+    make controls on the data inserted and printing errors to the user.
+    """
+
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
+    _RED_ERROR: str = f"\n{AnsiFontColors.RED}{AnsiFontWeights.BOLD}Error!{RESET}"
+
+    _ALPHANUMERIC_CHARACTERS_ERROR: str = (
+        f"Only {AnsiFontWeights.BOLD}alphanumeric{RESET} characters are allowed.\n"
+    )
+    _EMPTY_STRING_ERROR: str = (
+        f"No {AnsiFontWeights.BOLD}characters{RESET} or only {AnsiFontWeights.BOLD}whitespaces"
+        f"{RESET} were inserted.\n"
+    )
+    _ALLOWED_CHARACTERS_ERROR: str = "The only allowed characters are: %s\n"
+    _YES_ANSWERS: str = "yY"
+    _NO_ANSWERS: str = "nN"
+    _INTEGER_FORMAT_ERROR: str = (
+        f"The inserted data is in an {AnsiFontWeights.BOLD}incorrect{RESET} format. An "
+        f"{AnsiFontDecorations.UNDERLINE}integer{RESET} is required.\n"
+    )
+    _MINIMUM_ERROR: str = "A value greater than or equal to %.2f is required.\n"
+    _MAXIMUM_ERROR: str = "A value less than or equal to %.2f is required.\n"
+    _FLOAT_FORMAT_ERROR: str = (
+        f"The inserted data is in an {AnsiFontWeights.BOLD}incorrect{RESET} format. A "
+        f"{AnsiFontDecorations.UNDERLINE}float{RESET} is required.\n"
+    )
+
+    def __init__(self) -> None:
+        """Prevents the instantiation of this class.
+
+        Raises
+        ------
+        - NotImplementedError
+        """
+        raise NotImplementedError(InputData._CONSTRUCTOR_ERROR)
+
+    @staticmethod
+    def read_string(message: str, alphanumeric: bool = False) -> str:
+        """Prints message in the terminal and reads the text inserted by the user. It's also
+        possible to select if the inserted text needs to be alphanumeric or not via the
+        alphanumeric variable.
+
+        Params
+        ------
+        - message -> The message to print.
+        - alphanumeric -> If the input needs to be alphanumeric or not, defaulted to False.
+
+        Returns
+        -------
+        A string representing the user input.
+        """
+        if not alphanumeric:
+            return input(message)
+
+        is_alphanumeric: bool = False
+        while not is_alphanumeric:
+            read: str = input(message)
+
+            is_alphanumeric = read.isalnum() if read else True
+
+            if not is_alphanumeric:
+                print(InputData._RED_ERROR)
+                print(InputData._ALPHANUMERIC_CHARACTERS_ERROR)
+
+        return read
+
+    @staticmethod
+    def read_non_empty_string(message: str, alphanumeric: bool = False) -> str:
+        """Prints message in the terminal and reads the text inserted by the user, given that it
+        isn't empty. It's also possible to select if the inserted text needs to be alphanumeric or
+        not via the alphanumeric variable.
+
+        Params
+        ------
+        - message -> The message to print.
+        - alphanumeric -> If the input needs to be alphanumeric or not.
+
+        Returns
+        -------
+        A string representing the user input.
+        """
+        is_empty: bool = True
+
+        while is_empty:
+            read: str = InputData.read_string(message, alphanumeric).strip()
+
+            is_empty = not read
+            if is_empty:
+                print(InputData._RED_ERROR)
+                print(InputData._EMPTY_STRING_ERROR)
+
+        return read
+
+    @staticmethod
+    def read_char(message: str, allowed: str = None) -> str:
+        """Read a single character input from the user. It's also possible to give a list, in the
+        form of a string, of the possible allowed characters.
+
+        Params
+        ------
+        - message -> The message to display to the user.
+        - allowed -> Contains the allowed characters, defaulted to None.
+
+        Returns
+        -------
+        The single character input by the user.
+        """
+        if not allowed:
+            return InputData.read_non_empty_string(message, False)[0]
+
+        is_allowed = False
+
+        while not is_allowed:
+            read = InputData.read_non_empty_string(message, False)[0]
+
+            if read in allowed:
+                is_allowed = True
+            else:
+                print(InputData._RED_ERROR)
+                print(InputData._ALLOWED_CHARACTERS_ERROR % list(allowed))
+
+        return read
+
+    @staticmethod
+    def read_yes_or_no(question: str) -> bool:
+        """Prompts the user with a question and expects a yes or no response.
+
+        The idea is to give the question the usual unix terminal aspects, where the question is
+        followed by square brackets and the two possible answers, the upper case one is the default
+        if no answer is given.
+
+        Params
+        ------
+        - question -> The question to display the user without question mark.
+
+        Returns
+        -------
+        True if the user respond with 'y' or 'Y', False otherwise.
+        """
+        question = (
+            f"{question}? [{InputData._YES_ANSWERS[1]}/{InputData._NO_ANSWERS[0]}] "
+        )
+        response = InputData.read_string(question)
+
+        if not response:
+            return True
+
+        return response[0] in InputData._YES_ANSWERS
+
+    @staticmethod
+    def read_integer(message: str) -> int:
+        """Reads an integer input from the user.
+
+        Params
+        ------
+        - message -> The message to display the user.
+
+        Returns
+        -------
+        The integer input by the user.
+        """
+        is_integer: bool = False
+
+        while not is_integer:
+            try:
+                read: int = int(input(message))
+                is_integer = True
+            except ValueError:
+                print(InputData._RED_ERROR)
+                print(InputData._INTEGER_FORMAT_ERROR)
+
+        return read
+
+    @staticmethod
+    def read_integer_with_minimum(message: str, min_value: int) -> int:
+        """Reads an integer input from the user with a minimum value constraint.
+
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+
+        Returns
+        -------
+        The integer input by the user that is greater than or equal to min_value.
+        """
+        is_input_out_of_range: bool = True
+
+        while is_input_out_of_range:
+            read: int = InputData.read_integer(message)
+
+            if read >= min_value:
+                is_input_out_of_range = False
+            else:
+                print(InputData._RED_ERROR)
+                print(InputData._MINIMUM_ERROR % min_value)
+
+        return read
+
+    @staticmethod
+    def read_integer_with_maximum(message: str, max_value: int) -> int:
+        """Reads an integer input from the user with a maximum value constraint.
+
+        Params
+        ------
+        - message -> The message to display the user.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The integer input by the user that is less than or equal to max_value.
+        """
+        is_input_out_of_range: bool = True
+
+        while is_input_out_of_range:
+            read: int = InputData.read_integer(message)
+
+            if read <= max_value:
+                is_input_out_of_range = False
+            else:
+                print(InputData._RED_ERROR)
+                print(InputData._MAXIMUM_ERROR % max_value)
+
+        return read
+
+    @staticmethod
+    def read_integer_between(message: str, min_value: int, max_value: int) -> int:
+        """Reads an integer input from the user with a minimum and maximum value constraint.
+
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The integer input by the user that is greater than or equal to min_value and less than or
+        equal to max_value.
+        """
+        is_input_out_of_range: bool = True
+
+        while is_input_out_of_range:
+            read: int = InputData.read_integer(message)
+
+            if read < min_value:
+                print(InputData._RED_ERROR)
+                print(InputData._MINIMUM_ERROR % min_value)
+            elif read > max_value:
+                print(InputData._RED_ERROR)
+                print(InputData._MAXIMUM_ERROR % max_value)
+            else:
+                is_input_out_of_range = False
+
+        return read
+
+    @staticmethod
+    def read_float(message: str) -> float:
+        """Reads a float input from the user.
+
+        Params
+        ------
+        - message -> The message to display the user.
+
+        Returns
+        -------
+        The float input by the user.
+        """
+        is_float: bool = False
+
+        while not is_float:
+            try:
+                read = float(input(message))
+                is_float = True
+            except ValueError:
+                print(InputData._RED_ERROR)
+                print(InputData._FLOAT_FORMAT_ERROR)
+
+        return read
+
+    @staticmethod
+    def read_float_with_minimum(message: str, min_value: float) -> float:
+        """Reads a float input from the user with a minimum value constraint.
+
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+
+        Returns
+        -------
+        The float input by the user that is greater than or equal to min_value.
+        """
+        is_input_out_of_range: bool = True
+
+        while is_input_out_of_range:
+            read: float = InputData.read_float(message)
+
+            if read >= min_value:
+                is_input_out_of_range = False
+            else:
+                print(InputData._RED_ERROR)
+                print(InputData._MINIMUM_ERROR % min_value)
+
+        return read
+
+    @staticmethod
+    def read_float_with_maximum(message: str, max_value: float) -> float:
+        """Reads a float input from the user with a maximum value constraint.
+
+        Params
+        ------
+        - message -> The message to display the user.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The float input by the user that is less than or equal to max_value.
+        """
+        is_input_out_of_range: bool = True
+
+        while is_input_out_of_range:
+            read: float = InputData.read_float(message)
+
+            if read <= max_value:
+                is_input_out_of_range = False
+            else:
+                print(InputData._RED_ERROR)
+                print(InputData._MAXIMUM_ERROR % max_value)
+
+        return read
+
+    @staticmethod
+    def read_float_between(message: str, min_value: float, max_value: float) -> float:
+        """Reads a float input from the user with a minimum and maximum value constraint.
+
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The float input by the user that is greater than or equal to min_value and less than or
+        equal to max_value.
+        """
+        is_input_out_of_range: bool = True
+
+        while is_input_out_of_range:
+            read: float = InputData.read_float(message)
+
+            if read < min_value:
+                print(InputData._RED_ERROR)
+                print(InputData._MINIMUM_ERROR % min_value)
+            elif read > max_value:
+                print(InputData._RED_ERROR)
+                print(InputData._MAXIMUM_ERROR % max_value)
+            else:
+                is_input_out_of_range = False
+
+        return read
```

### Comparing `kibo_pgar_lib-1.1.0/kibo_pgar_lib/known_problems.py` & `kibo_pgar_lib-1.2.0/kibo_pgar_lib/known_problems.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""Module for the KnownProblems class"""
-
-
-class KnownProblems:
-    """
-    This class has the implementation of some of the usual problems that you always forget and need
-    to go watch the solution on StackOverflow even though you know you've already solved them.
-    """
-
-    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
-    _VALUES_ERROR: str = "Too few arguments were passed!"
-
-    def __init__(self) -> None:
-        """Prevents the instantiation of this class.
-
-        Raises
-        ------
-        - NotImplementedError
-        """
-        raise NotImplementedError(KnownProblems._CONSTRUCTOR_ERROR)
-
-    @staticmethod
-    def _mcd(a: int, b: int) -> int:
-        """Finds the MCD (Maximum Common Divider) between two integers.
-
-        Params
-        ------
-        - a -> The first number to calculate the MCD.
-        - b -> The second number to calculate the MCD.
-
-        Returns
-        -------
-        An integer representing the MCD.
-        """
-        while a != 0 and b != 0:
-            if a > b:
-                a %= b
-            else:
-                b %= a
-
-        return b if a == 0 else a
-
-    @staticmethod
-    def mcd(values: list[int]) -> int:
-        """Finds the MCD (Maximum Common Divider) between a list of integers.
-
-        Params
-        ------
-        - values -> The values used to find the MCD.
-
-        Returns
-        -------
-        An integer representing the MCD between all the values.
-
-        Raises
-        ------
-        - ValueError -> If less than two values are given.
-        """
-        if not values or len(values) < 2:
-            raise ValueError(KnownProblems._VALUES_ERROR)
-
-        mcd: int = values[0]
-
-        for value in values[1:]:
-            mcd = KnownProblems._mcd(mcd, value)
-
-        return mcd
-
-    @staticmethod
-    def _mcm(a: int, b: int) -> int:
-        """Finds the MCM (Minimum Common Multiplier) between two numbers.
-
-        Params
-        ------
-        - a -> The first number to calculate the MCM.
-        - b -> The second number to calculate the MCM.
-
-        Returns
-        -------
-        An integer representing the MCM.
-        """
-        mcd: int = KnownProblems._mcd(a, b)
-
-        return (a * b) // mcd
-
-    @staticmethod
-    def mcm(values: list[int]) -> int:
-        """Finds the MCM (Minimum Common Multiplier) between a list of integers.
-
-        Params
-        ------
-        - values -> The values used to find the MCM.
-
-        Returns
-        -------
-        An integer representing the MCM between all the values.
-
-        Raises
-        ------
-        - ValueError -> If less than two values are given.
-        """
-        if not values or len(values) < 2:
-            raise ValueError(KnownProblems._VALUES_ERROR)
-
-        mcm: int = values[0]
-
-        for value in values[1:]:
-            mcm = KnownProblems._mcm(mcm, value)
-
-        return mcm
-
-    @staticmethod
-    def count_integer_digits(n: int) -> int:
-        """Counts the number of digits of an integer.
-
-        Params
-        ------
-        - n -> The number to calculate the digits.
-
-        Returns
-        -------
-        An integer representing the number of digits of n.
-        """
-        return len(str(abs(n)))
-
-    @staticmethod
-    def count_decimal_digits(n: float) -> int:
-        """Counts the number of decimal digits in a float.
-
-        Params
-        ------
-        - n -> The number to calculate the decimal digits.
-
-        Returns
-        -------
-        An integer representing the number of decimal digits of n.
-        """
-        splitted_number: list[str] = str(abs(n)).split(".")
-
-        if len(splitted_number) < 2:
-            return 0
-
-        return len(splitted_number[1])
+"""Module for the KnownProblems class"""
+
+
+class KnownProblems:
+    """
+    This class has the implementation of some of the usual problems that you always forget and need
+    to go watch the solution on StackOverflow even though you know you've already solved them.
+    """
+
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
+    _VALUES_ERROR: str = "Too few arguments were passed!"
+
+    def __init__(self) -> None:
+        """Prevents the instantiation of this class.
+
+        Raises
+        ------
+        - NotImplementedError
+        """
+        raise NotImplementedError(KnownProblems._CONSTRUCTOR_ERROR)
+
+    @staticmethod
+    def _mcd(a: int, b: int) -> int:
+        """Finds the MCD (Maximum Common Divider) between two integers.
+
+        Params
+        ------
+        - a -> The first number to calculate the MCD.
+        - b -> The second number to calculate the MCD.
+
+        Returns
+        -------
+        An integer representing the MCD.
+        """
+        while a != 0 and b != 0:
+            if a > b:
+                a %= b
+            else:
+                b %= a
+
+        return b if a == 0 else a
+
+    @staticmethod
+    def mcd(values: list[int]) -> int:
+        """Finds the MCD (Maximum Common Divider) between a list of integers.
+
+        Params
+        ------
+        - values -> The values used to find the MCD.
+
+        Returns
+        -------
+        An integer representing the MCD between all the values.
+
+        Raises
+        ------
+        - ValueError -> If less than two values are given.
+        """
+        if not values or len(values) < 2:
+            raise ValueError(KnownProblems._VALUES_ERROR)
+
+        mcd: int = values[0]
+
+        for value in values[1:]:
+            mcd = KnownProblems._mcd(mcd, value)
+
+        return mcd
+
+    @staticmethod
+    def _mcm(a: int, b: int) -> int:
+        """Finds the MCM (Minimum Common Multiplier) between two numbers.
+
+        Params
+        ------
+        - a -> The first number to calculate the MCM.
+        - b -> The second number to calculate the MCM.
+
+        Returns
+        -------
+        An integer representing the MCM.
+        """
+        mcd: int = KnownProblems._mcd(a, b)
+
+        return (a * b) // mcd
+
+    @staticmethod
+    def mcm(values: list[int]) -> int:
+        """Finds the MCM (Minimum Common Multiplier) between a list of integers.
+
+        Params
+        ------
+        - values -> The values used to find the MCM.
+
+        Returns
+        -------
+        An integer representing the MCM between all the values.
+
+        Raises
+        ------
+        - ValueError -> If less than two values are given.
+        """
+        if not values or len(values) < 2:
+            raise ValueError(KnownProblems._VALUES_ERROR)
+
+        mcm: int = values[0]
+
+        for value in values[1:]:
+            mcm = KnownProblems._mcm(mcm, value)
+
+        return mcm
+
+    @staticmethod
+    def count_integer_digits(n: int) -> int:
+        """Counts the number of digits of an integer.
+
+        Params
+        ------
+        - n -> The number to calculate the digits.
+
+        Returns
+        -------
+        An integer representing the number of digits of n.
+        """
+        return len(str(abs(n)))
+
+    @staticmethod
+    def count_decimal_digits(n: float) -> int:
+        """Counts the number of decimal digits in a float.
+
+        Params
+        ------
+        - n -> The number to calculate the decimal digits.
+
+        Returns
+        -------
+        An integer representing the number of decimal digits of n.
+        """
+        splitted_number: list[str] = str(abs(n)).split(".")
+
+        if len(splitted_number) < 2:
+            return 0
+
+        return len(splitted_number[1])
```

### Comparing `kibo_pgar_lib-1.1.0/kibo_pgar_lib/pretty_strings.py` & `kibo_pgar_lib-1.2.0/kibo_pgar_lib/pretty_strings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,187 +1,175 @@
-"""Module for the PrettyStrings class"""
-
-
-class PrettyStrings:
-    """This class contains various methods to prettify print strings to the terminal."""
-
-    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
-    _SPACE = " "
-    _HORIZONTAL_FRAME = "-"
-    _VERTICAL_FRAME = "|"
-    _NEW_LINE = "\n"
-
-    def __init__(self) -> None:
-        """Prevents the instantiation of this class.
-
-        Raises
-        ------
-        - NotImplementedError
-        """
-        raise NotImplementedError(PrettyStrings._CONSTRUCTOR_ERROR)
-
-    @staticmethod
-    def frame(
-        to_frame: str, frame_length: int, centered: bool, vertical_frame: bool
-    ) -> str:
-        """Puts the given string in the center or in the beginning of the line surrounded by the
-        horizontal frame above and below and, if needed, also the vertical frame before and after.
-        It's required to specify a frame length for the horizontal frame.
-
-        Params
-        ------
-        - to_frame -> The string to put in the frame
-        - frame_length -> The length of the horizontal frame.
-        - centered -> If the string needs to be centered or not.
-        - vertical_frame -> If the vertical frame is needed or not.
-
-        Returns
-        -------
-        A string containing the framed original string.
-        """
-        framed: list[str] = []
-        horizontal_frame: list[str] = "".join(
-            [
-                PrettyStrings.repeat_char(
-                    PrettyStrings._HORIZONTAL_FRAME, frame_length
-                ),
-                PrettyStrings._NEW_LINE,
-            ]
-        )
-
-        framed.append(horizontal_frame)
-
-        if vertical_frame:
-            framed.append(PrettyStrings._VERTICAL_FRAME)
-
-        to_append: str
-        if centered:
-            to_append = (
-                PrettyStrings.center(to_frame, frame_length - 2)
-                if vertical_frame
-                else "".join(
-                    [
-                        PrettyStrings.center(to_frame, frame_length),
-                        PrettyStrings._NEW_LINE,
-                    ]
-                )
-            )
-        else:
-            to_append = (
-                PrettyStrings.column(to_frame, frame_length - 2)
-                if vertical_frame
-                else "".join(
-                    [
-                        PrettyStrings.column(to_frame, frame_length),
-                        PrettyStrings._NEW_LINE,
-                    ]
-                )
-            )
-        framed.append(to_append)
-
-        if vertical_frame:
-            framed.append(
-                "".join([PrettyStrings._VERTICAL_FRAME, PrettyStrings._NEW_LINE])
-            )
-
-        framed.append(horizontal_frame)
-
-        return "".join(framed)
-
-    @staticmethod
-    def column(to_columnize: str, width: int) -> str:
-        """Puts teh given string at the beginning of the line and adds spaces until the end of it.
-        If the string is too long for the width of the line, it will be cut off.
-
-        Params
-        ------
-        - to_columnize -> The string to put in column.
-        - width -> The length of the line.
-
-        Returns
-        -------
-        A string containing the columned string.
-        """
-        columned: list[str] = []
-        to_columnize_length: int = len(to_columnize)
-        chars_to_print: int = min(width, to_columnize_length)
-
-        columned.append(
-            to_columnize[:chars_to_print]
-            if to_columnize_length > chars_to_print
-            else to_columnize
-        )
-
-        columned.append(
-            PrettyStrings.repeat_char(
-                PrettyStrings._SPACE, max(0, width - to_columnize_length)
-            )
-        )
-
-        return "".join(columned)
-
-    @staticmethod
-    def center(to_center: str, width: int) -> str:
-        """Puts the given string in the center of the line of the given width. If the string is too
-        long it will be cut off.
-
-        Params
-        ------
-        - to_center -> The string to center.
-        - width -> The length of the line where to center the string.
-
-        Returns
-        -------
-        A string containing the centered string.
-        """
-        to_center_length: int = len(to_center)
-
-        if to_center_length > width:
-            return to_center[:width]
-
-        if to_center_length == width:
-            return to_center
-
-        centered: list[str] = []
-        whitespaces: int = width - to_center_length
-        whitespaces_before: int = whitespaces // 2
-        whitespaces_after: int = whitespaces - whitespaces_before
-
-        centered.append(
-            PrettyStrings.repeat_char(PrettyStrings._SPACE, whitespaces_before)
-        )
-        centered.append(to_center)
-        centered.append(
-            PrettyStrings.repeat_char(PrettyStrings._SPACE, whitespaces_after)
-        )
-
-        return "".join(centered)
-
-    @staticmethod
-    def repeat_char(char: str, times: int) -> str:
-        """Repeats a given character a given number of times.
-
-        Params
-        ------
-        - char -> The character to repeat.
-        - times -> The number of times to repeat the character.
-
-        Returns
-        -------
-        A string containing the character repeated. If times is less than or equal to 0 an empty
-        string will be returned.
-        """
-        return char * max(0, times)
-
-    @staticmethod
-    def isolated_line(to_isolate: str) -> str:
-        """Isolates a given string by adding an empty line before and after it.
-
-        Params
-        ------
-        - to_isolate -> The string to isolate.
-
-        Returns
-        -------
-        A string containing the isolated string.
-        """
-        return f"{PrettyStrings._NEW_LINE}{to_isolate}{PrettyStrings._NEW_LINE}"
+"""Module for the PrettyStrings class"""
+
+
+class PrettyStrings:
+    """This class contains various methods to prettify print strings to the terminal."""
+
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
+    _SPACE = " "
+    _HORIZONTAL_FRAME = "-"
+    _VERTICAL_FRAME = "|"
+    _NEW_LINE = "\n"
+
+    def __init__(self) -> None:
+        """Prevents the instantiation of this class.
+
+        Raises
+        ------
+        - NotImplementedError
+        """
+        raise NotImplementedError(PrettyStrings._CONSTRUCTOR_ERROR)
+
+    @staticmethod
+    def frame(
+        to_frame: str, frame_length: int, centered: bool, vertical_frame: bool
+    ) -> str:
+        """Puts the given string in the center or in the beginning of the line surrounded by the
+        horizontal frame above and below and, if needed, also the vertical frame before and after.
+        It's required to specify a frame length for the horizontal frame.
+
+        Params
+        ------
+        - to_frame -> The string to put in the frame
+        - frame_length -> The length of the horizontal frame.
+        - centered -> If the string needs to be centered or not.
+        - vertical_frame -> If the vertical frame is needed or not.
+
+        Returns
+        -------
+        A string containing the framed original string.
+        """
+        framed: list[str] = []
+        horizontal_frame: list[str] = [
+            PrettyStrings.repeat_char(PrettyStrings._HORIZONTAL_FRAME, frame_length),
+            PrettyStrings._NEW_LINE,
+        ]
+
+        framed.extend(horizontal_frame)
+
+        if vertical_frame:
+            to_append: str = PrettyStrings._VERTICAL_FRAME
+            to_append += (
+                PrettyStrings.center(to_frame, frame_length - 2)
+                if centered
+                else PrettyStrings.column(to_frame, frame_length - 2)
+            )
+            to_append += PrettyStrings._VERTICAL_FRAME + PrettyStrings._NEW_LINE
+        else:
+            to_append: str = (
+                PrettyStrings.center(to_frame, frame_length)
+                if centered
+                else PrettyStrings.column(to_frame, frame_length)
+            )
+            to_append += PrettyStrings._NEW_LINE
+
+        framed.append(to_append)
+
+        framed.extend(horizontal_frame)
+
+        return "".join(framed)
+
+    @staticmethod
+    def column(to_columnize: str, width: int) -> str:
+        """Puts teh given string at the beginning of the line and adds spaces until the end of it.
+        If the string is too long for the width of the line, it will be cut off.
+
+        Params
+        ------
+        - to_columnize -> The string to put in column.
+        - width -> The length of the line.
+
+        Returns
+        -------
+        A string containing the columned string.
+        """
+        columned: list[str] = []
+        to_columnize_length: int = len(to_columnize)
+        chars_to_print: int = min(width, to_columnize_length)
+
+        columned.append(
+            to_columnize[:chars_to_print]
+            if to_columnize_length > chars_to_print
+            else to_columnize
+        )
+
+        columned.append(
+            PrettyStrings.repeat_char(PrettyStrings._SPACE, width - to_columnize_length)
+        )
+
+        return "".join(columned)
+
+    @staticmethod
+    def center(to_center: str, width: int) -> str:
+        """Puts the given string in the center of the line of the given width. If the string is too
+        long it will be cut off.
+
+        Params
+        ------
+        - to_center -> The string to center.
+        - width -> The length of the line where to center the string.
+
+        Returns
+        -------
+        A string containing the centered string.
+        """
+        to_center_length: int = len(to_center)
+
+        if to_center_length > width:
+            return to_center[:width]
+
+        if to_center_length == width:
+            return to_center
+
+        centered: list[str] = []
+        whitespaces: int = width - to_center_length
+        whitespaces_before: int = whitespaces // 2
+        whitespaces_after: int = whitespaces - whitespaces_before
+
+        centered.append(
+            PrettyStrings.repeat_char(PrettyStrings._SPACE, whitespaces_before)
+        )
+        centered.append(to_center)
+        centered.append(
+            PrettyStrings.repeat_char(PrettyStrings._SPACE, whitespaces_after)
+        )
+
+        return "".join(centered)
+
+    @staticmethod
+    def repeat_char(char: str, times: int) -> str:
+        """Repeats a given character a given number of times.
+
+        Params
+        ------
+        - char -> The character to repeat.
+        - times -> The number of times to repeat the character.
+
+        Returns
+        -------
+        A string containing the character repeated. If times is less than or equal to 0 an empty
+        string will be returned.
+        """
+        return char * max(0, times)
+
+    @staticmethod
+    def isolated_line(to_isolate: str) -> str:
+        """Isolates a given string by adding an empty line before and after it.
+
+        Params
+        ------
+        - to_isolate -> The string to isolate.
+
+        Returns
+        -------
+        A string containing the isolated string.
+        """
+        return f"{PrettyStrings._NEW_LINE}{to_isolate}{PrettyStrings._NEW_LINE}"
+
+
+def main() -> None:
+    print(PrettyStrings.frame("Cock", 14, True, True))
+    print("Omega")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `kibo_pgar_lib-1.1.0/kibo_pgar_lib/random_draws.py` & `kibo_pgar_lib-1.2.0/kibo_pgar_lib/random_draws.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-"""Module for the RandomDraws class"""
-
-# Standard Libraries
-import random
-
-
-class RandomDraws:
-    """This class provides methods for drawing a specific data type in a pseudo-random way."""
-
-    _RAND = random.Random()
-    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
-
-    def __init__(self) -> None:
-        """Prevents the instantiation of this class.
-
-        Raises
-        ------
-        - NotImplementedError
-        """
-        raise NotImplementedError(RandomDraws._CONSTRUCTOR_ERROR)
-
-    @staticmethod
-    def draw_integer(minimum: int, maximum: int) -> int:
-        """Draws a random integer between given minimum and maximum values included.
-
-        Params
-        ------
-        - minimum -> The minimum value to draw.
-        - maximum -> The maximum value to draw
-
-        Returns
-        -------
-        An integer representing the drawn number.
-        """
-        return RandomDraws._RAND.randint(minimum, maximum)
-
-    @staticmethod
-    def draw_float(minimum: float, maximum: float) -> float:
-        """Draws a random float between given minimum and maximum values included.
-
-        Params
-        ------
-        - minimum -> The minimum value to draw.
-        - maximum -> The maximum value to draw
-
-        Returns
-        -------
-        An float representing the drawn number.
-        """
-        return RandomDraws._RAND.uniform(minimum, maximum)
-
-    @staticmethod
-    def draw_integer_with_distribution(
-        minimum: int, maximum: int, exponent: float
-    ) -> int:
-        """Draws a random integer between given minimum and maximum values, with a certain
-        distribution. In order to distribute the values you use the exponent:
-        - exponent &#8804; 0: Completely random values will be given, almost always not between the
-        given minimum and maximum values. This usage is not encouraged.
-        - 0 < exponent < 1: The values near the maximum have a greater probability of being drawn,
-        closer the exponent is to 0.
-        - exponent = 1: All the values have the same probability of being drawn.
-        - exponent &#8805; 1: The values near the minimum have a greater probability of being
-        drawn, greater exponents will increase this probability.
-
-        Params
-        ------
-        - minimum -> The minimum value to draw.
-        - maximum -> The maximum value to draw.
-        - exponent -> The exponent of the distribution.
-
-        Returns
-        -------
-        An integer representing the drawn number.
-        """
-        drawing_range: int = maximum + 1 - minimum
-        random_float: float = RandomDraws._RAND.random() ** exponent
-
-        return minimum + int(drawing_range * random_float)
-
-    @staticmethod
-    def draw_bool() -> bool:
-        """Draws a random bool.
-
-        Returns
-        -------
-        The drawn boolean.
-        """
-        return RandomDraws._RAND.choice([True, False])
+"""Module for the RandomDraws class"""
+
+# Standard Libraries
+import random
+
+
+class RandomDraws:
+    """This class provides methods for drawing a specific data type in a pseudo-random way."""
+
+    _RAND = random.Random()
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
+
+    def __init__(self) -> None:
+        """Prevents the instantiation of this class.
+
+        Raises
+        ------
+        - NotImplementedError
+        """
+        raise NotImplementedError(RandomDraws._CONSTRUCTOR_ERROR)
+
+    @staticmethod
+    def draw_integer(minimum: int, maximum: int) -> int:
+        """Draws a random integer between given minimum and maximum values included.
+
+        Params
+        ------
+        - minimum -> The minimum value to draw.
+        - maximum -> The maximum value to draw
+
+        Returns
+        -------
+        An integer representing the drawn number.
+        """
+        return RandomDraws._RAND.randint(minimum, maximum)
+
+    @staticmethod
+    def draw_float(minimum: float, maximum: float) -> float:
+        """Draws a random float between given minimum and maximum values included.
+
+        Params
+        ------
+        - minimum -> The minimum value to draw.
+        - maximum -> The maximum value to draw
+
+        Returns
+        -------
+        An float representing the drawn number.
+        """
+        return RandomDraws._RAND.uniform(minimum, maximum)
+
+    @staticmethod
+    def draw_integer_with_distribution(
+        minimum: int, maximum: int, exponent: float
+    ) -> int:
+        """Draws a random integer between given minimum and maximum values, with a certain
+        distribution. In order to distribute the values you use the exponent:
+        - exponent &#8804; 0: Completely random values will be given, almost always not between the
+        given minimum and maximum values. This usage is not encouraged.
+        - 0 < exponent < 1: The values near the maximum have a greater probability of being drawn,
+        closer the exponent is to 0.
+        - exponent = 1: All the values have the same probability of being drawn.
+        - exponent &#8805; 1: The values near the minimum have a greater probability of being
+        drawn, greater exponents will increase this probability.
+
+        Params
+        ------
+        - minimum -> The minimum value to draw.
+        - maximum -> The maximum value to draw.
+        - exponent -> The exponent of the distribution.
+
+        Returns
+        -------
+        An integer representing the drawn number.
+        """
+        drawing_range: int = maximum + 1 - minimum
+        random_float: float = RandomDraws._RAND.random() ** exponent
+
+        return minimum + int(drawing_range * random_float)
+
+    @staticmethod
+    def draw_bool() -> bool:
+        """Draws a random bool.
+
+        Returns
+        -------
+        The drawn boolean.
+        """
+        return RandomDraws._RAND.choice([True, False])
```

### Comparing `kibo_pgar_lib-1.1.0/kibo_pgar_lib.egg-info/PKG-INFO` & `kibo_pgar_lib-1.2.0/kibo_pgar_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 2.1
-Name: kibo_pgar_lib
-Version: 1.1.0
-Summary: KiboPgArLib modified, documented and converted in python.
-Home-page: https://github.com/AlessandroMuscio/kibo_pgar_lib
-Author: Alessandro Muscio
-Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
-License: MIT License
-        
-        Copyright (c) 2024 Alessandro Muscio
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: source, https://github.com/AlessandroMuscio/kibo_pgar_lib
-Project-URL: download, https://pypi.org/project/kibo-unibs-fp-lib/#files
-Project-URL: tracker, https://github.com/AlessandroMuscio/kibo_pgar_lib/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Typing :: Typed
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# kibo_pgar_lib
-
-This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
-
-## Installation
-
-This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
-
-```bash
-pip install kibo-unibs-fp-lib
-```
-
-## Usage
-
-For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/wiki) (**WIP!!**).
-
-*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
-
-## Reason for Rename
-
-This library is been renamed from `kibo_unibs_fp_lib` to `kibo_pgar_lib`, basically, just for one main reason. \
-Even thought its Java counterpart `KiboUniBSFpLib` used the already established `UniBSFpLib` as its starting point, hence the name, with the two main goal being:
-
-- Refactoring the code to make it more readable and work with IntelliJ Idea.
-- Adding documentation.
-
-I can already see that this library its evolving into something pretty different from where it started and the changes are just gonna keep coming.
-
-That was the main reason, there is also a second small reason, being that this library is meant to be used for the projects of the course "*Programma Arnaldo*". That does not mean it can only be exclusively used for that (because how the hell can I know what you are using it for?) but I also wanted a way to symbolize the fact that this library was created for that purpose.
+Metadata-Version: 2.1
+Name: kibo_pgar_lib
+Version: 1.2.0
+Summary: KiboUniBSFpLib modified, documented and converted in python.
+Home-page: https://github.com/AlessandroMuscio/kibo_pgar_lib
+Author: Alessandro Muscio
+Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
+License: MIT License
+        
+        Copyright (c) 2024 Alessandro Muscio
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: source, https://github.com/AlessandroMuscio/kibo_pgar_lib
+Project-URL: download, https://pypi.org/project/kibo-unibs-fp-lib/#files
+Project-URL: tracker, https://github.com/AlessandroMuscio/kibo_pgar_lib/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# kibo_pgar_lib
+
+This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
+
+## Installation
+
+This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
+
+```bash
+pip install kibo-pgar-lib
+```
+
+## Usage
+
+For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_pgar_lib/wiki) (**WIP!!**).
+
+*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
+
+## Reason for Rename
+
+This library has been renamed from `kibo_unibs_fp_lib` to `kibo_pgar_lib`, basically, just for one main reason. \
+Even thought its Java counterpart `KiboPgArLib` used the already established `UniBSFpLib` as its starting point, hence the name, with the two main goal being:
+
+- Refactoring the code to make it more readable and work with *IntelliJ Idea*.
+- Adding documentation.
+
+I can already see that this library its evolving into something pretty different from where it started and the changes are just gonna keep coming.
+
+That was the main reason, there is also a second small reason. The main purpose of this library is being used for the projects of the course "*Programma Arnaldo*". That **does not** mean it can only be exclusively used for that (because how the hell can I know what you are using it for?) but I also wanted a way to symbolize the fact that this library was created for that purpose.
```

### Comparing `kibo_pgar_lib-1.1.0/pyproject.toml` & `kibo_pgar_lib-1.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "kibo_pgar_lib"
-version = "1.1.0"
-license = {file = "LICENSE.txt"}
-
-description = "KiboPgArLib modified, documented and converted in python."
-authors = [{ name="Alessandro Muscio", email="a.muscio001@studenti.unibs.it"}]
-requires-python = ">=3.9"
-readme = "README.md"
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.12",
-    "Typing :: Typed",
-    "Operating System :: OS Independent"
-]
-
-[project.urls]
-source = "https://github.com/AlessandroMuscio/kibo_pgar_lib"
-download = "https://pypi.org/project/kibo-unibs-fp-lib/#files"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "kibo_pgar_lib"
+version = "1.2.0"
+license = {file = "LICENSE.txt"}
+
+description = "KiboUniBSFpLib modified, documented and converted in python."
+authors = [{ name="Alessandro Muscio", email="a.muscio001@studenti.unibs.it"}]
+requires-python = ">=3.9"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.12",
+    "Typing :: Typed",
+    "Operating System :: OS Independent"
+]
+
+[project.urls]
+source = "https://github.com/AlessandroMuscio/kibo_pgar_lib"
+download = "https://pypi.org/project/kibo-unibs-fp-lib/#files"
 tracker = "https://github.com/AlessandroMuscio/kibo_pgar_lib/issues"
```

