# Comparing `tmp/nonebot_plugin_mysticism-0.1.2.tar.gz` & `tmp/nonebot_plugin_mysticism-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mysticism-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_mysticism-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_mysticism-0.1.2.tar` & `nonebot_plugin_mysticism-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    11332 2024-05-09 12:35:24.261096 nonebot_plugin_mysticism-0.1.2/LICENSE
--rw-r--r--   0        0        0     2483 2024-05-09 12:35:24.261096 nonebot_plugin_mysticism-0.1.2/README.md
--rw-r--r--   0        0        0      466 2024-05-09 12:35:24.261096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/__init__.py
--rw-r--r--   0        0        0      158 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/config.py
--rw-r--r--   0        0        0      702 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/rule.py
--rw-r--r--   0        0        0     5325 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot.py
--rw-r--r--   0        0        0     3649 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_formations.yaml
--rw-r--r--   0        0        0        0 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/__init__.py
--rw-r--r--   0        0        0     3327 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
--rw-r--r--   0        0        0      774 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
--rw-r--r--   0        0        0     2176 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/waite.yaml
--rw-r--r--   0        0        0    11061 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_uitls.py
--rw-r--r--   0        0        0      959 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/utils.py
--rw-r--r--   0        0        0      555 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11332 2024-05-09 14:56:22.344444 nonebot_plugin_mysticism-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2483 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/README.md
+-rw-r--r--   0        0        0      466 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/config.py
+-rw-r--r--   0        0        0      702 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/rule.py
+-rw-r--r--   0        0        0     6351 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot.py
+-rw-r--r--   0        0        0     3611 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_formations.yaml
+-rw-r--r--   0        0        0    11099 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_keywords.yml
+-rw-r--r--   0        0        0        0 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/__init__.py
+-rw-r--r--   0        0        0     3327 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
+-rw-r--r--   0        0        0      774 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
+-rw-r--r--   0        0        0     2120 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/waite.yaml
+-rw-r--r--   0        0        0    11221 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_uitls.py
+-rw-r--r--   0        0        0     1043 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/utils.py
+-rw-r--r--   0        0        0      555 2024-05-09 14:56:22.348444 nonebot_plugin_mysticism-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_mysticism-0.1.2/LICENSE` & `nonebot_plugin_mysticism-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.2/README.md` & `nonebot_plugin_mysticism-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/rule.py` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot.py` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,54 +45,86 @@
     state["cnumber"] = []
     state["tarot_theme"] = random.choice(tarot_uitls.THEME)
     state["stack_card"] = tarot_uitls.TAROT_STACK.copy()
     random.shuffle(state["stack_card"])
     # 先洗牌更有仪式感（x）
 
     result += f"目前抽取到了：{formations}\n"
-    result += f'共计需要选择 {state["cards_num"]} 张牌。\n'
     result += f'所以接下来请发送 {state["cards_num"]} 个 1-78 的数字。\n'
     result += f"(注：其实不是1-78也行，我取模了（？）)\n"
-    result += f'(注：可以一次性发多个，例如"1 114514 3 8")\n'
+    result += f'(注：可以一次性发多个，例如"1 114514 3 8")'
     await tarot.send(result)
 
 
 @tarot.got("nums", prompt="请输入数字")
 async def _(bot: Bot, event, state: T_State, nums=ArgPlainText()):
     if nums.strip() == "cancel":
         tarot.finish("已取消占卜🔮")
     try:
-        nums = list(
-            filter(
-                lambda x: x not in state["cnumber"],
-                map(lambda x: x % 78, map(int, nums.split())),
-            )
-        )
-    except Exception as ex:
+        sep = None
+        if "," in nums:
+            sep = ","
+        elif "." in nums:
+            sep = "."
+        for i in map(lambda x: x % 78, map(int, nums.split(sep=sep))):
+            if i in state["cnumber"]:
+                continue
+            state["cnumber"].append(i)
+    except:
         await tarot.reject(
             f"似乎，这些不只是数字……\n你还得再输入 {state['cards_num']} 个数字"
         )
-    state["cnumber"].extend(nums)
-    state["cards_num"] -= len(nums)
-    if state["cards_num"] > 0:
-        await tarot.reject(f"你还得再输入 {state['cards_num']} 个数字")
 
+    if state["cards_num"] > len(state["cnumber"]):
+        await tarot.reject(
+            f"你还得再输入 {state['cards_num']-len(state['cnumber'])} 个数字"
+        )
+
+    await tarot.send("🔮占卜ing……\n请坐与放宽……")
     formation = state["formations"]
     random.seed(sum(state["cnumber"]) + random.random())
     representations = random.choice(formation.get("representations"))
-
+    meanings = []
     message = []
     for i in range(formation["cards_num"]):
         content = [V11Seg.text(f"第{i+1}张牌「{representations[i]}」\n")]
         _id = state["stack_card"][state["cnumber"][i]]
-        img = Image.open(await send_image_as_bytes(state["tarot_theme"][_id].face_url))
-        postfix = f"「{tarot_uitls.CN_Name[_id]} 正位」"
+        img = await send_image_as_bytes(state["tarot_theme"][_id].face_url)
+        if not img:
+            await tarot.finish(f"网络异常喵。\n主题名字：{state["tarot_theme"].name}" )
+        img = Image.open(img)
         if random.randint(0, 1) == 1:
             img = img.transpose(Image.ROTATE_180)
             postfix = f"「{tarot_uitls.CN_Name[_id]} 逆位」"
+            meanings.append(
+                {
+                    "type": "node",
+                    "data": {
+                        "uin": str(event.get_user_id()),
+                        "name": postfix,
+                        "content": postfix
+                        + "\n"
+                        + tarot_uitls.TAROT_KEYWORDS[_id]["rev"],
+                    },
+                },
+            )
+        else:
+            postfix = f"「{tarot_uitls.CN_Name[_id]} 正位」"
+            meanings.append(
+                {
+                    "type": "node",
+                    "data": {
+                        "uin": str(event.get_user_id()),
+                        "name": postfix,
+                        "content": postfix
+                        + "\n"
+                        + tarot_uitls.TAROT_KEYWORDS[_id]["up"],
+                    },
+                },
+            )
 
         image = BytesIO()
         img.convert("RGB").save(image, "JPEG")
         content.append(V11Seg.image(image))
         content.append(V11Seg.text(postfix))
 
         message.append(
@@ -103,14 +135,15 @@
                     "name": postfix,
                     "content": content,
                 },
             },
         )
 
     random.seed()
+    message.extend(meanings)
     # group
     if isinstance(event, V11G):
         await bot.call_api(
             "send_group_forward_msg", group_id=event.group_id, messages=message
         )
     else:
         await tarot.finish(
@@ -136,18 +169,17 @@
 async def _(bot: Bot, args=CommandArg()):
     args = args.extract_plain_text().strip()
     try:
         args = NUM2ID.get(args, "")
     except:
         args = ""
 
-    _list = list(filter(lambda x: x.startswith(args), tarot_uitls.TAROT_STACK))
-    if len(_list) <= 0:
-        _list = tarot_uitls.TAROT_STACK
-    _id = random.choice(_list)
+    _id = random.choice(
+        list(filter(lambda x: x.startswith(args), tarot_uitls.TAROT_STACK))
+    )
 
     theme = random.choice(tarot_uitls.THEME)
     img = Image.open(await send_image_as_bytes(theme[_id].face_url))
     postfix = f"「{tarot_uitls.CN_Name[_id]} 正位」"
     if random.randint(0, 1) == 1:
         img = img.transpose(Image.ROTATE_180)
         postfix = f"「{tarot_uitls.CN_Name[_id]} 逆位」"
```

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_formations.yaml` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_formations.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -68,24 +68,27 @@
     cards_num: 4
     is_cut: false
     representations:
       - - 人际关系现状
         - 与对方结识的因缘
         - 双方关系的发展
         - 双方关系的结论
-  沙迪若之星牌阵:
-    cards_num: 6
-    is_cut: true
+  档案馆牌阵:
+    cards_num: 9
+    is_cut: false
     representations:
-      - - 问卜者的感受
-        - 问卜者的问题
-        - 问题下的影响因素
-        - 将问卜者与问题纠缠在一起的往事
-        - 需要注意/考虑的
-        - 可能的结果
+      - - 分析1
+        - 分析2
+        - 分析3
+        - 预言1
+        - 预言2
+        - 预言3
+        - 改变方向1
+        - 改变方向2
+        - 改变方向3
   灵魂之旅牌阵:
     cards_num: 5
     is_cut: false
     representations:
       - - 自我认识
         - 挑战
         - 隐藏的影响
@@ -144,14 +147,14 @@
   time: 时间之流牌阵
   elements: 四要素牌阵
   five: 五牌阵
   gypsy: 吉普赛十字阵
   horseshoe: 马蹄牌阵
   star: 六芒星牌阵
   peace: 平安扇牌阵
-  shadow: 沙迪若之星牌阵
+  fengxue: 档案馆牌阵
   soul: 灵魂之旅牌阵
   tree: 生命之树牌阵
   guide: 星光指引牌阵
   moon: 月光之路牌阵
   dream: 梦境探索牌阵
   wisdom: 智慧之门牌阵
```

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/waite.yaml` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_theme/waite.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 - 2012/09/cups10.jpg
 - 2012/09/cups11.jpg
 - 2012/09/cups12.jpg
 - 2012/09/cups13.jpg
 - 2012/09/cups14.jpg
 
 pentacles:
-- 2012/09/pentacles01.jpg
-- 2012/09/pentacles02.jpg
-- 2012/09/pentacles03.jpg
-- 2012/09/pentacles04.jpg
-- 2012/09/pentacles05.jpg
-- 2012/09/pentacles06.jpg
-- 2012/09/pentacles07.jpg
-- 2012/09/pentacles08.jpg
-- 2012/09/pentacles09.jpg
-- 2012/09/pentacles10.jpg
-- 2012/09/pentacles11.jpg
-- 2012/09/pentacles12.jpg
-- 2012/09/pentacles13.jpg
-- 2012/09/pentacles14.jpg
+- 2012/09/pents01.jpg
+- 2012/09/pents02.jpg
+- 2012/09/pents03.jpg
+- 2012/09/pents04.jpg
+- 2012/09/pents05.jpg
+- 2012/09/pents06.jpg
+- 2012/09/pents07.jpg
+- 2012/09/pents08.jpg
+- 2012/09/pents09.jpg
+- 2012/09/pents10.jpg
+- 2012/09/pents11.jpg
+- 2012/09/pents12.jpg
+- 2012/09/pents13.jpg
+- 2012/09/pents14.jpg
 
 wands:
 - 2012/09/wands01.jpg
 - 2012/09/wands02.jpg
 - 2012/09/wands03.jpg
 - 2012/09/wands04.jpg
 - 2012/09/wands05.jpg
```

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_uitls.py` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/tarot_uitls.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,7 +396,11 @@
     "major.tower": "塔",
     "major.star": "星星",
     "major.moon": "月亮",
     "major.sun": "太阳",
     "major.judgement": "审判",
     "major.world": "世界",
 }
+
+TAROT_KEYWORDS = {}
+with open(pathlib.Path(__file__).parent / "tarot_keywords.yml", encoding="utf-8") as f:
+    TAROT_KEYWORDS = yaml.load(f, yaml.FullLoader)
```

### Comparing `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/utils.py` & `nonebot_plugin_mysticism-0.1.3/nonebot_plugin_mysticism/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 import hashlib
 import tempfile
 import pathlib
 
 
 # 返回BytesIO对象图片
 async def send_image_as_bytes(url: str, cache: bool = True):
-    path = pathlib.Path(tempfile.gettempdir()) / "tarot"
-    if not os.path.exists(path):
-        os.mkdir(path)
-    path /= hashlib.sha256(url.encode()).hexdigest()
+    if cache:
+        path = pathlib.Path(tempfile.gettempdir()) / "tarot"
+        if not os.path.exists(path):
+            os.mkdir(path)
+        path /= hashlib.sha256(url.encode()).hexdigest()
 
-    if os.path.exists(path):
-        with open(path, mode="rb") as f:
-            buffered = BytesIO(f.read())
-            buffered.seek(0)
-            return buffered
+        if os.path.exists(path):
+            with open(path, mode="rb") as f:
+                buffered = BytesIO(f.read())
+                buffered.seek(0)
+                return buffered
 
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             if response.status == 200:
                 image_data = await response.read()
-                with open(path, mode="wb+") as f:
-                    f.write(image_data)
+                if cache:
+                    with open(path, mode="wb+") as f:
+                        f.write(image_data)
                 buffered = BytesIO(image_data)
                 buffered.seek(0)
                 return buffered
             else:
                 return None
```

### Comparing `nonebot_plugin_mysticism-0.1.2/pyproject.toml` & `nonebot_plugin_mysticism-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mysticism"
-version = "0.1.2"
+version = "0.1.3"
 description = "占卜辅助工具"
 authors = ["Yan <1964649083@qq.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 keywords = ["tarot", "nonebot", "nonebot2", "bot", "qq"]
 homepage = "https://github.com/Yan-Zero/nonebot_plugin_mysticism"
```

### Comparing `nonebot_plugin_mysticism-0.1.2/PKG-INFO` & `nonebot_plugin_mysticism-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mysticism
-Version: 0.1.2
+Version: 0.1.3
 Summary: 占卜辅助工具
 Home-page: https://github.com/Yan-Zero/nonebot_plugin_mysticism
 License: Apache-2.0
 Keywords: tarot,nonebot,nonebot2,bot,qq
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.3 Summary:
 å åè¾å©å·¥å· Home-page: https://github.com/Yan-Zero/
 nonebot_plugin_mysticism License: Apache-2.0 Keywords:
 tarot,nonebot,nonebot2,bot,qq Author: Yan Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.5,<4.0.0) Requires-Dist: nonebot-
```

