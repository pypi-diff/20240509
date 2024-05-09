# Comparing `tmp/lab_door_access-0.1.0.tar.gz` & `tmp/lab_door_access-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab_door_access-0.1.0.tar", max compression
+gzip compressed data, was "lab_door_access-0.2.0.tar", max compression
```

## Comparing `lab_door_access-0.1.0.tar` & `lab_door_access-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-19 18:39:00.759472 lab_door_access-0.1.0/LICENSE
--rw-r--r--   0        0        0     4344 2024-04-30 21:00:40.283840 lab_door_access-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:39:11.079341 lab_door_access-0.1.0/door_access/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-30 20:10:02.407384 lab_door_access-0.1.0/door_access/find_reader.py
--rw-r--r--   0        0        0     2083 2024-04-26 23:08:51.316284 lab_door_access-0.1.0/door_access/loggerconf.py
--rw-r--r--   0        0        0     2482 2024-04-30 19:13:28.417968 lab_door_access-0.1.0/door_access/rfid_reader.py
--rw-r--r--   0        0        0      895 2024-04-30 21:55:12.512267 lab_door_access-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 lab_door_access-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 18:39:00.759472 lab_door_access-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4573 2024-05-09 06:26:33.843924 lab_door_access-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 21:13:25.155023 lab_door_access-0.2.0/door_access/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-03 21:13:25.155023 lab_door_access-0.2.0/door_access/find_reader.py
+-rw-r--r--   0        0        0     2083 2024-05-03 21:13:25.155023 lab_door_access-0.2.0/door_access/loggerconf.py
+-rw-r--r--   0        0        0     3022 2024-05-09 06:16:14.342381 lab_door_access-0.2.0/door_access/rfid_reader.py
+-rw-r--r--   0        0        0      895 2024-05-09 06:18:09.507639 lab_door_access-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 lab_door_access-0.2.0/PKG-INFO
```

### Comparing `lab_door_access-0.1.0/LICENSE` & `lab_door_access-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lab_door_access-0.1.0/README.md` & `lab_door_access-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 # Laboratory access door system
 
-System service to control access to the Laboratory door.
+System service to control access to the Laboratory door. Use supervisor for daemonize and it's resilent to usb disconnections.
 
-Use supervisor for daemonize and it's resilent to usb disconnections.
+Web interface: <https://github.com/rodrigodeleonv/door-access-mgm>
 
-- You need to configure: `/opt/rfid/config-reader.yml`
-- Logs: `tail -f /opt/rfid/app.log`
-- Control service with: `sudo supervisorctl status` | `sudo supervisorctl restart rfid-usb-reader`
+
+# TODO: PACKAGE THIS RELEASE
 
 ## Install
 
 Simple installation script.
 
 ```bash
-sudo curl -L https://raw.githubusercontent.com/rodrigodeleonv/lab-door-access/main/installer.sh | bash
+sudo curl -fsSL https://raw.githubusercontent.com/rodrigodeleonv/lab-door-access/main/installer.sh | bash
 ```
 
-* This application requires supervisor.
+1. Install the service
+1. You need to configure: `/opt/rfid/config-reader.yml`
+1. Go to admin (ex <https://127.0.0.1/admin/>) search or create the API Token
+1. Configure the correct URL endpoint
+1. Restart the service: `sudo supervisorctl restart rfid-usb-reader`
+
+Optional
+
+1. Logs: `tail -f /opt/rfid/app.log`
+1. Verify service: `sudo supervisorctl status`
 
 ## Development
 
 ### Configure Poetry
 
 - [Poetry publish - One time setup](https://stackoverflow.com/a/72524326)
 - [How to publish with Poetry](https://towardsdatascience.com/packages-part-2-how-to-publish-test-your-package-on-pypi-with-poetry-9fc7295df1a5)
```

### Comparing `lab_door_access-0.1.0/door_access/find_reader.py` & `lab_door_access-0.2.0/door_access/find_reader.py`

 * *Files identical despite different names*

### Comparing `lab_door_access-0.1.0/door_access/loggerconf.py` & `lab_door_access-0.2.0/door_access/loggerconf.py`

 * *Files identical despite different names*

### Comparing `lab_door_access-0.1.0/door_access/rfid_reader.py` & `lab_door_access-0.2.0/door_access/rfid_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,52 +20,64 @@
         The last digit of the scancode.
     """
     digit = (data.scancode - 1) % 10
     return str(digit)
 
 
 def send_post_request(
-    session: requests.Session, url: str, tag_id: str, timeout: int = 5
+    session: requests.Session,
+    url: str,
+    tag_id: str,
+    timeout: int = 5,
+    ssl_verify: bool = False,
 ) -> dict:
     """Sends a POST request to the URL with the tag ID.
 
     Args:
         session: The requests.Session object.
         url: The URL to send the POST request.
         tag_id: The tag ID to send in the request body.
+        ssl_verify: Whether to verify the SSL certificate.
+            False allows to use self cert in local/internal network.
 
     Returns:
         A dictionary containing the` response data` and `status code`.
     """
+
     body = {"tag_id": tag_id}
     data = {"status_code": None, "response": None}
     try:
-        response = session.post(url, json=body, timeout=timeout)
+        response = session.post(url, json=body, timeout=timeout, verify=ssl_verify)
     except requests.exceptions.RequestException:
         logger.exception("Failed to send POST request")
         return
     else:
         data["status_code"] = response.status_code
     try:
         data["response"] = response.json()
     except JSONDecodeError:
         logger.exception("Error parsing response")
         return
     return data
 
 
-def main_loop(reader: InputDevice, url: str):
+def main_loop(reader: InputDevice, url: str, api_token: str, api_auth_scheme: str):
     """Main loop of the RFID reader.
 
     Args:
         reader: InputDevice object representing the RFID reader.
         url: The URL to send the POST request.
+        api_token: The API token to send in the request headers.
+        api_auth_scheme: The API authentication scheme to send in the request headers.
+            example: Token (Basic, Bearer not supported)
     """
     rfid_tag = ""
+    headers = {"Authorization": f"{api_auth_scheme} {api_token}"}
     session = requests.Session()
+    session.headers.update(headers)
     logger.info(f"Listening for RFID scans on device: {reader.path}")
 
     # event: KeyEvent
     for event in reader.read_loop():
         if event.type != ecodes.EV_KEY:
             # logger.debug(f"Skipping non-key event: {event}")
             continue
```

### Comparing `lab_door_access-0.1.0/pyproject.toml` & `lab_door_access-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lab-door-access"
-version = "0.1.0"
+version = "0.2.0"
 description = "System app to control the door access"
 authors = ["R. D."]
 license = "Apache License Version 2.0"
 readme = "README.md"
 packages = [{include = "door_access"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `lab_door_access-0.1.0/PKG-INFO` & `lab_door_access-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-door-access
-Version: 0.1.0
+Version: 0.2.0
 Summary: System app to control the door access
 License: Apache License Version 2.0
 Author: R. D.
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
@@ -17,31 +17,39 @@
 Requires-Dist: evdev (>=1.7.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Laboratory access door system
 
-System service to control access to the Laboratory door.
+System service to control access to the Laboratory door. Use supervisor for daemonize and it's resilent to usb disconnections.
 
-Use supervisor for daemonize and it's resilent to usb disconnections.
+Web interface: <https://github.com/rodrigodeleonv/door-access-mgm>
 
-- You need to configure: `/opt/rfid/config-reader.yml`
-- Logs: `tail -f /opt/rfid/app.log`
-- Control service with: `sudo supervisorctl status` | `sudo supervisorctl restart rfid-usb-reader`
+
+# TODO: PACKAGE THIS RELEASE
 
 ## Install
 
 Simple installation script.
 
 ```bash
-sudo curl -L https://raw.githubusercontent.com/rodrigodeleonv/lab-door-access/main/installer.sh | bash
+sudo curl -fsSL https://raw.githubusercontent.com/rodrigodeleonv/lab-door-access/main/installer.sh | bash
 ```
 
-* This application requires supervisor.
+1. Install the service
+1. You need to configure: `/opt/rfid/config-reader.yml`
+1. Go to admin (ex <https://127.0.0.1/admin/>) search or create the API Token
+1. Configure the correct URL endpoint
+1. Restart the service: `sudo supervisorctl restart rfid-usb-reader`
+
+Optional
+
+1. Logs: `tail -f /opt/rfid/app.log`
+1. Verify service: `sudo supervisorctl status`
 
 ## Development
 
 ### Configure Poetry
 
 - [Poetry publish - One time setup](https://stackoverflow.com/a/72524326)
 - [How to publish with Poetry](https://towardsdatascience.com/packages-part-2-how-to-publish-test-your-package-on-pypi-with-poetry-9fc7295df1a5)
```

