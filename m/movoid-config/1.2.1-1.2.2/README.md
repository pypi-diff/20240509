# Comparing `tmp/movoid_config-1.2.1.tar.gz` & `tmp/movoid_config-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_config-1.2.1.tar", last modified: Mon Apr 22 16:54:38 2024, max compression
+gzip compressed data, was "movoid_config-1.2.2.tar", last modified: Thu May  9 13:04:03 2024, max compression
```

## Comparing `movoid_config-1.2.1.tar` & `movoid_config-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 16:54:38.122822 movoid_config-1.2.1/
--rw-rw-rw-   0        0        0     2330 2024-04-22 16:54:38.121739 movoid_config-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2163 2024-01-08 15:32:17.000000 movoid_config-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 16:54:38.116235 movoid_config-1.2.1/movoid_config/
--rw-rw-rw-   0        0        0      283 2024-02-06 12:25:13.000000 movoid_config-1.2.1/movoid_config/__init__.py
--rw-rw-rw-   0        0        0    19954 2024-04-22 16:52:11.000000 movoid_config-1.2.1/movoid_config/config.py
--rw-rw-rw-   0        0        0     1482 2024-04-22 16:54:22.000000 movoid_config-1.2.1/movoid_config/loop_run.py
-drwxrwxrwx   0        0        0        0 2024-04-22 16:54:38.121739 movoid_config-1.2.1/movoid_config.egg-info/
--rw-rw-rw-   0        0        0     2330 2024-04-22 16:54:38.000000 movoid_config-1.2.1/movoid_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-22 16:54:38.000000 movoid_config-1.2.1/movoid_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 16:54:38.000000 movoid_config-1.2.1/movoid_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-22 16:54:38.000000 movoid_config-1.2.1/movoid_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 16:54:38.122822 movoid_config-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      460 2024-04-22 16:52:11.000000 movoid_config-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:03.723173 movoid_config-1.2.2/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_config-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2330 2024-05-09 13:04:03.714546 movoid_config-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2163 2024-01-08 15:32:17.000000 movoid_config-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:03.706133 movoid_config-1.2.2/movoid_config/
+-rw-rw-rw-   0        0        0      243 2024-05-09 13:02:56.000000 movoid_config-1.2.2/movoid_config/__init__.py
+-rw-rw-rw-   0        0        0    20705 2024-05-09 13:02:56.000000 movoid_config-1.2.2/movoid_config/config.py
+-rw-rw-rw-   0        0        0     1477 2024-05-09 13:02:56.000000 movoid_config-1.2.2/movoid_config/loop_run.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:03.713511 movoid_config-1.2.2/movoid_config.egg-info/
+-rw-rw-rw-   0        0        0     2330 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:04:03.724193 movoid_config-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      460 2024-05-09 13:03:26.000000 movoid_config-1.2.2/setup.py
```

### Comparing `movoid_config-1.2.1/PKG-INFO` & `movoid_config-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movoid_config
-Version: 1.2.1
+Version: 1.2.2
 Home-page: 
 Author: movoid
 Author-email: bobrobotsun@163.com
 Description-Content-Type: text/markdown
 
 This is a simple program for developer to create a param-config reader.
 It only need config_dict and config_file_name to analyse all param and config
```

### Comparing `movoid_config-1.2.1/README.md` & `movoid_config-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `movoid_config-1.2.1/movoid_config/config.py` & `movoid_config-1.2.2/movoid_config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         rule_dict = dict(rule_dict) if rule_dict else {}
         for i, v in rule_dict.items():
             self.add_rule(i, __update=__update, **v)
 
     def init(self, _dict: Dict[str, dict] = None, _file: Union[str, None] = None):
         self.update_rule(_dict)
         self.__config_file = self.__config_file if _file is None else _file
+        self.__value = {}
         self.analyse_config_dict()
         self.read_file()
         self.param_read()
         self.param_default()
         self.param_check()
         self.write_file()
 
@@ -180,15 +181,15 @@
                     self.__config_key['full'][one_config_dict['false']['full']] = [key, 'false']
                 self.__config_key['key'][one_config_dict['key']] = [key, 'bool']
                 self.__config_key['ini'][one_config_dict['ini']] = [key, 'bool']
             else:
                 one_config_dict.setdefault('param', 1)
                 self.__config_key['key'][one_config_dict['key']] = key_type_list
                 self.__config_key['ini'][one_config_dict['ini']] = key_type_list
-                if one_config_dict['type'] in ('file', 'dir'):
+                if one_config_dict['type'] in ('file', 'files', 'dir'):
                     self.__tk = Tk()
                     self.__tk.withdraw()
             if 'single' in one_config_dict:
                 one_config_dict['single'] = str(one_config_dict['single'])[0]
                 self.__config_key['single'][one_config_dict['single']] = key_type_list
             if 'full' in one_config_dict:
                 one_config_dict['full'] = str(one_config_dict['full'])
@@ -281,27 +282,37 @@
         elif target_type == 'file':
             if str_value == '':
                 return str_value
             elif pathlib.Path(str_value).is_file():
                 return str(str_value)
             else:
                 raise Exception(f'{str_value} is not a file.')
+        elif target_type == 'files':
+            if str_value == '':
+                return []
+            else:
+                temp_list = str_value.split(',')
+                path_list = [pathlib.Path(_).is_file() for _ in temp_list]
+                if all(path_list):
+                    return temp_list
+                else:
+                    raise Exception(f'{[_v for _i, _v in enumerate(temp_list) if not path_list[_i]]} is not a file.')
         elif target_type == 'dir':
             if str_value == '':
                 return str_value
             elif pathlib.Path(str_value).is_dir():
                 return str(str_value)
             else:
                 raise Exception(f'{str_value} is not a folder.')
         else:
             return str_value
 
     @staticmethod
     def change_target_value_to_str(target_value, target_type, sub_type=None):
-        if target_type == 'list':
+        if target_type in ('list', 'files'):
             return ','.join([str(_) for _ in target_value])
         elif target_type == 'dict':
             return ','.join([f'{k}:{v}' for k, v in target_value.items()])
         elif target_type == 'kv':
             for k, v in sub_type.items():
                 if v == target_type:
                     return k
@@ -366,26 +377,30 @@
                     raise Exception(f'you must config [{i}] by [{" ; ".join(help_key)}]')
 
     def param_pre_ask(self, key, target_type, sub_type=None):
         if target_type == 'file':
             title = self.__config_dict[key].get('pre_ask_text', 'choose one file to input')
             input_file = filedialog.askopenfilename(title=title)
             return str(input_file)
+        elif target_type == 'files':
+            title = self.__config_dict[key].get('pre_ask_text', 'choose files to input')
+            input_file = filedialog.askopenfilenames(title=title)
+            return ','.join(input_file)
         elif target_type == 'dir':
             title = self.__config_dict[key].get('pre_ask_text', 'choose one folder to input')
             input_file = filedialog.askdirectory(title=title)
             return str(input_file)
 
     def param_ask(self, key):
         while True:
             pre_input = self.param_pre_ask(key, *self.__config_dict[key]['type_list'])
             if pre_input:
                 input_str = pre_input
             else:
-                if self.__config_dict[key]['type'] in ('file', 'dir'):
+                if self.__config_dict[key]['type'] in ('file', 'files', 'dir'):
                     input_ask = f"please input path to config [{key}], or input nothing to choose in dialog window:"
                 elif self.__config_dict[key]['type'] == 'enum':
                     input_ask = f"please input (enum)[" + ', '.join([f"{i + 1}.{v}" for i, v in enumerate(self.__config_dict[key]['sub'])]) + "] to config [{key}]:"
                 else:
                     input_ask = f"please input {self.__config_dict[key]['type_list']} to config [{key}]:"
                 input_str = input(self.__config_dict[key].get('ask_text', input_ask))
             try:
```

### Comparing `movoid_config-1.2.1/movoid_config/loop_run.py` & `movoid_config-1.2.2/movoid_config/loop_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         pass
 
     def start(self):
         while True:
             try:
                 print('process started')
                 self.init_config()
+                self._config.init()
                 self.start_main()
             except Exception as err:
                 print(f'something wrong happened:{err}')
                 traceback.print_exc()
                 self.start_exception()
             finally:
                 self.start_end()
@@ -51,11 +52,7 @@
         pass
 
     def start_end(self):
         pass
 
     def start_exit(self):
         pass
-
-
-if __name__ == '__main__':
-    pass
```

### Comparing `movoid_config-1.2.1/movoid_config.egg-info/PKG-INFO` & `movoid_config-1.2.2/movoid_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movoid_config
-Version: 1.2.1
+Version: 1.2.2
 Home-page: 
 Author: movoid
 Author-email: bobrobotsun@163.com
 Description-Content-Type: text/markdown
 
 This is a simple program for developer to create a param-config reader.
 It only need config_dict and config_file_name to analyse all param and config
```

