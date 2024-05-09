# Comparing `tmp/pytest_splunk_addon_ui_smartx-3.0.2.tar.gz` & `tmp/pytest_splunk_addon_ui_smartx-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon_ui_smartx-3.0.2.tar", max compression
+gzip compressed data, was "pytest_splunk_addon_ui_smartx-3.1.0.tar", max compression
```

## Comparing `pytest_splunk_addon_ui_smartx-3.0.2.tar` & `pytest_splunk_addon_ui_smartx-3.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11341 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/LICENSE
--rw-r--r--   0        0        0     1782 2024-03-26 10:44:07.327587 pytest_splunk_addon_ui_smartx-3.0.2/pyproject.toml
--rw-r--r--   0        0        0      668 2024-03-26 10:44:07.327587 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/__init__.py
--rw-r--r--   0        0        0     2984 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py
--rw-r--r--   0        0        0      579 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py
--rw-r--r--   0        0        0     6774 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py
--rw-r--r--   0        0        0     1766 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py
--rw-r--r--   0        0        0    10881 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py
--rw-r--r--   0        0        0     1971 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py
--rw-r--r--   0        0        0     1194 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py
--rw-r--r--   0        0        0     3054 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py
--rw-r--r--   0        0        0     3000 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py
--rw-r--r--   0        0        0     1572 2024-03-26 10:43:35.735463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py
--rw-r--r--   0        0        0     1753 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py
--rw-r--r--   0        0        0    19489 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py
--rw-r--r--   0        0        0     2808 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py
--rw-r--r--   0        0        0     1688 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py
--rw-r--r--   0        0        0     7200 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/backend_confs.py
--rw-r--r--   0        0        0    23257 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/base_test.py
--rw-r--r--   0        0        0      579 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/__init__.py
--rw-r--r--   0        0        0    10944 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/base_component.py
--rw-r--r--   0        0        0      816 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/conf_table.py
--rw-r--r--   0        0        0      579 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/__init__.py
--rw-r--r--   0        0        0     2537 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/base_control.py
--rw-r--r--   0        0        0     1179 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/button.py
--rw-r--r--   0        0        0     3217 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py
--rw-r--r--   0        0        0     3012 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py
--rw-r--r--   0        0        0     1979 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/message.py
--rw-r--r--   0        0        0     7094 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py
--rw-r--r--   0        0        0     3079 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py
--rw-r--r--   0        0        0    13813 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/single_select.py
--rw-r--r--   0        0        0     2718 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/textarea.py
--rw-r--r--   0        0        0     3119 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/textbox.py
--rw-r--r--   0        0        0     2547 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/toggle.py
--rw-r--r--   0        0        0     8201 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/dropdown.py
--rw-r--r--   0        0        0     4941 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/entity.py
--rw-r--r--   0        0        0     3678 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/input_table.py
--rw-r--r--   0        0        0     1887 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/login.py
--rw-r--r--   0        0        0     5142 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/message_tray.py
--rw-r--r--   0        0        0    22202 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/table.py
--rw-r--r--   0        0        0     1673 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/tabs.py
--rw-r--r--   0        0        0      579 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/__init__.py
--rw-r--r--   0        0        0     2824 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/logging.py
--rw-r--r--   0        0        0     1075 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/login.py
--rw-r--r--   0        0        0     1633 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/page.py
--rw-r--r--   0        0        0     4659 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/proxy.py
--rw-r--r--   0        0        0    10257 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/plugin.py
--rw-r--r--   0        0        0     1156 2024-03-26 10:43:35.739463 pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/utils.py
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 pytest_splunk_addon_ui_smartx-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-05-09 10:47:43.832617 pytest_splunk_addon_ui_smartx-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1782 2024-05-09 10:48:15.605106 pytest_splunk_addon_ui_smartx-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-09 10:48:15.601106 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/__init__.py
+-rw-r--r--   0        0        0     2984 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py
+-rw-r--r--   0        0        0     6774 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py
+-rw-r--r--   0        0        0     1766 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py
+-rw-r--r--   0        0        0    10881 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py
+-rw-r--r--   0        0        0     1971 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py
+-rw-r--r--   0        0        0     1194 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py
+-rw-r--r--   0        0        0     3054 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py
+-rw-r--r--   0        0        0     3000 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py
+-rw-r--r--   0        0        0     1572 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py
+-rw-r--r--   0        0        0     1753 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py
+-rw-r--r--   0        0        0    19489 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py
+-rw-r--r--   0        0        0     2808 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py
+-rw-r--r--   0        0        0     1688 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py
+-rw-r--r--   0        0        0     7200 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/backend_confs.py
+-rw-r--r--   0        0        0    23257 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/base_test.py
+-rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/__init__.py
+-rw-r--r--   0        0        0    10944 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/base_component.py
+-rw-r--r--   0        0        0      816 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/conf_table.py
+-rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/__init__.py
+-rw-r--r--   0        0        0     2537 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/base_control.py
+-rw-r--r--   0        0        0     1179 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/button.py
+-rw-r--r--   0        0        0     3217 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py
+-rw-r--r--   0        0        0     3012 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py
+-rw-r--r--   0        0        0     1979 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/message.py
+-rw-r--r--   0        0        0     7094 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py
+-rw-r--r--   0        0        0     3079 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py
+-rw-r--r--   0        0        0    13813 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/single_select.py
+-rw-r--r--   0        0        0     2718 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textarea.py
+-rw-r--r--   0        0        0     3119 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textbox.py
+-rw-r--r--   0        0        0     2547 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/toggle.py
+-rw-r--r--   0        0        0     8201 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/dropdown.py
+-rw-r--r--   0        0        0     4941 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/entity.py
+-rw-r--r--   0        0        0     3678 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/input_table.py
+-rw-r--r--   0        0        0     1887 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/login.py
+-rw-r--r--   0        0        0     5142 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/message_tray.py
+-rw-r--r--   0        0        0    23658 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/table.py
+-rw-r--r--   0        0        0     1673 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/tabs.py
+-rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/__init__.py
+-rw-r--r--   0        0        0     2824 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/logging.py
+-rw-r--r--   0        0        0     1075 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/login.py
+-rw-r--r--   0        0        0     1633 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/page.py
+-rw-r--r--   0        0        0     4659 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/proxy.py
+-rw-r--r--   0        0        0    10257 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/plugin.py
+-rw-r--r--   0        0        0     1156 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/utils.py
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 pytest_splunk_addon_ui_smartx-3.1.0/PKG-INFO
```

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/LICENSE` & `pytest_splunk_addon_ui_smartx-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pyproject.toml` & `pytest_splunk_addon_ui_smartx-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
 ]
 packages = [
         {include = "pytest_splunk_addon_ui_smartx/**/*.py"},
 ]
-version = "3.0.2"
+version = "3.1.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pytest-html = "*"
 urllib3 = "^1.21.1"
 selenium = "*"
 webdriver-manager = "*"
```

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from . import components, pages
 from .components import controls
 
-__version__ = "3.0.2"
+__version__ = "3.1.0"
```

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/backend_confs.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/backend_confs.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/base_test.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/base_test.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/base_component.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/base_component.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/conf_table.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/conf_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/base_control.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/base_control.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/button.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/button.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/message.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/message.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/single_select.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/single_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/textarea.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textarea.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/textbox.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/controls/toggle.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/toggle.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/dropdown.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/entity.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/entity.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/input_table.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/input_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/login.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/login.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/message_tray.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/message_tray.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/table.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
                     + ' [data-test="cell"][data-column="{column}"]'
                 ),
                 "col-number": Selector(
                     select=container.select + " td:nth-child({col_number})"
                 ),
                 "edit": Selector(select=".editBtn"),
                 "clone": Selector(select=".cloneBtn"),
+                "search": Selector(select=".searchBtn"),
                 "delete": Selector(select=".deleteBtn"),
                 "delete_prompt": Selector(select=".deletePrompt"),  # [data-test="body"]
                 "delete_btn": Selector(select='[data-test="button"][label="Delete"]'),
                 "delete_cancel": Selector(
                     select='[data-test="button"][label="Cancel"]'
                 ),
                 "delete_close": Selector(select='[data-test="close"]'),
@@ -260,14 +261,16 @@
                 each_col = each_col.lower()
                 if each_col == "actions":
                     table[row_name][each_col] = ""
                     if self.edit != None:
                         table[row_name][each_col] = "Edit"
                     if self.clone != None:
                         table[row_name][each_col] += " | Clone"
+                    if self.search != None:
+                        table[row_name][each_col] += " | Search"
                     if self.delete != None:
                         table[row_name][each_col] += " | Delete"
                     continue
                 if each_col == "status":
                     table[row_name][each_col] = each_row.find_element_by_css_selector(
                         '[data-test="status"]'
                     ).text
@@ -309,14 +312,16 @@
         """
         value_list = []
         _row = self._get_row(name)
         if _row.find_element(*list(self.elements["edit"]._asdict().values())) != None:
             value_list.append("Edit")
         if _row.find_element(*list(self.elements["clone"]._asdict().values())) != None:
             value_list.append("Clone")
+        if _row.find_element(*list(self.elements["search"]._asdict().values())) != None:
+            value_list.append("Search")
         if _row.find_element(*list(self.elements["delete"]._asdict().values())) != None:
             value_list.append("Delete")
 
         return value_list
 
     def edit_row(self, name):
         """
@@ -330,14 +335,22 @@
         """
         Clone the specified row. It will open the edit form(entity). The opened entity should be interacted with instance of entity-class only.
             :param name: row_name of the table
         """
         _row = self._get_row(name)
         _row.find_element(*list(self.elements["clone"]._asdict().values())).click()
 
+    def search_row_results(self, name):
+        """
+        Search the results of the selected input. It will open the search and its results in a new tab.
+            :param name: row_name of the table
+        """
+        _row = self._get_row(name)
+        _row.find_element(*list(self.elements["search"]._asdict().values())).click()
+
     def delete_row(self, name, cancel=False, close=False, prompt_msg=False):
         """
         Delete the specified row. Clicking on delete will open a pop-up. Delete the row if neither of (cancel, close) specified.
             :param name: row_name of the table
             :param cancel: if provided, after the popup is opened, click on cancel button and Do Not delete the row
             :param close:  if provided, after the popup is opened, click on close button and Do Not delete the row
             :return: Bool Returns true if successful or returns the string of the delete prompt if looking for prompt message
@@ -543,7 +556,26 @@
 
         _row = self._get_row(row_name)
         try:
             _row.find_element(*list(col._asdict().values()))
             return True
         except exceptions.NoSuchElementException:
             return False
+
+    def __getattr__(self, key):
+        """
+        Makes the web-elements to be accessible directly.
+        - For example self.elements = {"textbox": Selector(by=..., select=...),
+            Access the element by doing self.textbox directly.
+        - It also has implicit wait while finding the element.
+            :param key: The key of the element mentioned in self.elements
+            :returns: The webelement we are accessing
+        """
+        # NOTE: Overriding the implementation for only table component.
+        try:
+            return self.get_element(key)
+        except KeyError:
+            raise
+        except exceptions.TimeoutException:
+            # in case when the element isn't found, return None
+            # so that checks based on this class's properties are in sync.
+            return None
```

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/components/tabs.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/tabs.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/logging.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/logging.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/login.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/login.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/page.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/page.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/pages/proxy.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/proxy.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/plugin.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/pytest_splunk_addon_ui_smartx/utils.py` & `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.0.2/PKG-INFO` & `pytest_splunk_addon_ui_smartx-3.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon-ui-smartx
-Version: 3.0.2
+Version: 3.1.0
 Summary: Library to support testing Splunk Add-on UX
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

