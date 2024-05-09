# Comparing `tmp/kci_confluence_cli-0.1.0.tar.gz` & `tmp/kci_confluence_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kci_confluence_cli-0.1.0.tar", max compression
+gzip compressed data, was "kci_confluence_cli-0.2.0.tar", max compression
```

## Comparing `kci_confluence_cli-0.1.0.tar` & `kci_confluence_cli-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2029 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/README.md
--rw-r--r--   0        0        0       71 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/__init__.py
--rw-r--r--   0        0        0     1656 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/__main__.py
--rw-r--r--   0        0        0      131 2024-03-03 06:33:13.769642 kci_confluence_cli-0.1.0/confluence/__version__.py
--rw-r--r--   0        0        0        0 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/attachment/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/attachment/create_attachment.py
--rw-r--r--   0        0        0     3800 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/attachment/delete_attachment.py
--rw-r--r--   0        0        0     1999 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/attachment/get_attachment.py
--rw-r--r--   0        0        0     1004 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/attachment/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/common/__init__.py
--rw-r--r--   0        0        0     6425 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/common/api.py
--rw-r--r--   0        0        0     9554 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/common/cli.py
--rw-r--r--   0        0        0     2425 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/common/utils.py
--rw-r--r--   0        0        0        0 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/content/__init__.py
--rw-r--r--   0        0        0     1396 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/content/get_content_by_id.py
--rw-r--r--   0        0        0      824 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/content/subcommand.py
--rw-r--r--   0        0        0      462 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/data/logging.yaml
--rw-r--r--   0        0        0        0 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/local/__init__.py
--rw-r--r--   0        0        0     3575 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/local/convert_html_to_xml.py
--rw-r--r--   0        0        0      843 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/local/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/page/__init__.py
--rw-r--r--   0        0        0     1664 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/page/get_page_body.py
--rw-r--r--   0        0        0      895 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/page/subcommand.py
--rw-r--r--   0        0        0     1822 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/page/update_page.py
--rw-r--r--   0        0        0        0 2024-03-03 06:33:01.093713 kci_confluence_cli-0.1.0/confluence/py.typed
--rw-r--r--   0        0        0     4294 2024-03-03 06:33:13.769642 kci_confluence_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 kci_confluence_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1744 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/README.md
+-rw-r--r--   0        0        0       71 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/__init__.py
+-rw-r--r--   0        0        0     1672 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/__main__.py
+-rw-r--r--   0        0        0      131 2024-05-09 06:19:22.324425 kci_confluence_cli-0.2.0/confluence/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/__init__.py
+-rw-r--r--   0        0        0     4938 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/create_attachment.py
+-rw-r--r--   0        0        0     3816 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/delete_attachment.py
+-rw-r--r--   0        0        0     2015 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/get_attachment.py
+-rw-r--r--   0        0        0     1020 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/__init__.py
+-rw-r--r--   0        0        0     6889 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/api.py
+-rw-r--r--   0        0        0     9560 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/cli.py
+-rw-r--r--   0        0        0     2441 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/content/__init__.py
+-rw-r--r--   0        0        0     1412 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/content/get_content_by_id.py
+-rw-r--r--   0        0        0      840 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/content/subcommand.py
+-rw-r--r--   0        0        0      462 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/data/logging.yaml
+-rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/local/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/local/convert_html_to_xml.py
+-rw-r--r--   0        0        0      859 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/local/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/get_page_body.py
+-rw-r--r--   0        0        0      907 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/subcommand.py
+-rw-r--r--   0        0        0     1838 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/update_page.py
+-rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/py.typed
+-rw-r--r--   0        0        0     4057 2024-05-09 06:19:22.320425 kci_confluence_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 kci_confluence_cli-0.2.0/PKG-INFO
```

### Comparing `kci_confluence_cli-0.1.0/README.md` & `kci_confluence_cli-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # confluence-cli
 来栖川電算が利用しているConfluence v6.15.7を操作するためのCLIです。
 
+
+[![Build Status](https://app.travis-ci.com/kurusugawa-computer/confluence-cli.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/confluence-cli)
+[![PyPI version](https://badge.fury.io/py/kci-confluence-cli.svg)](https://badge.fury.io/py/kci-confluence-cli)
+[![Python Versions](https://img.shields.io/pypi/pyversions/kci-confluence-cli.svg)](https://pypi.org/project/kci-confluence-cli/)
+[![Documentation Status](https://readthedocs.org/projects/confluence-cli/badge/?version=latest)](https://confluence-cli.readthedocs.io/ja/latest/?badge=latest)
+
 # Requirements
 Python 3.9+
 
 # Install
 
 ```
 $ pip install kci-confluence-cli
@@ -29,30 +35,9 @@
 
 上記の方法で指定されない場合は、標準入力から入力できます。
 
 来栖川電算のConfluneceにアクセスする場合は、`https://kurusugawa.jp/confluence`を指定してください。
 
 
 # Command Reference
-### attachment get
-添付ファイル情報の取得
-
-
-### attachment create
-添付ファイルの作成
-
-
-### attachment delete
-添付ファイルを削除します。
-
-※添付ファイルをゴミ箱から完全に削除すると、ページを更新できない場合があります。その場合は、一時的に前のバージョンに戻せば、ページを更新できるようになります。
-https://qiita.com/yuji38kwmt/items/c88f039e02b8508926e6
-
-
-### attachment get
-コンテンツ（ページやブログ、添付ファイルなど）の情報を取得します。
+https://confluence-cli.readthedocs.io/ja/latest/command_reference/index.html を参照してください。
 
-### local convert_html
-HTMLをConfluence用のXMLに変換します。
-Google DocsのページをConfluenceに移行するときなどに利用できます。
-具体的な手順は以下を参照してください。
-https://github.com/kurusugawa-computer/confluence-cli/wiki/Google-Docs%E3%82%92Confluence%E3%81%AB%E7%A7%BB%E8%A1%8C%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95
```

### Comparing `kci_confluence_cli-0.1.0/confluence/__main__.py` & `kci_confluence_cli-0.2.0/confluence/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     confluence.attachment.subcommand.add_parser(subparsers)
     confluence.content.subcommand.add_parser(subparsers)
     confluence.page.subcommand.add_parser(subparsers)
     confluence.local.subcommand.add_parser(subparsers)
     return parser
 
 
-def main(arguments: Optional[Sequence[str]] = None):
+def main(arguments: Optional[Sequence[str]] = None):  # noqa: ANN201
     parser = create_parser()
     if arguments is None:
         args = parser.parse_args()
     else:
         args = parser.parse_args(arguments)
 
     if hasattr(args, "subcommand_func"):
```

### Comparing `kci_confluence_cli-0.1.0/confluence/attachment/create_attachment.py` & `kci_confluence_cli-0.2.0/confluence/attachment/create_attachment.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,85 +13,91 @@
 
 
 def create_attachments_from_file_list(
     api: Api, content_id: str, query_params: dict[str, Any], files: list[Path], filename_pattern: None | str, mime_type: None | str
 ) -> None:
     logger.info(f"{len(files)}件のファイルをアップロードします。")
     success_count = 0
-    total_count = 0
-    for file in files:
+    for index, file in enumerate(files):
         if not file.is_file():
             logger.warning(f"'{file}'はファイルでないので、アップロードしません。")
             continue
 
         if filename_pattern is not None and not file.glob(filename_pattern):
             continue
 
         try:
-            total_count += 1
             api.create_attachment(content_id, file, query_params=query_params, mime_type=mime_type)
-            logger.debug(f"{total_count+1}件目: '{file}'をアップロードしました。")
+            logger.debug(f"{index+1}件目: '{file}'をアップロードしました。")
+            if (index + 1) % 10 == 0:
+                logger.info(f"{index+1}件目のファイルのアップロードが完了しました。")
+
         except Exception:
             logger.warning(f"'{file}'のアップロードに失敗しました。", exc_info=True)
             continue
 
         logger.debug(f"'{file}'をアップロードしました。")
         success_count += 1
 
-    logger.info(f"{success_count}/{total_count} 件のファイルをアップロードしました。")
+    logger.info(f"{success_count}/{len(files)} 件のファイルをアップロードしました。")
 
 
 def create_attachments_from_directory(
     api: Api, content_id: str, query_params: dict[str, Any], directory: Path, filename_pattern: None | str, mime_type: None | str
 ) -> None:
     success_count = 0
-    total_count = 0
     if not directory.is_dir():
         logger.error(f"'{directory}'はディレクトリでないので、終了します。")
         return
 
-    logger.info(f"ディレクトリ'{directory}'内のファイルをアップロードします。")
-
+    files = []
     for file in directory.iterdir():
         if not file.is_file():
             continue
         if filename_pattern is not None and not file.glob(filename_pattern):
             continue
+        files.append(file)
+
+    logger.info(f"ディレクトリ'{directory}'内のファイル{len(files)}件をアップロードします。")
+
+    for index, file in enumerate(files):
         try:
-            total_count += 1
             api.create_attachment(content_id, file, query_params=query_params, mime_type=mime_type)
-            logger.debug(f"{total_count}件目: '{file}'をアップロードしました。")
+            logger.debug(f"{index+1}件目: '{file}'をアップロードしました。")
+            if (index + 1) % 10 == 0:
+                logger.info(f"{index+1}件目のファイルのアップロードが完了しました。")
+
         except Exception:
             logger.warning(f"'{file}'のアップロードに失敗しました。", exc_info=True)
             continue
         success_count += 1
 
-    logger.info(f"{success_count}/{total_count}件のファイルをアップロードしました。")
+    logger.info(f"{success_count}/{len(files)}件のファイルをアップロードしました。")
 
 
 def main(args: argparse.Namespace) -> None:
     api = create_api_instance(args)
     content_id = args.content_id
     query_params = {"allowDuplicated": args.allow_duplicated}
     if args.file is not None:
         create_attachments_from_file_list(api, content_id, query_params, args.file, filename_pattern=args.filename_pattern, mime_type=args.mime_type)
     elif args.dir is not None:
         create_attachments_from_directory(api, content_id, query_params, args.dir, filename_pattern=args.filename_pattern, mime_type=args.mime_type)
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-c", "--content_id", required=True, help="ファイルのアップロード先であるページのcontent_id")
 
     file_group = parser.add_mutually_exclusive_group(required=True)
     file_group.add_argument("--file", type=Path, nargs="+", help="アップロードするファイル")
     file_group.add_argument("--dir", type=Path, help="アップロードするディレクトリ")
 
     parser.add_argument("--mime_type", type=str, help="ファイル名からMIMEタイプが判別できないときに、この値を添付ファイルのMIMEタイプとします。")
 
-    parser.add_argument("--allow_duplicated", action="store_true", help="指定した場合は、すでに同じファイルが存在しても上書きします。")
+    parser.add_argument("--allow_duplicated", action="store_true", help="指定した場合は、アップロード先にすでに同じファイルが存在している場合に上書きます。指定しない場合は、400 Errorが発生します。")
 
     parser.add_argument("--filename_pattern", help="glob形式のパターンに一致するファイル名だけアップロードします。(ex) '*.png'")
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: argparse._SubParsersAction | None = None) -> argparse.ArgumentParser:
     subcommand_name = "create"
```

### Comparing `kci_confluence_cli-0.1.0/confluence/attachment/delete_attachment.py` & `kci_confluence_cli-0.2.0/confluence/attachment/delete_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         except Exception:
             logger.warning(f"{index+1}件目: id='{attachment_id}', title='{attachment_title}'の削除に失敗しました。", exc_info=True)
             continue
 
     logger.info(f"{success_count}/{len(results)} 件の添付ファイルを削除しました。")
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-c", "--content_id", required=True, help="削除したい添付ファイルが存在するページのcontent_id")
 
     parser.add_argument("--filename", help="filter parameter to return only the Attachment with the matching file name")
     parser.add_argument("--media_type", help="filter parameter to return only Attachments with a matching Media-Type")
     parser.add_argument("--purge", action="store_true", help="指定すると、ゴミ箱からも完全に削除します。復元できません。")
     parser.set_defaults(subcommand_func=main)
```

### Comparing `kci_confluence_cli-0.1.0/confluence/attachment/get_attachment.py` & `kci_confluence_cli-0.2.0/confluence/attachment/get_attachment.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         if result["size"] < limit:
             break
         start = start + limit
 
     print_json(results, is_pretty=True, output=args.output)
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-c", "--content_id", required=True, help="取得した添付ファイルが存在するページのcontent_id")
 
     parser.add_argument("--filename", help="filter parameter to return only the Attachment with the matching file name")
     parser.add_argument("--media_type", help="filter parameter to return only Attachments with a matching Media-Type")
 
     parser.add_argument("--expand", nargs="+", help="取得したい情報のプロパティ。指定できる値は出力結果の`_expandable`を参照してください。")
```

### Comparing `kci_confluence_cli-0.1.0/confluence/attachment/subcommand.py` & `kci_confluence_cli-0.2.0/confluence/attachment/subcommand.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import confluence
 import confluence.attachment.create_attachment
 import confluence.attachment.delete_attachment
 import confluence.attachment.get_attachment
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     confluence.attachment.create_attachment.add_parser(subparsers)
     confluence.attachment.delete_attachment.add_parser(subparsers)
     confluence.attachment.get_attachment.add_parser(subparsers)
```

### Comparing `kci_confluence_cli-0.1.0/confluence/common/api.py` & `kci_confluence_cli-0.2.0/confluence/common/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import copy
 import logging
 import mimetypes
 import time
 from pathlib import Path
 from typing import Any, Optional
 
 from requests_toolbelt import sessions
@@ -31,14 +32,26 @@
         self.base_url = base_url
         self.session = sessions.BaseUrlSession(base_url=base_url + "/rest/api/")
         self.session.auth = (username, password)
 
         self.delay_second = delay_second
         self._previous_timestamp: float = 0
 
+    @staticmethod
+    def mask_sensitive_info_of_headers(headers: dict[str, str] | None) -> dict[str, str] | None:
+        """HTTP headerのセンシティブな情報を`***`でマスクする"""
+        if headers is None:
+            return None
+        new_headers = copy.deepcopy(headers)
+
+        if "Authorization" in new_headers:
+            new_headers["Authorization"] = "***"
+
+        return new_headers
+
     def _request(
         self,
         http_method: str,
         url: str,
         *,
         headers: Optional[dict[str, Any]] = None,
         params: Optional[QueryParams] = None,
@@ -73,15 +86,15 @@
             "Sent a request :: %s",
             {
                 "requests": {
                     "http_method": http_method,
                     "url": url,
                     "query_params": params,
                     "request_body_json": data,
-                    "headers": response.request.headers,
+                    "headers": self.mask_sensitive_info_of_headers(headers),
                 },
                 "response": {
                     "status_code": response.status_code,
                     "content_length": len(response.content),
                 },
             },
         )
@@ -143,15 +156,15 @@
         https://docs.atlassian.com/ConfluenceServer/rest/6.15.7/#api/content-delete
 
         Notes:
             クエリパラーメタ`status`に`trashed`を指定すると400エラーが発生した。
         """
         self._request("delete", f"content/{content_id}", params=query_params)
 
-    def get_content_history(self, content_id: str, *, query_params: Optional[QueryParams] = None):
+    def get_content_history(self, content_id: str, *, query_params: Optional[QueryParams] = None):  # noqa: ANN201
         """Returns the history of a particular piece of content
 
         https://docs.atlassian.com/ConfluenceServer/rest/6.15.7/#api/content-getHistory
         """
         return self._request("get", f"content/{content_id}/history", params=query_params).json()
 
     def search_content(self, *, query_params: Optional[QueryParams] = None) -> dict[str, Any]:
```

### Comparing `kci_confluence_cli-0.1.0/confluence/common/cli.py` & `kci_confluence_cli-0.2.0/confluence/common/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Command Line Interfaceの共通部分
 """
+
 from __future__ import annotations
 
 import argparse
 import getpass
 import logging
 import os
 from typing import Optional
@@ -18,15 +19,15 @@
 COMMAND_LINE_ERROR_STATUS_CODE = 2
 
 
 class PrettyHelpFormatter(argparse.RawTextHelpFormatter, argparse.ArgumentDefaultsHelpFormatter):
     def _format_action(self, action: argparse.Action) -> str:
         return super()._format_action(action) + "\n"
 
-    def _get_help_string(self, action):  # noqa: ANN001
+    def _get_help_string(self, action) -> str:  # noqa: ANN001
         """引数説明用のメッセージを生成する。
         不要なデフォルト値（--debug や オプショナルな引数）を表示させないようにする.
         `argparse.ArgumentDefaultsHelpFormatter._get_help_string` をオーバライドしている。
 
         Args:
             action ([type]): [description]
 
@@ -205,15 +206,15 @@
         while value == "":
             value = input("Confluenceのユーザー名を入力してください。 : ")
         return value
 
     def get_confluence_base_url_from_stdin() -> str:
         value = ""
         while value == "":
-            value = input("ConfluenceのURLを入力してください。(例) `https://kurusugawa.jp/confluence` : ")
+            value = input("ConfluenceのURLを入力してください。(例) https://kurusugawa.jp/confluence : ")
         return value
 
     def format_url(url: str) -> str:
         url = url.strip()
         if url.endswith("/"):
             url = url[:-1]
         return url
```

### Comparing `kci_confluence_cli-0.1.0/confluence/common/utils.py` & `kci_confluence_cli-0.2.0/confluence/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     """
     if is_pretty:
         output_string(json.dumps(target, indent=2, ensure_ascii=False), output)
     else:
         output_string(json.dumps(target, ensure_ascii=False), output)
 
 
-def set_logger(is_debug_mode: bool = False):
+def set_logger(is_debug_mode: bool = False):  # noqa: ANN201
     """
     デフォルトのロガーを設定する。パッケージ内のlogging.yamlを読み込む。
     """
     data = pkgutil.get_data("confluence", "data/logging.yaml")
     if data is None:
         raise RuntimeError("confluence/data/logging.yaml の読み込みに失敗しました。")
```

### Comparing `kci_confluence_cli-0.1.0/confluence/content/get_content_by_id.py` & `kci_confluence_cli-0.2.0/confluence/content/get_content_by_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     api = create_api_instance(args)
     content_id = args.content_id
     expand = ",".join(args.expand) if args.expand else None
     result = api.get_content_by_id(content_id, query_params={"status": "any", "expand": expand})
     print_json(result, is_pretty=True, output=args.output)
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-c", "--content_id", required=True, help="取得対象のコンテンツのID")
     parser.add_argument("--expand", nargs="+", help="取得したい情報のプロパティ。指定できる値は出力結果の`_expandable`を参照してください。")
     parser.add_argument("-o", "--output", type=Path, help="出力先")
 
     parser.set_defaults(subcommand_func=main)
```

### Comparing `kci_confluence_cli-0.1.0/confluence/content/subcommand.py` & `kci_confluence_cli-0.2.0/confluence/content/subcommand.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 from typing import Optional
 
 import confluence
 import confluence.content.get_content_by_id
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     confluence.content.get_content_by_id.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
```

### Comparing `kci_confluence_cli-0.1.0/confluence/local/convert_html_to_xml.py` & `kci_confluence_cli-0.2.0/confluence/local/convert_html_to_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     output_xml_file.write_text(html_data, encoding="utf-8")
 
 
 def main(args: argparse.Namespace) -> None:
     convert(args.input_html, args.output_xml)
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "input_html",
         type=Path,
         help="変換元の入力用HTML",
     )
     parser.add_argument(
         "output_xml",
```

### Comparing `kci_confluence_cli-0.1.0/confluence/local/subcommand.py` & `kci_confluence_cli-0.2.0/confluence/local/subcommand.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 
 import confluence
 import confluence.attachment.get_attachment
 import confluence.local.convert_html_to_xml
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     confluence.local.convert_html_to_xml.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
```

### Comparing `kci_confluence_cli-0.1.0/confluence/page/get_page_body.py` & `kci_confluence_cli-0.2.0/confluence/page/get_page_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     content_id = args.content_id
 
     result = api.get_content_by_id(content_id, query_params={"expand": expand})
 
     output_string(result["body"][representation]["value"], output=args.output)
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-c", "--content_id", required=True, help="取得対象のコンテンツのID")
     parser.add_argument(
         "--representation", choices=[e.value for e in BodyRepresentation], default=BodyRepresentation.STORAGE.value, help="ページの中身の表現方法"
     )
     parser.add_argument("-o", "--output", type=Path, help="出力先")
 
     parser.set_defaults(subcommand_func=main)
```

### Comparing `kci_confluence_cli-0.1.0/confluence/page/subcommand.py` & `kci_confluence_cli-0.2.0/confluence/page/subcommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from typing import Optional
 
 import confluence
 import confluence.page.get_page_body
 import confluence.page.update_page
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     confluence.page.get_page_body.add_parser(subparsers)
-    # 動かないので一旦コメントアウトする
-    confluence.page.update_page.add_parser(subparsers)
+    # 動かないのでコメントアウトする
+    # confluence.page.update_page.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "page"
     subcommand_help = "ページに関するサブコマンド"
 
     parser = confluence.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
```

### Comparing `kci_confluence_cli-0.1.0/confluence/page/update_page.py` & `kci_confluence_cli-0.2.0/confluence/page/update_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "space": {"key": old_page["space"]["key"]},
         "body": {"storage": {"value": xml_text, "representation": "storage"}},
     }
     result = api.update_content(content_id, request_body=request_body)
     print_json(result, is_pretty=True, output=None)
 
 
-def add_arguments_to_parser(parser: argparse.ArgumentParser):
+def add_arguments_to_parser(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-c", "--content_id", required=True, help="取得対象のコンテンツのID")
     parser.add_argument(
         "--xml_file", required=True, type=Path, help="storageフォーマットで記載されたXMLファイルのパス。このファイルの内容でページが更新されます。"
     )
 
     parser.set_defaults(subcommand_func=main)
```

### Comparing `kci_confluence_cli-0.1.0/pyproject.toml` & `kci_confluence_cli-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kci-confluence-cli"
-version = "0.1.0"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
+version = "0.2.0"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "来栖川電算が利用しているConfluence v6.15.7を操作するためのCLIです。"
 authors = ["Kurusugawa Computer Inc."]
 license = "MIT"
 packages = [
     { include = "confluence" }
 ]
 readme="README.md"
@@ -29,15 +29,15 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7"
 pytest-xdist = "*"
 pytest-cov = "*"
 
 
 [tool.poetry.group.linter.dependencies]
-ruff = "^0.2"
+ruff = "^0.4"
 mypy = "^1"
 pylint = "^3"
 
 types-pytz = "*"
 types-requests = "*"
 types-python-dateutil = "*"
 types-PyYAML = "*"
@@ -69,31 +69,24 @@
 [tool.ruff]
 target-version = "py39"
 line-length = 150
 
 [tool.ruff.lint]
 ignore = [
     "G004", # `logging-f-string` : loggingでf-stringを使いたいので無視する
-    "PD901", #すでに`df`という変数をいろんなところで使っているため
-    "PD002", #すでにpandasで`inplace=True`はいろんなところで使っているため
     "RUF001", # 全角記号など`ambiguous unicode character`も使いたいため
     "RUF002",# 全角記号など`ambiguous unicode character`も使いたいため
     "RUF003",# 全角記号など`ambiguous unicode character`も使いたいため
-    "PLC1901", # compare-to-empty-string : `if a == "`のように空文字列で直接比較したいときがあるため
     "PLR2004", # magic-value-comparison: listのサイズで判定するときがよくあるため
     "ANN101", # missing-type-self: 引数selfには型ヒントは付けていないため
     "ANN102", # missing-type-cls: 引数clsには型ヒントは付けていないため
     "ANN002", # missing-type-args
     "ANN003", # missing-type-kwargs
     "ERA", # : 役立つこともあるが、コメントアウトしていないコードも警告されるので無視する
     "UP007", # non-pep604-annotation :
-    # いずれ無視しないようにする
-    "ANN201", # missing-return-type-public-function:
-    "ANN202", # missing-return-type-private-function:
-    "PLR",  # pylint Refactor
 
     # 以下のルールはコードに合っていないので無効化した
     "RSE", # flake8-raise
     "D", # pydocstyle, Docstringを中途半端にしか書いていないので、除外する
     "C90", # mccabe
     "T20", # flake8-print
     "SLF", #  flake8-self
@@ -115,14 +108,26 @@
 ]
 
 
 select = [
     "ALL"
 ]
 
+[tool.ruff.lint.per-file-ignores]
+# テストコードはチェックを緩和する
+"tests/**.py" = [
+    "PGH",  # pygrep-hooks
+    "DTZ",  # flake8-datetimez
+    "ANN",  # flake8-annotations
+    "E501",  # line-too-long
+    "RUF100"  # unused-noqa
+]
+
+
+
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.pylint]
 max-args = 10
```

### Comparing `kci_confluence_cli-0.1.0/PKG-INFO` & `kci_confluence_cli-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kci-confluence-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: 来栖川電算が利用しているConfluence v6.15.7を操作するためのCLIです。
 Home-page: https://github.com/kurusugawa-computer/confluence-cli
 License: MIT
 Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -25,14 +25,20 @@
 Requires-Dist: requests-toolbelt (>=1,<2)
 Project-URL: Repository, https://github.com/kurusugawa-computer/confluence-cli
 Description-Content-Type: text/markdown
 
 # confluence-cli
 来栖川電算が利用しているConfluence v6.15.7を操作するためのCLIです。
 
+
+[![Build Status](https://app.travis-ci.com/kurusugawa-computer/confluence-cli.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/confluence-cli)
+[![PyPI version](https://badge.fury.io/py/kci-confluence-cli.svg)](https://badge.fury.io/py/kci-confluence-cli)
+[![Python Versions](https://img.shields.io/pypi/pyversions/kci-confluence-cli.svg)](https://pypi.org/project/kci-confluence-cli/)
+[![Documentation Status](https://readthedocs.org/projects/confluence-cli/badge/?version=latest)](https://confluence-cli.readthedocs.io/ja/latest/?badge=latest)
+
 # Requirements
 Python 3.9+
 
 # Install
 
 ```
 $ pip install kci-confluence-cli
@@ -57,31 +63,10 @@
 
 上記の方法で指定されない場合は、標準入力から入力できます。
 
 来栖川電算のConfluneceにアクセスする場合は、`https://kurusugawa.jp/confluence`を指定してください。
 
 
 # Command Reference
-### attachment get
-添付ファイル情報の取得
-
-
-### attachment create
-添付ファイルの作成
-
-
-### attachment delete
-添付ファイルを削除します。
-
-※添付ファイルをゴミ箱から完全に削除すると、ページを更新できない場合があります。その場合は、一時的に前のバージョンに戻せば、ページを更新できるようになります。
-https://qiita.com/yuji38kwmt/items/c88f039e02b8508926e6
-
-
-### attachment get
-コンテンツ（ページやブログ、添付ファイルなど）の情報を取得します。
+https://confluence-cli.readthedocs.io/ja/latest/command_reference/index.html を参照してください。
 
-### local convert_html
-HTMLをConfluence用のXMLに変換します。
-Google DocsのページをConfluenceに移行するときなどに利用できます。
-具体的な手順は以下を参照してください。
-https://github.com/kurusugawa-computer/confluence-cli/wiki/Google-Docs%E3%82%92Confluence%E3%81%AB%E7%A7%BB%E8%A1%8C%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95
```

