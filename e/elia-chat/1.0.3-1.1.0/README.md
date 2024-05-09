# Comparing `tmp/elia_chat-1.0.3.tar.gz` & `tmp/elia_chat-1.1.0.tar.gz`

## Comparing `elia_chat-1.0.3.tar` & `elia_chat-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.0.3/.python-version
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 elia_chat-1.0.3/requirements-dev.lock
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 elia_chat-1.0.3/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/__main__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/app.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/config.py
--rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/locations.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/models.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/database/models.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.0.3/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.0.3/.gitignore
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 elia_chat-1.0.3/README.md
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 elia_chat-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.1.0/.python-version
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.1.0/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/app.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/config.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/constants.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/locations.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/models.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.1.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.1.0/.gitignore
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 elia_chat-1.1.0/README.md
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 elia_chat-1.1.0/PKG-INFO
```

### Comparing `elia_chat-1.0.3/.pre-commit-config.yaml` & `elia_chat-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/requirements-dev.lock` & `elia_chat-1.1.0/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 fsspec==2024.3.1
     # via huggingface-hub
 greenlet==3.0.3
     # via elia-chat
+    # via sqlalchemy
 h11==0.14.0
     # via httpcore
 httpcore==1.0.2
     # via httpx
 httpx==0.26.0
     # via openai
 huggingface-hub==0.22.2
```

### Comparing `elia_chat-1.0.3/requirements.lock` & `elia_chat-1.1.0/requirements.lock`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 fsspec==2024.3.1
     # via huggingface-hub
 greenlet==3.0.3
     # via elia-chat
+    # via sqlalchemy
 h11==0.14.0
     # via httpcore
 httpcore==1.0.2
     # via httpx
 httpx==0.26.0
     # via openai
 huggingface-hub==0.22.2
```

### Comparing `elia_chat-1.0.3/elia_chat/__main__.py` & `elia_chat-1.1.0/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/app.py` & `elia_chat-1.1.0/elia_chat/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from textual.app import App
 from textual.binding import Binding
 from textual.signal import Signal
 
 from elia_chat.chats_manager import ChatsManager
 from elia_chat.models import ChatData, ChatMessage
-from elia_chat.config import LaunchConfig
+from elia_chat.config import EliaChatModel, LaunchConfig, launch_config
 from elia_chat.runtime_config import RuntimeConfig
 from elia_chat.screens.chat_screen import ChatScreen
 from elia_chat.screens.help_screen import HelpScreen
 from elia_chat.screens.home_screen import HomeScreen
 
 if TYPE_CHECKING:
     from litellm.types.completion import (
@@ -23,22 +23,24 @@
     )
 
 
 class Elia(App[None]):
     ENABLE_COMMAND_PALETTE = False
     CSS_PATH = Path(__file__).parent / "elia.scss"
     BINDINGS = [
-        Binding("f1", "help", "Help", priority=True),
+        Binding("q", "app.quit", "Quit", show=False),
+        Binding("?", "help", "Help"),
     ]
 
     def __init__(self, config: LaunchConfig, startup_prompt: str = ""):
         super().__init__()
         self.launch_config = config
+        launch_config.set(config)
         self._runtime_config = RuntimeConfig(
-            selected_model=config.default_model,
+            selected_model=config.default_model_object,
             system_prompt=config.system_prompt,
         )
         self.runtime_config_signal = Signal[RuntimeConfig](
             self, "runtime-config-updated"
         )
         """Widgets can subscribe to this signal to be notified of
         when the user has changed configuration at runtime (e.g. using the UI)."""
@@ -60,42 +62,42 @@
         self.runtime_config_signal.publish(self.runtime_config)
 
     async def on_mount(self) -> None:
         self.push_screen(HomeScreen(self.runtime_config_signal))
         if self.startup_prompt:
             await self.launch_chat(
                 prompt=self.startup_prompt,
-                model_name=self.runtime_config.selected_model,
+                model=self.runtime_config.selected_model,
             )
 
-    async def launch_chat(self, prompt: str, model_name: str) -> None:
+    async def launch_chat(self, prompt: str, model: EliaChatModel) -> None:
         current_time = datetime.datetime.now(datetime.UTC)
         system_message: ChatCompletionSystemMessageParam = {
             "content": self.runtime_config.system_prompt,
             "role": "system",
         }
         user_message: ChatCompletionUserMessageParam = {
             "content": prompt,
             "role": "user",
         }
         chat = ChatData(
             id=None,
             title=None,
             create_timestamp=None,
-            model_name=model_name,
+            model=model,
             messages=[
                 ChatMessage(
                     message=system_message,
                     timestamp=current_time,
-                    model=model_name,
+                    model=model,
                 ),
                 ChatMessage(
                     message=user_message,
                     timestamp=current_time,
-                    model=model_name,
+                    model=model,
                 ),
             ],
         )
         chat.id = await ChatsManager.create_chat(chat_data=chat)
         await self.push_screen(ChatScreen(chat))
 
     async def action_help(self) -> None:
```

### Comparing `elia_chat-1.0.3/elia_chat/chats_manager.py` & `elia_chat-1.1.0/elia_chat/chats_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,33 +55,34 @@
         log.debug(f"Retrieved {len(chat_messages)} chats for chat {chat_id!r}")
         return chat_messages
 
     @staticmethod
     async def create_chat(chat_data: ChatData) -> int:
         log.debug(f"Creating chat in database: {chat_data!r}")
 
-        model = chat_data.model_name
+        model = chat_data.model
+        lookup_key = model.lookup_key
         async with get_session() as session:
             chat = ChatDao(
-                model=model,
+                model=lookup_key,
                 title="",
                 started_at=datetime.datetime.now(datetime.UTC),
             )
             session.add(chat)
             await session.commit()
 
             chat_id = chat.id
             for message in chat_data.messages:
                 litellm_message = message.message
                 content = litellm_message["content"]
                 new_message = MessageDao(
                     chat_id=chat_id,
                     role=litellm_message["role"],
                     content=content if isinstance(content, str) else "",
-                    model=model,
+                    model=lookup_key,
                     timestamp=message.timestamp,
                 )
                 (await chat.awaitable_attrs.messages).append(new_message)
 
             await session.commit()
 
         return chat.id
```

### Comparing `elia_chat-1.0.3/elia_chat/elia.scss` & `elia_chat-1.1.0/elia_chat/elia.scss`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,24 @@
 Tabs .underline--bar {
   color: $main-lighten-2 50%;
   background: $main 75%;
 }
 
 Screen {
   background: $background;
+  padding: 0 2 1 2;
 }
 
 ModalScreen {
   background: black 50%;
+  padding: 0;
+
+  & Footer {
+    margin: 0 2 1 2;
+  }
 }
 
 Rule {
   color: white 20%;
 
   &.-horizontal {
     margin: 0 0;
@@ -99,14 +105,15 @@
     & .text-area--selection {
       background: $main 60%;
     }
   }
   & .text-area--cursor-line {
     background: $background 0%;
   }
+
   & .text-area--cursor-gutter {
     background: $background 0%;
   }
   &:focus .text-area--cursor-gutter {
     color: yellowgreen;
     background: $background 0%;
   }
@@ -204,22 +211,33 @@
     & TextArea {
       & .text-area--selection {
         background: greenyellow 23%;
         color: white 93%;
       }
     }
 
+    & SelectionTextArea.visual-mode {
+      & .text-area--cursor {
+        background: greenyellow;
+      }
+    }
+
   }
 
   &.human-message {
     border: round $main-border-color;
     &:focus-within {
       border: round $main-border-color-focus;
       border-left: thick $main-border-color-focus;
     }
+    & SelectionTextArea.visual-mode {
+      & .text-area--cursor {
+        background: $main-lighten-2;
+      }
+    }
   }
 
 }
 
 Footer {
   background: $main-darken-1 0%;
 }
```

### Comparing `elia_chat-1.0.3/elia_chat/locations.py` & `elia_chat-1.1.0/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/models.py` & `elia_chat-1.1.0/elia_chat/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import UTC, datetime
 from typing import TYPE_CHECKING
 
 
-from elia_chat.config import LaunchConfig, EliaChatModel
+from elia_chat.config import LaunchConfig, EliaChatModel, launch_config
 
 if TYPE_CHECKING:
     from litellm.types.completion import ChatCompletionMessageParam
 
 
 class UnknownModel(EliaChatModel):
     pass
 
 
-def get_model_by_name(model_name: str, config: LaunchConfig) -> EliaChatModel:
-    """Given the name of a model as a string, return the EliaChatModel."""
+def get_model(
+    model_id_or_name: str, config: LaunchConfig | None = None
+) -> EliaChatModel:
+    """Given the id or name of a model as a string, return the EliaChatModel.
+
+    Models are looked up by ID first.
+    """
+    if config is None:
+        config = launch_config.get()
     try:
-        return {model.name: model for model in config.all_models}[model_name]
+        return {model.id: model for model in config.all_models}[model_id_or_name]
     except KeyError:
-        return UnknownModel(name=model_name)
+        try:
+            return {model.name: model for model in config.all_models}[model_id_or_name]
+        except KeyError:
+            pass
+    return UnknownModel(id="unknown", name="unknown model")
 
 
 @dataclass
 class ChatMessage:
     message: ChatCompletionMessageParam
     timestamp: datetime | None
-    model: str
+    model: EliaChatModel
 
 
 @dataclass
 class ChatData:
     id: int | None  # Can be None before the chat gets assigned ID from database.
-    model_name: str
+    model: EliaChatModel
     title: str | None
     create_timestamp: datetime | None
     messages: list[ChatMessage]
 
     @property
     def short_preview(self) -> str:
         first_message = self.first_user_message.message
```

### Comparing `elia_chat-1.0.3/elia_chat/time_display.py` & `elia_chat-1.1.0/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/database/converters.py` & `elia_chat-1.1.0/elia_chat/database/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Any
 
 
 from elia_chat.database.models import ChatDao, MessageDao
-from elia_chat.models import ChatData, ChatMessage
+from elia_chat.models import ChatData, ChatMessage, get_model
 
 if TYPE_CHECKING:
     from litellm.types.completion import ChatCompletionUserMessageParam
 
 
 def chat_message_to_message_dao(
     message: ChatMessage,
@@ -16,26 +16,26 @@
     meta: dict[str, Any] = {}
     content = message.message.get("content", "")
     return MessageDao(
         chat_id=chat_id,
         role=message.message["role"],
         content=content if isinstance(content, str) else "",
         timestamp=message.timestamp,
-        model=message.model,
+        model=message.model.lookup_key,
         meta=meta,
     )
 
 
 def chat_dao_to_chat_data(chat_dao: ChatDao) -> ChatData:
     """Convert the SQLModel chat to a ChatData."""
     model = chat_dao.model
     return ChatData(
         id=chat_dao.id,
         title=chat_dao.title,
-        model_name=model,
+        model=get_model(model),
         create_timestamp=chat_dao.started_at if chat_dao.started_at else None,
         messages=[
             message_dao_to_chat_message(message, model) for message in chat_dao.messages
         ],
     )
 
 
@@ -45,9 +45,9 @@
         "content": message_dao.content,
         "role": message_dao.role,  # type: ignore
     }
 
     return ChatMessage(
         message=message,
         timestamp=message_dao.timestamp,
-        model=model,
+        model=get_model(model),
     )
```

### Comparing `elia_chat-1.0.3/elia_chat/database/database.py` & `elia_chat-1.1.0/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/database/import_chatgpt.py` & `elia_chat-1.1.0/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/database/models.py` & `elia_chat-1.1.0/elia_chat/database/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/screens/chat_details.py` & `elia_chat-1.1.0/elia_chat/screens/chat_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import humanize
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Horizontal, Vertical, VerticalScroll
 from textual.screen import ModalScreen
 from textual.widgets import Label, Markdown, Rule
 
-from elia_chat.models import ChatData, get_model_by_name
+from elia_chat.models import ChatData
 
 if TYPE_CHECKING:
     from elia_chat.app import Elia
 
 
 class ChatDetails(ModalScreen[None]):
     BINDINGS = [
@@ -48,18 +48,18 @@
 
                 with VerticalScroll(id="right"):
                     yield Label("Identifier", classes="heading")
                     yield Label(str(chat.id) or "Unknown", classes="datum")
 
                     yield Rule()
 
+                    model = chat.model
                     yield Label("Model information", classes="heading")
-                    yield Label(chat.model_name, classes="datum")
+                    yield Label(model.name, classes="datum")
 
-                    model = get_model_by_name(chat.model_name, self.elia.launch_config)
                     if display_name := model.display_name:
                         yield Label(display_name, classes="datum")
                     if provider := model.provider:
                         yield Label(provider, classes="datum")
 
                     yield Rule()
```

### Comparing `elia_chat-1.0.3/elia_chat/screens/chat_screen.py` & `elia_chat-1.1.0/elia_chat/screens/chat_screen.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from elia_chat.chats_manager import ChatsManager
 from elia_chat.widgets.agent_is_typing import AgentIsTyping
 from elia_chat.widgets.chat import Chat
 from elia_chat.models import ChatData
 
 
 class ChatScreen(Screen[None]):
-    AUTO_FOCUS = "PromptInput"
+    AUTO_FOCUS = "ChatPromptInput"
     BINDINGS = [
         Binding(
-            key="m",
+            key="escape",
             action="focus('prompt')",
             description="Focus prompt",
-            key_display="m",
+            key_display="esc",
         ),
     ]
 
     def __init__(
         self,
         chat_data: ChatData,
     ):
```

### Comparing `elia_chat-1.0.3/elia_chat/screens/help_screen.py` & `elia_chat-1.1.0/elia_chat/screens/help_screen.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from textual.binding import Binding
 from textual.containers import Vertical, VerticalScroll
 from textual.screen import ModalScreen
 from textual.widgets import Footer, Markdown
 
 
 class HelpScreen(ModalScreen[None]):
-    BINDINGS = [Binding("escape,f1", "app.pop_screen()", "Close help")]
+    BINDINGS = [
+        Binding("q", "app.quit", "Quit", show=False),
+        Binding("escape,?", "app.pop_screen()", "Close help", key_display="esc"),
+    ]
 
     HELP_MARKDOWN = """\
 ### How do I quit Elia?
 
 Press `Ctrl+C` on your keyboard.ga
 
 ### Environment
@@ -31,14 +34,17 @@
 
 ### General navigation
 
 Use `tab` and `shift+tab` to move between different widgets on screen.
 
 In some places you can make use of the arrow keys or Vim nav keys to move around.
 
+In general, pressing `esc` will move you "closer to home".
+Pay attention to the bar at the bottom to see where `esc` will take you.
+
 If you can see a scrollbar, `pageup`, `pagedown`, `home`, and `end` can also
 be used to navigate.
 
 On the chat screen, pressing `up` and `down` will navigate through messages,
 but if you just wish to scroll a little, you can use `shift+up` and `shift+down`.
 
 ### The chat history
@@ -112,20 +118,22 @@
 
 Press `shift+tab` to focus the latest message (or move the cursor `up` from (0, 0)).
 
 You can use the arrow keys to move up and down through messages.
 
 _With a message focused_:
 
-- `c`: Copy the raw Markdown of the message to the clipboard.
+- `y,c`: Copy the raw Markdown of the message to the clipboard.
     - This requires terminal support. The default MacOS terminal is not supported.
-- `space`: Enter _select mode_.
-    - In this mode, you can move a cursor through the text, `optionally` holding
-        shift to select text as you move.
-    - With some text selected, press `c` to copy.
+- `enter`: Enter _select mode_.
+    - In this mode, you can move a cursor through the text, optionally holding
+        `shift` to select text as you move.
+    - Press `v` to toggle _visual mode_, allowing you to select without text without
+        needing to hold `shift`.
+    - With some text selected, press `y` or c` to copy.
 - `enter`: View more details about a message.
     - The amount of details available may vary depending on the model
         or provider being used.
 - `g`: Focus the first message.
 - `G`: Focus the latest message.
 - `m`: Move focus to the prompt box.
 - `up,down,k,j`: Navigate through messages.
```

### Comparing `elia_chat-1.0.3/elia_chat/screens/home_screen.py` & `elia_chat-1.1.0/elia_chat/screens/home_screen.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 from elia_chat.screens.chat_screen import ChatScreen
 from elia_chat.widgets.chat_options import OptionsModal
 
 if TYPE_CHECKING:
     from elia_chat.app import Elia
 
 
+class HomePromptInput(PromptInput):
+    BINDINGS = [Binding("escape", "app.quit", "Exit Elia", key_display="esc")]
+
+
 class HomeScreen(Screen[None]):
     CSS = """\
 ChatList {
     height: 1fr;
     width: 1fr;
     background: $background 15%;
 }
 """
 
     BINDINGS = [
-        Binding("escape,m", "focus('home-prompt')", "Focus prompt", key_display="esc"),
         Binding(
             "ctrl+j", "send_message", "Send message", priority=True, key_display="^j"
         ),
         Binding("o,ctrl+o", "options", "Options", key_display="^o"),
     ]
 
     def __init__(
@@ -48,15 +51,15 @@
         self.elia = cast("Elia", self.app)
 
     def on_mount(self) -> None:
         self.chats_manager = ChatsManager()
 
     def compose(self) -> ComposeResult:
         yield AppHeader(self.config_signal)
-        yield PromptInput(id="home-prompt")
+        yield HomePromptInput(id="home-prompt")
         yield ChatList()
         yield Footer()
 
     @on(ScreenResume)
     async def reload_screen(self) -> None:
         chat_list = self.query_one(ChatList)
         await chat_list.reload_and_refresh()
@@ -67,18 +70,17 @@
         assert chat_id is not None
         chat = await self.chats_manager.get_chat(chat_id)
         await self.app.push_screen(ChatScreen(chat))
 
     @on(PromptInput.PromptSubmitted)
     async def create_new_chat(self, event: PromptInput.PromptSubmitted) -> None:
         text = event.text
-        event.prompt_input.clear()
         await self.elia.launch_chat(  # type: ignore
             prompt=text,
-            model_name=self.elia.runtime_config.selected_model,
+            model=self.elia.runtime_config.selected_model,
         )
 
     @on(PromptInput.CursorEscapingBottom)
     async def move_focus_below(self) -> None:
         self.focus_next(ChatList)
 
     def action_send_message(self) -> None:
```

### Comparing `elia_chat-1.0.3/elia_chat/widgets/app_header.py` & `elia_chat-1.1.0/elia_chat/widgets/app_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from textual.containers import Horizontal, Vertical
 from textual.signal import Signal
 from textual.widget import Widget
 from textual.widgets import Label
 
 from rich.text import Text
 from elia_chat.config import EliaChatModel
-from elia_chat.models import get_model_by_name
+from elia_chat.models import get_model
 from elia_chat.runtime_config import RuntimeConfig
 
 
 if TYPE_CHECKING:
     from elia_chat.app import Elia
 
 
@@ -31,16 +31,15 @@
     ) -> None:
         super().__init__(name=name, id=id, classes=classes, disabled=disabled)
         self.config_signal: Signal[RuntimeConfig] = config_signal
         self.elia = cast("Elia", self.app)
 
     def on_mount(self) -> None:
         def on_config_change(config: RuntimeConfig) -> None:
-            model = get_model_by_name(config.selected_model, self.elia.launch_config)
-            self._update_selected_model(model)
+            self._update_selected_model(config.selected_model)
 
         self.config_signal.subscribe(self, on_config_change)
 
     def compose(self) -> ComposeResult:
         title_style = self.get_component_rich_style("app-title")
         subtitle_style = self.get_component_rich_style("app-subtitle")
 
@@ -49,17 +48,21 @@
                 yield Label(
                     Text.assemble(
                         ("elia ", title_style + Style(bold=True)),
                         ("///", subtitle_style),
                         (f" {version('elia_chat')}", title_style),
                     )
                 )
-            model_name = self.elia.runtime_config.selected_model
-            model = get_model_by_name(model_name, self.elia.launch_config)
+            model_name_or_id = (
+                self.elia.runtime_config.selected_model.id
+                or self.elia.runtime_config.selected_model.name
+            )
+            model = get_model(model_name_or_id, self.elia.launch_config)
             yield Label(self._get_selected_model_link_text(model), id="model-label")
 
     def _get_selected_model_link_text(self, model: EliaChatModel) -> str:
         return f"[@click=screen.options]{escape(model.display_name or model.name)}[/]"
 
     def _update_selected_model(self, model: EliaChatModel) -> None:
+        print(self.elia.runtime_config)
         model_label = self.query_one("#model-label", Label)
         model_label.update(self._get_selected_model_link_text(model))
```

### Comparing `elia_chat-1.0.3/elia_chat/widgets/chat.py` & `elia_chat-1.1.0/elia_chat/widgets/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, cast
 
+from elia_chat import constants
 from textual import log, on, work, events
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import VerticalScroll
 from textual.css.query import NoMatches
 from textual.message import Message
 from textual.reactive import reactive
@@ -15,32 +16,31 @@
 
 from elia_chat.chats_manager import ChatsManager
 from elia_chat.models import ChatData, ChatMessage
 from elia_chat.screens.chat_details import ChatDetails
 from elia_chat.widgets.agent_is_typing import AgentIsTyping
 from elia_chat.widgets.chat_header import ChatHeader
 from elia_chat.widgets.prompt_input import PromptInput
-from elia_chat.models import (
-    EliaChatModel,
-    get_model_by_name,
-)
 from elia_chat.widgets.chatbox import Chatbox
 
 
 if TYPE_CHECKING:
     from elia_chat.app import Elia
     from litellm.types.completion import (
         ChatCompletionUserMessageParam,
         ChatCompletionAssistantMessageParam,
     )
 
 
+class ChatPromptInput(PromptInput):
+    BINDINGS = [Binding("escape", "app.pop_screen", "Close chat", key_display="esc")]
+
+
 class Chat(Widget):
     BINDINGS = [
-        Binding("escape", "close", "Close", key_display="esc"),
         Binding("shift+down", "scroll_container_down", show=False),
         Binding("shift+up", "scroll_container_up", show=False),
         Binding(
             key="g",
             action="focus_first_message",
             description="First message",
             key_display="g",
@@ -58,42 +58,44 @@
     allow_input_submit = reactive(True)
     """Used to lock the chat input while the agent is responding."""
 
     def __init__(self, chat_data: ChatData) -> None:
         super().__init__()
         self.chat_data = chat_data
         self.elia = cast("Elia", self.app)
-        self.model = get_model_by_name(chat_data.model_name, self.elia.launch_config)
+        self.model = chat_data.model
 
     @dataclass
     class AgentResponseStarted(Message):
         pass
 
     @dataclass
     class AgentResponseComplete(Message):
         chat_id: int | None
         message: ChatMessage
         chatbox: Chatbox
 
     @dataclass
-    class FirstMessageSent(Message):
-        chat_data: ChatData
+    class AgentResponseFailed(Message):
+        """Sent when the agent fails to respond e.g. cant connect.
+        Can be used to reset UI state."""
+
+        last_message: ChatMessage
 
     @dataclass
-    class UserMessageSubmitted(Message):
-        chat_id: int
-        message: ChatMessage
+    class FirstMessageSent(Message):
+        chat_data: ChatData
 
     def compose(self) -> ComposeResult:
         yield ChatHeader(chat=self.chat_data, model=self.model)
 
         with VerticalScroll(id="chat-container") as vertical_scroll:
             vertical_scroll.can_focus = False
 
-        yield PromptInput(id="prompt")
+        yield ChatPromptInput(id="prompt")
         yield AgentIsTyping()
 
     async def on_mount(self, _: events.Mount) -> None:
         """
         When the component is mounted, we need to check if there is a new chat to start
         """
         await self.load_chat(self.chat_data)
@@ -115,82 +117,92 @@
         return len(self.chat_data.messages) == 1  # Contains system message at first.
 
     def scroll_to_latest_message(self):
         container = self.chat_container
         container.refresh()
         container.scroll_end(animate=False, force=True)
 
-    def key_d(self):
-        print(self.chat_container.scroll_y)
-        print(self.chat_container.max_scroll_y)
+    @on(AgentResponseFailed)
+    def restore_state_on_agent_failure(self, event: Chat.AgentResponseFailed) -> None:
+        original_prompt = event.last_message.message.get("content", "")
+        if isinstance(original_prompt, str):
+            self.query_one(ChatPromptInput).text = original_prompt
 
     async def new_user_message(self, content: str) -> None:
         log.debug(f"User message submitted in chat {self.chat_data.id!r}: {content!r}")
+
         now_utc = datetime.datetime.now(datetime.UTC)
         user_message: ChatCompletionUserMessageParam = {
             "content": content,
             "role": "user",
         }
-        user_chat_message = ChatMessage(
-            user_message, now_utc, self.chat_data.model_name
-        )
-        self.chat_data.messages.append(user_chat_message)
-        await ChatsManager.add_message_to_chat(
-            chat_id=self.chat_data.id, message=user_chat_message
-        )
 
-        self.post_message(
-            Chat.UserMessageSubmitted(
-                chat_id=self.chat_data.id, message=user_chat_message
-            )
-        )
-        user_message_chatbox = Chatbox(user_chat_message, self.chat_data.model_name)
+        user_chat_message = ChatMessage(user_message, now_utc, self.chat_data.model)
+        self.chat_data.messages.append(user_chat_message)
+        user_message_chatbox = Chatbox(user_chat_message, self.chat_data.model)
 
         assert (
             self.chat_container is not None
         ), "Textual has mounted container at this point in the lifecycle."
 
         await self.chat_container.mount(user_message_chatbox)
         self.scroll_to_latest_message()
+
+        await ChatsManager.add_message_to_chat(
+            chat_id=self.chat_data.id, message=user_chat_message
+        )
+
         self.stream_agent_response()
 
     @work
     async def stream_agent_response(self) -> None:
-        log.debug(
-            f"Creating streaming response with model {self.chat_data.model_name!r}"
-        )
-        model: EliaChatModel = get_model_by_name(
-            self.chat_data.model_name, self.elia.launch_config
-        )
+        model = self.chat_data.model
+        log.debug(f"Creating streaming response with model {model.name!r}")
 
+        import litellm
         from litellm import ModelResponse, acompletion
         from litellm.utils import trim_messages
 
         raw_messages = [message.message for message in self.chat_data.messages]
+
         messages: list[ChatCompletionUserMessageParam] = trim_messages(
             raw_messages, model.name
         )  # type: ignore
-        response = await acompletion(
-            messages=messages,
-            stream=True,
-            model=model.name,
-            temperature=model.temperature,
-            max_retries=model.max_retries,
-        )
+
+        litellm.organization = model.organization
+        try:
+            response = await acompletion(
+                messages=messages,
+                stream=True,
+                model=model.name,
+                temperature=model.temperature,
+                max_retries=model.max_retries,
+                api_key=model.api_key.get_secret_value() if model.api_key else None,
+                api_base=model.api_base.unicode_string() if model.api_base else None,
+            )
+        except Exception as exception:
+            self.app.notify(
+                f"{exception}",
+                title="Error",
+                severity="error",
+                timeout=constants.ERROR_NOTIFY_TIMEOUT_SECS,
+            )
+            self.post_message(self.AgentResponseFailed(self.chat_data.messages[-1]))
+            return
+
         ai_message: ChatCompletionAssistantMessageParam = {
             "content": "",
             "role": "assistant",
         }
         now = datetime.datetime.now(datetime.UTC)
-        message = ChatMessage(message=ai_message, model=model.name, timestamp=now)
+        message = ChatMessage(message=ai_message, model=model, timestamp=now)
 
-        assert self.chat_data.model_name is not None
         response_chatbox = Chatbox(
             message=message,
-            model_name=self.chat_data.model_name,
+            model=self.chat_data.model,
             classes="response-in-progress",
         )
         assert (
             self.chat_container is not None
         ), "Textual has mounted container at this point in the lifecycle."
 
         try:
@@ -217,16 +229,17 @@
                 chunk_count += 1
         except Exception:
             self.notify(
                 "There was a problem using this model. "
                 "Please check your configuration file.",
                 title="Error",
                 severity="error",
-                timeout=15,
+                timeout=constants.ERROR_NOTIFY_TIMEOUT_SECS,
             )
+            self.post_message(self.AgentResponseFailed(self.chat_data.messages[-1]))
         else:
             self.post_message(
                 self.AgentResponseComplete(
                     chat_id=self.chat_data.id,
                     message=response_chatbox.message,
                     chatbox=response_chatbox,
                 )
@@ -242,15 +255,14 @@
     @on(PromptInput.PromptSubmitted)
     async def user_chat_message_submitted(
         self, event: PromptInput.PromptSubmitted
     ) -> None:
         if self.allow_input_submit is True:
             user_message = event.text
             await self.new_user_message(user_message)
-            event.prompt_input.clear()
 
     @on(PromptInput.CursorEscapingTop)
     async def on_cursor_up_from_prompt(self) -> None:
         self.focus_latest_message()
 
     def get_latest_chatbox(self) -> Chatbox:
         return self.query(Chatbox).last()
@@ -278,25 +290,24 @@
         if self.chat_container:
             self.chat_container.scroll_down()
 
     async def action_details(self) -> None:
         await self.app.push_screen(ChatDetails(self.chat_data))
 
     async def load_chat(self, chat_data: ChatData) -> None:
-        assert self.chat_container is not None
         chatboxes = [
-            Chatbox(chat_message, self.chat_data.model_name)
-            for chat_message in self.chat_data.non_system_messages
+            Chatbox(chat_message, chat_data.model)
+            for chat_message in chat_data.non_system_messages
         ]
         await self.chat_container.mount_all(chatboxes)
         self.chat_container.scroll_end(animate=False, force=True)
         chat_header = self.query_one(ChatHeader)
         chat_header.update_header(
             chat=chat_data,
-            model=get_model_by_name(chat_data.model_name, self.elia.launch_config),
+            model=chat_data.model,
         )
 
         # If the last message didn't receive a response, try again.
         messages = chat_data.messages
         if messages and messages[-1].message["role"] == "user":
             self.stream_agent_response()
```

### Comparing `elia_chat-1.0.3/elia_chat/widgets/chat_header.py` & `elia_chat-1.1.0/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/elia_chat/widgets/chat_list.py` & `elia_chat-1.1.0/elia_chat/widgets/chat_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 from textual.binding import Binding
 from textual.message import Message
 from textual.widgets import OptionList
 from textual.widgets.option_list import Option
 
 from elia_chat.chats_manager import ChatsManager
 from elia_chat.config import LaunchConfig
-from elia_chat.models import ChatData, get_model_by_name
+from elia_chat.models import ChatData
 
 
 @dataclass
 class ChatListItemRenderable:
     chat: ChatData
     config: LaunchConfig
 
     def __rich_console__(
         self, console: Console, options: ConsoleOptions
     ) -> RenderResult:
         now = datetime.datetime.now(datetime.UTC)
         delta = now - self.chat.update_time
         time_ago = humanize.naturaltime(delta)
         time_ago_text = Text(time_ago, style="dim i")
-        model = get_model_by_name(self.chat.model_name, self.config)
+        model = self.chat.model
         subtitle = f"[dim]{escape(model.display_name or model.name)}"
         if model.provider:
             subtitle += f" [i]by[/] {escape(model.provider)}"
         model_text = Text.from_markup(subtitle)
         title = self.chat.title or self.chat.short_preview.replace("\n", " ")
         yield Padding(
             Text.assemble(title, "\n", model_text, "\n", time_ago_text),
@@ -52,14 +52,17 @@
         super().__init__(ChatListItemRenderable(chat, config))
         self.chat = chat
         self.config = config
 
 
 class ChatList(OptionList):
     BINDINGS = [
+        Binding(
+            "escape", "screen.focus('home-prompt')", "Focus prompt", key_display="esc"
+        ),
         Binding("j,down", "cursor_down", "Down", show=False),
         Binding("k,up", "cursor_up", "Up", show=False),
         Binding("G,end", "last", "Last", show=False),
         Binding("l,enter", "select", "Select", show=False),
         Binding("g,home", "first", "First", show=False),
         Binding("pagedown", "page_down", "Page Down", show=False),
         Binding("pageup", "page_up", "Page Up", show=False),
```

### Comparing `elia_chat-1.0.3/elia_chat/widgets/chat_options.py` & `elia_chat-1.1.0/elia_chat/widgets/chat_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,18 @@
             classes=classes,
             disabled=disabled,
         )
         self.model = model
 
 
 class OptionsModal(ModalScreen[RuntimeConfig]):
-    BINDINGS = [Binding("escape", "app.pop_screen", "Close options", key_display="esc")]
+    BINDINGS = [
+        Binding("q", "app.quit", "Quit", show=False),
+        Binding("escape", "app.pop_screen", "Close options", key_display="esc"),
+    ]
 
     def __init__(
         self,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
     ) -> None:
@@ -66,17 +69,22 @@
                 selected_model = self.runtime_config.selected_model
                 models_rs.border_title = "Available Models"
                 for model in self.elia.launch_config.all_models:
                     label = f"[dim]{escape(model.display_name or model.name)}"
                     provider = model.provider
                     if provider:
                         label += f" [i]by[/] {provider}"
+
+                    ids_defined = selected_model.id and model.id
+                    same_id = ids_defined and selected_model.id == model.id
+                    same_name = selected_model.name == model.name
+                    is_selected = same_id or same_name
                     yield ModelRadioButton(
                         model=model,
-                        value=selected_model == model.name,
+                        value=is_selected,
                         label=label,
                     )
             system_prompt_ta = TextArea(
                 self.runtime_config.system_prompt, id="system-prompt-ta"
             )
             system_prompt_ta.border_title = "System Message"
             yield system_prompt_ta
@@ -101,30 +109,33 @@
         system_prompt_ta = self.query_one("#system-prompt-ta", TextArea)
         selected_model_rs = self.query_one("#available-models", RadioSet)
         if selected_model_rs.pressed_button is None:
             selected_model_rs._selected = 0
             assert selected_model_rs.pressed_button is not None
 
         model_button = cast(ModelRadioButton, selected_model_rs.pressed_button)
+        model = model_button.model
         self.elia.runtime_config = self.elia.runtime_config.model_copy(
             update={
                 "system_prompt": system_prompt_ta.text,
-                "selected_model": model_button.model.name,
+                "selected_model": model,
             }
         )
 
         self.apply_overridden_subtitles(system_prompt_ta, selected_model_rs)
         self.refresh()
 
     def apply_overridden_subtitles(
         self, system_prompt_ta: TextArea, selected_model_rs: RadioSet
     ) -> None:
         if (
             self.elia.launch_config.default_model
-            != self.elia.runtime_config.selected_model
+            != self.elia.runtime_config.selected_model.id
+            and self.elia.launch_config.default_model
+            != self.elia.runtime_config.selected_model.name
         ):
             selected_model_rs.border_subtitle = "overrides config"
         else:
             selected_model_rs.border_subtitle = ""
 
         if system_prompt_ta.text != self.elia.launch_config.system_prompt:
             system_prompt_ta.border_subtitle = "overrides config"
```

### Comparing `elia_chat-1.0.3/elia_chat/widgets/prompt_input.py` & `elia_chat-1.1.0/elia_chat/widgets/prompt_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,8 +61,9 @@
         #  I think this may be a Textual bug.
         #  The refresh below should not be required.
         self.parent.refresh()
 
     def action_submit_prompt(self) -> None:
         if self.submit_ready:
             message = self.PromptSubmitted(self.text, prompt_input=self)
+            self.clear()
             self.post_message(message)
```

### Comparing `elia_chat-1.0.3/elia_chat/widgets/token_analysis.py` & `elia_chat-1.1.0/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/.gitignore` & `elia_chat-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.3/README.md` & `elia_chat-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -45,32 +45,52 @@
 
 The location of the configuration file is noted at the bottom of
 the options window (`ctrl+o`).
 
 The example file below shows the available options, as well as examples of how to add new models.
 
 ```toml
-# the model that is selected by default on launch
-default_model = "gpt-3.5-turbo"
+# the *ID* for the model that is selected by default on launch
+# to use one of the default builtin OpenAI/anthropic models, prefix
+# the model name with `elia-`.
+default_model = "elia-gpt-3.5-turbo"
 # the system prompt on launch
 system_prompt = "You are a helpful assistant who talks like a pirate."
 
 # example of adding local llama3 support
 # only the `name` field is required here.
 [[models]]
 name = "ollama/llama3"
 
+# example of a model running on a local server, e.g. LocalAI
+[[models]]
+name = "openai/some-model"
+api_base = "http://localhost:8080/v1/chat/completions"
+api_key = "api-key-if-required"
+
 # example of add a groq model, showing some other fields
 [[models]]
 name = "groq/llama2-70b-4096"
 display_name = "Llama 2 70B"  # appears in UI
 provider = "Groq"  # appears in UI
 temperature = 1.0  # high temp = high variation in output
 max_retries = 0  # number of retries on failed request
-```
+
+# example of multiple instances of one model, e.g. you might
+# have a 'work' OpenAI org and a 'personal' org.
+[[models]]
+id = "work-gpt-3.5-turbo"
+name = "gpt-3.5-turbo"
+display_name = "GPT 3.5 Turbo (Work)"
+
+[[models]]
+id = "personal-gpt-3.5-turbo"
+name = "gpt-3.5-turbo"
+display_name = "GPT 3.5 Turbo (Personal)"
+
 
 ### Import from ChatGPT
 
 Export your conversations to a JSON file using the ChatGPT UI, then import them using the `import` command.
 
 ```bash
 elia import 'path/to/conversations.json'
```

### Comparing `elia_chat-1.0.3/pyproject.toml` & `elia_chat-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elia_chat"
-version = "1.0.3"
+version = "1.1.0"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
     "textual[syntax]==0.58.1",
     "sqlmodel>=0.0.9",
```

### Comparing `elia_chat-1.0.3/PKG-INFO` & `elia_chat-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.0.3
+Version: 1.1.0
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: greenlet>=3.0.3
@@ -63,32 +63,52 @@
 
 The location of the configuration file is noted at the bottom of
 the options window (`ctrl+o`).
 
 The example file below shows the available options, as well as examples of how to add new models.
 
 ```toml
-# the model that is selected by default on launch
-default_model = "gpt-3.5-turbo"
+# the *ID* for the model that is selected by default on launch
+# to use one of the default builtin OpenAI/anthropic models, prefix
+# the model name with `elia-`.
+default_model = "elia-gpt-3.5-turbo"
 # the system prompt on launch
 system_prompt = "You are a helpful assistant who talks like a pirate."
 
 # example of adding local llama3 support
 # only the `name` field is required here.
 [[models]]
 name = "ollama/llama3"
 
+# example of a model running on a local server, e.g. LocalAI
+[[models]]
+name = "openai/some-model"
+api_base = "http://localhost:8080/v1/chat/completions"
+api_key = "api-key-if-required"
+
 # example of add a groq model, showing some other fields
 [[models]]
 name = "groq/llama2-70b-4096"
 display_name = "Llama 2 70B"  # appears in UI
 provider = "Groq"  # appears in UI
 temperature = 1.0  # high temp = high variation in output
 max_retries = 0  # number of retries on failed request
-```
+
+# example of multiple instances of one model, e.g. you might
+# have a 'work' OpenAI org and a 'personal' org.
+[[models]]
+id = "work-gpt-3.5-turbo"
+name = "gpt-3.5-turbo"
+display_name = "GPT 3.5 Turbo (Work)"
+
+[[models]]
+id = "personal-gpt-3.5-turbo"
+name = "gpt-3.5-turbo"
+display_name = "GPT 3.5 Turbo (Personal)"
+
 
 ### Import from ChatGPT
 
 Export your conversations to a JSON file using the ChatGPT UI, then import them using the `import` command.
 
 ```bash
 elia import 'path/to/conversations.json'
```

