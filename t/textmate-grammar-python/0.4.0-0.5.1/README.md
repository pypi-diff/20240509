# Comparing `tmp/textmate_grammar_python-0.4.0.tar.gz` & `tmp/textmate_grammar_python-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textmate_grammar_python-0.4.0.tar", max compression
+gzip compressed data, was "textmate_grammar_python-0.5.1.tar", max compression
```

## Comparing `textmate_grammar_python-0.4.0.tar` & `textmate_grammar_python-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2024-02-28 10:00:04.451773 textmate_grammar_python-0.4.0/LICENSE
--rw-r--r--   0        0        0     5085 2024-03-26 19:33:21.226060 textmate_grammar_python-0.4.0/README.md
--rw-r--r--   0        0        0     2382 2024-03-26 19:50:04.825282 textmate_grammar_python-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-26 19:50:04.853283 textmate_grammar_python-0.4.0/src/textmate_grammar/__init__.py
--rw-r--r--   0        0        0    20041 2024-03-26 19:33:21.226060 textmate_grammar_python-0.4.0/src/textmate_grammar/elements.py
--rw-r--r--   0        0        0        0 2024-02-28 10:00:04.451773 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/__init__.py
--rw-r--r--   0        0        0     1076 2024-02-28 10:00:04.451773 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/markdown/LICENSE.txt
--rw-r--r--   0        0        0      530 2024-03-26 19:39:36.485900 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/markdown/__init__.py
--rw-r--r--   0        0        0    22103 2024-02-28 10:00:04.451773 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/markdown/grammar.yaml
--rw-r--r--   0        0        0      736 2024-03-26 19:39:43.021983 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/matlab/__init__.py
--rw-r--r--   0        0        0    36373 2024-02-28 10:00:04.455772 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/matlab/grammar.yaml
--rw-r--r--   0        0        0     1271 2024-02-28 10:00:04.455772 textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/matlab/license.txt
--rw-r--r--   0        0        0     6390 2024-03-26 19:38:57.729400 textmate_grammar_python-0.4.0/src/textmate_grammar/language.py
--rw-r--r--   0        0        0    35809 2024-03-08 14:48:57.212572 textmate_grammar_python-0.4.0/src/textmate_grammar/parser.py
--rw-r--r--   0        0        0        0 2024-02-28 10:00:04.455772 textmate_grammar_python-0.4.0/src/textmate_grammar/py.typed
--rw-r--r--   0        0        0        0 2024-03-08 14:48:57.212572 textmate_grammar_python-0.4.0/src/textmate_grammar/utils/__init__.py
--rw-r--r--   0        0        0     5107 2024-03-26 19:43:43.944940 textmate_grammar_python-0.4.0/src/textmate_grammar/utils/cache.py
--rw-r--r--   0        0        0     2133 2024-03-26 19:39:14.401615 textmate_grammar_python-0.4.0/src/textmate_grammar/utils/exceptions.py
--rw-r--r--   0        0        0    11678 2024-03-26 19:39:19.817685 textmate_grammar_python-0.4.0/src/textmate_grammar/utils/handler.py
--rw-r--r--   0        0        0     5673 2024-03-26 19:41:08.503058 textmate_grammar_python-0.4.0/src/textmate_grammar/utils/logger.py
--rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 textmate_grammar_python-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5028 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/README.md
+-rw-r--r--   0        0        0     2454 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/__init__.py
+-rw-r--r--   0        0        0    20035 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/elements.py
+-rw-r--r--   0        0        0    12051 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/handler.py
+-rw-r--r--   0        0        0    35912 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parser.py
+-rw-r--r--   0        0        0        0 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/__init__.py
+-rw-r--r--   0        0        0     6930 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/base.py
+-rw-r--r--   0        0        0     1076 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/LICENSE.txt
+-rw-r--r--   0        0        0      770 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/__init__.py
+-rw-r--r--   0        0        0    22103 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/grammar.yaml
+-rw-r--r--   0        0        0     2074 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/__init__.py
+-rw-r--r--   0        0        0    36373 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/grammar.yaml
+-rw-r--r--   0        0        0     1271 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/license.txt
+-rw-r--r--   0        0        0        0 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/py.typed
+-rw-r--r--   0        0        0        0 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/__init__.py
+-rw-r--r--   0        0        0     5107 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/cache.py
+-rw-r--r--   0        0        0     2133 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/exceptions.py
+-rw-r--r--   0        0        0     5673 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/logger.py
+-rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 textmate_grammar_python-0.5.1/PKG-INFO
```

### Comparing `textmate_grammar_python-0.4.0/LICENSE` & `textmate_grammar_python-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/README.md` & `textmate_grammar_python-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 ```bash
 pip install textmate-grammar-python
 ```
 
 Before tokenization is possible, a `LanguageParser` needs to be initialized using a loaded grammar. 
 
 ```python
-from textmate_grammar.language import LanguageParser
-from textmate_grammar.grammars import matlab
-parser = LanguageParser(matlab.GRAMMAR)
+from textmate_grammar.parsers.matlab import MatlabParser
+parser = MatlabParser()
 ```
 
 After this, one can either choose to call [`parser.parsing_string`](https://textmate-grammar-python.readthedocs.io/en/latest/apidocs/textmate_grammar/textmate_grammar.language.html#textmate_grammar.language.LanguageParser.parse_string) to parse a input string directly, or call [`parser.parse_file`](https://textmate-grammar-python.readthedocs.io/en/latest/apidocs/textmate_grammar/textmate_grammar.language.html#textmate_grammar.language.LanguageParser.parse_file) with the path to the appropiate source file as the first argument, such as in the example [`example.py`](https://github.com/watermarkhu/textmate-grammar-python/blob/main/example.py). 
 
 The parsed `element` object can be displayed directly by calling the [`print`](https://textmate-grammar-python.readthedocs.io/en/latest/apidocs/textmate_grammar/textmate_grammar.elements.html#textmate_grammar.elements.ContentElement.print) method. By default the element is printed as an element tree in a dictionary format. 
 
 ```python
```

### Comparing `textmate_grammar_python-0.4.0/pyproject.toml` & `textmate_grammar_python-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+[project]
+name = "textmate-grammar-python"
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "textmate-grammar-python"
-version = "0.4.0"
+version = "0.5.1"
 description = "A lexer and tokenizer for grammar files as defined by TextMate and used in VSCode, implemented in Python."
 authors = ["Mark Shui Hu <watermarkhu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/watermarkhu/textmate-grammar-python"
 documentation = "https://textmate-grammar-python.readthedocs.io"
 keywords = ["textmate", "tokenization"]
 packages = [{include = "textmate_grammar", from = "src"}]
 
+[tool.rye]
+managed = true
+
 [tool.poetry.dependencies]
 python = "^3.9"
 onigurumacffi = "^1.3.0"
 PyYAML = "^6.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.3.1,<9.0.0"
```

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/elements.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from abc import ABC
 from collections import defaultdict
 from itertools import groupby
 from pprint import pprint
 from typing import TYPE_CHECKING, Generator
 
-from .utils.handler import POS, ContentHandler, Match, Pattern
+from .handler import POS, ContentHandler, Match, Pattern
 from .utils.logger import LOGGER
 
 if TYPE_CHECKING:
     from .parser import GrammarParser
 
 
 TOKEN_DICT = dict[POS, list[str]]
```

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/markdown/LICENSE.txt` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/markdown/__init__.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import annotations
 
 import shutil
 from pathlib import Path
 
 import yaml
 
-tmLanguageFile = (
-    Path(__file__).parents[3] / "syntaxes" / "markdown" / "markdown.tmLanguage.base.yaml"
-)
-tmLanguageYAML = Path(__file__).parent / "grammar.yaml"
+from ..base import LanguageParser
 
 
-if tmLanguageFile.exists():
-    shutil.copyfile(tmLanguageFile, tmLanguageYAML)
-
-with open(tmLanguageYAML) as file:
-    try:
-        GRAMMAR = yaml.load(file.read(), Loader=yaml.CLoader)
-    except ImportError:
-        GRAMMAR = yaml.load(file.read(), Loader=yaml.Loader)
+class MarkdownParser(LanguageParser):
+    def __init__(self, **kwargs):
+        tmLanguageFile = (
+            Path(__file__).parents[3] / "syntaxes" / "markdown" / "markdown.tmLanguage.base.yaml"
+        )
+        tmLanguageYAML = Path(__file__).parent / "grammar.yaml"
+
+        if tmLanguageFile.exists():
+            shutil.copyfile(tmLanguageFile, tmLanguageYAML)
+
+        with open(tmLanguageYAML) as file:
+            try:
+                grammar = yaml.load(file.read(), Loader=yaml.CLoader)
+            except ImportError:
+                grammar = yaml.load(file.read(), Loader=yaml.Loader)
+
+        super().__init__(grammar, **kwargs)
```

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/markdown/grammar.yaml` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/grammar.yaml`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/matlab/grammar.yaml` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/grammar.yaml`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/grammars/matlab/license.txt` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/license.txt`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/language.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from pathlib import Path
 
-from .elements import Capture, ContentElement
-from .parser import GrammarParser, PatternsParser
-from .utils.cache import TextmateCache, init_cache
-from .utils.exceptions import IncompatibleFileType
-from .utils.handler import POS, ContentHandler
-from .utils.logger import LOGGER
+from ..elements import Capture, ContentElement
+from ..handler import POS, ContentHandler
+from ..parser import GrammarParser, PatternsParser
+from ..utils.cache import TextmateCache, init_cache
+from ..utils.exceptions import IncompatibleFileType
+from ..utils.logger import LOGGER
 
 LANGUAGE_PARSERS = {}
 
 
 class DummyParser(GrammarParser):
     """A dummy parser object"""
 
@@ -30,47 +30,61 @@
     """The parser of a language grammar."""
 
     def __init__(self, grammar: dict, **kwargs):
         """
         Initialize a Language object.
 
         :param grammar: The grammar definition for the language.
+        :type grammar: dict
+        :param pre_processor: A pre-processor to use on the input string of the parser
+        :type pre_processor: BasePreProcessor
         :param kwargs: Additional keyword arguments.
 
         :ivar name: The name of the language.
         :ivar uuid: The UUID of the language.
         :ivar file_types: The file types associated with the language.
         :ivar token: The scope name of the language.
         :ivar repository: The repository of grammar rules for the language.
         :ivar injections: The list of injection rules for the language.
         :ivar _cache: The cache object for the language.
         """
-        super().__init__(grammar, key=grammar.get("name", "myLanguage"), language=self, **kwargs)
+
+        super().__init__(
+            grammar, key=grammar.get("name", "myLanguage"), language_parser=self, **kwargs
+        )
 
         self.name = grammar.get("name", "")
         self.uuid = grammar.get("uuid", "")
         self.file_types = grammar.get("fileTypes", [])
         self.token = grammar.get("scopeName", "myScope")
         self.repository = {}
         self.injections: list[dict] = []
         self._cache: TextmateCache = init_cache()
 
         # Initialize grammars in repository
         for repo in _gen_repositories(grammar):
             for key, parser_grammar in repo.items():
                 self.repository[key] = GrammarParser.initialize(
-                    parser_grammar, key=key, language=self
+                    parser_grammar, key=key, language_parser=self
                 )
 
         # Update language parser store
         language_name = grammar.get("scopeName", "myLanguage")
         LANGUAGE_PARSERS[language_name] = self
 
         self._initialize_repository()
 
+    def pre_process(self, input: str) -> str:
+        """
+        Pre-processes the input string before parsing.
+
+        This method can be overloaded in language specific parsers with custom pre-processing logic.
+        """
+        return input
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}:{self.key}"
 
     @staticmethod
     def _find_include_scopes(key: str):
         return LANGUAGE_PARSERS.get(key, DummyParser())
 
@@ -84,15 +98,15 @@
             if not target_string:
                 target_string = self.grammar.get("scopeName", "myLanguage")
             target_language = LANGUAGE_PARSERS[target_string]
 
             injected_parser = GrammarParser.initialize(
                 injected_grammar,
                 key=f"{target_string}.injection",
-                language=target_language,
+                language_parser=target_language,
             )
             injected_parser._initialize_repository()
 
             scope_string = key[key.index("-") :]
             exception_scopes = [s.strip() for s in scope_string.split("-") if s.strip()]
             target_language.injections.append([exception_scopes, injected_parser])
 
@@ -111,16 +125,16 @@
 
         if filePath.suffix.split(".")[-1] not in self.file_types:
             raise IncompatibleFileType(extensions=self.file_types)
 
         if self._cache.cache_valid(filePath):
             element = self._cache.load(filePath)
         else:
-            handler = ContentHandler.from_path(filePath)
-            if handler.source == "":
+            handler = ContentHandler.from_path(filePath, pre_processor=self.pre_process, **kwargs)
+            if handler.content == "":
                 return None
 
             # Configure logger
             LOGGER.configure(self, height=len(handler.lines), width=max(handler.line_lengths))
             element = self._parse_language(handler, **kwargs)  # type: ignore
 
             if element is not None:
@@ -131,15 +145,16 @@
         """
         Parses an input string.
 
         :param input: The input string to be parsed.
         :param kwargs: Additional keyword arguments.
         :return: The result of parsing the input string.
         """
-        handler = ContentHandler(input)
+        handler = ContentHandler(input, pre_processor=self.pre_process, **kwargs)
+
         # Configure logger
         LOGGER.configure(self, height=len(handler.lines), width=max(handler.line_lengths))
 
         element = self._parse_language(handler, **kwargs)
 
         return element
```

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/parser.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 import onigurumacffi as re
 
 from .elements import Capture, ContentBlockElement, ContentElement
+from .handler import POS, ContentHandler, Pattern
 from .utils.exceptions import IncludedParserNotFound
-from .utils.handler import POS, ContentHandler, Pattern
 from .utils.logger import LOGGER, track_depth
 
 if TYPE_CHECKING:
-    from .language import LanguageParser
+    from .parsers.base import LanguageParser
 
 
 class GrammarParser(ABC):
     """The abstract grammar parser object"""
 
     @staticmethod
     def initialize(grammar: dict, **kwargs):
@@ -38,15 +38,15 @@
             return PatternsParser(grammar, **kwargs)
         else:
             return TokenParser(grammar, **kwargs)
 
     def __init__(
         self,
         grammar: dict,
-        language: LanguageParser | None = None,
+        language_parser: LanguageParser | None = None,
         key: str = "",
         is_capture: bool = False,
         **kwargs,
     ) -> None:
         """
         Initialize a Parser object.
 
@@ -55,15 +55,15 @@
         :param key: The key for the parser. Defaults to "".
         :param is_capture: Indicates if the parser is a capture. Defaults to False.
         :param kwargs: Additional keyword arguments.
 
         :return: None
         """
         self.grammar = grammar
-        self.language = language
+        self.language_parser = language_parser
         self.key = key
         self.token = grammar.get("name", "")
         self.is_capture = is_capture
         self.initialized = False
         self.anchored = False
 
     @property
@@ -79,29 +79,29 @@
 
     def _init_captures(self, grammar: dict, key: str = "captures", **kwargs) -> dict:
         """Initializes a captures dictionary"""
         captures = {}
         if key in grammar:
             for group_id, pattern in grammar[key].items():
                 captures[int(group_id)] = self.initialize(
-                    pattern, language=self.language, is_capture=True
+                    pattern, language_parser=self.language_parser, is_capture=True
                 )
         return captures
 
     def _find_include(self, key: str, **kwargs) -> GrammarParser:
         """Find the included grammars and during repository initialization"""
-        if not self.language:
+        if not self.language_parser:
             raise IncludedParserNotFound(key)
 
         if key in ["$self", "$base"]:  # TODO there is a difference between these
-            return self.language
+            return self.language_parser
         elif key[0] == "#":
-            return self.language.repository.get(key[1:], None)
+            return self.language_parser.repository.get(key[1:], None)
         else:
-            return self.language._find_include_scopes(key)
+            return self.language_parser._find_include_scopes(key)
 
     @abstractmethod
     def _parse(
         self,
         handler: ContentHandler,
         starting: POS,
         **kwargs,
@@ -142,16 +142,16 @@
         :param **kwargs: Additional keyword arguments that can be passed to the parser.
 
         :return: A tuple containing:
             - parsed: A boolean indicating whether the parsing was successful.
             - elements: A list of Capture or ContentElement objects representing the parsed content.
             - span: A tuple containing the starting and ending positions of the parsed content, or None if parsing failed.
         """
-        if not self.initialized and self.language is not None:
-            self.language._initialize_repository()
+        if not self.initialized and self.language_parser is not None:
+            self.language_parser._initialize_repository()
         parsed, elements, span = self._parse(handler, starting, boundary=boundary, **kwargs)
         return parsed, elements, span
 
     def match_and_capture(
         self,
         handler: ContentHandler,
         pattern: Pattern,
@@ -321,15 +321,15 @@
         return True, elements, span
 
 
 class ParserHasPatterns(GrammarParser, ABC):
     def __init__(self, grammar: dict, **kwargs) -> None:
         super().__init__(grammar, **kwargs)
         self.patterns = [
-            self.initialize(pattern, language=self.language)
+            self.initialize(pattern, language_parser=self.language_parser)
             for pattern in grammar.get("patterns", [])
         ]
 
     def _initialize_repository(self):
         """When the grammar has patterns, this method should called to initialize its inclusions."""
         self.initialized = True
         self.patterns = [
@@ -343,15 +343,15 @@
         # Copy patterns from included pattern parsers
         pattern_parsers = [parser for parser in self.patterns if isinstance(parser, PatternsParser)]
         for parser in pattern_parsers:
             parser_index = self.patterns.index(parser)
             self.patterns[parser_index : parser_index + 1] = parser.patterns
 
         # Injection grammars
-        for exception_scopes, injection_pattern in self.language.injections:
+        for exception_scopes, injection_pattern in self.language_parser.injections:
             if self.token:
                 if self.token.split(".")[0] not in exception_scopes:
                     self.patterns.append(injection_pattern)
             elif self.is_capture:
                 self.patterns.append(injection_pattern)
 
 
@@ -438,15 +438,15 @@
                     elements.extend(options_elements[parser])
                     LOGGER.info(
                         f"{self.__class__.__name__} chosen pattern of {parser}",
                         self,
                         current,
                         kwargs.get("depth", 0),
                     )
-                elif self != self.language:
+                elif self != self.language_parser:
                     break
                 else:
                     remainder = handler.read_line(current)
                     if not remainder.isspace():
                         LOGGER.warning(
                             f"{self.__class__.__name__} remainder of line not parsed: {remainder}",
                             self,
```

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/utils/cache.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/utils/cache.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/utils/exceptions.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/utils/handler.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from __future__ import annotations
 
 from pathlib import Path
+from typing import Callable
 
 from onigurumacffi import _Match as Match
 from onigurumacffi import _Pattern as Pattern
 from onigurumacffi import compile
 
-from .exceptions import FileNotFound, ImpossibleSpan
-from .logger import LOGGER
+from .utils.exceptions import FileNotFound, ImpossibleSpan
+from .utils.logger import LOGGER
 
 POS = tuple[int, int]
 
 
+def _dummy_pre_processor(input: str) -> str:
+    return input
+
+
 class ContentHandler:
     """The handler object targetted for parsing.
 
     To parse a string or file, it needs to be loaded into the ContentHandler object.
     The handler will take care of all read actions on the input stream, where the contents
     are index by a tuple (line_number, line_position). Additionally, the handler contains the
     search method to match a search span against a input oniguruma regex pattern.
     """
 
     notLookForwardEOL = compile(r"(?<!\(\?=[^\(]*)\$")
 
-    def __init__(self, source: str) -> None:
+    def __init__(
+        self, content: str, pre_processor: Callable[[str], str] = _dummy_pre_processor
+    ) -> None:
         """
         Initialize a new instance of the Handler class.
 
-        :param source: The source code to be processed.
-        :type source: str
+        :param content: The source code to be processed.
+        :type content: str
+        :param pre_processor: A pre-processor to use on the input string of the parser
+        :type pre_processor: BasePreProcessor
 
-        :ivar source: The source code to be processed.
+        :ivar content: The source code to be processed.
         :ivar lines: A list of lines in the source code, with a newline character at the end of each line.
         :ivar line_lengths: A list of lengths of each line in the source code.
         :ivar anchor: The current position in the source code.
         """
-        self.source = source
-        self.lines = [line + "\n" for line in source.split("\n")]
+        prepared_content = pre_processor(content.replace("\r\n", "\n").replace("\r", "\n"))
+
+        self.content = prepared_content
+        self.lines = [line + "\n" for line in prepared_content.split("\n")]
         self.line_lengths = [len(line) for line in self.lines]
         self.anchor: int = 0
 
     @classmethod
-    def from_path(cls, file_path: Path):
+    def from_path(cls, file_path: Path, **kwargs) -> ContentHandler:
         """Loads a file from a path"""
 
         if not file_path.exists():
             raise FileNotFound(str(file_path))
 
         # Open file and replace Windows/Mac line endings
         with open(file_path) as file:
             content = file.read()
-        content = content.replace("\r\n", "\n")
-        content = content.replace("\r", "\n")
 
-        return cls(content)
+        return cls(content, **kwargs)
 
     def _check_pos(self, pos: POS):
         if pos[0] > len(self.lines) or pos[1] > self.line_lengths[pos[0]]:
             raise ImpossibleSpan
 
     def next(self, pos: POS, step: int = 1) -> POS:
         """Returns the next position on the current handler.
```

### Comparing `textmate_grammar_python-0.4.0/src/textmate_grammar/utils/logger.py` & `textmate_grammar_python-0.5.1/src/textmate_grammar/utils/logger.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.4.0/PKG-INFO` & `textmate_grammar_python-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textmate-grammar-python
-Version: 0.4.0
+Version: 0.5.1
 Summary: A lexer and tokenizer for grammar files as defined by TextMate and used in VSCode, implemented in Python.
 Home-page: https://github.com/watermarkhu/textmate-grammar-python
 License: MIT
 Keywords: textmate,tokenization
 Author: Mark Shui Hu
 Author-email: watermarkhu@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -40,17 +40,16 @@
 ```bash
 pip install textmate-grammar-python
 ```
 
 Before tokenization is possible, a `LanguageParser` needs to be initialized using a loaded grammar. 
 
 ```python
-from textmate_grammar.language import LanguageParser
-from textmate_grammar.grammars import matlab
-parser = LanguageParser(matlab.GRAMMAR)
+from textmate_grammar.parsers.matlab import MatlabParser
+parser = MatlabParser()
 ```
 
 After this, one can either choose to call [`parser.parsing_string`](https://textmate-grammar-python.readthedocs.io/en/latest/apidocs/textmate_grammar/textmate_grammar.language.html#textmate_grammar.language.LanguageParser.parse_string) to parse a input string directly, or call [`parser.parse_file`](https://textmate-grammar-python.readthedocs.io/en/latest/apidocs/textmate_grammar/textmate_grammar.language.html#textmate_grammar.language.LanguageParser.parse_file) with the path to the appropiate source file as the first argument, such as in the example [`example.py`](https://github.com/watermarkhu/textmate-grammar-python/blob/main/example.py). 
 
 The parsed `element` object can be displayed directly by calling the [`print`](https://textmate-grammar-python.readthedocs.io/en/latest/apidocs/textmate_grammar/textmate_grammar.elements.html#textmate_grammar.elements.ContentElement.print) method. By default the element is printed as an element tree in a dictionary format. 
 
 ```python
```

