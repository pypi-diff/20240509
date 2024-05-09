# Comparing `tmp/nonebot_plugin_cnrail-0.2.2.post1.tar.gz` & `tmp/nonebot_plugin_cnrail-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cnrail-0.2.2.post1.tar", last modified: Fri May  3 11:29:43 2024, max compression
+gzip compressed data, was "nonebot_plugin_cnrail-0.2.3.tar", last modified: Thu May  9 14:56:16 2024, max compression
```

## Comparing `nonebot_plugin_cnrail-0.2.2.post1.tar` & `nonebot_plugin_cnrail-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-05-03 11:29:29.950398 nonebot_plugin_cnrail-0.2.2.post1/LICENSE
--rw-r--r--   0        0        0     4604 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/README.md
--rw-r--r--   0        0        0      687 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__init__.py
--rw-r--r--   0        0        0     4233 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__main__.py
--rw-r--r--   0        0        0      308 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/config.py
--rw-r--r--   0        0        0     5526 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/data_source.py
--rw-r--r--   0        0        0     4830 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/models.py
--rw-r--r--   0        0        0    15513 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/templates/train_table.html.jinja
--rw-r--r--   0        0        0      814 2024-05-03 11:29:43.098519 nonebot_plugin_cnrail-0.2.2.post1/pyproject.toml
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.2.post1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4642 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/README.md
+-rw-r--r--   0        0        0      681 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/__init__.py
+-rw-r--r--   0        0        0     4233 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/__main__.py
+-rw-r--r--   0        0        0      308 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/config.py
+-rw-r--r--   0        0        0     5525 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/data_source.py
+-rw-r--r--   0        0        0     4830 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/models.py
+-rw-r--r--   0        0        0    15513 2024-05-09 14:56:00.890486 nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/templates/train_table.html.jinja
+-rw-r--r--   0        0        0      808 2024-05-09 14:56:16.838516 nonebot_plugin_cnrail-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/LICENSE` & `nonebot_plugin_cnrail-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/README.md` & `nonebot_plugin_cnrail-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,18 @@
 
 **[赞助我](https://blog.lgc2333.top/donate)**
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 ## 📝 更新日志
 
+### 0.2.3
+
+- 更换上游 API 域名
+
 ### 0.2.2
 
 - 修复列车行驶进度条计算问题（fix by [@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)）
 
 ### 0.2.1
 
 - 适配 [MoeFactory API](https://train.moefactory.com)
```

#### html2text {}

```diff
@@ -23,18 +23,19 @@
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [æµ·å°å¾·å°å©æ](https://qun.qq.com/qunpro/
 robot/qunshare?robot_uin=3889001607) & [Train-QQBot æä»¶](https://github.com/
 staytomorrow/FindTrain) çµææ¥æº ### [MoeFactory æä¾çæ¥è¯¢ API]
 (https://train.moefactory.com/) æ°æ®æ¥æº ## ð° èµå© **[èµå©æ]
 (https://blog.lgc2333.top/donate)**
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
-ð æ´æ°æ¥å¿ ### 0.2.2 - ä¿®å¤åè½¦è¡é©¶è¿åº¦æ¡è®¡ç®é®é¢ï¼fix by
-[@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)ï¼ ### 0.2.1 - éé
-[MoeFactory API](https://train.moefactory.com) - æ°å¢éç½®é¡¹
-`CNRAIL_ACG_IMAGE_URL` ### 0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ###
-0.1.7 - æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ -
-bug fix ### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 -
-ä¿®å¤ `-h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº
-### 0.1.3 - fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/
-issues/2) ### 0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~
-åååæ¥ï¼ ### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢
-### 0.1.0 - ð Create this project
+ð æ´æ°æ¥å¿ ### 0.2.3 - æ´æ¢ä¸æ¸¸ API åå ### 0.2.2 -
+ä¿®å¤åè½¦è¡é©¶è¿åº¦æ¡è®¡ç®é®é¢ï¼fix by [@This-is-XiaoDeng](https://
+github.com/This-is-XiaoDeng)ï¼ ### 0.2.1 - éé [MoeFactory API](https://
+train.moefactory.com) - æ°å¢éç½®é¡¹ `CNRAIL_ACG_IMAGE_URL` ### 0.2.0 -
+éé Pydantic V1 & V2 - æ ·å¼å¾®è° ### 0.1.7 -
+æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ - bug fix
+### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 - ä¿®å¤ `-
+h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº ### 0.1.3 -
+fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/issues/2) ###
+0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~ åååæ¥ï¼
+### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢ ### 0.1.0 - ð
+Create this project
```

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__init__.py` & `nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.2.post1"
+__version__ = "0.2.3"
 __plugin_meta__ = PluginMetadata(
     name="CNRail",
     description="查询 12306 列车时刻表",
     usage="使用指令 train -h 查看帮助",
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__main__.py` & `nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/data_source.py` & `nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nonebot.compat import type_validate_python
 from nonebot_plugin_htmlrender import get_new_page
 from playwright.async_api import Request, Route
 
 from .config import config
 from .models import ReturnData, TrainDetailData, TrainSearchResult, TrainSNData
 
-MOERAIL_API_BASE = "https://train.moefactory.com/api/"
+MOERAIL_API_BASE = "https://rail.moefactory.com/api/"
 
 TEMPLATE_PATH = Path(__file__).parent / "templates" / "train_table.html.jinja"
 
 ROUTE_BASE_URL = "https://cnrail.nonebot/"
 ROUTE_IMAGE_URL = f"{ROUTE_BASE_URL}image"
 
 TZ_SHANGHAI = pytz.timezone("Asia/Shanghai")
```

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/models.py` & `nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/templates/train_table.html.jinja` & `nonebot_plugin_cnrail-0.2.3/nonebot_plugin_cnrail/templates/train_table.html.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -329,33 +329,32 @@
         <div class="bottom-title">经停站</div>
         <div class="station-table-wrapper">
           <table class="station-table">
             <thead>
               <tr>
                 <th></th>
                 <th>停靠站</th>
-                <th>到点</th>
                 <th>开点</th>
+                <th>到点</th>
                 <th>停留</th>
                 <th>车次</th>
               </tr>
             </thead>
             <tbody>
               {% for station in detail.via_stations -%}
               <tr>
                 <td>
-
                   <div class="station-point{% if detail.arrived(loop.index0, train_date) %} arrived{% endif %}"></div>
                 </td>
                 <td>{{ station.station_name }}</td>
                 <td>
-                  {% if loop.first %}-{% else %}{{ station.arrival_time}}{% endif %}
+                  {% if loop.last %}-{% else %}{{ station.departure_time }}{% endif %}
                 </td>
                 <td>
-                  {% if loop.last %}-{% else %}{{ station.departure_time }}{% endif %}
+                  {% if loop.first %}-{% else %}{{ station.arrival_time}}{% endif %}
                 </td>
                 <td>{% if loop.first %}始发站{% elif loop.last %}终点站{% else %}{{ station.stop_minutes }} 分{% endif %}</td>
                 <td>{{ station.train_number }}</td>
               </tr>
               {% endfor -%}
             </tbody>
           </table>
@@ -581,8 +580,8 @@
     doneDivElem.id = 'done';
     document.body.appendChild(doneDivElem);
   }
 
   main();
 </script>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 担当路局：{{ detail.company_name }}
 {%- if sn -%}
 车组号：{{ sn }}
 {%- else -%}
 列车型号：{{ detail.routing.train_model }}
 {%- endif %}
 经停站
- ?停?靠?站                  ?到?点                     ?开?点                     ?停?留                   ?车?次
+ ?停?靠?站                  ?开?点                     ?到?点                     ?停?留                   ?车?次
                                                                     {% if loop.first
- {                    {% if loop.first %}-{% {% if loop.last %}-{%  %}始发站{% elif         {
+ {                    {% if loop.last %}-{%  {% if loop.first %}-{% %}始发站{% elif         {
  {                    else %}{               else %}{               loop.last %}终点站{%    {
  station.station_name {                      {                      else %}{             station.train_number
- }}                   station.arrival_time}} station.departure_time {                    }}
-                      {% endif %}            }}{% endif %}          station.stop_minutes
+ }}                   station.departure_time station.arrival_time}} {                    }}
+                      }}{% endif %}          {% endif %}            station.stop_minutes
                                                                     }} 分{% endif %}
```

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/pyproject.toml` & `nonebot_plugin_cnrail-0.2.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "nonebot-plugin-alconna>=0.40.1",
     "nonebot-plugin-htmlrender>=0.2.2",
     "jinja2>=3.1.2",
     "pytz>=2023.3.post1",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.2.post1"
+version = "0.2.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail"
```

### Comparing `nonebot_plugin_cnrail-0.2.2.post1/PKG-INFO` & `nonebot_plugin_cnrail-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cnrail
-Version: 0.2.2.post1
+Version: 0.2.3
 Summary: NoneBot2 plugin for query the train time table
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Author-Email: student_2333 <lgc2333@126.com>, XieXiLin <support@xiexilin.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
@@ -158,14 +158,18 @@
 
 **[赞助我](https://blog.lgc2333.top/donate)**
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 ## 📝 更新日志
 
+### 0.2.3
+
+- 更换上游 API 域名
+
 ### 0.2.2
 
 - 修复列车行驶进度条计算问题（fix by [@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)）
 
 ### 0.2.1
 
 - 适配 [MoeFactory API](https://train.moefactory.com)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.2.post1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.3 Summary:
 NoneBot2 plugin for query the train time table Home-page: https://github.com/
 lgc-NB2Dev/nonebot-plugin-cnrail Author-Email: student_2333
 126.com>, XieXiLin
 xiexilin.com> License: MIT Project-URL: Homepage, https://github.com/lgc-
 NB2Dev/nonebot-plugin-cnrail Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonebot2>=2.2.0 Requires-Dist: httpx>=0.24 Requires-Dist: nonebot-plugin-
 alconna>=0.40.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.2 Requires-Dist:
@@ -33,18 +33,19 @@
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [æµ·å°å¾·å°å©æ](https://qun.qq.com/qunpro/
 robot/qunshare?robot_uin=3889001607) & [Train-QQBot æä»¶](https://github.com/
 staytomorrow/FindTrain) çµææ¥æº ### [MoeFactory æä¾çæ¥è¯¢ API]
 (https://train.moefactory.com/) æ°æ®æ¥æº ## ð° èµå© **[èµå©æ]
 (https://blog.lgc2333.top/donate)**
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
-ð æ´æ°æ¥å¿ ### 0.2.2 - ä¿®å¤åè½¦è¡é©¶è¿åº¦æ¡è®¡ç®é®é¢ï¼fix by
-[@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)ï¼ ### 0.2.1 - éé
-[MoeFactory API](https://train.moefactory.com) - æ°å¢éç½®é¡¹
-`CNRAIL_ACG_IMAGE_URL` ### 0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ###
-0.1.7 - æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ -
-bug fix ### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 -
-ä¿®å¤ `-h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº
-### 0.1.3 - fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/
-issues/2) ### 0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~
-åååæ¥ï¼ ### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢
-### 0.1.0 - ð Create this project
+ð æ´æ°æ¥å¿ ### 0.2.3 - æ´æ¢ä¸æ¸¸ API åå ### 0.2.2 -
+ä¿®å¤åè½¦è¡é©¶è¿åº¦æ¡è®¡ç®é®é¢ï¼fix by [@This-is-XiaoDeng](https://
+github.com/This-is-XiaoDeng)ï¼ ### 0.2.1 - éé [MoeFactory API](https://
+train.moefactory.com) - æ°å¢éç½®é¡¹ `CNRAIL_ACG_IMAGE_URL` ### 0.2.0 -
+éé Pydantic V1 & V2 - æ ·å¼å¾®è° ### 0.1.7 -
+æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ - bug fix
+### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 - ä¿®å¤ `-
+h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº ### 0.1.3 -
+fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/issues/2) ###
+0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~ åååæ¥ï¼
+### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢ ### 0.1.0 - ð
+Create this project
```

