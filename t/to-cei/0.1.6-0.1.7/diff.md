# Comparing `tmp/to_cei-0.1.6.tar.gz` & `tmp/to_cei-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_cei-0.1.6.tar", last modified: Wed Mar 15 10:25:22 2023, max compression
+gzip compressed data, was "to_cei-0.1.7.tar", last modified: Wed May 24 14:16:32 2023, max compression
```

## Comparing `to_cei-0.1.6.tar` & `to_cei-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-15 10:25:22.170204 to_cei-0.1.6/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    35149 2023-03-14 08:19:22.000000 to_cei-0.1.6/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)      889 2023-03-15 10:25:22.160204 to_cei-0.1.6/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      329 2023-03-14 08:19:22.000000 to_cei-0.1.6/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-03-15 10:25:22.170204 to_cei-0.1.6/setup.cfg
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1012 2023-03-15 08:53:37.000000 to_cei-0.1.6/setup.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-15 10:25:22.150204 to_cei-0.1.6/test/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    49595 2023-03-15 09:53:49.000000 to_cei-0.1.6/test/test_charter.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1139 2023-03-15 10:08:46.000000 to_cei-0.1.6/test/test_charter_group.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      699 2023-03-14 08:19:22.000000 to_cei-0.1.6/test/test_helpers.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     2989 2023-03-14 08:19:22.000000 to_cei-0.1.6/test/test_seal.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      287 2023-03-14 08:19:22.000000 to_cei-0.1.6/test/test_validator.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-15 10:25:22.160204 to_cei-0.1.6/to_cei/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    40492 2023-03-15 10:20:20.000000 to_cei-0.1.6/to_cei/charter.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     2425 2023-03-15 10:19:53.000000 to_cei-0.1.6/to_cei/charter_group.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      594 2023-03-15 09:47:31.000000 to_cei-0.1.6/to_cei/config.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      815 2023-03-14 08:19:22.000000 to_cei-0.1.6/to_cei/filecache.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     2114 2023-03-14 08:19:22.000000 to_cei-0.1.6/to_cei/helpers.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3886 2023-03-14 08:19:22.000000 to_cei-0.1.6/to_cei/seal.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      570 2023-03-15 06:51:27.000000 to_cei-0.1.6/to_cei/validator.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1854 2023-03-15 10:21:15.000000 to_cei-0.1.6/to_cei/xml_assembler.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-15 10:25:22.160204 to_cei-0.1.6/to_cei.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      889 2023-03-15 10:25:22.000000 to_cei-0.1.6/to_cei.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      441 2023-03-15 10:25:22.000000 to_cei-0.1.6/to_cei.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-03-15 10:25:22.000000 to_cei-0.1.6/to_cei.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       32 2023-03-15 10:25:22.000000 to_cei-0.1.6/to_cei.egg-info/requires.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        7 2023-03-15 10:25:22.000000 to_cei-0.1.6/to_cei.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-24 14:16:32.537151 to_cei-0.1.7/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35149 2023-03-15 11:24:38.000000 to_cei-0.1.7/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      889 2023-05-24 14:16:32.537151 to_cei-0.1.7/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      329 2023-03-15 11:24:38.000000 to_cei-0.1.7/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-24 14:16:32.537151 to_cei-0.1.7/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1012 2023-05-24 14:09:48.000000 to_cei-0.1.7/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-24 14:16:32.527151 to_cei-0.1.7/test/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    51108 2023-05-24 14:07:23.000000 to_cei-0.1.7/test/test_charter.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1139 2023-03-15 11:24:38.000000 to_cei-0.1.7/test/test_charter_group.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      699 2023-03-15 11:24:38.000000 to_cei-0.1.7/test/test_helpers.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2989 2023-03-15 11:24:38.000000 to_cei-0.1.7/test/test_seal.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      287 2023-03-15 11:24:38.000000 to_cei-0.1.7/test/test_validator.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-24 14:16:32.537151 to_cei-0.1.7/to_cei/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42280 2023-05-24 14:08:52.000000 to_cei-0.1.7/to_cei/charter.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2425 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/charter_group.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      594 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/config.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      815 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/filecache.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2114 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/helpers.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3886 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/seal.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      570 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/validator.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1854 2023-03-15 11:24:38.000000 to_cei-0.1.7/to_cei/xml_assembler.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-24 14:16:32.537151 to_cei-0.1.7/to_cei.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      889 2023-05-24 14:16:32.000000 to_cei-0.1.7/to_cei.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      441 2023-05-24 14:16:32.000000 to_cei-0.1.7/to_cei.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-24 14:16:32.000000 to_cei-0.1.7/to_cei.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       32 2023-05-24 14:16:32.000000 to_cei-0.1.7/to_cei.egg-info/requires.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        7 2023-05-24 14:16:32.000000 to_cei-0.1.7/to_cei.egg-info/top_level.txt
```

### Comparing `to_cei-0.1.6/LICENSE` & `to_cei-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/PKG-INFO` & `to_cei-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to_cei
-Version: 0.1.6
+Version: 0.1.7
 Summary: to-CEI
 Home-page: https://github.com/icaruseu/to-cei
 Author: Daniel Jeller
 Author-email: it@icar-us.eu
 License: GPL 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `to_cei-0.1.6/setup.py` & `to_cei-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(path.join(pwd, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="to_cei",
-    version="0.1.6",
+    version="0.1.7",
     description="to-CEI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/icaruseu/to-cei",
     author="Daniel Jeller",
     author_email="it@icar-us.eu",
     license="GPL 3.0",
```

### Comparing `to_cei-0.1.6/test/test_charter.py` & `to_cei-0.1.7/test/test_charter.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,50 @@
     assert charter.date == "unknown"
     assert charter.date_value == None
     date_xml = xps(charter, "/cei:text/cei:body/cei:chDesc/cei:issued/cei:date")
     assert date_xml.text == "unknown"
     assert date_xml.get("value") == NO_DATE_VALUE
 
 
+def test_has_correct_date_with_99_as_month():
+    charter = Charter(id_text="1", date_value="14009905")
+    assert charter.date_value == (
+        Time("1400-01-01", format="isot", scale="ut1").ymdhms,
+        Time("1400-12-31", format="isot", scale="ut1").ymdhms,
+    )
+    date_xml = xps(charter, "/cei:text/cei:body/cei:chDesc/cei:issued/cei:dateRange")
+    assert date_xml.text == "+01400-01-01 - +01400-12-31"
+    assert date_xml.get("from") == "14000101"
+    assert date_xml.get("to") == "14001231"
+
+
+def test_has_correct_date_with_99_as_day():
+    charter = Charter(id_text="1", date_value="14000299")
+    assert charter.date_value == (
+        Time("1400-02-01", format="isot", scale="ut1").ymdhms,
+        Time("1400-02-28", format="isot", scale="ut1").ymdhms,
+    )
+    date_xml = xps(charter, "/cei:text/cei:body/cei:chDesc/cei:issued/cei:dateRange")
+    assert date_xml.text == "+01400-02-01 - +01400-02-28"
+    assert date_xml.get("from") == "14000201"
+    assert date_xml.get("to") == "14000228"
+
+
+def test_has_correct_leap_year_date_with_99_as_day():
+    charter = Charter(id_text="1", date_value="14040299")
+    assert charter.date_value == (
+        Time("1404-02-01", format="isot", scale="ut1"),
+        Time("1404-02-29", format="isot", scale="ut1"),
+    )
+    date_xml = xps(charter, "/cei:text/cei:body/cei:chDesc/cei:issued/cei:dateRange")
+    assert date_xml.text == "+01404-02-01 - +01404-02-29"
+    assert date_xml.get("from") == "14040201"
+    assert date_xml.get("to") == "14040229"
+
+
 def test_has_correct_date_range_with_datetime():
     charter = Charter(
         id_text="1",
         date="1300",
         date_value=(datetime(1300, 1, 1), datetime(1300, 12, 31)),
     )
     assert charter.date == "1300"
```

### Comparing `to_cei-0.1.6/test/test_charter_group.py` & `to_cei-0.1.7/test/test_charter_group.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/test/test_helpers.py` & `to_cei-0.1.7/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/test/test_seal.py` & `to_cei-0.1.7/test/test_seal.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/charter.py` & `to_cei-0.1.7/to_cei/charter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import calendar
 import re
 from datetime import datetime
 from typing import List, Optional, Tuple
 from urllib.parse import quote
 
 from astropy.time import Time
 from lxml import etree
@@ -40,15 +41,15 @@
     return "{year}{month}{day}".format(
         year=str(year).zfill(3) if year >= 0 else "-" + str(year * -1).zfill(3),
         month=str(month).zfill(2),
         day=str(day).zfill(2),
     )
 
 
-def mom_date_to_time(value: str) -> Time:
+def mom_date_to_time(value: str) -> Time | Tuple[Time, Time]:
     """Converts a mom-compatible date string into an astropy.Time object if possible.
 
     Args:
         value (str): A mom-compatible date string in the form of -?[129]?[0-9][0-9][0-9][019][0-9][01239][0-9]
 
     Returns:
         A astropy.Time object
@@ -65,21 +66,69 @@
         raise ValueError("Invalid year in mom date value: {}".format(year))
     month = match.group("month")
     if not isinstance(month, str):
         raise ValueError("Invalid month in mom date value: {}".format(month))
     day = match.group("day")
     if not isinstance(day, str):
         raise ValueError("Invalid day in mom date value: {}".format(day))
+    if month == "99":
+        return (
+            Time(
+                {"year": int(year), "month": 1, "day": 1},
+                format="ymdhms",
+                scale="ut1",
+            ),
+            Time(
+                {
+                    "year": int(year),
+                    "month": 12,
+                    "day": 31,
+                },
+                format="ymdhms",
+                scale="ut1",
+            ),
+        )
+    if day == "99":
+        return (
+            Time(
+                {"year": int(year), "month": int(month), "day": 1},
+                format="ymdhms",
+                scale="ut1",
+            ),
+            Time(
+                {
+                    "year": int(year),
+                    "month": int(month),
+                    "day": calendar.monthrange(int(year), int(month))[1],
+                },
+                format="ymdhms",
+                scale="ut1",
+            ),
+        )
     return Time(
         {"year": int(year), "month": int(month), "day": int(day)},
         format="ymdhms",
         scale="ut1",
     )
 
 
+def extract_time(time: Time | Tuple[Time, Time]) -> Time:
+    """Extract time from date
+    Args:
+    time (Time | Tuple[Time, Time])
+
+    Returns:
+        The first date if a tuple is provided, the date if a date is provided.
+    """
+    if isinstance(time, Tuple):
+        return time[0]
+    else:
+        return time
+
+
 def string_to_time(value: str | Tuple[str, str]) -> Time | Tuple[Time, Time]:
     """Converts a single date string or a tuple of date strings to a matching single or tuple astropy.Time object.
 
     Args:
         value (str | Tuple[str, str]): A single or tuple of date strings. Can be either an iso-compatible or a mom-ca compatible date string.
 
     Returns:
@@ -99,15 +148,23 @@
                 Time(value[0], format="isot", scale="ut1"),
                 Time(value[1], format="isot", scale="ut1"),
             )
         )
     # Direct conversion not possible, try to convert mom date strings
     except Exception:
         if isinstance(value, Tuple):
-            return (mom_date_to_time(value[0]), mom_date_to_time(value[1]))
+            try:
+                return (
+                    extract_time(mom_date_to_time(value[0])),
+                    extract_time(mom_date_to_time(value[1])),
+                )
+            except Exception:
+                raise ValueError(
+                    "Failed to transform mom string to Time: '{}'".format(value)
+                )
         else:
             return mom_date_to_time(value)
 
 
 class Charter(XmlAssembler):
     _abstract: Optional[str | etree._Element] = None
     _abstract_sources: List[str] = []
@@ -194,17 +251,17 @@
             id_text: The human readable id of the charter. If id_norm is not present, id_text will be used in a normalized form. If it is missing or empty, an exception will be raised.
             abstract: The abstract either as a simple text or a complete cei:abstract etree._Element.
             abstract_sources: The bibliography source or sources for the abstract.
             archive: The name of the archive that owns the original charter.
             chancellary_remarks: Chancellary remarks as a single text or list of texts.
             comments: Diplomatic commentary as text or list of texts.
             condition: A description of the charter's condition in text form.
-            date: The date the charter was issued at either as text to use when converting to CEI or a complete cei:date or cei:dateRange etree._Element. If the date is given as an XML element, date_value needs to remain emptyself. Missing values will be constructed as having a date of "No date" in the XML.
+            date: The date the charter was issued at either as text to use when converting to CEI or a complete cei:date or cei:dateRange etree._Element. If the date is given as an XML element, date_value needs to remain empty. Missing values will be constructed as having a date of "No date" in the XML.
             date_quote: The charter's date in the original text either as text or a complete cel:quoteOriginaldatierung etree._Element object.
-            date_value: The actual date value in case the value in date is just a text and not an XML element. Can bei either an ISO date string, a MOM-compatible string, a python datetime object (can only be between years 1 and 9999) or an astropy Time object - or a tuple with two such values. If a single value is given, it is interpreted as an exact value, otherwise the two values will be used as from/to attributes of a cei:dateRange object. Missing values will be added to the xml as @value="99999999" to conform with the MOM data practices. When a date_value is added and date is an XML element, an exception is raised.
+            date_value: The actual date value in case the value in date is just a text and not an XML element. Can bei either an ISO date string, a MOM-compatible string, a python datetime object (can only be between years 1 and 9999) or an astropy Time object - or a tuple with two such values. If a single value is given, it is interpreted as an exact value, otherwise the two values will be used as from/to attributes of a cei:dateRange object. Missing values will be added to the xml as @value="99999999" to conform with the MOM data practices. When a date_value is added and date is an XML element, an exception is raised. Values with "99" for month or date will be converted to full year or month date ranges. For months "99" any day value after will be ignored and assumed to be unclear. This means, month "99" will always mean the whole given year.
             dimensions: The description of the physical dimensions of the charter as text.
             external_link: A link to an external representation of the charter as text.
             footnotes: Footnotes as text or list of texts.
             graphic_urls: A list of strings that represents the urls of various images representing the charter. Can bei either full urls or just the filenames of the image files, depending on the charter fond / collection settings.
             id_norm: A normalized id for the charter. It will be percent-encoded to ensure only valid characters are used. If it is ommitted, the normalized version of id_text will be used.
             id_old: An old, now obsolete identifier of the charter.
             index: A list of terms as texts or cei:index etree._Element objects to be included in the index.
```

### Comparing `to_cei-0.1.6/to_cei/charter_group.py` & `to_cei-0.1.7/to_cei/charter_group.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/config.py` & `to_cei-0.1.7/to_cei/config.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/filecache.py` & `to_cei-0.1.7/to_cei/filecache.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/helpers.py` & `to_cei-0.1.7/to_cei/helpers.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/seal.py` & `to_cei-0.1.7/to_cei/seal.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/validator.py` & `to_cei-0.1.7/to_cei/validator.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei/xml_assembler.py` & `to_cei-0.1.7/to_cei/xml_assembler.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.1.6/to_cei.egg-info/PKG-INFO` & `to_cei-0.1.7/to_cei.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cei
-Version: 0.1.6
+Version: 0.1.7
 Summary: to-CEI
 Home-page: https://github.com/icaruseu/to-cei
 Author: Daniel Jeller
 Author-email: it@icar-us.eu
 License: GPL 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

