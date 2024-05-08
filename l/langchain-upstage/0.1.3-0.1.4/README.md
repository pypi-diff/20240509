# Comparing `tmp/langchain_upstage-0.1.3.tar.gz` & `tmp/langchain_upstage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.3.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.4.tar", max compression
```

## Comparing `langchain_upstage-0.1.3.tar` & `langchain_upstage-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/LICENSE
--rw-r--r--   0        0        0      979 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/README.md
--rw-r--r--   0        0        0      567 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9097 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0     6430 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/layout_analysis.py
--rw-r--r--   0        0        0    12390 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/layout_analysis_parsers.py
--rw-r--r--   0        0        0        0 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/py.typed
--rw-r--r--   0        0        0     4323 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/tools/groundedness_check.py
--rw-r--r--   0        0        0     2727 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/LICENSE
+-rw-r--r--   0        0        0      979 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/README.md
+-rw-r--r--   0        0        0      567 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     3848 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9097 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0     7105 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/layout_analysis.py
+-rw-r--r--   0        0        0    12942 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/layout_analysis_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     4323 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/tools/groundedness_check.py
+-rw-r--r--   0        0        0     2732 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.4/PKG-INFO
```

### Comparing `langchain_upstage-0.1.3/LICENSE` & `langchain_upstage-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.3/README.md` & `langchain_upstage-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.3/langchain_upstage/__init__.py` & `langchain_upstage-0.1.4/langchain_upstage/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.3/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.4/langchain_upstage/chat_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 import openai
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.utils import (
     convert_to_secret_str,
     get_from_dict_or_env,
 )
-from langchain_openai import ChatOpenAI
+from langchain_openai.chat_models.base import BaseChatOpenAI
 
 
-class ChatUpstage(ChatOpenAI):
+class ChatUpstage(BaseChatOpenAI):
     """ChatUpstage chat model.
 
     To use, you should have the environment variable `UPSTAGE_API_KEY`
     set with your API key or pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
@@ -55,14 +55,24 @@
     model_name: str = Field(default="solar-1-mini-chat", alias="model")
     """Model name to use."""
     upstage_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     """Automatically inferred from env are `UPSTAGE_API_KEY` if not provided."""
     upstage_api_base: Optional[str] = Field(
         default="https://api.upstage.ai/v1/solar", alias="base_url"
     )
+    """Base URL path for API requests, leave blank if not using a proxy or service 
+    emulator."""
+    openai_api_key: Optional[SecretStr] = Field(default=None)
+    """openai api key is not supported for upstage. use `upstage_api_key` instead."""
+    openai_api_base: Optional[str] = Field(default=None)
+    """openai api base is not supported for upstage. use `upstage_api_base` instead."""
+    openai_organization: Optional[str] = Field(default=None)
+    """openai organization is not supported for upstage."""
+    tiktoken_model_name: Optional[str] = None
+    """tiktoken is not supported for upstage."""
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         if values["n"] < 1:
             raise ValueError("n must be at least 1.")
         if values["n"] > 1 and values["streaming"]:
```

### Comparing `langchain_upstage-0.1.3/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.4/langchain_upstage/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.3/langchain_upstage/layout_analysis.py` & `langchain_upstage-0.1.4/langchain_upstage/layout_analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from pathlib import Path
 from typing import Iterator, List, Literal, Optional, Union
 
 from langchain_core.document_loaders import BaseLoader, Blob
 from langchain_core.documents import Document
 
 from .layout_analysis_parsers import UpstageLayoutAnalysisParser
@@ -69,15 +70,15 @@
             f"  `{key}` as a named parameter."
         )
 
 
 class UpstageLayoutAnalysisLoader(BaseLoader):
     """Upstage Layout Analysis.
 
-    To use, you should have the environment variable `UPSTAGE_DOCUMENT_AI_API_KEY`
+    To use, you should have the environment variable `UPSTAGE_API_KEY`
     set with your API key or pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
 
             from langchain_upstage import UpstageLayoutAnalysis
 
@@ -86,44 +87,55 @@
                         file_path, split="page", output_type="text"
                      )
     """
 
     def __init__(
         self,
         file_path: Union[str, Path, List[str], List[Path]],
-        output_type: Union[OutputType, dict] = "text",
+        output_type: Union[OutputType, dict] = "html",
         split: SplitType = "none",
         api_key: Optional[str] = None,
         use_ocr: bool = False,
+        exclude: list = ["header", "footer"],
     ):
         """
         Initializes an instance of the Upstage document loader.
 
         Args:
             file_path (Union[str, Path, List[str], List[Path]): The path to the document
                                                                 to be loaded.
             output_type (Union[OutputType, dict], optional): The type of output to be
                                                              generated by the parser.
-                                                             Defaults to "text".
+                                                             Defaults to "html".
             split (SplitType, optional): The type of splitting to be applied.
                                          Defaults to "none" (no splitting).
             api_key (str, optional): The API key for accessing the Upstage API.
                                      Defaults to None, in which case it will be
                                      fetched from the environment variable
-                                     `UPSTAGE_DOCUMENT_AI_API_KEY`.
+                                     `UPSTAGE_API_KEY`.
             use_ocr (bool, optional): Extract text from images in the document.
                                       Defaults to False. (Use text info in PDF file)
+            exclude (list, optional): Exclude specific elements from
+                                                     the output.
+                                                     Defaults to ["header", "footer"].
         """
         self.file_path = file_path
         self.output_type = output_type
         self.split = split
+        if deprecated_key := os.environ.get("UPSTAGE_DOCUMENT_AI_API_KEY"):
+            warnings.warn(
+                "UPSTAGE_DOCUMENT_AI_API_KEY is deprecated."
+                "Please use UPSTAGE_API_KEY instead."
+            )
+
         self.api_key = get_from_param_or_env(
-            "UPSTAGE_DOCUMENT_AI_API_KEY", api_key, "UPSTAGE_DOCUMENT_AI_API_KEY"
+            "UPSTAGE_API_KEY", api_key, "UPSTAGE_API_KEY", deprecated_key
         )
         self.use_ocr = use_ocr
+        self.exclude = exclude
 
         validate_file_path(self.file_path)
         validate_api_key(self.api_key)
 
     def load(self) -> List[Document]:
         """
         Loads and parses the document using the UpstageLayoutAnalysisParser.
@@ -139,27 +151,29 @@
                 blob = Blob.from_path(file_path)
 
                 parser = UpstageLayoutAnalysisParser(
                     self.api_key,
                     split=self.split,
                     output_type=self.output_type,
                     use_ocr=self.use_ocr,
+                    exclude=self.exclude,
                 )
                 result.extend(list(parser.lazy_parse(blob, is_batch=True)))
 
             return result
 
         else:
             blob = Blob.from_path(self.file_path)
 
             parser = UpstageLayoutAnalysisParser(
                 self.api_key,
                 split=self.split,
                 output_type=self.output_type,
                 use_ocr=self.use_ocr,
+                exclude=self.exclude,
             )
             return list(parser.lazy_parse(blob, is_batch=True))
 
     def lazy_load(self) -> Iterator[Document]:
         """
         Lazily loads and parses the document using the UpstageLayoutAnalysisParser.
 
@@ -172,19 +186,21 @@
                 blob = Blob.from_path(file_path)
 
                 parser = UpstageLayoutAnalysisParser(
                     self.api_key,
                     split=self.split,
                     output_type=self.output_type,
                     use_ocr=self.use_ocr,
+                    exclude=self.exclude,
                 )
                 yield from parser.lazy_parse(blob, is_batch=True)
         else:
             blob = Blob.from_path(self.file_path)
 
             parser = UpstageLayoutAnalysisParser(
                 self.api_key,
                 split=self.split,
                 output_type=self.output_type,
                 use_ocr=self.use_ocr,
+                exclude=self.exclude,
             )
             yield from parser.lazy_parse(blob)
```

### Comparing `langchain_upstage-0.1.3/langchain_upstage/layout_analysis_parsers.py` & `langchain_upstage-0.1.4/langchain_upstage/layout_analysis_parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import json
 import os
+import warnings
 from typing import Dict, Iterator, List, Literal, Optional, Union
 
 import fitz  # type: ignore
 import requests
 from fitz import Document as fitzDocument
 from langchain_core.document_loaders import BaseBlobParser, Blob
 from langchain_core.documents import Document
@@ -99,59 +100,68 @@
             f"  `{key}` as a named parameter."
         )
 
 
 class UpstageLayoutAnalysisParser(BaseBlobParser):
     """Upstage Layout Analysis Parser.
 
-    To use, you should have the environment variable `UPSTAGE_DOCUMENT_AI_API_KEY`
+    To use, you should have the environment variable `UPSTAGE_API_KEY`
     set with your API key or pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
 
             from langchain_upstage import UpstageLayoutAnalysisParser
 
             loader = UpstageLayoutAnalysisParser(split="page", output_type="text")
     """
 
     def __init__(
         self,
         api_key: Optional[str] = None,
-        output_type: Union[OutputType, dict] = "text",
+        output_type: Union[OutputType, dict] = "html",
         split: SplitType = "none",
         use_ocr: bool = False,
+        exclude: list = [],
     ):
         """
         Initializes an instance of the Upstage class.
 
         Args:
             api_key (str, optional): The API key for accessing the Upstage API.
                                      Defaults to None, in which case it will be
                                      fetched from the environment variable
-                                     `UPSTAGE_DOCUMENT_AI_API_KEY`.
+                                     `UPSTAGE_API_KEY`.
             output_type (Union[OutputType, dict], optional): The type of output to be
                                                              generated by the parser.
-                                                             Defaults to "text".
+                                                             Defaults to "html".
             split (SplitType, optional): The type of splitting to be applied.
                                          Defaults to "none" (no splitting).
             use_ocr (bool, optional): Extract text from images in the document.
                                       Defaults to False. (Use text info in PDF file)
+            exclude (list, optional): Exclude specific elements from the output.
+                                      Defaults to [] (all included).
         """
+        if deprecated_key := os.environ.get("UPSTAGE_DOCUMENT_AI_API_KEY"):
+            warnings.warn(
+                "UPSTAGE_DOCUMENT_AI_API_KEY is deprecated."
+                "Please use UPSTAGE_API_KEY instead."
+            )
         self.api_key = get_from_param_or_env(
-            "UPSTAGE_DOCUMENT_AI_API_KEY", api_key, "UPSTAGE_DOCUMENT_AI_API_KEY"
+            "UPSTAGE_API_KEY", api_key, "UPSTAGE_API_KEY", deprecated_key
         )
 
         self.output_type = output_type
         self.split = split
         self.use_ocr = use_ocr
+        self.exclude = exclude
 
         validate_api_key(self.api_key)
 
-    def _get_response(self, files: Dict) -> Dict:
+    def _get_response(self, files: Dict) -> List:
         """
         Sends a POST request to the API endpoint with the provided files and
         returns the response.
 
         Args:
             files (dict): A dictionary containing the files to be sent in the request.
 
@@ -161,36 +171,40 @@
         Raises:
             ValueError: If there is an error in the API call.
         """
         try:
             headers = {"Authorization": f"Bearer {self.api_key}"}
             options = {"ocr": self.use_ocr}
             response = requests.post(
-                LAYOUT_ANALYSIS_URL, headers=headers, files=files, json=options
+                LAYOUT_ANALYSIS_URL, headers=headers, files=files, data=options
             )
             response.raise_for_status()
 
-            result = response.json()
+            result = response.json().get("elements", [])
 
         except requests.RequestException as req_err:
             # Handle any request-related exceptions
             print(f"Request Exception: {req_err}")
         except json.JSONDecodeError as json_err:
             # Handle JSON decode errors
             print(f"JSON Decode Error: {json_err}")
             raise ValueError(f"Failed to decode JSON response: {json_err}")
 
-        return result
+        elements = [
+            element for element in result if element["category"] not in self.exclude
+        ]
+
+        return elements
 
     def _split_and_request(
         self,
         full_docs: fitzDocument,
         start_page: int,
         num_pages: int = DEFAULT_NUMBER_OF_PAGE,
-    ) -> Dict:
+    ) -> List:
         """
         Splits the full pdf document into partial pages and sends a request to the
         server.
 
         Args:
             full_docs (str): The full document to be split and requested.
             start_page (int): The starting page number for splitting the document.
@@ -231,20 +245,20 @@
                 "page": elements["page"],
                 "id": elements["id"],
                 "type": self.output_type,
                 "split": self.split,
             },
         )
 
-    def _page_document(self, elements: Dict) -> List[Document]:
+    def _page_document(self, elements: List) -> List[Document]:
         """
         Combines elements with the same page number into a single Document object.
 
         Args:
-            elements (List[Dict]): A list of elements containing page numbers.
+            elements (List): A list of elements containing page numbers.
 
         Returns:
             List[Document]: A list of Document objects, each representing a page
                             with its content and metadata.
         """
         _docs = []
         pages = sorted(set(map(lambda x: x["page"], elements)))
@@ -302,25 +316,30 @@
                 result = ""
                 start_page = 0
                 num_pages = DEFAULT_NUMBER_OF_PAGE
                 for _ in range(number_of_pages):
                     if start_page >= number_of_pages:
                         break
 
-                    response = self._split_and_request(full_docs, start_page, num_pages)
-                    result += parse_output(response, self.output_type)
+                    elements = self._split_and_request(full_docs, start_page, num_pages)
+                    for element in elements:
+                        result += parse_output(element, self.output_type)
 
                     start_page += num_pages
 
             else:
                 if not blob.path:
                     raise ValueError("Blob path is required for non-PDF files.")
+
+                result = ""
                 with open(blob.path, "rb") as f:
-                    response = self._get_response({"document": f})
-                    result = parse_output(response, self.output_type)
+                    elements = self._get_response({"document": f})
+
+                for element in elements:
+                    result += parse_output(element, self.output_type)
 
             yield Document(
                 page_content=result,
                 metadata={
                     "total_pages": number_of_pages,
                     "type": self.output_type,
                     "split": self.split,
@@ -330,46 +349,43 @@
         elif self.split == "element":
             if full_docs.is_pdf:
                 start_page = 0
                 for _ in range(number_of_pages):
                     if start_page >= number_of_pages:
                         break
 
-                    response = self._split_and_request(full_docs, start_page, num_pages)
-                    for element in response["elements"]:
+                    elements = self._split_and_request(full_docs, start_page, num_pages)
+                    for element in elements:
                         yield self._element_document(element)
 
                     start_page += num_pages
 
             else:
                 if not blob.path:
                     raise ValueError("Blob path is required for non-PDF files.")
                 with open(blob.path, "rb") as f:
-                    response = self._get_response({"document": f})
+                    elements = self._get_response({"document": f})
 
-                for element in response["elements"]:
+                for element in elements:
                     yield self._element_document(element)
 
         elif self.split == "page":
             if full_docs.is_pdf:
                 start_page = 0
                 for _ in range(number_of_pages):
                     if start_page >= number_of_pages:
                         break
 
-                    response = self._split_and_request(full_docs, start_page, num_pages)
-                    elements = response["elements"]
+                    elements = self._split_and_request(full_docs, start_page, num_pages)
                     yield from self._page_document(elements)
 
                     start_page += num_pages
             else:
                 if not blob.path:
                     raise ValueError("Blob path is required for non-PDF files.")
                 with open(blob.path, "rb") as f:
-                    response = self._get_response({"document": f})
-
-                elements = response["elements"]
+                    elements = self._get_response({"document": f})
 
                 yield from self._page_document(elements)
 
         else:
             raise ValueError(f"Invalid split type: {self.split}")
```

### Comparing `langchain_upstage-0.1.3/langchain_upstage/tools/groundedness_check.py` & `langchain_upstage-0.1.4/langchain_upstage/tools/groundedness_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,12 +106,12 @@
             [HumanMessage(context), AIMessage(answer)], stream=False
         )
         return str(response.content)
 
 
 @deprecated(
     since="0.1.3",
-    removal="0.2.0",
+    removal="0.3.0",
     alternative_import="langchain_upstage.UpstageGroundednessCheck",
 )
 class GroundednessCheck(UpstageGroundednessCheck):
     pass
```

### Comparing `langchain_upstage-0.1.3/pyproject.toml` & `langchain_upstage-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-upstage"
-version = "0.1.3"
+version = "0.1.4"
 description = "An integration package connecting Upstage and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -57,15 +57,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
 
 [tool.mypy]
```

### Comparing `langchain_upstage-0.1.3/PKG-INFO` & `langchain_upstage-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.3
+Version: 0.1.4
 Summary: An integration package connecting Upstage and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

