# Comparing `tmp/correpy-0.4.1.tar.gz` & `tmp/correpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "correpy-0.4.1.tar", max compression
+gzip compressed data, was "correpy-0.5.0.tar", max compression
```

## Comparing `correpy-0.4.1.tar` & `correpy-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-04-26 20:11:58.518864 correpy-0.4.1/LICENSE
--rw-r--r--   0        0        0     5010 2024-04-26 20:11:58.518864 correpy-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/brokerage_note.py
--rw-r--r--   0        0        0     1405 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/security.py
--rw-r--r--   0        0        0      703 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/transaction.py
--rw-r--r--   0        0        0      596 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/enums.py
--rw-r--r--   0        0        0       64 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/__init__.py
--rw-r--r--   0        0        0    11260 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py
--rw-r--r--   0        0        0     2012 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/nuinvest.py
--rw-r--r--   0        0        0     5988 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/base_parser.py
--rw-r--r--   0        0        0      908 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/brokerage_note_section.py
--rw-r--r--   0        0        0      108 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/word_rectangle.py
--rw-r--r--   0        0        0      118 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/exceptions.py
--rw-r--r--   0        0        0     2567 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/fitz_parser.py
--rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/py.typed
--rw-r--r--   0        0        0     1123 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/utils.py
--rw-r--r--   0        0        0     2164 2024-04-26 20:11:58.518864 correpy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 correpy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 14:52:48.682944 correpy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5015 2024-05-09 14:52:48.682944 correpy-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/entities/__init__.py
+-rw-r--r--   0        0        0     2263 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/entities/brokerage_note.py
+-rw-r--r--   0        0        0     1405 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/entities/security.py
+-rw-r--r--   0        0        0      703 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/entities/transaction.py
+-rw-r--r--   0        0        0      596 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/enums.py
+-rw-r--r--   0        0        0       64 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/domain/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/b3_parser/__init__.py
+-rw-r--r--   0        0        0    11220 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py
+-rw-r--r--   0        0        0     5988 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/base_parser.py
+-rw-r--r--   0        0        0      908 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/brokerage_note_section.py
+-rw-r--r--   0        0        0       74 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/nuinvest_parser/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/nuinvest_parser/nuinvest.py
+-rw-r--r--   0        0        0     1298 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/parser_factory.py
+-rw-r--r--   0        0        0      108 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/brokerage_notes/word_rectangle.py
+-rw-r--r--   0        0        0      118 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/exceptions.py
+-rw-r--r--   0        0        0     2776 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/parsers/fitz_parser.py
+-rw-r--r--   0        0        0        0 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/py.typed
+-rw-r--r--   0        0        0     1123 2024-05-09 14:52:48.682944 correpy-0.5.0/correpy/utils.py
+-rw-r--r--   0        0        0     2164 2024-05-09 14:52:48.682944 correpy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 correpy-0.5.0/PKG-INFO
```

### Comparing `correpy-0.4.1/LICENSE` & `correpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/README.md` & `correpy-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 O conteúdo da sua nota de corretagem estará na variável `content` e é ela quem iremos usar para inicializar a nossa lib.
 Se a sua nota de corretagem possuir senha, você precisará informar também, caso contrário o parser nâo irá funcionar.
 
 ```python
 import io
 
-from correpy.parsers.brokerage_notes.b3_parser.b3_parser import B3Parser
+from correpy.parsers.brokerage_notes.parser_factory import ParserFactory
 
 with open('path to your pdf file', 'rb') as f:
     content = io.BytesIO(f.read())
     content.seek(0)
     
-    brokerage_notes = B3Parser(brokerage_note=content, password="password").parse_brokerage_note()
+    brokerage_notes = ParserFactory(brokerage_note=content, password="password").parse_brokerage_note()
 ```
 
 ### Resultado
 Depois de efetuar o parser da sua nota de corretagem, `correpy` irá retornar uma lista no formato abaixo. Os valores de cada campo serão explicados em seguida.
 
 ```python
 [
```

### Comparing `correpy-0.4.1/correpy/domain/entities/brokerage_note.py` & `correpy-0.5.0/correpy/domain/entities/brokerage_note.py`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/correpy/domain/entities/security.py` & `correpy-0.5.0/correpy/domain/entities/security.py`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/correpy/domain/entities/transaction.py` & `correpy-0.5.0/correpy/domain/entities/transaction.py`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/correpy/domain/enums.py` & `correpy-0.5.0/correpy/domain/enums.py`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py` & `correpy-0.5.0/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,31 +97,27 @@
             page=page, text=self.REFERENCE_NOTE_ID
         )
         try:
             ci_rect = self.fitz_parser.search_and_extract_rectangle_from_text(page=page, text=self.CI_TITLE)
         except ProblemParsingBrokerageNoteException:
             # From the initial text to 1/4 of the end of the page. It is this way because
             # the final text (CI_TITLE) is not always available (multiple pages).
-            ci_rect = fitz.Rect(
-                reference_id_rect.x0, reference_id_rect.y0,
-                page.rect.width, page.rect.height * 0.25
-            )
+            ci_rect = fitz.Rect(reference_id_rect.x0, reference_id_rect.y0, page.rect.width, page.rect.height * 0.25)
         brokerage_note_summary_section = self._build_brokerage_note_section_from_two_rectangles(
             first_rectangle=reference_id_rect, second_rectangle=ci_rect, page_number=page_number
         )
         current_reference_id = self.__get_reference_id_from_section(
             brokerage_note_section=brokerage_note_summary_section
         )
         current_reference_date = self.__get_reference_date_from_section(
             brokerage_note_section=brokerage_note_summary_section
         )
         note_key = (current_reference_id, current_reference_date)
         if (brokerage_note := self.brokerage_notes.get(note_key)) is None:
-            brokerage_note = BrokerageNote(reference_id=current_reference_id,
-                                           reference_date=current_reference_date)
+            brokerage_note = BrokerageNote(reference_id=current_reference_id, reference_date=current_reference_date)
             self.brokerage_notes[note_key] = brokerage_note
         return brokerage_note
 
     def set_brokerage_note_transactions(self) -> None:
         for page_document in self.fitz_parser.document:  # type:ignore[union-attr]
             page = page_document.get_textpage()
             page_number = page_document.number
@@ -141,16 +137,18 @@
                     rectangle_after_transactions = self.__build_full_width_rectangle(
                         y_axis_start=transactions_summary_title_rectangle.y0,  # pylint:disable=no-member
                         y_axis_end=transactions_summary_title_rectangle.y1,  # pylint:disable=no-member
                     )
                 except ProblemParsingBrokerageNoteException:
                     # From the text rectangle 'rectangle_before_transactions' to the end of the page.
                     rectangle_after_transactions = fitz.Rect(
-                        transactions_title_rectangle.x0, transactions_title_rectangle.y0,
-                        page.rect.width, page.rect.height
+                        transactions_title_rectangle.x0,
+                        transactions_title_rectangle.y0,
+                        page.rect.width,
+                        page.rect.height,
                     )
                 transactions_brokerage_note_section = self._build_brokerage_note_section_from_two_rectangles(
                     first_rectangle=rectangle_before_transactions,
                     second_rectangle=rectangle_after_transactions,
                     page_number=page_number,
                 )
                 transactions = self._get_transaction_lines_text_from_words(
```

### Comparing `correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/nuinvest.py` & `correpy-0.5.0/correpy/parsers/brokerage_notes/nuinvest_parser/nuinvest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 from typing import List
 
 from correpy.domain.enums import BrokerageNoteFeeType
 from correpy.parsers.brokerage_notes.b3_parser.b3_parser import B3Parser
 from correpy.parsers.brokerage_notes.brokerage_note_section import BrokerageNoteSection
 
 
-class NunInvestParser(B3Parser):
-	REFERENCE_NOTE_ID = "Número da nota"
-	CI_TITLE = "Valor/Ajuste D/C"
-	TRANSACTIONS_SECTION_TITLE = 'Nome do Cliente'
-	TRANSACTIONS_SUMMARY_TITLE = "Resumo dos Negócios"
-	first_column_transactions = "Mercado"
-	last_transaction_item = "BOVESPA"
-
-	financial_summary_header_mapper = {
-		"Taxa de Liquidação": BrokerageNoteFeeType.SETTLEMENT_FEE,
-		"Taxa de Registro": BrokerageNoteFeeType.REGISTRATION_FE,
-		"Taxa de Termo / Opções": BrokerageNoteFeeType.TERM_FEE,
-		"Taxa A.N.A.": BrokerageNoteFeeType.ANA_FEE,
-		"Emolumentos": BrokerageNoteFeeType.EMOLUMENTS,
-		"Taxa Operacional": BrokerageNoteFeeType.OPERATIONAL_FEE,
-		"Execução": BrokerageNoteFeeType.EXECUTION,
-		"Taxa de Custódia": BrokerageNoteFeeType.CUSTODY_FEE,
-		"Impostos": BrokerageNoteFeeType.TAXES,
-		"Outros": BrokerageNoteFeeType.OTHERS,
-	}
-
-	def __is_transactions_line(self, line_text: str) -> bool:
-		"""checks whether the row of data represents an asset transaction."""
-		return line_text[: len(self.last_transaction_item)] == self.last_transaction_item
-
-	def _get_transaction_lines_text_from_words(
-			self, transactions_brokerage_note_section: BrokerageNoteSection
-	) -> List[str]:
-		transaction_lines_text = []
-		can_include_transactions = False
-		for transaction_full_line in transactions_brokerage_note_section.text_by_lines:
-			if not self.__is_transactions_line(line_text=transaction_full_line):
-				can_include_transactions = False
-
-			if can_include_transactions:
-				logging.info("Parsed transaction line: %s", transaction_full_line)
-				transaction_lines_text.append(transaction_full_line)
+class NuInvestParser(B3Parser):
+    REFERENCE_NOTE_ID = "Número da nota"
+    CI_TITLE = "Valor/Ajuste D/C"
+    TRANSACTIONS_SECTION_TITLE = "Nome do Cliente"
+    TRANSACTIONS_SUMMARY_TITLE = "Resumo dos Negócios"
+    first_column_transactions = "Mercado"
+    last_transaction_item = "BOVESPA"
+
+    financial_summary_header_mapper = {
+        "Taxa de Liquidação": BrokerageNoteFeeType.SETTLEMENT_FEE,
+        "Taxa de Registro": BrokerageNoteFeeType.REGISTRATION_FE,
+        "Taxa de Termo / Opções": BrokerageNoteFeeType.TERM_FEE,
+        "Taxa A.N.A.": BrokerageNoteFeeType.ANA_FEE,
+        "Emolumentos": BrokerageNoteFeeType.EMOLUMENTS,
+        "Taxa Operacional": BrokerageNoteFeeType.OPERATIONAL_FEE,
+        "Execução": BrokerageNoteFeeType.EXECUTION,
+        "Taxa de Custódia": BrokerageNoteFeeType.CUSTODY_FEE,
+        "Impostos": BrokerageNoteFeeType.TAXES,
+        "Outros": BrokerageNoteFeeType.OTHERS,
+    }
+
+    def __is_transactions_line(self, line_text: str) -> bool:
+        """checks whether the row of data represents an asset transaction."""
+        return line_text[: len(self.last_transaction_item)] == self.last_transaction_item
+
+    def _get_transaction_lines_text_from_words(
+        self, transactions_brokerage_note_section: BrokerageNoteSection
+    ) -> List[str]:
+        transaction_lines_text = []
+        can_include_transactions = False
+        for transaction_full_line in transactions_brokerage_note_section.text_by_lines:
+            if not self.__is_transactions_line(line_text=transaction_full_line):
+                can_include_transactions = False
+
+            if can_include_transactions:
+                logging.info("Parsed transaction line: %s", transaction_full_line)
+                transaction_lines_text.append(transaction_full_line)
 
-			if self._is_transactions_header_line(line_text=transaction_full_line):
-				can_include_transactions = True
+            if self._is_transactions_header_line(line_text=transaction_full_line):
+                can_include_transactions = True
 
-		return transaction_lines_text
+        return transaction_lines_text
```

### Comparing `correpy-0.4.1/correpy/parsers/brokerage_notes/base_parser.py` & `correpy-0.5.0/correpy/parsers/brokerage_notes/base_parser.py`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/correpy/parsers/brokerage_notes/brokerage_note_section.py` & `correpy-0.5.0/correpy/parsers/brokerage_notes/brokerage_note_section.py`

 * *Files identical despite different names*

### Comparing `correpy-0.4.1/correpy/parsers/fitz_parser.py` & `correpy-0.5.0/correpy/parsers/fitz_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,7 +56,13 @@
             text_page = page.get_textpage()
             self.words.append(self.__parse_fitz_word_tuple_to_word_object(text_page))
 
     @staticmethod
     def __parse_fitz_word_tuple_to_word_object(text_page: fitz.TextPage) -> List[WordRectangle]:
         extracted_words = text_page.extractWORDS()
         return [WordRectangle(word[0], word[1], word[2], word[3], word[4]) for word in extracted_words]
+
+    def is_text_in_document(self, *, text: str) -> bool:
+        for page_document in self.document:
+            if page_document.get_textpage().search(text):
+                return True
+        return False
```

### Comparing `correpy-0.4.1/correpy/utils.py` & `correpy-0.5.0/correpy/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from datetime import date, datetime
 from decimal import Decimal
 
 NUMBER_STRUCTURE_REGEX = r"(?<![\d(\.|,)])(?:0,\d{2}|[1-9]\d{0,2}(?:\.\d{3})*,\d{2}|[1-9]\d{0,2})(?![\d(\.|,)])"
 AMOUNT_STRUCTURE_REGEX = r"(?<![\d.,])(?:0|[1-9]\d{0,2}(?:\.\d{3})*)(?![\d.,])"
 DATE_STRUCTURE_REGEX = r"[\d]{1,2}/[\d]{1,2}/[\d]{4}"
-ID_STRUCTURE_REGEX = r'^\D*(\d+)'
+ID_STRUCTURE_REGEX = r"^\D*(\d+)"
 
 
 def extract_value_from_line(*, line: str) -> Decimal:
     if total_value := re.findall(NUMBER_STRUCTURE_REGEX, line):
         return Decimal(total_value[-1].replace(".", "").replace(",", "."))
 
     return Decimal(0)
```

### Comparing `correpy-0.4.1/pyproject.toml` & `correpy-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "correpy"
-version = "0.4.1"
+version = "0.5.0"
 description = "CorrePy (Corretagem Python) é uma lib responsável por parsear notas de corretagem no padrão B3 (Sinacor) e retornar os dados no formato JSON."
 authors = ["Thiago  Salvatore <thiago.salvatore@gmail.com>"]
 license = "Apache License 2.0"
 keywords = ["corretagem", "parser", "b3", "nota de corretagem", "imposto de renda"]
 readme = "README.md"
 homepage = "https://github.com/thiagosalvatore/correpy"
 repository = "https://github.com/thiagosalvatore/correpy"
```

### Comparing `correpy-0.4.1/PKG-INFO` & `correpy-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: correpy
-Version: 0.4.1
+Version: 0.5.0
 Summary: CorrePy (Corretagem Python) é uma lib responsável por parsear notas de corretagem no padrão B3 (Sinacor) e retornar os dados no formato JSON.
 Home-page: https://github.com/thiagosalvatore/correpy
 License: Apache-2.0
 Keywords: corretagem,parser,b3,nota de corretagem,imposto de renda
 Author: Thiago  Salvatore
 Author-email: thiago.salvatore@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -44,21 +44,21 @@
 
 O conteúdo da sua nota de corretagem estará na variável `content` e é ela quem iremos usar para inicializar a nossa lib.
 Se a sua nota de corretagem possuir senha, você precisará informar também, caso contrário o parser nâo irá funcionar.
 
 ```python
 import io
 
-from correpy.parsers.brokerage_notes.b3_parser.b3_parser import B3Parser
+from correpy.parsers.brokerage_notes.parser_factory import ParserFactory
 
 with open('path to your pdf file', 'rb') as f:
     content = io.BytesIO(f.read())
     content.seek(0)
     
-    brokerage_notes = B3Parser(brokerage_note=content, password="password").parse_brokerage_note()
+    brokerage_notes = ParserFactory(brokerage_note=content, password="password").parse_brokerage_note()
 ```
 
 ### Resultado
 Depois de efetuar o parser da sua nota de corretagem, `correpy` irá retornar uma lista no formato abaixo. Os valores de cada campo serão explicados em seguida.
 
 ```python
 [
```

