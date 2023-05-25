# Comparing `tmp/vnfaker-0.0.4.tar.gz` & `tmp/vnfaker-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnfaker-0.0.4.tar", last modified: Thu May  4 09:54:59 2023, max compression
+gzip compressed data, was "vnfaker-0.0.5.tar", last modified: Thu May 25 17:27:48 2023, max compression
```

## Comparing `vnfaker-0.0.4.tar` & `vnfaker-0.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.605848 vnfaker-0.0.4/
--rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.4/LICENSE.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 09:54:59.605461 vnfaker-0.0.4/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.4/README.md
--rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-04 09:54:59.606043 vnfaker-0.0.4/setup.cfg
--rw-r--r--   0 ducquang   (501) admin       (80)     1033 2023-05-04 09:54:41.000000 vnfaker-0.0.4/setup.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.570328 vnfaker-0.0.4/src/
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.575322 vnfaker-0.0.4/src/vnfaker/
--rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.4/src/vnfaker/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     3102 2023-05-04 09:14:37.000000 vnfaker-0.0.4/src/vnfaker/commonUtils.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.579537 vnfaker-0.0.4/src/vnfaker/data/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.4/src/vnfaker/data/__init__.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.581898 vnfaker-0.0.4/src/vnfaker/data/company/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/company/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)    14530 2023-05-01 04:39:51.000000 vnfaker-0.0.4/src/vnfaker/data/company/company.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.584691 vnfaker-0.0.4/src/vnfaker/data/occupation/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/occupation/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.4/src/vnfaker/data/occupation/occupation.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.588488 vnfaker-0.0.4/src/vnfaker/data/person/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/person/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     1132 2023-05-01 04:04:14.000000 vnfaker-0.0.4/src/vnfaker/data/person/female.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-05-01 04:04:55.000000 vnfaker-0.0.4/src/vnfaker/data/person/female_middle.name
--rw-r--r--   0 ducquang   (501) admin       (80)      439 2023-05-02 10:33:11.000000 vnfaker-0.0.4/src/vnfaker/data/person/last.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1778 2023-05-01 03:46:35.000000 vnfaker-0.0.4/src/vnfaker/data/person/male.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1172 2023-05-01 04:09:43.000000 vnfaker-0.0.4/src/vnfaker/data/person/male_middle.name
--rw-r--r--   0 ducquang   (501) admin       (80)      363 2023-05-04 08:20:57.000000 vnfaker-0.0.4/src/vnfaker/data/person/religion.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.599377 vnfaker-0.0.4/src/vnfaker/data/provinces/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/provinces/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.4/src/vnfaker/data/provinces/flat-divisions.json
--rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.4/src/vnfaker/data/provinces/nested-divisions.json
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.603540 vnfaker-0.0.4/src/vnfaker/data/religion/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-05-04 08:18:11.000000 vnfaker-0.0.4/src/vnfaker/data/religion/__init__.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.604384 vnfaker-0.0.4/src/vnfaker/data/sentence/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.4/src/vnfaker/data/sentence/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.4/src/vnfaker/data/sentence/sentence.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     9674 2023-05-04 09:54:41.000000 vnfaker-0.0.4/src/vnfaker/generator.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.578824 vnfaker-0.0.4/src/vnfaker.egg-info/
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)      980 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/SOURCES.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/dependency_links.txt
--rw-r--r--   0 ducquang   (501) admin       (80)       32 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/requires.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/top_level.txt
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.465890 vnfaker-0.0.5/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.5/LICENSE.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-25 17:27:48.465399 vnfaker-0.0.5/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.5/README.md
+-rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-25 17:27:48.466050 vnfaker-0.0.5/setup.cfg
+-rw-r--r--   0 ducquang   (501) admin       (80)     1032 2023-05-25 17:26:49.000000 vnfaker-0.0.5/setup.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.429091 vnfaker-0.0.5/src/
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.433890 vnfaker-0.0.5/src/vnfaker/
+-rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.5/src/vnfaker/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     4609 2023-05-25 17:22:32.000000 vnfaker-0.0.5/src/vnfaker/commonUtils.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.436414 vnfaker-0.0.5/src/vnfaker/data/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.5/src/vnfaker/data/__init__.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.437117 vnfaker-0.0.5/src/vnfaker/data/company/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.5/src/vnfaker/data/company/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    14530 2023-05-01 04:39:51.000000 vnfaker-0.0.5/src/vnfaker/data/company/company.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.438343 vnfaker-0.0.5/src/vnfaker/data/occupation/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.5/src/vnfaker/data/occupation/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.5/src/vnfaker/data/occupation/occupation.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.445338 vnfaker-0.0.5/src/vnfaker/data/person/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.5/src/vnfaker/data/person/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     1132 2023-05-01 04:04:14.000000 vnfaker-0.0.5/src/vnfaker/data/person/female.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-05-01 04:04:55.000000 vnfaker-0.0.5/src/vnfaker/data/person/female_middle.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      439 2023-05-02 10:33:11.000000 vnfaker-0.0.5/src/vnfaker/data/person/last.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1778 2023-05-01 03:46:35.000000 vnfaker-0.0.5/src/vnfaker/data/person/male.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1172 2023-05-01 04:09:43.000000 vnfaker-0.0.5/src/vnfaker/data/person/male_middle.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      363 2023-05-04 08:20:57.000000 vnfaker-0.0.5/src/vnfaker/data/person/religion.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.453313 vnfaker-0.0.5/src/vnfaker/data/provinces/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.5/src/vnfaker/data/provinces/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)  4487951 2023-05-25 17:14:05.000000 vnfaker-0.0.5/src/vnfaker/data/provinces/flat-divisions.json
+-rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.5/src/vnfaker/data/provinces/nested-divisions.json
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.461432 vnfaker-0.0.5/src/vnfaker/data/religion/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-05-04 08:18:11.000000 vnfaker-0.0.5/src/vnfaker/data/religion/__init__.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.462241 vnfaker-0.0.5/src/vnfaker/data/sentence/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.5/src/vnfaker/data/sentence/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.5/src/vnfaker/data/sentence/sentence.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)    10357 2023-05-25 17:27:33.000000 vnfaker-0.0.5/src/vnfaker/generator.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-25 17:27:48.436036 vnfaker-0.0.5/src/vnfaker.egg-info/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-25 17:27:48.000000 vnfaker-0.0.5/src/vnfaker.egg-info/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)      980 2023-05-25 17:27:48.000000 vnfaker-0.0.5/src/vnfaker.egg-info/SOURCES.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-25 17:27:48.000000 vnfaker-0.0.5/src/vnfaker.egg-info/dependency_links.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)       32 2023-05-25 17:27:48.000000 vnfaker-0.0.5/src/vnfaker.egg-info/requires.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-25 17:27:48.000000 vnfaker-0.0.5/src/vnfaker.egg-info/top_level.txt
```

### Comparing `vnfaker-0.0.4/LICENSE.txt` & `vnfaker-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/PKG-INFO` & `vnfaker-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.4
+Version: 0.0.5
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.4/README.md` & `vnfaker-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/setup.py` & `vnfaker-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     README = fh.read()
 
 setuptools.setup(
     name="vnfaker",
-    version="0.0.4",
+    version="0.0.5",
     author="Phan Duc Quang",
     author_email="phanducquang07@gmail.com",
     description="vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/phanducquang/vnfaker",
     project_urls={
@@ -17,15 +17,15 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
-    package_data={"": ["data/*/*.name", "data/*/*.json", "data/*/*.txt"],},
+    package_data={"": ["data/*/*.name", "data/*/*.json", "data/*/*.txt"]},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
     install_requires=[
         "orjson>=3.8.10",
         "unidecode>=1.3.6"
     ],
 )
```

### Comparing `vnfaker-0.0.4/src/vnfaker/data/company/company.name` & `vnfaker-0.0.5/src/vnfaker/data/company/company.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/occupation/occupation.name` & `vnfaker-0.0.5/src/vnfaker/data/occupation/occupation.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/person/female.name` & `vnfaker-0.0.5/src/vnfaker/data/person/female.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/person/female_middle.name` & `vnfaker-0.0.5/src/vnfaker/data/person/female_middle.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/person/male.name` & `vnfaker-0.0.5/src/vnfaker/data/person/male.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/person/male_middle.name` & `vnfaker-0.0.5/src/vnfaker/data/person/male_middle.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/provinces/nested-divisions.json` & `vnfaker-0.0.5/src/vnfaker/data/provinces/nested-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/data/sentence/sentence.txt` & `vnfaker-0.0.5/src/vnfaker/data/sentence/sentence.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.4/src/vnfaker/generator.py` & `vnfaker-0.0.5/src/vnfaker/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from datetime import datetime
 from datetime import timedelta
 from datetime import tzinfo
 from typing import Optional
 
 from unidecode import unidecode
 
-from .commonUtils import CommonUtils, str_clean, change_year, date_time_ad
+from .commonUtils import CommonUtils, str_clean, change_year, date_time_ad, random_circumference_point
 
 
 class Generator:
 
     def __init__(self):
+        self.__radius_random = None
+        self.__province_long = None
+        self.__province_lat = None
         self.__religion_value = None
         self.__username_value = None
         self.__email_value = None
         self.__district_name = None
         self.__ward_name = None
         self.__province_name = None
         self.__known_location_value = None
@@ -168,23 +171,32 @@
             dob_temp = date_time_ad(tzinfo=tz_info, start_datetime=start_date, end_datetime=end_date).date()
 
             self.__birth_date = dob_temp if dob_temp != start_date else dob_temp + timedelta(days=1)
         if timestamp:
             return datetime.fromisoformat(self.__birth_date.isoformat()).timestamp() * 1000
         return self.__birth_date
 
-    def address(self):
+    def address(self, is_geo: bool = False):
         if self.__address_value is None:
             address_value_obj = random.choice(CommonUtils.address)
             self.__province_name = address_value_obj.get("province_name")
+            self.__province_lat = address_value_obj.get("province_lat")
+            self.__province_long = address_value_obj.get("province_long")
+            self.__radius_random = address_value_obj.get("radius_random")
             self.__ward_name = address_value_obj.get("ward_name")
             self.__district_name = address_value_obj.get("district_name")
             self.__address_value = "{}, {}, {}".format(self.__ward_name,
                                                        self.__district_name,
                                                        self.__province_name)
+        if is_geo:
+            center_point = {
+                "latitude": self.__province_lat,
+                "longitude": self.__province_long
+            }
+            return random_circumference_point(center_point, self.__radius_random)
         return self.__address_value
 
     def address_province(self):
         if self.__address_value is None:
             self.address()
         return self.__province_name
 
@@ -199,18 +211,19 @@
         return self.__ward_name
 
     def company(self):
         if self.__company_value is None:
             self.__company_value = random.choice(CommonUtils.companyNames)
         return self.__company_value
 
-    def known_location(self):
+    def known_location(self,
+                       number_location: int = 5):
         if self.__known_location_value is None:
             self.__known_location_value = [random.choice(CommonUtils.address).get("province_name") for _ in
-                                           range(random.randint(1, 5))]
+                                           range(random.randint(1, number_location))]
         return self.__known_location_value
 
     def occupation(self):
         if self.__occupation_value is None:
             self.__occupation_value = random.choice(CommonUtils.occupationNames)
         return self.__occupation_value
```

### Comparing `vnfaker-0.0.4/src/vnfaker.egg-info/PKG-INFO` & `vnfaker-0.0.5/src/vnfaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.4
+Version: 0.0.5
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.4/src/vnfaker.egg-info/SOURCES.txt` & `vnfaker-0.0.5/src/vnfaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

