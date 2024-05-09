# Comparing `tmp/mainshortcuts-1.6.89.tar.gz` & `tmp/mainshortcuts-1.6.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.89.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.90.tar", max compression
```

## Comparing `mainshortcuts-1.6.89.tar` & `mainshortcuts-1.6.90.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.89/README.md
--rwxr-xr-x   0        0        0      696 2024-05-08 08:44:03.000000 mainshortcuts-1.6.89/pyproject.toml
--rwxr-xr-x   0        0        0     5677 2024-05-07 03:19:44.000000 mainshortcuts-1.6.89/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0      937 2024-05-08 08:43:59.000000 mainshortcuts-1.6.89/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      465 2024-04-28 11:33:14.000000 mainshortcuts-1.6.89/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     4956 2024-05-07 15:08:20.000000 mainshortcuts-1.6.89/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0     1003 2024-05-01 01:56:58.000000 mainshortcuts-1.6.89/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1472 2024-04-28 11:59:24.000000 mainshortcuts-1.6.89/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     4183 2024-05-08 08:41:00.000000 mainshortcuts-1.6.89/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     2923 2024-04-28 12:09:32.000000 mainshortcuts-1.6.89/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     5925 2024-04-28 12:17:10.000000 mainshortcuts-1.6.89/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     2672 2024-05-08 08:44:03.000000 mainshortcuts-1.6.89/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3603 2024-04-28 12:27:24.000000 mainshortcuts-1.6.89/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2174 2024-04-28 12:29:34.000000 mainshortcuts-1.6.89/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.89/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.89/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6265 2024-04-28 12:35:16.000000 mainshortcuts-1.6.89/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      789 2024-04-28 12:36:52.000000 mainshortcuts-1.6.89/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.89/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0      983 2024-04-28 12:40:04.000000 mainshortcuts-1.6.89/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    14818 2024-04-28 12:41:38.000000 mainshortcuts-1.6.89/src/MainShortcuts/values.py
--rwxr-xr-x   0        0        0     1194 2024-04-26 04:58:06.000000 mainshortcuts-1.6.89/src/MainShortcuts/win.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.89/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.90/README.md
+-rwxr-xr-x   0        0        0      696 2024-05-09 12:24:07.000000 mainshortcuts-1.6.90/pyproject.toml
+-rwxr-xr-x   0        0        0     5954 2024-05-08 16:40:54.000000 mainshortcuts-1.6.90/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0     1008 2024-05-09 12:24:00.000000 mainshortcuts-1.6.90/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      495 2024-05-08 16:41:02.000000 mainshortcuts-1.6.90/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     4958 2024-05-08 16:41:08.000000 mainshortcuts-1.6.90/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0     1057 2024-05-08 16:41:00.000000 mainshortcuts-1.6.90/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1538 2024-05-08 16:41:02.000000 mainshortcuts-1.6.90/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     4183 2024-05-08 08:41:00.000000 mainshortcuts-1.6.90/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     3043 2024-05-08 16:40:46.000000 mainshortcuts-1.6.90/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     6183 2024-05-08 16:41:04.000000 mainshortcuts-1.6.90/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     2731 2024-05-09 12:24:11.000000 mainshortcuts-1.6.90/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3818 2024-05-09 12:23:15.000000 mainshortcuts-1.6.90/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2292 2024-05-08 16:41:06.000000 mainshortcuts-1.6.90/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1073 2024-05-08 16:40:46.000000 mainshortcuts-1.6.90/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       93 2024-05-08 16:40:46.000000 mainshortcuts-1.6.90/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6585 2024-05-08 16:40:58.000000 mainshortcuts-1.6.90/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      857 2024-05-08 16:41:06.000000 mainshortcuts-1.6.90/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0     1507 2024-05-08 16:40:50.000000 mainshortcuts-1.6.90/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0     1047 2024-05-08 16:41:08.000000 mainshortcuts-1.6.90/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    15238 2024-05-08 16:40:50.000000 mainshortcuts-1.6.90/src/MainShortcuts/values.py
+-rwxr-xr-x   0        0        0     1327 2024-05-08 16:41:00.000000 mainshortcuts-1.6.90/src/MainShortcuts/win.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.90/PKG-INFO
```

### Comparing `mainshortcuts-1.6.89/README.md` & `mainshortcuts-1.6.90/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.89/pyproject.toml` & `mainshortcuts-1.6.90/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "1.6.89"
+version = "1.6.90"
 name = "MainShortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.90/src/MainShortcuts/MainCore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,146 +1,156 @@
-import os,sys,traceback
+import os
+import sys
+import traceback
 import MainShortcuts as ms
 from MainShortcuts.dictplus import dictplus
+
+
 class _MainCore:
   """Переменные:
   .args - то же самое, что и sys.argv
   .dir - папка с текущей программой (использует __file__)
   .execdir - если программа находится в папке "_internal", указана родительская папка
   .embed - тексты для всраивания MainCore в программу
   .run - запущена ли программа или её импортируют? (использует __name__)"""
-  def __init__(self,color:bool=True,*,__name__,__file__):
-    self.args=sys.argv
-    self.core_name="MainCore"
-    self.core_version=5
-    self.dir=os.path.dirname(__file__) # Папка, в которой находится программа
-    self.execdir=self.dir # Если программа собрана через "pyinstaller --onedir", указывает папку с исполняемым файлом
+
+  def __init__(self, color: bool = True, *, __name__, __file__):
+    self.args = sys.argv
+    self.core_name = "MainCore"
+    self.core_version = 5
+    self.dir = os.path.dirname(__file__)  # Папка, в которой находится программа
+    self.execdir = self.dir  # Если программа собрана через "pyinstaller --onedir", указывает папку с исполняемым файлом
     try:
-      tmp=os.path.split(self.dir)
-      if tmp[1]=="_internal":
-        self.execdir=tmp[0]
+      tmp = os.path.split(self.dir)
+      if tmp[1] == "_internal":
+        self.execdir = tmp[0]
     except:
       pass
-    self.exception=traceback.format_exc # Получить traceback в виде текста
-    self.pid=os.getpid() # PID программы
-    self.run=__name__=="__main__" # Запущена программа или её импортируют?
-    self.embed=dictplus()
-    self.embed.lines=[
-      "from MainShortcuts.MainCore import *",
-      "from MainShortcuts.MainCore import _MainCore",
-      "mcore=_MainCore(__name__=__name__,__file__=__file__)",
-      "cprint,cformat=mcore.cprint,mcore.cformat",
-      "globals=dictplus()",
-      'cfg=ms.cfg(mcore.execdir+"/cfg.json")',
-      "cfg.default={}",
-      "cfg.dload()",
-      ]
-    self.embed.text="\n".join(self.embed.lines)+"\n" # Текст для встраивания MainCore в программу
-    self.color_names=[
-      "",
-      "BG_BLACK",
-      "BG_BLUE",
-      "BG_GREEN",
-      "BG_LIGHTBLACK",
-      "BG_LIGHTBLUE",
-      "BG_LIGHTGREEN",
-      "BG_LIGHTPINK",
-      "BG_LIGHTRED",
-      "BG_LIGHTWHITE",
-      "BG_LIGHTYELLOW",
-      "BG_PINK",
-      "BG_RED",
-      "BG_WHITE",
-      "BG_YELLOW",
-      "BLACK",
-      "BLUE",
-      "GREEN",
-      "HIGH",
-      "LIGHTBLACK",
-      "LIGHTBLUE",
-      "LIGHTGREEN",
-      "LIGHTPINK",
-      "LIGHTRED",
-      "LIGHTWHITE",
-      "LIGHTYELLOW",
-      "LOW",
-      "PINK",
-      "RED",
-      "RESET",
-      "WHITE",
-      "YELLOW",
-      ]
-    self.colors={}
+    self.exception = traceback.format_exc  # Получить traceback в виде текста
+    self.pid = os.getpid()  # PID программы
+    self.run = __name__ == "__main__"  # Запущена программа или её импортируют?
+    self.embed = dictplus()
+    self.embed.lines = [
+        "from MainShortcuts.MainCore import *",
+        "from MainShortcuts.MainCore import _MainCore",
+        "mcore=_MainCore(__name__=__name__,__file__=__file__)",
+        "cprint,cformat=mcore.cprint,mcore.cformat",
+        "globals=dictplus()",
+        'cfg=ms.cfg(mcore.execdir+"/cfg.json")',
+        "cfg.default={}",
+        "cfg.dload()",
+    ]
+    self.embed.text = "\n".join(self.embed.lines) + "\n"  # Текст для встраивания MainCore в программу
+    self.color_names = [
+        "",
+        "BG_BLACK",
+        "BG_BLUE",
+        "BG_GREEN",
+        "BG_LIGHTBLACK",
+        "BG_LIGHTBLUE",
+        "BG_LIGHTGREEN",
+        "BG_LIGHTPINK",
+        "BG_LIGHTRED",
+        "BG_LIGHTWHITE",
+        "BG_LIGHTYELLOW",
+        "BG_PINK",
+        "BG_RED",
+        "BG_WHITE",
+        "BG_YELLOW",
+        "BLACK",
+        "BLUE",
+        "GREEN",
+        "HIGH",
+        "LIGHTBLACK",
+        "LIGHTBLUE",
+        "LIGHTGREEN",
+        "LIGHTPINK",
+        "LIGHTRED",
+        "LIGHTWHITE",
+        "LIGHTYELLOW",
+        "LOW",
+        "PINK",
+        "RED",
+        "RESET",
+        "WHITE",
+        "YELLOW",
+    ]
+    self.colors = {}
     for i in self.color_names:
-      self.colors[i]=""
+      self.colors[i] = ""
     if color:
       try:
         import colorama as clr
         clr.init()
-        self.colors["BG_BLACK"]=clr.Back.BLACK
-        self.colors["BG_BLUE"]=clr.Back.BLUE
-        self.colors["BG_GREEN"]=clr.Back.GREEN
-        self.colors["BG_LIGHTBLACK"]=clr.Back.LIGHTBLACK_EX
-        self.colors["BG_LIGHTBLUE"]=clr.Back.LIGHTBLUE_EX
-        self.colors["BG_LIGHTGREEN"]=clr.Back.LIGHTGREEN_EX
-        self.colors["BG_LIGHTPINK"]=clr.Back.LIGHTMAGENTA_EX
-        self.colors["BG_LIGHTRED"]=clr.Back.LIGHTRED_EX
-        self.colors["BG_LIGHTWHITE"]=clr.Back.LIGHTWHITE_EX
-        self.colors["BG_LIGHTYELLOW"]=clr.Back.LIGHTYELLOW_EX
-        self.colors["BG_PINK"]=clr.Back.MAGENTA
-        self.colors["BG_RED"]=clr.Back.RED
-        self.colors["BG_WHITE"]=clr.Back.WHITE
-        self.colors["BG_YELLOW"]=clr.Back.YELLOW
-        self.colors["BLACK"]=clr.Fore.BLACK
-        self.colors["BLUE"]=clr.Fore.BLUE
-        self.colors["GREEN"]=clr.Fore.GREEN
-        self.colors["HIGH"]=clr.Style.BRIGHT
-        self.colors["LIGHTBLACK"]=clr.Fore.LIGHTBLACK_EX
-        self.colors["LIGHTBLUE"]=clr.Fore.LIGHTBLUE_EX
-        self.colors["LIGHTGREEN"]=clr.Fore.LIGHTGREEN_EX
-        self.colors["LIGHTPINK"]=clr.Fore.LIGHTMAGENTA_EX
-        self.colors["LIGHTRED"]=clr.Fore.LIGHTRED_EX
-        self.colors["LIGHTWHITE"]=clr.Fore.LIGHTWHITE_EX
-        self.colors["LIGHTYELLOW"]=clr.Fore.LIGHTYELLOW_EX
-        self.colors["LOW"]=clr.Style.DIM
-        self.colors["PINK"]=clr.Fore.MAGENTA
-        self.colors["RED"]=clr.Fore.RED
-        self.colors["RESET"]=clr.Style.RESET_ALL
-        self.colors["WHITE"]=clr.Fore.WHITE
-        self.colors["YELLOW"]=clr.Fore.YELLOW
+        self.colors["BG_BLACK"] = clr.Back.BLACK
+        self.colors["BG_BLUE"] = clr.Back.BLUE
+        self.colors["BG_GREEN"] = clr.Back.GREEN
+        self.colors["BG_LIGHTBLACK"] = clr.Back.LIGHTBLACK_EX
+        self.colors["BG_LIGHTBLUE"] = clr.Back.LIGHTBLUE_EX
+        self.colors["BG_LIGHTGREEN"] = clr.Back.LIGHTGREEN_EX
+        self.colors["BG_LIGHTPINK"] = clr.Back.LIGHTMAGENTA_EX
+        self.colors["BG_LIGHTRED"] = clr.Back.LIGHTRED_EX
+        self.colors["BG_LIGHTWHITE"] = clr.Back.LIGHTWHITE_EX
+        self.colors["BG_LIGHTYELLOW"] = clr.Back.LIGHTYELLOW_EX
+        self.colors["BG_PINK"] = clr.Back.MAGENTA
+        self.colors["BG_RED"] = clr.Back.RED
+        self.colors["BG_WHITE"] = clr.Back.WHITE
+        self.colors["BG_YELLOW"] = clr.Back.YELLOW
+        self.colors["BLACK"] = clr.Fore.BLACK
+        self.colors["BLUE"] = clr.Fore.BLUE
+        self.colors["GREEN"] = clr.Fore.GREEN
+        self.colors["HIGH"] = clr.Style.BRIGHT
+        self.colors["LIGHTBLACK"] = clr.Fore.LIGHTBLACK_EX
+        self.colors["LIGHTBLUE"] = clr.Fore.LIGHTBLUE_EX
+        self.colors["LIGHTGREEN"] = clr.Fore.LIGHTGREEN_EX
+        self.colors["LIGHTPINK"] = clr.Fore.LIGHTMAGENTA_EX
+        self.colors["LIGHTRED"] = clr.Fore.LIGHTRED_EX
+        self.colors["LIGHTWHITE"] = clr.Fore.LIGHTWHITE_EX
+        self.colors["LIGHTYELLOW"] = clr.Fore.LIGHTYELLOW_EX
+        self.colors["LOW"] = clr.Style.DIM
+        self.colors["PINK"] = clr.Fore.MAGENTA
+        self.colors["RED"] = clr.Fore.RED
+        self.colors["RESET"] = clr.Style.RESET_ALL
+        self.colors["WHITE"] = clr.Fore.WHITE
+        self.colors["YELLOW"] = clr.Fore.YELLOW
       except:
-        color=False
+        color = False
+
   def __repr__(self):
-    return ms.json.encode({"name":self.core_name,"version":self.core_version},mode="c")
-  def cprint(self,a:str,start:str="",**kwargs): # Вывести цветной текст | cprint("Обычный текст, {BLUE}Синий текст")
+    return ms.json.encode({"name": self.core_name, "version": self.core_version}, mode="c")
+
+  def cprint(self, a: str, start: str = "", **kwargs):  # Вывести цветной текст | cprint("Обычный текст, {BLUE}Синий текст")
     try:
-      b=str(a).rstrip().format(**self.colors)
+      b = str(a).rstrip().format(**self.colors)
     except KeyError:
-      b=str(a).rstrip()
-      for k,v in self.colors.items():
+      b = str(a).rstrip()
+      for k, v in self.colors.items():
         try:
-          arg={k:v}
-          b=b.format(**arg)
+          arg = {k: v}
+          b = b.format(**arg)
         except KeyError:
           pass
-    print(self.colors["RESET"]+self.colors[start]+b.rstrip()+self.colors["RESET"],**kwargs)
-  def cformat(self,a:str,start:str="")->str: # Аналогично cprint, но вывод в return, и нет strip
+    print(self.colors["RESET"] + self.colors[start] + b.rstrip() + self.colors["RESET"], **kwargs)
+
+  def cformat(self, a: str, start: str = "") -> str:  # Аналогично cprint, но вывод в return, и нет strip
     try:
-      b=str(a).format(**self.colors)
+      b = str(a).format(**self.colors)
     except KeyError:
-      b=str(a).rstrip()
-      for k,v in self.colors.items():
+      b = str(a).rstrip()
+      for k, v in self.colors.items():
         try:
-          arg={k:v}
-          b=b.format(**arg)
+          arg = {k: v}
+          b = b.format(**arg)
         except KeyError:
           pass
-    return self.colors["RESET"]+self.colors[start]+b+self.colors["RESET"]
-  def ctest(self): # Вывод всех доступных цветов
-    for k,v in self.colors.items():
-      if k!="":
-        print("{0}{1}: {2}EXAMPLE ░▒▓ ███{0}".format(self.colors["RESET"],k,v))
-  def ignoreException(self,target,*args,**kwargs):
+    return self.colors["RESET"] + self.colors[start] + b + self.colors["RESET"]
+
+  def ctest(self):  # Вывод всех доступных цветов
+    for k, v in self.colors.items():
+      if k != "":
+        print("{0}{1}: {2}EXAMPLE ░▒▓ ███{0}".format(self.colors["RESET"], k, v))
+
+  def ignoreException(self, target, *args, **kwargs):
     try:
-      return target(*args,**kwargs)
+      return target(*args, **kwargs)
     except:
       return self.exception()
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.90/src/MainShortcuts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
 https://t.me/MainPlay_InfoCh"""
 
-__version_tuple__=(1,6,89)
-__depends__={
-  "required":[
-    "json",
-    "os",
-    "platform",
-    "shutil",
-    "subprocess",
-    "sys",
+__version_tuple__ = (1, 6, 90)
+__depends__ = {
+    "required": [
+        "json",
+        "os",
+        "platform",
+        "shutil",
+        "subprocess",
+        "sys",
     ],
-  "optional":[
-    "colorama",
-    "cPickle",
-    "hashlib",
-    "pickle",
-    "toml",
+    "optional": [
+        "colorama",
+        "cPickle",
+        "hashlib",
+        "pickle",
+        "toml",
     ]
-  }
-__scripts__=[
-  "MS-getCore",
-  "MS-getCoreMini",
-  "MS-jsonC",
-  "MS-jsonP",
-  "MS-mkdir",
-  ]
+}
+__scripts__ = [
+    "MS-getCore",
+    "MS-getCoreMini",
+    "MS-jsonC",
+    "MS-jsonP",
+    "MS-mkdir",
+]
 from MainShortcuts.imports import *
-__all__=imports_all.copy()
-__import_errors__=imports_import_errors.copy()
-del imports_all,imports_import_errors
-__version__="{}.{}.{}".format(*__version_tuple__)
+__all__ = imports_all.copy()
+__import_errors__ = imports_import_errors.copy()
+del imports_all, imports_import_errors
+__version__ = "{}.{}.{}".format(*__version_tuple__)
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/cfg.py` & `mainshortcuts-1.6.90/src/MainShortcuts/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     if path == None:
       path = self.path
     if type == None:
       type = self.type
     else:
       type = _checkType(path, type)
     _checkImport(type)
-    if os.path.dirname(path)!="":
+    if os.path.dirname(path) != "":
       m_dir.create(os.path.dirname(path), force=force)
     if type == "json":
       kw["encoding"] = encoding
       json.write(path, self.data, **kw)
     elif type == "pickle":
       with open(path, "wb") as f:
         pickle.dump(self.data, f, **kw)
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.90/src/MainShortcuts/dictplus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 class dictplus:
   """Улучшенный словарь
   Можно получить элементы и через dictplus["key"], и через dictplus.key
   Вариант использования через аттрибуты может работать не на все ключи"""
-  def __init__(self,data:dict=None):
+
+  def __init__(self, data: dict = None):
     """Без аргументов создаётся {}
     Аргументом можно указать любой словарь"""
-    if data==None:
-      self.__data__={}
+    if data == None:
+      self.__data__ = {}
     else:
-      self.__data__=data.copy()
-  def __getattr__(self,k):
-    if k=="__data__":
+      self.__data__ = data.copy()
+
+  def __getattr__(self, k):
+    if k == "__data__":
       return self.__dict__[k]
     else:
       return self[k]
-  def __setattr__(self,k,v):
-    if k=="__data__":
-      self.__dict__[k]=v
+
+  def __setattr__(self, k, v):
+    if k == "__data__":
+      self.__dict__[k] = v
     else:
-      self[k]=v
+      self[k] = v
+
   def __repr__(self):
     return f"dictplus({str(self.__data__)})"
+
   def __dir__(self):
-    return list(self.__data__.keys())+["__data__"]
+    return list(self.__data__.keys()) + ["__data__"]
+
   def __len__(self):
     return len(self.__data__.keys())
-  def __contains__(self,k):
+
+  def __contains__(self, k):
     return (k in self.__data__)
-  __hasattr__=__contains__
-  def __eq__(self,o):
-    if type(o)==dict:
-      return self.__data__==o
+  __hasattr__ = __contains__
+
+  def __eq__(self, o):
+    if type(o) == dict:
+      return self.__data__ == o
     else:
-      return self.__data__==o.__data__
-  def __getitem__(self,k):
+      return self.__data__ == o.__data__
+
+  def __getitem__(self, k):
     return self.__dict__["__data__"][k]
-  def __setitem__(self,k,v):
-    self.__dict__["__data__"][k]=v
-  def __delitem__(self,k):
+
+  def __setitem__(self, k, v):
+    self.__dict__["__data__"][k] = v
+
+  def __delitem__(self, k):
+    self.__dict__["__data__"].pop(k)
+
+  def __delattr__(self, k):
     self.__dict__["__data__"].pop(k)
-  def __delattr__(self,k):
-    self.__dict__["__data__"].pop(k)
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.90/src/MainShortcuts/dir.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/file.py` & `mainshortcuts-1.6.90/src/MainShortcuts/file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,102 @@
 import MainShortcuts.path as m_path
 import os as _os
 import shutil as _shutil
-_open=open
-def read(path:str,encoding:str="utf-8"):
+_open = open
+
+
+def read(path: str, encoding: str = "utf-8"):
   """Прочитать файл как текст
   encoding - кодировка
   Если файла нет, возвращает пустую строку"""
   if _os.path.isfile(path):
-    with _open(path,"rb") as f:
-      text=f.read().decode(encoding)
+    with _open(path, "rb") as f:
+      text = f.read().decode(encoding)
   else:
-    text=""
+    text = ""
   return text
-def write(path:str,text:str="",encoding:str="utf-8",force=False):
+
+
+def write(path: str, text: str = "", encoding: str = "utf-8", force=False):
   """Записать текст в файл
   text - текст для записи
   encoding - кодировка
   force - принудительно создать файл"""
   if _os.path.isdir(path) and force:
     m_path.rm(path)
-  with _open(path,"wb") as f:
+  with _open(path, "wb") as f:
     f.write(str(text).encode(encoding))
   return True
-def open(path:str):
+
+
+def open(path: str):
   """Прочитать файл как байты
   Если файла нет, возвращает пустые байты"""
   if _os.path.isfile(path):
-    with _open(path,"rb") as f:
-      content=f.read()
+    with _open(path, "rb") as f:
+      content = f.read()
   else:
-    content=b""
+    content = b""
   return content
-load=open
-def save(path:str,content=b"",force=False):
+
+
+load = open
+
+
+def save(path: str, content=b"", force=False):
   """Записать байты в файл
   content - байты для записи
   force - принудительно создать файл"""
   if _os.path.isdir(path) and force:
     m_path.rm(path)
-  with _open(path,"wb") as f:
+  with _open(path, "wb") as f:
     f.write(content)
   return True
-def delete(path:str):
+
+
+def delete(path: str):
   """Удалить файл
   Если он не существует, ничего не изменится
   Если на месте папка, выдаст ошибку"""
-  type=m_path.info(path)["type"]
-  if type=="file":
+  type = m_path.info(path)["type"]
+  if type == "file":
     m_path.rm(path)
   elif not _os.path.exists(path):
     pass
   else:
-    raise Exception("Unknown type: "+type)
-def copy(fr:str,to:str,force:bool=False):
+    raise Exception("Unknown type: " + type)
+
+
+def copy(fr: str, to: str, force: bool = False):
   """Копировать файл
   force - если в месте назначения папка, удалить её"""
-  type=m_path.info(fr)["type"]
-  if type=="file":
+  type = m_path.info(fr)["type"]
+  if type == "file":
     if m_path.exists(to) and force:
       m_path.delete(to)
-    _shutil.copy(fr,to)
+    _shutil.copy(fr, to)
   else:
-    raise Exception("Unknown type: "+type)
-def move(fr:str,to:str,force:bool=False):
+    raise Exception("Unknown type: " + type)
+
+
+def move(fr: str, to: str, force: bool = False):
   """Переместить файл
   force - если в месте назначения папка, удалить её"""
-  type=m_path.info(fr)["type"]
-  if type=="file":
+  type = m_path.info(fr)["type"]
+  if type == "file":
     if m_path.exists(to) and force:
       m_path.delete(to)
-    _shutil.move(fr,to)
+    _shutil.move(fr, to)
   else:
-    raise Exception("Unknown type: "+type)
-def rename(fr:str,to:str,force:bool=False):
+    raise Exception("Unknown type: " + type)
+
+
+def rename(fr: str, to: str, force: bool = False):
   """Переименовать файл
   force - если в месте назначения папка, удалить её"""
-  type=m_path.info(fr)["type"]
-  if type=="file":
+  type = m_path.info(fr)["type"]
+  if type == "file":
     if m_path.exists(to) and force:
       m_path.delete(to)
-    _os.rename(fr,to)
+    _os.rename(fr, to)
   else:
-    raise Exception("Unknown type: "+type)
+    raise Exception("Unknown type: " + type)
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.90/src/MainShortcuts/fileobj.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,217 +1,241 @@
-import os, shutil
+import os
+import shutil
 try:
   import hashlib as hl
-  hl_err=False
+  hl_err = False
 except Exception as e:
-  hl_err=e
+  hl_err = e
+
+
 class hash:
   """Получить контрольные суммы и размер файла
   Может зависнуть при больших файлах"""
-  def __init__(self,path:str):
-    if hl_err!=False:
+
+  def __init__(self, path: str):
+    if hl_err != False:
       raise hl_err
-    algs=[
-      "blake2b",
-      "blake2s",
-      "md5",
-      "sha1",
-      "sha224",
-      "sha256",
-      "sha384",
-      "sha3_224",
-      "sha3_256",
-      "sha3_384",
-      "sha3_512",
-      "sha512",
-      ]
-    self.size=os.path.getsize(path)
-    with open(path,"rb") as f:
-      b=f.read()
+    algs = [
+        "blake2b",
+        "blake2s",
+        "md5",
+        "sha1",
+        "sha224",
+        "sha256",
+        "sha384",
+        "sha3_224",
+        "sha3_256",
+        "sha3_384",
+        "sha3_512",
+        "sha512",
+    ]
+    self.size = os.path.getsize(path)
+    with open(path, "rb") as f:
+      b = f.read()
       for i in algs:
-        self[i]=getattr(hl,i)(b).hexdigest()
-  def __getitem__(self,k):
-    return getattr(self,k)
-  def __setitem__(self,k,v):
-    setattr(self,k,v)
+        self[i] = getattr(hl, i)(b).hexdigest()
+
+  def __getitem__(self, k):
+    return getattr(self, k)
+
+  def __setitem__(self, k, v):
+    setattr(self, k, v)
+
+
 class fileobj:
   """Улучшенная работа с файлом
   Переменные класса:
     .content / .data / .bytes - байты файла (получить/записать)
     .text / .str - текст файла (получить/записать)
     .lines - текстовые линии файла (получить/записать)
     .size - размер файла в байтах. Если force=True и файл отсутствует, возвращает 0
     .exists - существует ли файл?"""
-  def __init__(self,p:str,encoding:str="utf-8",force:bool=False):
+
+  def __init__(self, p: str, encoding: str = "utf-8", force: bool = False):
     """
     p - путь к файлу
     encoding - кодировка (при работе с текстом)
     force - принудительно выполнять"""
     if os.path.isdir(p) and not force:
       raise IsADirectoryError("Can't work with folder")
-    self.encoding=encoding
-    self.force=force
-    self.path=p
-  def __getattr__(self,k):
-    if k in ["content","data","bytes"]:
+    self.encoding = encoding
+    self.force = force
+    self.path = p
+
+  def __getattr__(self, k):
+    if k in ["content", "data", "bytes"]:
       return self.open()
-    elif k in ["text","str"]:
+    elif k in ["text", "str"]:
       return self.read()
-    elif k=="lines":
+    elif k == "lines":
       return self.read().split("\n")
-    elif k=="size":
+    elif k == "size":
       if self.force and not os.path.exists(self.path):
         return 0
       return os.path.getsize(self.path)
-    elif k=="exists":
+    elif k == "exists":
       return os.path.exists(self.path)
-    elif k=="__dict__":
+    elif k == "__dict__":
       return self.__dict__
     else:
       return self.__dict__[k]
-  def __setattr__(self,k,v):
-    nochange=[
-      "checksum",
-      "copy",
-      "delete",
-      "exists",
-      "link",
-      "move",
-      "open",
-      "read",
-      "save",
-      "size",
-      "write",
-      ]
-    if k in ["content","data","bytes"]:
+
+  def __setattr__(self, k, v):
+    nochange = [
+        "checksum",
+        "copy",
+        "delete",
+        "exists",
+        "link",
+        "move",
+        "open",
+        "read",
+        "save",
+        "size",
+        "write",
+    ]
+    if k in ["content", "data", "bytes"]:
       self.save(v)
-    elif k in ["text","str"]:
+    elif k in ["text", "str"]:
       self.write(v)
-    elif k=="lines":
+    elif k == "lines":
       self.write("\n".join(list(v)))
     elif k in nochange:
       raise AttributeError("This attribute cannot be changed")
-    elif k=="__dict__":
-      self.__dict__=v
+    elif k == "__dict__":
+      self.__dict__ = v
     else:
-      self.__dict__[k]=v
-  def __getitem__(self,k):
+      self.__dict__[k] = v
+
+  def __getitem__(self, k):
     return self.lines[k]
-  def __setitem__(self,k,v):
-    self.lines[k]=v
+
+  def __setitem__(self, k, v):
+    self.lines[k] = v
+
   def __dir__(self):
-    f=[
-      "checksum",
-      "copy",
-      "delete",
-      "link",
-      "move",
-      "open",
-      "read",
-      "save",
-      "write",
-      ]
-    f2=[
-      "cp",
-      "hash",
-      "ln",
-      "load",
-      "mv",
-      "rm",
-      ]
-    v=[
-      "bytes",
-      "content",
-      "data",
-      "encoding",
-      "exists",
-      "force",
-      "lines",
-      "path",
-      "size",
-      "str",
-      "text",
-      ]
-    return v+f+f2
+    f = [
+        "checksum",
+        "copy",
+        "delete",
+        "link",
+        "move",
+        "open",
+        "read",
+        "save",
+        "write",
+    ]
+    f2 = [
+        "cp",
+        "hash",
+        "ln",
+        "load",
+        "mv",
+        "rm",
+    ]
+    v = [
+        "bytes",
+        "content",
+        "data",
+        "encoding",
+        "exists",
+        "force",
+        "lines",
+        "path",
+        "size",
+        "str",
+        "text",
+    ]
+    return v + f + f2
+
   def __repr__(self):
     return f"ms.fileobj('{self.path}',encoding='{self.encoding}',force={self.force})"
-  def open(self)->bytes:
+
+  def open(self) -> bytes:
     """Получить байты из файла"""
     if self.force:
       try:
-        with open(self.path,"rb") as f:
-          a=f.read()
+        with open(self.path, "rb") as f:
+          a = f.read()
       except:
-        a=b""
+        a = b""
     else:
-      with open(self.path,"rb") as f:
-        a=f.read()
+      with open(self.path, "rb") as f:
+        a = f.read()
     return a
-  def save(self,v:bytes):
+
+  def save(self, v: bytes):
     """Записать байты в файл"""
     if self.force:
       if os.path.isdir(self.path):
         shutil.rmtree(self.path)
-      if type(v)!=bytes:
-        v=str(v).encode(self.encoding)
-    with open(self.path,"wb") as f:
-      a=f.write(v)
+      if type(v) != bytes:
+        v = str(v).encode(self.encoding)
+    with open(self.path, "wb") as f:
+      a = f.write(v)
     return a
-  def read(self)->str:
+
+  def read(self) -> str:
     """Получить текст из файла"""
     return self.open().decode(self.encoding)
-  def write(self,v:str):
+
+  def write(self, v: str):
     """Записать текст в файл"""
     return self.save(v.encode(self.encoding))
+
   def delete(self):
     """Удалить файл"""
     if os.path.islink(self.path):
       os.unlink(self.path)
     elif os.path.isfile(self.path):
       os.remove(self.path)
     elif os.path.isdir(self.path):
       shutil.rmtree(self.path)
-  def move(self,dest:str,follow:bool=True):
+
+  def move(self, dest: str, follow: bool = True):
     """Переместить файл
     follow - следовать за файлом"""
     if os.path.exists(dest) and self.force:
       if os.path.islink(dest):
         os.unlink(dest)
       elif os.path.isfile(dest):
         os.remove(dest)
       elif os.path.isdir(dest):
         shutil.rmtree(dest)
-    shutil.move(self.path,dest)
+    shutil.move(self.path, dest)
     if follow:
-      self.path=dest
-  def copy(self,dest:str,follow:bool=False):
+      self.path = dest
+
+  def copy(self, dest: str, follow: bool = False):
     """Копировать файл
     follow - следовать за файлом"""
     if os.path.exists(dest) and self.force:
       if os.path.islink(dest):
         os.unlink(dest)
       elif os.path.isfile(dest):
         os.remove(dest)
       elif os.path.isdir(dest):
         shutil.rmtree(dest)
-    shutil.copy(self.path,dest)
+    shutil.copy(self.path, dest)
     if follow:
-      self.path=dest
-  def link(self,dest:str):
+      self.path = dest
+
+  def link(self, dest: str):
     """Сделать символическую ссылку на файл"""
     if os.path.exists(dest) and self.force:
       if os.path.islink(dest):
         os.unlink(dest)
       elif os.path.isfile(dest):
         os.remove(dest)
       elif os.path.isdir(dest):
         shutil.rmtree(dest)
-    os.symlink(self.path,dest)
-  def checksum(self)->hash:
+    os.symlink(self.path, dest)
+
+  def checksum(self) -> hash:
     """Получить контрольные суммы и размер файла"""
     return hash(self.path)
-  cp=copy
-  hash=checksum
-  ln=link
-  load=open
-  mv=move
-  rm=delete
+  cp = copy
+  hash = checksum
+  ln = link
+  load = open
+  mv = move
+  rm = delete
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.90/src/MainShortcuts/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,106 @@
 """Этот файл просто импортирует части модуля
 Он создаётся автоматически"""
 import MainShortcuts.main as main
-imports_all=[]
-imports_import_errors={}
+imports_all = []
+imports_import_errors = {}
 try:
-  cd=main.cd
+  cd = main.cd
   imports_all.append('cd')
 except Exception as e:
-  imports_import_errors['cd']=e
+  imports_import_errors['cd'] = e
 try:
-  clear_ANSI=main.clear_ANSI
+  clear_ANSI = main.clear_ANSI
   imports_all.append('clear_ANSI')
 except Exception as e:
-  imports_import_errors['clear_ANSI']=e
+  imports_import_errors['clear_ANSI'] = e
 try:
-  cls_ANSI=main.cls_ANSI
+  cls_ANSI = main.cls_ANSI
   imports_all.append('cls_ANSI')
 except Exception as e:
-  imports_import_errors['cls_ANSI']=e
+  imports_import_errors['cls_ANSI'] = e
 try:
-  clear=main.clear
+  clear = main.clear
   imports_all.append('clear')
 except Exception as e:
-  imports_import_errors['clear']=e
+  imports_import_errors['clear'] = e
 try:
-  cls=main.cls
+  cls = main.cls
   imports_all.append('cls')
 except Exception as e:
-  imports_import_errors['cls']=e
+  imports_import_errors['cls'] = e
 try:
-  exit=main.exit
+  exit = main.exit
   imports_all.append('exit')
 except Exception as e:
-  imports_import_errors['exit']=e
+  imports_import_errors['exit'] = e
 try:
-  pwd=main.pwd
+  pwd = main.pwd
   imports_all.append('pwd')
 except Exception as e:
-  imports_import_errors['pwd']=e
+  imports_import_errors['pwd'] = e
 try:
   from MainShortcuts.cfg import cfg
   imports_all.append('cfg')
 except Exception as e:
-  imports_import_errors['cfg']=e
+  imports_import_errors['cfg'] = e
 try:
   from MainShortcuts.dictplus import dictplus
   imports_all.append('dictplus')
 except Exception as e:
-  imports_import_errors['dictplus']=e
+  imports_import_errors['dictplus'] = e
 try:
   from MainShortcuts.fileobj import fileobj
   imports_all.append('fileobj')
 except Exception as e:
-  imports_import_errors['fileobj']=e
+  imports_import_errors['fileobj'] = e
 try:
   import MainShortcuts.dict as dict
   imports_all.append('dict')
 except Exception as e:
-  imports_import_errors['dict']=e
+  imports_import_errors['dict'] = e
 try:
   import MainShortcuts.dir as dir
   imports_all.append('dir')
 except Exception as e:
-  imports_import_errors['dir']=e
+  imports_import_errors['dir'] = e
 try:
   import MainShortcuts.file as file
   imports_all.append('file')
 except Exception as e:
-  imports_import_errors['file']=e
+  imports_import_errors['file'] = e
 try:
   import MainShortcuts.json as json
   imports_all.append('json')
 except Exception as e:
-  imports_import_errors['json']=e
+  imports_import_errors['json'] = e
 try:
   import MainShortcuts.list as list
   imports_all.append('list')
 except Exception as e:
-  imports_import_errors['list']=e
+  imports_import_errors['list'] = e
 try:
   import MainShortcuts.os as os
   imports_all.append('os')
 except Exception as e:
-  imports_import_errors['os']=e
+  imports_import_errors['os'] = e
 try:
   import MainShortcuts.path as path
   imports_all.append('path')
 except Exception as e:
-  imports_import_errors['path']=e
+  imports_import_errors['path'] = e
 try:
   import MainShortcuts.proc as proc
   imports_all.append('proc')
 except Exception as e:
-  imports_import_errors['proc']=e
+  imports_import_errors['proc'] = e
 try:
   import MainShortcuts.str as str
   imports_all.append('str')
 except Exception as e:
-  imports_import_errors['str']=e
+  imports_import_errors['str'] = e
 try:
   import MainShortcuts.win as win
   imports_all.append('win')
 except Exception as e:
-  imports_import_errors['win']=e
-imports_all.sort()
+  imports_import_errors['win'] = e
+imports_all.sort()
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/json.py` & `mainshortcuts-1.6.90/src/MainShortcuts/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,111 @@
 import MainShortcuts.file as m_file
 import MainShortcuts.path as m_path
-import json as _json
+try:
+  import json5 as _json
+except:
+  import json as _json
 import sys as _sys
-_print=print
-def _obj_encoder(obj,recurse=2,func=lambda k:not k.startswith("_"))->dict:
+_print = print
+
+
+def _obj_encoder(obj, recurse=2, func=lambda k: not k.startswith("_")) -> dict:
   """Преобразование объекта в словарь
   obj - сам объект
   recurse - глубина рекурсивной обработки
   func - фильтр атрибутов"""
-  if hasattr(obj,"to_dict"):
-    to_dict=getattr(obj,"to_dict")
+  if hasattr(obj, "to_dict"):
+    to_dict = getattr(obj, "to_dict")
     if callable(to_dict):
       return to_dict()
-  types=[
-    str,
-    dict,
-    tuple,
-    list,
-    int,
-    float,
-    type(True),
-    type(False),
-    type(None),
-    ]
-  d={}
+  types = [
+      str,
+      dict,
+      tuple,
+      list,
+      int,
+      float,
+      type(True),
+      type(False),
+      type(None),
+  ]
+  d = {}
   for k in dir(obj):
     if func(k):
-      v=getattr(obj,k)
-      if callable(v):continue
+      v = getattr(obj, k)
+      if callable(v):
+        continue
       if type(v) in types:
-        d[k]=v
-      elif recurse>0:
-        d[k]=_obj_encoder(v,recurse=recurse-1)
+        d[k] = v
+      elif recurse > 0:
+        d[k] = _obj_encoder(v, recurse=recurse - 1)
   return d
-def encode(data,mode:str="c",indent:int=2,sort:bool=True,force:bool=True,**kwargs)->str:
+
+
+def encode(data, mode: str = "c", indent: int = 2, sort: bool = True, force: bool = True, **kwargs) -> str:
   """Данные в текст JSON
   data - данные для кодирования
   mode - c/compress/min/zip: сжатый JSON
          p/pretty/max/print: развёрнутый JSON
   indent - кол-во отступов в развёрнутом JSON
   sort - сортировка словарей
   force - преобразовывать объекты в словари
   остальные аргументы как в json.dumps"""
   if force:
-    kwargs["default"]=_obj_encoder
-  kwargs["sort_keys"]=sort
-  if mode in ["c","compress","min","zip"]: # Сжатый
-    kwargs["separators"]=[",",":"]
-  elif mode in ["pretty","p","print","max"]: # Развёрнутый
-    kwargs["indent"]=int(indent)
-  return _json.dumps(data,**kwargs)
-def decode(text:str,**kwargs):
+    kwargs["default"] = _obj_encoder
+  kwargs["sort_keys"] = sort
+  if mode in ["c", "compress", "min", "zip"]:  # Сжатый
+    kwargs["separators"] = [",", ":"]
+  elif mode in ["pretty", "p", "print", "max"]:  # Развёрнутый
+    kwargs["indent"] = int(indent)
+  return _json.dumps(data, **kwargs)
+
+
+def decode(text: str, **kwargs):
   """Текст JSON в данные
   text - текст для декодирования
   остальные аргументы как в json.loads"""
-  return _json.loads(str(text),**kwargs)
-def write(path:str,data,encoding:str="utf-8",force:bool=False,**kwargs):
+  return _json.loads(str(text), **kwargs)
+
+
+def write(path: str, data, encoding: str = "utf-8", force: bool = False, **kwargs):
   """Записать данные в файл JSON
   path - путь к файлу
   data - данные
   encoding - кодировка
   force - если в месте назначения папка, удалить её
   остальные аргументы как в ms.json.encode"""
-  if m_path.info(path)["type"]=="dir" and force:
+  if m_path.info(path)["type"] == "dir" and force:
     m_path.rm(path)
-  return m_file.write(path,encode(data,**kwargs),encoding=encoding)
-def read(path:str,encoding:str="utf-8",**kwargs):
+  return m_file.write(path, encode(data, **kwargs), encoding=encoding)
+
+
+def read(path: str, encoding: str = "utf-8", **kwargs):
   """Прочитать данные из JSON файла
   path - путь к файлу
   encoding - кодировка
   остальные аргументы как в ms.json.decode"""
-  return decode(m_file.read(path,encoding=encoding),**kwargs)
-def print(data,file=_sys.stdout,mode:str="p",**kwargs):
+  return decode(m_file.read(path, encoding=encoding), **kwargs)
+
+
+def print(data, file=_sys.stdout, mode: str = "p", **kwargs):
   """Вывести данные в stdout в виде JSON
   mode - как в ms.json.encode
   file - как в print"""
-  kwargs["mode"]=mode
-  _print(encode(data,**kwargs),file=file)
-def rebuild(text:str,**kwargs):
+  kwargs["mode"] = mode
+  _print(encode(data, **kwargs), file=file)
+
+
+def rebuild(text: str, **kwargs):
   """Перестроить текст JSON
   text - сам текст
   остальные аргументы как в ms.json.encode"""
-  return encode(decode(text),**kwargs)
-def rewrite(path:str,encoding:str="utf-8",**kwargs):
+  return encode(decode(text), **kwargs)
+
+
+def rewrite(path: str, encoding: str = "utf-8", **kwargs):
   """Перестроить JSON в файле
   path - путь к файлу
   encoding - кодировка
   остальные аргументы как в ms.json.write"""
-  kwargs["encoding"]=encoding
-  return write(path,read(path,encoding=encoding),**kwargs)
+  kwargs["encoding"] = encoding
+  return write(path, read(path, encoding=encoding), **kwargs)
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/main.py` & `mainshortcuts-1.6.90/src/MainShortcuts/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import MainShortcuts.os as m_os
 import os as _os
 import sys as _sys
 # Универсальные команды
-exit=_sys.exit
-cd=_os.chdir
-pwd=_os.getcwd
+exit = _sys.exit
+cd = _os.chdir
+pwd = _os.getcwd
+
+
 def clear_ANSI():
   print("\u001b[2J")
-cls_ANSI=clear_ANSI
+
+
+cls_ANSI = clear_ANSI
 # Команды для разных ОС
-if m_os.platform=="Windows": # Windows
+if m_os.platform == "Windows":  # Windows
   def clear():
     '''Очистить весь текст в терминале (использует "cls")'''
     _os.system("cls")
-  cls=clear
-elif m_os.platform=="Linux": # Linux
+  cls = clear
+elif m_os.platform == "Linux":  # Linux
   def clear():
     '''Очистить весь текст в терминале (использует "clear")'''
     _os.system("clear")
-  cls=clear
-elif m_os.platform=="Darwin": # MacOS
+  cls = clear
+elif m_os.platform == "Darwin":  # MacOS
   def clear():
     """На этой ОС функция недоступна. На других очищает весь текст в терминале"""
     raise Exception("This feature is not available on the current operating system")
-  cls=clear
-else: # Неизвестный тип
-  print("MainShortcuts WARN: Unknown OS \""+m_os.platform+"\"",file=_sys.stderr)
+  cls = clear
+else:  # Неизвестный тип
+  print("MainShortcuts WARN: Unknown OS \"" + m_os.platform + "\"", file=_sys.stderr)
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/path.py` & `mainshortcuts-1.6.90/src/MainShortcuts/path.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,210 @@
 import MainShortcuts.addon as _a
 import os as _os
 import shutil as _shutil
-sep=_os.sep # Разделитель в пути файла
-extsep=_os.extsep # Разделитель в расширении файла
-pathsep=sep
-separator=sep
-pwd=_os.getcwd
-cd=_os.chdir
-exists=_os.path.exists
-def merge(array:list,sep:str=pathsep):
+sep = _os.sep  # Разделитель в пути файла
+extsep = _os.extsep  # Разделитель в расширении файла
+pathsep = sep
+separator = sep
+pwd = _os.getcwd
+cd = _os.chdir
+exists = _os.path.exists
+
+
+def merge(array: list, sep: str = pathsep):
   """Собрать путь к объекту из массива"""
   return sep.join(array)
-def split(path:str):
+
+
+def split(path: str):
   """Разложить путь к объекту на массив"""
-  return path.replace("\\","/").split("/")
-def info(path:str=_os.getcwd(),listdir:bool=False,listlinks:bool=False)->dict:
+  return path.replace("\\", "/").split("/")
+
+
+def info(path: str = _os.getcwd(), listdir: bool = False, listlinks: bool = False) -> dict:
   """Информация о файле/папке
   path - путь к объекту
   listdir - если папка, то рекурсивно создать список содержимого и суммарный размер
   listlinks - проверять ссылки при рекурсии?"""
-  path=path.replace("\\","/")
-  i={
-    "dir":None, # Папка, в которой находится объект
-    "dirs":None, # Рекурсивный список папок (если аргумент listdir=True)
-    "exists":None, # Существует ли объект? | True/False
-    "ext":None, # Расширение файла, даже если это папка
-    "files":None, # Рекурсивный список файлов (если аргумент listdir=True)
-    "fullname":None, # Полное название объекта (включая расширение)
-    "fullpath":None, # Полный путь к объекту
-    "link":None, # Это ссылка или оригинал? | True/False
-    "name":None, # Название файла без расширения, даже если это папка
-    "path":None, # Полученный путь к объекту
-    "realpath":None, # Путь к оригиналу, если указана ссылка
-    "relpath":None, # Относительный путь
-    "size":None, # Размер. Для получения размера папки укажите аргумент listdir=True
-    "split":[], # Путь, разделённый на массив
-    "type":None, # Тип объекта | "file"/"dir"
-    "errors":{}, # Параметры, при получении которых возникла ошибка
-    "created":None, # Timestamp создания файла
-    "modified":None, # Timestamp последнего изменения файла
-    "used":None, # Timestamp последнего использования файла
-    }
-  errors={}
-  i["path"]=path
-  i["split"]=path.split("/")
-  i["dir"],i["fullname"]=_os.path.split(path)
+  path = path.replace("\\", "/")
+  i = {
+      "dir": None,  # Папка, в которой находится объект
+      "dirs": None,  # Рекурсивный список папок (если аргумент listdir=True)
+      "exists": None,  # Существует ли объект? | True/False
+      "ext": None,  # Расширение файла, даже если это папка
+      "files": None,  # Рекурсивный список файлов (если аргумент listdir=True)
+      "fullname": None,  # Полное название объекта (включая расширение)
+      "fullpath": None,  # Полный путь к объекту
+      "link": None,  # Это ссылка или оригинал? | True/False
+      "name": None,  # Название файла без расширения, даже если это папка
+      "path": None,  # Полученный путь к объекту
+      "realpath": None,  # Путь к оригиналу, если указана ссылка
+      "relpath": None,  # Относительный путь
+      "size": None,  # Размер. Для получения размера папки укажите аргумент listdir=True
+      "split": [],  # Путь, разделённый на массив
+      "type": None,  # Тип объекта | "file"/"dir"
+      "errors": {},  # Параметры, при получении которых возникла ошибка
+      "created": None,  # Timestamp создания файла
+      "modified": None,  # Timestamp последнего изменения файла
+      "used": None,  # Timestamp последнего использования файла
+  }
+  errors = {}
+  i["path"] = path
+  i["split"] = path.split("/")
+  i["dir"], i["fullname"] = _os.path.split(path)
   try:
-    i["fullpath"]=_os.path.abspath(path)
+    i["fullpath"] = _os.path.abspath(path)
   except Exception as e:
-    errors["fullpath"]=e
+    errors["fullpath"] = e
   try:
-    i["relpath"]=_os.path.relpath(path)
+    i["relpath"] = _os.path.relpath(path)
   except Exception as e:
-    errors["relpath"]=e
+    errors["relpath"] = e
   if "." in i["fullname"]:
-    i["ext"]=i["fullname"].split(".")[-1]
-    i["name"]=".".join(i["fullname"].split(".")[:-1])
+    i["ext"] = i["fullname"].split(".")[-1]
+    i["name"] = ".".join(i["fullname"].split(".")[:-1])
   else:
-    i["ext"]=None
-    i["name"]=i["fullname"]
+    i["ext"] = None
+    i["name"] = i["fullname"]
   try:
-    i["exists"]=exists(path)
+    i["exists"] = exists(path)
   except Exception as e:
-    errors["exists"]=e
+    errors["exists"] = e
   if i["exists"]:
-    i["created"]=_os.path.getctime(path)
-    i["modified"]=_os.path.getmtime(path)
-    i["used"]=_os.path.getatime(path)
-    i["link"]=_os.path.islink(path)
+    i["created"] = _os.path.getctime(path)
+    i["modified"] = _os.path.getmtime(path)
+    i["used"] = _os.path.getatime(path)
+    i["link"] = _os.path.islink(path)
     if i["link"]:
       try:
-        i["realpath"]=_os.path.realpath(path)
+        i["realpath"] = _os.path.realpath(path)
       except Exception as e:
-        errors["realpath"]=e
+        errors["realpath"] = e
     if _os.path.isfile(path):
-      i["size"]=_os.path.getsize(path)
-      i["type"]="file"
+      i["size"] = _os.path.getsize(path)
+      i["type"] = "file"
     elif _os.path.isdir(path):
-      i["type"]="dir"
+      i["type"] = "dir"
       if listdir:
-        tmp=_a.listdir(path,listlinks)
-        i["dirs"]=tmp["d"]
-        i["files"]=tmp["f"]
-        i["size"]=tmp["s"]
+        tmp = _a.listdir(path, listlinks)
+        i["dirs"] = tmp["d"]
+        i["files"] = tmp["f"]
+        i["size"] = tmp["s"]
     else:
-      i["type"]="unknown"
-  i["errors"]=errors
+      i["type"] = "unknown"
+  i["errors"] = errors
   return i
+
+
 class recurse_info:
   """Рекурсивная информация о папке
   В разработке"""
-  def __init__(self,p:str=_os.getcwd(),links:bool=False):
-    self.path=p
-    for k,v in info(p,listdir=True,listlinks=links).items():
-      self[k]=v
-    if self.type=="dir":
-      f={}
-      d={}
+
+  def __init__(self, p: str = _os.getcwd(), links: bool = False):
+    self.path = p
+    for k, v in info(p, listdir=True, listlinks=links).items():
+      self[k] = v
+    if self.type == "dir":
+      f = {}
+      d = {}
       for i in self.files:
-        f[i]=info(i)
+        f[i] = info(i)
       for i in self.dirs:
-        d[i]=info(i)
-      self.files=f
-      self.dirs=d
+        d[i] = info(i)
+      self.files = f
+      self.dirs = d
+
   def __repr__(self):
     return f"ms.recurse_info('{self.path}')"
+
   def __bool__(self):
     return self.exists
-  def __getitem__(self,k):
-    return getattr(self,k)
-  def __setitem__(self,k,v):
-    setattr(self,k,v)
-  def __delitem__(self,k):
-    delattr(self,k)
-  def __eq__(self,other):
+
+  def __getitem__(self, k):
+    return getattr(self, k)
+
+  def __setitem__(self, k, v):
+    setattr(self, k, v)
+
+  def __delitem__(self, k):
+    delattr(self, k)
+
+  def __eq__(self, other):
     try:
-      myD={}
-      otD={}
+      myD = {}
+      otD = {}
       for k in dir(self):
         if not k.startswith("_"):
-          myD[k]=self[k]
+          myD[k] = self[k]
       for k in dir(other):
         if not k.startswith("_"):
-          otD[k]=other[k]
-      return myD==otD
+          otD[k] = other[k]
+      return myD == otD
     except:
       return False
-def delete(path:str):
+
+
+def delete(path: str):
   """Удалить папку или файл, если существует"""
   if _os.path.exists(path):
     if _os.path.islink(path):
       _os.unlink(path)
     elif _os.path.isfile(path):
       _os.remove(path)
     elif _os.path.isdir(path):
       _shutil.rmtree(path)
     else:
       raise Exception("Unknown type")
-rm=delete
+
+
+rm = delete
 # del=delete
-def copy(fr:str,to:str):
+
+
+def copy(fr: str, to: str):
   """Копировать"""
   if _os.path.isfile(fr):
-    _shutil.copy(fr,to)
+    _shutil.copy(fr, to)
   elif _os.path.isdir(fr):
-    _shutil.copytree(fr,to)
+    _shutil.copytree(fr, to)
   else:
     raise Exception("Unknown type")
-cp=copy
-def move(fr:str,to:str):
+
+
+cp = copy
+
+
+def move(fr: str, to: str):
   """Переместить"""
-  _shutil.move(fr,to)
-mv=move
-def rename(fr:str,to:str):
+  _shutil.move(fr, to)
+
+
+mv = move
+
+
+def rename(fr: str, to: str):
   """Переименовать"""
-  _os.rename(fr,to)
-rn=rename
-def link(fr:str,to:str,force:bool=False):
+  _os.rename(fr, to)
+
+
+rn = rename
+
+
+def link(fr: str, to: str, force: bool = False):
   """Сделать символическую ссылку"""
   if exists(to) and force:
     delete(to)
-  _os.symlink(fr,to)
-ln=link
-def format(path:str,replace_to:str=None,sep=pathsep)->str:
+  _os.symlink(fr, to)
+
+
+ln = link
+
+
+def format(path: str, replace_to: str = None, sep=pathsep) -> str:
   """Форматировать путь к файлу (изменить разделитель, удалить недопустимые символы)
   replace_to - заменить недопустимые символы на указанный"""
-  for i in ["/","\\"]:
-    path=path.replace(i,sep)
-  if replace_to!=None:
-    for i in ["\n",":","*","?","\"","<",">","|","+","%","!","@"]:
-      path=path.replace(i,replace_to)
+  for i in ["/", "\\"]:
+    path = path.replace(i, sep)
+  if replace_to != None:
+    for i in ["\n", ":", "*", "?", "\"", "<", ">", "|", "+", "%", "!", "@"]:
+      path = path.replace(i, replace_to)
   return path
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/script.py` & `mainshortcuts-1.6.90/src/MainShortcuts/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 from MainShortcuts.MainCore import ms, _MainCore
-mcore=_MainCore(__file__=__file__,__name__=__name__)
-cprint=mcore.cprint
-cformat=mcore.cformat
-argv=mcore.args[1:]
+mcore = _MainCore(__file__=__file__, __name__=__name__)
+cprint = mcore.cprint
+cformat = mcore.cformat
+argv = mcore.args[1:]
+
+
 def mkdir(path=argv):
-  if type(path)==str:
-    p=[path]
-  elif type(path)==tuple:
-    p=list(path)
+  if type(path) == str:
+    p = [path]
+  elif type(path) == tuple:
+    p = list(path)
   else:
-    p=path
+    p = path
   for i in p:
     try:
       ms.dir.create(i)
     except Exception as e:
-      cprint(e,start="RED")
+      cprint(e, start="RED")
+
+
 def jsonPretty(path=argv):
-  if type(path)==str:
-    p=[path]
-  elif type(path)==tuple:
-    p=list(path)
+  if type(path) == str:
+    p = [path]
+  elif type(path) == tuple:
+    p = list(path)
   else:
-    p=path
+    p = path
   for i in p:
     try:
-      d=ms.json.read(i)
-      ms.json.write(i,d,mode="p")
+      d = ms.json.read(i)
+      ms.json.write(i, d, mode="p")
     except Exception as e:
-      cprint(e,start="RED")
+      cprint(e, start="RED")
+
+
 def jsonCompress(path=argv):
-  if type(path)==str:
-    p=[path]
-  elif type(path)==tuple:
-    p=list(path)
+  if type(path) == str:
+    p = [path]
+  elif type(path) == tuple:
+    p = list(path)
   else:
-    p=path
+    p = path
   for i in p:
     try:
-      d=ms.json.read(i)
-      ms.json.write(i,d,mode="c")
+      d = ms.json.read(i)
+      ms.json.write(i, d, mode="c")
     except Exception as e:
-      cprint(e,start="RED")
+      cprint(e, start="RED")
+
+
 def getCore(path=argv):
-  if type(path)==str:
-    p=[path]
-  elif type(path)==tuple:
-    p=list(path)
+  if type(path) == str:
+    p = [path]
+  elif type(path) == tuple:
+    p = list(path)
   else:
-    p=path
+    p = path
   for i in p:
     try:
       if ms.path.exists(i):
-        a=ms.file.read(i)
-        c=mcore.embed.text+a
-        ms.file.write(i,c.rstrip())
-        cprint(f'MainCore added to the beginning of the file "{i}"',start="GREEN")
+        a = ms.file.read(i)
+        c = mcore.embed.text + a
+        ms.file.write(i, c.rstrip())
+        cprint(f'MainCore added to the beginning of the file "{i}"', start="GREEN")
       else:
-        ms.file.write(i,mcore.embed.text)
-        cprint(f'MainCore is written to file "{i}"',start="GREEN")
+        ms.file.write(i, mcore.embed.text)
+        cprint(f'MainCore is written to file "{i}"', start="GREEN")
     except Exception as e:
-      cprint(e,start="RED")
+      cprint(e, start="RED")
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/str.py` & `mainshortcuts-1.6.90/src/MainShortcuts/str.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from typing import Union
-def array2str(a:Union[list,tuple])->list:
+
+
+def array2str(a: Union[list, tuple]) -> list:
   """Преобразовать каждый элемент в строку"""
-  b=[]
+  b = []
   for i in a:
     b.append(str(i))
   return b
-list2str=array2str
-def dict2str(a:dict)->dict:
+
+
+list2str = array2str
+
+
+def dict2str(a: dict) -> dict:
   """Преобразовать каждое значение в строку"""
-  b={}
-  for key,value in a.items():
-    b[key]=str(value)
+  b = {}
+  for key, value in a.items():
+    b[key] = str(value)
   return b
+
+
 class replace:
-  def multi(text:str,d:dict)->str:
+  def multi(text: str, d: dict) -> str:
     """Мульти-замена {"что заменить":"чем заменить"}"""
-    t=str(text)
-    for k,v in d.items():
-      t=t.replace(k,str(v))
+    t = str(text)
+    for k, v in d.items():
+      t = t.replace(k, str(v))
     return t
-  def all(text:str,fr:str,to:str)->str:
+
+  def all(text: str, fr: str, to: str) -> str:
     """Замена пока заменяемый текст не исчезнет"""
-    t=str(text)
-    a=str(fr)
-    b=str(to)
+    t = str(text)
+    a = str(fr)
+    b = str(to)
     if a in b:
-      raise Exception('"{0}" is contained in "{1}", this causes an infinite loop'.format(a,b))
+      raise Exception('"{0}" is contained in "{1}", this causes an infinite loop'.format(a, b))
     while a in t:
-      t=t.replace(a,b)
-    return t
+      t = t.replace(a, b)
+    return t
```

### Comparing `mainshortcuts-1.6.89/src/MainShortcuts/values.py` & `mainshortcuts-1.6.90/src/MainShortcuts/values.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,490 +1,616 @@
 """Модифицированные версии встроенных значений"""
-import builtins,json
+import builtins
+import json
+
+
 class int:
-  def __init__(self,data:int=0):
-    self.data=builtins.int(data)
+  def __init__(self, data: int = 0):
+    self.data = builtins.int(data)
+
   def __repr__(self):
     return f"ms.values.int({json.dumps(self.data)})"
+
   def __str__(self):
     return builtins.str(self.data)
+
   def __neg__(self):
     return self.data.__neg__(self)
+
   def __pos__(self):
     return self.data.__pos__(self)
+
   def __abs__(self):
     return self.data.__abs__(self)
+
   def __invert__(self):
     return self.data.__invert__(self)
+
   def __int__(self):
     return self.data.__int__(self)
+
   def __float__(self):
     return self.data.__float__(self)
+
   def __index__(self):
     return self.data.__index__(self)
+
   def __trunc__(self):
     return self.data.__trunc__(self)
+
   def __floor__(self):
     return self.data.__floor__(self)
+
   def __ceil__(self):
     return self.data.__ceil__(self)
-  def __add__(self,other):
-    if type(self)==type(other):
+
+  def __add__(self, other):
+    if type(self) == type(other):
       return self.data.__add__(other.data)
     else:
       return self.data.__add__(other)
-  def __and__(self,other):
-    if type(self)==type(other):
+
+  def __and__(self, other):
+    if type(self) == type(other):
       return self.data.__and__(other.data)
     else:
       return self.data.__and__(other)
-  def __divmod__(self,other):
-    if type(self)==type(other):
+
+  def __divmod__(self, other):
+    if type(self) == type(other):
       return self.data.__divmod__(other.data)
     else:
       return self.data.__divmod__(other)
-  def __eq__(self,other):
-    if type(self)==type(other):
+
+  def __eq__(self, other):
+    if type(self) == type(other):
       return self.data.__eq__(other.data)
     else:
       return self.data.__eq__(other)
-  def __floordiv__(self,other):
-    if type(self)==type(other):
+
+  def __floordiv__(self, other):
+    if type(self) == type(other):
       return self.data.__floordiv__(other.data)
     else:
       return self.data.__floordiv__(other)
-  def __ge__(self,other):
-    if type(self)==type(other):
+
+  def __ge__(self, other):
+    if type(self) == type(other):
       return self.data.__ge__(other.data)
     else:
       return self.data.__ge__(other)
-  def __gt__(self,other):
-    if type(self)==type(other):
+
+  def __gt__(self, other):
+    if type(self) == type(other):
       return self.data.__gt__(other.data)
     else:
       return self.data.__gt__(other)
-  def __le__(self,other):
-    if type(self)==type(other):
+
+  def __le__(self, other):
+    if type(self) == type(other):
       return self.data.__le__(other.data)
     else:
       return self.data.__le__(other)
-  def __lshift__(self,other):
-    if type(self)==type(other):
+
+  def __lshift__(self, other):
+    if type(self) == type(other):
       return self.data.__lshift__(other.data)
     else:
       return self.data.__lshift__(other)
-  def __lt__(self,other):
-    if type(self)==type(other):
+
+  def __lt__(self, other):
+    if type(self) == type(other):
       return self.data.__lt__(other.data)
     else:
       return self.data.__lt__(other)
-  def __mod__(self,other):
-    if type(self)==type(other):
+
+  def __mod__(self, other):
+    if type(self) == type(other):
       return self.data.__mod__(other.data)
     else:
       return self.data.__mod__(other)
-  def __mul__(self,other):
-    if type(self)==type(other):
+
+  def __mul__(self, other):
+    if type(self) == type(other):
       return self.data.__mul__(other.data)
     else:
       return self.data.__mul__(other)
-  def __ne__(self,other):
-    if type(self)==type(other):
+
+  def __ne__(self, other):
+    if type(self) == type(other):
       return self.data.__ne__(other.data)
     else:
       return self.data.__ne__(other)
-  def __or__(self,other):
-    if type(self)==type(other):
+
+  def __or__(self, other):
+    if type(self) == type(other):
       return self.data.__or__(other.data)
     else:
       return self.data.__or__(other)
-  def __radd__(self,other):
-    if type(self)==type(other):
+
+  def __radd__(self, other):
+    if type(self) == type(other):
       return self.data.__radd__(other.data)
     else:
       return self.data.__radd__(other)
-  def __rand__(self,other):
-    if type(self)==type(other):
+
+  def __rand__(self, other):
+    if type(self) == type(other):
       return self.data.__rand__(other.data)
     else:
       return self.data.__rand__(other)
-  def __rdivmod__(self,other):
-    if type(self)==type(other):
+
+  def __rdivmod__(self, other):
+    if type(self) == type(other):
       return self.data.__rdivmod__(other.data)
     else:
       return self.data.__rdivmod__(other)
-  def __rfloordiv__(self,other):
-    if type(self)==type(other):
+
+  def __rfloordiv__(self, other):
+    if type(self) == type(other):
       return self.data.__rfloordiv__(other.data)
     else:
       return self.data.__rfloordiv__(other)
-  def __rlshift__(self,other):
-    if type(self)==type(other):
+
+  def __rlshift__(self, other):
+    if type(self) == type(other):
       return self.data.__rlshift__(other.data)
     else:
       return self.data.__rlshift__(other)
-  def __rmod__(self,other):
-    if type(self)==type(other):
+
+  def __rmod__(self, other):
+    if type(self) == type(other):
       return self.data.__rmod__(other.data)
     else:
       return self.data.__rmod__(other)
-  def __rmul__(self,other):
-    if type(self)==type(other):
+
+  def __rmul__(self, other):
+    if type(self) == type(other):
       return self.data.__rmul__(other.data)
     else:
       return self.data.__rmul__(other)
-  def __ror__(self,other):
-    if type(self)==type(other):
+
+  def __ror__(self, other):
+    if type(self) == type(other):
       return self.data.__ror__(other.data)
     else:
       return self.data.__ror__(other)
-  def __rrshift__(self,other):
-    if type(self)==type(other):
+
+  def __rrshift__(self, other):
+    if type(self) == type(other):
       return self.data.__rrshift__(other.data)
     else:
       return self.data.__rrshift__(other)
-  def __rshift__(self,other):
-    if type(self)==type(other):
+
+  def __rshift__(self, other):
+    if type(self) == type(other):
       return self.data.__rshift__(other.data)
     else:
       return self.data.__rshift__(other)
-  def __rsub__(self,other):
-    if type(self)==type(other):
+
+  def __rsub__(self, other):
+    if type(self) == type(other):
       return self.data.__rsub__(other.data)
     else:
       return self.data.__rsub__(other)
-  def __rtruediv__(self,other):
-    if type(self)==type(other):
+
+  def __rtruediv__(self, other):
+    if type(self) == type(other):
       return self.data.__rtruediv__(other.data)
     else:
       return self.data.__rtruediv__(other)
-  def __rxor__(self,other):
-    if type(self)==type(other):
+
+  def __rxor__(self, other):
+    if type(self) == type(other):
       return self.data.__rxor__(other.data)
     else:
       return self.data.__rxor__(other)
-  def __sub__(self,other):
-    if type(self)==type(other):
+
+  def __sub__(self, other):
+    if type(self) == type(other):
       return self.data.__sub__(other.data)
     else:
       return self.data.__sub__(other)
-  def __truediv__(self,other):
-    if type(self)==type(other):
+
+  def __truediv__(self, other):
+    if type(self) == type(other):
       return self.data.__truediv__(other.data)
     else:
       return self.data.__truediv__(other)
-  def __xor__(self,other):
-    if type(self)==type(other):
+
+  def __xor__(self, other):
+    if type(self) == type(other):
       return self.data.__xor__(other.data)
     else:
       return self.data.__xor__(other)
+
+
 class float:
-  def __init__(self,data:float=0.0):
-    self.data=builtins.float(data)
+  def __init__(self, data: float = 0.0):
+    self.data = builtins.float(data)
+
   def __repr__(self):
     return f"ms.values.float({json.dumps(self.data)})"
+
   def __str__(self):
     return builtins.str(self.data)
+
   def __neg__(self):
     return self.data.__neg__(self)
+
   def __pos__(self):
     return self.data.__pos__(self)
+
   def __abs__(self):
     return self.data.__abs__(self)
+
   def __int__(self):
     return self.data.__int__(self)
+
   def __float__(self):
     return self.data.__float__(self)
+
   def __trunc__(self):
     return self.data.__trunc__(self)
+
   def __floor__(self):
     return self.data.__floor__(self)
+
   def __ceil__(self):
     return self.data.__ceil__(self)
-  def __add__(self,other):
-    if type(self)==type(other):
+
+  def __add__(self, other):
+    if type(self) == type(other):
       return self.data.__add__(other.data)
     else:
       return self.data.__add__(other)
-  def __divmod__(self,other):
-    if type(self)==type(other):
+
+  def __divmod__(self, other):
+    if type(self) == type(other):
       return self.data.__divmod__(other.data)
     else:
       return self.data.__divmod__(other)
-  def __eq__(self,other):
-    if type(self)==type(other):
+
+  def __eq__(self, other):
+    if type(self) == type(other):
       return self.data.__eq__(other.data)
     else:
       return self.data.__eq__(other)
-  def __floordiv__(self,other):
-    if type(self)==type(other):
+
+  def __floordiv__(self, other):
+    if type(self) == type(other):
       return self.data.__floordiv__(other.data)
     else:
       return self.data.__floordiv__(other)
-  def __ge__(self,other):
-    if type(self)==type(other):
+
+  def __ge__(self, other):
+    if type(self) == type(other):
       return self.data.__ge__(other.data)
     else:
       return self.data.__ge__(other)
-  def __gt__(self,other):
-    if type(self)==type(other):
+
+  def __gt__(self, other):
+    if type(self) == type(other):
       return self.data.__gt__(other.data)
     else:
       return self.data.__gt__(other)
-  def __le__(self,other):
-    if type(self)==type(other):
+
+  def __le__(self, other):
+    if type(self) == type(other):
       return self.data.__le__(other.data)
     else:
       return self.data.__le__(other)
-  def __lt__(self,other):
-    if type(self)==type(other):
+
+  def __lt__(self, other):
+    if type(self) == type(other):
       return self.data.__lt__(other.data)
     else:
       return self.data.__lt__(other)
-  def __mod__(self,other):
-    if type(self)==type(other):
+
+  def __mod__(self, other):
+    if type(self) == type(other):
       return self.data.__mod__(other.data)
     else:
       return self.data.__mod__(other)
-  def __mul__(self,other):
-    if type(self)==type(other):
+
+  def __mul__(self, other):
+    if type(self) == type(other):
       return self.data.__mul__(other.data)
     else:
       return self.data.__mul__(other)
-  def __ne__(self,other):
-    if type(self)==type(other):
+
+  def __ne__(self, other):
+    if type(self) == type(other):
       return self.data.__ne__(other.data)
     else:
       return self.data.__ne__(other)
-  def __radd__(self,other):
-    if type(self)==type(other):
+
+  def __radd__(self, other):
+    if type(self) == type(other):
       return self.data.__radd__(other.data)
     else:
       return self.data.__radd__(other)
-  def __rdivmod__(self,other):
-    if type(self)==type(other):
+
+  def __rdivmod__(self, other):
+    if type(self) == type(other):
       return self.data.__rdivmod__(other.data)
     else:
       return self.data.__rdivmod__(other)
-  def __rfloordiv__(self,other):
-    if type(self)==type(other):
+
+  def __rfloordiv__(self, other):
+    if type(self) == type(other):
       return self.data.__rfloordiv__(other.data)
     else:
       return self.data.__rfloordiv__(other)
-  def __rmod__(self,other):
-    if type(self)==type(other):
+
+  def __rmod__(self, other):
+    if type(self) == type(other):
       return self.data.__rmod__(other.data)
     else:
       return self.data.__rmod__(other)
-  def __rmul__(self,other):
-    if type(self)==type(other):
+
+  def __rmul__(self, other):
+    if type(self) == type(other):
       return self.data.__rmul__(other.data)
     else:
       return self.data.__rmul__(other)
-  def __rsub__(self,other):
-    if type(self)==type(other):
+
+  def __rsub__(self, other):
+    if type(self) == type(other):
       return self.data.__rsub__(other.data)
     else:
       return self.data.__rsub__(other)
-  def __rtruediv__(self,other):
-    if type(self)==type(other):
+
+  def __rtruediv__(self, other):
+    if type(self) == type(other):
       return self.data.__rtruediv__(other.data)
     else:
       return self.data.__rtruediv__(other)
-  def __sub__(self,other):
-    if type(self)==type(other):
+
+  def __sub__(self, other):
+    if type(self) == type(other):
       return self.data.__sub__(other.data)
     else:
       return self.data.__sub__(other)
-  def __truediv__(self,other):
-    if type(self)==type(other):
+
+  def __truediv__(self, other):
+    if type(self) == type(other):
       return self.data.__truediv__(other.data)
     else:
       return self.data.__truediv__(other)
+
+
 class str:
-  def __init__(self,data:str=""):
-    self.data=builtins.str(data)
+  def __init__(self, data: str = ""):
+    self.data = builtins.str(data)
+
   def __repr__(self):
     return f"ms.values.str({json.dumps(self.data)})"
+
   def __str__(self):
     return builtins.str(self.data)
-  def __getitem__(self,k):
+
+  def __getitem__(self, k):
     return self.data[k]
-  def __setitem__(self,k,v):
-    self.data[k]=v
-  def __add__(self,other):
-    if type(self)==type(other):
+
+  def __setitem__(self, k, v):
+    self.data[k] = v
+
+  def __add__(self, other):
+    if type(self) == type(other):
       return self.data.__add__(other.data)
     else:
       return self.data.__add__(other)
-  def __eq__(self,other):
-    if type(self)==type(other):
+
+  def __eq__(self, other):
+    if type(self) == type(other):
       return self.data.__eq__(other.data)
     else:
       return self.data.__eq__(other)
-  def __ge__(self,other):
-    if type(self)==type(other):
+
+  def __ge__(self, other):
+    if type(self) == type(other):
       return self.data.__ge__(other.data)
     else:
       return self.data.__ge__(other)
-  def __gt__(self,other):
-    if type(self)==type(other):
+
+  def __gt__(self, other):
+    if type(self) == type(other):
       return self.data.__gt__(other.data)
     else:
       return self.data.__gt__(other)
-  def __le__(self,other):
-    if type(self)==type(other):
+
+  def __le__(self, other):
+    if type(self) == type(other):
       return self.data.__le__(other.data)
     else:
       return self.data.__le__(other)
-  def __lt__(self,other):
-    if type(self)==type(other):
+
+  def __lt__(self, other):
+    if type(self) == type(other):
       return self.data.__lt__(other.data)
     else:
       return self.data.__lt__(other)
-  def __mod__(self,other):
-    if type(self)==type(other):
+
+  def __mod__(self, other):
+    if type(self) == type(other):
       return self.data.__mod__(other.data)
     else:
       return self.data.__mod__(other)
-  def __mul__(self,other):
-    if type(self)==type(other):
+
+  def __mul__(self, other):
+    if type(self) == type(other):
       return self.data.__mul__(other.data)
     else:
       return self.data.__mul__(other)
-  def __ne__(self,other):
-    if type(self)==type(other):
+
+  def __ne__(self, other):
+    if type(self) == type(other):
       return self.data.__ne__(other.data)
     else:
       return self.data.__ne__(other)
-  def __rmod__(self,other):
-    if type(self)==type(other):
+
+  def __rmod__(self, other):
+    if type(self) == type(other):
       return self.data.__rmod__(other.data)
     else:
       return self.data.__rmod__(other)
-  def __rmul__(self,other):
-    if type(self)==type(other):
+
+  def __rmul__(self, other):
+    if type(self) == type(other):
       return self.data.__rmul__(other.data)
     else:
       return self.data.__rmul__(other)
+
+
 class list:
-  def __init__(self,data:list=[]):
-    self.data=builtins.list(data)
+  def __init__(self, data: list = []):
+    self.data = builtins.list(data)
+
   def __repr__(self):
     return f"ms.values.list({json.dumps(self.data)})"
+
   def __str__(self):
     return builtins.str(self.data)
-  def __getitem__(self,k):
+
+  def __getitem__(self, k):
     return self.data[k]
-  def __setitem__(self,k,v):
-    self.data[k]=v
-  def __add__(self,other):
-    if type(self)==type(other):
+
+  def __setitem__(self, k, v):
+    self.data[k] = v
+
+  def __add__(self, other):
+    if type(self) == type(other):
       return self.data.__add__(other.data)
     else:
       return self.data.__add__(other)
-  def __eq__(self,other):
-    if type(self)==type(other):
+
+  def __eq__(self, other):
+    if type(self) == type(other):
       return self.data.__eq__(other.data)
     else:
       return self.data.__eq__(other)
-  def __ge__(self,other):
-    if type(self)==type(other):
+
+  def __ge__(self, other):
+    if type(self) == type(other):
       return self.data.__ge__(other.data)
     else:
       return self.data.__ge__(other)
-  def __gt__(self,other):
-    if type(self)==type(other):
+
+  def __gt__(self, other):
+    if type(self) == type(other):
       return self.data.__gt__(other.data)
     else:
       return self.data.__gt__(other)
-  def __iadd__(self,other):
-    if type(self)==type(other):
+
+  def __iadd__(self, other):
+    if type(self) == type(other):
       return self.data.__iadd__(other.data)
     else:
       return self.data.__iadd__(other)
-  def __imul__(self,other):
-    if type(self)==type(other):
+
+  def __imul__(self, other):
+    if type(self) == type(other):
       return self.data.__imul__(other.data)
     else:
       return self.data.__imul__(other)
-  def __le__(self,other):
-    if type(self)==type(other):
+
+  def __le__(self, other):
+    if type(self) == type(other):
       return self.data.__le__(other.data)
     else:
       return self.data.__le__(other)
-  def __lt__(self,other):
-    if type(self)==type(other):
+
+  def __lt__(self, other):
+    if type(self) == type(other):
       return self.data.__lt__(other.data)
     else:
       return self.data.__lt__(other)
-  def __mul__(self,other):
-    if type(self)==type(other):
+
+  def __mul__(self, other):
+    if type(self) == type(other):
       return self.data.__mul__(other.data)
     else:
       return self.data.__mul__(other)
-  def __ne__(self,other):
-    if type(self)==type(other):
+
+  def __ne__(self, other):
+    if type(self) == type(other):
       return self.data.__ne__(other.data)
     else:
       return self.data.__ne__(other)
-  def __rmul__(self,other):
-    if type(self)==type(other):
+
+  def __rmul__(self, other):
+    if type(self) == type(other):
       return self.data.__rmul__(other.data)
     else:
       return self.data.__rmul__(other)
+
+
 class dict:
-  def __init__(self,data:dict={}):
-    self.data=builtins.dict(data)
+  def __init__(self, data: dict = {}):
+    self.data = builtins.dict(data)
+
   def __repr__(self):
     return f"ms.values.dict({json.dumps(self.data)})"
+
   def __str__(self):
     return builtins.str(self.data)
-  def __getitem__(self,k):
+
+  def __getitem__(self, k):
     return self.data[k]
-  def __setitem__(self,k,v):
-    self.data[k]=v
-  def __eq__(self,other):
-    if type(self)==type(other):
+
+  def __setitem__(self, k, v):
+    self.data[k] = v
+
+  def __eq__(self, other):
+    if type(self) == type(other):
       return self.data.__eq__(other.data)
     else:
       return self.data.__eq__(other)
-  def __ge__(self,other):
-    if type(self)==type(other):
+
+  def __ge__(self, other):
+    if type(self) == type(other):
       return self.data.__ge__(other.data)
     else:
       return self.data.__ge__(other)
-  def __gt__(self,other):
-    if type(self)==type(other):
+
+  def __gt__(self, other):
+    if type(self) == type(other):
       return self.data.__gt__(other.data)
     else:
       return self.data.__gt__(other)
-  def __ior__(self,other):
-    if type(self)==type(other):
+
+  def __ior__(self, other):
+    if type(self) == type(other):
       return self.data.__ior__(other.data)
     else:
       return self.data.__ior__(other)
-  def __le__(self,other):
-    if type(self)==type(other):
+
+  def __le__(self, other):
+    if type(self) == type(other):
       return self.data.__le__(other.data)
     else:
       return self.data.__le__(other)
-  def __lt__(self,other):
-    if type(self)==type(other):
+
+  def __lt__(self, other):
+    if type(self) == type(other):
       return self.data.__lt__(other.data)
     else:
       return self.data.__lt__(other)
-  def __ne__(self,other):
-    if type(self)==type(other):
+
+  def __ne__(self, other):
+    if type(self) == type(other):
       return self.data.__ne__(other.data)
     else:
       return self.data.__ne__(other)
-  def __or__(self,other):
-    if type(self)==type(other):
+
+  def __or__(self, other):
+    if type(self) == type(other):
       return self.data.__or__(other.data)
     else:
       return self.data.__or__(other)
-  def __ror__(self,other):
-    if type(self)==type(other):
+
+  def __ror__(self, other):
+    if type(self) == type(other):
       return self.data.__ror__(other.data)
     else:
       return self.data.__ror__(other)
```

### Comparing `mainshortcuts-1.6.89/PKG-INFO` & `mainshortcuts-1.6.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainShortcuts
-Version: 1.6.89
+Version: 1.6.90
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

