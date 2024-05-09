# Comparing `tmp/xmanager_slurm-0.3.0-py3-none-any.whl.zip` & `tmp/xmanager_slurm-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 51859 bytes, number of entries: 38
+Zip file size: 51843 bytes, number of entries: 38
 -rw-r--r--  2.0 unx     1019 b- defN 16-Jan-01 00:00 xm_slurm/__init__.py
 -rw-r--r--  2.0 unx     9533 b- defN 16-Jan-01 00:00 xm_slurm/api.py
 -rw-r--r--  2.0 unx     4379 b- defN 16-Jan-01 00:00 xm_slurm/batching.py
 -rw-r--r--  2.0 unx     4955 b- defN 16-Jan-01 00:00 xm_slurm/config.py
 -rw-r--r--  2.0 unx       54 b- defN 16-Jan-01 00:00 xm_slurm/console.py
 -rw-r--r--  2.0 unx     1600 b- defN 16-Jan-01 00:00 xm_slurm/contrib/clusters/__init__.py
 -rw-r--r--  2.0 unx     5201 b- defN 16-Jan-01 00:00 xm_slurm/contrib/clusters/drac.py
@@ -27,14 +27,14 @@
 -rw-r--r--  2.0 unx      748 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/pdm.Dockerfile
 -rw-r--r--  2.0 unx      738 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/python.Dockerfile
 -rw-r--r--  2.0 unx     1071 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/monitor.bash.j2
 -rw-r--r--  2.0 unx      814 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/proxy.bash.j2
 -rw-r--r--  2.0 unx      599 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-array.bash.j2
 -rw-r--r--  2.0 unx     1120 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-group.bash.j2
 -rw-r--r--  2.0 unx     1852 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job.bash.j2
--rw-r--r--  2.0 unx     3241 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
+-rw-r--r--  2.0 unx     3222 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
 -rw-r--r--  2.0 unx     1469 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/podman.bash.j2
 -rw-r--r--  2.0 unx     1930 b- defN 16-Jan-01 00:00 xm_slurm/utils.py
--rw-r--r--  2.0 unx      909 b- defN 16-Jan-01 00:00 xmanager_slurm-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xmanager_slurm-0.3.0.dist-info/WHEEL
-?rw-------  2.0 unx     3305 b- defN 16-Jan-01 00:00 xmanager_slurm-0.3.0.dist-info/RECORD
-38 files, 169148 bytes uncompressed, 46547 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx      909 b- defN 16-Jan-01 00:00 xmanager_slurm-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xmanager_slurm-0.3.1.dist-info/WHEEL
+?rw-------  2.0 unx     3305 b- defN 16-Jan-01 00:00 xmanager_slurm-0.3.1.dist-info/RECORD
+38 files, 169129 bytes uncompressed, 46531 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -99,17 +99,17 @@
 
 Filename: xm_slurm/templates/slurm/runtimes/podman.bash.j2
 Comment: 
 
 Filename: xm_slurm/utils.py
 Comment: 
 
-Filename: xmanager_slurm-0.3.0.dist-info/METADATA
+Filename: xmanager_slurm-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: xmanager_slurm-0.3.0.dist-info/WHEEL
+Filename: xmanager_slurm-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: xmanager_slurm-0.3.0.dist-info/RECORD
+Filename: xmanager_slurm-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_slurm/templates/slurm/runtimes/apptainer.bash.j2

```diff
@@ -73,15 +73,15 @@
   --no-init \
   --no-umask \
   --no-home \
   --cleanenv \
   --containall \
 {% if cluster.mounts %}
 {% for source, dest in cluster.mounts.items() %}
-  --mount type=bind,src={{ source }},dst={{ dest }} \
+  --bind {{ source }}:{{ dest }} \
 {% endfor %}
 {% endif %}
   --workdir "$SLURM_TMPDIR"/container-workdir \
 {% if (cluster.runtime | string) == "apptainer" %}
   --overlay "$SLURM_TMPDIR"/container-overlay \
 {% else %}
   --writable \
```

## Comparing `xmanager_slurm-0.3.0.dist-info/METADATA` & `xmanager_slurm-0.3.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmanager-slurm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Slurm backend for XManager.
 Author-Email: Jesse Farebrother <jfarebro@cs.mcgill.ca>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: xmanager>=0.4.0
 Requires-Dist: asyncssh>=2.13.2
 Requires-Dist: humanize>=4.8.0
```

## Comparing `xmanager_slurm-0.3.0.dist-info/RECORD` & `xmanager_slurm-0.3.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 xm_slurm/templates/docker/pdm.Dockerfile,sha256=Yg5-lOXkNVJr0OER_yOnRvn9NlFLnt3RfdYfq4f0ilg,748
 xm_slurm/templates/docker/python.Dockerfile,sha256=O6lHesmsLz7cX-efVQpsafEVYmbHPyV73xA9WbBKGKg,738
 xm_slurm/templates/slurm/fragments/monitor.bash.j2,sha256=CxtbxOJzd0Un-ApDO6T8JHuKlSv6uwwBFMJPeGjCKnk,1071
 xm_slurm/templates/slurm/fragments/proxy.bash.j2,sha256=VJLglZo-Nvx9R-qe3rHTxr07CylTQ6Z9NwBzvIpAZrA,814
 xm_slurm/templates/slurm/job-array.bash.j2,sha256=d4twfV1PATGQwTIleFBUIGmMAIHH-F7RjBsdfaAIQko,599
 xm_slurm/templates/slurm/job-group.bash.j2,sha256=UkjfBE7jg9mepcUWaHZEAjkiXsIM1j_sLxLzxkteD-Y,1120
 xm_slurm/templates/slurm/job.bash.j2,sha256=EUeq3P2xqTIqlHi2SVhFBT7NL4lUj8okYUa3GnlaIIc,1852
-xm_slurm/templates/slurm/runtimes/apptainer.bash.j2,sha256=Z8Mc4wbmOJW_n9V0hcKsPNEnveZFqsASg8Z3dICaETk,3241
+xm_slurm/templates/slurm/runtimes/apptainer.bash.j2,sha256=dMntzelhs8DqKyIpO9S6wzMfH2PDevmgvyjCW8Xc2dY,3222
 xm_slurm/templates/slurm/runtimes/podman.bash.j2,sha256=xKXYFvQvazMx0PgvmlRXR6eecoiBUl8y52dIzQtWkBE,1469
 xm_slurm/utils.py,sha256=PNd0vTn33UKm5LpC41TdO9QIFe21V5A0RbYEhQIMjrA,1930
-xmanager_slurm-0.3.0.dist-info/METADATA,sha256=Cjiev-9s_DlKicsDWSgja-m3fYRcnG8UOEXaWTdxyI0,909
-xmanager_slurm-0.3.0.dist-info/WHEEL,sha256=vnE8JVcI2Wz7GRKorsPArnBdnW2SWKWGow5gu5tHlRU,90
-xmanager_slurm-0.3.0.dist-info/RECORD,,
+xmanager_slurm-0.3.1.dist-info/METADATA,sha256=uESSCwHQ0YvVRFwvqo3D-YIJQ9oW-tcufqTZoAruzto,909
+xmanager_slurm-0.3.1.dist-info/WHEEL,sha256=vnE8JVcI2Wz7GRKorsPArnBdnW2SWKWGow5gu5tHlRU,90
+xmanager_slurm-0.3.1.dist-info/RECORD,,
```

