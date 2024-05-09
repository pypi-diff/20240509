# Comparing `tmp/liveflask-1.0.9rc2.tar.gz` & `tmp/liveflask-1.0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.9rc2.tar", last modified: Wed May  8 15:09:19 2024, max compression
+gzip compressed data, was "liveflask-1.0.9rc3.tar", last modified: Wed May  8 20:12:33 2024, max compression
```

## Comparing `liveflask-1.0.9rc2.tar` & `liveflask-1.0.9rc3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.196335 liveflask-1.0.9rc2/
--rw-rw-rw-   0        0        0     1294 2024-05-08 15:09:19.195335 liveflask-1.0.9rc2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.137650 liveflask-1.0.9rc2/liveflask/
--rw-rw-rw-   0        0        0     6326 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.147657 liveflask-1.0.9rc2/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.148656 liveflask-1.0.9rc2/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3654 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.150655 liveflask-1.0.9rc2/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.165687 liveflask-1.0.9rc2/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1924 2024-05-08 15:04:13.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0     1328 2024-05-08 13:29:26.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/init.js
--rw-rw-rw-   0        0        0      894 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     9170 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.168985 liveflask-1.0.9rc2/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      348 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.179297 liveflask-1.0.9rc2/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.193334 liveflask-1.0.9rc2/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      871 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      202 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3296 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4276 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2839 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4780 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 19:41:30.000000 liveflask-1.0.9rc2/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.145656 liveflask-1.0.9rc2/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1294 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 15:09:19.196335 liveflask-1.0.9rc2/setup.cfg
--rw-rw-rw-   0        0        0     1225 2024-05-08 15:09:16.000000 liveflask-1.0.9rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.081877 liveflask-1.0.9rc3/
+-rw-rw-rw-   0        0        0     1294 2024-05-08 20:12:33.080403 liveflask-1.0.9rc3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:32.991315 liveflask-1.0.9rc3/liveflask/
+-rw-rw-rw-   0        0        0     6326 2024-05-08 13:26:44.000000 liveflask-1.0.9rc3/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.002288 liveflask-1.0.9rc3/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.004288 liveflask-1.0.9rc3/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3654 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.006287 liveflask-1.0.9rc3/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.023622 liveflask-1.0.9rc3/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1924 2024-05-08 15:04:13.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0     1328 2024-05-08 13:29:26.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/init.js
+-rw-rw-rw-   0        0        0     1409 2024-05-08 20:11:56.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     9170 2024-05-08 13:26:44.000000 liveflask-1.0.9rc3/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.027612 liveflask-1.0.9rc3/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      348 2024-05-08 13:26:44.000000 liveflask-1.0.9rc3/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.045613 liveflask-1.0.9rc3/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.076388 liveflask-1.0.9rc3/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      871 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      202 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3296 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4276 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2839 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4780 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 20:13:57.000000 liveflask-1.0.9rc3/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-01 19:41:30.000000 liveflask-1.0.9rc3/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:12:33.000316 liveflask-1.0.9rc3/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1294 2024-05-08 20:12:32.000000 liveflask-1.0.9rc3/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2024-05-08 20:12:32.000000 liveflask-1.0.9rc3/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 20:12:32.000000 liveflask-1.0.9rc3/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 20:12:32.000000 liveflask-1.0.9rc3/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 20:12:32.000000 liveflask-1.0.9rc3/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 20:12:33.081877 liveflask-1.0.9rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-05-08 20:12:19.000000 liveflask-1.0.9rc3/setup.py
```

### Comparing `liveflask-1.0.9rc2/PKG-INFO` & `liveflask-1.0.9rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc2
+Version: 1.0.9rc3
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.9rc2/liveflask/__init__.py` & `liveflask-1.0.9rc3/liveflask/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/attributes/__init__.py` & `liveflask-1.0.9rc3/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.9rc3/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/static/liveflask/action.js` & `liveflask-1.0.9rc3/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/static/liveflask/init.js` & `liveflask-1.0.9rc3/liveflask/static/liveflask/init.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.9rc3/liveflask/static/liveflask/liveflask.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,27 @@
 ///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 // INITIALIZERS
 ///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
+
+window.liveflask = {
+    components: [],
+    first: function() {
+        return this.components.length > 0 ? this.components[0] : null;
+    },
+    find: function(id) {
+        return this.components.find(component => component.data.key === id) || null;
+    },
+    get_by_name: function(name) {
+        return this.components.filter(component => component.class === name);
+    },
+    all: function() {
+        return this.components;
+    }
+}
+
 document.querySelectorAll('[data-component]').forEach(el => {
     let live_flask_children = [];
 
     el.__liveflask = JSON.parse(el.getAttribute('data-snapshot'));
     el.removeAttribute('data-snapshot')
 
 
@@ -16,14 +33,16 @@
     el.__liveflask.set = function(key, value) {
         el.__liveflask[key] = value
         send_request(el, {
             update_property: [key, value]
         }, undefined)
     }
 
+    window.liveflask.components.push(el.__liveflask);
+
     // register event named liveflask:initialized
     document.dispatchEvent(new CustomEvent('liveflask:initialized', {
         detail: el.__liveflask,
         target: el
     }))
     init_inits(el)
```

### Comparing `liveflask-1.0.9rc2/liveflask/static/liveflask/model.js` & `liveflask-1.0.9rc3/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/static/liveflask/polling.js` & `liveflask-1.0.9rc3/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/static/liveflask/utils.js` & `liveflask-1.0.9rc3/liveflask/static/liveflask/utils.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/static/lodash.min.js` & `liveflask-1.0.9rc3/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.9rc3/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.9rc3/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/has_actions.py` & `liveflask-1.0.9rc3/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/has_props.py` & `liveflask-1.0.9rc3/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/has_renders.py` & `liveflask-1.0.9rc3/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/traits/has_snapshots.py` & `liveflask-1.0.9rc3/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask/utils.py` & `liveflask-1.0.9rc3/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.9rc3/liveflask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc2
+Version: 1.0.9rc3
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.9rc2/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.9rc3/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc2/setup.py` & `liveflask-1.0.9rc3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.9rc2",
+    version="1.0.9rc3",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

