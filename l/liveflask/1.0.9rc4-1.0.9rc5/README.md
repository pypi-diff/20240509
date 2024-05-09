# Comparing `tmp/liveflask-1.0.9rc4.tar.gz` & `tmp/liveflask-1.0.9rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.9rc4.tar", last modified: Thu May  9 10:51:53 2024, max compression
+gzip compressed data, was "liveflask-1.0.9rc5.tar", last modified: Thu May  9 12:05:02 2024, max compression
```

## Comparing `liveflask-1.0.9rc4.tar` & `liveflask-1.0.9rc5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.215731 liveflask-1.0.9rc4/
--rw-rw-rw-   0        0        0     1371 2024-05-09 10:51:53.213732 liveflask-1.0.9rc4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.157730 liveflask-1.0.9rc4/liveflask/
--rw-rw-rw-   0        0        0     6326 2024-05-08 12:07:33.000000 liveflask-1.0.9rc4/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.167731 liveflask-1.0.9rc4/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.169731 liveflask-1.0.9rc4/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3650 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.171731 liveflask-1.0.9rc4/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.185731 liveflask-1.0.9rc4/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     4161 2024-05-09 10:51:01.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0     1328 2024-05-09 00:40:19.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/init.js
--rw-rw-rw-   0        0        0     1409 2024-05-09 00:40:19.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     9170 2024-05-08 11:46:18.000000 liveflask-1.0.9rc4/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.187730 liveflask-1.0.9rc4/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      348 2024-05-04 23:19:29.000000 liveflask-1.0.9rc4/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.200730 liveflask-1.0.9rc4/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.211731 liveflask-1.0.9rc4/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      867 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      198 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3292 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4272 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2835 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4776 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 21:07:09.000000 liveflask-1.0.9rc4/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:51:53.166732 liveflask-1.0.9rc4/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1371 2024-05-09 10:51:53.000000 liveflask-1.0.9rc4/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-05-09 10:51:53.000000 liveflask-1.0.9rc4/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 10:51:53.000000 liveflask-1.0.9rc4/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-09 10:51:53.000000 liveflask-1.0.9rc4/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 10:51:53.000000 liveflask-1.0.9rc4/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 10:51:53.215731 liveflask-1.0.9rc4/setup.cfg
--rw-rw-rw-   0        0        0     1225 2024-05-09 10:51:49.000000 liveflask-1.0.9rc4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.325068 liveflask-1.0.9rc5/
+-rw-rw-rw-   0        0        0     1371 2024-05-09 12:05:02.324069 liveflask-1.0.9rc5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.264068 liveflask-1.0.9rc5/liveflask/
+-rw-rw-rw-   0        0        0     6326 2024-05-08 12:07:33.000000 liveflask-1.0.9rc5/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.275068 liveflask-1.0.9rc5/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.277068 liveflask-1.0.9rc5/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3650 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.279069 liveflask-1.0.9rc5/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.294068 liveflask-1.0.9rc5/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     4161 2024-05-09 10:51:01.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0     1328 2024-05-09 00:40:19.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/init.js
+-rw-rw-rw-   0        0        0     1649 2024-05-09 12:00:18.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     9669 2024-05-09 12:00:26.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.299068 liveflask-1.0.9rc5/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      348 2024-05-04 23:19:29.000000 liveflask-1.0.9rc5/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.311068 liveflask-1.0.9rc5/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.321068 liveflask-1.0.9rc5/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      867 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      198 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3292 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4272 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2835 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4776 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.273068 liveflask-1.0.9rc5/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1371 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:05:02.325068 liveflask-1.0.9rc5/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-05-09 12:04:59.000000 liveflask-1.0.9rc5/setup.py
```

### Comparing `liveflask-1.0.9rc4/PKG-INFO` & `liveflask-1.0.9rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc4
+Version: 1.0.9rc5
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.9rc4/liveflask/__init__.py` & `liveflask-1.0.9rc5/liveflask/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/attributes/__init__.py` & `liveflask-1.0.9rc5/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.9rc5/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/static/liveflask/action.js` & `liveflask-1.0.9rc5/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/static/liveflask/init.js` & `liveflask-1.0.9rc5/liveflask/static/liveflask/init.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.9rc5/liveflask/static/liveflask/liveflask.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -16,19 +16,26 @@
     all: function() {
         return this.components;
     }
 }
 
 document.querySelectorAll('[data-component]').forEach(el => {
     let live_flask_children = [];
+    let elementsWithDataLoading = el.querySelectorAll('[data-loading]');
 
     el.__liveflask = JSON.parse(el.getAttribute('data-snapshot'));
     el.removeAttribute('data-snapshot')
 
 
+    elementsWithDataLoading.forEach(element => {
+        console.log("Element with data-loading: ", element);
+        element.style.display = "none";
+    });
+
+
     init_model(el)
     init_action(el)
     init_polling(el)
 
 
     el.__liveflask.set = function(key, value) {
         el.__liveflask[key] = value
```

### Comparing `liveflask-1.0.9rc4/liveflask/static/liveflask/model.js` & `liveflask-1.0.9rc5/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/static/liveflask/polling.js` & `liveflask-1.0.9rc5/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/static/liveflask/utils.js` & `liveflask-1.0.9rc5/liveflask/static/liveflask/utils.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -125,14 +125,20 @@
 // SERVER CALL
 ///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 function send_request(el, add_to_payload, target) {
     let updated_element;
     let emits;
     let snapshot = el.__liveflask
     let children = attr_beginswith('data-component', el);
+    let elementsWithDataLoading = el.querySelectorAll('[data-loading]');
+    elementsWithDataLoading.forEach(element => {
+        console.log("Element with data-loading: ", element);
+        element.style.display = "block";
+    });
+
     fetch("/liveflask/", {
         method: "POST",
         headers: {
             "Content-Type": "application/json",
             "X-CSRF-Token": csrfToken
         },
         body: JSON.stringify({
@@ -233,14 +239,21 @@
             let url = new URL(window.location.href);
             Object.keys(url_object).forEach(key => {
                 url.searchParams.set(key, url_object[key]);
             });
             window.history.pushState({}, '', url);
         }
 
+
+        let elementsWithDataLoading = el.querySelectorAll('[data-loading]');
+        elementsWithDataLoading.forEach(element => {
+            console.log("Element with data-loading: ", element);
+            element.style.display = "none";
+        });
+
     }).then(el => {
 
 
     })
 }
```

### Comparing `liveflask-1.0.9rc4/liveflask/static/lodash.min.js` & `liveflask-1.0.9rc5/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.9rc5/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/has_actions.py` & `liveflask-1.0.9rc5/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/has_props.py` & `liveflask-1.0.9rc5/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/has_renders.py` & `liveflask-1.0.9rc5/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/traits/has_snapshots.py` & `liveflask-1.0.9rc5/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask/utils.py` & `liveflask-1.0.9rc5/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.9rc5/liveflask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc4
+Version: 1.0.9rc5
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.9rc4/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.9rc5/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc4/setup.py` & `liveflask-1.0.9rc5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.9rc4",
+    version="1.0.9rc5",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

