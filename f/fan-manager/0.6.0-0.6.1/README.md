# Comparing `tmp/fan_manager-0.6.0-py2.py3-none-any.whl.zip` & `tmp/fan_manager-0.6.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5640 bytes, number of entries: 9
--rw-r--r--  2.0 unx      320 b- defN 23-Oct-15 15:19 fan_manager/__init__.py
--rw-r--r--  2.0 unx     5763 b- defN 23-Oct-15 15:19 fan_manager/fan_manager.py
--rw-r--r--  2.0 unx      116 b- defN 23-Oct-28 03:24 fan_manager/version.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-28 03:24 fan_manager-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4778 b- defN 23-Oct-28 03:24 fan_manager-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-28 03:24 fan_manager-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 23-Oct-28 03:24 fan_manager-0.6.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Oct-28 03:24 fan_manager-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      746 b- defN 23-Oct-28 03:24 fan_manager-0.6.0.dist-info/RECORD
-9 files, 12966 bytes uncompressed, 4346 bytes compressed:  66.5%
+Zip file size: 5682 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      356 b- defN 24-May-09 04:44 fan_manager/__init__.py
+-rw-r--r--  2.0 unx     5705 b- defN 24-May-09 04:44 fan_manager/fan_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 24-May-09 04:44 fan_manager/version.py
+-rw-r--r--  2.0 unx     1060 b- defN 24-May-09 04:45 fan_manager-0.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4771 b- defN 24-May-09 04:45 fan_manager-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-09 04:45 fan_manager-0.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-May-09 04:45 fan_manager-0.6.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-09 04:45 fan_manager-0.6.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      746 b- defN 24-May-09 04:45 fan_manager-0.6.1.dist-info/RECORD
+9 files, 12938 bytes uncompressed, 4388 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: fan_manager/fan_manager.py
 Comment: 
 
 Filename: fan_manager/version.py
 Comment: 
 
-Filename: fan_manager-0.6.0.dist-info/LICENSE
+Filename: fan_manager-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: fan_manager-0.6.0.dist-info/METADATA
+Filename: fan_manager-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: fan_manager-0.6.0.dist-info/WHEEL
+Filename: fan_manager-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: fan_manager-0.6.0.dist-info/entry_points.txt
+Filename: fan_manager-0.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: fan_manager-0.6.0.dist-info/top_level.txt
+Filename: fan_manager-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fan_manager-0.6.0.dist-info/RECORD
+Filename: fan_manager-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fan_manager/__init__.py

```diff
@@ -1,14 +1,17 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from fan_manager.version import __version__, __author__, __credits__
 from fan_manager.fan_manager import main, fan_manager
+
 """
 fan-manager
 
 Manager your Dell PowerEdge Fan Speed with this handy tool!
 """
 
 __version__ = __version__
 __author__ = __author__
 __credits__ = __credits__
+
+__all__ = ["main", "fan_manager"]
```

## fan_manager/fan_manager.py

```diff
@@ -4,169 +4,184 @@
 import os
 import sys
 import getopt
 import json
 import time
 
 
-def get_core_temp(cpus, sensors):
+def get_core_temp(cpus, sensors) -> int:
     highest_temp = 0
     highest_core = 0
     highest_cpu = ""
     cores = 0
     temp_cpu = 0
     for cpu in cpus:
         if cpu in sensors:
             for key in sensors[cpu].keys():
-                if 'Core' in key:
+                if "Core" in key:
                     cores = cores + 1
                     for temp_key in sensors[cpu][key].keys():
-                        if '_input' in temp_key:
+                        if "_input" in temp_key:
                             temp_cpu = sensors[cpu][key][temp_key]
                             if temp_cpu > highest_temp:
                                 highest_temp = temp_cpu
                                 highest_core = cores
                                 highest_cpu = cpu
             temp_cpu = highest_temp
-    print(f"Highest \n\tCPU: {highest_cpu} \n\tCore: {highest_core} \n\tTemperature: {highest_temp}")
+    print(
+        f"Highest \n\tCPU: {highest_cpu} \n\tCore: {highest_core} \n\tTemperature: {highest_temp}"
+    )
     return temp_cpu
 
 
-def get_temp():
-    sensors = json.loads(os.popen('sensors -j').read())
-    cpus = ['coretemp-isa-0000', 'coretemp-isa-0001']
+def get_temp() -> int:
+    sensors = json.loads(os.popen("sensors -j").read())
+    cpus = ["coretemp-isa-0000", "coretemp-isa-0001"]
     temp_cpu = get_core_temp(cpus, sensors)
-    print(f'Current Temperature: {temp_cpu}')
+    print(f"Current Temperature: {temp_cpu}")
     return temp_cpu
 
 
 def set_fan(fan_level: int):
     # manual fan control
-    cmd = f"ipmitool raw 0x30 0x30 0x01 0x00"
+    cmd = "ipmitool raw 0x30 0x30 0x01 0x00"
     os.system(cmd)
     # set fan level
     cmd = f"ipmitool raw 0x30 0x30 0x02 0xff {hex(fan_level)}"
     os.system(cmd)
 
 
-def run_service(temperature_poll_rate: int = 24, minimum_fan_speed: int = 5, maximum_fan_speed: int = 100,
-                minimum_temperature: int = 50, maximum_temperature: int = 80, temperature_power: int = 5):
+def run_service(
+    temperature_poll_rate: int = 24,
+    minimum_fan_speed: int = 5,
+    maximum_fan_speed: int = 100,
+    minimum_temperature: int = 50,
+    maximum_temperature: int = 80,
+    temperature_power: int = 5,
+):
     while True:
         cpu_temperature = get_temp()
-        x = min(1, max(0, (cpu_temperature - minimum_temperature) / (maximum_temperature - minimum_temperature)))
+        x = min(
+            1,
+            max(
+                0,
+                (cpu_temperature - minimum_temperature)
+                / (maximum_temperature - minimum_temperature),
+            ),
+        )
         fan_level = int(
             min(
                 maximum_fan_speed,
-                max(minimum_fan_speed,
-                    pow(x, temperature_power) * (maximum_fan_speed - minimum_fan_speed) + minimum_fan_speed)
+                max(
+                    minimum_fan_speed,
+                    pow(x, temperature_power) * (maximum_fan_speed - minimum_fan_speed)
+                    + minimum_fan_speed,
+                ),
             )
         )
         set_fan(fan_level)
         time.sleep(temperature_poll_rate)
 
 
 def usage():
-    print(f"Usage: \n"
-          f"-h | --help      [ See usage for fan-speed ]\n"
-          f"-i | --intensity [ Intensity of Fan Speed - Scales Logarithmically (0-10) ]\n"
-          f"-c | --cold      [ Minimum Temperature for Fan Speed (40-90) ]\n"
-          f"-w | --warm      [ Maximum Temperature for Fan Speed (40-90) ]\n"          
-          f"-s | --slow      [ Minimum Fan Speed (0-100) ]\n"
-          f"-f | --fast      [ Maximum Fan Speed (0-100) ]\n"
-          f"-p | --poll-rate [ Poll Rate for CPU Temperature in Seconds (1-300) ]\n"
-          f"\nExample: \n\t"
-          f"fan-manager --intensity 5 --cold 50 --warm 80 --slow 5 --fast 100 --poll-rate 24\n")
+    print(
+        "Usage: \n"
+        "-h | --help      [ See usage for fan-speed ]\n"
+        "-i | --intensity [ Intensity of Fan Speed - Scales Logarithmically (0-10) ]\n"
+        "-c | --cold      [ Minimum Temperature for Fan Speed (40-90) ]\n"
+        "-w | --warm      [ Maximum Temperature for Fan Speed (40-90) ]\n"
+        "-s | --slow      [ Minimum Fan Speed (0-100) ]\n"
+        "-f | --fast      [ Maximum Fan Speed (0-100) ]\n"
+        "-p | --poll-rate [ Poll Rate for CPU Temperature in Seconds (1-300) ]\n"
+        "\nExample: \n\t"
+        "fan-manager --intensity 5 --cold 50 --warm 80 --slow 5 --fast 100 --poll-rate 24\n"
+    )
 
 
 def fan_manager(argv):
     temperature_poll_rate = 24
     minimum_fan_speed = 5
     maximum_fan_speed = 100
 
     minimum_temperature = 50
     maximum_temperature = 80
 
     temperature_power = 5
 
     try:
-        opts, args = getopt.getopt(argv, "hi:c:w:s:f:p:",
-                                   ["help", "intensity=", "cold=", "warm=", "slow=", "fast=", "poll-rate="])
+        opts, args = getopt.getopt(
+            argv,
+            "hi:c:w:s:f:p:",
+            ["help", "intensity=", "cold=", "warm=", "slow=", "fast=", "poll-rate="],
+        )
     except getopt.GetoptError:
         usage()
         sys.exit(2)
     for opt, arg in opts:
         if opt in ("-h", "--help"):
             usage()
             sys.exit()
         elif opt in ("-i", "--intensity"):
             try:
                 temperature_power = int(arg)
             except Exception as e:
-                print(f"Unable to parse input as integer: {arg}"
-                      f"Error: "
-                      f"{e}")
+                print(f"Unable to parse input as integer: {arg}" f"Error: " f"{e}")
                 usage()
                 sys.exit(2)
         elif opt in ("-c", "--cold"):
             try:
                 minimum_temperature = int(arg)
             except Exception as e:
-                print(f"Unable to parse input as integer: {arg}"
-                      f"Error: "
-                      f"{e}")
+                print(f"Unable to parse input as integer: {arg}" f"Error: " f"{e}")
                 usage()
                 sys.exit(2)
         elif opt in ("-w", "--warm"):
             try:
                 maximum_temperature = int(arg)
             except Exception as e:
-                print(f"Unable to parse input as integer: {arg}"
-                      f"Error: "
-                      f"{e}")
+                print(f"Unable to parse input as integer: {arg}" f"Error: " f"{e}")
                 usage()
                 sys.exit(2)
         elif opt in ("-s", "--slow"):
             try:
                 minimum_fan_speed = int(arg)
             except Exception as e:
-                print(f"Unable to parse input as integer: {arg}"
-                      f"Error: "
-                      f"{e}")
+                print(f"Unable to parse input as integer: {arg}" f"Error: " f"{e}")
                 usage()
                 sys.exit(2)
         elif opt in ("-f", "--fast"):
             try:
                 maximum_fan_speed = int(arg)
             except Exception as e:
-                print(f"Unable to parse input as integer: {arg}"
-                      f"Error: "
-                      f"{e}")
+                print(f"Unable to parse input as integer: {arg}" f"Error: " f"{e}")
                 usage()
                 sys.exit(2)
         elif opt in ("-p", "--poll-rate"):
             try:
                 temperature_poll_rate = int(arg)
             except Exception as e:
-                print(f"Unable to parse input as integer: {arg}"
-                      f"Error: "
-                      f"{e}")
+                print(f"Unable to parse input as integer: {arg}" f"Error: " f"{e}")
                 usage()
                 sys.exit(2)
 
-    run_service(temperature_poll_rate=temperature_poll_rate, minimum_fan_speed=minimum_fan_speed,
-                maximum_fan_speed=maximum_fan_speed, minimum_temperature=minimum_temperature,
-                maximum_temperature=maximum_temperature, temperature_power=temperature_power)
+    run_service(
+        temperature_poll_rate=temperature_poll_rate,
+        minimum_fan_speed=minimum_fan_speed,
+        maximum_fan_speed=maximum_fan_speed,
+        minimum_temperature=minimum_temperature,
+        maximum_temperature=maximum_temperature,
+        temperature_power=temperature_power,
+    )
 
 
 def main():
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     fan_manager(sys.argv[1:])
 
 
 if __name__ == "__main__":
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     fan_manager(sys.argv[1:])
-
```

## fan_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.6.0'
-__author__ = 'Audel Rouhi'
-__credits__ = 'Audel Rouhi'
+__version__ = '0.6.1'
+__author__ = "Audel Rouhi"
+__credits__ = "Audel Rouhi"
```

## Comparing `fan_manager-0.6.0.dist-info/LICENSE` & `fan_manager-0.6.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `fan_manager-0.6.0.dist-info/METADATA` & `fan_manager-0.6.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fan-manager
-Version: 0.6.0
+Version: 0.6.1
 Summary: Manager your Dell PowerEdge Fan Speed with this handy tool!
 Home-page: https://github.com/Knuckles-Team/fan-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/fan-manager)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/fan-manager)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/fan-manager)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/fan-manager)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/fan-manager)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/fan-manager)
 
-*Version: 0.6.0*
+*Version: 0.6.1*
 
 Manager your Dell PowerEdge Fan Speed with this handy tool!
 
 This repository is actively maintained - Contributions are welcome!
 
 Contribution Opportunities:
 - Increase support of Dell PowerEdge Devices
@@ -53,21 +53,21 @@
 - Support Non-Dell Devices
 
 <details>
   <summary><b>Usage:</b></summary>
 
 | Short Flag | Long Flag   | Description                                            |
 |------------|-------------|--------------------------------------------------------|
-| -h         | --help      | See usage for fan-manager                              | 
-| -i         | --intensity | Intensity of Fan Speed - Scales Logarithmically (0-10) | 
-| -c         | --cold      | Minimum Temperature for Fan Speed                      | 
-| -w         | --warm      | Maximum Temperature for Fan Speed                      | 
-| -s         | --slow      | Minimum Fan Speed                                      | 
-| -f         | --fast      | Maximum Fan Speed                                      | 
-| -p         | --poll-rate | Poll Rate for CPU Temperature in Seconds               | 
+| -h         | --help      | See usage for fan-manager                              |
+| -i         | --intensity | Intensity of Fan Speed - Scales Logarithmically (0-10) |
+| -c         | --cold      | Minimum Temperature for Fan Speed                      |
+| -w         | --warm      | Maximum Temperature for Fan Speed                      |
+| -s         | --slow      | Minimum Fan Speed                                      |
+| -f         | --fast      | Maximum Fan Speed                                      |
+| -p         | --poll-rate | Poll Rate for CPU Temperature in Seconds               |
 
 </details>
 
 <details>
   <summary><b>Example:</b></summary>
 
 Python
```

