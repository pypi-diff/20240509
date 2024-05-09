# Comparing `tmp/bezier-interpolation-0.0.1.tar.gz` & `tmp/bezier-interpolation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bezier-interpolation-0.0.1.tar", last modified: Mon Apr 29 22:08:41 2024, max compression
+gzip compressed data, was "bezier-interpolation-0.0.2.tar", last modified: Thu May  9 02:12:53 2024, max compression
```

## Comparing `bezier-interpolation-0.0.1.tar` & `bezier-interpolation-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:08:41.888492 bezier-interpolation-0.0.1/
--rw-rw-rw-   0        0        0     5019 2024-04-29 22:08:41.887326 bezier-interpolation-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4601 2024-04-29 22:07:29.000000 bezier-interpolation-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 22:08:41.867736 bezier-interpolation-0.0.1/bezier_interpolation/
--rw-rw-rw-   0        0        0      114 2024-04-29 18:30:06.000000 bezier-interpolation-0.0.1/bezier_interpolation/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-04-29 19:30:39.000000 bezier-interpolation-0.0.1/bezier_interpolation/cubic_interpolation.py
--rw-rw-rw-   0        0        0     2029 2024-04-29 19:29:21.000000 bezier-interpolation-0.0.1/bezier_interpolation/quadratic_interpolation.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:08:41.883336 bezier-interpolation-0.0.1/bezier_interpolation.egg-info/
--rw-rw-rw-   0        0        0     5019 2024-04-29 22:08:41.000000 bezier-interpolation-0.0.1/bezier_interpolation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-04-29 22:08:41.000000 bezier-interpolation-0.0.1/bezier_interpolation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:08:41.000000 bezier-interpolation-0.0.1/bezier_interpolation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-29 22:08:41.000000 bezier-interpolation-0.0.1/bezier_interpolation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-29 22:08:41.000000 bezier-interpolation-0.0.1/bezier_interpolation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 22:08:41.889477 bezier-interpolation-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-04-29 22:08:31.000000 bezier-interpolation-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:12:53.894463 bezier-interpolation-0.0.2/
+-rw-rw-rw-   0        0        0     7353 2024-05-09 02:12:53.892439 bezier-interpolation-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6935 2024-05-09 02:09:40.000000 bezier-interpolation-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:12:53.816558 bezier-interpolation-0.0.2/bezier_interpolation/
+-rw-rw-rw-   0        0        0      114 2024-04-29 18:30:06.000000 bezier-interpolation-0.0.2/bezier_interpolation/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-04-29 19:30:39.000000 bezier-interpolation-0.0.2/bezier_interpolation/cubic_interpolation.py
+-rw-rw-rw-   0        0        0     2029 2024-04-29 19:29:21.000000 bezier-interpolation-0.0.2/bezier_interpolation/quadratic_interpolation.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:12:53.886457 bezier-interpolation-0.0.2/bezier_interpolation.egg-info/
+-rw-rw-rw-   0        0        0     7353 2024-05-09 02:12:53.000000 bezier-interpolation-0.0.2/bezier_interpolation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-05-09 02:12:53.000000 bezier-interpolation-0.0.2/bezier_interpolation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:12:53.000000 bezier-interpolation-0.0.2/bezier_interpolation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-09 02:12:53.000000 bezier-interpolation-0.0.2/bezier_interpolation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-09 02:12:53.000000 bezier-interpolation-0.0.2/bezier_interpolation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:12:53.895432 bezier-interpolation-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-09 02:12:47.000000 bezier-interpolation-0.0.2/setup.py
```

### Comparing `bezier-interpolation-0.0.1/PKG-INFO` & `bezier-interpolation-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bezier-interpolation
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for generating smooth curves between given points using cubic and quadratic Bezier interpolation.
 Home-page: https://github.com/balexandermunoz/bezier-interpolation
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -20,14 +20,31 @@
 
 ## Installation instructions
 
 ```sh
 pip install bezier_interpolation
 ```
 
+## Usage
+```python
+from bezier_interpolation import cubic_interpolation, quadratic_interpolation
+
+c_data = {"x": [1, 2, 3], "y": [-1, -5, 3]}
+c_data = list(zip(c_data["x"], c_data["y"]))
+c_interpolated_data = cubic_interpolation(c_data)
+print(c_interpolated_data)
+# Returns: [[1, -1], [1.3, -3.3], [1.6 -5.6], [2, -5], [2.3, -4.3], [2.6, -0.6], [3, 3]]
+
+q_data = [(1, 1), (2, 4), (3, 9)]
+q_interpolated_data = quadratic_interpolation(q_data)
+print(q_interpolated_data)
+# Returns:  [[1, 1], [1.5, 2.5], [2, 4], [2.5, 5.5], [3, 9]]
+
+```
+
 ## Math explanation: 
 
 ### Cubic segments:
 Let's say we have this 3 green points $P_{0,0}$, $P_{3,0} = P_{0,1}$ and $P_{3,1}$ and we want to have a smooth curve between them.   
 ![Cubic Bezier Interpolation](https://github.com/balexandermunoz/bezier-interpolation/blob/master/bezier-interpolation.png?raw=true)
 
 We need to find where to set the control points $P_{1,0}$, $P_{2,0}$, $P_{1,1}$ and $P_{2,1}$.   
@@ -119,20 +136,20 @@
 0 & 0 & \cdots & 0 & 2 & 7
 \end{bmatrix}
 $$
 
 x is this vector:
 $$
 \begin{bmatrix}
-P_{1,1}  \\
-P_{1,2}  \\
-P_{1,3}  \\
-\vdots  \\
-P_{1,n-2}  \\
-P_{1, n-1} 
+P_{1,1} \\
+P_{1,2} \\
+P_{1,3} \\
+\vdots \\
+P_{1,n-2} \\
+P_{1, n-1}
 \end{bmatrix}
 $$
 
 and b this one: 
 $$
 \begin{bmatrix}
 K_{0} + 2K_1  \\
@@ -146,14 +163,43 @@
 
 and if we solve this system, we can get $P_{2}$ with:
 
 $$P_{2, i} = 2K_i + P_{1,i}$$
 and 
 $$P_{2, n-1} = (1/2)(K_n + P_{1,n-1})$$
 
-### Quadratic segments:
- TODO
+### Quadratic segments. Geometrical approach:
+We could follow a process similar to the one we did above, but this one would be straightforward and it will have no dependency with t. We want to control the start angle, so let's try a geomterical approach.    
+Let's suppose we now want just one control point between two data points, so we have something like this 
+![Quadratic Bezier Interpolation](https://github.com/balexandermunoz/bezier-interpolation/blob/master/bezier-interpolation2.png?raw=true)
+Did you notice that now we need points $P_{1,0}$ and $P_{1,1}$ in the same line?   
+In general, we need $P_{1, i}$ align for $i \in 0,1,...,n-1$ when $n$ = number of data points, and $n-1$ is the number of segments.   
+
+We are going to set the first control point in the middle of $P_{0,0}$ and $P_{0,2}$, so, we can say for the midpoint formula:
+
+$$ P_{0,1} = P_{0,0} + \frac{1}{2}(P_{0, 2} - P_{0,0}) $$
+
+If we want to add the control parameter $t$, we can control the distance and relative altitude respect the last point, so we write
+
+$$ P_{0,1} = P_{0,0} + t (P_{0, 2} - P_{0,0}) $$
+
+Now that we have the first control point, we need to compute the line between $P_{0,1}$ and $P_{0,2}$ and set the next control point in that line.  
+
+We call the line between $P_{i,1}$ and $P_{i,2}$ $L_{i}$ which is defined by the equation $Y_i = m_i  X_{i-1} + b_i$.    
+$Y_i$ is the $Y$ component of $P_{i,1}$ and  $X_{i-1}$ is the $X$ component of $P_{i-1,1}$.   
+
+So, in general, for the next $n-2$ points we can write:
+$$m_i = \frac{Y_{i, 0} - Y_{i-1, 1}}{X_{i, 0} - X_{i-1, 1}}$$
+
+$$b_i = Y_{i, 0} - m_i X_{i, 0} $$
+
+and 
+
+$$X_{i,1} = X_{i,0} + \frac{1}{2}(x_{i,2} - X_{i,0})$$   
+
+$$Y_{i,1} = m_i  X_{i,1} + b_i$$
 
+wich are the X,Y components of the desired $P_{i,1}$  point respectively. 
 ### References:
 - [Smooth Bezier Spiline Through Prescribed Points](https://www.particleincell.com/2012/bezier-splines/)   
 
 - [Drawing Smooth Cubic Bezier Curve through prescribed points](https://exploringswift.com/blog/Drawing-Smooth-Cubic-Bezier-Curve-through-prescribed-points-using-Swift)
```

### Comparing `bezier-interpolation-0.0.1/bezier_interpolation/cubic_interpolation.py` & `bezier-interpolation-0.0.2/bezier_interpolation/cubic_interpolation.py`

 * *Files identical despite different names*

### Comparing `bezier-interpolation-0.0.1/bezier_interpolation/quadratic_interpolation.py` & `bezier-interpolation-0.0.2/bezier_interpolation/quadratic_interpolation.py`

 * *Files identical despite different names*

### Comparing `bezier-interpolation-0.0.1/bezier_interpolation.egg-info/PKG-INFO` & `bezier-interpolation-0.0.2/bezier_interpolation.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bezier-interpolation
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for generating smooth curves between given points using cubic and quadratic Bezier interpolation.
 Home-page: https://github.com/balexandermunoz/bezier-interpolation
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -20,14 +20,31 @@
 
 ## Installation instructions
 
 ```sh
 pip install bezier_interpolation
 ```
 
+## Usage
+```python
+from bezier_interpolation import cubic_interpolation, quadratic_interpolation
+
+c_data = {"x": [1, 2, 3], "y": [-1, -5, 3]}
+c_data = list(zip(c_data["x"], c_data["y"]))
+c_interpolated_data = cubic_interpolation(c_data)
+print(c_interpolated_data)
+# Returns: [[1, -1], [1.3, -3.3], [1.6 -5.6], [2, -5], [2.3, -4.3], [2.6, -0.6], [3, 3]]
+
+q_data = [(1, 1), (2, 4), (3, 9)]
+q_interpolated_data = quadratic_interpolation(q_data)
+print(q_interpolated_data)
+# Returns:  [[1, 1], [1.5, 2.5], [2, 4], [2.5, 5.5], [3, 9]]
+
+```
+
 ## Math explanation: 
 
 ### Cubic segments:
 Let's say we have this 3 green points $P_{0,0}$, $P_{3,0} = P_{0,1}$ and $P_{3,1}$ and we want to have a smooth curve between them.   
 ![Cubic Bezier Interpolation](https://github.com/balexandermunoz/bezier-interpolation/blob/master/bezier-interpolation.png?raw=true)
 
 We need to find where to set the control points $P_{1,0}$, $P_{2,0}$, $P_{1,1}$ and $P_{2,1}$.   
@@ -119,20 +136,20 @@
 0 & 0 & \cdots & 0 & 2 & 7
 \end{bmatrix}
 $$
 
 x is this vector:
 $$
 \begin{bmatrix}
-P_{1,1}  \\
-P_{1,2}  \\
-P_{1,3}  \\
-\vdots  \\
-P_{1,n-2}  \\
-P_{1, n-1} 
+P_{1,1} \\
+P_{1,2} \\
+P_{1,3} \\
+\vdots \\
+P_{1,n-2} \\
+P_{1, n-1}
 \end{bmatrix}
 $$
 
 and b this one: 
 $$
 \begin{bmatrix}
 K_{0} + 2K_1  \\
@@ -146,14 +163,43 @@
 
 and if we solve this system, we can get $P_{2}$ with:
 
 $$P_{2, i} = 2K_i + P_{1,i}$$
 and 
 $$P_{2, n-1} = (1/2)(K_n + P_{1,n-1})$$
 
-### Quadratic segments:
- TODO
+### Quadratic segments. Geometrical approach:
+We could follow a process similar to the one we did above, but this one would be straightforward and it will have no dependency with t. We want to control the start angle, so let's try a geomterical approach.    
+Let's suppose we now want just one control point between two data points, so we have something like this 
+![Quadratic Bezier Interpolation](https://github.com/balexandermunoz/bezier-interpolation/blob/master/bezier-interpolation2.png?raw=true)
+Did you notice that now we need points $P_{1,0}$ and $P_{1,1}$ in the same line?   
+In general, we need $P_{1, i}$ align for $i \in 0,1,...,n-1$ when $n$ = number of data points, and $n-1$ is the number of segments.   
+
+We are going to set the first control point in the middle of $P_{0,0}$ and $P_{0,2}$, so, we can say for the midpoint formula:
+
+$$ P_{0,1} = P_{0,0} + \frac{1}{2}(P_{0, 2} - P_{0,0}) $$
+
+If we want to add the control parameter $t$, we can control the distance and relative altitude respect the last point, so we write
+
+$$ P_{0,1} = P_{0,0} + t (P_{0, 2} - P_{0,0}) $$
+
+Now that we have the first control point, we need to compute the line between $P_{0,1}$ and $P_{0,2}$ and set the next control point in that line.  
+
+We call the line between $P_{i,1}$ and $P_{i,2}$ $L_{i}$ which is defined by the equation $Y_i = m_i  X_{i-1} + b_i$.    
+$Y_i$ is the $Y$ component of $P_{i,1}$ and  $X_{i-1}$ is the $X$ component of $P_{i-1,1}$.   
+
+So, in general, for the next $n-2$ points we can write:
+$$m_i = \frac{Y_{i, 0} - Y_{i-1, 1}}{X_{i, 0} - X_{i-1, 1}}$$
+
+$$b_i = Y_{i, 0} - m_i X_{i, 0} $$
+
+and 
+
+$$X_{i,1} = X_{i,0} + \frac{1}{2}(x_{i,2} - X_{i,0})$$   
+
+$$Y_{i,1} = m_i  X_{i,1} + b_i$$
 
+wich are the X,Y components of the desired $P_{i,1}$  point respectively. 
 ### References:
 - [Smooth Bezier Spiline Through Prescribed Points](https://www.particleincell.com/2012/bezier-splines/)   
 
 - [Drawing Smooth Cubic Bezier Curve through prescribed points](https://exploringswift.com/blog/Drawing-Smooth-Cubic-Bezier-Curve-through-prescribed-points-using-Swift)
```

### Comparing `bezier-interpolation-0.0.1/setup.py` & `bezier-interpolation-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bezier-interpolation",
-    version="0.0.1",
+    version="0.0.2",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Python library for generating smooth curves between given points using cubic and quadratic Bezier interpolation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/bezier-interpolation",
     packages=setuptools.find_packages(),
```

