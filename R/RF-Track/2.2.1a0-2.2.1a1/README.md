# Comparing `tmp/RF_Track-2.2.1a0-py3-none-manylinux_2_35_x86_64.whl.zip` & `tmp/RF_Track-2.2.1a1-cp311-cp311-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 1357296 bytes, number of entries: 8
--rw-rw-r--  2.0 unx   129966 b- defN 23-Nov-28 22:36 RF_Track/RF_Track.py
--rwxr-xr-x  2.0 unx  4587928 b- defN 23-Dec-08 15:05 RF_Track/_RF_Track.so
--rw-rw-r--  2.0 unx   120585 b- defN 23-Dec-08 15:05 RF_Track/__init__.py
--rw-r--r--  2.0 unx      635 b- defN 23-Dec-08 15:06 RF_Track-2.2.1a0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1752 b- defN 23-Dec-08 15:06 RF_Track-2.2.1a0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Dec-08 15:06 RF_Track-2.2.1a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Dec-08 15:06 RF_Track-2.2.1a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      639 b- defN 23-Dec-08 15:06 RF_Track-2.2.1a0.dist-info/RECORD
-8 files, 4841624 bytes uncompressed, 1356196 bytes compressed:  72.0%
+Zip file size: 1004502 bytes, number of entries: 7
+-rw-r--r--  2.0 unx   122435 b- defN 24-Mar-04 15:34 RF_Track.py
+-rwxr-xr-x  2.0 unx  3873804 b- defN 24-Mar-04 21:30 _RF_Track.cpython-311-darwin.so
+-rw-r--r--  2.0 unx      638 b- defN 24-Mar-04 21:30 RF_Track-2.2.1a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1733 b- defN 24-Mar-04 21:30 RF_Track-2.2.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Mar-04 21:30 RF_Track-2.2.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Mar-04 21:30 RF_Track-2.2.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      562 b- defN 24-Mar-04 21:30 RF_Track-2.2.1a1.dist-info/RECORD
+7 files, 3999301 bytes uncompressed, 1003516 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
-Filename: RF_Track/RF_Track.py
+Filename: RF_Track.py
 Comment: 
 
-Filename: RF_Track/_RF_Track.so
+Filename: _RF_Track.cpython-311-darwin.so
 Comment: 
 
-Filename: RF_Track/__init__.py
+Filename: RF_Track-2.2.1a1.dist-info/LICENSE
 Comment: 
 
-Filename: RF_Track-2.2.1a0.dist-info/LICENSE
+Filename: RF_Track-2.2.1a1.dist-info/METADATA
 Comment: 
 
-Filename: RF_Track-2.2.1a0.dist-info/METADATA
+Filename: RF_Track-2.2.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: RF_Track-2.2.1a0.dist-info/WHEEL
+Filename: RF_Track-2.2.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: RF_Track-2.2.1a0.dist-info/top_level.txt
-Comment: 
-
-Filename: RF_Track-2.2.1a0.dist-info/RECORD
+Filename: RF_Track-2.2.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `RF_Track/__init__.py` & `RF_Track.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (https://www.swig.org).
-# Version 4.2.0
+# Version 4.2.1
 #
 # Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 from sys import version_info as _swig_python_version_info
 # Import the low-level C/C++ module
 if __package__ or "." in __name__:
@@ -164,19 +164,22 @@
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined - class is abstract")
     __repr__ = _swig_repr
     __swig_destroy__ = _RF_Track.delete_Element
     clone = _swig_new_instance_method(_RF_Track.Element_clone)
     set_offsets = _swig_new_instance_method(_RF_Track.Element_set_offsets)
+    get_S = _swig_new_instance_method(_RF_Track.Element_get_S)
+    get_name = _swig_new_instance_method(_RF_Track.Element_get_name)
     get_nsteps = _swig_new_instance_method(_RF_Track.Element_get_nsteps)
     get_tt_nsteps = _swig_new_instance_method(_RF_Track.Element_get_tt_nsteps)
     get_sc_nsteps = _swig_new_instance_method(_RF_Track.Element_get_sc_nsteps)
     get_cfx_nsteps = _swig_new_instance_method(_RF_Track.Element_get_cfx_nsteps)
     get_length = _swig_new_instance_method(_RF_Track.Element_get_length)
+    set_name = _swig_new_instance_method(_RF_Track.Element_set_name)
     set_tt_nsteps = _swig_new_instance_method(_RF_Track.Element_set_tt_nsteps)
     set_sc_nsteps = _swig_new_instance_method(_RF_Track.Element_set_sc_nsteps)
     set_cfx_nsteps = _swig_new_instance_method(_RF_Track.Element_set_cfx_nsteps)
     set_nsteps = _swig_new_instance_method(_RF_Track.Element_set_nsteps)
     get_field = _swig_new_instance_method(_RF_Track.Element_get_field)
     add_collective_effect = _swig_new_instance_method(_RF_Track.Element_add_collective_effect)
     clear_collective_effects = _swig_new_instance_method(_RF_Track.Element_clear_collective_effects)
@@ -292,14 +295,15 @@
     set_Brho = _swig_new_instance_method(_RF_Track.SBend_set_Brho)
     set_Bfield = _swig_new_instance_method(_RF_Track.SBend_set_Bfield)
     set_P_over_Q = _swig_new_instance_method(_RF_Track.SBend_set_P_over_Q)
     __swig_destroy__ = _RF_Track.delete_SBend
 
 # Register SBend in _RF_Track:
 _RF_Track.SBend_swigregister(SBend)
+RBend = _RF_Track.RBend
 class Absorber(ConstantField):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         _RF_Track.Absorber_swiginit(self, _RF_Track.new_Absorber(*args))
     enable_log_term = _swig_new_instance_method(_RF_Track.Absorber_enable_log_term)
@@ -483,15 +487,14 @@
     apply_force = _swig_new_instance_method(_RF_Track.Bunch6dT_apply_force)
     kick = _swig_new_instance_method(_RF_Track.Bunch6dT_kick)
     drift = _swig_new_instance_method(_RF_Track.Bunch6dT_drift)
     load = _swig_new_instance_method(_RF_Track.Bunch6dT_load)
     save = _swig_new_instance_method(_RF_Track.Bunch6dT_save)
     save_as_dst_file = _swig_new_instance_method(_RF_Track.Bunch6dT_save_as_dst_file)
     save_as_sdds_file = _swig_new_instance_method(_RF_Track.Bunch6dT_save_as_sdds_file)
-    __brace__ = _swig_new_instance_method(_RF_Track.Bunch6dT___brace__)
     __swig_destroy__ = _RF_Track.delete_Bunch6dT
 
 # Register Bunch6dT in _RF_Track:
 _RF_Track.Bunch6dT_swigregister(Bunch6dT)
 class Bunch6d(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -527,29 +530,30 @@
     apply_force = _swig_new_instance_method(_RF_Track.Bunch6d_apply_force)
     kick = _swig_new_instance_method(_RF_Track.Bunch6d_kick)
     drift = _swig_new_instance_method(_RF_Track.Bunch6d_drift)
     load = _swig_new_instance_method(_RF_Track.Bunch6d_load)
     save = _swig_new_instance_method(_RF_Track.Bunch6d_save)
     save_as_dst_file = _swig_new_instance_method(_RF_Track.Bunch6d_save_as_dst_file)
     save_as_sdds_file = _swig_new_instance_method(_RF_Track.Bunch6d_save_as_sdds_file)
-    __brace__ = _swig_new_instance_method(_RF_Track.Bunch6d___brace__)
     __swig_destroy__ = _RF_Track.delete_Bunch6d
 
 # Register Bunch6d in _RF_Track:
 _RF_Track.Bunch6d_swigregister(Bunch6d)
 Bunch6d_QR = _RF_Track.Bunch6d_QR
 class Bunch6d_info(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     S = property(_RF_Track.Bunch6d_info_S_get, _RF_Track.Bunch6d_info_S_set)
     mean_x = property(_RF_Track.Bunch6d_info_mean_x_get, _RF_Track.Bunch6d_info_mean_x_set)
     mean_y = property(_RF_Track.Bunch6d_info_mean_y_get, _RF_Track.Bunch6d_info_mean_y_set)
     mean_t = property(_RF_Track.Bunch6d_info_mean_t_get, _RF_Track.Bunch6d_info_mean_t_set)
     mean_xp = property(_RF_Track.Bunch6d_info_mean_xp_get, _RF_Track.Bunch6d_info_mean_xp_set)
     mean_yp = property(_RF_Track.Bunch6d_info_mean_yp_get, _RF_Track.Bunch6d_info_mean_yp_set)
+    mean_Px = property(_RF_Track.Bunch6d_info_mean_Px_get, _RF_Track.Bunch6d_info_mean_Px_set)
+    mean_Py = property(_RF_Track.Bunch6d_info_mean_Py_get, _RF_Track.Bunch6d_info_mean_Py_set)
     mean_P = property(_RF_Track.Bunch6d_info_mean_P_get, _RF_Track.Bunch6d_info_mean_P_set)
     mean_K = property(_RF_Track.Bunch6d_info_mean_K_get, _RF_Track.Bunch6d_info_mean_K_set)
     mean_E = property(_RF_Track.Bunch6d_info_mean_E_get, _RF_Track.Bunch6d_info_mean_E_set)
     sigma_x = property(_RF_Track.Bunch6d_info_sigma_x_get, _RF_Track.Bunch6d_info_sigma_x_set)
     sigma_y = property(_RF_Track.Bunch6d_info_sigma_y_get, _RF_Track.Bunch6d_info_sigma_y_set)
     sigma_t = property(_RF_Track.Bunch6d_info_sigma_t_get, _RF_Track.Bunch6d_info_sigma_t_set)
     sigma_px = property(_RF_Track.Bunch6d_info_sigma_px_get, _RF_Track.Bunch6d_info_sigma_px_set)
@@ -856,14 +860,34 @@
     set_z0 = _swig_new_instance_method(_RF_Track.SW_Structure_set_z0)
     set_z1 = _swig_new_instance_method(_RF_Track.SW_Structure_set_z1)
     set_cell_length = _swig_new_instance_method(_RF_Track.SW_Structure_set_cell_length)
     __swig_destroy__ = _RF_Track.delete_SW_Structure
 
 # Register SW_Structure in _RF_Track:
 _RF_Track.SW_Structure_swigregister(SW_Structure)
+class Pillbox_Cavity(RF_Field):
+    thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
+    __repr__ = _swig_repr
+
+    def __init__(self, *args):
+        _RF_Track.Pillbox_Cavity_swiginit(self, _RF_Track.new_Pillbox_Cavity(*args))
+    get_cell_length = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_get_cell_length)
+    get_z0 = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_get_z0)
+    get_z1 = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_get_z1)
+    get_coefficients = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_get_coefficients)
+    get_static_Bfield = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_get_static_Bfield)
+    set_static_Bfield = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_set_static_Bfield)
+    set_coefficients = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_set_coefficients)
+    set_z0 = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_set_z0)
+    set_z1 = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_set_z1)
+    set_cell_length = _swig_new_instance_method(_RF_Track.Pillbox_Cavity_set_cell_length)
+    __swig_destroy__ = _RF_Track.delete_Pillbox_Cavity
+
+# Register Pillbox_Cavity in _RF_Track:
+_RF_Track.Pillbox_Cavity_swigregister(Pillbox_Cavity)
 class TW_Structure(RF_Field):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         _RF_Track.TW_Structure_swiginit(self, _RF_Track.new_TW_Structure(*args))
     get_cell_length = _swig_new_instance_method(_RF_Track.TW_Structure_get_cell_length)
@@ -957,20 +981,20 @@
 _RF_Track.TransportTable_swigregister(TransportTable)
 class Multipole(GenericField):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         _RF_Track.Multipole_swiginit(self, _RF_Track.new_Multipole(*args))
-    set_Bn = _swig_new_instance_method(_RF_Track.Multipole_set_Bn)
     get_Bn = _swig_new_instance_method(_RF_Track.Multipole_get_Bn)
     get_KnL = _swig_new_instance_method(_RF_Track.Multipole_get_KnL)
     get_strengths = _swig_new_instance_method(_RF_Track.Multipole_get_strengths)
-    set_strengths = _swig_new_instance_method(_RF_Track.Multipole_set_strengths)
+    set_Bn = _swig_new_instance_method(_RF_Track.Multipole_set_Bn)
     set_KnL = _swig_new_instance_method(_RF_Track.Multipole_set_KnL)
+    set_strengths = _swig_new_instance_method(_RF_Track.Multipole_set_strengths)
     get_static_Efield = _swig_new_instance_method(_RF_Track.Multipole_get_static_Efield)
     get_static_Bfield = _swig_new_instance_method(_RF_Track.Multipole_get_static_Bfield)
     set_static_Efield = _swig_new_instance_method(_RF_Track.Multipole_set_static_Efield)
     set_static_Bfield = _swig_new_instance_method(_RF_Track.Multipole_set_static_Bfield)
     __swig_destroy__ = _RF_Track.delete_Multipole
 
 # Register Multipole in _RF_Track:
@@ -1036,38 +1060,39 @@
     get_solenoids = _swig_new_instance_method(_RF_Track.Lattice_get_solenoids)
     get_lattices = _swig_new_instance_method(_RF_Track.Lattice_get_lattices)
     get_volumes = _swig_new_instance_method(_RF_Track.Lattice_get_volumes)
     get_sbends = _swig_new_instance_method(_RF_Track.Lattice_get_sbends)
     get_drifts = _swig_new_instance_method(_RF_Track.Lattice_get_drifts)
     get_coils = _swig_new_instance_method(_RF_Track.Lattice_get_coils)
     get_bpms = _swig_new_instance_method(_RF_Track.Lattice_get_bpms)
+    get_elements_by_name = _swig_new_instance_method(_RF_Track.Lattice_get_elements_by_name)
     set_bpm_resolution = _swig_new_instance_method(_RF_Track.Lattice_set_bpm_resolution)
     get_bpm_resolution = _swig_new_instance_method(_RF_Track.Lattice_get_bpm_resolution)
     get_bpm_readings = _swig_new_instance_method(_RF_Track.Lattice_get_bpm_readings)
     get_corrector_strengths = _swig_new_instance_method(_RF_Track.Lattice_get_corrector_strengths)
     set_corrector_strengths = _swig_new_instance_method(_RF_Track.Lattice_set_corrector_strengths)
     vary_corrector_strengths = _swig_new_instance_method(_RF_Track.Lattice_vary_corrector_strengths)
     reset_correctors = _swig_new_instance_method(_RF_Track.Lattice_reset_correctors)
     get_response_matrix = _swig_new_instance_method(_RF_Track.Lattice_get_response_matrix)
     scatter_elements = _swig_new_instance_method(_RF_Track.Lattice_scatter_elements)
     align_elements = _swig_new_instance_method(_RF_Track.Lattice_align_elements)
-    get_offsets = _swig_new_instance_method(_RF_Track.Lattice_get_offsets)
-    set_offsets = _swig_new_instance_method(_RF_Track.Lattice_set_offsets)
+    get_elements_offsets = _swig_new_instance_method(_RF_Track.Lattice_get_elements_offsets)
+    set_elements_offsets = _swig_new_instance_method(_RF_Track.Lattice_set_elements_offsets)
     orbit_correction = _swig_new_instance_method(_RF_Track.Lattice_orbit_correction)
-    __brace__ = _swig_new_instance_method(_RF_Track.Lattice___brace__)
+    __getitem__ = _swig_new_instance_method(_RF_Track.Lattice___getitem__)
 
 # Register Lattice in _RF_Track:
 _RF_Track.Lattice_swigregister(Lattice)
 class Volume(Element, TrackingOptions):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-
-    def __init__(self):
-        _RF_Track.Volume_swiginit(self, _RF_Track.new_Volume())
     __swig_destroy__ = _RF_Track.delete_Volume
+
+    def __init__(self, *args):
+        _RF_Track.Volume_swiginit(self, _RF_Track.new_Volume(*args))
     add = _swig_new_instance_method(_RF_Track.Volume_add)
     add_ref = _swig_new_instance_method(_RF_Track.Volume_add_ref)
     size = _swig_new_instance_method(_RF_Track.Volume_size)
     clear = _swig_new_instance_method(_RF_Track.Volume_clear)
     track = _swig_new_instance_method(_RF_Track.Volume_track)
     btrack = _swig_new_instance_method(_RF_Track.Volume_btrack)
     get_transport_table = _swig_new_instance_method(_RF_Track.Volume_get_transport_table)
@@ -1077,26 +1102,28 @@
     get_s0 = _swig_new_instance_method(_RF_Track.Volume_get_s0)
     get_s1 = _swig_new_instance_method(_RF_Track.Volume_get_s1)
     get_path_length = _swig_new_instance_method(_RF_Track.Volume_get_path_length)
     get_rf_elements = _swig_new_instance_method(_RF_Track.Volume_get_rf_elements)
     get_quadrupoles = _swig_new_instance_method(_RF_Track.Volume_get_quadrupoles)
     get_solenoids = _swig_new_instance_method(_RF_Track.Volume_get_solenoids)
     get_coils = _swig_new_instance_method(_RF_Track.Volume_get_coils)
+    get_elements_by_name = _swig_new_instance_method(_RF_Track.Volume_get_elements_by_name)
     set_s0 = _swig_new_instance_method(_RF_Track.Volume_set_s0)
     set_s1 = _swig_new_instance_method(_RF_Track.Volume_set_s1)
     set_s0_from_s1 = _swig_new_instance_method(_RF_Track.Volume_set_s0_from_s1)
     set_s1_from_s0 = _swig_new_instance_method(_RF_Track.Volume_set_s1_from_s0)
     set_length = _swig_new_instance_method(_RF_Track.Volume_set_length)
     get_static_Efield = _swig_new_instance_method(_RF_Track.Volume_get_static_Efield)
     get_static_Bfield = _swig_new_instance_method(_RF_Track.Volume_get_static_Bfield)
     set_static_Efield = _swig_new_instance_method(_RF_Track.Volume_set_static_Efield)
     set_static_Bfield = _swig_new_instance_method(_RF_Track.Volume_set_static_Bfield)
     set_t0 = _swig_new_instance_method(_RF_Track.Volume_set_t0)
     unset_t0 = _swig_new_instance_method(_RF_Track.Volume_unset_t0)
     autophase = _swig_new_instance_method(_RF_Track.Volume_autophase)
+    __getitem__ = _swig_new_instance_method(_RF_Track.Volume___getitem__)
 
 # Register Volume in _RF_Track:
 _RF_Track.Volume_swigregister(Volume)
 class Plasma(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     null_cell = property(_RF_Track.Plasma_null_cell_get, _RF_Track.Plasma_null_cell_set)
```

## Comparing `RF_Track-2.2.1a0.dist-info/LICENSE` & `RF_Track-2.2.1a1.dist-info/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright (c) CERN 2016-2023. All rights reserved.
+Copyright (c) CERN 2016-2024. All rights reserved.
 
 Since version 2.1, RF-Track is released under a CERN proprietary
 software licence. RF-Track can be used freely, but we have deemed
 it unsuited to share its source code. Any specific request shall be
 formulated in writing and addressed to CERN through mail-KT@cern.ch
 
-Any suggestions for extensions or new features can be addressed
-directly to the author: Andrea Latina <andrea.latina@cern.ch>
+Suggestions for extensions or new features can be addressed directly
+to the author: Andrea Latina <andrea.latina@cern.ch>
 
-The previous version of RF-Track, version 2.0, was free software
-released under GNU Public Licence. Accordingly, its source code is
+The previous version of RF-Track, version 2.0, was released as Free
+Software under the GNU Public Licence. Accordingly, its source code is
 freely available at the root of this Gitlab repository.
```

## Comparing `RF_Track-2.2.1a0.dist-info/METADATA` & `RF_Track-2.2.1a1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: RF-Track
-Version: 2.2.1a0
+Version: 2.2.1a1
 Summary: The CERN tracking code RF-Track
 Home-page: https://gitlab.cern.ch/rf-track
 Author: Andrea Latina
 Author-email: andrea.latina@cern.ch
 License: Proprietary
-Project-URL: Documentation, https://gitlab.cern.ch/rf-track/download/-/raw/master/rf-track-2.2.0/RF_Track_reference_manual.pdf?ref_type=heads
+Project-URL: Documentation, https://gitlab.cern.ch/rf-track/download/-/raw/master/rf-track-2.2.1a0/RF_Track_reference_manual.pdf?ref_type=heads
 Project-URL: Tracker, https://gitlab.cern.ch/groups/rf-track/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
-Provides: RF_Track
-Requires-Python: <3.12
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gsl
+Requires-Dist: fftw3
 
 RF-Track is a tracking code developed at CERN for the optimization of particle accelerators, which offers outstanding flexibility and rapid simulation speed.
 
 RF-Track can simulate beams of particles with arbitrary energy, mass, and charge, even mixed, solving fully relativistic equations of motion.  It can simulate the effects of space-charge forces, both in bunched and continuous-wave beams. It can transport the beams through common elements as well as through special ones: 1D, 2D, and 3D static or oscillating radio-frequency electromagnetic field maps (real and complex), flux concentrators, and electron coolers. It allows element overlap, and direct and indirect space-charge calculation using fast parallel algorithms.
 
 RF-Track is written in optimized and parallel C++ and uses the scripting languages Octave and Python as user interfaces. General knowledge of Octave or Python is recommended to get the best out of RF-Track.
```
