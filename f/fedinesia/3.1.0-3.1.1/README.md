# Comparing `tmp/fedinesia-3.1.0.tar.gz` & `tmp/fedinesia-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedinesia-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedinesia-3.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedinesia-3.1.0.tar` & `fedinesia-3.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3544 2024-04-19 09:32:31.690687 fedinesia-3.1.0/README.rst
--rw-r--r--   0        0        0     2484 2024-04-19 09:32:31.690687 fedinesia-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      618 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/__init__.py
--rw-r--r--   0        0        0    11337 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/amnesia.py
--rw-r--r--   0        0        0    12472 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/config.py
--rw-r--r--   0        0        0     7655 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/util.py
--rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 fedinesia-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3544 2023-12-16 07:32:50.402722 fedinesia-3.1.1/README.rst
+-rw-r--r--   0        0        0     2450 2024-05-09 09:31:01.887985 fedinesia-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      488 2024-05-09 09:31:01.887985 fedinesia-3.1.1/src/fedinesia/__init__.py
+-rw-r--r--   0        0        0    11359 2024-05-09 09:31:01.887985 fedinesia-3.1.1/src/fedinesia/amnesia.py
+-rw-r--r--   0        0        0    12276 2024-05-09 09:31:01.887985 fedinesia-3.1.1/src/fedinesia/config.py
+-rw-r--r--   0        0        0     7583 2024-05-09 09:31:01.887985 fedinesia-3.1.1/src/fedinesia/util.py
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 fedinesia-3.1.1/PKG-INFO
```

### Comparing `fedinesia-3.1.0/README.rst` & `fedinesia-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `fedinesia-3.1.0/pyproject.toml` & `fedinesia-3.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Deletes old posts from fediverse accounts. Confirmed working with Mastodon, Pleroma (and Forks), and Takahe'
 readme = "README.rst"
 authors = [
   { name = "marvin8", email = "marvin8@tuta.io" },
 ]
 requires-python = ">=3.9, <3.13"
 license = {text = "AGPL-3.0-or-later"}
-version = "3.1.0"
+version = "3.1.1"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
@@ -24,31 +24,30 @@
 dependencies = [
     "loguru>=0.7.2",
     "minimal-activitypub>=1.2.0",
     "msgspec>=0.18.6",
     "python-dateutil>=2.9.0.post0",
     "stamina>=24.2.0",
     "tomli>=2.0.1",
-    "tqdm>=4.66.2",
+    "tqdm>=4.66.4",
     "typer>=0.12.3",
-    "typing-extensions>=4.11.0",
 ]
 
 [project.scripts]
 fedinesia = "fedinesia.amnesia:start"
 
 [project.urls]
 Documentation = "https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/README.rst"
 Issues = "https://codeberg.org/MarvinsMastodonTools/fedinesia/issues"
 Source = "https://codeberg.org/MarvinsMastodonTools/fedinesia"
 Changelog = "https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/CHANGELOG.rst"
 
 [project.optional-dependencies]
 dev = [
-    "constable>=0.3.1",
+    "icecream>=2.1.3",
 ]
 
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
```

### Comparing `fedinesia-3.1.0/src/fedinesia/amnesia.py` & `fedinesia-3.1.1/src/fedinesia/amnesia.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 import msgspec
 import stamina
 import typer
 from dateutil.parser import isoparse
 from httpx import AsyncClient
 from httpx import HTTPError
 from loguru import logger as log
+from minimal_activitypub import Status
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ActivityPubError
 from minimal_activitypub.client_2_server import NetworkError
 from minimal_activitypub.client_2_server import NotFoundError
 from minimal_activitypub.client_2_server import RatelimitError
 from stamina import retry_context
 from tqdm import tqdm
 from tqdm import trange
 from typing_extensions import Annotated
 
 from fedinesia import UTC
-from fedinesia import Status
 from fedinesia import __display_name__
 from fedinesia import __version__
 from fedinesia.config import setup_shop
 from fedinesia.util import AuditLog
 from fedinesia.util import should_keep
 
 logging_config_path = Path("logging-config.toml")
@@ -80,15 +80,15 @@
 
     oldest_to_keep = datetime.now(tz=UTC) - timedelta(seconds=config.bot.delete_after)
 
     log.info(f"Welcome to {__display_name__} {__version__}")
     log.debug(f"{config=}")
 
     try:
-        client = AsyncClient(http2=True)
+        client = AsyncClient(http2=True, timeout=30)
 
         instance = ActivityPub(
             instance=config.mastodon.instance,
             access_token=config.mastodon.access_token,
             client=client,
         )
         await instance.determine_instance_type()
```

### Comparing `fedinesia-3.1.0/src/fedinesia/config.py` & `fedinesia-3.1.1/src/fedinesia/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,55 +13,43 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import logging
 import sys
-from enum import Enum
 from pathlib import Path
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import msgspec
 from httpx import AsyncClient
+from minimal_activitypub import Visibility
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ActivityPubError
 
 from fedinesia import CLIENT_WEBSITE
 from fedinesia import USER_AGENT
 
 BC = TypeVar("BC", bound="BotConfig")
 ConfigClass = TypeVar("ConfigClass", bound="Configuration")
 MC = TypeVar("MC", bound="MastodonConfig")
 
 
-class Visibility(str, Enum):
-    """Enumerating different audit log file styles implemented."""
-
-    PUBLIC = "public"
-    UNLISTED = "unlisted"
-    PRIVATE = "private"
-    DIRECT = "direct"
-
-
 class BotConfig(msgspec.Struct):
     """Class holding configuration values for general behaviour of Fedinesia."""
 
-    log_level: str
     delete_after: int
     skip_deleting_pinned: bool = False
     skip_deleting_faved: bool = False
     skip_deleting_bookmarked: bool = False
     skip_deleting_poll: bool = False
-    skip_deleting_dm: bool = False  # This is deprecated, use `skip_visibility = [Visibility.DIRECT]` instead
-    skip_deleting_visibility: List[Visibility] = []
+    skip_deleting_visibility: List[Visibility] = msgspec.field(default_factory=lambda: [])
     skip_deleting_media: bool = False
     skip_deleting_faved_at_least: int = 0
     skip_deleting_boost_at_least: int = 0
     skip_deleting_reactions_at_least: int = 0
 
     def get_config_values(self: BC) -> None:
         """Initialise instance."""
@@ -94,17 +82,17 @@
     def _get_skip_dm(self: BC) -> None:
         """Private method to get skip deleting 'private' messages value from
         user if this value has not yet been configured.
         """
         print("Should Direct Messages be deleted when they get old enough?")
         y_or_n = input("[..] Please enter Y for yes or N for no: ")
         if y_or_n in ("Y", "y"):
-            self.skip_deleting_dm = False
+            self.skip_deleting_visibility = []
         elif y_or_n in ("N", "n"):
-            self.skip_deleting_dm = True
+            self.skip_deleting_visibility = [Visibility.DIRECT]
         else:
             print("! ERROR ... please only respond with 'Y' or 'N'")
             print("! Cannot continue. Exiting now.")
             sys.exit(1)
 
     def _get_skip_media(self: BC) -> None:
         """Private method to get skip deleting statuses with media value from
@@ -237,15 +225,15 @@
 
     @classmethod
     async def establish_new_mastodon_config(cls: Type[MC]) -> MC:
         """Establish Mastodon configuration from scratch."""
         instance = input("[..] Enter instance (domain name) for Mastodon account host: ")
 
         try:
-            with AsyncClient(http2=True) as client:
+            async with AsyncClient(http2=True) as client:
                 # Create app
                 client_id, client_secret = await ActivityPub.create_app(
                     instance_url=instance,
                     client=client,
                     user_agent=USER_AGENT,
                     client_website=CLIENT_WEBSITE,
                 )
@@ -294,16 +282,18 @@
     """
     config_file_path = Path(config_file)
     if config_file_path.exists():
         with config_file_path.open(mode="rb") as config_file_file:
             config: Configuration = msgspec.json.decode(config_file_file.read(), type=Configuration)
 
     else:
-        bot = BotConfig(log_level=logging.WARNING, delete_after=30)
+        bot = BotConfig(delete_after=30)
         bot.get_config_values()
-        config = Configuration(bot=bot, mastodon=MastodonConfig.establish_new_mastodon_config())
+        mastodon = await MastodonConfig.establish_new_mastodon_config()
+        config = Configuration(bot=bot, mastodon=mastodon)
 
-        config_json = msgspec.json.format(msgspec.json.encode(obj=config), indent=4)
+        config_encoded = msgspec.json.encode(config)
+        config_json = msgspec.json.format(buf=config_encoded, indent=4)
         with config_file_path.open(mode="wb") as config_file_file:
             config_file_file.write(config_json)
 
     return config
```

### Comparing `fedinesia-3.1.0/src/fedinesia/util.py` & `fedinesia-3.1.1/src/fedinesia/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from typing import Any
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from dateutil.parser import isoparse
 from loguru import logger as log
+from minimal_activitypub.client_2_server import Status
 
-from fedinesia import Status
 from fedinesia import __display_name__
 from fedinesia.config import Configuration
 
 logger = logging.getLogger(__display_name__)
 
 
 AL = TypeVar("AL", bound="AuditLog")
@@ -157,17 +157,14 @@
 
     if config.bot.skip_deleting_pinned and bool(status.get("pinned")):
         return True
 
     if config.bot.skip_deleting_poll and bool(status.get("poll")):
         return True
 
-    if config.bot.skip_deleting_dm and status.get("visibility") == "direct":
-        return True
-
     if status.get("visibility") in config.bot.skip_deleting_visibility:
         return True
 
     medias = status.get("media_attachments")
     if config.bot.skip_deleting_media and isinstance(medias, list) and bool(len(medias)):
         return True
```

### Comparing `fedinesia-3.1.0/PKG-INFO` & `fedinesia-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedinesia
-Version: 3.1.0
+Version: 3.1.1
 Summary: Deletes old posts from fediverse accounts. Confirmed working with Mastodon, Pleroma (and Forks), and Takahe
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
@@ -13,18 +13,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: minimal-activitypub>=1.2.0
 Requires-Dist: msgspec>=0.18.6
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: stamina>=24.2.0
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: tqdm>=4.66.2
+Requires-Dist: tqdm>=4.66.4
 Requires-Dist: typer>=0.12.3
-Requires-Dist: typing-extensions>=4.11.0
-Requires-Dist: constable>=0.3.1 ; extra == "dev"
+Requires-Dist: icecream>=2.1.3 ; extra == "dev"
 Project-URL: Changelog, https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/CHANGELOG.rst
 Project-URL: Documentation, https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/README.rst
 Project-URL: Issues, https://codeberg.org/MarvinsMastodonTools/fedinesia/issues
 Project-URL: Source, https://codeberg.org/MarvinsMastodonTools/fedinesia
 Provides-Extra: dev
 
 """"""""""""""""""""""""""
```

