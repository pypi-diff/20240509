# Comparing `tmp/TUIFIManager-4.0.5.tar.gz` & `tmp/TUIFIManager-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TUIFIManager-4.0.5.tar", last modified: Tue Apr 23 17:46:12 2024, max compression
+gzip compressed data, was "TUIFIManager-4.0.6.tar", last modified: Thu May  9 03:51:13 2024, max compression
```

## Comparing `TUIFIManager-4.0.5.tar` & `TUIFIManager-4.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/
--rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.gitattributes
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.919638 TUIFIManager-4.0.5/.github/
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.936304 TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/.github/workflows/
--rw-r--r--   0 xou       (1000) xou       (1000)      652 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.github/workflows/nox_ci.yml
--rw-r--r--   0 xou       (1000) xou       (1000)      605 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.gitignore
--rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.scrutinizer.yml
--rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.sourcery.yaml
--rw-r--r--   0 xou       (1000) xou       (1000)     7868 2024-04-22 12:52:13.000000 TUIFIManager-4.0.5/CHANGELOG.md
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)    10668 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)  1632442 2024-04-19 15:58:04.000000 TUIFIManager-4.0.5/Peek.gif
--rw-r--r--   0 xou       (1000) xou       (1000)     9570 2024-04-23 13:43:58.000000 TUIFIManager-4.0.5/README.md
--rw-r--r--   0 xou       (1000) xou       (1000)   246555 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/TUIFI.png
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/TUIFIManager/
--rw-r--r--   0 xou       (1000) xou       (1000)    31045 2024-04-23 17:34:12.000000 TUIFIManager-4.0.5/TUIFIManager/TUIFIProfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     5509 2024-04-11 13:08:50.000000 TUIFIManager-4.0.5/TUIFIManager/TUIFile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     5044 2024-04-19 15:56:05.000000 TUIFIManager-4.0.5/TUIFIManager/TUIMenu.py
--rw-r--r--   0 xou       (1000) xou       (1000)     8368 2024-04-23 15:42:02.000000 TUIFIManager-4.0.5/TUIFIManager/TUISynthXDND.py
--rw-r--r--   0 xou       (1000) xou       (1000)    11793 2024-04-20 08:55:32.000000 TUIFIManager-4.0.5/TUIFIManager/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)    74525 2024-04-23 17:42:38.000000 TUIFIManager-4.0.5/TUIFIManager/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     3109 2024-04-23 17:45:25.000000 TUIFIManager-4.0.5/TUIFIManager/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/TUIFIManager.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)    10668 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      700 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       53 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1497 2024-04-05 13:07:00.000000 TUIFIManager-4.0.5/flake.lock
--rw-r--r--   0 xou       (1000) xou       (1000)     1792 2024-04-23 13:02:57.000000 TUIFIManager-4.0.5/flake.nix
--rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/noxfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     1093 2024-04-23 17:43:22.000000 TUIFIManager-4.0.5/pyproject.toml
--rw-r--r--   0 xou       (1000) xou       (1000)       40 2024-04-05 13:07:00.000000 TUIFIManager-4.0.5/requirements.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1272 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-05-09 03:51:13.980270 TUIFIManager-4.0.6/
+-rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/.gitattributes
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-05-09 03:51:13.960271 TUIFIManager-4.0.6/.github/
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-05-09 03:51:13.976937 TUIFIManager-4.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-05-09 03:51:13.976937 TUIFIManager-4.0.6/.github/workflows/
+-rw-r--r--   0 xou       (1000) xou       (1000)      662 2024-04-25 22:13:30.000000 TUIFIManager-4.0.6/.github/workflows/nox_ci.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      605 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/.gitignore
+-rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/.scrutinizer.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/.sourcery.yaml
+-rw-r--r--   0 xou       (1000) xou       (1000)     7868 2024-04-22 12:52:13.000000 TUIFIManager-4.0.6/CHANGELOG.md
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)    10673 2024-05-09 03:51:13.980270 TUIFIManager-4.0.6/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)  1632442 2024-04-19 15:58:04.000000 TUIFIManager-4.0.6/Peek.gif
+-rw-r--r--   0 xou       (1000) xou       (1000)     9573 2024-05-09 02:10:25.000000 TUIFIManager-4.0.6/README.md
+-rw-r--r--   0 xou       (1000) xou       (1000)   246555 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/TUIFI.png
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-05-09 03:51:13.980270 TUIFIManager-4.0.6/TUIFIManager/
+-rw-r--r--   0 xou       (1000) xou       (1000)    31049 2024-05-09 02:08:14.000000 TUIFIManager-4.0.6/TUIFIManager/TUIFIProfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     5509 2024-04-11 13:08:50.000000 TUIFIManager-4.0.6/TUIFIManager/TUIFile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     5044 2024-04-19 15:56:05.000000 TUIFIManager-4.0.6/TUIFIManager/TUIMenu.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     8368 2024-04-23 15:42:02.000000 TUIFIManager-4.0.6/TUIFIManager/TUISynthXDND.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    11793 2024-04-20 08:55:32.000000 TUIFIManager-4.0.6/TUIFIManager/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    75093 2024-05-09 03:47:02.000000 TUIFIManager-4.0.6/TUIFIManager/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     3109 2024-05-09 03:19:43.000000 TUIFIManager-4.0.6/TUIFIManager/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-05-09 03:51:13.980270 TUIFIManager-4.0.6/TUIFIManager.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)    10673 2024-05-09 03:51:13.000000 TUIFIManager-4.0.6/TUIFIManager.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      700 2024-05-09 03:51:13.000000 TUIFIManager-4.0.6/TUIFIManager.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2024-05-09 03:51:13.000000 TUIFIManager-4.0.6/TUIFIManager.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       53 2024-05-09 03:51:13.000000 TUIFIManager-4.0.6/TUIFIManager.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2024-05-09 03:51:13.000000 TUIFIManager-4.0.6/TUIFIManager.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2024-05-09 03:51:13.000000 TUIFIManager-4.0.6/TUIFIManager.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1497 2024-04-05 13:07:00.000000 TUIFIManager-4.0.6/flake.lock
+-rw-r--r--   0 xou       (1000) xou       (1000)     2700 2024-04-25 21:48:29.000000 TUIFIManager-4.0.6/flake.nix
+-rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/noxfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1093 2024-05-09 03:47:36.000000 TUIFIManager-4.0.6/pyproject.toml
+-rw-r--r--   0 xou       (1000) xou       (1000)       40 2024-04-05 13:07:00.000000 TUIFIManager-4.0.6/requirements.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1272 2024-05-09 03:51:13.980270 TUIFIManager-4.0.6/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-10-01 12:46:14.000000 TUIFIManager-4.0.6/setup.py
```

### Comparing `TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `TUIFIManager-4.0.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/.github/workflows/nox_ci.yml` & `TUIFIManager-4.0.6/.github/workflows/nox_ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,19 @@
   push:
     branches: [ master ]
   workflow_dispatch:
   pull_request:
 
 jobs:
   ci:
-    runs-on: ${{ matrix.os }}-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python: [ '3.8', '3.9', '3.10' ]
-        os: [ ubuntu, windows, macos ]
+        os: [ ubuntu-latest, windows-latest, macos-13 ]
       fail-fast: false
 
     name: Nox - py ${{ matrix.python-version }} - ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v2
       - name: Python Setup
         uses: actions/setup-python@v2
```

### Comparing `TUIFIManager-4.0.5/.gitignore` & `TUIFIManager-4.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/CHANGELOG.md` & `TUIFIManager-4.0.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/LICENSE` & `TUIFIManager-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/PKG-INFO` & `TUIFIManager-4.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 4.0.5
+Version: 4.0.6
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
-Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: windows
 Classifier: Intended Audience :: Developers
@@ -22,14 +21,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: uni-curses>=2.1.3
+Requires-Dist: Send2Trash>=1.8.0
 
 
 
 <div align="center">
 <h1>TUIFI Manager</h1>
 <p>
     <a href="https://github.com/GiorgosXou/TUIFIManager/pulse">
@@ -138,15 +139,15 @@
 **(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
 | Cmd | Type | Attributes | Label Information|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
-|`yat` | copy | 'pattern':'.+\.txt'                     ||
+|`yat` | copy | 'pattern':'.+\\\\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
 **Available Type-keywords:** `open`, `copy`, `cut`, [`find`](## 'Attributes: `filename`')
 
 **important note:** `o` is also used for ordering in `vim_mode`. In this case you can first press space-bar before proceeding with `owv` or with any other already reserved starting key, or just change it. 
 
 **Additionally** there are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.5 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.6 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
-gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
-https://github.com/GiorgosXou/TUIFIManager Keywords: file-
+gxousos@gmail.com License: General Public License v3.0 Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: End Users/Desktop Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+uni-curses>=2.1.3 Requires-Dist: Send2Trash>=1.8.0
                           ************ TTUUIIFFII MMaannaaggeerr ************
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_G_i_o_r_g_o_s_X_o_u_/
  _T_U_I_F_I_M_a_n_a_g_e_r_?_c_o_l_o_r_=_%_4_d_c_7_1_f_&_l_a_b_e_l_=_L_a_s_t_%_2_0_C_o_m_m_i_t_&_l_o_g_o_=_g_i_t_h_u_b_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
               _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_G_i_o_r_g_o_s_X_o_u_/
             _T_U_I_F_I_M_a_n_a_g_e_r_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_l_o_g_o_=_G_N_U_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
@@ -67,47 +67,48 @@
 first have to press the space-bar and then type the command. Alternatively, use
 `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice:
 it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen
 below and can be found under the `~/.config/tuifi/cmds.conf` where you can add
 your custom ones too:** | Cmd | Type | Attributes | Label Information| |---|---
 |---|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` |
 open | 'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':
-'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
-'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`, [`find`]
-(## 'Attributes: `filename`') **important note:** `o` is also used for ordering
-in `vim_mode`. In this case you can first press space-bar before proceeding
-with `owv` or with any other already reserved starting key, or just change it.
-**Additionally** there are also some "static" ones like the `m`+character which
-marks the current directory into the character, so you can navigate back to it
-by using \` or `;`+that_character # ð Documentation Work in progress
-ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
-`tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests
-pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
-slightly, **use it as: Drag&drop + click afterwords where you want the file to
-be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
-discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
-issues/21) How do I set the default editor? > Set `tuifi_default_editor`
-enviroment variable to `vim` or whatever you prefer How do I disable the auto-
-find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
-to `False` How do I change the scroll sensitivity? > You can set either or both
-`tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental
-variables, to the disered number of characters per scroll action *(they default
-to 1 and 7)* How do I change the default keys (besides commands)? > This is not
-possible right now althought you could play around with the content of
-`toggle_vim_mode` function under `__init__.py` How do I change the number of
-visible lines of filenames that are visible? > You can set how mnay lines you
-want using `tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the
-default configuration path? > Set `tuifi_config_path` enviroment variable to
-whatever you prefer most How do I toggle hidden files/folders? > You can either
-`CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True` How do I
-change the default colors? > [look here for more informations](https://
-github.com/GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need
-money to survive, I have no job, living in a basement, making things for free,
-because I love to. - [***Paypal Address***](https://www.paypal.com/donate/
+'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\\\\.txt' || |`yy` | copy
+| 'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`,
+[`find`](## 'Attributes: `filename`') **important note:** `o` is also used for
+ordering in `vim_mode`. In this case you can first press space-bar before
+proceeding with `owv` or with any other already reserved starting key, or just
+change it. **Additionally** there are also some "static" ones like the
+`m`+character which marks the current directory into the character, so you can
+navigate back to it by using \` or `;`+that_character # ð Documentation Work
+in progress ð ï¸ð ... # ð­ Customization How do I enable vim_mode? >
+Set `tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic
+XDND? > set `tuifi_synth_dnd` enviroment variable to `True`. `pip install
+requests pynput PySide6 python-xlib`. Know it's expirimental! You'll need to
+adapt to it slightly, **use it as: Drag&drop + click afterwords where you want
+the file to be dropped.** [See also](https://github.com/GiorgosXou/
+TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/
+TUIFIManager/issues/21) How do I set the default editor? > Set
+`tuifi_default_editor` enviroment variable to `vim` or whatever you prefer How
+do I disable the auto-find-mode? > You can just set `tuifi_auto_find_on_typing`
+enviroment variable to `False` How do I change the scroll sensitivity? > You
+can set either or both `tuifi_scroll_sensitivity`,
+`tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number
+of characters per scroll action *(they default to 1 and 7)* How do I change the
+default keys (besides commands)? > This is not possible right now althought you
+could play around with the content of `toggle_vim_mode` function under
+`__init__.py` How do I change the number of visible lines of filenames that are
+visible? > You can set how mnay lines you want using
+`tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the default
+configuration path? > Set `tuifi_config_path` enviroment variable to whatever
+you prefer most How do I toggle hidden files/folders? > You can either `CTRL +
+T` or set `tuifi_show_hidden` enviroment variable to `True` How do I change the
+default colors? > [look here for more informations](https://github.com/
+GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need money to
+survive, I have no job, living in a basement, making things for free, because I
+love to. - [***Paypal Address***](https://www.paypal.com/donate/
 ?hosted_button_id=QNQN23M55EJVS) - ***Monero Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
 # ð«¶ Special thanks to - [@KORBEN for this article](https://korben.info/
 gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-
 personnalisable.html) - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
```

### Comparing `TUIFIManager-4.0.5/Peek.gif` & `TUIFIManager-4.0.6/Peek.gif`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/README.md` & `TUIFIManager-4.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 **(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
 | Cmd | Type | Attributes | Label Information|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
-|`yat` | copy | 'pattern':'.+\.txt'                     ||
+|`yat` | copy | 'pattern':'.+\\\\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
 **Available Type-keywords:** `open`, `copy`, `cut`, [`find`](## 'Attributes: `filename`')
 
 **important note:** `o` is also used for ordering in `vim_mode`. In this case you can first press space-bar before proceeding with `owv` or with any other already reserved starting key, or just change it. 
 
 **Additionally** there are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character
```

#### html2text {}

```diff
@@ -52,47 +52,48 @@
 first have to press the space-bar and then type the command. Alternatively, use
 `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice:
 it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen
 below and can be found under the `~/.config/tuifi/cmds.conf` where you can add
 your custom ones too:** | Cmd | Type | Attributes | Label Information| |---|---
 |---|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` |
 open | 'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':
-'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
-'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`, [`find`]
-(## 'Attributes: `filename`') **important note:** `o` is also used for ordering
-in `vim_mode`. In this case you can first press space-bar before proceeding
-with `owv` or with any other already reserved starting key, or just change it.
-**Additionally** there are also some "static" ones like the `m`+character which
-marks the current directory into the character, so you can navigate back to it
-by using \` or `;`+that_character # ð Documentation Work in progress
-ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
-`tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests
-pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
-slightly, **use it as: Drag&drop + click afterwords where you want the file to
-be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
-discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
-issues/21) How do I set the default editor? > Set `tuifi_default_editor`
-enviroment variable to `vim` or whatever you prefer How do I disable the auto-
-find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
-to `False` How do I change the scroll sensitivity? > You can set either or both
-`tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental
-variables, to the disered number of characters per scroll action *(they default
-to 1 and 7)* How do I change the default keys (besides commands)? > This is not
-possible right now althought you could play around with the content of
-`toggle_vim_mode` function under `__init__.py` How do I change the number of
-visible lines of filenames that are visible? > You can set how mnay lines you
-want using `tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the
-default configuration path? > Set `tuifi_config_path` enviroment variable to
-whatever you prefer most How do I toggle hidden files/folders? > You can either
-`CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True` How do I
-change the default colors? > [look here for more informations](https://
-github.com/GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need
-money to survive, I have no job, living in a basement, making things for free,
-because I love to. - [***Paypal Address***](https://www.paypal.com/donate/
+'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\\\\.txt' || |`yy` | copy
+| 'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`,
+[`find`](## 'Attributes: `filename`') **important note:** `o` is also used for
+ordering in `vim_mode`. In this case you can first press space-bar before
+proceeding with `owv` or with any other already reserved starting key, or just
+change it. **Additionally** there are also some "static" ones like the
+`m`+character which marks the current directory into the character, so you can
+navigate back to it by using \` or `;`+that_character # ð Documentation Work
+in progress ð ï¸ð ... # ð­ Customization How do I enable vim_mode? >
+Set `tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic
+XDND? > set `tuifi_synth_dnd` enviroment variable to `True`. `pip install
+requests pynput PySide6 python-xlib`. Know it's expirimental! You'll need to
+adapt to it slightly, **use it as: Drag&drop + click afterwords where you want
+the file to be dropped.** [See also](https://github.com/GiorgosXou/
+TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/
+TUIFIManager/issues/21) How do I set the default editor? > Set
+`tuifi_default_editor` enviroment variable to `vim` or whatever you prefer How
+do I disable the auto-find-mode? > You can just set `tuifi_auto_find_on_typing`
+enviroment variable to `False` How do I change the scroll sensitivity? > You
+can set either or both `tuifi_scroll_sensitivity`,
+`tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number
+of characters per scroll action *(they default to 1 and 7)* How do I change the
+default keys (besides commands)? > This is not possible right now althought you
+could play around with the content of `toggle_vim_mode` function under
+`__init__.py` How do I change the number of visible lines of filenames that are
+visible? > You can set how mnay lines you want using
+`tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the default
+configuration path? > Set `tuifi_config_path` enviroment variable to whatever
+you prefer most How do I toggle hidden files/folders? > You can either `CTRL +
+T` or set `tuifi_show_hidden` enviroment variable to `True` How do I change the
+default colors? > [look here for more informations](https://github.com/
+GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need money to
+survive, I have no job, living in a basement, making things for free, because I
+love to. - [***Paypal Address***](https://www.paypal.com/donate/
 ?hosted_button_id=QNQN23M55EJVS) - ***Monero Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
 # ð«¶ Special thanks to - [@KORBEN for this article](https://korben.info/
 gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-
 personnalisable.html) - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
```

### Comparing `TUIFIManager-4.0.5/TUIFI.png` & `TUIFIManager-4.0.6/TUIFI.png`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/TUIFIManager/TUIFIProfile.py` & `TUIFIManager-4.0.6/TUIFIManager/TUIFIProfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,21 +404,21 @@
         ' ╭━━━━━━╮ \n'
         ' ┃ $_   ┃ \n'
         ' ┇ BASH ┇ \n'
         ' ╰━━━━━━╯ '
     ),2, DEFAULT_EDITOR),
     '/cmd':TUIFIProfile((
         ' ╭━━━━━━╮ \n'
-        ' ┃ C:\> ┃ \n'
+        ' ┃ C:\\> ┃ \n'
         ' ┇ CMD_ ┇ \n'
         ' ╰━━━━━━╯ '
     ),2, DEFAULT_EDITOR),
     '/bat':TUIFIProfile((
         ' ╭━━━━━━╮ \n'
-        ' ┃ C:\> ┃ \n'
+        ' ┃ C:\\> ┃ \n'
         ' ┇ BAT_ ┇ \n'
         ' ╰━━━━━━╯ '
     ),2, DEFAULT_EDITOR),
     '/so':TUIFIProfile((
         ' ╭━╭━┳╭━╮ \n'
         ' │S│O┠│Ξ│ \n'
         ' │▒│█┠│▒│ \n'
@@ -715,17 +715,17 @@
         ' ┃DB┇┏▄ ┇ \n'
         ' ┇▓░ ┣┻▄┃ \n'
         ' ┗━━ ▀  ┛ '
     ),8, DEFAULT_EDITOR),
 
 
     '/tuifi':TUIFIProfile((
-        '             \                                      [            \n'
+        '             \\                                      [            \n'
         '              @                 ⟡                  ╢             \n'
-        '      /       ╣▒                                  ]▒       \     \n'
+        '      /       ╣▒                                  ]▒       \\     \n'
         '     ╔       ]Ñ▒                                  ╟╣┐       ▓    \n'
         '    ╢╣       ╣▓            √          t            ▓╣       ▓╣   \n'
         '   ▓╣▒╖    ╓╫╜           ╥▓   #TUIFI   ▓@           ╙▓╖    ╔╣╢║  \n'
         '   ▓▓▓▓  ,p▓,,,,,,      ╜╙▓▄╖,      ,╓╥╜╙╙    ,,,,,,,,▓▓,  ▀▓▓╣U \n'
         '   ▀▓Ö   ╙█▓▓▓▓▓▓╢╫╣▓▓▓▓▓╦, ▀▓▓╗  g╢▓╝ ,╓H╢╢╢╢╢╢▓▓▓▓▓▓▒▓╜   ]▓▓  \n'
         '    ▓▓▓╦╥╖ ╙╙╙╙`     `""▀▓▓@ ▐█▓L]▓╫╛ Æ▒╨╜"       ""╙╙` ╓╖∩▒▒▓   \n'
         ' ╒▓▒╜""╙▀▓▓                ▀  █▒Γ▐▓▓  ╩                ▓╢╜""╙▀█╫L\n'
```

### Comparing `TUIFIManager-4.0.5/TUIFIManager/TUIFile.py` & `TUIFIManager-4.0.6/TUIFIManager/TUIFile.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/TUIFIManager/TUIMenu.py` & `TUIFIManager-4.0.6/TUIFIManager/TUIMenu.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/TUIFIManager/TUISynthXDND.py` & `TUIFIManager-4.0.6/TUIFIManager/TUISynthXDND.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/TUIFIManager/TUItilities.py` & `TUIFIManager-4.0.6/TUIFIManager/TUItilities.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/TUIFIManager/__init__.py` & `TUIFIManager-4.0.6/TUIFIManager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 from        os.path import basename
 from       .TUIMenu import TUIMenu
 from       .TUIFile import TUIFile
 from   .TUItilities import WindowPad, Cd, Label, END_MOUSE, BEGIN_MOUSE, BEGIN_MOUSE, END_MOUSE, IS_WINDOWS, HOME_DIR, IS_TERMUX
 from  .TUIFIProfile import TUIFIProfiles, DEFAULT_PROFILE , DEFAULT_WITH, DEFAULT_OPENER
 import   subprocess
 import    unicurses
+import     warnings
 import       shutil
 import       signal
 import         json
 import          ast
 import           re
 import           os
 
-__version__: Final[str] = "4.0.5"
+__version__: Final[str] = "4.0.6"
 
 PADDING_LEFT   = 2
 PADDING_RIGHT  = 2
 PADDING_TOP    = 1
 PADDING_BOTTOM = 0
 
 SCROLL_SENSITIVITY      = int(os.getenv('tuifi_scroll_sensitivity'     , 1))
@@ -94,14 +95,15 @@
     info_label         = None
 
     def __init__(self, y=0, x=0, height=30, width=45, anchor=(False,False,False,False), directory=HOME_DIR, suffixes=[], sort_by=None, has_label=True, win=None, draw_files=True, termux_touch_only=True, auto_find_on_typing=True, auto_cmd_on_typing=False, vim_mode=False, is_focused=False, cd=False, show_hidden=False):
         if has_label:
             height -= 1
             self.info_label       = Label(y+height, x, 1, width, (False,anchor[1],anchor[2],anchor[3]), f' TUIFIManager {__version__} | Powered by uni-curses', win)
             self.info_label.style = unicurses.A_REVERSE | unicurses.A_BOLD
+            warnings.showwarning = self.custom_warning_handler
 
         super().__init__(win, y, x, height, width, anchor, is_focused)
         self.__order_method      = sort_by
         self.suffixes            = suffixes
         self.draw_files          = draw_files
         self.termux_touch_only   = termux_touch_only
         self.auto_find_on_typing = os.getenv('tuifi_auto_find_on_typing'   , str(auto_find_on_typing)) == 'True' 
@@ -133,14 +135,25 @@
         self.__set_normal_events()
         if stty_a('^Z')               : signal.signal(signal.SIGTSTP, self.suspend_proccess)
         if stty_a('^C') or IS_WINDOWS : signal.signal(signal.SIGINT , self.copy            ) # https://docs.microsoft.com/en-us/windows/console/ctrl-c-and-ctrl-break-signals
         if os.getenv('tuifi_vim_mode', str(vim_mode)) == 'True'   : self.toggle_vim_mode()
         if IS_DRAG_N_DROP: self.drag_and_drop = SyntheticXDND(self.handle_gui_to_tui_dropped_file, self.__get_selected_files) #NOTE: https://stackoverflow.com/a/14829479/11465149
 
 
+    def custom_warning_handler(self, message, category, filename, lineno, file=None, line=None):
+        self.info_label.color_pair = 3
+        self.info_label.style = unicurses.A_BOLD
+        if category.__name__ == SyntaxWarning.__name__:
+            self.__set_label_text(f" Please check Issue #111 | {category.__name__}: {message} at {filename}:{lineno}")
+        else:
+            self.__set_label_text(f" {category.__name__}: {message} at {filename}:{lineno}")
+        self.info_label.color_pair = 2
+        self.info_label.style = unicurses.A_REVERSE | unicurses.A_BOLD
+
+
     def suspend_proccess(self, signum, frame): # Kinda SuS but you know the deal...
         print(END_MOUSE)
         with self.suspend():
             os.kill(os.getpid(), signal.SIGSTOP)
         print(BEGIN_MOUSE)
         unicurses.clear()
 
@@ -339,16 +352,15 @@
             unicurses.endwin()
             yield
         finally:
             unicurses.doupdate()
 
 
     def __try_open_with(self, directory: str, open_with: Optional[str], multiple=False) -> None:
-        if not open_with:
-            return self.__set_label_on_file_selection()
+        if not open_with: return
 
         dirs = []
         if multiple: # puke-able shit lol xD, sorry for that
             for f in self.files: # TODO: Save selected to a temp list becuase this is really costy! (decisions..) 
                 if f.is_selected: 
                     if f.profile.open_with != DEFAULT_OPENER:
                         dirs.append(self.directory+sep+f.name)
@@ -361,15 +373,14 @@
         if not dirs: return # Although not needed just in case for other DEFAULT_OPENERs
 
         print(END_MOUSE, end='\r')
         with self.suspend():
             proc = subprocess.Popen([open_with, *dirs], shell=IS_WINDOWS) # TODO: optional stdout=subprocess.DEVNULL when I'll add loading TUIFIProfiles from external file ?
             proc.wait()
         print(BEGIN_MOUSE, end='\r')
-        self.__set_label_on_file_selection()
         return
 
 
     def __reset_open(self):
         if self.vim_mode and self.escape_event_consumed and not self.is_in_command_mode: # SuS SuS SuS SuS SuS damn that's so Sus lol | 2024-04-05 08:48:24 PM this was for keeping search/find/input mode after opening a folder but i didn't like it and removed it
             self.find()
         else:
@@ -1075,15 +1086,15 @@
         conf_path = path + sep + 'cmds.conf'
         if not os.path.isfile(conf_path): 
             f = open(conf_path, 'w')
             f.write(
                 "gt  | open | 'directory':'~/.config/tuifi' | - tuifi -\n"       +
                 "gh  | open | 'directory':'~/'              | - Home -\n"        +
                 "owv | open | 'directory':None,'_with':'vim'|Opened With Vim\n"  +
-                "yat | copy | 'pattern':'.+\.txt'           |\n"                 +
+                "yat | copy | 'pattern':'.+\\\\.txt'          |\n"               +
                 "yy  | copy | 'pattern':None                |\n" 
             )
             f.close()
         f = open(conf_path, 'r')
         for line in f:
             ln = line.strip()
             if ln == '': continue
```

### Comparing `TUIFIManager-4.0.5/TUIFIManager/__main__.py` & `TUIFIManager-4.0.6/TUIFIManager/__main__.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/TUIFIManager.egg-info/PKG-INFO` & `TUIFIManager-4.0.6/TUIFIManager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 4.0.5
+Version: 4.0.6
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
-Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: windows
 Classifier: Intended Audience :: Developers
@@ -22,14 +21,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: uni-curses>=2.1.3
+Requires-Dist: Send2Trash>=1.8.0
 
 
 
 <div align="center">
 <h1>TUIFI Manager</h1>
 <p>
     <a href="https://github.com/GiorgosXou/TUIFIManager/pulse">
@@ -138,15 +139,15 @@
 **(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
 | Cmd | Type | Attributes | Label Information|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
-|`yat` | copy | 'pattern':'.+\.txt'                     ||
+|`yat` | copy | 'pattern':'.+\\\\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
 **Available Type-keywords:** `open`, `copy`, `cut`, [`find`](## 'Attributes: `filename`')
 
 **important note:** `o` is also used for ordering in `vim_mode`. In this case you can first press space-bar before proceeding with `owv` or with any other already reserved starting key, or just change it. 
 
 **Additionally** there are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.5 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.6 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
-gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
-https://github.com/GiorgosXou/TUIFIManager Keywords: file-
+gxousos@gmail.com License: General Public License v3.0 Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: End Users/Desktop Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+uni-curses>=2.1.3 Requires-Dist: Send2Trash>=1.8.0
                           ************ TTUUIIFFII MMaannaaggeerr ************
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_G_i_o_r_g_o_s_X_o_u_/
  _T_U_I_F_I_M_a_n_a_g_e_r_?_c_o_l_o_r_=_%_4_d_c_7_1_f_&_l_a_b_e_l_=_L_a_s_t_%_2_0_C_o_m_m_i_t_&_l_o_g_o_=_g_i_t_h_u_b_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
               _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_G_i_o_r_g_o_s_X_o_u_/
             _T_U_I_F_I_M_a_n_a_g_e_r_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_l_o_g_o_=_G_N_U_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
@@ -67,47 +67,48 @@
 first have to press the space-bar and then type the command. Alternatively, use
 `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice:
 it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen
 below and can be found under the `~/.config/tuifi/cmds.conf` where you can add
 your custom ones too:** | Cmd | Type | Attributes | Label Information| |---|---
 |---|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` |
 open | 'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':
-'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
-'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`, [`find`]
-(## 'Attributes: `filename`') **important note:** `o` is also used for ordering
-in `vim_mode`. In this case you can first press space-bar before proceeding
-with `owv` or with any other already reserved starting key, or just change it.
-**Additionally** there are also some "static" ones like the `m`+character which
-marks the current directory into the character, so you can navigate back to it
-by using \` or `;`+that_character # ð Documentation Work in progress
-ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
-`tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests
-pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
-slightly, **use it as: Drag&drop + click afterwords where you want the file to
-be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
-discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
-issues/21) How do I set the default editor? > Set `tuifi_default_editor`
-enviroment variable to `vim` or whatever you prefer How do I disable the auto-
-find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
-to `False` How do I change the scroll sensitivity? > You can set either or both
-`tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental
-variables, to the disered number of characters per scroll action *(they default
-to 1 and 7)* How do I change the default keys (besides commands)? > This is not
-possible right now althought you could play around with the content of
-`toggle_vim_mode` function under `__init__.py` How do I change the number of
-visible lines of filenames that are visible? > You can set how mnay lines you
-want using `tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the
-default configuration path? > Set `tuifi_config_path` enviroment variable to
-whatever you prefer most How do I toggle hidden files/folders? > You can either
-`CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True` How do I
-change the default colors? > [look here for more informations](https://
-github.com/GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need
-money to survive, I have no job, living in a basement, making things for free,
-because I love to. - [***Paypal Address***](https://www.paypal.com/donate/
+'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\\\\.txt' || |`yy` | copy
+| 'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`,
+[`find`](## 'Attributes: `filename`') **important note:** `o` is also used for
+ordering in `vim_mode`. In this case you can first press space-bar before
+proceeding with `owv` or with any other already reserved starting key, or just
+change it. **Additionally** there are also some "static" ones like the
+`m`+character which marks the current directory into the character, so you can
+navigate back to it by using \` or `;`+that_character # ð Documentation Work
+in progress ð ï¸ð ... # ð­ Customization How do I enable vim_mode? >
+Set `tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic
+XDND? > set `tuifi_synth_dnd` enviroment variable to `True`. `pip install
+requests pynput PySide6 python-xlib`. Know it's expirimental! You'll need to
+adapt to it slightly, **use it as: Drag&drop + click afterwords where you want
+the file to be dropped.** [See also](https://github.com/GiorgosXou/
+TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/
+TUIFIManager/issues/21) How do I set the default editor? > Set
+`tuifi_default_editor` enviroment variable to `vim` or whatever you prefer How
+do I disable the auto-find-mode? > You can just set `tuifi_auto_find_on_typing`
+enviroment variable to `False` How do I change the scroll sensitivity? > You
+can set either or both `tuifi_scroll_sensitivity`,
+`tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number
+of characters per scroll action *(they default to 1 and 7)* How do I change the
+default keys (besides commands)? > This is not possible right now althought you
+could play around with the content of `toggle_vim_mode` function under
+`__init__.py` How do I change the number of visible lines of filenames that are
+visible? > You can set how mnay lines you want using
+`tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the default
+configuration path? > Set `tuifi_config_path` enviroment variable to whatever
+you prefer most How do I toggle hidden files/folders? > You can either `CTRL +
+T` or set `tuifi_show_hidden` enviroment variable to `True` How do I change the
+default colors? > [look here for more informations](https://github.com/
+GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need money to
+survive, I have no job, living in a basement, making things for free, because I
+love to. - [***Paypal Address***](https://www.paypal.com/donate/
 ?hosted_button_id=QNQN23M55EJVS) - ***Monero Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
 # ð«¶ Special thanks to - [@KORBEN for this article](https://korben.info/
 gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-
 personnalisable.html) - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
```

### Comparing `TUIFIManager-4.0.5/TUIFIManager.egg-info/SOURCES.txt` & `TUIFIManager-4.0.6/TUIFIManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/flake.lock` & `TUIFIManager-4.0.6/flake.lock`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.5/flake.nix` & `TUIFIManager-4.0.6/flake.nix`

 * *Files 23% similar despite different names*

```diff
@@ -14,60 +14,87 @@
     flake-utils.lib.eachSystem [
       "x86_64-linux"
       "aarch64-linux"
       "aarch64-darwin"
       "x86_64-darwin"
     ] (system: let
       pkgs = nixpkgs.legacyPackages.${system};
+      py = {
+        env = pkgs.python311.withPackages (p: py.deps);
+        pkgs = pkgs.python311.pkgs;
+        deps = with pkgs.python311.pkgs;
+          [
+            send2trash
+            unicurses
+          ]
+          # pyinput is marked as broken for darwin
+          # pkgs.gnome3.gnome-themes-extra
+          ++ (pkgs.lib.optionals pkgs.stdenv.isLinux [
+            pynput
+            pyside6
+            requests
+            xlib
+          ]);
+      };
     in {
-      devShells.default = let
-        py-env = pkgs.python310.withPackages (p: [
-          p.send2trash
-          p.unicurses
-        ]);
-      in
-        pkgs.mkShell {
-          LD_LIBRARY_PATH = pkgs.lib.makeLibraryPath [pkgs.ncurses];
-          packages = [
-            py-env
-            py-env.pkgs.venvShellHook
-            pkgs.gnumake
-          ];
-
-          venvDir = "venv";
-          postVenvCreation = ''
-            pip install -r requirements.txt
-            pip install -e .
-          '';
-        };
+      devShells.default = pkgs.mkShell {
+        LD_LIBRARY_PATH = pkgs.lib.makeLibraryPath [pkgs.ncurses];
+        packages = [
+          py.env
+          py.env.pkgs.venvShellHook
+          pkgs.gnumake
+        ];
+
+        venvDir = "venv";
+        postVenvCreation = ''
+          pip install -r requirements.txt
+          pip install -e .
+        '';
+      };
 
       formatter = pkgs.alejandra;
       packages = rec {
         default = tuifi-manager;
         tuifi-manager = let
           pyproject = builtins.readFile ./pyproject.toml;
           version = (builtins.fromTOML pyproject).project.version;
         in
-          with pkgs.python3.pkgs;
-            buildPythonApplication {
-              pname = "tuifi-manager";
-              inherit version;
+          py.pkgs.buildPythonApplication {
+            pname = "tuifi-manager";
+            inherit version;
 
-              src = ./.;
-              format = "pyproject";
+            src = ./.;
+            format = "pyproject";
 
-              nativeBuildInputs = [
+            nativeBuildInputs =
+              (with py.pkgs; [
                 setuptools
                 setuptools-scm
-              ];
-
-              propagatedBuildInputs = [
-                send2trash
-                unicurses
-              ];
-
-              pythonImportsCheck = ["TUIFIManager"];
-              meta.mainProgram = "tuifi";
-            };
+              ])
+              ++ (pkgs.lib.optionals pkgs.stdenv.isLinux [
+                pkgs.qt6.wrapQtAppsHook
+                pkgs.makeWrapper
+              ]);
+
+            propagatedBuildInputs =
+              py.deps
+              ++ (with pkgs.kdePackages;
+                pkgs.lib.optionals pkgs.stdenv.isLinux [
+                  qtbase
+                  qt6gtk2
+                ]);
+
+            postFixup = let
+              # https://github.com/NixOS/nixpkgs/issues/60918
+              theme = pkgs.gnome3.gnome-themes-extra;
+            in
+              pkgs.lib.optionalString pkgs.stdenv.isLinux ''
+                wrapProgram $out/bin/tuifi \
+                  --prefix GTK_PATH : "${theme}/lib/gtk-2.0"
+              '';
+
+            pythonImportsCheck = ["TUIFIManager"];
+            meta.mainProgram = "tuifi";
+          };
       };
     });
 }
```

### Comparing `TUIFIManager-4.0.5/pyproject.toml` & `TUIFIManager-4.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TUIFIManager"
-version = "4.0.5"
+version = "4.0.6"
 
 description = "A cross-platform terminal-based termux-oriented file manager."
 requires-python = ">=3.8"
 readme = "README.md"
 
 dependencies = [
     "uni-curses >= 2.1.3",
```

### Comparing `TUIFIManager-4.0.5/setup.cfg` & `TUIFIManager-4.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TUIFIManager
-version = 4.0.5
+version = 4.0.6
 description = A cross-platform terminal-based termux-oriented file manager
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 author = George Chousos
 author_email = gxousos@gmail.com
 keywords = file-manager, terminal, tui, ncurses, pdcurses, uni-curses, termux, vim, vim-motions, cross-platform
 license = GPL-3.0
```

