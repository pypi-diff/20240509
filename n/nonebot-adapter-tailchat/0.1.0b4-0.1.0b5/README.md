# Comparing `tmp/nonebot_adapter_tailchat-0.1.0b4.tar.gz` & `tmp/nonebot_adapter_tailchat-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b4.tar", max compression
+gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b5.tar", max compression
```

## Comparing `nonebot_adapter_tailchat-0.1.0b4.tar` & `nonebot_adapter_tailchat-0.1.0b5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11335 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/LICENSE
--rw-r--r--   0        0        0     1488 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/README.md
--rw-r--r--   0        0        0      260 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/__init__.py
--rw-r--r--   0        0        0     6874 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/adapter.py
--rw-r--r--   0        0        0    21563 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/api.py
--rw-r--r--   0        0        0     8081 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bbcode.py
--rw-r--r--   0        0        0     3759 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bot.py
--rw-r--r--   0        0        0      675 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/config.py
--rw-r--r--   0        0        0       26 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/const.py
--rw-r--r--   0        0        0     6135 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/event.py
--rw-r--r--   0        0        0      761 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/exception.py
--rw-r--r--   0        0        0    11184 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/message.py
--rw-r--r--   0        0        0     4505 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/model.py
--rw-r--r--   0        0        0      374 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/permission.py
--rw-r--r--   0        0        0      203 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/rule.py
--rw-r--r--   0        0        0     2103 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/util.py
--rw-r--r--   0        0        0     1232 2024-05-07 14:52:26.131946 nonebot_adapter_tailchat-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     2272 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/LICENSE
+-rw-r--r--   0        0        0     1488 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/README.md
+-rw-r--r--   0        0        0      260 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/__init__.py
+-rw-r--r--   0        0        0     7340 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/adapter.py
+-rw-r--r--   0        0        0    23978 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/api.py
+-rw-r--r--   0        0        0     8081 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/bbcode.py
+-rw-r--r--   0        0        0     4454 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/bot.py
+-rw-r--r--   0        0        0      675 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/config.py
+-rw-r--r--   0        0        0      158 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/const.py
+-rw-r--r--   0        0        0     7752 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/event.py
+-rw-r--r--   0        0        0     1498 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/exception.py
+-rw-r--r--   0        0        0    11198 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/message.py
+-rw-r--r--   0        0        0     5266 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/model.py
+-rw-r--r--   0        0        0      374 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/permission.py
+-rw-r--r--   0        0        0      203 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/rule.py
+-rw-r--r--   0        0        0     2103 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/util.py
+-rw-r--r--   0        0        0     1232 2024-05-08 14:38:07.230515 nonebot_adapter_tailchat-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0     2272 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b5/PKG-INFO
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/LICENSE` & `nonebot_adapter_tailchat-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b4/README.md` & `nonebot_adapter_tailchat-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/adapter.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from nonebot.drivers import Driver
 from nonebot.internal.driver import ContentTypes, HTTPClientMixin, Request, Response
 from typing_extensions import override
 from yarl import URL
 
 from .bot import Bot
 from .config import BotInfo, Config
-from .const import ADAPTER_NAME
-from .event import EVENT_CLASSES, Event
-from .exception import ActionFailed, DisconnectException
+from .const import ADAPTER_NAME, Undefined
+from .event import get_event
+from .exception import ConnectionException, DisconnectException, get_error
 from .message import Message
 from .util import log, retry
 
 
 class Adapter(BaseAdapter):
     @override
     def __init__(self, driver: Driver, **kwargs: Any):
@@ -48,22 +48,22 @@
             if not self.is_http_client_driver:
                 raise RuntimeError("HTTPClientMixin is required when use http")
             self.driver: HTTPClientMixin
             resp = await self.driver.request(
                 Request(
                     "POST",
                     str((URL(bot.url) / "api" if use_api else URL(bot.url)) / api),
-                    json=data,
+                    json={key: value for key, value in data.items() if value != Undefined},
                     headers={"X-Token": bot.base_info.jwt or ""},
                 )
             )
             data = self._loads(resp.content)
             self._handle_http_api(resp, data)
         else:
-            data = await bot.sio.call(api, data)
+            data = await bot.sio.call(api, {key: value for key, value in data.items() if value != Undefined})
             self._handle_socketio_api(data)
         return data.get("data")
 
     async def _setup(self):
         if any(i.useHttp for i in self.adapter_config.bots_info) and not self.is_http_client_driver:
             raise RuntimeError("HTTPClientMixin is required when use http")
         for i in self.adapter_config.bots_info:
@@ -79,17 +79,15 @@
         for task in self.tasks:
             if not task.done():
                 task.cancel()
 
         await gather(*self.tasks, return_exceptions=True)
 
     async def _handle_bot(self, bot_info: BotInfo):
-        first = True
         connected = False
-        added = False
 
         async def _wait():  # 确保断连后打断wait
             nonlocal connected
             while True:
                 if not connected:
                     raise DisconnectException()
                 await sleep(1)
@@ -100,34 +98,30 @@
 
         bot = Bot(self, bot_info.appId, bot_info)
         bot.sio.on("*", partial(self._handle_event, bot))
         bot.sio.on("disconnect", _check)
         while True:
             try:
                 await wait_for(bot.login(bot.base_info.jwt), self.adapter_config.time_out)
-                if first:
-                    await wait_for(self._connect_bot(bot, first), self.adapter_config.time_out)
-                    first = False
+                await wait_for(self._connect_bot(bot), self.adapter_config.time_out)
                 await bot.update_info(bot.base_info.jwt)
-                if not added:
-                    self._bot_connect(bot)
-                    added = True
+                self._bot_connect(bot)
                 connected = True
                 await gather(bot.sio.wait(), _wait())
             except DisconnectException:
                 log.warning(f"Bot {escape_tag(str(bot))} socketio connection closed")
             except AsyncTimeoutError:
                 log.warning(f"Bot {escape_tag(str(bot))} connection timeout")
+            except ConnectionException as e:
+                log.error(f"Error when chat.converse.findAndJoinRoom: {repr(e)}")
             except Exception as e:
                 log.error(f"Error when _handle_bot: {repr(e)}")
                 print_exc()
             connected = False
-            if added:
-                self._bot_disconnect(bot)
-                added = False
+            self._bot_disconnect(bot)
             log.debug(f"Bot {escape_tag(str(bot))} will reconnect in {self.adapter_config.reconnect_interval} seconds")
             await sleep(self.adapter_config.reconnect_interval)
 
     def _bot_connect(self, bot: Bot):
         try:
             self.bot_connect(bot)
         except Exception as e:
@@ -136,41 +130,54 @@
     def _bot_disconnect(self, bot: Bot):
         try:
             self.bot_disconnect(bot)
         except Exception as e:
             log.trace(f"Error when bot_disconnect: {repr(e)}")
 
     @staticmethod
-    async def _connect_bot(bot: Bot, first: bool = True):
-        if first:
-            log.debug(f"try to connect bot {escape_tag(str(bot))}")
+    async def _connect_bot(bot: Bot):
+        log.debug(f"try to connect bot {escape_tag(str(bot))}")
+        try:
             await bot.connect()
-        else:
-            log.info(f"try to reconnect bot {escape_tag(str(bot))}")
-        log.success(f"<y>Bot {escape_tag(str(bot))}</y> connected")
-        await bot.sio.emit("chat.converse.findAndJoinRoom")
+        except Exception as e:
+            log.trace(f"Error when bot.connect: {repr(e)}")
+        try:
+            await bot.sio.emit("chat.converse.findAndJoinRoom")
+            log.success(f"<y>Bot {escape_tag(str(bot))}</y> connected")
+        except Exception:
+            raise ConnectionException(f"Bot {str(bot)} join room fail")
 
     @staticmethod
     async def _handle_event(bot: Bot, event: str, data: dict, _: Optional[any] = None):
-        model = EVENT_CLASSES.get(event)
+        model = get_event(event)
         log.trace(f"Event: {event}, MatchModel: {model}, Data: {data}")
-        data["event_name"] = event
-        data["self_id"] = bot.self_id
-        await bot.handle_event((model or Event).model_validate(data))
+        data["event_name"] = data.get("event_name", event)
+        data["self_id"] = data.get("self_id", bot.self_id)
+        await bot.handle_event(model.model_validate(data))
 
     @staticmethod
     def _loads(data: ContentTypes) -> Any:
         try:
             return json.loads(data)
         except json.JSONDecodeError:
             log.error("Error when loads data", escape_tag(data.decode() if isinstance(data, bytes) else str(data)))
             raise
 
     @staticmethod
     def _handle_http_api(resp: Response, data: dict):
         if resp.status_code != 200:
-            raise ActionFailed(message=f'{data.get("name", "unknown")}:{data.get("message")}', code=resp.status_code)
+            name = data.get("name")
+            code = data.get("code")
+            message = data.get("message")
+            error = get_error(data.get("name"))
+            name = name or "unknown"
+            raise error(name=name, message=f"{name}:{message}", code=code)
 
     @staticmethod
     def _handle_socketio_api(data: dict):
         if not data.get("result", True):
-            raise ActionFailed(message=f'{data.get("name", "unknown")}:{data.get("message")}', code=data.get("code"))
+            name = data.get("name")
+            code = data.get("code")
+            message = data.get("message")
+            error = get_error(data.get("name"))
+            name = name or "unknown"
+            raise error(name=name, message=f"{name}:{message}", code=code)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/api.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from abc import ABC
-from typing import Any, Literal, Optional, Union
+from typing import Any, Literal, Union
 
 from nonebot.adapters import Bot as BaseBot
 from pydantic import TypeAdapter
 
+from .const import Optional, Undefined
 from .message import Message
 from .model import (
     Ack,
+    AddFriendRequestRet,
+    BaseGroupInfo,
     ClientConfig,
     ConverseInfo,
     FileInfo,
+    GroupAndPanelIds,
     GroupInfo,
     Health,
     InviteCodeInfo,
     LastMessages,
     MessageRet,
     Panel,
+    TemporaryUserInfo,
     TokenInfo,
     UserInfo,
     Whoami,
 )
 
 
 class API(BaseBot, ABC):
@@ -40,32 +45,34 @@
         return TypeAdapter(Whoami).validate_python(await self.call_api("user.whoami"))
 
     async def getFile(self, *, objectName: str):
         """获取文件url (但是参数不知道填啥)"""
         return await self.call_api("file.get", objectName=objectName)
 
     async def ackInbox(self, *, inboxItemIds: list[str]):
+        """标记消息为已读"""
         return await self.call_api("chat.inbox.ack", inboxItemIds=inboxItemIds)
 
-    async def allInbox(self):
-        return await self.call_api("chat.inbox.all")
+    async def allInbox(self) -> Message:
+        """获取全部收件箱内的消息"""
+        return TypeAdapter(Message).validate_python(await self.call_api("chat.inbox.all"))
 
     async def isMember(self, *, groupId: str):
         """是否为指定群的成员"""
         return await self.call_api("group.isMember", groupId=groupId)
 
     async def register(
         self,
         *,
         password: str,
-        email: Optional[str] = None,
-        avatar: Optional[str] = None,
-        emailOTP: Optional[str] = None,
-        nickname: Optional[str] = None,
-        username: Optional[str] = None,
+        email: Optional[str] = Undefined,
+        avatar: Optional[str] = Undefined,
+        emailOTP: Optional[str] = Undefined,
+        nickname: Optional[str] = Undefined,
+        username: Optional[str] = Undefined,
     ):
         return await self.call_api(
             "user.register",
             email=email,
             avatar=avatar,
             emailOTP=emailOTP,
             nickname=nickname,
@@ -81,39 +88,48 @@
 
     async def upload(self, *, file: bytes) -> FileInfo:
         """上传文件"""
         return TypeAdapter(FileInfo).validate_python(
             await self.call_api("upload", file=file, use_api_=False, use_http_=True, use_sio_=False)
         )
 
-    async def authToken(self, *, appId: str, token: str, capability: Optional[list[str]] = None):
+    async def authToken(self, *, appId: str, token: str, capability: Optional[list[str]] = Undefined):
         """验证token"""
         return await self.call_api("openapi.app.authToken", appId=appId, token=token, capability=capability)
 
     async def createApp(self, *, appDesc: str, appIcon: str, appName: str):
         return await self.call_api("openapi.app.create", appDesc=appDesc, appIcon=appIcon, appName=appName)
 
     async def deleteApp(self, *, appId: str):
         return await self.call_api("openapi.app.delete", appId=appId)
 
-    async def loginUser(self, *, password: str, email: Optional[str] = None, username: Optional[str] = None):
-        return await self.call_api("user.login", email=email, password=password, username=username)
+    async def loginUser(
+        self, *, password: str, email: Optional[str] = Undefined, username: Optional[str] = Undefined
+    ) -> TokenInfo:
+        """标准登录API"""
+        return TypeAdapter(TokenInfo).validate_python(
+            await self.call_api("user.login", email=email, password=password, username=username)
+        )
 
     async def quitGroup(self, *, groupId: str):
         """退群"""
         return await self.call_api("group.quitGroup", groupId=groupId)
 
     async def updateAck(self, *, converseId: str, lastMessageId: str):
+        """标记已读消息(应该)"""
         return await self.call_api("chat.ack.update", converseId=converseId, lastMessageId=lastMessageId)
 
     async def addBotUser(self, *, appId: str, groupId: str):
         return await self.call_api("openapi.integration.addBotUser", appId=appId, groupId=groupId)
 
-    async def addRequest(self, *, to: str, message: Optional[str] = None):
-        return await self.call_api("friend.request.add", to=to, message=message)
+    async def addRequest(self, *, to: str, message: Optional[str] = Undefined) -> AddFriendRequestRet:
+        """发送好友申请(message好像没用, 请求处理界面看不到message).不存在的id也能发送成功.不符合格式的id会报错."""
+        return TypeAdapter(AddFriendRequestRet).validate_python(
+            await self.call_api("friend.request.add", to=to, message=message)
+        )
 
     async def allRelated(self):
         return await self.call_api("friend.request.allRelated")
 
     async def clearInbox(self):
         return await self.call_api("chat.inbox.clear")
 
@@ -134,28 +150,29 @@
     async def createGroup(self, *, name: str, panels: list[Union[Panel, dict]]) -> GroupInfo:
         """创建群组"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.createGroup", name=name, panels=panels)
         )
 
     async def denyRequest(self, *, requestId: str):
+        """拒绝好友请求"""
         return await self.call_api("friend.request.deny", requestId=requestId)
 
     async def getUserInfo(self, *, userId: str) -> UserInfo:
         """获取用户信息"""
         return TypeAdapter(UserInfo).validate_python(await self.call_api("user.getUserInfo", userId=userId))
 
     async def sendMessage(
         self,
         *,
         content: str,
         converseId: str,
-        meta: Optional[dict] = None,
-        plain: Optional[str] = None,
-        groupId: Optional[str] = None,
+        meta: Optional[dict] = Undefined,
+        plain: Optional[str] = Undefined,
+        groupId: Optional[str] = Undefined,
     ) -> MessageRet:
         """发送消息"""
         return TypeAdapter(MessageRet).validate_python(
             await self.call_api(
                 "chat.message.sendMessage",
                 meta=meta,
                 plain=plain,
@@ -180,47 +197,56 @@
         return await self.call_api("group.extra.getGroupData", name=name, groupId=groupId)
 
     async def getPanelData(self, *, name: str, groupId: str, panelId: str):
         """获取面板数据"""
         return await self.call_api("group.extra.getPanelData", name=name, groupId=groupId, panelId=panelId)
 
     async def isGroupOwner(self, *, groupId: str):
+        """是否为创建者"""
         return await self.call_api("group.isGroupOwner", groupId=groupId)
 
     async def listRegistry(self):
         return await self.call_api("plugin.registry.list")
 
     async def removeFriend(self, *, friendUserId: str):
+        """删除好友"""
         return await self.call_api("friend.removeFriend", friendUserId=friendUserId)
 
     async def resolveToken(self, *, token: str) -> TokenInfo:
         """获取token信息"""
         return TypeAdapter(TokenInfo).validate_python(await self.call_api("user.resolveToken", token=token))
 
     async def acceptRequest(self, *, requestId: str):
+        """接受好友请求"""
         return await self.call_api("friend.request.accept", requestId=requestId)
 
     async def cancelRequest(self, *, requestId: str):
+        """撤销申请好友请求. 填不存在的requestId会报错, 不符合格式的也会报错"""
         return await self.call_api("friend.request.cancel", requestId=requestId)
 
     async def checkIsFriend(self, *, targetId: str):
+        """判断是否为好友"""
         return await self.call_api("friend.checkIsFriend", targetId=targetId)
 
     async def deleteMessage(self, *, messageId: str):
+        """删除消息"""
         return await self.call_api("chat.message.deleteMessage", messageId=messageId)
 
     async def gatewayHealth(self) -> Health:
         """获取网关健康状态"""
         return TypeAdapter(Health).validate_python(await self.call_api("gateway.health"))
 
     async def getAllFriends(self):
+        """获取全部好友的ID
+        [{'id': '***'}]"""
         return await self.call_api("friend.getAllFriends")
 
-    async def getUserGroups(self):
-        return await self.call_api("group.getUserGroups")
+    async def getUserGroups(self) -> list[GroupInfo]:
+        """获取用户的群组"""
+        return TypeAdapter(list[GroupInfo]).validate_python(await self.call_api("group.getUserGroups"))
 
     async def recallMessage(self, *, messageId: str) -> Message:
         """撤回消息, 大于15分钟的消息无法撤回, 会报错"""
         return TypeAdapter(Message).validate_python(
             await self.call_api("chat.message.recallMessage", messageId=messageId)
         )
 
@@ -230,36 +256,39 @@
     async def saveGroupData(self, *, data: str, name: str, groupId: str):
         return await self.call_api("group.extra.saveGroupData", data=data, name=name, groupId=groupId)
 
     async def savePanelData(self, *, data: str, name: str, groupId: str, panelId: str):
         """保存面板数据"""
         return await self.call_api("group.extra.savePanelData", data=data, name=name, groupId=groupId, panelId=panelId)
 
-    async def searchMessage(self, *, text: str, converseId: str, groupId: Optional[str] = None) -> list[Message]:
+    async def searchMessage(self, *, text: str, converseId: str, groupId: Optional[str] = Undefined) -> list[Message]:
         """搜索消息"""
         return TypeAdapter(list[Message]).validate_python(
             await self.call_api("chat.message.searchMessage", text=text, groupId=groupId, converseId=converseId)
         )
 
     async def setAppBotInfo(self, *, appId: str, fieldName: str, fieldValue: Any):
         return await self.call_api("openapi.app.setAppBotInfo", appId=appId, fieldName=fieldName, fieldValue=fieldValue)
 
     async def forgetPassword(self, *, email: str):
         return await self.call_api("user.forgetPassword", email=email)
 
-    async def getAllConverse(self):
-        return await self.call_api("user.dmlist.getAllConverse")
+    async def getAllConverse(self) -> list[str]:
+        """获取所有会话"""
+        return TypeAdapter(list[str]).validate_python(await self.call_api("user.dmlist.getAllConverse"))
 
     async def getPermissions(self, *, groupId: str):
         return await self.call_api("group.getPermissions", groupId=groupId)
 
     async def modifyPassword(self, *, newPassword: str, oldPassword: str):
+        """修改密码(好像没啥用)"""
         return await self.call_api("user.modifyPassword", newPassword=newPassword, oldPassword=oldPassword)
 
     async def removeConverse(self, *, converseId: str):
+        """删除会话\n{"modifiedCount":1}"""
         return await self.call_api("user.dmlist.removeConverse", converseId=converseId)
 
     async def removeReaction(self, *, emoji: str, messageId: str):
         """删除消息表情"""
         return await self.call_api("chat.message.removeReaction", emoji=emoji, messageId=messageId)
 
     async def checkTokenValid(self, *, token: str):
@@ -278,22 +307,22 @@
     async def deleteGroupRole(self, *, roleId: str, groupId: str) -> GroupInfo:
         """删除群用户组"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.deleteGroupRole", roleId=roleId, groupId=groupId)
         )
 
     async def editGroupInvite(
-        self, *, code: str, groupId: str, expireAt: Optional[int] = None, usageLimit: Optional[int] = None
+        self, *, code: str, groupId: str, expireAt: Optional[int] = Undefined, usageLimit: Optional[int] = Undefined
     ):
         """编辑群组邀请码"""
         return await self.call_api(
             "group.invite.editGroupInvite", code=code, groupId=groupId, expireAt=expireAt, usageLimit=usageLimit
         )
 
-    async def ensurePluginBot(self, *, botId: str, nickname: str, avatar: Optional[str] = None):
+    async def ensurePluginBot(self, *, botId: str, nickname: str, avatar: Optional[str] = Undefined):
         return await self.call_api("user.ensurePluginBot", botId=botId, avatar=avatar, nickname=nickname)
 
     async def findAndJoinRoom(self):
         return await self.call_api("chat.converse.findAndJoinRoom")
 
     async def getUserInfoList(self, *, userIds: list[str]) -> list[UserInfo]:
         """获取多个用户信息"""
@@ -315,45 +344,54 @@
     async def setUserSettings(self, *, settings: dict):
         """修改用户设置"""
         return await self.call_api("user.setUserSettings", settings=settings)
 
     async def updateUserExtra(self, *, fieldName: str, fieldValue: Any):
         return await self.call_api("user.updateUserExtra", fieldName=fieldName, fieldValue=fieldValue)
 
-    async def updateUserField(self, *, fieldName: str, fieldValue: Any):
-        return await self.call_api("user.updateUserField", fieldName=fieldName, fieldValue=fieldValue)
+    async def updateUserField(self, *, fieldName: str, fieldValue: Any) -> UserInfo:
+        """更改用户信息"""
+        return TypeAdapter(UserInfo).validate_python(
+            await self.call_api("user.updateUserField", fieldName=fieldName, fieldValue=fieldValue)
+        )
 
-    async def createDMConverse(self, *, memberIds: list[str]):
-        return await self.call_api("chat.converse.createDMConverse", memberIds=memberIds)
+    async def createDMConverse(self, *, memberIds: list[str]) -> ConverseInfo:
+        """创建会话"""
+        return TypeAdapter(ConverseInfo).validate_python(
+            await self.call_api("chat.converse.createDMConverse", memberIds=memberIds)
+        )
 
     async def createGroupPanel(
         self,
         *,
         name: str,
         meta: dict,
         type_: int,
         groupId: str,
-        provider: Optional[str] = None,
-        pluginPanelName: Optional[str] = None,
+        provider: Optional[str] = Undefined,
+        pluginPanelName: Optional[str] = Undefined,
     ):
         """创建群组面板"""
         return await self.call_api(
             "group.createGroupPanel",
             meta=meta,
             name=name,
             type=type_,
             groupId=groupId,
             provider=provider,
             pluginPanelName=pluginPanelName,
         )
 
-    async def deleteGroupPanel(self, *, groupId: str, panelId: str):
-        return await self.call_api("group.deleteGroupPanel", groupId=groupId, panelId=panelId)
+    async def deleteGroupPanel(self, *, groupId: str, panelId: str) -> GroupInfo:
+        """删除群组面板"""
+        return TypeAdapter(GroupInfo).validate_python(
+            await self.call_api("group.deleteGroupPanel", groupId=groupId, panelId=panelId)
+        )
 
-    async def ensureOpenapiBot(self, *, botId: str, nickname: str, avatar: Optional[str] = None):
+    async def ensureOpenapiBot(self, *, botId: str, nickname: str, avatar: Optional[str] = Undefined):
         return await self.call_api("user.ensureOpenapiBot", botId=botId, avatar=avatar, nickname=nickname)
 
     async def findConverseInfo(self, *, converseId: str) -> ConverseInfo:
         """获取会话信息"""
         return TypeAdapter(ConverseInfo).validate_python(
             await self.call_api("chat.converse.findConverseInfo", converseId=converseId)
         )
@@ -369,19 +407,19 @@
     async def modifyGroupPanel(
         self,
         *,
         name: str,
         type_: int,
         groupId: str,
         panelId: str,
-        meta: Optional[dict] = None,
-        provider: Optional[str] = None,
-        permissionMap: Optional[dict] = None,
-        pluginPanelName: Optional[str] = None,
-        fallbackPermissions: Optional[list[str]] = None,
+        meta: Optional[dict] = Undefined,
+        provider: Optional[str] = Undefined,
+        permissionMap: Optional[dict] = Undefined,
+        pluginPanelName: Optional[str] = Undefined,
+        fallbackPermissions: Optional[list[str]] = Undefined,
     ):
         return await self.call_api(
             "group.modifyGroupPanel",
             meta=meta,
             name=name,
             type=type_,
             groupId=groupId,
@@ -404,30 +442,41 @@
     async def createGroupInvite(self, *, groupId: str, inviteType: Literal["normal", "permanent"]) -> InviteCodeInfo:
         """创建群组邀请码"""
         return TypeAdapter(InviteCodeInfo).validate_python(
             await self.call_api("group.invite.createGroupInvite", groupId=groupId, inviteType=inviteType)
         )
 
     async def deleteGroupMember(self, *, groupId: str, memberId: str):
+        """删除群成员"""
         return await self.call_api("group.deleteGroupMember", groupId=groupId, memberId=memberId)
 
-    async def getGroupBasicInfo(self, *, groupId: str):
-        return await self.call_api("group.getGroupBasicInfo", groupId=groupId)
+    async def getGroupBasicInfo(self, *, groupId: str) -> BaseGroupInfo:
+        """获取群基本消息"""
+        return TypeAdapter(BaseGroupInfo).validate_python(
+            await self.call_api("group.getGroupBasicInfo", groupId=groupId)
+        )
 
     async def setFriendNickname(self, *, nickname: str, targetId: str):
+        """更改好友昵称"""
         return await self.call_api("friend.setFriendNickname", nickname=nickname, targetId=targetId)
 
     async def updateGroupConfig(self, *, groupId: str, configName: str, configValue: Any):
         """更新群组配置"""
         return await self.call_api(
             "group.updateGroupConfig", groupId=groupId, configName=configName, configValue=configValue
         )
 
     async def claimTemporaryUser(
-        self, *, email: str, userId: str, password: str, emailOTP: Optional[str] = None, username: Optional[str] = None
+        self,
+        *,
+        email: str,
+        userId: str,
+        password: str,
+        emailOTP: Optional[str] = Undefined,
+        username: Optional[str] = Undefined,
     ):
         return await self.call_api(
             "user.claimTemporaryUser",
             email=email,
             userId=userId,
             emailOTP=emailOTP,
             password=password,
@@ -445,16 +494,19 @@
     async def verifyEmailWithOTP(self, *, emailOTP: str):
         """验证邮箱"""
         return await self.call_api("user.verifyEmailWithOTP", emailOTP=emailOTP)
 
     async def buildFriendRelation(self, *, user1: str, user2: str):
         return await self.call_api("friend.buildFriendRelation", user1=user1, user2=user2)
 
-    async def createTemporaryUser(self, *, nickname: str):
-        return await self.call_api("user.createTemporaryUser", nickname=nickname)
+    async def createTemporaryUser(self, *, nickname: str) -> TemporaryUserInfo:
+        """创建临时用户"""
+        return TypeAdapter(TemporaryUserInfo).validate_python(
+            await self.call_api("user.createTemporaryUser", nickname=nickname)
+        )
 
     async def updateGroupRoleName(self, *, roleId: str, groupId: str, roleName: str) -> GroupInfo:
         """更新群用户组名称"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.updateGroupRoleName", roleId=roleId, groupId=groupId, roleName=roleName)
         )
 
@@ -478,27 +530,32 @@
         """移除群用户组成员"""
         return await self.call_api("group.removeGroupMemberRoles", roles=roles, groupId=groupId, memberIds=memberIds)
 
     async def appendDMConverseMembers(self, *, converseId: str, memberIds: list[str]):
         return await self.call_api("chat.converse.appendDMConverseMembers", memberIds=memberIds, converseId=converseId)
 
     async def getGroupLobbyConverseId(self, *, groupId: str):
+        """不知道啥作用, 但是返回的是converseId"""
         return await self.call_api("group.getGroupLobbyConverseId", groupId=groupId)
 
-    async def searchUserWithUniqueName(self, *, uniqueName: str):
-        return await self.call_api("user.searchUserWithUniqueName", uniqueName=uniqueName)
+    async def searchUserWithUniqueName(self, *, uniqueName: str) -> Optional[UserInfo]:
+        """根据唯一名搜索用户"""
+        return TypeAdapter(Optional[UserInfo]).validate_python(
+            await self.call_api("user.searchUserWithUniqueName", uniqueName=uniqueName)
+        )
 
     async def fetchConverseLastMessages(self, *, converseIds: list[str]) -> list[LastMessages]:
         """获取多个会话的最后一条消息"""
         return TypeAdapter(list[LastMessages]).validate_python(
             await self.call_api("chat.message.fetchConverseLastMessages", converseIds=converseIds)
         )
 
-    async def getJoinedGroupAndPanelIds(self):
-        return await self.call_api("group.getJoinedGroupAndPanelIds")
+    async def getJoinedGroupAndPanelIds(self) -> GroupAndPanelIds:
+        """获取加入的群组和面板ID"""
+        return TypeAdapter(GroupAndPanelIds).validate_python(await self.call_api("group.getJoinedGroupAndPanelIds"))
 
     async def updateGroupRolePermission(self, *, roleId: str, groupId: str, permissions: list[str]) -> GroupInfo:
         """更新群用户组权限"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api(
                 "group.updateGroupRolePermission", roleId=roleId, groupId=groupId, permissions=permissions
             )
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bbcode.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/bbcode.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bot.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from base64 import urlsafe_b64decode
+from functools import wraps
 from hashlib import md5
 from json import loads
 from time import time
 from typing import TYPE_CHECKING, Optional, Union
 
 from nonebot.message import handle_event
 from pydantic import TypeAdapter
@@ -20,14 +21,24 @@
     TokenInfo,
 )
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
+def _with_update_info(func):
+    @wraps(func)
+    async def wrapper(self: "Bot", *args, **kwargs):
+        _ = await func(self, *args, **kwargs)
+        await self.update_info(self.base_info.jwt)
+        return _
+
+    return wrapper
+
+
 class Bot(API):
     def __str__(self):
         return f"{self.info.nickname}-{self.self_id}" if self.info else self.self_id
 
     async def connect(self):
         return await self.sio.connect(
             url=self.url,
@@ -108,7 +119,17 @@
                 self.base_info.jwt = jwt
                 return
         if self.base_info.appId and self.base_info.appSecret:
             data = await self.loginBot(appId=self.base_info.appId, appSecret=self.base_info.appSecret)
             self.base_info.jwt = data.jwt
             return
         raise ValueError("必须提供jwt或appId和appSecret")
+
+    @_with_update_info
+    async def updateNickname(self, nickname: str):
+        """更新昵称，机器人重登后就失效了"""
+        return await self.updateUserField(fieldName="nickname", fieldValue=nickname)
+
+    @_with_update_info
+    async def updateAvatar(self, avatar: str):
+        """更新头像，机器人重登后就失效了"""
+        return await self.updateUserField(fieldName="avatar", fieldValue=avatar)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/config.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/event.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/event.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from abc import ABC, abstractmethod
-from typing import Literal, Optional, TypeVar, get_args
+from typing import TYPE_CHECKING, Literal, Optional, TypeVar, get_args
 
 from nonebot.adapters import Event as BaseEvent
 from nonebot.compat import model_dump
 from pydantic import Field
+from pydantic_core import PydanticUndefined
 from typing_extensions import override
 
 from .message import Message
 from .model import MemberInfo, MessageMeta, Panel, Payload, Reaction, Replay, datetime
 
+if TYPE_CHECKING:
+    from .bot import Bot
 
-class Event(BaseEvent):
+
+class Event(BaseEvent, ABC):
     event_name: str
-    event_type: str = Field(alias="event_name")
+    event_type: str
+
     self_id: str
 
     @override
     def get_type(self) -> str:
         return self.event_type
 
     @override
@@ -30,76 +35,106 @@
     @override
     def get_session_id(self) -> str:
         raise ValueError("Event has no context!")
 
     def get_user_id(self) -> str:
         raise ValueError("Event has no context!")
 
-    def get_message(self) -> "Message":
+    def get_message(self) -> Message:
         raise ValueError("Event has no message!")
 
     @override
     def is_tome(self) -> bool:
         return not self.is_self() and self._is_tome()
 
     @staticmethod
     def _is_tome() -> bool:
         return True
 
     def is_self(self) -> bool:
         return self.self_id == self.get_user_id()
 
 
+class UnknownEvent(Event):
+    event_type: Literal["unknown"] = "unknown"
+
+
 EVENT_CLASSES: dict[str, type[Event]] = {}
 
 E = TypeVar("E", bound=Event)
 
 
+def get_event(event_name: str) -> type[Event]:
+    return EVENT_CLASSES.get(event_name, UnknownEvent)
+
+
 def register_event_class(event_class: type[E]) -> type[E]:
+    if event_class.model_fields["event_type"].default == PydanticUndefined:
+        raise ValueError(f"Event class {event_class} must have a field `event_type`")
     try:
         event_name = getattr(event_class, "event_name", get_args(event_class.__annotations__["event_name"])[0])
     except Exception as e:
         raise ValueError(
             f"Event class {event_class} must have a default value or Literal[str] type annotation for `event_name`"
         ) from e  # event_name 必须 有默认值 或 Literal[str] 类型注解
     EVENT_CLASSES[event_name] = event_class
     return event_class
 
 
+class NoticeEvent(Event):
+    event_type: Literal["notice"] = "notice"
+
+
+@register_event_class
+class DMConverseUpdateEvent(NoticeEvent):
+    """创建私信会话时的事件"""
+
+    event_name: Literal["notify:chat.converse.updateDMConverse"]
+
+    id: str = Field(alias="_id")  # 应该是converseId
+    type_: str = Field(alias="type")
+    members: list[str]
+    createdAt: datetime
+    updatedAt: datetime
+
+    v: int = Field(alias="__v")
+
+
 @register_event_class
-class MessageDeleteEvent(Event):
-    event_name: Literal["notify:chat.message.delete"] = "notify:chat.message.delete"
+class MessageDeleteEvent(NoticeEvent):
+    event_name: Literal["notify:chat.message.delete"]
 
     converseId: str
     messageId: str
 
 
-class GroupInfoEvent(Event):
+class GroupInfoEvent(NoticeEvent):
     id: str = Field(alias="_id")
     name: str
     owner: str
     members: list[MemberInfo]
     panels: list[Panel]
     roles: list[str]
     fallbackPermissions: list[str]
     createdAt: datetime
     updatedAt: datetime
-    __v: int
+
+    v: int = Field(alias="__v")
 
     config: Optional[dict] = None
     description: Optional[int] = None
     avatar: Optional[int] = None
 
 
 @register_event_class
 class GroupInfoUpdateEvent(GroupInfoEvent):
     event_name: Literal["notify:group.updateInfo"]
 
 
-class ReactionEvent(Event):
+class ReactionEvent(NoticeEvent):
     converseId: str
     messageId: str
     reaction: Reaction
 
 
 @register_event_class
 class ReactionAddEvent(ReactionEvent):
@@ -148,14 +183,15 @@
     id: str = Field(alias="_id")
     author: str
     hasRecall: bool
     converseId: str
     meta: Optional[MessageMeta] = Field(default=None)
 
     content: Message
+    raw_content: str = Field(alias="content")
     reactions: list[Reaction]
     createdAt: datetime
     updatedAt: datetime
 
     groupId: Optional[str] = Field(default=None)
 
     @property
@@ -185,15 +221,27 @@
             + f" {self.content.show()}"
         )
 
     def is_group(self) -> bool:
         return not not self.groupId
 
 
+@register_event_class
+class MessageAddEvent(DefaultMessageEvent):
+    event_name: Literal["notify:chat.message.add"]
+
+
+@register_event_class
+class MessageUpdateEvent(DefaultMessageEvent):
+    event_name: Literal["notify:chat.message.update"]
+
+
 class AtEvent(Event):
+    event_type: Literal["message"] = "message"
+
     type: str
 
     v: int = Field(alias="__v")
 
 
 @register_event_class
 class AtMessageEvent(AtEvent, MessageEvent):
@@ -233,15 +281,32 @@
         return (
             f"AtMessage {self.payload.messageId} from {self.payload.messageAuthor}"
             + (f"@[群:{self.get_group_id()}]" if self.payload.groupId else "")
             + f" {self.payload.messageSnippet.show()}"
         )
 
 
+class RequestEvent(Event):
+    event_type: Literal["request"] = "request"
+
+
 @register_event_class
-class MessageAddEvent(DefaultMessageEvent):
-    event_name: Literal["notify:chat.message.add"]
+class FriendRequestAddEvent(RequestEvent):
+    event_name: Literal["notify:friend.request.add"]
+
+    id: str = Field(alias="_id")
+    from_: str = Field(alias="from")
+    to: str
+    v: int = Field(alias="__v")
+
+    async def accept(self, bot: "Bot"):
+        return await bot.acceptRequest(requestId=self.id)
+
+    async def deny(self, bot: "Bot"):
+        return await bot.denyRequest(requestId=self.id)
 
 
 @register_event_class
-class MessageUpdateEvent(DefaultMessageEvent):
-    event_name: Literal["notify:chat.message.update"]
+class FriendRequestRemoveEvent(RequestEvent):
+    event_name: Literal["notify:friend.request.remove"]
+
+    requestId: str
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/message.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,15 @@
         cls.update_parser()
 
     @staticmethod
     def register_text(bbcode: type[B]) -> type[B]:
         """注册文本类型"""
         return _register_text(bbcode)
 
+    @override
     def __contains__(  # pyright: ignore[reportIncompatibleMethodOverride]
         self, value: Union[MessageSegment, str, type[B]]
     ) -> bool:
         if issubclass(value, BBCode):
             return value.tag_in(self)
         return super().__contains__(value)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/model.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime as raw_datetime
 from typing import Annotated, Optional
 
-from pydantic import BaseModel, BeforeValidator, ByteSize, ConfigDict, Field
+from pydantic import BaseModel, BeforeValidator, ByteSize, ConfigDict, Field, RootModel
 
 from .config import BotInfo
-from .message import Message
+from .message import Message, MessageSegment
 from .util import unpack
 
 datetime = Annotated[
     raw_datetime,
     BeforeValidator(unpack),
 ]
 
@@ -37,16 +37,28 @@
 
 class Replay(RawModel):
     id: str = Field(alias="_id")
     content: str
     author: str
 
 
+class Emoji(RootModel[str]):
+    @property
+    def name(self):
+        return self.root[1:-1]
+
+    def to_seg(self) -> MessageSegment:
+        return MessageSegment.emoji(self.name)
+
+    def __str__(self):
+        return self.root
+
+
 class Reaction(RawModel):
-    name: str
+    name: Emoji
     author: str
     id: Optional[str] = Field(default=None, alias="_id")
 
 
 class MessageMeta(RawModel):
     mentions: list[str]
 
@@ -105,25 +117,31 @@
     temporary: bool
     type: str
     emailVerified: bool
     banned: bool
     createdAt: datetime
     token: str
 
+    discriminator: Optional[str] = None
+
+
+TemporaryUserInfo = TokenInfo
+
 
 class MessageRet(RawModel):
     _id: str
     content: str
     author: str
     converseId: str
     hasRecall: bool
     reactions: list[Reaction]
     createdAt: datetime
     updatedAt: datetime
-    __v: int
+
+    v: int = Field(alias="__v")
 
     groupId: Optional[str] = None
     meta: Optional[MessageMeta] = None
 
 
 class ClientConfig(RawModel):
     uploadFileLimit: ByteSize
@@ -139,30 +157,22 @@
 
 class Ack(RawModel):
     userId: str
     converseId: str
     lastMessageId: str
 
 
-class BaseUserInfo(RawModel):
-    _id: str
-    nickname: str
-    email: str
-
-    avatar: Optional[str] = None
-
-
 class UserInfo(BaseUserInfo):
     temporary: bool  # 临时用户
     type: str
     emailVerified: bool
     banned: bool
     createdAt: datetime
 
-    discriminator: Optional[str] = None
+    discriminator: Optional[str] = None  # eya46#1145 -> nickname#discriminator
 
 
 class Whoami(RawModel):
     userAgent: str
     language: str
     user: BaseUserInfo
     token: str
@@ -171,15 +181,16 @@
 
 class ConverseInfo(RawModel):
     _id: str
     type: str
     members: list[str]
     createdAt: datetime
     updatedAt: datetime
-    __v: int
+
+    v: int = Field(alias="__v")
 
 
 class LastMessages(RawModel):
     converseId: str
     lastMessageId: str
 
 
@@ -232,25 +243,47 @@
     _id: str
     code: str
     creator: str
     groupId: str
     usage: int
     createdAt: datetime
     updatedAt: datetime
-    __v: int
+
+    v: int = Field(alias="__v")
+
+
+class BaseGroupInfo(RawModel):
+    name: str
+    owner: str
+    description: str
+    memberCount: int
 
 
 class GroupInfo(RawModel):
     _id: str
     name: str
     owner: str
     members: list[MemberInfo]
     panels: list[Panel]
     roles: list[str]
     fallbackPermissions: list[str]
     createdAt: datetime
     updatedAt: datetime
-    __v: int
+
+    v: int = Field(alias="__v")
 
     config: Optional[dict] = None
     description: Optional[int] = None
     avatar: Optional[int] = None
+
+
+class AddFriendRequestRet(RawModel):
+    id: str = Field(alias="_id")  # requestId
+    from_: str = Field(alias="from")
+    to: str = Field(alias="to")
+    v: int = Field(alias="__v")
+
+
+class GroupAndPanelIds(RawModel):
+    groupIds: list[str]
+    textPanelIds: list[str]
+    subscribeFeaturePanelIds: list[str]
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/util.py` & `nonebot_adapter_tailchat-0.1.0b5/nonebot_adapter_tailchat/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b4/pyproject.toml` & `nonebot_adapter_tailchat-0.1.0b5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-tailchat"
-version = "0.1.0b4"
+version = "0.1.0b5"
 description = "NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2"
 authors = ["eya46 <61458340+eya46@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "nonebot_adapter_tailchat" }]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_adapter_tailchat-0.1.0b4/PKG-INFO` & `nonebot_adapter_tailchat-0.1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-tailchat
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2
 License: Apache-2.0
 Author: eya46
 Author-email: 61458340+eya46@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b4 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b5 Summary:
 NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 License: Apache-2.0
 Author: eya46 Author-email: 61458340+eya46@users.noreply.github.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: msgpack (>=1.0.8,<2.0.0) Requires-
```

