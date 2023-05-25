# Comparing `tmp/keyauth-tech-0.0.2.tar.gz` & `tmp/keyauth-tech-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyauth-tech-0.0.2.tar", last modified: Wed May 24 11:27:01 2023, max compression
+gzip compressed data, was "keyauth-tech-0.0.3.tar", last modified: Thu May 25 15:16:22 2023, max compression
```

## Comparing `keyauth-tech-0.0.2.tar` & `keyauth-tech-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:27:01.348130 keyauth-tech-0.0.2/
--rw-r--r--   0 ecom       (502) staff       (20)       94 2023-05-24 11:26:55.000000 keyauth-tech-0.0.2/CHANGELOG.txt
--rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.2/LICENSE.txt
--rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.2/MANIFEST.in
--rw-r--r--   0 ecom       (502) staff       (20)      815 2023-05-24 11:27:01.347980 keyauth-tech-0.0.2/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      116 2023-05-24 11:09:48.000000 keyauth-tech-0.0.2/README.txt
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:27:01.347071 keyauth-tech-0.0.2/keyauth/
--rw-r--r--   0 ecom       (502) staff       (20)     2342 2023-05-24 11:03:49.000000 keyauth-tech-0.0.2/keyauth/__init__.py
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:27:01.347766 keyauth-tech-0.0.2/keyauth_tech.egg-info/
--rw-r--r--   0 ecom       (502) staff       (20)      815 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      264 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/SOURCES.txt
--rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/dependency_links.txt
--rw-r--r--   0 ecom       (502) staff       (20)       18 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/requires.txt
--rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/top_level.txt
--rw-r--r--   0 ecom       (502) staff       (20)     2102 2023-05-24 11:25:21.000000 keyauth-tech-0.0.2/req.txt
--rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-24 11:27:01.348170 keyauth-tech-0.0.2/setup.cfg
--rw-r--r--   0 ecom       (502) staff       (20)      811 2023-05-24 11:26:34.000000 keyauth-tech-0.0.2/setup.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-25 15:16:22.863857 keyauth-tech-0.0.3/
+-rw-r--r--   0 ecom       (502) staff       (20)       84 2023-05-25 15:15:38.000000 keyauth-tech-0.0.3/CHANGELOG.txt
+-rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.3/LICENSE.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.3/MANIFEST.in
+-rw-r--r--   0 ecom       (502) staff       (20)      805 2023-05-25 15:16:22.863722 keyauth-tech-0.0.3/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      116 2023-05-24 11:09:48.000000 keyauth-tech-0.0.3/README.txt
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-25 15:16:22.862862 keyauth-tech-0.0.3/keyauth/
+-rw-r--r--   0 ecom       (502) staff       (20)     2487 2023-05-25 15:13:23.000000 keyauth-tech-0.0.3/keyauth/__init__.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-25 15:16:22.863519 keyauth-tech-0.0.3/keyauth_tech.egg-info/
+-rw-r--r--   0 ecom       (502) staff       (20)      805 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      264 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/SOURCES.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/dependency_links.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       18 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/requires.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/top_level.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-25 15:16:22.863898 keyauth-tech-0.0.3/setup.cfg
+-rw-r--r--   0 ecom       (502) staff       (20)      811 2023-05-25 15:16:19.000000 keyauth-tech-0.0.3/setup.py
+-rw-r--r--   0 ecom       (502) staff       (20)      232 2023-05-24 11:31:31.000000 keyauth-tech-0.0.3/test.py
```

### Comparing `keyauth-tech-0.0.2/LICENSE.txt` & `keyauth-tech-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keyauth-tech-0.0.2/PKG-INFO` & `keyauth-tech-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyauth-tech
-Version: 0.0.2
+Version: 0.0.3
 Summary: An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 Home-page: https://keyauth.tech
 Author: Collin Stokes
 Author-email: rehan009a@outlook.com
 License: MIT
 Keywords: authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENSE.txt
 
 An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 
 Change Log
 ==========
 
-0.0.2 (24/05/2023)
+0.0.3 (25/05/2023)
 -------------------
-- Fixed Bugs & Issues Installing
+- Added Clear Function
```

### Comparing `keyauth-tech-0.0.2/keyauth/__init__.py` & `keyauth-tech-0.0.3/keyauth/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import subprocess
 import requests
 import platform
+import os
 from colorama import Fore, init
 
 init(autoreset=True)  # Automatically reset colorama color styles after they're printed
 
+def clear():
+    os.system('cls' if os.name == 'nt' else 'clear')
+
 class KeyAuth:
 
     def __init__(self, app_id, base_url="https://api.keyauth.tech/api/v1"):
         self.app_id = app_id
         self.auth_url = f"{base_url}/auth/{app_id}"
         self.license_url = f"{base_url}/license"
 
@@ -38,18 +42,21 @@
         json_response = response.json()
         if json_response.get('message') == 'Login Success' and json_response.get('status') == 'success':
             print(f"{Fore.GREEN}[+] Successfully authenticated!{Fore.RESET}")
             return True
         else:
             print(f"{Fore.RED}[!] HWID: {self.get_hwid()} is not authenticated!{Fore.RESET}")
             key = input(f"{Fore.RED}License Key: {Fore.RESET}")
+            clear()
             key_payload = {'license_key': key, 'hwid': self.get_hwid()}
             headers = {'x-app-id': self.app_id}
 
             key_response = requests.post(self.license_url, json=key_payload, headers=headers, timeout=100)
             license_response = key_response.json()
             if license_response.get('message') == 'License key is valid. HWID added.' and license_response.get('status') == 'success':
+                clear()
                 print(f"{Fore.GREEN}[+] Successfully authenticated!{Fore.RESET}")
                 return True
             else:
+                clear()
                 print(f"{Fore.RED}[!] Invalid License Key!{Fore.RESET}")
                 return False
```

### Comparing `keyauth-tech-0.0.2/keyauth_tech.egg-info/PKG-INFO` & `keyauth-tech-0.0.3/keyauth_tech.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyauth-tech
-Version: 0.0.2
+Version: 0.0.3
 Summary: An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 Home-page: https://keyauth.tech
 Author: Collin Stokes
 Author-email: rehan009a@outlook.com
 License: MIT
 Keywords: authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENSE.txt
 
 An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 
 Change Log
 ==========
 
-0.0.2 (24/05/2023)
+0.0.3 (25/05/2023)
 -------------------
-- Fixed Bugs & Issues Installing
+- Added Clear Function
```

### Comparing `keyauth-tech-0.0.2/setup.py` & `keyauth-tech-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='keyauth-tech',
-  version='0.0.2',
+  version='0.0.3',
   description='An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='https://keyauth.tech',  
   author='Collin Stokes',
   author_email='rehan009a@outlook.com',
   license='MIT', 
   classifiers=classifiers,
```

