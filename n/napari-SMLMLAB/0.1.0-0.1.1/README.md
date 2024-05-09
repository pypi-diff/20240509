# Comparing `tmp/napari_smlmlab-0.1.0.tar.gz` & `tmp/napari_smlmlab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-mqpxpvd3\napari_smlmlab-0.1.0.tar", last modified: Wed May  8 14:34:50 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-fndmupiv\napari_smlmlab-0.1.1.tar", last modified: Thu May  9 15:51:56 2024, max compression
```

## Comparing `napari_smlmlab-0.1.0.tar` & `napari_smlmlab-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.085157 napari_smlmlab-0.1.0/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4669 2024-05-08 14:34:50.085157 napari_smlmlab-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.1.0/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1829 2024-05-08 14:34:50.089107 napari_smlmlab-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.011745 napari_smlmlab-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.082153 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4669 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2024-05-08 14:34:50.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.049198 napari_smlmlab-0.1.0/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-05-08 14:33:29.000000 napari_smlmlab-0.1.0/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.053205 napari_smlmlab-0.1.0/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.1.0/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.1.0/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0    12689 2024-05-08 14:33:46.000000 napari_smlmlab-0.1.0/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    43726 2024-05-08 13:37:00.000000 napari_smlmlab-0.1.0/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.1.0/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.079163 napari_smlmlab-0.1.0/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    29165 2024-05-08 11:10:02.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    21490 2024-05-08 11:10:02.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0    12393 2024-05-08 12:05:51.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/plot_utils.py
--rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/undrift_utils.py
--rw-rw-rw-   0        0        0     8199 2024-05-07 14:43:51.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:51:56.934281 napari_smlmlab-0.1.1/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4669 2024-05-09 15:51:56.934281 napari_smlmlab-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1829 2024-05-09 15:51:56.934281 napari_smlmlab-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 15:51:56.871792 napari_smlmlab-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 15:51:56.934281 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4669 2024-05-09 15:51:56.000000 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2024-05-09 15:51:56.000000 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:51:56.000000 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-09 15:51:56.000000 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2024-05-09 15:51:56.000000 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-09 15:51:56.000000 napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 15:51:56.903038 napari_smlmlab-0.1.1/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-05-09 15:43:28.000000 napari_smlmlab-0.1.1/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:51:56.903038 napari_smlmlab-0.1.1/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.1.1/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.1.1/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    18958 2024-05-09 15:38:24.000000 napari_smlmlab-0.1.1/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    49316 2024-05-09 15:50:16.000000 napari_smlmlab-0.1.1/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.1.1/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-09 15:51:56.934281 napari_smlmlab-0.1.1/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    29293 2024-05-09 13:57:48.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    21743 2024-05-09 13:57:52.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24954 2024-05-09 15:40:53.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0    12445 2024-05-09 08:01:41.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/plot_utils.py
+-rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/undrift_utils.py
+-rw-rw-rw-   0        0        0     8199 2024-05-07 14:43:51.000000 napari_smlmlab-0.1.1/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.1.0/LICENSE` & `napari_smlmlab-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/PKG-INFO` & `napari_smlmlab-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.1.0
+Version: 0.1.1
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.1.0/README.md` & `napari_smlmlab-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/pyproject.toml` & `napari_smlmlab-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/setup.cfg` & `napari_smlmlab-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.1.0
+Version: 0.1.1
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.1.1/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.1.1/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/gui.py` & `napari_smlmlab-0.1.1/src/smlmlab/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Frame(object):
     def setupUi(self, Frame):
         Frame.setObjectName("Frame")
-        Frame.resize(482, 710)
+        Frame.resize(542, 710)
         self.verticalLayout = QtWidgets.QVBoxLayout(Frame)
         self.verticalLayout.setObjectName("verticalLayout")
         self.tabWidget = QtWidgets.QTabWidget(Frame)
         self.tabWidget.setObjectName("tabWidget")
         self.tab = QtWidgets.QWidget()
         self.tab.setObjectName("tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.tab)
@@ -218,14 +218,90 @@
         self.undrift_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.undrift_progressbar.setProperty("value", 0)
         self.undrift_progressbar.setObjectName("undrift_progressbar")
         self.verticalLayout_9.addWidget(self.undrift_progressbar)
         spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_9.addItem(spacerItem2)
         self.tabWidget_2.addTab(self.tab_8, "")
+        self.tab_10 = QtWidgets.QWidget()
+        self.tab_10.setObjectName("tab_10")
+        self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.tab_10)
+        self.verticalLayout_11.setObjectName("verticalLayout_11")
+        self.label_36 = QtWidgets.QLabel(self.tab_10)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_36.setFont(font)
+        self.label_36.setObjectName("label_36")
+        self.verticalLayout_11.addWidget(self.label_36)
+        self.formLayout_9 = QtWidgets.QFormLayout()
+        self.formLayout_9.setObjectName("formLayout_9")
+        self.label_30 = QtWidgets.QLabel(self.tab_10)
+        self.label_30.setObjectName("label_30")
+        self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_30)
+        self.picasso_filter_dataset = QtWidgets.QComboBox(self.tab_10)
+        self.picasso_filter_dataset.setObjectName("picasso_filter_dataset")
+        self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_filter_dataset)
+        self.label_31 = QtWidgets.QLabel(self.tab_10)
+        self.label_31.setObjectName("label_31")
+        self.formLayout_9.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_31)
+        self.picasso_filter_channel = QtWidgets.QComboBox(self.tab_10)
+        self.picasso_filter_channel.setObjectName("picasso_filter_channel")
+        self.formLayout_9.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_filter_channel)
+        self.label_37 = QtWidgets.QLabel(self.tab_10)
+        self.label_37.setObjectName("label_37")
+        self.formLayout_9.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_37)
+        self.filter_criterion = QtWidgets.QComboBox(self.tab_10)
+        self.filter_criterion.setObjectName("filter_criterion")
+        self.formLayout_9.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.filter_criterion)
+        self.verticalLayout_11.addLayout(self.formLayout_9)
+        self.filter_graph_container = QtWidgets.QWidget(self.tab_10)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.filter_graph_container.sizePolicy().hasHeightForWidth())
+        self.filter_graph_container.setSizePolicy(sizePolicy)
+        self.filter_graph_container.setObjectName("filter_graph_container")
+        self.verticalLayout_11.addWidget(self.filter_graph_container)
+        self.label_38 = QtWidgets.QLabel(self.tab_10)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_38.setFont(font)
+        self.label_38.setObjectName("label_38")
+        self.verticalLayout_11.addWidget(self.label_38)
+        self.gridLayout_3 = QtWidgets.QGridLayout()
+        self.gridLayout_3.setObjectName("gridLayout_3")
+        self.formLayout_11 = QtWidgets.QFormLayout()
+        self.formLayout_11.setObjectName("formLayout_11")
+        self.label_40 = QtWidgets.QLabel(self.tab_10)
+        self.label_40.setObjectName("label_40")
+        self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_40)
+        self.filter_min = QtWidgets.QDoubleSpinBox(self.tab_10)
+        self.filter_min.setMinimum(-999999999.0)
+        self.filter_min.setMaximum(9999999999.0)
+        self.filter_min.setObjectName("filter_min")
+        self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.filter_min)
+        self.gridLayout_3.addLayout(self.formLayout_11, 0, 0, 1, 1)
+        self.formLayout_14 = QtWidgets.QFormLayout()
+        self.formLayout_14.setObjectName("formLayout_14")
+        self.label_43 = QtWidgets.QLabel(self.tab_10)
+        self.label_43.setObjectName("label_43")
+        self.formLayout_14.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_43)
+        self.filter_max = QtWidgets.QDoubleSpinBox(self.tab_10)
+        self.filter_max.setMinimum(-99999999999.0)
+        self.filter_max.setMaximum(9999999999.0)
+        self.filter_max.setObjectName("filter_max")
+        self.formLayout_14.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.filter_max)
+        self.gridLayout_3.addLayout(self.formLayout_14, 0, 1, 1, 1)
+        self.verticalLayout_11.addLayout(self.gridLayout_3)
+        self.filter_localisations = QtWidgets.QPushButton(self.tab_10)
+        self.filter_localisations.setObjectName("filter_localisations")
+        self.verticalLayout_11.addWidget(self.filter_localisations)
+        self.tabWidget_2.addTab(self.tab_10, "")
         self.tab_5 = QtWidgets.QWidget()
         self.tab_5.setObjectName("tab_5")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.tab_5)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.label_2 = QtWidgets.QLabel(self.tab_5)
         font = QtGui.QFont()
         font.setBold(True)
@@ -442,14 +518,17 @@
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.graph_container.sizePolicy().hasHeightForWidth())
         self.graph_container.setSizePolicy(sizePolicy)
         self.graph_container.setMinimumSize(QtCore.QSize(50, 0))
         self.graph_container.setToolTipDuration(0)
         self.graph_container.setObjectName("graph_container")
         self.verticalLayout_7.addWidget(self.graph_container)
+        self.export_profile_data = QtWidgets.QPushButton(self.tab_6)
+        self.export_profile_data.setObjectName("export_profile_data")
+        self.verticalLayout_7.addWidget(self.export_profile_data)
         self.tabWidget.addTab(self.tab_6, "")
         self.tab_9 = QtWidgets.QWidget()
         self.tab_9.setObjectName("tab_9")
         self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.tab_9)
         self.verticalLayout_10.setObjectName("verticalLayout_10")
         self.label_24 = QtWidgets.QLabel(self.tab_9)
         font = QtGui.QFont()
@@ -612,15 +691,24 @@
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_3), _translate("Frame", "Detect"))
         self.label_7.setText(_translate("Frame", "Detect Localisations (Picasso)"))
         self.label_19.setText(_translate("Frame", "Dataset"))
         self.label_20.setText(_translate("Frame", "Channel"))
         self.label_21.setText(_translate("Frame", "Segmentation"))
         self.picasso_undrift.setText(_translate("Frame", "Undrift Localisations"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_8), _translate("Frame", "Undrift"))
-        self.label_2.setText(_translate("Frame", "Render Fiducials (Picasso)"))
+        self.label_36.setText(_translate("Frame", "Filter Localisations (Picasso)"))
+        self.label_30.setText(_translate("Frame", "Dataset"))
+        self.label_31.setText(_translate("Frame", "Channel"))
+        self.label_37.setText(_translate("Frame", "Filter By"))
+        self.label_38.setText(_translate("Frame", "Filter Ranges"))
+        self.label_40.setText(_translate("Frame", "Min"))
+        self.label_43.setText(_translate("Frame", "Max"))
+        self.filter_localisations.setText(_translate("Frame", "Filter Localisations"))
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_10), _translate("Frame", "Filter"))
+        self.label_2.setText(_translate("Frame", "Render Localisations (Picasso)"))
         self.label_4.setText(_translate("Frame", "Dataset"))
         self.label_9.setText(_translate("Frame", "Channel"))
         self.label_10.setText(_translate("Frame", "Blur Method"))
         self.picasso_render_blur_method.setItemText(0, _translate("Frame", "None"))
         self.picasso_render_blur_method.setItemText(1, _translate("Frame", "One-Pixel-Blur"))
         self.picasso_render_blur_method.setItemText(2, _translate("Frame", "Global Localisation Precision"))
         self.picasso_render_blur_method.setItemText(3, _translate("Frame", "Individual Localisation Precision"))
@@ -628,15 +716,15 @@
         self.label_13.setText(_translate("Frame", "Min. Blur (cam. pixel)"))
         self.picasso_render.setText(_translate("Frame", "Render Localisations"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_5), _translate("Frame", "Render"))
         self.label_74.setText(_translate("Frame", "Picasso HDF5 Localisations will be exported at the Dataset import directory"))
         self.label_72.setText(_translate("Frame", "Dataset"))
         self.label_71.setText(_translate("Frame", "Channel"))
         self.export_locs.setText(_translate("Frame", "Export Localisations"))
-        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_7), _translate("Frame", "Export Localisations"))
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_7), _translate("Frame", "Export"))
         self.label_27.setText(_translate("Frame", "Localisation Visualisation Settings"))
         self.picasso_vis_size.setItemText(0, _translate("Frame", "1"))
         self.picasso_vis_size.setItemText(1, _translate("Frame", "2"))
         self.picasso_vis_size.setItemText(2, _translate("Frame", "3"))
         self.picasso_vis_size.setItemText(3, _translate("Frame", "4"))
         self.picasso_vis_size.setItemText(4, _translate("Frame", "5"))
         self.picasso_vis_size.setItemText(5, _translate("Frame", "6"))
@@ -681,14 +769,15 @@
         self.label_16.setText(_translate("Frame", "Plot Mode"))
         self.plot_mode.setItemText(0, _translate("Frame", "Line Profiles"))
         self.plot_mode.setItemText(1, _translate("Frame", "Line Profiles With Gaussian Fit"))
         self.plot_mode.setItemText(2, _translate("Frame", "Single Molecule Time Series"))
         self.label_17.setText(_translate("Frame", "Plot Dataset"))
         self.label_18.setText(_translate("Frame", "Plot Channel"))
         self.subtract_background.setText(_translate("Frame", "Subtract Background (Single Molecule Time Series)"))
+        self.export_profile_data.setText(_translate("Frame", "Export Plot Data"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Plot Profiles"))
         self.label_24.setText(_translate("Frame", "Lifetime Histogram Settings"))
         self.label_25.setText(_translate("Frame", "Dataset"))
         self.label_26.setText(_translate("Frame", "Channel"))
         self.label_29.setText(_translate("Frame", "Histogram N Bins"))
         self.label_33.setText(_translate("Frame", "Min Lifetime"))
         self.label_34.setText(_translate("Frame", "Max Lifetime"))
```

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/events_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,15 @@
                 print("Populating channel selectors")
 
             self.update_channel_selector(dataset_selector="picasso_dataset", channel_selector="picasso_channel", )
             self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel", )
             self.update_channel_selector(dataset_selector="locs_export_dataset", channel_selector="locs_export_channel")
             self.update_channel_selector(dataset_selector="picasso_undrift_dataset", channel_selector="picasso_undrift_channel")
             self.update_channel_selector(dataset_selector="lifetimes_dataset", channel_selector="lifetimes_channel")
+            self.update_channel_selector(dataset_selector="picasso_filter_dataset", channel_selector="picasso_filter_channel")
 
         except:
             print(traceback.format_exc())
 
     def update_channel_select_buttons(self):
         try:
             datast_name = self.gui.dataset_selector.currentText()
```

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,14 +442,19 @@
             self.gui.picasso_undrift_dataset.blockSignals(False)
 
             self.gui.lifetimes_dataset.blockSignals(True)
             self.gui.lifetimes_dataset.clear()
             self.gui.lifetimes_dataset.addItems(dataset_names)
             self.gui.lifetimes_dataset.blockSignals(False)
 
+            self.gui.picasso_filter_dataset.blockSignals(True)
+            self.gui.picasso_filter_dataset.clear()
+            self.gui.picasso_filter_dataset.addItems(dataset_names)
+            self.gui.picasso_filter_dataset.blockSignals(False)
+
         except:
             print(traceback.format_exc())
 
     def initialise_localisation_dict(self):
         if hasattr(self, "localisation_dict"):
             self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
```

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/picasso_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
 
             self.update_active_image(channel=image_channel.lower(), dataset=dataset_name,
                 frame_index = active_frame_index)
 
             self.draw_bounding_boxes()
 
             self.update_ui()
+            self.update_filter_criterion()
+            self.update_criterion_ranges()
 
         except:
             print(traceback.format_exc())
 
 
     def get_frame_locs(self, dataset_name, image_channel, frame_index):
         try:
@@ -457,14 +459,16 @@
             image = np.zeros(image_shape[-2:], dtype=np.int8)
 
         return image, pixel_size, oversampling
 
     def picasso_render_finished(self):
 
         self.update_ui(init=False)
+        self.update_filter_criterion()
+        self.update_criterion_ranges()
 
 
     def draw_picasso_render(self, data):
 
         try:
             image, pixel_size, oversampling = data
```

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/plot_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/plot_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
             print(traceback.format_exc())
             print(plot_data)
 
     def custom_gaussian(self, x, a, b, c, d):
         """ Custom Gaussian model with baseline and peak height parameters. """
         return a + (b - a) * np.exp(-(x - c) ** 2 / (2 * d ** 2))
 
-    def fit_custom_gaussian(self, x_data, y_data):
+    def fit_custom_gaussian(self, x_data, y_data, upscale=True):
         """ Fit the custom Gaussian model to 1D data. """
         # Initial guesses:
         # a: Minimum y-data (baseline)
         # b: Maximum y-data
         # c: x value at the maximum y
         # d: Approximate width from data spread
 
@@ -298,16 +298,18 @@
         y_data = np.array(y_data)
 
         initial_guess = [min(y_data), max(y_data), x_data[np.argmax(y_data)], np.std(x_data) / 2]
 
         # Fit the model
         popt, pcov = curve_fit(self.custom_gaussian, x_data, y_data, p0=initial_guess)
 
-        #high rest x values
-        fitX = np.linspace(start = min(x_data), stop = max(x_data), num = 1000)
+        if upscale:
+            fitX = np.linspace(start = min(x_data), stop = max(x_data), num = 1000)
+        else:
+            fitX = x_data
 
         # Generate the fitted curve
         fitY = self.custom_gaussian(fitX, *popt)
 
         width = 2 * np.sqrt(2 * np.log(2)) * popt[3]
 
         return fitX, fitY, width
```

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/undrift_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/undrift_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.1.0/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.1.1/src/smlmlab/utils/viewer_utils.py`

 * *Files identical despite different names*

