# Comparing `tmp/cugdt-1.0.2.tar.gz` & `tmp/cugdt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cugdt-1.0.2.tar", last modified: Thu May  9 11:01:36 2024, max compression
+gzip compressed data, was "dist\cugdt-1.0.3.tar", last modified: Thu May  9 11:13:06 2024, max compression
```

## Comparing `cugdt-1.0.2.tar` & `cugdt-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:36.521918 cugdt-1.0.2/
--rw-rw-rw-   0        0        0      281 2024-05-09 11:01:36.521918 cugdt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      122 2024-05-09 10:58:55.000000 cugdt-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:36.520476 cugdt-1.0.2/cugdt/
--rw-rw-rw-   0        0        0     2294 2024-05-09 10:53:12.000000 cugdt-1.0.2/cugdt/Tiff.py
--rw-rw-rw-   0        0        0        0 2024-05-09 07:05:34.000000 cugdt-1.0.2/cugdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:36.521918 cugdt-1.0.2/cugdt.egg-info/
--rw-rw-rw-   0        0        0      281 2024-05-09 11:01:36.000000 cugdt-1.0.2/cugdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-09 11:01:36.000000 cugdt-1.0.2/cugdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:01:36.000000 cugdt-1.0.2/cugdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-09 11:01:36.000000 cugdt-1.0.2/cugdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 11:01:36.000000 cugdt-1.0.2/cugdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 11:01:36.522919 cugdt-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2024-05-09 10:59:40.000000 cugdt-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:13:06.701720 cugdt-1.0.3/
+-rw-rw-rw-   0        0        0      281 2024-05-09 11:13:06.701720 cugdt-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-09 11:04:12.000000 cugdt-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 11:13:06.690421 cugdt-1.0.3/cugdt/
+-rw-rw-rw-   0        0        0     2294 2024-05-09 10:53:12.000000 cugdt-1.0.3/cugdt/Tiff.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 07:05:34.000000 cugdt-1.0.3/cugdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:13:06.700718 cugdt-1.0.3/cugdt.egg-info/
+-rw-rw-rw-   0        0        0      281 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:13:06.701720 cugdt-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-09 11:12:59.000000 cugdt-1.0.3/setup.py
```

### Comparing `cugdt-1.0.2/cugdt/Tiff.py` & `cugdt-1.0.3/cugdt/Tiff.py`

 * *Files identical despite different names*

### Comparing `cugdt-1.0.2/setup.py` & `cugdt-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
     name="cugdt",  # 这里是pip项目发布的名称
-    version="1.0.2",  # 版本号，数值大的会优先被pip
+    version="1.0.3",  # 版本号，数值大的会优先被pip
     keywords=["pip", "tiff", "cugdt"],  # 关键字
     description="Tiff文件读取，写入，压缩",  # 描述
     license="MIT Licence",  # 许可证
 
     url="https://gitee.com/HaixuHe/cugdt",  # 项目相关文件地址，一般是github项目地址即可
     author="HaixuHe",  # 作者
     author_email="20161001925@cug.edu.cn",
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
-    install_requires=["gdal"]  # 这个项目依赖的第三方库
+    install_requires=[]  # 这个项目依赖的第三方库
 )
```

