# Comparing `tmp/pxgrid-api-0.2.4.tar.gz` & `tmp/pxgrid-api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgrid-api-0.2.4.tar", last modified: Wed May 24 16:12:44 2023, max compression
+gzip compressed data, was "pxgrid-api-0.2.5.tar", last modified: Thu May 25 14:57:41 2023, max compression
```

## Comparing `pxgrid-api-0.2.4.tar` & `pxgrid-api-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.636604 pxgrid-api-0.2.4/
--rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.4/LICENSE
--rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.4/MANIFEST.in
--rw-r--r--   0 vibobrov   (503) staff       (20)    29738 2023-05-24 16:12:44.636133 pxgrid-api-0.2.4/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)    16236 2023-05-19 19:04:16.000000 pxgrid-api-0.2.4/README.rst
--rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-24 16:12:35.000000 pxgrid-api-0.2.4/pyproject.toml
--rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-24 16:12:44.636758 pxgrid-api-0.2.4/setup.cfg
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.623376 pxgrid-api-0.2.4/src/
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.631039 pxgrid-api-0.2.4/src/pxapi/
--rw-r--r--   0 vibobrov   (503) staff       (20)      149 2023-05-24 16:10:42.000000 pxgrid-api-0.2.4/src/pxapi/__init__.py
--rwxr-xr-x   0 vibobrov   (503) staff       (20)    20351 2023-05-16 03:54:31.000000 pxgrid-api-0.2.4/src/pxapi/__main__.py
--rw-r--r--   0 vibobrov   (503) staff       (20)    29250 2023-05-24 16:09:22.000000 pxgrid-api-0.2.4/src/pxapi/pxapi.py
--rw-r--r--   0 vibobrov   (503) staff       (20)     1555 2023-05-16 13:17:07.000000 pxgrid-api-0.2.4/src/pxapi/stompframe.py
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.635150 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/
--rw-r--r--   0 vibobrov   (503) staff       (20)    29738 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/SOURCES.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/dependency_links.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/entry_points.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/requires.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/top_level.txt
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-25 14:57:41.860257 pxgrid-api-0.2.5/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.5/LICENSE
+-rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.5/MANIFEST.in
+-rw-r--r--   0 vibobrov   (503) staff       (20)      161 2023-05-24 16:51:09.000000 pxgrid-api-0.2.5/NOTICE
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29977 2023-05-25 14:57:41.859733 pxgrid-api-0.2.5/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)    16454 2023-05-24 18:48:27.000000 pxgrid-api-0.2.5/README.rst
+-rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-25 14:57:10.000000 pxgrid-api-0.2.5/pyproject.toml
+-rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-25 14:57:41.860467 pxgrid-api-0.2.5/setup.cfg
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-25 14:57:41.848298 pxgrid-api-0.2.5/src/
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-25 14:57:41.854302 pxgrid-api-0.2.5/src/pxapi/
+-rw-r--r--   0 vibobrov   (503) staff       (20)      149 2023-05-25 14:57:04.000000 pxgrid-api-0.2.5/src/pxapi/__init__.py
+-rwxr-xr-x   0 vibobrov   (503) staff       (20)    20351 2023-05-16 03:54:31.000000 pxgrid-api-0.2.5/src/pxapi/__main__.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29264 2023-05-25 14:56:38.000000 pxgrid-api-0.2.5/src/pxapi/pxapi.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)     1555 2023-05-16 13:17:07.000000 pxgrid-api-0.2.5/src/pxapi/stompframe.py
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-25 14:57:41.858597 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29977 2023-05-25 14:57:41.000000 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)      369 2023-05-25 14:57:41.000000 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-25 14:57:41.000000 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-25 14:57:41.000000 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/entry_points.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-25 14:57:41.000000 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/requires.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-25 14:57:41.000000 pxgrid-api-0.2.5/src/pxgrid_api.egg-info/top_level.txt
```

### Comparing `pxgrid-api-0.2.4/LICENSE` & `pxgrid-api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.4/PKG-INFO` & `pxgrid-api-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,15 +210,20 @@
 Keywords: pxgrid
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+License-File: NOTICE
 
+|Generic badge|
+
+.. |Generic badge| image:: https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg
+   :target: https://developer.cisco.com/codeexchange/github/repo/vbobrov/pxgrid-api
 
 Introduction
 ============
 
 This repo includes two components:
 - A python API library making it easier to interact with pxGrid services on ISE
 - Interactive CLI utility to interface with pxGrid without writing any code
```

### Comparing `pxgrid-api-0.2.4/README.rst` & `pxgrid-api-0.2.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+|Generic badge|
+
+.. |Generic badge| image:: https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg
+   :target: https://developer.cisco.com/codeexchange/github/repo/vbobrov/pxgrid-api
 
 Introduction
 ============
 
 This repo includes two components:
 - A python API library making it easier to interact with pxGrid services on ISE
 - Interactive CLI utility to interface with pxGrid without writing any code
```

### Comparing `pxgrid-api-0.2.4/pyproject.toml` & `pxgrid-api-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools","wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pxgrid-api"
-version = "0.2.4"
+version = "0.2.5"
 description = "pxGrid API library and command line tool"
 readme = "README.rst"
 authors = [{ name = "Viktor Bobrov", email = "vibobrov@cisco.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pxgrid-api-0.2.4/src/pxapi/__main__.py` & `pxgrid-api-0.2.5/src/pxapi/__main__.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.4/src/pxapi/pxapi.py` & `pxgrid-api-0.2.5/src/pxapi/pxapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         """Retrieve active session by IP Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/Session-Directory#post-restbaseurlgetsessionbyipaddress
 
         :param ip: endpoint IP Address
         :return: dict containing all sessions for the IP Address
         """
         self.__check_ip(ip)
-        return(self.__send_px_api(self.SERVICE_SESSION,"getSessionByIpAddress",{"ip":ip}))
+        return(self.__send_px_api(self.SERVICE_SESSION,"getSessionByIpAddress",{"ipAddress":ip}))
 
     def get_session_by_mac_address(self,mac):
         """Retrieve active session by MAC Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/Session-Directory#post-restbaseurlgetsessionbymacaddress
 
         :param mac: endpoint MAC Address
         :return: dict containing all sessions for the MAC Address
@@ -406,15 +406,15 @@
         """Apply ANC Policy by IP Address. Requires that the endpoint is connected to the network.\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlapplyendpointbyipaddress
 
         :param policyName: name of ANC Policy
         :param ip: IP Address of endpoint
         """
         self.__check_ip(ip)
-        return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointByIpAddress",{"policyName":policy,"ip":ip}))
+        return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointByIpAddress",{"policyName":policy,"ipAddress":ip}))
 
     def anc_apply_endpoint_policy(self,policy,mac,nas_ip):
         """Apply ANC Policy by MAC Address and NAS-IP-Address. Endpoint does not need to be connected to the network.\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlapplyendpointpolicy-since-ise-26p7-27p2-30
 
         :param policy: name of ANC Policy
         :param mac: MAC Address of endpoint
```

### Comparing `pxgrid-api-0.2.4/src/pxapi/stompframe.py` & `pxgrid-api-0.2.5/src/pxapi/stompframe.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.4/src/pxgrid_api.egg-info/PKG-INFO` & `pxgrid-api-0.2.5/src/pxgrid_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,15 +210,20 @@
 Keywords: pxgrid
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+License-File: NOTICE
 
+|Generic badge|
+
+.. |Generic badge| image:: https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg
+   :target: https://developer.cisco.com/codeexchange/github/repo/vbobrov/pxgrid-api
 
 Introduction
 ============
 
 This repo includes two components:
 - A python API library making it easier to interact with pxGrid services on ISE
 - Interactive CLI utility to interface with pxGrid without writing any code
```

