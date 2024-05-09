# Comparing `tmp/cugdt-1.0.4.tar.gz` & `tmp/cugdt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cugdt-1.0.4.tar", last modified: Thu May  9 11:20:24 2024, max compression
+gzip compressed data, was "dist\cugdt-1.0.5.tar", last modified: Thu May  9 13:58:52 2024, max compression
```

## Comparing `cugdt-1.0.4.tar` & `cugdt-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:20:24.343888 cugdt-1.0.4/
--rw-rw-rw-   0        0        0      781 2024-05-09 11:20:24.343888 cugdt-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-09 11:04:12.000000 cugdt-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:20:24.341888 cugdt-1.0.4/cugdt/
--rw-rw-rw-   0        0        0     2294 2024-05-09 10:53:12.000000 cugdt-1.0.4/cugdt/Tiff.py
--rw-rw-rw-   0        0        0        0 2024-05-09 07:05:34.000000 cugdt-1.0.4/cugdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:20:24.343888 cugdt-1.0.4/cugdt.egg-info/
--rw-rw-rw-   0        0        0      781 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 11:20:24.343888 cugdt-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1341 2024-05-09 11:20:12.000000 cugdt-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:58:52.158626 cugdt-1.0.5/
+-rw-rw-rw-   0        0        0      781 2024-05-09 13:58:52.158626 cugdt-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-09 11:04:12.000000 cugdt-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 13:58:52.155626 cugdt-1.0.5/cugdt/
+-rw-rw-rw-   0        0        0     2163 2024-05-09 13:56:21.000000 cugdt-1.0.5/cugdt/Tiff.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 07:05:34.000000 cugdt-1.0.5/cugdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:58:52.158626 cugdt-1.0.5/cugdt.egg-info/
+-rw-rw-rw-   0        0        0      781 2024-05-09 13:58:52.000000 cugdt-1.0.5/cugdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-05-09 13:58:52.000000 cugdt-1.0.5/cugdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:58:52.000000 cugdt-1.0.5/cugdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 13:58:52.000000 cugdt-1.0.5/cugdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:58:52.158626 cugdt-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2024-05-09 13:58:45.000000 cugdt-1.0.5/setup.py
```

### Comparing `cugdt-1.0.4/PKG-INFO` & `cugdt-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cugdt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tiff文件读取，写入，压缩
 Home-page: https://gitee.com/HaixuHe/cugdt
 Author: HaixuHe
 Author-email: 20161001925@cug.edu.cn
 License: MIT Licence
 Description: UNKNOWN
 Keywords: pip,tiff,cugdt
```

### Comparing `cugdt-1.0.4/cugdt/Tiff.py` & `cugdt-1.0.5/cugdt/Tiff.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,52 +13,54 @@
 
     im_geotrans = dataset.GetGeoTransform()  # 获取仿射矩阵信息
     im_proj = dataset.GetProjection()  # 获取投影信息
     return im_data, im_geotrans, im_proj
 
 
 # 写入tiff文件
-def CreateGeoTiff(outRaster, image, geo_transform, projection, dtype='float'):
+def CreateGeoTiff(outRaster, image, geo_transform, projection, dtype='float', compress=False):
     no_bands = 0
     rows = 0
     cols = 0
 
     driver = gdal.GetDriverByName('GTiff')
     if len(image.shape) == 2:
         no_bands = 1
         rows, cols = image.shape
     elif len(image.shape) == 3:
         no_bands, rows, cols = image.shape
 
     if dtype == 'int16' or dtype == 'int':
-        DataSet = driver.Create(outRaster, cols, rows, no_bands, gdal.GDT_Int16,
-                                options=["TILED=YES", "COMPRESS={0}".format("LZW")])
+        dtype = gdal.GDT_Int16
     elif dtype == 'int32':
-        DataSet = driver.Create(outRaster, cols, rows, no_bands, gdal.GDT_Int32,
-                                options=["TILED=YES", "COMPRESS={0}".format("LZW")])
+        dtype = gdal.GDT_Int32
     else:
-        DataSet = driver.Create(outRaster, cols, rows, no_bands, gdal.GDT_Float32,
+        dtype = gdal.GDT_Float32
+    if compress:
+        DataSet = driver.Create(outRaster, cols, rows, no_bands, dtype,
                                 options=["TILED=YES", "COMPRESS={0}".format("LZW")])
+    else:
+        DataSet = driver.Create(outRaster, cols, rows, no_bands, dtype)
 
     DataSet.SetGeoTransform(geo_transform)
     DataSet.SetProjection(projection)
 
     if no_bands == 1:
         DataSet.GetRasterBand(1).WriteArray(image)  # 写入数组数据
     else:
         for i in range(no_bands):
             DataSet.GetRasterBand(i + 1).WriteArray(image[i])
     del DataSet
 
+
 # 压缩tiff文件
 def CompressGeoTiff(path, method="LZW"):
     """使用gdal进行文件压缩，
           LZW方法属于无损压缩"""
     dataset = gdal.Open(path)
     driver = gdal.GetDriverByName('GTiff')
     target_path = path.replace('.tif', '_temp.tif')
 
     driver.CreateCopy(target_path, dataset, strict=1, options=["TILED=YES", "COMPRESS={0}".format(method)])
     os.remove(path)
     os.rename(target_path, path)
     del dataset
-
```

### Comparing `cugdt-1.0.4/cugdt.egg-info/PKG-INFO` & `cugdt-1.0.5/cugdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cugdt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tiff文件读取，写入，压缩
 Home-page: https://gitee.com/HaixuHe/cugdt
 Author: HaixuHe
 Author-email: 20161001925@cug.edu.cn
 License: MIT Licence
 Description: UNKNOWN
 Keywords: pip,tiff,cugdt
```

### Comparing `cugdt-1.0.4/setup.py` & `cugdt-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
     name="cugdt",  # 这里是pip项目发布的名称
-    version="1.0.4",  # 版本号，数值大的会优先被pip
+    version="1.0.5",  # 版本号，数值大的会优先被pip
     keywords=["pip", "tiff", "cugdt"],  # 关键字
     description="Tiff文件读取，写入，压缩",  # 描述
     license="MIT Licence",  # 许可证
 
     url="https://gitee.com/HaixuHe/cugdt",  # 项目相关文件地址，一般是github项目地址即可
     author="HaixuHe",  # 作者
     author_email="20161001925@cug.edu.cn",
```

