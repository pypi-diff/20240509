# Comparing `tmp/proc_plot-1.7.tar.gz` & `tmp/proc_plot-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proc_plot-1.7.tar", last modified: Fri Dec 22 03:43:59 2023, max compression
+gzip compressed data, was "proc_plot-1.8.tar", last modified: Thu May  9 02:00:01 2024, max compression
```

## Comparing `proc_plot-1.7.tar` & `proc_plot-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-12-22 03:43:59.142910 proc_plot-1.7/
--rw-rw-rw-   0        0        0    35823 2020-04-10 20:44:32.000000 proc_plot-1.7/LICENSE
--rw-rw-rw-   0        0        0       52 2020-04-24 22:58:58.000000 proc_plot-1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2865 2023-12-22 03:43:59.142910 proc_plot-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1965 2022-04-30 03:58:33.000000 proc_plot-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-12-22 03:43:59.080176 proc_plot-1.7/proc_plot/
--rw-rw-rw-   0        0        0      787 2022-04-30 03:05:19.000000 proc_plot-1.7/proc_plot/__init__.py
--rw-rw-rw-   0        0        0    33462 2023-12-22 03:38:34.000000 proc_plot-1.7/proc_plot/pp.py
-drwxrwxrwx   0        0        0        0 2023-12-22 03:43:59.142910 proc_plot-1.7/proc_plot.egg-info/
--rw-rw-rw-   0        0        0     2865 2023-12-22 03:43:58.000000 proc_plot-1.7/proc_plot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-12-22 03:43:58.000000 proc_plot-1.7/proc_plot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-22 03:43:58.000000 proc_plot-1.7/proc_plot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-12-22 03:43:58.000000 proc_plot-1.7/proc_plot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-22 03:43:58.000000 proc_plot-1.7/proc_plot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-12-22 03:43:59.146680 proc_plot-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1444 2023-12-22 03:43:03.000000 proc_plot-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:00:01.587078 proc_plot-1.8/
+-rw-rw-rw-   0        0        0    35823 2020-04-10 20:44:32.000000 proc_plot-1.8/LICENSE
+-rw-rw-rw-   0        0        0       52 2020-04-24 22:58:58.000000 proc_plot-1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2865 2024-05-09 02:00:01.587078 proc_plot-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1965 2022-04-30 03:58:33.000000 proc_plot-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:00:01.573297 proc_plot-1.8/proc_plot/
+-rw-rw-rw-   0        0        0      787 2022-04-30 03:05:19.000000 proc_plot-1.8/proc_plot/__init__.py
+-rw-rw-rw-   0        0        0    33682 2024-05-09 01:54:27.000000 proc_plot-1.8/proc_plot/pp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:00:01.587078 proc_plot-1.8/proc_plot.egg-info/
+-rw-rw-rw-   0        0        0     2865 2024-05-09 02:00:01.000000 proc_plot-1.8/proc_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-09 02:00:01.000000 proc_plot-1.8/proc_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:00:01.000000 proc_plot-1.8/proc_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-09 02:00:01.000000 proc_plot-1.8/proc_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 02:00:01.000000 proc_plot-1.8/proc_plot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-09 02:00:01.599970 proc_plot-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2024-05-09 01:57:33.000000 proc_plot-1.8/setup.py
```

### Comparing `proc_plot-1.7/LICENSE` & `proc_plot-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proc_plot-1.7/PKG-INFO` & `proc_plot-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: proc_plot
-Version: 1.7
+Version: 1.8
 Summary: Trending for Process Control Data Analysis
 Home-page: https://github.com/fpieterse/proc_plot
-Download-URL: https://github.com/fpieterse/proc_plot/archive/v1.7.tar.gz
+Download-URL: https://github.com/fpieterse/proc_plot/archive/v1.8.tar.gz
 Author: Francois Pieterse
 Author-email: francois.pieterse@greenferndynamics.com
 License: GPLv3
 Keywords: Trend,Process Control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `proc_plot-1.7/README.md` & `proc_plot-1.8/README.md`

 * *Files identical despite different names*

### Comparing `proc_plot-1.7/proc_plot/__init__.py` & `proc_plot-1.8/proc_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `proc_plot-1.7/proc_plot/pp.py` & `proc_plot-1.8/proc_plot/pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,25 @@
             print('PlotManager::home_clicked()')
 
         try:
             #plt.margins(0,0.05)
             if len(self._plotinfo) > 0:
                 for pi in self._plotinfo:
                     pi.ax.autoscale(axis='x',tight=True)
-                    pi.ax.autoscale(axis='y',tight=False)
+
+                    # Autoscale on y doesn't work.  I think the cursor is making
+                    # trouble.  Just scale it manually.
+                    #pi.ax.autoscale(axis='y',tight=False)
+                    ymin = float( self._df[ pi.tagnames ].min().min() )
+                    ymax = float( self._df[ pi.tagnames ].max().max() )
+                    margin = 0.05*(ymax-ymin)
+                    if margin <= 0:
+                        margin = 0.01
+                        
+                    pi.ax.set_ylim( ymin-margin,ymax+margin)
             self.plot_window.canvas.draw()
 
         except Exception as e:
             sys.stderr.write(str(e))
 
     @QtCore.pyqtSlot()
     def clear_all_plots(self):
@@ -314,31 +324,35 @@
 
             # Only plot new tag so that zoom doesn't change
             if DEBUG:
                 print("Adding tag to axis")
 
             #xlim = plotinfo.ax.get_xlim()
 
+            # Get current y-lim before plotting:
+            ylim_before = plotinfo.ax.get_ylim()
+
             plotinfo.ax.plot(
                 self._df[tag],
                 color=taginfo.color,
                 label=tag,
                 scalex=False,
             )
             plotinfo.ax.legend(loc=self.legend_loc,
                                fontsize=self.legend_fontsize)
-            '''
-            self._df[tag].plot(color=taginfo.color,
-                               ax=plotinfo.ax,
-                               legend=True,
-                               include_bool=True)
-            '''
 
             #plotinfo.ax.set_xlim(xlim)
 
+            # Set the y-lim to accommodate newly plotted value
+            margin = 0.05*(ylim_before[1] - ylim_before[0])
+            ymin = float( min(ylim_before[0], self._df[ tag ].min()-margin) )
+            ymax = float( max(ylim_before[1], self._df[ tag ].max()+margin) )
+                
+            plotinfo.ax.set_ylim( ymin,ymax)
+
         else:
             nplots = len(self._plotinfo)
 
             # make a new trend
             if nplots > 0:
                 sharex = self._plotinfo[0].ax
             else:
@@ -1035,60 +1049,46 @@
 
 def show():
     '''
     Show the plot window.
     '''
     global main_window
     global _isInit
-    global _execApp
 
     if not _isInit:
         sys.stderr.write('Dataframe is not initialised, use set_dataframe to'
                         +' initialise dataframe\n')
         return
 
     main_window.show()
 
     if DEBUG:
         print("Showing main window")
 
-    if _execApp:
-        app.exec_()
-        app.exit()
+    if DEBUG:
+        print("Backend: ", plt.get_backend())
+        print("Interactive: ", plt.isinteractive())
 
-def set_exec_on_show(on=True):
-    '''
-    Set whether Qt app .exec function should be called on show().  When
-    proc_plot is used in a jupyter notebook with %matplotlib qt magic then the
-    gui loop is already running and starting it again will break the app.
-    proc_plot tries to figure it out automatically but you can override the
-    setting with this function.
+    # For Qt backends, the GUI loop is already running, don't call app.exec()
+    if ( (plt.get_backend().lower() in ['qt5agg','qtagg'] ) and
+        plt.isinteractive() ):
+        # Do Nothing
+        pass
+    else:
+        app.exec_()
+        # app.exit() is useful if you want to be able to continue to execute
+        # other code cells in a jupyter notebook.  It however breaks the
+        # notebook the next time you switch to a qt backend.  So don't do it
+        #app.exit()
 
-    Parameters:
-    -----------
-    on : bool, optional
-        set to False to disable runnnig app.exec.
 
-    '''
-    global _execApp
-    _execApp = on
 
 _isInit = False # has the window been initialised with a dataframe?
-_execApp = True # if started with qt, gui loop is running
 
-if DEBUG:
-    print("Backend: ", plt.get_backend())
 
-if (plt.get_backend().lower() == 'qt5agg' and
-    plt.isinteractive() ):
-    # looks like you are running a jupyter notebook with %matplotlib qt
-    _execApp = False
-    print("It looks like you are running a jupyter notebook with " \
-         +"%matplotlib qt magic.\nThe gui loop is disabled, if you " \
-         +"want to enable it, use proc_plot.set_exec_on_show()")
 
 app = QtCore.QCoreApplication.instance()
 if app is None:
     app = QApplication([])
     if DEBUG:
         print("app was None")
```

### Comparing `proc_plot-1.7/proc_plot.egg-info/PKG-INFO` & `proc_plot-1.8/proc_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: proc-plot
-Version: 1.7
+Version: 1.8
 Summary: Trending for Process Control Data Analysis
 Home-page: https://github.com/fpieterse/proc_plot
-Download-URL: https://github.com/fpieterse/proc_plot/archive/v1.7.tar.gz
+Download-URL: https://github.com/fpieterse/proc_plot/archive/v1.8.tar.gz
 Author: Francois Pieterse
 Author-email: francois.pieterse@greenferndynamics.com
 License: GPLv3
 Keywords: Trend,Process Control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `proc_plot-1.7/setup.py` & `proc_plot-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-__version__ = '1.7'
+__version__ = '1.8'
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description=f.read()
```

