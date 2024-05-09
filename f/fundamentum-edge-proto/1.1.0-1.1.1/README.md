# Comparing `tmp/fundamentum_edge_proto-1.1.0.tar.gz` & `tmp/fundamentum_edge_proto-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundamentum_edge_proto-1.1.0.tar", last modified: Fri May  3 20:22:48 2024, max compression
+gzip compressed data, was "fundamentum_edge_proto-1.1.1.tar", last modified: Thu May  9 19:45:12 2024, max compression
```

## Comparing `fundamentum_edge_proto-1.1.0.tar` & `fundamentum_edge_proto-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-05-03 20:22:37.431906 fundamentum_edge_proto-1.1.0/LICENSE
--rw-r--r--   0        0        0     1161 2024-05-03 20:22:37.431906 fundamentum_edge_proto-1.1.0/README.md
--rw-r--r--   0        0        0     1878 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/__init__.py
--rw-r--r--   0        0        0     1430 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.py
--rw-r--r--   0        0        0      660 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.pyi
--rw-r--r--   0        0        0     3362 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     2139 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.pyi
--rw-r--r--   0        0        0     1539 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.py
--rw-r--r--   0        0        0     1352 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.pyi
--rw-r--r--   0        0        0     2223 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.py
--rw-r--r--   0        0        0     2078 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/py.typed
--rw-r--r--   0        0        0      875 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2.py
--rw-r--r--   0        0        0      471 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2.pyi
--rw-r--r--   0        0        0       87 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2_grpc.py
--rw-r--r--   0        0        0      382 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2_grpc.pyi
--rw-r--r--   0        0        0     1989 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2.py
--rw-r--r--   0        0        0     1666 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2.pyi
--rw-r--r--   0        0        0     2180 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2_grpc.py
--rw-r--r--   0        0        0     1771 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2_grpc.pyi
--rw-r--r--   0        0        0     1360 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.py
--rw-r--r--   0        0        0      726 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.pyi
--rw-r--r--   0        0        0     2158 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.py
--rw-r--r--   0        0        0     1703 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2429 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/typed_stubs.py
--rw-r--r--   0        0        0     2153 2024-05-03 20:22:48.047951 fundamentum_edge_proto-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    14505 1970-01-01 00:00:00.000000 fundamentum_edge_proto-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 19:45:01.100425 fundamentum_edge_proto-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1161 2024-05-09 19:45:01.100425 fundamentum_edge_proto-1.1.1/README.md
+-rw-r--r--   0        0        0     1878 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/__init__.py
+-rw-r--r--   0        0        0     1430 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2.py
+-rw-r--r--   0        0        0      660 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2.pyi
+-rw-r--r--   0        0        0     3362 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     2139 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1539 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2.py
+-rw-r--r--   0        0        0     1352 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2.pyi
+-rw-r--r--   0        0        0     2223 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.py
+-rw-r--r--   0        0        0     2078 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/py.typed
+-rw-r--r--   0        0        0      875 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/qos_pb2.py
+-rw-r--r--   0        0        0      471 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/qos_pb2.pyi
+-rw-r--r--   0        0        0       87 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/qos_pb2_grpc.py
+-rw-r--r--   0        0        0      382 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/qos_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1989 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2.py
+-rw-r--r--   0        0        0     1666 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2.pyi
+-rw-r--r--   0        0        0     2180 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2_grpc.py
+-rw-r--r--   0        0        0     1771 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1360 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2.py
+-rw-r--r--   0        0        0      726 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2.pyi
+-rw-r--r--   0        0        0     2158 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.py
+-rw-r--r--   0        0        0     1703 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2429 2024-05-09 19:45:02.612433 fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/typed_stubs.py
+-rw-r--r--   0        0        0     2167 2024-05-09 19:45:12.704480 fundamentum_edge_proto-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14527 1970-01-01 00:00:00.000000 fundamentum_edge_proto-1.1.1/PKG-INFO
```

### Comparing `fundamentum_edge_proto-1.1.0/LICENSE` & `fundamentum_edge_proto-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/README.md` & `fundamentum_edge_proto-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/__init__.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/__init__.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/configuration_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/qos_pb2.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2_grpc.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/states_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/typed_stubs.py` & `fundamentum_edge_proto-1.1.1/fundamentum_edge_proto/typed_stubs.py`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.1.0/pyproject.toml` & `fundamentum_edge_proto-1.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     { name = "Alex Sirois", email = "asirois@dimonoff.com" },
     { name = "Jonathan Chouinard", email = "jchouinard@dimonoff.com" },
 ]
 dynamic = []
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
+    "grpcio",
     "protobuf>=3.20.3",
 ]
-version = "1.1.0"
+version = "1.1.1"
 
 [project.urls]
 repository = "https://bitbucket.org/amotus/fundamentum-edge-proto-python"
 
 [project.license]
 file = "LICENSE"
```

### Comparing `fundamentum_edge_proto-1.1.0/PKG-INFO` & `fundamentum_edge_proto-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundamentum-edge-proto
-Version: 1.1.0
+Version: 1.1.1
 Summary: fundamentum-edge protobufs
 Author-Email: Alex Sirois <asirois@dimonoff.com>, Jonathan Chouinard <jchouinard@dimonoff.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,14 +202,15 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: Repository, https://bitbucket.org/amotus/fundamentum-edge-proto-python
 Requires-Python: >=3.10
+Requires-Dist: grpcio
 Requires-Dist: protobuf>=3.20.3
 Description-Content-Type: text/markdown
 
 # Fundamentum Edge Proto Python
 
 [![Crates.io][crate-badge]][crate-url]
 [![License][licence-badge]][licence-url]
```

