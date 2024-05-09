# Comparing `tmp/babelfish-0.6.0b1.tar.gz` & `tmp/babelfish-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelfish-0.6.0b1.tar", max compression
+gzip compressed data, was "babelfish-0.6.1.tar", max compression
```

## Comparing `babelfish-0.6.0b1.tar` & `babelfish-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1529 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/LICENSE
--rw-r--r--   0        0        0     1766 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/README.md
--rw-r--r--   0        0        0      761 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/__init__.py
--rw-r--r--   0        0        0     9366 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/__init__.py
--rw-r--r--   0        0        0      556 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/alpha2.py
--rw-r--r--   0        0        0      559 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/alpha3b.py
--rw-r--r--   0        0        0      559 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/alpha3t.py
--rw-r--r--   0        0        0     1077 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/countryname.py
--rw-r--r--   0        0        0      551 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/name.py
--rw-r--r--   0        0        0     1774 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/opensubtitles.py
--rw-r--r--   0        0        0      847 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/scope.py
--rw-r--r--   0        0        0      898 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/converters/type.py
--rw-r--r--   0        0        0     3242 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/country.py
--rw-r--r--   0        0        0     4113 2021-07-14 06:55:54.619769 babelfish-0.6.0b1/babelfish/data/iso-3166-1.txt
--rw-r--r--   0        0        0   184527 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/babelfish/data/iso-639-3.tab
--rw-r--r--   0        0        0     9872 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/babelfish/data/iso15924-utf8-20131012.txt
--rw-r--r--   0        0        0     9582 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/babelfish/data/opensubtitles_languages.txt
--rw-r--r--   0        0        0     2332 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/babelfish/exceptions.py
--rw-r--r--   0        0        0     6874 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/babelfish/language.py
--rw-r--r--   0        0        0     2054 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/babelfish/script.py
--rw-r--r--   0        0        0     1287 2021-07-14 06:55:54.623769 babelfish-0.6.0b1/pyproject.toml
--rw-r--r--   0        0        0     2497 2021-07-14 06:56:09.066116 babelfish-0.6.0b1/setup.py
--rw-r--r--   0        0        0     2852 2021-07-14 06:56:09.066444 babelfish-0.6.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1529 2024-05-09 21:16:12.576434 babelfish-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1818 2024-05-09 21:16:12.576434 babelfish-0.6.1/README.md
+-rw-r--r--   0        0        0      761 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/__init__.py
+-rw-r--r--   0        0        0      976 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/compat.py
+-rw-r--r--   0        0        0     9361 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/__init__.py
+-rw-r--r--   0        0        0      556 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/alpha2.py
+-rw-r--r--   0        0        0      559 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/alpha3b.py
+-rw-r--r--   0        0        0      559 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/alpha3t.py
+-rw-r--r--   0        0        0     1077 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/countryname.py
+-rw-r--r--   0        0        0      551 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/name.py
+-rw-r--r--   0        0        0     1774 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/opensubtitles.py
+-rw-r--r--   0        0        0      847 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/scope.py
+-rw-r--r--   0        0        0      898 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/converters/type.py
+-rw-r--r--   0        0        0     3215 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/country.py
+-rw-r--r--   0        0        0     4113 2024-05-09 21:16:12.576434 babelfish-0.6.1/babelfish/data/iso-3166-1.txt
+-rw-r--r--   0        0        0   184527 2024-05-09 21:16:12.580434 babelfish-0.6.1/babelfish/data/iso-639-3.tab
+-rw-r--r--   0        0        0     9872 2024-05-09 21:16:12.580434 babelfish-0.6.1/babelfish/data/iso15924-utf8-20131012.txt
+-rw-r--r--   0        0        0     9582 2024-05-09 21:16:12.580434 babelfish-0.6.1/babelfish/data/opensubtitles_languages.txt
+-rw-r--r--   0        0        0     2332 2024-05-09 21:16:12.580434 babelfish-0.6.1/babelfish/exceptions.py
+-rw-r--r--   0        0        0     6847 2024-05-09 21:16:12.580434 babelfish-0.6.1/babelfish/language.py
+-rw-r--r--   0        0        0     2027 2024-05-09 21:16:12.580434 babelfish-0.6.1/babelfish/script.py
+-rw-r--r--   0        0        0     1401 2024-05-09 21:16:12.580434 babelfish-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 babelfish-0.6.1/PKG-INFO
```

### Comparing `babelfish-0.6.0b1/LICENSE` & `babelfish-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/README.md` & `babelfish-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 >>> country = babelfish.Country('GB')
 >>> country
 <Country [GB]>
 ```
 
 Built-in country converters (name):
 ```python
->>> country = babelfish.Country('GB')
+>>> country = babelfish.Country.fromname('United Kingdom')
 >>> country
 <Country [GB]>
 ```
 
 ### Language
 Language representation from 3-letter code (ISO-639-3):
 ```python
@@ -55,14 +55,16 @@
 ```
 
 Built-in language converters (alpha2, alpha3b, alpha3t, name, scope, type and opensubtitles):
 ```python
 >>> language = babelfish.Language('por', 'BR')
 >>> language.alpha2
 'pt'
+>>> language.name
+'Portuguese'
 >>> language.scope
 'individual'
 >>> language.type
 'living'
 >>> language.opensubtitles
 'pob'
 >>> babelfish.Language.fromalpha3b('fre')
```

#### html2text {}

```diff
@@ -4,23 +4,23 @@
 Usage BabelFish provides scripts, countries and languages from their respective
 ISO standards and a handy way to manipulate them with converters. ### Script
 Script representation from 4-letter code (ISO-15924): ```python >>> import
 babelfish >>> script = babelfish.Script('Hira') >>> script
 Hira]> ``` ### Country Country representation from 2-letter code (ISO-3166):
 ```python >>> country = babelfish.Country('GB') >>> country
 GB]> ``` Built-in country converters (name): ```python >>> country =
-babelfish.Country('GB') >>> country
+babelfish.Country.fromname('United Kingdom') >>> country
 GB]> ``` ### Language Language representation from 3-letter code (ISO-639-3):
 ```python >>> language = babelfish.Language("eng") >>> language
 en]> ``` Country-specific language: ```python >>> language = babelfish.Language
 ('por', 'BR') >>> language
 pt-BR]> ``` Language with specific script: ```python >>> language =
 babelfish.Language.fromalpha2('sr') >>> language.script = babelfish.Script
 ('Cyrl') >>> language
 sr-Cyrl]> ``` Built-in language converters (alpha2, alpha3b, alpha3t, name,
 scope, type and opensubtitles): ```python >>> language = babelfish.Language
-('por', 'BR') >>> language.alpha2 'pt' >>> language.scope 'individual' >>>
-language.type 'living' >>> language.opensubtitles 'pob' >>>
-babelfish.Language.fromalpha3b('fre')
+('por', 'BR') >>> language.alpha2 'pt' >>> language.name 'Portuguese' >>>
+language.scope 'individual' >>> language.type 'living' >>>
+language.opensubtitles 'pob' >>> babelfish.Language.fromalpha3b('fre')
 fr]> ``` ## License BabelFish is licensed under the [3-clause BSD license]
 (http://opensource.org/licenses/BSD-3-Clause>) Copyright (c) 2013, the
 BabelFish authors and contributors.
```

### Comparing `babelfish-0.6.0b1/babelfish/__init__.py` & `babelfish-0.6.1/babelfish/__init__.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/__init__.py` & `babelfish-0.6.1/babelfish/converters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2013 the BabelFish authors. All rights reserved.
 # Use of this source code is governed by the 3-clause BSD license
 # that can be found in the LICENSE file.
 #
-from pkg_resources import iter_entry_points, EntryPoint
+from ..compat import iter_entry_points, EntryPoint
 from ..exceptions import LanguageConvertError, LanguageReverseError
 
 try:
     # Python 3.3+
     from collections.abc import Mapping, MutableMapping
 except ImportError:
     from collections import Mapping, MutableMapping
```

### Comparing `babelfish-0.6.0b1/babelfish/converters/alpha2.py` & `babelfish-0.6.1/babelfish/converters/alpha2.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/alpha3b.py` & `babelfish-0.6.1/babelfish/converters/alpha3b.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/alpha3t.py` & `babelfish-0.6.1/babelfish/converters/alpha3t.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/countryname.py` & `babelfish-0.6.1/babelfish/converters/countryname.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/name.py` & `babelfish-0.6.1/babelfish/converters/name.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/opensubtitles.py` & `babelfish-0.6.1/babelfish/converters/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/scope.py` & `babelfish-0.6.1/babelfish/converters/scope.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/converters/type.py` & `babelfish-0.6.1/babelfish/converters/type.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/country.py` & `babelfish-0.6.1/babelfish/country.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Copyright (c) 2013 the BabelFish authors. All rights reserved.
 # Use of this source code is governed by the 3-clause BSD license
 # that can be found in the LICENSE file.
 #
 from __future__ import unicode_literals
 from collections import namedtuple
 from functools import partial
-from pkg_resources import resource_stream  # @UnresolvedImport
 from .converters import ConverterManager
 from . import basestr
+from .compat import resource_stream
 
 
 COUNTRIES = {}
 COUNTRY_MATRIX = []
 
 #: The namedtuple used in the :data:`COUNTRY_MATRIX`
 IsoCountry = namedtuple('IsoCountry', ['name', 'alpha2'])
```

### Comparing `babelfish-0.6.0b1/babelfish/data/iso-3166-1.txt` & `babelfish-0.6.1/babelfish/data/iso-3166-1.txt`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/data/iso-639-3.tab` & `babelfish-0.6.1/babelfish/data/iso-639-3.tab`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/data/iso15924-utf8-20131012.txt` & `babelfish-0.6.1/babelfish/data/iso15924-utf8-20131012.txt`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/data/opensubtitles_languages.txt` & `babelfish-0.6.1/babelfish/data/opensubtitles_languages.txt`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/exceptions.py` & `babelfish-0.6.1/babelfish/exceptions.py`

 * *Files identical despite different names*

### Comparing `babelfish-0.6.0b1/babelfish/language.py` & `babelfish-0.6.1/babelfish/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # Copyright (c) 2013 the BabelFish authors. All rights reserved.
 # Use of this source code is governed by the 3-clause BSD license
 # that can be found in the LICENSE file.
 #
 from __future__ import unicode_literals
 from collections import namedtuple
 from functools import partial
-from pkg_resources import resource_stream  # @UnresolvedImport
 from .converters import ConverterManager
 from .country import Country
 from .exceptions import LanguageConvertError
 from .script import Script
 from . import basestr
+from .compat import resource_stream
 
 
 LANGUAGES = set()
 LANGUAGE_MATRIX = []
 
 #: The namedtuple used in the :data:`LANGUAGE_MATRIX`
 IsoLanguage = namedtuple('IsoLanguage', ['alpha3', 'alpha3b', 'alpha3t', 'alpha2', 'scope', 'type', 'name', 'comment'])
```

### Comparing `babelfish-0.6.0b1/babelfish/script.py` & `babelfish-0.6.1/babelfish/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # Copyright (c) 2013 the BabelFish authors. All rights reserved.
 # Use of this source code is governed by the 3-clause BSD license
 # that can be found in the LICENSE file.
 #
 from __future__ import unicode_literals
 from collections import namedtuple
-from pkg_resources import resource_stream  # @UnresolvedImport
 from . import basestr
+from .compat import resource_stream
 
 #: Script code to script name mapping
 SCRIPTS = {}
 
 #: List of countries in the ISO-15924 as namedtuple of code, number, name, french_name, pva and date
 SCRIPT_MATRIX = []
```

### Comparing `babelfish-0.6.0b1/pyproject.toml` & `babelfish-0.6.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "babelfish"
-version = "0.6.0-beta.1"
+version = "0.6.1"
 description = "A module to work with countries and languages"
 authors = [
     "Antoine Bertin <ant.bertin@gmail.com>",
     "Nicolas Wack <wackou@gmail.com>",
     "Rémi Alvergnat <toilal.dev@gmail.com>",
 ]
 license = "BSD-3-Clause"
@@ -19,26 +19,27 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Internationalization",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-include = ["data/"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
+importlib-resources = {version = "^5.0", python = "<3.9"}
+importlib-metadata = {version = "^4.6", python = "<3.10"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.4"
-pytest-cov = "^2.12.1"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `babelfish-0.6.0b1/PKG-INFO` & `babelfish-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: babelfish
-Version: 0.6.0b1
+Version: 0.6.1
 Summary: A module to work with countries and languages
 Home-page: https://github.com/Diaoul/babelfish
 License: BSD-3-Clause
 Keywords: language,country,locale
 Author: Antoine Bertin
 Author-email: ant.bertin@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: importlib-metadata (>=4.6,<5.0) ; python_version < "3.10"
+Requires-Dist: importlib-resources (>=5.0,<6.0) ; python_version < "3.9"
 Project-URL: Repository, https://github.com/Diaoul/babelfish
 Description-Content-Type: text/markdown
 
 # BabelFish
 BabelFish is a Python library to work with countries and languages.
 
 [![tests](https://github.com/Diaoul/babelfish/actions/workflows/test.yml/badge.svg)](https://github.com/Diaoul/babelfish/actions/workflows/test.yml)
@@ -48,15 +51,15 @@
 >>> country = babelfish.Country('GB')
 >>> country
 <Country [GB]>
 ```
 
 Built-in country converters (name):
 ```python
->>> country = babelfish.Country('GB')
+>>> country = babelfish.Country.fromname('United Kingdom')
 >>> country
 <Country [GB]>
 ```
 
 ### Language
 Language representation from 3-letter code (ISO-639-3):
 ```python
@@ -81,14 +84,16 @@
 ```
 
 Built-in language converters (alpha2, alpha3b, alpha3t, name, scope, type and opensubtitles):
 ```python
 >>> language = babelfish.Language('por', 'BR')
 >>> language.alpha2
 'pt'
+>>> language.name
+'Portuguese'
 >>> language.scope
 'individual'
 >>> language.type
 'living'
 >>> language.opensubtitles
 'pob'
 >>> babelfish.Language.fromalpha3b('fre')
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: babelfish Version: 0.6.0b1 Summary: A module to
-work with countries and languages Home-page: https://github.com/Diaoul/
-babelfish License: BSD-3-Clause Keywords: language,country,locale Author:
-Antoine Bertin Author-email: ant.bertin@gmail.com Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Software Development :: Internationalization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Repository, https://github.com/Diaoul/babelfish Description-
-Content-Type: text/markdown # BabelFish BabelFish is a Python library to work
-with countries and languages. [![tests](https://github.com/Diaoul/babelfish/
-actions/workflows/test.yml/badge.svg)](https://github.com/Diaoul/babelfish/
-actions/workflows/test.yml) ## Usage BabelFish provides scripts, countries and
-languages from their respective ISO standards and a handy way to manipulate
-them with converters. ### Script Script representation from 4-letter code (ISO-
-15924): ```python >>> import babelfish >>> script = babelfish.Script('Hira')
->>> script
+Metadata-Version: 2.1 Name: babelfish Version: 0.6.1 Summary: A module to work
+with countries and languages Home-page: https://github.com/Diaoul/babelfish
+License: BSD-3-Clause Keywords: language,country,locale Author: Antoine Bertin
+Author-email: ant.bertin@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development :: Internationalization Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Dist: importlib-metadata
+(>=4.6,<5.0) ; python_version < "3.10" Requires-Dist: importlib-resources
+(>=5.0,<6.0) ; python_version < "3.9" Project-URL: Repository, https://
+github.com/Diaoul/babelfish Description-Content-Type: text/markdown # BabelFish
+BabelFish is a Python library to work with countries and languages. [![tests]
+(https://github.com/Diaoul/babelfish/actions/workflows/test.yml/badge.svg)]
+(https://github.com/Diaoul/babelfish/actions/workflows/test.yml) ## Usage
+BabelFish provides scripts, countries and languages from their respective ISO
+standards and a handy way to manipulate them with converters. ### Script Script
+representation from 4-letter code (ISO-15924): ```python >>> import babelfish
+>>> script = babelfish.Script('Hira') >>> script
 Hira]> ``` ### Country Country representation from 2-letter code (ISO-3166):
 ```python >>> country = babelfish.Country('GB') >>> country
 GB]> ``` Built-in country converters (name): ```python >>> country =
-babelfish.Country('GB') >>> country
+babelfish.Country.fromname('United Kingdom') >>> country
 GB]> ``` ### Language Language representation from 3-letter code (ISO-639-3):
 ```python >>> language = babelfish.Language("eng") >>> language
 en]> ``` Country-specific language: ```python >>> language = babelfish.Language
 ('por', 'BR') >>> language
 pt-BR]> ``` Language with specific script: ```python >>> language =
 babelfish.Language.fromalpha2('sr') >>> language.script = babelfish.Script
 ('Cyrl') >>> language
 sr-Cyrl]> ``` Built-in language converters (alpha2, alpha3b, alpha3t, name,
 scope, type and opensubtitles): ```python >>> language = babelfish.Language
-('por', 'BR') >>> language.alpha2 'pt' >>> language.scope 'individual' >>>
-language.type 'living' >>> language.opensubtitles 'pob' >>>
-babelfish.Language.fromalpha3b('fre')
+('por', 'BR') >>> language.alpha2 'pt' >>> language.name 'Portuguese' >>>
+language.scope 'individual' >>> language.type 'living' >>>
+language.opensubtitles 'pob' >>> babelfish.Language.fromalpha3b('fre')
 fr]> ``` ## License BabelFish is licensed under the [3-clause BSD license]
 (http://opensource.org/licenses/BSD-3-Clause>) Copyright (c) 2013, the
 BabelFish authors and contributors.
```

