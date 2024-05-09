# Comparing `tmp/Fr1997v011-1.4.4.tar.gz` & `tmp/Fr1997v011-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.4.tar", last modified: Mon Apr 29 18:50:03 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.5.tar", last modified: Tue Apr 30 03:06:58 2024, max compression
```

## Comparing `Fr1997v011-1.4.4.tar` & `Fr1997v011-1.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.791046 Fr1997v011-1.4.4/
-drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.774978 Fr1997v011-1.4.4/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.4/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-29 18:50:03.789042 Fr1997v011-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-29 09:24:56.000000 Fr1997v011-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.777005 Fr1997v011-1.4.4/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.4/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.783010 Fr1997v011-1.4.4/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.4/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   173742 2024-04-29 09:28:37.000000 Fr1997v011-1.4.4/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.786516 Fr1997v011-1.4.4/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.4/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-29 18:50:03.791046 Fr1997v011-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-29 18:50:00.000000 Fr1997v011-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.848653 Fr1997v011-1.4.5/
+drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.840137 Fr1997v011-1.4.5/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-30 03:06:58.847664 Fr1997v011-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-29 18:50:20.000000 Fr1997v011-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.841137 Fr1997v011-1.4.5/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.5/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.844648 Fr1997v011-1.4.5/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.5/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   175297 2024-04-30 03:06:53.000000 Fr1997v011-1.4.5/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.845652 Fr1997v011-1.4.5/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.5/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 03:06:58.848653 Fr1997v011-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-30 03:06:53.000000 Fr1997v011-1.4.5/setup.py
```

### Comparing `Fr1997v011-1.4.4/LICENSE` & `Fr1997v011-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.4/README.md` & `Fr1997v011-1.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.3.tar.gz
+pip install dist/Fr1997v011-1.4.4.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.4.4/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.5/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -2653,14 +2653,57 @@
                 hits_list = response.get('hits')['hits']
                 print(f'总个数:{value} 取出:{len(hits_list)}')
                 if ret_num == 0:
                     return hits_list
                 else:
                     return [hits_list, value]
 
+    # ES 查询
+    def es_search_new_20231215_old(self, table, query, _source, size=1, sort_info=None, is_ret_num=1, ret_num=0,
+                                   **kwargs):
+        body = {
+            "query": query,
+            "track_total_hits": True if is_ret_num == 1 else False,
+            "size": size,
+            "_source": _source,
+        }
+
+        # 排序
+        if sort_info and sort_info != 0:
+            body['sort'] = sort_info
+        else:
+            body['sort'] = {
+                "_script": {
+                    "script": "Math.random()",
+                    "type": "number"
+                }
+            }
+
+        es_cfg = 'es_jike_out'
+        es_ip = config_dict['es'][es_cfg]['ip']
+        es_user = config_dict['es'][es_cfg]['user']
+        es_pwb = config_dict['es'][es_cfg]['pwd']
+        es_port = config_dict['es'][es_cfg]['port']
+        es = Elasticsearch([f'{es_ip}:{es_port}'], http_auth=(es_user, es_pwb))
+        response = es.search(
+            index=table,
+            body=body
+        )
+        _shards = response.get('_shards')
+        if _shards:
+            successful = _shards.get('successful')
+            if successful > 0:
+                value = response.get('hits')['total']['value']
+                hits_list = response.get('hits')['hits']
+                print(f'总个数:{value} 取出:{len(hits_list)}')
+                if ret_num == 0:
+                    return hits_list
+                else:
+                    return [hits_list, value]
+
     # ES 查询 单条
     def es_search_one(self, table, _id, is_print=1):
         body = {
             "track_total_hits": True,
             "query": {
                 "match": {"_id": _id}
             }
```

