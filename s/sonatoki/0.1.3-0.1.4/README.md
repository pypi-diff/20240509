# Comparing `tmp/sonatoki-0.1.3.tar.gz` & `tmp/sonatoki-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatoki-0.1.3.tar", last modified: Sun May  5 21:18:08 2024, max compression
+gzip compressed data, was "sonatoki-0.1.4.tar", last modified: Thu May  9 15:18:28 2024, max compression
```

## Comparing `sonatoki-0.1.3.tar` & `sonatoki-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2024-05-05 21:17:54.139527 sonatoki-0.1.3/LICENSE
--rw-r--r--   0        0        0     4765 2024-05-05 21:17:54.139527 sonatoki-0.1.3/README.md
--rw-r--r--   0        0        0     2013 2024-05-05 21:18:08.203592 sonatoki-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Cleaners.py
--rw-r--r--   0        0        0     1939 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Configs.py
--rw-r--r--   0        0        0     4194 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Filters.py
--rw-r--r--   0        0        0     3347 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Preprocessors.py
--rw-r--r--   0        0        0     4129 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Scorers.py
--rw-r--r--   0        0        0     1942 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Tokenizers.py
--rw-r--r--   0        0        0        0 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/__init__.py
--rw-r--r--   0        0        0       82 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/__main__.py
--rw-r--r--   0        0        0     1647 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/constants.py
--rw-r--r--   0        0        0     4343 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/ilo.py
--rw-r--r--   0        0        0   271013 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/linku.json
--rw-r--r--   0        0        0    77650 2024-05-05 21:17:54.143527 sonatoki-0.1.3/src/sonatoki/sandbox.json
--rw-r--r--   0        0        0        0 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_cleaners.py
--rw-r--r--   0        0        0     2536 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_filters.py
--rw-r--r--   0        0        0     4063 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_ilo.py
--rw-r--r--   0        0        0     2808 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_preprocessors.py
--rw-r--r--   0        0        0      986 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_scorers.py
--rw-r--r--   0        0        0     3039 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_tokenize.py
--rw-r--r--   0        0        0      821 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_utils.py
--rw-r--r--   0        0        0      151 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_sentences.yml
--rw-r--r--   0        0        0      743 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_sentences_tok.yml
--rw-r--r--   0        0        0      440 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_words.yml
--rw-r--r--   0        0        0     1522 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_words_tok.yml
--rw-r--r--   0        0        0     5225 1970-01-01 00:00:00.000000 sonatoki-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-09 15:18:10.812224 sonatoki-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4765 2024-05-09 15:18:10.812224 sonatoki-0.1.4/README.md
+-rw-r--r--   0        0        0     2013 2024-05-09 15:18:28.876055 sonatoki-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Cleaners.py
+-rw-r--r--   0        0        0     1935 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Configs.py
+-rw-r--r--   0        0        0     4190 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Filters.py
+-rw-r--r--   0        0        0     4205 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Preprocessors.py
+-rw-r--r--   0        0        0     4129 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Scorers.py
+-rw-r--r--   0        0        0     1942 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Tokenizers.py
+-rw-r--r--   0        0        0        0 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/__main__.py
+-rw-r--r--   0        0        0     1647 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/constants.py
+-rw-r--r--   0        0        0     4343 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/ilo.py
+-rw-r--r--   0        0        0   271013 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/linku.json
+-rw-r--r--   0        0        0    77650 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/sandbox.json
+-rw-r--r--   0        0        0        0 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_cleaners.py
+-rw-r--r--   0        0        0     2530 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_filters.py
+-rw-r--r--   0        0        0     4063 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_ilo.py
+-rw-r--r--   0        0        0     4145 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_preprocessors.py
+-rw-r--r--   0        0        0     1062 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_scorers.py
+-rw-r--r--   0        0        0     3039 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_tokenize.py
+-rw-r--r--   0        0        0      821 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_utils.py
+-rw-r--r--   0        0        0      151 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_sentences.yml
+-rw-r--r--   0        0        0      743 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_sentences_tok.yml
+-rw-r--r--   0        0        0      440 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_words.yml
+-rw-r--r--   0        0        0     1522 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_words_tok.yml
+-rw-r--r--   0        0        0     5225 1970-01-01 00:00:00.000000 sonatoki-0.1.4/PKG-INFO
```

### Comparing `sonatoki-0.1.3/LICENSE` & `sonatoki-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/README.md` & `sonatoki-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/pyproject.toml` & `sonatoki-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sonatoki"
-version = "0.1.3"
+version = "0.1.4"
 description = "ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?"
 authors = [
     { name = "jan Kekan San (@gregdan3)", email = "gregory.danielson3@gmail.com" },
 ]
 dependencies = [
     "unidecode>=1.3.6",
     "regex>=2023.12.25",
```

### Comparing `sonatoki-0.1.3/src/sonatoki/Cleaners.py` & `sonatoki-0.1.4/src/sonatoki/Cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/src/sonatoki/Configs.py` & `sonatoki-0.1.4/src/sonatoki/Configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 # PDM
 from typing_extensions import NotRequired
 
 # LOCAL
 from sonatoki.Filters import (
     Filter,
     NimiPu,
-    Numerics,
+    Numeric,
     Syllabic,
     NimiLinku,
     NimiPuAle,
     Alphabetic,
     ProperName,
     Phonotactic,
+    Punctuation,
     NimiLinkuAle,
-    Punctuations,
 )
 from sonatoki.Scorers import Number, Scorer, PassFail, SoftScaling, SoftPassFail
 from sonatoki.Cleaners import Cleaner, ConsecutiveDuplicates
 from sonatoki.Tokenizers import Tokenizer, WordTokenizerTok
 from sonatoki.Preprocessors import (
     URLs,
     Preprocessor,
@@ -41,15 +41,15 @@
     scorer: Type[Scorer]
     passing_score: Number
 
 
 BaseConfig: IloConfig = {
     "preprocessors": [URLs],
     "cleaners": [ConsecutiveDuplicates],
-    "ignoring_filters": [Numerics, Punctuations],
+    "ignoring_filters": [Numeric, Punctuation],
     "scoring_filters": [],
     "scorer": PassFail,
     "passing_score": 0.8,
     "word_tokenizer": WordTokenizerTok,
 }
```

### Comparing `sonatoki-0.1.3/src/sonatoki/Filters.py` & `sonatoki-0.1.4/src/sonatoki/Filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     @override
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
         # Faster than regex version
         return set(token.lower()).issubset(ALPHABET_SET)
 
 
-class Numerics(Filter):
+class Numeric(Filter):
     """Determine if a given token is entirely numeric.
     Covers all numeric symbols in Unicode.
 
     This will fail to find numeric tokens such as "1.111" or "-42",
     but if used with the aggressive tokenizer designed for `tok`, these will be
     split into `["1", ".", "111"]` and `["-", "42"]` respectively. As such, the
     numeric tokens will be split from their punctuation."""
@@ -143,22 +143,22 @@
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, msg: str) -> bool:
         return msg.isnumeric()
 
 
-class Punctuations(RegexFilter):
+class Punctuation(RegexFilter):
     pattern = re.compile(r"[\p{Punctuation}\p{posix_punct}]+")
 
 
 __all__ = [
     "NimiPu",
     "NimiLinku",
     "NimiLinkuAle",
     "Phonotactic",
     "Syllabic",
     "Alphabetic",
     "ProperName",
-    "Punctuations",
-    "Numerics",
+    "Punctuation",
+    "Numeric",
 ]
```

### Comparing `sonatoki-0.1.3/src/sonatoki/Preprocessors.py` & `sonatoki-0.1.4/src/sonatoki/Preprocessors.py`

 * *Files 19% similar despite different names*

```diff
@@ -58,14 +58,21 @@
 
 class URLs(RegexPreprocessor):
     """Remove http(s) protocol URLs"""
 
     pattern = re.compile(r"https?:\/\/\S+")
 
 
+class Reference(RegexPreprocessor):
+    """Remove text contained in double brackets.
+    Often used to fetch articles on Wikipedia, or Magic the Gathering cards."""
+
+    pattern = re.compile(r"\[\[.+\]\]")
+
+
 class DiscordEmotes(RegexPreprocessor):
     """Remove text-formatted Discord emotes `<flags:name:id>`"""
 
     pattern = re.compile(r"<a?:[a-zA-Z0-9_]{2,}:[0-9]{2,}>")
 
 
 class DiscordMentions(RegexPreprocessor):
@@ -76,56 +83,80 @@
     pattern = re.compile(r"<#[0-9]{2,}>")
 
 
 class DiscordSpecial(RegexPreprocessor):
     pattern = re.compile(r"<id:[a-zA-Z0-9_]{4,}>")
 
 
+class AngleBracketObject(RegexPreprocessor):
+    """A generalized version of the Discord-specific angle bracket objects.
+    Removes any contiguous (not broken by whitespace) text in angle brackets."""
+
+    pattern = re.compile(r"<[^<>\s]+>")
+
+
 """
 The following classes are Containers.
 
 Containers are a special case of Ignorables, where an entire segment of an input
 may be removed and not counted toward the accepted or total number of tokens.
 
 Some users may prefer to use these so that they may quote third parties who 
 would likely be using a language other than Toki Pona.
 """
 
 
 class SingleQuotes(RegexPreprocessor):
-    pattern = re.compile(r"'[^']+'", flags=re.S)  # . matches newline
+    pattern = re.compile(r"'[^']+'", flags=re.DOTALL)
 
 
 class DoubleQuotes(RegexPreprocessor):
-    pattern = re.compile(r'"[^"]+"', flags=re.S)
+    pattern = re.compile(r'"[^"]+"', flags=re.DOTALL)
 
 
 class Backticks(RegexPreprocessor):
     """Remove paired backticks and their contents `like this`"""
 
-    pattern = re.compile(r"`[^`]+`", flags=re.S)
+    pattern = re.compile(r"`[^`]+`", flags=re.DOTALL)
 
 
 class Spoilers(RegexPreprocessor):
     """Remove paired double bars and their contents `||like this||`"""
 
-    pattern = re.compile(r"\|\|(?:(?!\|\|).)+\|\|", flags=re.S)
+    pattern = re.compile(r"\|\|(?:(?!\|\|).)+\|\|", flags=re.DOTALL)
 
 
 class ArrowQuote(RegexPreprocessor):
     """Remove lines beginning with `> `"""
 
     pattern = re.compile(r"^>\ .+$", re.MULTILINE)
 
 
+class AllQuotes(RegexPreprocessor):
+    pattern = re.compile(
+        "|".join(
+            [
+                SingleQuotes.pattern.pattern,
+                DoubleQuotes.pattern.pattern,
+                Backticks.pattern.pattern,
+                ArrowQuote.pattern.pattern,
+            ]
+        ),
+        flags=re.MULTILINE | re.DOTALL,
+    )
+
+
 __all__ = [
+    "AngleBracketObject",
     "DiscordChannels",
     "DiscordMentions",
     "DiscordSpecial",
     "DiscordEmotes",
     "SingleQuotes",
     "DoubleQuotes",
     "ArrowQuote",
+    "AllQuotes",
     "Backticks",
+    "Reference",
     "Spoilers",
     "URLs",
 ]
```

### Comparing `sonatoki-0.1.3/src/sonatoki/Scorers.py` & `sonatoki-0.1.4/src/sonatoki/Scorers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/src/sonatoki/Tokenizers.py` & `sonatoki-0.1.4/src/sonatoki/Tokenizers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/src/sonatoki/constants.py` & `sonatoki-0.1.4/src/sonatoki/constants.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/src/sonatoki/ilo.py` & `sonatoki-0.1.4/src/sonatoki/ilo.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/src/sonatoki/linku.json` & `sonatoki-0.1.4/src/sonatoki/linku.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/src/sonatoki/sandbox.json` & `sonatoki-0.1.4/src/sonatoki/sandbox.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/tests/test_cleaners.py` & `sonatoki-0.1.4/tests/test_cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/tests/test_filters.py` & `sonatoki-0.1.4/tests/test_filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import regex as re
 import hypothesis.strategies as st
 from hypothesis import HealthCheck, given, assume, example, settings
 
 # LOCAL
 from sonatoki.Filters import (
     NimiPu,
-    Numerics,
+    Numeric,
     Syllabic,
     NimiLinku,
     Alphabetic,
     ProperName,
     Phonotactic,
-    Punctuations,
+    Punctuation,
 )
 from sonatoki.Cleaners import ConsecutiveDuplicates
 from sonatoki.constants import NIMI_PU, NIMI_LINKU
 
 # FILESYSTEM
 from .test_utils import ALPHABETIC_RE, PROPER_NAME_RE
 
@@ -86,19 +86,19 @@
 # So I have to provide a different regex tha doesn't technically match
 @given(st.from_regex(r"[^\w\s]+", fullmatch=True))
 @example("⟨·⟩")
 @example("…")
 @example("「　」")
 @example(string.punctuation)
 @settings(suppress_health_check=[HealthCheck.filter_too_much])  # FIXME
-def test_Punctuations(s: str):
-    _ = assume(re.fullmatch(Punctuations.pattern.pattern, s))
-    res = Punctuations.filter(s)
+def test_Punctuation(s: str):
+    _ = assume(re.fullmatch(Punctuation.pattern.pattern, s))
+    res = Punctuation.filter(s)
     assert res, repr(s)
 
 
 @given(st.from_regex(r"\d+", fullmatch=True))
 @example("124125")
 @example("99990000")
 def test_Numeric(s: str):
-    res = Numerics.filter(s)
+    res = Numeric.filter(s)
     assert res, repr(s)
```

### Comparing `sonatoki-0.1.3/tests/test_ilo.py` & `sonatoki-0.1.4/tests/test_ilo.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/tests/test_tokenize.py` & `sonatoki-0.1.4/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/tests/test_utils.py` & `sonatoki-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/tests/tokenize_cases/tokenize_sentences_tok.yml` & `sonatoki-0.1.4/tests/tokenize_cases/tokenize_sentences_tok.yml`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/tests/tokenize_cases/tokenize_words_tok.yml` & `sonatoki-0.1.4/tests/tokenize_cases/tokenize_words_tok.yml`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.3/PKG-INFO` & `sonatoki-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonatoki
-Version: 0.1.3
+Version: 0.1.4
 Summary: ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?
 Author-Email: "jan Kekan San (@gregdan3)" <gregory.danielson3@gmail.com>
 License: AGPL-3.0-or-later
 Requires-Python: >=3.8
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: regex>=2023.12.25
 Requires-Dist: typing-extensions>=4.11.0
```

