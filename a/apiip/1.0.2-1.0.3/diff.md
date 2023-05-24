# Comparing `tmp/apiip-1.0.2.tar.gz` & `tmp/apiip-1.0.3.tar.gz`

## Comparing `apiip-1.0.2.tar` & `apiip-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 apiip-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 apiip-1.0.2/src/apiip/__init__.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 apiip-1.0.2/LICENCE
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 apiip-1.0.2/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apiip-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 apiip-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 apiip-1.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 apiip-1.0.3/src/apiip/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 apiip-1.0.3/LICENCE
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 apiip-1.0.3/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apiip-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 apiip-1.0.3/PKG-INFO
```

### Comparing `apiip-1.0.2/src/apiip/__init__.py` & `apiip-1.0.3/src/apiip/__init__.py`

 * *Files identical despite different names*

### Comparing `apiip-1.0.2/LICENCE` & `apiip-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `apiip-1.0.2/README.md` & `apiip-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -81,24 +81,24 @@
   "continentCode": "NA",
   "continentName": "North America",
   "countryCode": "US",
   "countryName": "United States",
   "countryNameNative": "United States",
   "regionCode":"NY"
   "regionName":"New York"
-  "cityGeoNameId":5128581,
+  "cityGeoNameId": 5128581,
   "city": "New York",
   "postalCode": "10001",
   "latitude": 40.8271,
   "longitude": -73.9359,
   "capital": "Washington D.C.",
   "phoneCode": "1",
   "countryFlagEmoj": "🇺🇸",
   "countryFlagEmojUnicode": "U+1F1FA U+1F1F8",
-  "isEu": false,
+  "isEu": False,
   "borders": [
     "CAN",
     "MEX"
   ],
   "topLevelDomains": [
     ".us"
   ],
@@ -122,38 +122,38 @@
     "id": "America/New_York",
     "currentTime": "10/26/2021, 2:54:10 PM",
     "code": "EDT",
     "timeZoneName": "EDT",
     "utcOffset": -14400
   },
    "userAgent": {
-    "isMobile": false,
-    "isiPod": false,
-    "isTablet": false,
-    "isDesktop": true,
-    "isSmartTV": false,
-    "isRaspberry": false,
-    "isBot": false,
+    "isMobile": False,
+    "isiPod": False,
+    "isTablet": False,
+    "isDesktop": True,
+    "isSmartTV": False,
+    "isRaspberry": False,
+    "isBot": False,
     "browser": "Chrome",
     "browserVersion": "100.0.4896.127",
     "operatingSystem": "Windows 10.0",
     "platform": "Microsoft Windows",
     "source": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36"
   },
   "connection": {
     "asn": 12271,
     "isp": "Charter Communications Inc"
   },
   "security": {
-    "isProxy": false,
-    "isBogon": false,
-    "isTorExitNode": false,
-    "isCloud": false,
-    "isHosting": false,
-    "isSpamhaus": false,
+    "isProxy": False,
+    "isBogon": False,
+    "isTorExitNode": False,
+    "isCloud": False,
+    "isHosting": False,
+    "isSpamhaus": False,
     "suggestion": "allow",
     "network": "67.250.176.0/20"
   }
 }
 
 ```
```

### Comparing `apiip-1.0.2/pyproject.toml` & `apiip-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apiip"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="apiip", email="apiipnet.business@gmail.com" },
 ]
 description = "Official python package for apiip.net, it offers one of the leading IP to geolocation API, get the location of any IP with a world-class API serving city, region, country, lat/long data, etc."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `apiip-1.0.2/PKG-INFO` & `apiip-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiip
-Version: 1.0.2
+Version: 1.0.3
 Summary: Official python package for apiip.net, it offers one of the leading IP to geolocation API, get the location of any IP with a world-class API serving city, region, country, lat/long data, etc.
 Project-URL: Homepage, https://apiip.net
 Project-URL: Documentation, https://apiip.net/documentation
 Author-email: apiip <apiipnet.business@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -94,24 +94,24 @@
   "continentCode": "NA",
   "continentName": "North America",
   "countryCode": "US",
   "countryName": "United States",
   "countryNameNative": "United States",
   "regionCode":"NY"
   "regionName":"New York"
-  "cityGeoNameId":5128581,
+  "cityGeoNameId": 5128581,
   "city": "New York",
   "postalCode": "10001",
   "latitude": 40.8271,
   "longitude": -73.9359,
   "capital": "Washington D.C.",
   "phoneCode": "1",
   "countryFlagEmoj": "🇺🇸",
   "countryFlagEmojUnicode": "U+1F1FA U+1F1F8",
-  "isEu": false,
+  "isEu": False,
   "borders": [
     "CAN",
     "MEX"
   ],
   "topLevelDomains": [
     ".us"
   ],
@@ -135,38 +135,38 @@
     "id": "America/New_York",
     "currentTime": "10/26/2021, 2:54:10 PM",
     "code": "EDT",
     "timeZoneName": "EDT",
     "utcOffset": -14400
   },
    "userAgent": {
-    "isMobile": false,
-    "isiPod": false,
-    "isTablet": false,
-    "isDesktop": true,
-    "isSmartTV": false,
-    "isRaspberry": false,
-    "isBot": false,
+    "isMobile": False,
+    "isiPod": False,
+    "isTablet": False,
+    "isDesktop": True,
+    "isSmartTV": False,
+    "isRaspberry": False,
+    "isBot": False,
     "browser": "Chrome",
     "browserVersion": "100.0.4896.127",
     "operatingSystem": "Windows 10.0",
     "platform": "Microsoft Windows",
     "source": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36"
   },
   "connection": {
     "asn": 12271,
     "isp": "Charter Communications Inc"
   },
   "security": {
-    "isProxy": false,
-    "isBogon": false,
-    "isTorExitNode": false,
-    "isCloud": false,
-    "isHosting": false,
-    "isSpamhaus": false,
+    "isProxy": False,
+    "isBogon": False,
+    "isTorExitNode": False,
+    "isCloud": False,
+    "isHosting": False,
+    "isSpamhaus": False,
     "suggestion": "allow",
     "network": "67.250.176.0/20"
   }
 }
 
 ```
```

