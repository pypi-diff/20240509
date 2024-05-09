# Comparing `tmp/smartplug_energy_controller-0.0.2.tar.gz` & `tmp/smartplug_energy_controller-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartplug_energy_controller-0.0.2.tar", max compression
+gzip compressed data, was "smartplug_energy_controller-0.0.3.tar", max compression
```

## Comparing `smartplug_energy_controller-0.0.2.tar` & `smartplug_energy_controller-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2024-05-02 18:06:02.290017 smartplug_energy_controller-0.0.2/LICENSE
--rw-r--r--   0        0        0     4451 2024-05-02 18:06:02.290017 smartplug_energy_controller-0.0.2/README.md
--rw-r--r--   0        0        0      655 2024-05-02 18:06:02.290017 smartplug_energy_controller-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      511 2024-05-02 18:06:02.290017 smartplug_energy_controller-0.0.2/smartplug_energy_controller/__init__.py
--rw-r--r--   0        0        0     2794 2024-05-02 18:06:02.290017 smartplug_energy_controller-0.0.2/smartplug_energy_controller/app.py
--rw-r--r--   0        0        0     3946 2024-05-02 18:06:02.290017 smartplug_energy_controller-0.0.2/smartplug_energy_controller/plug_controller.py
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 smartplug_energy_controller-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4621 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/README.md
+-rw-r--r--   0        0        0      684 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      511 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/smartplug_energy_controller/__init__.py
+-rw-r--r--   0        0        0     2059 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/smartplug_energy_controller/app.py
+-rw-r--r--   0        0        0     4039 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/smartplug_energy_controller/plug_controller.py
+-rw-r--r--   0        0        0     5431 1970-01-01 00:00:00.000000 smartplug_energy_controller-0.0.3/PKG-INFO
```

### Comparing `smartplug_energy_controller-0.0.2/LICENSE` & `smartplug_energy_controller-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartplug_energy_controller-0.0.2/README.md` & `smartplug_energy_controller-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,19 +25,26 @@
 ```bash
 python3 -m pip install --upgrade pip setuptools
 ```
 5. Install smartplug-energy-controller
 ```bash
 pip install smartplug-energy-controller
 ```
-6. Provide environment variables. You can e.g. pass a .env file to smartplug-energy-controller via the option *--dotenv_path*. Or provide them by any other means (e.g. in your ~/.profile).
+6. Provide environment variables (e.g. in your ~/.profile).
 ```bash
 TAPO_PLUG_IP='192.168.x.x'
 TAPO_CONTROL_USER='your_user'
 TAPO_CONTROL_PASSWD='your_passwd'
+
+# Following values can be considered as parameters, but have to be provided as env variables 
+# (see: https://fastapi.tiangolo.com/advanced/settings/#create-the-settings-object)
+EVAL_COUNT=10
+EXPECTED_CONSUMPTION=100
+LOG_FILE='path_to_file'
+LOG_LEVEL=20
 ```
 
 ## Autostart after reboot and on failure ##
 Create a systemd service by opening the file */etc/systemd/system/smartplug_energy_controller.service* and copy paste the following contents. Replace User/Group/ExecStart accordingly. 
 ```bash
 [Unit]
 Description=smartplug_energy_controller
@@ -47,15 +54,19 @@
 [Service]
 Type=simple
 User=ubuntu
 Group=ubuntu
 UMask=002
 Restart=on-failure
 RestartSec=5s
-ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && python /home/ubuntu/smart_meter_py_env/lib/python3.11/site-packages/smartplug-energy-controller/app.py --logfile /home/ubuntu/plug_controller.log -vv > /dev/null"
+Environment="EVAL_COUNT=10"
+Environment="EXPECTED_CONSUMPTION=100"
+Environment="LOG_FILE=/home/ubuntu/plug_controller.log"
+Environment="LOG_LEVEL=20"
+ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && uvicorn smartplug_energy_controller.app:app > /dev/null"
 
 [Install]
 WantedBy=multi-user.target
 ```
 
 Now execute the following commands to enable autostart:
 ```bash
```

### Comparing `smartplug_energy_controller-0.0.2/smartplug_energy_controller/plug_controller.py` & `smartplug_energy_controller-0.0.3/smartplug_energy_controller/plug_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from abc import ABC, abstractmethod
 from typing import List, Any, Optional
 
 from plugp100.common.credentials import AuthCredential
 from plugp100.new.device_factory import connect, DeviceConnectConfiguration
 from plugp100.new.tapoplug import TapoPlug
 
+# TODO: use a redis timeseries db: https://redis.io/docs/latest/develop/data-types/timeseries/
 def _manage_rolling_list(list : List[Any], max_value_count : int, new_end_value : Any) -> List[Any]:
     if len(list) < max_value_count:
         return list+[new_end_value]
     else:
         return list[1:]+[new_end_value]
 
 class PlugController(ABC):
     def __init__(self, logger : Logger, watt_consumption_eval_count : int, expected_watt_consumption : float) -> None:
         self._logger=logger
         self._watt_consumption_eval_count=watt_consumption_eval_count
-        assert expected_watt_consumption >= 10
+        assert expected_watt_consumption >= 1
         self._expected_watt_consumption=expected_watt_consumption
         self._watt_consumption_values : List[float] = []
 
     @abstractmethod
     def reset(self) -> None:
         pass
 
@@ -45,15 +46,15 @@
         try:
             self._watt_consumption_values=_manage_rolling_list(self._watt_consumption_values, 
                                                             self._watt_consumption_eval_count, 
                                                             value)
 
             await self.update()
             if len(self._watt_consumption_values) == self._watt_consumption_eval_count:
-                consumption_threshold=self._expected_watt_consumption if self.is_on() else 10
+                consumption_threshold=self._expected_watt_consumption if self.is_on() else 1
                 values_less_threshold=[value for value in self._watt_consumption_values if value < consumption_threshold]
                 if len(values_less_threshold) > self._watt_consumption_eval_count/2:
                     await self.turn_on()
                 else:
                     await self.turn_off()
         except Exception as e:
             # Just log as warning since the plug could just be unconnected
```

### Comparing `smartplug_energy_controller-0.0.2/PKG-INFO` & `smartplug_energy_controller-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: smartplug_energy_controller
-Version: 0.0.2
+Version: 0.0.3
 Summary: Turning Tapo smartplug on/off depending on current electricity consumption
 Home-page: https://github.com/die-bauerei/smartplug-energy-controller
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fastapi (>=0.110.0,<0.111.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: plugp100 (>=5.1.3,<6.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: uvicorn (>=0.28.0,<0.29.0)
 Project-URL: Repository, https://github.com/die-bauerei/smartplug-energy-controller
 Description-Content-Type: text/markdown
 
 # smartplug-energy-controller
 
 A microservice to turn a smartplug on/off depending on current electricity consumption.
@@ -43,19 +44,26 @@
 ```bash
 python3 -m pip install --upgrade pip setuptools
 ```
 5. Install smartplug-energy-controller
 ```bash
 pip install smartplug-energy-controller
 ```
-6. Provide environment variables. You can e.g. pass a .env file to smartplug-energy-controller via the option *--dotenv_path*. Or provide them by any other means (e.g. in your ~/.profile).
+6. Provide environment variables (e.g. in your ~/.profile).
 ```bash
 TAPO_PLUG_IP='192.168.x.x'
 TAPO_CONTROL_USER='your_user'
 TAPO_CONTROL_PASSWD='your_passwd'
+
+# Following values can be considered as parameters, but have to be provided as env variables 
+# (see: https://fastapi.tiangolo.com/advanced/settings/#create-the-settings-object)
+EVAL_COUNT=10
+EXPECTED_CONSUMPTION=100
+LOG_FILE='path_to_file'
+LOG_LEVEL=20
 ```
 
 ## Autostart after reboot and on failure ##
 Create a systemd service by opening the file */etc/systemd/system/smartplug_energy_controller.service* and copy paste the following contents. Replace User/Group/ExecStart accordingly. 
 ```bash
 [Unit]
 Description=smartplug_energy_controller
@@ -65,15 +73,19 @@
 [Service]
 Type=simple
 User=ubuntu
 Group=ubuntu
 UMask=002
 Restart=on-failure
 RestartSec=5s
-ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && python /home/ubuntu/smart_meter_py_env/lib/python3.11/site-packages/smartplug-energy-controller/app.py --logfile /home/ubuntu/plug_controller.log -vv > /dev/null"
+Environment="EVAL_COUNT=10"
+Environment="EXPECTED_CONSUMPTION=100"
+Environment="LOG_FILE=/home/ubuntu/plug_controller.log"
+Environment="LOG_LEVEL=20"
+ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && uvicorn smartplug_energy_controller.app:app > /dev/null"
 
 [Install]
 WantedBy=multi-user.target
 ```
 
 Now execute the following commands to enable autostart:
 ```bash
```

