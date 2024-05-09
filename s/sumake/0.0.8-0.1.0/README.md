# Comparing `tmp/sumake-0.0.8.tar.gz` & `tmp/sumake-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumake-0.0.8.tar", last modified: Mon Apr  1 06:49:13 2024, max compression
+gzip compressed data, was "sumake-0.1.0.tar", last modified: Thu May  9 03:56:50 2024, max compression
```

## Comparing `sumake-0.0.8.tar` & `sumake-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-04-01 06:49:13.530713 sumake-0.0.8/
--rw-r--r--   0 peng       (501) staff       (20)       32 2023-05-11 04:17:43.000000 sumake-0.0.8/MANIFEST.in
--rw-r--r--   0 peng       (501) staff       (20)      474 2024-04-01 06:49:13.530476 sumake-0.0.8/PKG-INFO
--rw-r--r--   0 peng       (501) staff       (20)      259 2023-08-04 10:39:20.000000 sumake-0.0.8/README.md
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-04-01 06:49:13.527916 sumake-0.0.8/bin/
--rw-r--r--   0 peng       (501) staff       (20)      923 2024-04-01 06:49:13.000000 sumake-0.0.8/bin/sumake
--rw-r--r--   0 peng       (501) staff       (20)       38 2024-04-01 06:49:13.530762 sumake-0.0.8/setup.cfg
--rw-r--r--   0 peng       (501) staff       (20)     2472 2024-03-29 09:56:34.000000 sumake-0.0.8/setup.py
--rwxr--r--   0 peng       (501) staff       (20)      913 2023-11-29 14:52:46.000000 sumake-0.0.8/sumake
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-04-01 06:49:13.529117 sumake-0.0.8/sumake.egg-info/
--rw-r--r--   0 peng       (501) staff       (20)      474 2024-04-01 06:49:13.000000 sumake-0.0.8/sumake.egg-info/PKG-INFO
--rw-r--r--   0 peng       (501) staff       (20)      254 2024-04-01 06:49:13.000000 sumake-0.0.8/sumake.egg-info/SOURCES.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2024-04-01 06:49:13.000000 sumake-0.0.8/sumake.egg-info/dependency_links.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2024-04-01 06:49:13.000000 sumake-0.0.8/sumake.egg-info/not-zip-safe
--rw-r--r--   0 peng       (501) staff       (20)       11 2024-04-01 06:49:13.000000 sumake-0.0.8/sumake.egg-info/requires.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2024-04-01 06:49:13.000000 sumake-0.0.8/sumake.egg-info/top_level.txt
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-04-01 06:49:13.528846 sumake-0.0.8/test/
--rw-r--r--   0 peng       (501) staff       (20)      167 2023-05-10 05:44:52.000000 sumake-0.0.8/test/test_setup.py
--rw-r--r--   0 peng       (501) staff       (20)     1188 2024-03-29 09:59:43.000000 sumake-0.0.8/utils.mk
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-05-09 03:56:50.749072 sumake-0.1.0/
+-rw-r--r--   0 peng       (501) staff       (20)       32 2023-05-11 04:17:43.000000 sumake-0.1.0/MANIFEST.in
+-rw-r--r--   0 peng       (501) staff       (20)      474 2024-05-09 03:56:50.748777 sumake-0.1.0/PKG-INFO
+-rw-r--r--   0 peng       (501) staff       (20)      259 2023-08-04 10:39:20.000000 sumake-0.1.0/README.md
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-05-09 03:56:50.747637 sumake-0.1.0/bin/
+-rw-r--r--   0 peng       (501) staff       (20)      923 2024-05-09 03:56:50.000000 sumake-0.1.0/bin/sumake
+-rw-r--r--   0 peng       (501) staff       (20)       38 2024-05-09 03:56:50.749132 sumake-0.1.0/setup.cfg
+-rw-r--r--   0 peng       (501) staff       (20)     2737 2024-05-09 03:14:23.000000 sumake-0.1.0/setup.py
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-05-09 03:56:50.748387 sumake-0.1.0/sumake.egg-info/
+-rw-r--r--   0 peng       (501) staff       (20)      474 2024-05-09 03:56:50.000000 sumake-0.1.0/sumake.egg-info/PKG-INFO
+-rw-r--r--   0 peng       (501) staff       (20)      250 2024-05-09 03:56:50.000000 sumake-0.1.0/sumake.egg-info/SOURCES.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2024-05-09 03:56:50.000000 sumake-0.1.0/sumake.egg-info/dependency_links.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2024-05-09 03:56:50.000000 sumake-0.1.0/sumake.egg-info/not-zip-safe
+-rw-r--r--   0 peng       (501) staff       (20)       11 2024-05-09 03:56:50.000000 sumake-0.1.0/sumake.egg-info/requires.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2024-05-09 03:56:50.000000 sumake-0.1.0/sumake.egg-info/top_level.txt
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2024-05-09 03:56:50.747864 sumake-0.1.0/test/
+-rw-r--r--   0 peng       (501) staff       (20)      167 2023-05-10 05:44:52.000000 sumake-0.1.0/test/test_setup.py
```

### Comparing `sumake-0.0.8/bin/sumake` & `sumake-0.1.0/bin/sumake`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   -h, --help: show this help
   -v, --version: show version
   --zsh-init: init zsh completion
       "
       args+=("$1")
       ;;
     -v|--version)
-      echo "sumake: 0.0.8"
+      echo "sumake: 0.1.0"
       args+=("$1")
       ;;
     --zsh-init)
 append_content=$(cat <<EOF
 # sumake zsh completion
 autoload -U compinit
 compinit
```

### Comparing `sumake-0.0.8/setup.py` & `sumake-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,92 @@
 import os.path
 import shutil
 import sysconfig
 from pathlib import Path
 import time
 
-from setuptools import setup
+from setuptools import setup, find_packages
 from setuptools.command.install import install
 from setuptools.command.sdist import sdist
 from wheel.bdist_wheel import bdist_wheel
 
 
 home_dir = Path.home()
-install_dir = sysconfig.get_paths()['purelib']
+install_dir = sysconfig.get_paths()["purelib"]
 print(home_dir)
 print(install_dir)
 
 current = Path(__file__).parent.absolute()
+src_dir = current / "src"
 
+VERSION = "0.1.0"
 
-VERSION = "0.0.8"
 
 def generate_sumake(home_dir, current):
     sumake_dir = home_dir / ".sumake"
     bin_dir = current / "bin"
 
-    utils_mk = sumake_dir / "utils.mk"
-
     if not os.path.exists(sumake_dir):
         os.makedirs(sumake_dir)
     if not os.path.exists(bin_dir):
         os.makedirs(bin_dir)
     print("current", current)
+    print("src_dir", src_dir)
 
-    shutil.copy(current / "utils.mk", utils_mk)
+    utils_mk = sumake_dir / "utils.mk"
+    shutil.copy(src_dir / "utils.mk", utils_mk)
+    shutil.copy(src_dir / "utils.py", sumake_dir / "utils.py")
     # open("./sumake")
-    with open(current / "./sumake", "r") as template:
+    with open(src_dir / "sumake", "r") as template:
         with open(bin_dir / "sumake", "w") as target:
             res = template.read().format(
                 UTILS_MK=utils_mk,
-                VERSION=VERSION, )
+                VERSION=VERSION,
+            )
             target.write(res)
 
+
 def generate_version():
     with open(current / "version.txt", "w") as f:
         f.write(VERSION)
         # f.write(f"""VERSION = "{VERSION}" """)
 
+
 class PreBdistWheel(bdist_wheel):
     def run(self):
         generate_sumake(home_dir, current)
         bdist_wheel.run(self)
 
+
 class PreSDist(sdist):
     def run(self):
         generate_sumake(home_dir, current)
         sdist.run(self)
 
+
 class PreInstall(install):
     def run(self):
         generate_sumake(home_dir, current)
         install.run(self)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     generate_version()
     setup(
         author="SuCicada",
         author_email="pengyifu@gmail.com",
         classifiers=[],
         description="A generic makefile for projects.",
         scripts=["bin/sumake"],
         cmdclass={
             "install": PreInstall,
             "bdist_wheel": PreBdistWheel,
             "sdist": PreSDist,
         },
         install_requires=["setuptools"],
-
         include_package_data=True,
         # package_data={
         #     '': ['sumake', 'utils.mk'],
         # },
         # install_requires=[],
         # keywords="",
         # license="",
@@ -88,8 +95,11 @@
         # namespace_packages=[],
         # packages=find_packages(),
         # py_modules=["."],
         # test_suite="",
         url="https://github.com/SuCicada/sumake",
         version=VERSION,
         zip_safe=False,
-    )
+        packages=find_packages("src"),
+        package_dir={"": "src"},
+        options={'egg_info': {'egg_base': "./"}},
+)
```

