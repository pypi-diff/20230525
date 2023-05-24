# Comparing `tmp/lidl-plus-0.2.3.tar.gz` & `tmp/lidl-plus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidl-plus-0.2.3.tar", last modified: Thu Jan  5 23:54:08 2023, max compression
+gzip compressed data, was "lidl-plus-0.2.4.tar", last modified: Mon Jan 16 22:43:40 2023, max compression
```

## Comparing `lidl-plus-0.2.3.tar` & `lidl-plus-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 23:54:08.792731 lidl-plus-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-01-05 23:54:08.792731 lidl-plus-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 23:54:08.792731 lidl-plus-0.2.3/lidl_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-01-05 23:54:08.000000 lidl-plus-0.2.3/lidl_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-05 23:54:08.000000 lidl-plus-0.2.3/lidl_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 23:54:08.000000 lidl-plus-0.2.3/lidl_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-05 23:54:08.000000 lidl-plus-0.2.3/lidl_plus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-05 23:54:08.000000 lidl-plus-0.2.3/lidl_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-05 23:54:08.000000 lidl-plus-0.2.3/lidl_plus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 23:54:08.792731 lidl-plus-0.2.3/lidlplus/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/lidlplus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4055 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/lidlplus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/lidlplus/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/lidlplus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 23:54:08.792731 lidl-plus-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-01-05 23:53:58.000000 lidl-plus-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:43:40.515983 lidl-plus-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-01-16 22:43:40.515983 lidl-plus-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:43:40.515983 lidl-plus-0.2.4/lidl_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-01-16 22:43:40.000000 lidl-plus-0.2.4/lidl_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-16 22:43:40.000000 lidl-plus-0.2.4/lidl_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 22:43:40.000000 lidl-plus-0.2.4/lidl_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-16 22:43:40.000000 lidl-plus-0.2.4/lidl_plus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-16 22:43:40.000000 lidl-plus-0.2.4/lidl_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-16 22:43:40.000000 lidl-plus-0.2.4/lidl_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:43:40.515983 lidl-plus-0.2.4/lidlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/lidlplus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4810 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/lidlplus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/lidlplus/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/lidlplus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 22:43:40.515983 lidl-plus-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-16 22:43:30.000000 lidl-plus-0.2.4/setup.py
```

### Comparing `lidl-plus-0.2.3/LICENCE` & `lidl-plus-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `lidl-plus-0.2.3/PKG-INFO` & `lidl-plus-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: lidl-plus
-Version: 0.2.3
+Version: 0.2.4
 Summary: Fetch receipts and more from Lidl Plus
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/lidl-plus
 Project-URL: PyPI, https://pypi.org/project/lidl-plus/
 Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lidl-plus-0.2.3/README.md` & `lidl-plus-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lidl-plus-0.2.3/lidl_plus.egg-info/PKG-INFO` & `lidl-plus-0.2.4/lidl_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: lidl-plus
-Version: 0.2.3
+Version: 0.2.4
 Summary: Fetch receipts and more from Lidl Plus
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/lidl-plus
 Project-URL: PyPI, https://pypi.org/project/lidl-plus/
 Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lidl-plus-0.2.3/lidlplus/__main__.py` & `lidl-plus-0.2.4/lidlplus/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #!/usr/bin/env python3
 """
 lidl plus command line tool
 """
 import argparse
 import json
+import os
 import sys
 from getpass import getpass
 from pathlib import Path
 
 if __name__ == "__main__":
     sys.path.insert(0, str(Path(__file__).parent.parent))
 # pylint: disable=wrong-import-position
 from lidlplus import LidlPlusApi
-from lidlplus.exceptions import WebBrowserException, LoginError
+from lidlplus.exceptions import WebBrowserException, LoginError, LegalTermsException
 
 
 def get_arguments():
     """Get parsed arguments."""
     parser = argparse.ArgumentParser(description="Lidl Plus api")
     parser.add_argument("-c", "--country", help="country (DE, EN, FR, IT, ...)")
     parser.add_argument("-l", "--language", help="language (de, be, nl, at, ...)")
     parser.add_argument("-u", "--user", help="Lidl Plus login user")
     parser.add_argument("-p", "--password", help="Lidl Plus login password")
     parser.add_argument("--2fa", choices=["phone", "email"], default="phone", help="set 2fa method")
     parser.add_argument("-r", "--refresh-token", help="refresh token to authenticate")
+    parser.add_argument("--skip-verify", help="skip ssl verification", action="store_true")
+    parser.add_argument("--not-accept-legal-terms", help="Deny legal terms updates", action="store_true")
+    parser.add_argument("-d", "--debug", help="debug mode", action="store_true")
     subparser = parser.add_subparsers(title="commands", metavar="command", required=True)
     auth = subparser.add_parser("auth", help="authenticate and get refresh_token")
     auth.add_argument("auth", help="authenticate and get refresh_token", action="store_true")
     receipt = subparser.add_parser("receipt", help="last receipt as json")
     receipt.add_argument("receipt", help="last receipt as json", action="store_true")
     receipt.add_argument("-a", "--all", help="fetch all receipts", action="store_true")
     return vars(parser.parse_args())
@@ -48,31 +52,45 @@
             "You also need google chrome to be installed."
         )
         sys.exit(1)
 
 
 def lidl_plus_login(args):
     """handle authentication"""
+    if not args.get("refresh_token"):
+        check_auth()
+    if args.get("skip_verify"):
+        os.environ["WDM_SSL_VERIFY"] = "0"
+        os.environ["CURL_CA_BUNDLE"] = ""
     language = args.get("language") or input("Enter your language (DE, EN, ...): ")
     country = args.get("country") or input("Enter your country (de, at, ...): ")
     if args.get("refresh_token"):
         return LidlPlusApi(language, country, args.get("refresh_token"))
-    username = args.get("username") or input("Enter your lidl plus username (phone number): ")
+    username = args.get("user") or input("Enter your lidl plus username (phone number): ")
     password = args.get("password") or getpass("Enter your lidl plus password: ")
-    check_auth()
     lidl_plus = LidlPlusApi(language, country)
     try:
         text = f"Enter the verify code you received via {args['2fa']}: "
-        lidl_plus.login(username, password, verify_token_func=lambda: input(text), verify_mode=args["2fa"])
+        lidl_plus.login(
+            username,
+            password,
+            verify_token_func=lambda: input(text),
+            verify_mode=args["2fa"],
+            headless=not args.get("debug"),
+            accept_legal_terms=not args.get("not_accept_legal_terms"),
+        )
     except WebBrowserException:
         print("Can't connect to web browser. Please install Chrome, Chromium or Firefox")
         sys.exit(101)
     except LoginError as error:
         print(f"Login failed - {error}")
         sys.exit(102)
+    except LegalTermsException as error:
+        print(f"Legal terms not accepted - {error}")
+        sys.exit(103)
     return lidl_plus
 
 
 def print_refresh_token(args):
     """pretty print refresh token"""
     lidl_plus = lidl_plus_login(args)
     length = len(token := lidl_plus.refresh_token) - len("refresh token")
```

### Comparing `lidl-plus-0.2.3/lidlplus/api.py` & `lidl-plus-0.2.4/lidlplus/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import html
 import logging
 import re
 from datetime import datetime, timedelta
 
 import requests
 
-from lidlplus.exceptions import WebBrowserException, LoginError
+from lidlplus.exceptions import WebBrowserException, LoginError, LegalTermsException
 
 try:
     from getuseragent import UserAgent
     from oic.oic import Client
     from oic.utils.authn.client import CLIENT_AUTHN_METHOD
     from selenium.webdriver.chrome.service import Service as ChromeService
     from selenium.webdriver.common.by import By
@@ -139,19 +139,30 @@
         args = {
             "Country": self._country,
             "language": f"{self._language}-{self._country}",
         }
         params = "&".join([f"{key}={value}" for key, value in args.items()])
         return f"{self._register_oauth_client()}&{params}"
 
-    def _parse_code(self, all_request):
-        for request in reversed(all_request):
+    @staticmethod
+    def _accept_legal_terms(browser, wait, accept=True):
+        wait.until(expected_conditions.visibility_of_element_located((By.ID, "checkbox_Accepted"))).click()
+        if not accept:
+            title = browser.find_element(By.TAG_NAME, "h2").text
+            raise LegalTermsException(title)
+        browser.find_element(By.TAG_NAME, "button").click()
+
+    def _parse_code(self, browser, wait, accept_legal_terms=True):
+        for request in reversed(browser.requests):
             if f"{self._AUTH_API}/connect" not in request.url:
                 continue
             location = request.response.headers.get("Location", "")
+            if "legalTerms" in location:
+                self._accept_legal_terms(browser, wait, accept=accept_legal_terms)
+                return self._parse_code(browser, wait, False)
             if code := re.findall("code=([0-9A-F]+)", location):
                 return code[0]
         return ""
 
     def _click(self, browser, button, request=""):
         del browser.requests
         browser.backend.storage.clear_requests()
@@ -194,15 +205,15 @@
         self._click(browser, (By.ID, "button_btn_submit_email"))
         self._click(browser, (By.ID, "button_btn_submit_email"), request=f"{self._AUTH_API}/api/phone/exists.*")
         wait.until(expected_conditions.element_to_be_clickable((By.ID, "field_Password"))).send_keys(password)
         self._click(browser, (By.ID, "button_submit"))
         self._check_login_error(browser)
         self._check_2fa_auth(browser, wait, kwargs.get("verify_mode", "phone"), kwargs.get("verify_token_func"))
         browser.wait_for_request(f"{self._AUTH_API}/connect.*")
-        code = self._parse_code(browser.requests)
+        code = self._parse_code(browser, wait, accept_legal_terms=kwargs.get("accept_legal_terms", True))
         self._authorization_code(code)
 
     def _default_headers(self):
         if (not self._token and self._refresh_token) or datetime.utcnow() >= self._expires:
             self._renew_token()
         if not self._token:
             raise Exception("You need to login!")
```

### Comparing `lidl-plus-0.2.3/setup.py` & `lidl-plus-0.2.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lidl-plus",
-    version="0.2.3",
+    version="0.2.4",
     author="Andre Basche",
     description="Fetch receipts and more from Lidl Plus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/lidl-plus",
         "PyPI": "https://pypi.org/project/lidl-plus/",
     },
     license="MIT",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

