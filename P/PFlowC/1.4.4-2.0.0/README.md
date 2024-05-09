# Comparing `tmp/PFlowC-1.4.4.tar.gz` & `tmp/PFlowC-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.4.4.tar", last modified: Sun Apr 28 10:53:40 2024, max compression
+gzip compressed data, was "PFlowC-2.0.0.tar", last modified: Thu May  9 11:26:58 2024, max compression
```

## Comparing `PFlowC-1.4.4.tar` & `PFlowC-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.470011 PFlowC-1.4.4/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.467629 PFlowC-1.4.4/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:53:34.000000 PFlowC-1.4.4/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     6067 2024-04-28 10:41:10.000000 PFlowC-1.4.4/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.4/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.468720 PFlowC-1.4.4/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.4/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.4/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.469148 PFlowC-1.4.4/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.4/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.4/PFlowC/utils/logger.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.468416 PFlowC-1.4.4/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2625 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      382 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/requires.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2625 2024-04-28 10:53:40.469822 PFlowC-1.4.4/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1665 2024-04-28 10:53:21.000000 PFlowC-1.4.4/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:53:40.470053 PFlowC-1.4.4/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1634 2024-04-28 10:53:29.000000 PFlowC-1.4.4/setup.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.469501 PFlowC-1.4.4/tests/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-1.4.4/tests/test-banner.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.153543 PFlowC-2.0.0/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.113946 PFlowC-2.0.0/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:53:34.000000 PFlowC-2.0.0/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3207 2024-05-09 03:46:04.000000 PFlowC-2.0.0/PFlowC/geo_proxy.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7872 2024-04-29 09:28:01.000000 PFlowC-2.0.0/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.0.0/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.115196 PFlowC-2.0.0/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.0.0/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.0.0/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.150308 PFlowC-2.0.0/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.0.0/PFlowC/utils/Country.mmdb
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.0.0/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.0.0/PFlowC/utils/logger.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2000 2024-04-30 09:01:33.000000 PFlowC-2.0.0/PFlowC/utils/net.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.114822 PFlowC-2.0.0/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2627 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      588 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2627 2024-05-09 11:26:58.153218 PFlowC-2.0.0/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1667 2024-04-28 10:54:57.000000 PFlowC-2.0.0/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-09 11:26:58.153607 PFlowC-2.0.0/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1702 2024-04-30 08:23:30.000000 PFlowC-2.0.0/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.152693 PFlowC-2.0.0/tests/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.0.0/tests/test-agent-service.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.0.0/tests/test-api.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.0.0/tests/test-banner.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.0.0/tests/test-dns-socket.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.0.0/tests/test-dnspython.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.0.0/tests/test-json-dump.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.0.0/tests/test-salary.py
```

### Comparing `PFlowC-1.4.4/PFlowC/proxy.py` & `PFlowC-2.0.0/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.4/PFlowC/proxy_helper/macosx.py` & `PFlowC-2.0.0/PFlowC/proxy_helper/macosx.py`

 * *Files 12% similar despite different names*

```diff
@@ -146,7 +146,46 @@
 
             cmd = ["/usr/sbin/networksetup", "-set" + proxy_type + "state", service, "off"]
             resp = subprocess.run(cmd, check=True)
             if resp.returncode != 0:
                 logging.error(f"执行{cmd}时发生异常!")
             else:
                 logging.info(f"网络[{service}]代理[{proxy_type}]关闭成功!")
+
+
+def set_bypass_domains(bypass_domains):
+    network_services = get_network_services()
+    logging.info(f"network services:{network_services}")
+    for service in network_services:
+        cmd = ["/usr/sbin/networksetup", "-setproxybypassdomains", service, *bypass_domains]
+        resp = subprocess.run(cmd)
+        if resp.returncode != 0:
+            logging.error(f"执行{cmd}时发生异常!")
+        logging.info(f"网络[{service}]配置代理成功!")
+
+    no_proxy_domains = ",".join(bypass_domains)
+    for env_rc_file in env_rc_files:
+        # 要编辑的文件路径
+        env_rc_fp = os.path.expanduser(f"~/{env_rc_file}")
+
+        # 检查并读取文件内容
+        if not os.path.isfile(env_rc_fp):
+            pass
+        else:
+            with open(env_rc_fp, "r+") as zshrc_file:
+                lines = zshrc_file.readlines()
+                updated_lines = []
+
+                # 查找并移除旧的代理设置
+                for line in lines:
+                    if not "no_proxy=" in line:
+                        updated_lines.append(line)
+
+                # 添加新的代理设置
+                updated_lines.append(f"export no_proxy=\"{no_proxy_domains}\"\n")
+
+                # 将更新后的行重写回文件
+                zshrc_file.seek(0)
+                zshrc_file.truncate()
+                zshrc_file.writelines(updated_lines)
+
+            logging.info(f"代理设置已在{env_rc_file}文件中更新，请运行 'source ~/{env_rc_file}' 以应用新的环境变量设置。")
```

### Comparing `PFlowC-1.4.4/PFlowC/utils/logger.py` & `PFlowC-2.0.0/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.4/PFlowC.egg-info/PKG-INFO` & `PFlowC-2.0.0/PFlowC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.4
+Version: 2.0.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,16 @@
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
 A net flow pilot in order to handle some proxy configuration automatically.
-Usage::
+
+Usage ::
 
     ██████╗ ███████╗██╗      ██████╗ ██╗    ██╗ ██████╗
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
```

### Comparing `PFlowC-1.4.4/PKG-INFO` & `PFlowC-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.4
+Version: 2.0.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,16 @@
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
 A net flow pilot in order to handle some proxy configuration automatically.
-Usage::
+
+Usage ::
 
     ██████╗ ███████╗██╗      ██████╗ ██╗    ██╗ ██████╗
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
```

### Comparing `PFlowC-1.4.4/README.rst` & `PFlowC-2.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
 A net flow pilot in order to handle some proxy configuration automatically.
-Usage::
+
+Usage ::
 
     ██████╗ ███████╗██╗      ██████╗ ██╗    ██╗ ██████╗
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
```

### Comparing `PFlowC-1.4.4/setup.py` & `PFlowC-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 except ImportError:
     from distutils.core import setup
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.4.4',
+    version='2.0.0',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=['colorlog', 'click'],
+    package_data={
+        'PFlowC.utils': ['Country.mmdb'],
+    },
     include_package_data=True,
     python_requires='>=3.7',
     long_description=long_description,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `PFlowC-1.4.4/tests/test-banner.py` & `PFlowC-2.0.0/tests/test-banner.py`

 * *Files identical despite different names*

