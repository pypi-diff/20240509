# Comparing `tmp/reviutils-1.4.0b2.tar.gz` & `tmp/reviutils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviutils-1.4.0b2.tar", last modified: Wed Apr 17 07:11:22 2024, max compression
+gzip compressed data, was "reviutils-1.4.1.tar", last modified: Thu May  9 08:47:27 2024, max compression
```

## Comparing `reviutils-1.4.0b2.tar` & `reviutils-1.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.893143 reviutils-1.4.0b2/
--rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0b2/LICENSE
--rw-rw-rw-   0        0        0     2942 2024-04-17 07:11:22.893143 reviutils-1.4.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2024-04-17 02:27:29.000000 reviutils-1.4.0b2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.852265 reviutils-1.4.0b2/reviutils/
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.865168 reviutils-1.4.0b2/reviutils/api/
--rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0b2/reviutils/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.868167 reviutils-1.4.0b2/reviutils/api/amap/
--rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0b2/reviutils/api/amap/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0b2/reviutils/api/amap/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.871194 reviutils-1.4.0b2/reviutils/audio/
--rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0b2/reviutils/audio/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0b2/reviutils/audio/clipper.py
--rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0b2/reviutils/audio/reader.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.873295 reviutils-1.4.0b2/reviutils/common/
--rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0b2/reviutils/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.877293 reviutils-1.4.0b2/reviutils/gis/
--rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0b2/reviutils/gis/__init__.py
--rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0b2/reviutils/gis/convertor.py
--rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0b2/reviutils/gis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.884635 reviutils-1.4.0b2/reviutils/noisepollution/
--rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0b2/reviutils/noisepollution/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0b2/reviutils/noisepollution/evaluation.py
--rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0b2/reviutils/noisepollution/funcarea.py
--rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0b2/reviutils/noisepollution/hourhelper.py
--rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0b2/reviutils/noisepollution/splhelper.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.887638 reviutils-1.4.0b2/reviutils/omap/
--rw-rw-rw-   0        0        0      767 2024-04-17 07:11:03.000000 reviutils-1.4.0b2/reviutils/omap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.888639 reviutils-1.4.0b2/reviutils/omap/constants/
--rw-rw-rw-   0        0        0     3751 2024-04-17 03:20:28.000000 reviutils-1.4.0b2/reviutils/omap/constants/__init__.py
--rw-rw-rw-   0        0        0     1906 2024-04-17 07:05:36.000000 reviutils-1.4.0b2/reviutils/omap/demo.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.892138 reviutils-1.4.0b2/reviutils/omap/samples/
--rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.0b2/reviutils/omap/samples/Base.py
--rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.0b2/reviutils/omap/samples/__init__.py
--rw-rw-rw-   0        0        0    12837 2024-04-17 07:04:25.000000 reviutils-1.4.0b2/reviutils/omap/samples/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:11:22.864163 reviutils-1.4.0b2/reviutils.egg-info/
--rw-rw-rw-   0        0        0     2942 2024-04-17 07:11:22.000000 reviutils-1.4.0b2/reviutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      866 2024-04-17 07:11:22.000000 reviutils-1.4.0b2/reviutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 07:11:22.000000 reviutils-1.4.0b2/reviutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 07:11:22.000000 reviutils-1.4.0b2/reviutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2024-04-17 07:11:22.000000 reviutils-1.4.0b2/reviutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 07:11:22.000000 reviutils-1.4.0b2/reviutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 07:11:22.894144 reviutils-1.4.0b2/setup.cfg
--rw-rw-rw-   0        0        0     2371 2024-04-17 07:11:19.000000 reviutils-1.4.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.620639 reviutils-1.4.1/
+-rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2940 2024-05-09 08:47:27.620639 reviutils-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2024-04-17 02:27:29.000000 reviutils-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.578548 reviutils-1.4.1/reviutils/
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.593107 reviutils-1.4.1/reviutils/api/
+-rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.1/reviutils/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.595617 reviutils-1.4.1/reviutils/api/amap/
+-rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.1/reviutils/api/amap/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.1/reviutils/api/amap/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.598616 reviutils-1.4.1/reviutils/audio/
+-rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.1/reviutils/audio/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.1/reviutils/audio/clipper.py
+-rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.1/reviutils/audio/reader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.600616 reviutils-1.4.1/reviutils/common/
+-rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.1/reviutils/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.605126 reviutils-1.4.1/reviutils/gis/
+-rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.1/reviutils/gis/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.1/reviutils/gis/convertor.py
+-rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.1/reviutils/gis/main.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.611130 reviutils-1.4.1/reviutils/noisepollution/
+-rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.1/reviutils/noisepollution/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.1/reviutils/noisepollution/evaluation.py
+-rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.1/reviutils/noisepollution/funcarea.py
+-rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.1/reviutils/noisepollution/hourhelper.py
+-rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.1/reviutils/noisepollution/splhelper.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.613130 reviutils-1.4.1/reviutils/omap/
+-rw-rw-rw-   0        0        0      872 2024-04-17 07:16:30.000000 reviutils-1.4.1/reviutils/omap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.614633 reviutils-1.4.1/reviutils/omap/constants/
+-rw-rw-rw-   0        0        0     4414 2024-05-09 07:42:00.000000 reviutils-1.4.1/reviutils/omap/constants/__init__.py
+-rw-rw-rw-   0        0        0     3289 2024-05-09 07:54:01.000000 reviutils-1.4.1/reviutils/omap/demo.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.618656 reviutils-1.4.1/reviutils/omap/samples/
+-rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.1/reviutils/omap/samples/Base.py
+-rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.1/reviutils/omap/samples/__init__.py
+-rw-rw-rw-   0        0        0    17006 2024-05-09 07:56:54.000000 reviutils-1.4.1/reviutils/omap/samples/main.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:47:27.592108 reviutils-1.4.1/reviutils.egg-info/
+-rw-rw-rw-   0        0        0     2940 2024-05-09 08:47:27.000000 reviutils-1.4.1/reviutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2024-05-09 08:47:27.000000 reviutils-1.4.1/reviutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 08:47:27.000000 reviutils-1.4.1/reviutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 08:47:27.000000 reviutils-1.4.1/reviutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-05-09 08:47:27.000000 reviutils-1.4.1/reviutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 08:47:27.000000 reviutils-1.4.1/reviutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 08:47:27.620639 reviutils-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2369 2024-05-09 08:47:16.000000 reviutils-1.4.1/setup.py
```

### Comparing `reviutils-1.4.0b2/LICENSE` & `reviutils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/PKG-INFO` & `reviutils-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0b2
+Version: 1.4.1
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0b2 Summary: A common
-library frequently used on python Home-page: https://github.com/Viyyy/viutils
-Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.1 Summary: A common library
+frequently used on python Home-page: https://github.com/Viyyy/viutils Author:
+Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_g_i_t_h_u_b_-_r_e_v_i_u_t_i_l_s_-_r_e_d_?_l_o_g_o_=_g_i_t_h_u_b_]Â Â  _[_h_t_t_p_s_:_/_/
       _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_a_s_t_a_p_i_-_d_e_m_o_-_g_r_e_e_n_?_l_o_g_o_=_f_a_s_t_a_p_i_]Â Â  _[_h_t_t_p_s_:_/_/
```

### Comparing `reviutils-1.4.0b2/README.md` & `reviutils-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/api/amap/__init__.py` & `reviutils-1.4.1/reviutils/api/amap/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/audio/clipper.py` & `reviutils-1.4.1/reviutils/audio/clipper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/audio/reader.py` & `reviutils-1.4.1/reviutils/audio/reader.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/common/__init__.py` & `reviutils-1.4.1/reviutils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/gis/convertor.py` & `reviutils-1.4.1/reviutils/gis/convertor.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/gis/main.py` & `reviutils-1.4.1/reviutils/gis/main.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/noisepollution/evaluation.py` & `reviutils-1.4.1/reviutils/noisepollution/evaluation.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/noisepollution/funcarea.py` & `reviutils-1.4.1/reviutils/noisepollution/funcarea.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/noisepollution/hourhelper.py` & `reviutils-1.4.1/reviutils/noisepollution/hourhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/noisepollution/splhelper.py` & `reviutils-1.4.1/reviutils/noisepollution/splhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/omap/__init__.py` & `reviutils-1.4.1/reviutils/omap/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from .samples import *
 import json
 
 class ItemManager:
-    def __init__(self):
-        self.items:list[ItemBase] = []
+    def __init__(self, items:list[ItemBase]=None):
+        if items is None:
+            self.items:list[ItemBase] = []
+        else:
+            self.items = items
         
     def add_item(self, item:ItemBase):
         self.items.append(item)
         
     def __len__(self):
         return len(self.items)
```

### Comparing `reviutils-1.4.0b2/reviutils/omap/constants/__init__.py` & `reviutils-1.4.1/reviutils/omap/constants/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -116,8 +116,19 @@
     
 class PolylineTypes(EnumBase):
     Polyline = PolylineType(name="折线", id=8, Mtp=2, ShowType=5, length_min=2, length_max=9999)
     Arc = PolylineType(name="圆弧", id=8, Mtp=3, ShowType=7, length_min=3, length_max=3)
     Ellipse = PolylineType(name="椭圆", id=8, Mtp=3, ShowType=9, length_min=3, length_max=3)
     Circle = PolylineType(name="圆", id=8, Mtp=2, ShowType=7, length_min=2, length_max=2)
     
+class PolygonType(ConstantsBase):
+    start_angle: int = Field(description="起始角度")
+    end_angle: int = Field(description="终止角度")
+    
+    length_min: int = Field(description="至少需要的坐标数")
+    length_max: int = Field(description="最多允许的坐标数")
+    
+class PolygonTypes(EnumBase):
+    Polygon = PolygonType(name="多边形", id=13, start_angle=180, end_angle=180, length_min=3, length_max=9999)
+    Rectangle = PolygonType(name="矩形", id=13, start_angle=180, end_angle=180, length_min=2, length_max=2)
+    Ellipse = PolygonType(name="椭圆", id=13, start_angle=0, end_angle=360, length_min=2, length_max=2)
 # endregion
```

### Comparing `reviutils-1.4.0b2/reviutils/omap/demo.py` & `reviutils-1.4.1/reviutils/omap/demo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .samples import Point, Polyline, Text, MarkerTypes, PolylineTypes, Colors
+from .samples import Point, Polyline, Text, MarkerTypes, PolylineTypes, Colors, Polygon, PolygonTypes
 
 def create_point_obj(name: str, lng: float, lat: float, is_gcj02: bool):
     style = {"marker_type": MarkerTypes.OvalNailRed}
     return Point(
         name=name,
         lng=lng,
         lat=lat,
@@ -64,8 +64,62 @@
         is_gcj02=is_gcj02,
         lng=lng,
         lat=lat,
         font_size=font_size,
         rotation=rotation,
         **styles_dict[building_type],
     )
-    return text
+    return text
+
+def create_rectange_obj(name: str, latlng:list[float], is_gcj02: bool):
+    assert len(latlng) == 4
+    style = {
+        "polygon_type": PolygonTypes.Rectangle,
+        "line_width": 3,
+        "line_alpha": 40,
+        "line_color": Colors.Yellow,
+        "area_color":Colors.Green,
+        "area_alpha": 10,
+    }
+    
+    return Polygon(
+        name=name,
+        latlng=latlng,
+        is_gcj02=is_gcj02,
+        **style,
+    )
+    
+def create_polygon_obj(name: str, latlng:list[float], is_gcj02: bool):
+    assert len(latlng) >= 6
+    style = {
+        "polygon_type": PolygonTypes.Polygon,
+        "line_width": 3,
+        "line_alpha": 40,
+        "line_color": Colors.Yellow,
+        "area_color":Colors.Pink,
+        "area_alpha": 10,
+    }
+    
+    return Polygon(
+        name=name,
+        latlng=latlng,
+        is_gcj02=is_gcj02,
+        **style,
+    )
+    
+def create_ellipse_obj(name: str, latlng:list[float], is_gcj02: bool):
+    assert len(latlng) == 4
+    style = {
+        "polygon_type": PolygonTypes.Ellipse,
+        "line_width": 3,
+        "line_alpha": 40,
+        "line_color": Colors.Yellow,
+        "area_color":Colors.Green,
+        "area_alpha": 10,
+    }
+    
+    return Polygon(
+        name=name,
+        latlng=latlng,
+        is_gcj02=is_gcj02,
+        **style,
+    )
```

### Comparing `reviutils-1.4.0b2/reviutils/omap/samples/Base.py` & `reviutils-1.4.1/reviutils/omap/samples/Base.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/reviutils/omap/samples/main.py` & `reviutils-1.4.1/reviutils/omap/samples/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .Base import ObjectTypes
 from .Base import DetailBase
 from .Base import ObjectBase
 from .Base import ItemBase
 from ..constants import MarkerTypes
 from ..constants import Colors
 from ..constants import PolylineTypes
+from ..constants import PolygonTypes
 
 from pydantic import Field, BaseModel
 from typing import List, Union
 import datetime
 
 
 def obj_to_json(obj):
@@ -24,20 +25,94 @@
                 else:
                     result[k].append(item)
         else:
             result[k] = v
     return result
 
 
-class PolygonDetail(BaseModel):
-    pass
-
-
+class PolygonDetail(DetailBase):
+    '''
+    "ObjectDetail":
+    {"Gcj02":0,"OverlayIdx":0,"ShowLevel":1,"ShowLevelMax":0,"OuterRgnIdx":0,"EditMode":1,"ShowFlag":0,"LineClr":65535,"LineWidth":1,"CadLineShowWid":0,"LineAlpha":50,"AreaClr":65535,"AreaAlpha":50,"StartAngle":0.00000000,"EndAngle":360.00000000,"FillType":0,"FillSubType":0,"FillPattern":0,"FillChgClr":0,"FillRotate":0.00000000,"FillScale":0.00000000,"FillOffsetX":0.00000000,"FillOffsetY":0.00000000,"Mtp":2,"Latlng":[23.24304351,109.16585804,23.23694565,109.17243418]
+    }
+    '''
+    Mtp: int = Field(description="Mtp of the polygon")
+    Latlng: List[float] = Field(description="List of latitude and longitude of the polygon")
+    LineClr: int = Field(default=65535, description="Line color of the polygon")
+    LineWidth: int = Field(default=1, description="Line width of the polygon")
+    
+    AreaClr: int = Field(default=65535, description="Area color of the polygon")
+    Gcj02: int = Field(description="Whether the coordinates are in GCJ02")
+    
+    LineAlpha: int = Field(default=50, description="Line alpha of the polygon")
+    
+    AreaAlpha: int = Field(default=50, description="Area alpha of the polygon")
+    
+    # 决定形状的值
+    StartAngle: float = Field(description="Start angle of the polygon")
+    EndAngle: float = Field(description="End angle of the polygon")
+    
+    OverlayIdx: int = Field(default=0, description="Overlay index of the polygon")
+    OuterRgnIdx: int = Field(default=0, description="Outer region index of the polygon")
+    EditMode: int = Field(default=1, description="Edit mode of the polygon")
+    ShowFlag: int = Field(default=0, description="Show flag of the polygon")
+    CadLineShowWid: int = Field(default=0, description="Cad line show width of the polygon")
+
+    FillType: int = Field(default=0, description="Fill type of the polygon")
+    FillSubType: int = Field(default=0, description="Fill sub type of the polygon")
+    FillPattern: int = Field(default=0, description="Fill pattern of the polygon")
+    FillChgClr: int = Field(default=0, description="Fill change color of the polygon")
+    FillRotate: float = Field(default=0.0, description="Fill rotate of the polygon")
+    FillScale: float = Field(default=0.0, description="Fill scale of the polygon")
+    FillOffsetX: float = Field(default=0.0, description="Fill offset x of the polygon")
+    FillOffsetY: float = Field(default=0.0, description="Fill offset y of the polygon")
+
+class PolygonObject(ObjectBase):
+    def __init__(self, name, detail:PolygonDetail,comment=""):
+        super().__init__(name=name, obj_detail=detail, type_id=ObjectTypes.Polygon.value.id)
+        self.Comment = comment
+        
 class Polygon(ItemBase):
-    pass
+    def __init__(
+        self,
+        name: str,
+        polygon_type: PolygonTypes,
+        latlng: List[float],
+        is_gcj02: bool,
+        line_color: Union[Colors,int] = Colors.Default,
+        line_width: int = 1,
+        line_alpha: int = 0,
+        area_color: Union[Colors,int] = Colors.Default,
+        area_alpha: int = 0,
+        edit: bool = True,
+        parent_id: int = 1,
+    ):
+        # 检查坐标数量是否符合要求
+        if len(latlng) % 2 != 0:
+            raise ValueError("Polygon coordinates should be even number")
+        assert len(latlng)>=polygon_type.value.length_min*2 and len(latlng)<=polygon_type.value.length_max*2, f"Polygon coordinates should be between {polygon_type.value.length_min*2} and {polygon_type.value.length_max*2}"
+        detail = PolygonDetail(
+            Mtp=len(latlng)//2,
+            Latlng=latlng,
+            StartAngle=polygon_type.value.start_angle,
+            EndAngle=polygon_type.value.end_angle,
+            LineClr=line_color.value.id,
+            LineWidth=line_width,
+            AreaClr=area_color.value.id,
+            Gcj02=is_gcj02,
+            LineAlpha=line_alpha,
+            AreaAlpha=area_alpha,
+            EditMode=int(edit),
+        )
+        obj = PolygonObject(name=name, detail=detail)
+        super().__init__(
+            obj=obj,
+            parent_id=parent_id,
+            type_id=ObjectTypes.Polygon.value.id,
+        )
 
 
 class TrackDrawObject(BaseModel):
     ShowType: int = Field(description="Show type of the track draw object")
     LineClr: int = Field(description="Line color of the track draw object")
     LineWidth: int = Field(description="Line width of the track draw object", gt=0)
     LineAlpha: int = Field(
```

### Comparing `reviutils-1.4.0b2/reviutils.egg-info/PKG-INFO` & `reviutils-1.4.1/reviutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0b2
+Version: 1.4.1
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0b2 Summary: A common
-library frequently used on python Home-page: https://github.com/Viyyy/viutils
-Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.1 Summary: A common library
+frequently used on python Home-page: https://github.com/Viyyy/viutils Author:
+Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_g_i_t_h_u_b_-_r_e_v_i_u_t_i_l_s_-_r_e_d_?_l_o_g_o_=_g_i_t_h_u_b_]Â Â  _[_h_t_t_p_s_:_/_/
       _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_a_s_t_a_p_i_-_d_e_m_o_-_g_r_e_e_n_?_l_o_g_o_=_f_a_s_t_a_p_i_]Â Â  _[_h_t_t_p_s_:_/_/
```

### Comparing `reviutils-1.4.0b2/reviutils.egg-info/SOURCES.txt` & `reviutils-1.4.1/reviutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0b2/setup.py` & `reviutils-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import os, shutil
 from setuptools import setup
 
 
 name = "reviutils"
-version = "1.4.0b2"
+version = "1.4.1"
 packages = [
     "reviutils.common",
     "reviutils.noisepollution",
     "reviutils.audio",
     "reviutils.api",
     "reviutils.api.amap",
     "reviutils.gis",
```

