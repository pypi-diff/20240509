# Comparing `tmp/suskabot-0.2.0.tar.gz` & `tmp/suskabot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suskabot-0.2.0.tar", max compression
+gzip compressed data, was "suskabot-0.2.1.tar", max compression
```

## Comparing `suskabot-0.2.0.tar` & `suskabot-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2024-05-08 00:36:47.241516 suskabot-0.2.0/LICENSE
--rw-r--r--   0        0        0     1706 2024-05-08 00:36:47.241516 suskabot-0.2.0/README.md
--rw-r--r--   0        0        0      779 2024-05-08 00:36:47.248516 suskabot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/__init__.py
--rw-r--r--   0        0        0      914 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/__main__.py
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/app/__init__.py
--rw-r--r--   0        0        0     1529 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/app/app.py
--rw-r--r--   0        0        0      295 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/config/.env.example
--rw-r--r--   0        0        0        4 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/config/.gitignore
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/config/__init__.py
--rw-r--r--   0        0        0     4915 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/config/config.py
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/controllers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/controllers/telegram_api/__init__.py
--rw-r--r--   0        0        0     1494 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/controllers/telegram_api/bot.py
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/__init__.py
--rw-r--r--   0        0        0     1339 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/app.py
--rw-r--r--   0        0        0     1783 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/translator.py
--rw-r--r--   0        0        0     5917 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/services/__init__.py
--rw-r--r--   0        0        0     4158 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/services/translator.py
--rw-r--r--   0        0        0     5948 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/services/youtube_downloader.py
--rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/utils/__init__.py
--rw-r--r--   0        0        0      861 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/utils/utils.py
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 suskabot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 12:49:48.494382 suskabot-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1706 2024-05-08 12:49:48.494382 suskabot-0.2.1/README.md
+-rw-r--r--   0        0        0      815 2024-05-08 12:49:48.501382 suskabot-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      510 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/__main__.py
+-rw-r--r--   0        0        0       23 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/app/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/app/app.py
+-rw-r--r--   0        0        0      381 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/config/.env.example
+-rw-r--r--   0        0        0        4 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/config/.gitignore
+-rw-r--r--   0        0        0       26 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/config/__init__.py
+-rw-r--r--   0        0        0     4908 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/config/config.py
+-rw-r--r--   0        0        0       32 2024-05-08 12:49:48.501382 suskabot-0.2.1/suskabot/controllers/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/controllers/telegram_api/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/controllers/telegram_api/bot.py
+-rw-r--r--   0        0        0       67 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/__init__.py
+-rw-r--r--   0        0        0     1331 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/app.py
+-rw-r--r--   0        0        0     1776 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/translator.py
+-rw-r--r--   0        0        0     6758 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
+-rw-r--r--   0        0        0       56 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/services/__init__.py
+-rw-r--r--   0        0        0     4151 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/services/translator.py
+-rw-r--r--   0        0        0     5924 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/services/youtube_downloader.py
+-rw-r--r--   0        0        0       25 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/utils/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-08 12:49:48.502382 suskabot-0.2.1/suskabot/utils/utils.py
+-rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 suskabot-0.2.1/PKG-INFO
```

### Comparing `suskabot-0.2.0/LICENSE` & `suskabot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.0/README.md` & `suskabot-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.0/pyproject.toml` & `suskabot-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 package-mode = true
 name = "suskabot"
-version = "0.2.0"
+version = "0.2.1"
 description = "telegram bot with various functions"
 authors = ["vinyl_summer <vinyl6428@gmail.dotcom>"]
 readme = "README.md"
 license = "LICENSE"
 
 [[tool.poetry.source]]
 name = "gitlab"
@@ -13,15 +13,15 @@
 priority = "primary"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 lingua-language-detector = "^2.0.2"
 translators = "^5.9.1"
 pytube = { source = "gitlab", version = "15.0.1" }
-python-telegram-bot = "^21.1.1"
+python-telegram-bot = {extras = ["job-queue"], version = "^21.1.1"}
 pydantic = "^2.7.1"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4"
 pytest-sugar = "*"
 ruff = "^0.4.2"
```

### Comparing `suskabot-0.2.0/suskabot/app/app.py` & `suskabot-0.2.1/suskabot/app/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.0/suskabot/config/config.py` & `suskabot-0.2.1/suskabot/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import telegram.constants
 import pydantic
 import dotenv
 
 from suskabot.utils import utils
 
-logger = logging.getLogger(__name__)
+
+logger = logging.getLogger()
 
 
 class VideoResolution(enum.Enum):
     RES_144 = 144
     RES_240 = 240
     RES_360 = 360
     RES_480 = 480
```

### Comparing `suskabot-0.2.0/suskabot/controllers/telegram_api/bot.py` & `suskabot-0.2.1/suskabot/controllers/telegram_api/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from suskabot.controllers.telegram_api.handlers.app import AppHandlers
 from suskabot.controllers.telegram_api.handlers.translator import TranslatorHandlers
 from suskabot.controllers.telegram_api.handlers.youtube_downloader import YTDownloaderHandlers
 from suskabot.services.translator import TranslatorService
 from suskabot.services.youtube_downloader import YTDownloaderService
 
 
-logger: logging.Logger = logging.getLogger(__name__)
+logger: logging.Logger = logging.getLogger()
 
 
 class TGBot:
     _application: Application
     _translator_service: TranslatorService
     _yt_downloader_service: YTDownloaderService
```

### Comparing `suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/app.py` & `suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from telegram import Update
 from telegram.ext import ContextTypes, Application, CommandHandler
 
 
-logger: logging.Logger = logging.getLogger(__name__)
+logger: logging.Logger = logging.getLogger()
 
 
 class AppHandlers:
     _application: Application
 
     def __init__(self, application: Application) -> None:
         self._application = application
```

### Comparing `suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/translator.py` & `suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from telegram import Update
 from telegram.ext import ContextTypes, Application, MessageHandler, filters
 from translators.server import TranslatorError
 
 from suskabot.services.translator import TranslatorService
 
-logger: logging.Logger = logging.getLogger(__name__)
+
+logger: logging.Logger = logging.getLogger()
 
 
 class TranslatorHandlers:
     _application: Application
     _translator_service: TranslatorService
 
     def __init__(
```

### Comparing `suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/youtube_downloader.py` & `suskabot-0.2.1/suskabot/controllers/telegram_api/handlers/youtube_downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import logging
 import concurrent.futures
 
 from asyncio import AbstractEventLoop
 from typing import Set
 
 import telegram.error
+
 from pytube import Stream
 from pytube.exceptions import RegexMatchError, VideoUnavailable, PytubeError
 from telegram import Update, Message
 from telegram.ext import ContextTypes, Application, MessageHandler, filters
 
 from suskabot.services.youtube_downloader import YTDownloaderService, VideoTooLarge
 from suskabot.utils import utils
 
-logger: logging.Logger = logging.getLogger(__name__)
+
+logger: logging.Logger = logging.getLogger()
 
 
 class YTDownloaderHandlers:
     _application: Application
     _yt_downloader_service: YTDownloaderService
 
     # set of telegram user ids
@@ -69,16 +71,28 @@
         progressbar: str = utils.get_formatted_progressbar(video_stream.title, 0)
         progressbar_message: Message = await update.effective_message.reply_text(progressbar)
 
         self._users_with_a_download_in_progress.add(update.effective_user.id)
         logger.debug(f"Added {update.effective_user.id} to the set of downloading user, "
                      f"current set:{self._users_with_a_download_in_progress}")
 
+        async def _delete_progressbar_callback(ctx: ContextTypes.DEFAULT_TYPE) -> None:
+            message_to_delete: Message = ctx.job.data
+            await message_to_delete.delete()
+
+        async def _delayed_progressbar_deletion(progressbar_msg: Message, delay_seconds: float) -> None:
+            context.job_queue.run_once(
+                callback=_delete_progressbar_callback,
+                when=delay_seconds,
+                data=progressbar_msg,
+                name="delayed progressbar deletion"
+            )
+
         async def _clean_up():
-            await progressbar_message.delete()
+            await _delayed_progressbar_deletion(progressbar_message, 1)
             self._users_with_a_download_in_progress.remove(update.effective_user.id)
             logger.debug(f"Successfully deleted the progressbar and "
                          f"Removed {update.effective_user.id} from the set of downloading user, "
                          f"current set:{self._users_with_a_download_in_progress}")
 
         def download_progress_callback(stream: Stream, b: bytes, remaining_bytes: int) -> None:
             logger.debug(f"Got a progress callback for {update.effective_user.full_name} {update.effective_user.id}, "
@@ -100,34 +114,38 @@
                     text=updated_progressbar,
                     chat_id=update.effective_chat.id,
                     message_id=progressbar_message.id
                 ),
                 self._asyncio_loop
             )
 
+        logger.info(f"Downloading video {video_url} for {update.effective_user.full_name}..")
+
         download_yt_video = self._yt_downloader_service.download_youtube_video_stream
         this_loop = self._asyncio_loop
         with concurrent.futures.ThreadPoolExecutor() as pool:
-            logger.debug(f"Spinning up the youtube video downloader thread for "
+            logger.debug("Spinning up the youtube video downloader thread for "
                          f"{update.effective_user.full_name} {update.effective_user.id}")
             try:
                 downloaded_video: bytes | None = await this_loop.run_in_executor(
                     pool,
                     download_yt_video,
                     video_stream,
                     download_progress_callback
                 )
             except (OSError, PytubeError) as e:
                 await _clean_up()
                 logger.error(f"Couldn't download video to disk, {e}")
                 await update.effective_message.reply_text("Service error, please try again later")
                 return
 
-        await progressbar_message.edit_text("Download complete! Sending the video..")
-        logger.debug("Video downloaded, starting to send it")
+        complete_progressbar: str = utils.get_formatted_progressbar(video_stream.title, 100)
+        complete_progressbar += "\nDownload complete! Sending the video.."
+        await progressbar_message.edit_text(complete_progressbar)
+        logger.info(f"{video_stream.title} download completed, sending it to {update.effective_user.full_name}")
 
         try:
             await context.bot.send_video(
                 chat_id=update.effective_chat.id,
                 video=downloaded_video,
                 caption=video_stream.title
             )
```

### Comparing `suskabot-0.2.0/suskabot/services/translator.py` & `suskabot-0.2.1/suskabot/services/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from typing import List, Dict
 
 import translators
 
 from lingua import Language, LanguageDetector, LanguageDetectorBuilder
 from translators.server import TranslatorError
 
-logger = logging.getLogger(__name__)
+
+logger = logging.getLogger()
 
 
 class TranslatorService:
     _translation_services: List[str]
     _user_language: str
     _default_language_to_translate_to: str
```

### Comparing `suskabot-0.2.0/suskabot/services/youtube_downloader.py` & `suskabot-0.2.1/suskabot/services/youtube_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import logging
 import pathlib
-import shutil
-from io import BytesIO
 
+import io
 from typing import Optional, Callable
 
 from pytube import YouTube, StreamQuery, Stream
-from pytube.exceptions import RegexMatchError, VideoUnavailable
+from pytube.exceptions import PytubeError
 
 from suskabot.utils import utils
 
-logger: logging.Logger = logging.getLogger(__name__)
+
+logger: logging.Logger = logging.getLogger()
 
 
 class VideoTooLarge(Exception):
     """Raise if a video file size exceeds set limits"""
 
 
 class YTVideoMetadata:
@@ -86,24 +86,23 @@
         :raises VideoUnavailable: If the video is unavailable for some reason
         :raises VideoTooLarge: If video file size exceeds set limits
         """
 
         try:
             video_data = YouTube(url=video_url)
             video_data.check_availability()
-        except RegexMatchError as e:
-            raise e
-        except VideoUnavailable as e:
+        except PytubeError as e:
+            logger.exception("Failed to get video stream data: ", exc_info=e)
             raise e
 
         progressive_video_streams: StreamQuery = video_data.streams.filter(progressive=True)
         logger.debug(f"Found progressive streams:\n{progressive_video_streams}")
 
         video_stream: Stream | None = self._get_best_quality_stream_under_limits(progressive_video_streams)
-        logger.debug(f"Selected video stream:\n{video_stream}")
+        logger.info(f"Selected video stream:\n{video_stream}")
 
         if not video_stream:
             raise VideoTooLarge(f"Can't download videos larger than {self._file_size_limit_mb}MB")
 
         return video_stream
 
     def download_youtube_video_stream(
@@ -131,23 +130,23 @@
         video_stream._monostate.on_progress = progress_callback
 
         if self._save_to_drive:
             video_path: str = video_stream.download(
                 output_path=str(self._default_download_path)
             )
         else:
-            with BytesIO() as buffer:
+            with io.BytesIO() as buffer:
                 video_stream.stream_to_buffer(buffer)
-                logger.info(f"Successfully downloaded {video_stream.url} to RAM")
+                logger.info(f"Successfully downloaded {video_stream.title} to RAM")
                 return buffer.getvalue()
 
         with open(video_path, "rb") as video_file:
             logger.info(f"Successfully downloaded {video_stream.url} to drive")
             return video_file.read()
 
     # doesn't serve any purpose as of now, but I'll leave it here for a bit
-    def __clear_download_directory(self) -> None:
-        try:
-            shutil.rmtree(self._default_download_path)
-        except Exception as e:
-            logger.warning(f"Could not clear download directory, {e}")
-            raise e
+    # def __clear_download_directory(self) -> None:
+    #     try:
+    #         shutil.rmtree(self._default_download_path)
+    #     except Exception as e:
+    #         logger.warning(f"Could not clear download directory, {e}")
+    #         raise e
```

### Comparing `suskabot-0.2.0/suskabot/utils/utils.py` & `suskabot-0.2.1/suskabot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.0/PKG-INFO` & `suskabot-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: suskabot
-Version: 0.2.0
+Version: 0.2.1
 Summary: telegram bot with various functions
 License: LICENSE
 Author: vinyl_summer
 Author-email: vinyl6428@gmail.dotcom
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: python-telegram-bot (>=21.1.1,<22.0.0)
+Requires-Dist: python-telegram-bot[job-queue] (>=21.1.1,<22.0.0)
 Requires-Dist: pytube (==15.0.1)
 Requires-Dist: translators (>=5.9.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Suskabot
 Telegram Bot that really can do it all!
```

