# Comparing `tmp/robotframework-bsnlibrary-1.0.0.tar.gz` & `tmp/robotframework-bsnlibrary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-bsnlibrary-1.0.0.tar", last modified: Sun Apr 26 15:13:07 2020, max compression
+gzip compressed data, was "robotframework-bsnlibrary-1.1.0.tar", last modified: Thu May 25 19:52:42 2023, max compression
```

## Comparing `robotframework-bsnlibrary-1.0.0.tar` & `robotframework-bsnlibrary-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/BSNLibrary/
--rw-rw-rw-   0        0        0    20737 2020-04-26 14:57:50.000000 robotframework-bsnlibrary-1.0.0/BSNLibrary/__init__.py
--rw-rw-rw-   0        0        0      511 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/BSNLibrary/exceptions.py
--rw-rw-rw-   0        0        0     4806 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3155 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/docs/
--rw-rw-rw-   0        0        0   147418 2020-04-26 15:05:08.000000 robotframework-bsnlibrary-1.0.0/docs/index.html
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/
--rw-rw-rw-   0        0        0     4806 2020-04-26 15:13:06.000000 robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      795 2020-04-26 15:13:06.000000 robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-26 15:13:06.000000 robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2020-04-26 15:13:06.000000 robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2020-04-26 15:13:06.000000 robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2159 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/tests/
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/
--rw-rw-rw-   0        0        0    16974 2020-04-26 12:04:00.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/1_Functional_tests.robot
--rw-rw-rw-   0        0        0    14905 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/2_Error_handling.robot
--rw-rw-rw-   0        0        0     4275 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/3_Demos.robot
--rw-rw-rw-   0        0        0    14292 2020-04-26 12:04:00.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/Resource.robot
--rw-rw-rw-   0        0        0      783 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/__init__.robot
-drwxrwxrwx   0        0        0        0 2020-04-26 15:13:07.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test_old_syntax/
--rw-rw-rw-   0        0        0    16914 2020-04-26 12:04:00.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test_old_syntax/1_Functional_tests.robot
--rw-rw-rw-   0        0        0    14810 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test_old_syntax/2_Error_handling.robot
--rw-rw-rw-   0        0        0     4258 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test_old_syntax/3_Demos.robot
--rw-rw-rw-   0        0        0    14248 2020-04-26 12:04:00.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test_old_syntax/Resource.robot
--rw-rw-rw-   0        0        0      773 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test_old_syntax/__init__.robot
+drwxrwxrwx   0        0        0        0 2023-05-25 19:52:42.467716 robotframework-bsnlibrary-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-25 19:52:42.409961 robotframework-bsnlibrary-1.1.0/BSNLibrary/
+-rw-rw-rw-   0        0        0    20725 2023-05-25 15:21:53.000000 robotframework-bsnlibrary-1.1.0/BSNLibrary/__init__.py
+-rw-rw-rw-   0        0        0      511 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.1.0/BSNLibrary/exceptions.py
+-rw-rw-rw-   0        0        0     1065 2023-05-25 17:07:45.000000 robotframework-bsnlibrary-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4192 2023-05-25 19:52:42.468716 robotframework-bsnlibrary-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3155 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 19:52:42.413304 robotframework-bsnlibrary-1.1.0/docs/
+-rw-rw-rw-   0        0        0   179746 2023-05-25 19:51:58.000000 robotframework-bsnlibrary-1.1.0/docs/index.html
+drwxrwxrwx   0        0        0        0 2023-05-25 19:52:42.434449 robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/
+-rw-rw-rw-   0        0        0     4192 2023-05-25 19:52:42.000000 robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-05-25 19:52:42.000000 robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 19:52:42.000000 robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 19:52:42.000000 robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 19:52:42.000000 robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-05-25 19:52:42.471133 robotframework-bsnlibrary-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1721 2023-05-25 15:29:38.000000 robotframework-bsnlibrary-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:52:42.389010 robotframework-bsnlibrary-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2023-05-25 19:52:42.464548 robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/
+-rw-rw-rw-   0        0        0    16974 2023-05-25 15:14:01.000000 robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/1_Functional_tests.robot
+-rw-rw-rw-   0        0        0    14905 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/2_Error_handling.robot
+-rw-rw-rw-   0        0        0     4275 2020-04-26 00:06:45.000000 robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/3_Demos.robot
+-rw-rw-rw-   0        0        0    14292 2020-04-26 12:04:00.000000 robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/Resource.robot
+-rw-rw-rw-   0        0        0      679 2023-05-25 15:44:53.000000 robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/__init__.robot
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `robotframework-bsnlibrary-1.0.0/BSNLibrary/__init__.py` & `robotframework-bsnlibrary-1.1.0/BSNLibrary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 [https://github.com/HaaiHenkie/bsnlibrary/releases|Release notes]
 
 Create date: 01-03-2020
 
 Author: Henk van den Akker
 
-License: GNU General Public License v3.0
+License: MIT License (Expat)
 
 = Scope of uniqueness and exclusion =
 `Generate BSN` will by default generate a unique BSN every time it is used throughout the test run. After using
 `Exclude BSNs` with a list of BSNs, `Generate BSN` will exclude those BSNs every time it is used until the end of the
 test run. These are the normal scopes for uniqueness and exclusion and they are suitable for most purposes. The
 following information is relevant for the few cases that need a smaller or larger scope.
 
@@ -136,15 +136,15 @@
 
 import random
 import textwrap
 from BSNLibrary import exceptions
 from robot.api import deco
 import logging
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 ROBOT_LIBRARY_SCOPE = 'GLOBAL'
 VALID_LENGTH = {6, 7, 8, 9}
 used_bsns = []
 excluded_bsns = []
 
 
 @deco.keyword('Generate BSN')
```

### Comparing `robotframework-bsnlibrary-1.0.0/PKG-INFO` & `robotframework-bsnlibrary-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 Metadata-Version: 2.1
 Name: robotframework-bsnlibrary
-Version: 1.0.0
+Version: 1.1.0
 Summary: Robot Framework library for generating BSNs (Dutch citizen service number)
 Home-page: https://github.com/HaaiHenkie/bsnlibrary
 Author: Henk van den Akker
 Author-email: haaihenkie@users.noreply.github.com
-License: GNU General Public License v3 (GPLv3)
+License: MIT License (Expat)
 Project-URL: Documentation, https://haaihenkie.github.io/bsnlibrary/
 Project-URL: Source, https://github.com/HaaiHenkie/bsnlibrary
 Project-URL: Tracker, https://github.com/HaaiHenkie/bsnlibrary/issues
-Description: # BSNLibrary for Robot Framework
-        
-        Robot Framework Library for generating a random BSN (Burger Service Nummer, i.e. a
-        Dutch citizen service number) for test purposes.
-        
-        A BSN is used in Netherlands to identify a person for government organisations, see
-        [this information of the Dutch government](https://www.government.nl/topics/personal-data/citizen-service-number-bsn).
-        The number consists of 9 digits and has to pass the eleven test.
-        
-        This test can be explained with the example 211551557. Each digit is multiplied with
-        its position and the results are added up together:
-        
-        ``(9*2) + (8*1) + (7*1) + (6*5) + (5*5) + (4*1) + (3*5) + (2*5) - (1*7) = 110``
-        
-        Note that the digit in position 1 is subtracted from the other results. The total
-        sum can be divided by 11, which means that this number has passed the eleven test.
-        
-        This library generates BSNs for test purposes in the sense that it generates random
-        9 digit numbers that pass the eleven test. By coincidence a generated number could
-        be a real person's BSN. Yet this library cannot violate such a person's privacy,
-        because it cannot tell you whether a number belongs to a real person or not, nor
-        will it provide you with any personal data related to a BSN. Obviously you should
-        only use this library in test environments.
-        
-        This library brings the following features to Robot Framework:
-        - generating a valid BSN
-        - generating a BSN that is unique within the current test run
-        - generating a number that will not pass the eleven test
-        - generating a BSN that starts with specific digits
-        - generating a BSN that is less than 9 digits long
-        - checking if a given number passes the eleven test
-        - returning a list of BSNs generated during the current test run
-        - specifying BSNs that should not be generated
-        
-        Possible use cases:
-        - A test message that is processed by one or more systems can be tracked by its unique BSN
-        - Creating messages with BSNs in a certain range that leads to a certain response from a system or stub
-        - Checking whether a test message contains a valid BSN
-        
-        ## Backward compatibility
-        BSNLibrary v1.0.0 and later is not compatible with previous versions in the sense that is does not allow you to 
-        validate a BSN with _Generate BSN_. You should use _Validate BSN_ instead. If your test suite still uses _Generate 
-        BSN_ for validation it will generate an error saying that the length of ``given`` exceeds the maximum value. In case 
-        you have test suites using _Generate BSN_ for validation you can install BSNLibrary v0.4.0 for a smooth transition: 
-        
-        ``pip install robotframework-bsnlibrary==0.4.0``
-        
-        Your test suite will still run, but you will receive a warning of any deprecated use of _Generate BSN_ and a 
-        recommendation to replace it with the keyword _Validate BSN_. This allows you to convert your test suites at your own 
-        pace. 
-        
-        ## Installation
-        ``pip install robotframework-bsnlibrary``
-        
-        ## General information
-        [Keyword documentation](https://haaihenkie.github.io/bsnlibrary/)
-        
-        [Installation package on PyPI](https://pypi.org/project/robotframework-bsnlibrary/)
-        
-        [Release notes](https://github.com/HaaiHenkie/bsnlibrary/releases)
-        
-        Create date: 01-03-2020
-        
-        Author: Henk van den Akker
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework :: Library
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2.7
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
+Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# BSNLibrary for Robot Framework
+
+Robot Framework Library for generating a random BSN (Burger Service Nummer, i.e. a
+Dutch citizen service number) for test purposes.
+
+A BSN is used in Netherlands to identify a person for government organisations, see
+[this information of the Dutch government](https://www.government.nl/topics/personal-data/citizen-service-number-bsn).
+The number consists of 9 digits and has to pass the eleven test.
+
+This test can be explained with the example 211551557. Each digit is multiplied with
+its position and the results are added up together:
+
+``(9*2) + (8*1) + (7*1) + (6*5) + (5*5) + (4*1) + (3*5) + (2*5) - (1*7) = 110``
+
+Note that the digit in position 1 is subtracted from the other results. The total
+sum can be divided by 11, which means that this number has passed the eleven test.
+
+This library generates BSNs for test purposes in the sense that it generates random
+9 digit numbers that pass the eleven test. By coincidence a generated number could
+be a real person's BSN. Yet this library cannot violate such a person's privacy,
+because it cannot tell you whether a number belongs to a real person or not, nor
+will it provide you with any personal data related to a BSN. Obviously you should
+only use this library in test environments.
+
+This library brings the following features to Robot Framework:
+- generating a valid BSN
+- generating a BSN that is unique within the current test run
+- generating a number that will not pass the eleven test
+- generating a BSN that starts with specific digits
+- generating a BSN that is less than 9 digits long
+- checking if a given number passes the eleven test
+- returning a list of BSNs generated during the current test run
+- specifying BSNs that should not be generated
+
+Possible use cases:
+- A test message that is processed by one or more systems can be tracked by its unique BSN
+- Creating messages with BSNs in a certain range that leads to a certain response from a system or stub
+- Checking whether a test message contains a valid BSN
+
+## Backward compatibility
+BSNLibrary v1.0.0 and later is not compatible with previous versions in the sense that is does not allow you to 
+validate a BSN with _Generate BSN_. You should use _Validate BSN_ instead. If your test suite still uses _Generate 
+BSN_ for validation it will generate an error saying that the length of ``given`` exceeds the maximum value. In case 
+you have test suites using _Generate BSN_ for validation you can install BSNLibrary v0.4.0 for a smooth transition: 
+
+``pip install robotframework-bsnlibrary==0.4.0``
+
+Your test suite will still run, but you will receive a warning of any deprecated use of _Generate BSN_ and a 
+recommendation to replace it with the keyword _Validate BSN_. This allows you to convert your test suites at your own 
+pace. 
+
+## Installation
+``pip install robotframework-bsnlibrary``
+
+## General information
+[Keyword documentation](https://haaihenkie.github.io/bsnlibrary/)
+
+[Installation package on PyPI](https://pypi.org/project/robotframework-bsnlibrary/)
+
+[Release notes](https://github.com/HaaiHenkie/bsnlibrary/releases)
+
+Create date: 01-03-2020
+
+Author: Henk van den Akker
```

### Comparing `robotframework-bsnlibrary-1.0.0/README.md` & `robotframework-bsnlibrary-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-bsnlibrary-1.0.0/docs/index.html` & `robotframework-bsnlibrary-1.1.0/docs/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,169 +1,676 @@
 <!DOCTYPE html>
-<html>
+<html id="library-documentation-top" lang="en">
 <head>
-    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <meta http-equiv="Pragma" content="no-cache">
-    <meta http-equiv="Expires" content="-1">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta content="Robot Framework 3.1.2 (Python 3.7.6 on win32)" name="Generator">
-    <link rel="icon" type="image/x-icon" href="data:image/x-icon;base64,AAABAAEAEBAAAAEAIABoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAKcAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAAqAAAAAAAAAAAAAAAAAAAALIAAAD/AAAA4AAAANwAAADcAAAA3AAAANwAAADcAAAA3AAAANwAAADcAAAA4AAAAP8AAACxAAAAAAAAAKYAAAD/AAAAuwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAC/AAAA/wAAAKkAAAD6AAAAzAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAN8AAAD/AAAA+gAAAMMAAAAAAAAAAgAAAGsAAABrAAAAawAAAGsAAABrAAAAawAAAGsAAABrAAAADAAAAAAAAADaAAAA/wAAAPoAAADDAAAAAAAAAIsAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAANEAAAAAAAAA2gAAAP8AAAD6AAAAwwAAAAAAAAAAAAAAMgAAADIAAAAyAAAAMgAAADIAAAAyAAAAMgAAADIAAAAFAAAAAAAAANoAAAD/AAAA+gAAAMMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADaAAAA/wAAAPoAAADDAAAAAAAAADwAAAB8AAAAAAAAAGAAAABcAAAAAAAAAH8AAABKAAAAAAAAAAAAAAAAAAAA2gAAAP8AAAD6AAAAwwAAAAAAAADCAAAA/wAAACkAAADqAAAA4QAAAAAAAAD7AAAA/wAAALAAAAAGAAAAAAAAANoAAAD/AAAA+gAAAMMAAAAAAAAAIwAAAP4AAAD/AAAA/wAAAGAAAAAAAAAAAAAAAMkAAAD/AAAAigAAAAAAAADaAAAA/wAAAPoAAADDAAAAAAAAAAAAAAAIAAAAcAAAABkAAAAAAAAAAAAAAAAAAAAAAAAAEgAAAAAAAAAAAAAA2gAAAP8AAAD7AAAAywAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAN4AAAD/AAAAqwAAAP8AAACvAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALIAAAD/AAAAsgAAAAAAAAC5AAAA/wAAAMoAAADAAAAAwAAAAMAAAADAAAAAwAAAAMAAAADAAAAAwAAAAMkAAAD/AAAAvAAAAAAAAAAAAAAAAAAAAKwAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAArQAAAAAAAAAAwAMAAIABAAAf+AAAP/wAAD/8AAAgBAAAP/wAAD/8AAA//AAAJIwAADHEAAA//AAAP/wAAB/4AACAAQAAwAMAAA==">
-    <style media="all" type="text/css">
+<meta content="text/html; charset=utf-8" http-equiv="Content-Type">
+<meta content="width=device-width, initial-scale=1.0, maximum-scale=1, user-scalable=0" name="viewport">
+<meta content="no-cache" http-equiv="Pragma">
+<meta content="-1" http-equiv="Expires">
+<meta content="IE=edge" http-equiv="X-UA-Compatible">
+<meta content="Robot Framework 6.0.2 (Python 3.11.3 on win32)" name="Generator">
+<link href="data:image/x-icon;base64,AAABAAEAEBAAAAEAIABoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAKcAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAAqAAAAAAAAAAAAAAAAAAAALIAAAD/AAAA4AAAANwAAADcAAAA3AAAANwAAADcAAAA3AAAANwAAADcAAAA4AAAAP8AAACxAAAAAAAAAKYAAAD/AAAAuwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAC/AAAA/wAAAKkAAAD6AAAAzAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAN8AAAD/AAAA+gAAAMMAAAAAAAAAAgAAAGsAAABrAAAAawAAAGsAAABrAAAAawAAAGsAAABrAAAADAAAAAAAAADaAAAA/wAAAPoAAADDAAAAAAAAAIsAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAANEAAAAAAAAA2gAAAP8AAAD6AAAAwwAAAAAAAAAAAAAAMgAAADIAAAAyAAAAMgAAADIAAAAyAAAAMgAAADIAAAAFAAAAAAAAANoAAAD/AAAA+gAAAMMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADaAAAA/wAAAPoAAADDAAAAAAAAADwAAAB8AAAAAAAAAGAAAABcAAAAAAAAAH8AAABKAAAAAAAAAAAAAAAAAAAA2gAAAP8AAAD6AAAAwwAAAAAAAADCAAAA/wAAACkAAADqAAAA4QAAAAAAAAD7AAAA/wAAALAAAAAGAAAAAAAAANoAAAD/AAAA+gAAAMMAAAAAAAAAIwAAAP4AAAD/AAAA/wAAAGAAAAAAAAAAAAAAAMkAAAD/AAAAigAAAAAAAADaAAAA/wAAAPoAAADDAAAAAAAAAAAAAAAIAAAAcAAAABkAAAAAAAAAAAAAAAAAAAAAAAAAEgAAAAAAAAAAAAAA2gAAAP8AAAD7AAAAywAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAN4AAAD/AAAAqwAAAP8AAACvAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALIAAAD/AAAAsgAAAAAAAAC5AAAA/wAAAMoAAADAAAAAwAAAAMAAAADAAAAAwAAAAMAAAADAAAAAwAAAAMkAAAD/AAAAvAAAAAAAAAAAAAAAAAAAAKwAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAArQAAAAAAAAAAwAMAAIABAAAf+AAAP/wAAD/8AAAgBAAAP/wAAD/8AAA//AAAJIwAADHEAAA//AAAP/wAAB/4AACAAQAAwAMAAA==" rel="icon" type="image/x-icon">
+<style media="all" type="text/css">
+:root {
+    --background-color: white;
+    --text-color: black;
+    --border-color: #e0e0e2;
+    --light-background-color: #f3f3f3;
+    --robot-highlight: #00c0b5;
+    --highlighted-color: var(--text-color);
+    --highlighted-background-color: yellow;
+    --less-important-text-color: gray;
+    --link-color: #0000ee;
+}
+[data-theme="dark"] {
+    --background-color: #1c2227;
+    --text-color: #e2e1d7;
+    --border-color: #4e4e4e;
+    --light-background-color: #002b36;
+    --robot-highlight: yellow;
+    --highlighted-color: var(--background-color);
+    --highlighted-background-color: yellow;
+    --less-important-text-color: #5b6a6f;
+    --link-color: #52adff;
+    color-scheme: dark;
+}
 body {
-    background: white;
-    color: black;
-    font-size: small;
-    font-family: sans-serif;
-    padding: 0 0.5em;
+    background: var(--background-color);
+    color: var(--text-color);
+    margin: 0;
+    font-family: system-ui, -apple-system, sans-serif;
 }
-.metadata th {
-    text-align: left;
-    padding-right: 1em;
+input, button, select {
+    background: var(--background-color);
+    color: var(--text-color);
 }
-a.name, span.name {
-    font-style: italic;
+a {
+    color: var(--link-color);
 }
-a, a:link, a:visited {
-    color: #c30;
+.base-container {
+    display: flex;
 }
-a img {
-    border: 1px solid #c30 !important;
+.libdoc-overview {
+    height: 100vh;
+    display: flex;
+    flex-direction: column;
+    background: white;
+    background: var(--background-color);
+    position: -webkit-sticky; /* Safari */
+    position: sticky;
+    top: 0;
+}
+.libdoc-overview h4 {
+    margin-bottom: 0.5rem;
+    margin-top: 0.5rem;
+}
+.keyword-search-box {
+    display: flex;
+    justify-content: space-between;
+    height: 30px;
+    border: 1px solid var(--border-color);
+    border-radius: 3px;
+    margin-top: 0.5rem;
+}
+#tags-shortcuts-container {
+    margin-top: 0.5rem;
+    height: 30px;
+    border: 1px solid var(--border-color);
+    border-radius: 3px;
+}
+.search-input {
+    flex: 1;
+    border: none;
+    text-indent: 4px;
+}
+.clear-search {
+    border: none;
+}
+#shortcuts-container {
+    display: flex;
+    flex-direction: column;
+    height: 100%;
+}
+.libdoc-details {
+    margin-top: 60px;
+    padding-left: 2%;
+    padding-right: 2%;
+    overflow: auto;
+    max-width: 1000px;
 }
-a:hover, a:active {
-    text-decoration: underline;
-    color: black;
+.libdoc-title {
+    position: fixed;
+    left: 0;
+    top: 0;
+    width: 300px;
+    height: 36px;
+    padding: 0.5rem;
+    margin: 0.5rem;
+    display: flex;
+    align-items: center;
+    text-decoration: none;
+    color: var(--text-color);
 }
-a:hover {
-    text-decoration: underline !important;
+.hamburger-menu {
+    display: none;
+    position: fixed;
+    z-index: 100;
+}
+input.hamburger-menu
+{
+  display: none;
+  width: 67px;
+  height: 46px;
+  position: fixed;
+  top: 0;
+  right: 0;
+  cursor: pointer;
+  opacity: 0;
+  z-index: 2;
+  -webkit-touch-callout: none;
+}
+span.hamburger-menu
+{
+  width: 31px;
+  height: 2px;
+  margin-bottom: 5px;
+  position: fixed;
+  right: 20px;
+  background: black;
+  background: var(--text-color);
+  border-radius: 2px;
+  z-index: 1;
+  transform-origin: 4px 0;
+  transition: transform 0.3s cubic-bezier(0.77,0.2,0.05,1.0),
+              opacity 0.35s ease;
+}
+span.hamburger-menu-1
+{
+    top: 14px;
+    transform-origin: 0 0;
+}
+span.hamburger-menu-2
+{
+    top: 24px;
+}
+span.hamburger-menu-3
+{
+    top: 34px;
+    transform-origin: 0 100%;
+}
+input.hamburger-menu:checked ~ span.hamburger-menu-1
+{
+  opacity: 1;
+  transform: rotate(45deg) translate(2px, -3px);
+  background: var(--text-color);
+}
+input.hamburger-menu:checked ~ span.hamburger-menu-2
+{
+  opacity: 0;
+  transform: rotate(0deg) scale(0.2, 0.2);
+}
+input.hamburger-menu:checked ~ span.hamburger-menu-3
+{
+  transform: rotate(-45deg) translate(2px, 3px);
+  background: var(--text-color);
+}
+.libdoc-title > svg {
+    padding-top: 2px;
+    height: 42px;
+    width: 42px;
+}
+#robot-svg-path {
+    fill: var(--text-color);
+    stroke: none;
+    fill-opacity:1;
+    fill-rule:nonzero;
+}
+.keywords-overview {
+    display: flex;
+    flex-direction: column;
+    height: 0;
+    max-height: calc(100vh - 60px - 0.5rem);
+    flex: 1;
+    border: 1px solid var(--border-color);
+    border-radius: 3px;
+    padding-right: 0.5rem;
+    padding-left: 0.5rem;
+    margin: 60px 0 0.5rem 0.5rem;
+}
+.keywords-overview-header-row {
+    display: flex;
+    justify-content: space-between;
 }
 .shortcuts {
-    margin: 1em 0;
     font-size: 0.9em;
+    overflow: auto;
+    list-style: none;
+    padding-left: 0;
+    margin: 0;
+    flex: 1;
+    max-width: 320px;
+}
+.shortcuts.keyword-wall{
+    flex: unset;
 }
 .shortcuts a {
-    display: inline-block;
+    display: block;
     text-decoration: none;
     white-space: nowrap;
-    color: black;
+    color: var(--text-color);
+    padding: 0.5rem;
+}
+.shortcuts a:hover {
+    background: var(--light-background-color);
 }
 .shortcuts a::first-letter {
     font-weight: bold;
     letter-spacing: 0.1em;
 }
+.shortcuts.keyword-wall a {
+    padding: 0;
+    padding-right: 0.5rem;
+    padding-bottom: 0.5rem;
+}
+.shortcuts.keyword-wall a::after {
+    content: '·';
+    padding-left: 0.5rem;
+}
+.enum-type-members, .dt-usages-list {
+    list-style: none;
+    padding-left: 1em;
+}
+.dt-usages-list > li {
+    margin-bottom: 0.2em;
+}
+.dt-usages a {
+    text-decoration: none;
+    color: var(--text-color);
+    display: inline-block;
+    font-size: 0.9em;
+}
+.dt-usages a::first-letter {
+    font-weight: bold;
+    letter-spacing: 0.1em;
+}
+.arguments-list-container {
+    overflow-y: auto;
+}
+.arguments-list {
+    display: -ms-inline-grid;
+    display: inline-grid;
+    -ms-grid-columns: 1fr 1fr 1fr;
+    grid-template-columns: auto auto auto;
+    row-gap: 3px;
+}
+.typed-dict-annotation > span,
+.enum-type-members span,
+.arguments-list .arg-name {
+    -ms-grid-column: 1;
+    grid-column: 1;
+    border-radius: 3px;
+    white-space: nowrap;
+    padding-left: 0.5rem;
+    padding-right: 0.5rem;
+    justify-self: start;
+}
+.arguments-list .arg-default-container {
+    -ms-grid-column: 2;
+    grid-column: 2;
+    display: flex;
+}
+.optional-key {
+    font-style: italic;
+}
+.arguments-list .arg-default-eq {
+    margin-left: 2rem;
+    margin-right: 0.5rem;
+    background: var(--background-color);
+}
+.arguments-list .arg-default-value {
+    padding-left: 0.5rem;
+    padding-right: 0.5rem;
+    border-radius: 3px;
+}
+.arguments-list .base-arg-data {
+    display: flex;
+    min-width: 150px;
+}
+.arguments-list .arg-type {
+    margin-left: 2rem;
+    -ms-grid-column: 3;
+    grid-column: 3;
+    background: var(--background-color);
+    white-space: nowrap;
+    -webkit-text-size-adjust: none;
+}
+.arguments-list .arg-kind {
+  color: transparent;
+  text-shadow: 0 0 0 var(--less-important-text-color);
+  padding: 0;
+  font-size: 0.8em;
+}
+@media only screen and (min-width: 900px) {
+    .libdoc-details {
+        z-index: 1;
+        background: var(--background-color);
+    }
+    #toggle-keyword-shortcuts {
+        border: 1px solid var(--border-color);
+        border-radius: 3px;
+        margin-top: 3px;
+        margin-bottom: 3px;
+    }
+    #toggle-keyword-shortcuts:hover {
+        background: var(--light-background-color);
+    }
+    .shortcuts.keyword-wall {
+        display: flex;
+        flex-wrap: wrap;
+        width: 320px;
+        max-width: none;
+    }
+}
+@media only screen and (min-width: 1200px) {
+    .shortcuts.keyword-wall {
+        width: 640px;
+    }
+}
+@media only screen and (max-width: 899px) {
+    .libdoc-overview {
+        display: none;
+    }
+    #toggle-keyword-shortcuts {
+        display: none;
+    }
+    .libdoc-title {
+        width: 100%;
+        padding: 0.5rem;
+        margin: 0;
+        border-bottom: 1px solid var(--border-color);
+        background: white;
+        background: var(--background-color);
+    }
+    .libdoc-title > svg {
+        margin-right: 60px;
+    }
+    .libdoc-details {
+        padding-left: 0.5rem;
+    }
+    input.hamburger-menu {
+        display: block;
+    }
+    .hamburger-menu {
+        display: block;
+    }
+    .hamburger-menu:checked ~ .libdoc-overview {
+        display: block;
+        position: fixed;
+        height: 100vh;
+        width: 100%;
+    }
+    .keywords-overview {
+        border: none;
+        margin: 60px 0 0;
+    }
+    .shortcuts {
+        max-width: 100vw;
+        overscroll-behavior: none;
+    }
+}
+.metadata {
+    margin-top: 0.5rem;
+ }
+.metadata th {
+    text-align: left;
+    padding-right: 1em;
+}
+a.name, span.name {
+    font-style: italic;
+}
+.libdoc-details a img {
+    border: 1px solid #c30 !important;
+}
+a:hover, a:active {
+    text-decoration: underline;
+    color: var(--text-color);
+}
+a:hover {
+    text-decoration: underline !important;
+}
 .normal-first-letter::first-letter {
     font-weight: normal !important;
     letter-spacing: 0 !important;
 }
+.shortcut-list-toggle, .tag-list-toggle {
+    margin-bottom: 1em;
+    font-size: 0.9em;
+}
+input.switch {
+    display: none;
+}
+.slider {
+    background-color: var(--border-color);
+    display: inline-block;
+    position: relative;
+    top: 5px;
+    height: 18px;
+    width: 36px;
+}
+.slider:before {
+    background-color: var(--background-color);
+    content: "";
+    position: absolute;
+    top: 3px;
+    left: 3px;
+    height: 12px;
+    width: 12px;
+}
+input.switch:checked + .slider::before {
+    background-color: var(--background-color);
+    left: 21px;
+}
 .keywords {
-    border: 1px solid #ccc;
-    border-collapse: collapse;
-    empty-cells: show;
-    margin: 0.3em 0;
-    width: 100%;
+    display: flex;
+    flex-direction: column;
 }
-.keywords th, .keywords td {
-    border: 1px solid #ccc;
-    padding: 0.2em;
-    vertical-align: top;
+.kw-overview {
+    display: flex;
+    flex-direction: column;
+    justify-content: start;
+}
+@media only screen and (min-width: 899px) {
+    .kw-overview {
+        max-width: 850px;
+        margin-right: 1.5rem;
+    }
+}
+.kw-docs {
+    display: flex;
+    flex-direction: column;
+    overflow-y: auto;
 }
-.keywords th {
-    background: #ddd;
-    color: black;
+.dt-name:link,
+.kw-name:link {
+    text-decoration: none;
+    color: var(--text-color);
+}
+.dt-name:visited,
+.kw-name:visited {
+    text-decoration: none;
+    color: var(--text-color);
 }
-.kw, .args, .tags {
-    min-width: 100px;
-    max-width: 20%;
+.kw {
+    display: flex;
+    align-items: baseline;
+    min-width: 250px
+}
+h4 {
+    margin-right: 0.5rem;
+}
+.keyword-container {
+    border: 1px solid var(--border-color);
+    border-radius: 3px;
+    padding: 0.5rem 1.0rem 0.5rem 1.0rem;
+    margin-bottom: 0.5rem;
+    display: flex;
+    flex-direction: column;
+    scroll-margin-top: 60px;
+}
+.keyword-container:target {
+    box-shadow: 0 0 4px var(--robot-highlight);
+}
+.data-type-content,
+.keyword-content {
+    display: flex;
+    flex-direction: column;
+}
+.data-type-container {
+    border-top: 1px solid var(--border-color);
+    padding: 0.5rem 1.0rem 0.5rem 1.0rem;
+    margin-bottom: 0.5rem;
+    display: flex;
+    flex-direction: column;
+    scroll-margin-top: 60px;
+}
+.kw-row {
+    display: flex;
+    flex-direction: column;
+    text-decoration: none;
+    justify-content: start;
+    border: 1px solid var(--border-color);
+    border-radius: 3px;
+    padding: 0.5rem 1.0rem 0.5rem 1.0rem;
+    margin-bottom: 0.5rem;
 }
-td.kw a {
+.kw a {
     color: inherit;
     text-decoration: none;
     font-weight: bold;
 }
-.args span {
-    font-style: italic;
+.args {
+    min-width: 200px;
+}
+.enum-type-members span,
+.args span,
+.args a
+ {
+    font-family: monospace;
+    background: var(--light-background-color);
     padding: 0 0.1em;
+    font-size: 1.1em;
+}
+span.type,
+a.type {
+    font-size: 1em;
+    background: none;
+    padding: 0 0
+}
+.arg-type span.or::after {
+    content: ' or ';
+}
+span.or {
+    background: none;
+    font-size: 0.7em;
+    font-family: system-ui, -apple-system, sans-serif;
+}
+.arg-type span.or:nth-last-of-type(1) {
+    display: none;
+}
+.typed-dict-item .td-type::after {
+    content: ',';
+}
+.typed-dict-item .td-type:nth-last-child(2)::after {
+    content: '';
+}
+.td-item::before {
+    content: '  ';
+    white-space: pre;
+}
+.typed-dict-item {
+    display: block;
+    padding: 0.4rem;
+    font-family: monospace;
+    background: var(--light-background-color);
+    font-size: 1.1em;
+}
+.args span .highlight {
+    background: var(--highlighted-background-color);
+    color: var(--highlighted-color);
+}
+.tags {
+    display: flex;
+    align-items: baseline;
 }
 .tags a {
     color: inherit;
     text-decoration: none;
     padding: 0 0.1em;
 }
 .footer {
     font-size: 0.9em;
 }
-/* Docs originating from HTML and reST are wrapped to divs. */
-.doc div > *:first-child {
-    margin-top: 0;
-}
-.doc div > *:last-child {    /* Does not work with IE8. */
+.doc div > *:last-child {
     margin-bottom: 0;
 }
-#search, #open-search {
-    position: fixed;
-    bottom: 5px;
-    right: 5px;
-    z-index: 1000;
-}
-#search {
-    width: 30em;
-    display: none;
-}
-#open-search {
-    border: 2px solid #ccc;
-    border-radius: 4px;
-    width: 40px;
-    height: 40px;
-    background-color: white;
-    background-repeat: no-repeat;
-    background-position: center;
-    background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEwAACxMBAJqcGAAAAY5JREFUSImt1LtrFGEUBfCfURsFHwEr29UNkS3MFklrQK0EIYUk/5IQ0FSmCCKW1mpAommToCKoK+lsLUKeSFbXFLuT3B13Hjt64INvOPeec+fOnUs2mpjHBrbRwQE+YQFTObm5qGMZf0qct7gxjPgM9kqKJ+cAs2XFf4fEX3iOe7iKsxjFHTxFO8R2ikzqqcq/oVFQUANfUm8ynhUce97qVVoGo/gaclcGBTVDQDuvigw09Lfrr+maD+TSkOIJngWNx2lyI5C3KxrcDRof0+R2IC9XNLgSNPbTZDKa7YricFr/v3EqIUZ0xxPO4FxFg0vhnoz7scFmICcqGjTDvRWJEayG57mKBg/C/U2anHDSu5+oDSlex6GTlTE2KOhVMPmACyXFL+qOZZL7Xf/3OMY17KZMrheI13px6e26nmVyX3eDxnYt4lav0qTiaTzp8VkrPNdkNyOpkyM4lEkNL0uK/CjgXw8ySHATD7GGLd0/fgfv8QiTOI93BSb/jCKT/4Isk1ZOTiWTF0H8M8aPANvFyARlADGFAAAAAElFTkSuQmCC);
-    background-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSI4IiBoZWlnaHQ9IjgiIHZpZXdCb3g9IjAgMCA4IDgiPgogIDxwYXRoIGQ9Ik0zLjUgMGMtMS45MyAwLTMuNSAxLjU3LTMuNSAzLjVzMS41NyAzLjUgMy41IDMuNWMuNTkgMCAxLjE3LS4xNCAxLjY2LS40MWExIDEgMCAwIDAgLjEzLjEzbDEgMWExLjAyIDEuMDIgMCAxIDAgMS40NC0xLjQ0bC0xLTFhMSAxIDAgMCAwLS4xNi0uMTNjLjI3LS40OS40NC0xLjA2LjQ0LTEuNjYgMC0xLjkzLTEuNTctMy41LTMuNS0zLjV6bTAgMWMxLjM5IDAgMi41IDEuMTEgMi41IDIuNSAwIC42Ni0uMjQgMS4yNy0uNjYgMS43Mi0uMDEuMDEtLjAyLjAyLS4wMy4wM2ExIDEgMCAwIDAtLjEzLjEzYy0uNDQuNC0xLjA0LjYzLTEuNjkuNjMtMS4zOSAwLTIuNS0xLjExLTIuNS0yLjVzMS4xMS0yLjUgMi41LTIuNXoiCiAgLz4KPC9zdmc+), none;
-    background-size: 24px 24px;
-}
-#open-search:hover {
-    background-color: #ccc;
-}
-fieldset {
-    background: white;
-    border: 2px solid #ccc;
-    border-radius: 4px;
-    padding: 6px 8px;
-}
-fieldset fieldset {
-    border: 1px solid #ccc;
-    margin: 4px 0;
+.highlight {
+    background: var(--highlighted-background-color);
+    color: var(--highlighted-color);
 }
-#search-title {
-    font-size: 1.1em;
-    font-weight: bold;
-    letter-spacing: 1px;
+.data-type {
+    font-style: italic;
 }
-#search-string {
-    box-sizing: border-box;
-    width: 100%;
+.no-match {
+    color: var(--less-important-text-color) !important;
 }
-#hide-unmatched {
-    margin: 0.5em 0 0 1em;
+.no-match .dt-name,
+.no-match .kw-name {
+    color: var(--less-important-text-color);
+}
+.modal-icon {
+    cursor: pointer;
+    font-size: 12px;
+    font-weight: 600;
+    margin: 0 0.25rem;
+    width: 1rem;
+    height: 1rem;
+    padding: 0;
+    border: none;
+    background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" height="100%" width="100%"><path stroke="black" fill="none" stroke-width="2px" stroke-linecap="round" d="M1 8 L1 1 L8 1 M16 1 L23 1 L23 8 M23 16 L23 23 L16 23 M8 23 L1 23 L1 16"></path><path fill="black" stroke="none" stroke-width="1px" transform="scale(1.3) translate(-3 -2.5)" d="M19 7.97zm-8 9.2-4-2.3v-4.63l4 2.33v4.6zm1-6.33L8.04 8.53 12 6.25l3.96 2.28L12 10.84zm5 4.03-4 2.3v-4.6l4-2.33v4.63z"></path></svg>');
 }
-#search-buttons {
-    float: right;
+@media (prefers-color-scheme: dark) {
+    .modal-icon {
+        background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" height="100%" width="100%"><path stroke="%23e2e1d7" fill="none" stroke-width="2px" stroke-linecap="round" d="M1 8 L1 1 L8 1 M16 1 L23 1 L23 8 M23 16 L23 23 L16 23 M8 23 L1 23 L1 16"></path><path fill="%23e2e1d7" stroke="none" stroke-width="1px" transform="scale(1.3) translate(-3 -2.5)" d="M19 7.97zm-8 9.2-4-2.3v-4.63l4 2.33v4.6zm1-6.33L8.04 8.53 12 6.25l3.96 2.28L12 10.84zm5 4.03-4 2.3v-4.6l4-2.33v4.63z"></path></svg>');
+    }
 }
-.highlight {
-    background: yellow;
+.modal-background, .modal {
+    opacity: 0;
+    pointer-events: none;
+    transition: opacity 0.2s;
 }
-.no-match {
-    color: gray !important;
+.modal-background {
+    position: fixed;
+    top: 0;
+    right: 0;
+    bottom: 0;
+    left: 0;
+    background-color: rgba(0, 0, 0, 0.7);
+    z-index: 1;
+}
+.modal {
+    display: flex;
+    flex-wrap: nowrap;
+    flex-direction: column;
+    width: 720px;
+    max-width: calc(100vw - 2rem);
+    margin: 0 auto;
+    height: calc(100vh - 6rem);
+    overflow: auto;
+    background-color: var(--background-color);
+    border: 1px solid var(--border-color);
+    border-radius: 3px;
+    z-index: 2;
+    transition-delay: 0.1s;
+}
+.modal-content {
+    margin-bottom: 3rem;
+}
+.modal > .modal-content > .data-type-container {
+    border-top: none;
+}
+.modal-close-button-wrapper {
+    display: flex;
+    justify-content: flex-end;
+}
+.modal-close-button-container {
+    width: 720px;
+    max-width: calc(100vw - 2rem);
+    margin: 0 auto;
+    overflow: auto;
+}
+.modal-close-button {
+    margin: 0.5rem 0;
+    padding: 0.25rem 0.5rem;
+    border-radius:3px;
+    border: 1px solid var(--border-color);
+    cursor: pointer;
+}
+.modal-background.visible, .modal.visible {
+    opacity: 1;
+    pointer-events: all;
 }
-tr.no-match.hide-unmatched {
+#data-types-container {
     display: none;
 }
 </style>
-    <style media="all" type="text/css">
+<style media="all" type="text/css">
 /* Pygments 'default' style sheet. Generated with Pygments 2.1.3 using:
-     pygmentize -S default -f html -a .code > src/robot/htmldata/libdoc/pygments.css
+    pygmentize -S default -f html -a .code > src/robot/htmldata/libdoc/pygments.css
+    and added for dark mode
+    @media (prefers-color-scheme: dark)
+    pygmentize -S solarized-dark -f html -a .code > src/robot/htmldata/libdoc/pygments.css
 */
 .code .hll { background-color: #ffffcc }
 .code  { background: #f8f8f8; }
 .code .c { color: #408080; font-style: italic } /* Comment */
 .code .err { border: 1px solid #FF0000 } /* Error */
 .code .k { color: #008000; font-weight: bold } /* Keyword */
 .code .o { color: #666666 } /* Operator */
@@ -206,45 +713,129 @@
 .code .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
 .code .w { color: #bbbbbb } /* Text.Whitespace */
 .code .mb { color: #666666 } /* Literal.Number.Bin */
 .code .mf { color: #666666 } /* Literal.Number.Float */
 .code .mh { color: #666666 } /* Literal.Number.Hex */
 .code .mi { color: #666666 } /* Literal.Number.Integer */
 .code .mo { color: #666666 } /* Literal.Number.Oct */
+.code .sa { color: #BA2121 } /* Literal.String.Affix */
 .code .sb { color: #BA2121 } /* Literal.String.Backtick */
 .code .sc { color: #BA2121 } /* Literal.String.Char */
+.code .dl { color: #BA2121 } /* Literal.String.Delimiter */
 .code .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
 .code .s2 { color: #BA2121 } /* Literal.String.Double */
 .code .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
 .code .sh { color: #BA2121 } /* Literal.String.Heredoc */
 .code .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
 .code .sx { color: #008000 } /* Literal.String.Other */
 .code .sr { color: #BB6688 } /* Literal.String.Regex */
 .code .s1 { color: #BA2121 } /* Literal.String.Single */
 .code .ss { color: #19177C } /* Literal.String.Symbol */
 .code .bp { color: #008000 } /* Name.Builtin.Pseudo */
+.code .fm { color: #0000FF } /* Name.Function.Magic */
 .code .vc { color: #19177C } /* Name.Variable.Class */
 .code .vg { color: #19177C } /* Name.Variable.Global */
 .code .vi { color: #19177C } /* Name.Variable.Instance */
+.code .vm { color: #19177C } /* Name.Variable.Magic */
 .code .il { color: #666666 } /* Literal.Number.Integer.Long */
+@media (prefers-color-scheme: dark) {
+    .code .hll { background-color: #073642 }
+    .code  { background: #002b36; color: #839496 }
+    .code .c { color: #586e75; font-style: italic } /* Comment */
+    .code .err { color: #839496; background-color: #dc322f } /* Error */
+    .code .esc { color: #839496 } /* Escape */
+    .code .g { color: #839496 } /* Generic */
+    .code .k { color: #859900 } /* Keyword */
+    .code .l { color: #839496 } /* Literal */
+    .code .n { color: #839496 } /* Name */
+    .code .o { color: #586e75 } /* Operator */
+    .code .x { color: #839496 } /* Other */
+    .code .p { color: #839496 } /* Punctuation */
+    .code .ch { color: #586e75; font-style: italic } /* Comment.Hashbang */
+    .code .cm { color: #586e75; font-style: italic } /* Comment.Multiline */
+    .code .cp { color: #d33682 } /* Comment.Preproc */
+    .code .cpf { color: #586e75 } /* Comment.PreprocFile */
+    .code .c1 { color: #586e75; font-style: italic } /* Comment.Single */
+    .code .cs { color: #586e75; font-style: italic } /* Comment.Special */
+    .code .gd { color: #dc322f } /* Generic.Deleted */
+    .code .ge { color: #839496; font-style: italic } /* Generic.Emph */
+    .code .gr { color: #dc322f } /* Generic.Error */
+    .code .gh { color: #839496; font-weight: bold } /* Generic.Heading */
+    .code .gi { color: #859900 } /* Generic.Inserted */
+    .code .go { color: #839496 } /* Generic.Output */
+    .code .gp { color: #839496 } /* Generic.Prompt */
+    .code .gs { color: #839496; font-weight: bold } /* Generic.Strong */
+    .code .gu { color: #839496; text-decoration: underline } /* Generic.Subheading */
+    .code .gt { color: #268bd2 } /* Generic.Traceback */
+    .code .kc { color: #2aa198 } /* Keyword.Constant */
+    .code .kd { color: #2aa198 } /* Keyword.Declaration */
+    .code .kn { color: #cb4b16 } /* Keyword.Namespace */
+    .code .kp { color: #859900 } /* Keyword.Pseudo */
+    .code .kr { color: #859900 } /* Keyword.Reserved */
+    .code .kt { color: #b58900 } /* Keyword.Type */
+    .code .ld { color: #839496 } /* Literal.Date */
+    .code .m { color: #2aa198 } /* Literal.Number */
+    .code .s { color: #2aa198 } /* Literal.String */
+    .code .na { color: #839496 } /* Name.Attribute */
+    .code .nb { color: #268bd2 } /* Name.Builtin */
+    .code .nc { color: #268bd2 } /* Name.Class */
+    .code .no { color: #268bd2 } /* Name.Constant */
+    .code .nd { color: #268bd2 } /* Name.Decorator */
+    .code .ni { color: #268bd2 } /* Name.Entity */
+    .code .ne { color: #268bd2 } /* Name.Exception */
+    .code .nf { color: #268bd2 } /* Name.Function */
+    .code .nl { color: #268bd2 } /* Name.Label */
+    .code .nn { color: #268bd2 } /* Name.Namespace */
+    .code .nx { color: #839496 } /* Name.Other */
+    .code .py { color: #839496 } /* Name.Property */
+    .code .nt { color: #268bd2 } /* Name.Tag */
+    .code .nv { color: #268bd2 } /* Name.Variable */
+    .code .ow { color: #859900 } /* Operator.Word */
+    .code .w { color: #839496 } /* Text.Whitespace */
+    .code .mb { color: #2aa198 } /* Literal.Number.Bin */
+    .code .mf { color: #2aa198 } /* Literal.Number.Float */
+    .code .mh { color: #2aa198 } /* Literal.Number.Hex */
+    .code .mi { color: #2aa198 } /* Literal.Number.Integer */
+    .code .mo { color: #2aa198 } /* Literal.Number.Oct */
+    .code .sa { color: #2aa198 } /* Literal.String.Affix */
+    .code .sb { color: #2aa198 } /* Literal.String.Backtick */
+    .code .sc { color: #2aa198 } /* Literal.String.Char */
+    .code .dl { color: #2aa198 } /* Literal.String.Delimiter */
+    .code .sd { color: #586e75 } /* Literal.String.Doc */
+    .code .s2 { color: #2aa198 } /* Literal.String.Double */
+    .code .se { color: #2aa198 } /* Literal.String.Escape */
+    .code .sh { color: #2aa198 } /* Literal.String.Heredoc */
+    .code .si { color: #2aa198 } /* Literal.String.Interpol */
+    .code .sx { color: #2aa198 } /* Literal.String.Other */
+    .code .sr { color: #cb4b16 } /* Literal.String.Regex */
+    .code .s1 { color: #2aa198 } /* Literal.String.Single */
+    .code .ss { color: #2aa198 } /* Literal.String.Symbol */
+    .code .bp { color: #268bd2 } /* Name.Builtin.Pseudo */
+    .code .fm { color: #268bd2 } /* Name.Function.Magic */
+    .code .vc { color: #268bd2 } /* Name.Variable.Class */
+    .code .vg { color: #268bd2 } /* Name.Variable.Global */
+    .code .vi { color: #268bd2 } /* Name.Variable.Instance */
+    .code .vm { color: #268bd2 } /* Name.Variable.Magic */
+    .code .il { color: #2aa198 } /* Literal.Number.Integer.Long */
+}
 </style>
-    <style media="print" type="text/css">
+<style media="print" type="text/css">
 body {
     margin: 0;
     padding: 0;
     font-size: 8pt;
 }
 a {
     text-decoration: none;
 }
 #search, #open-search {
     display: none;
 }
 </style>
-    <style media="all" type="text/css">
+<style media="all" type="text/css">
 #javascript-disabled {
     width: 600px;
     margin: 100px auto 0 auto;
     padding: 20px;
     color: black;
     border: 1px solid #ccc;
     background: #eee;
@@ -259,66 +850,118 @@
 #javascript-disabled li {
     margin: 0.5em 0;
 }
 #javascript-disabled b {
     font-style: italic;
 }
 </style>
-    <style media="all" type="text/css">
-.doc > * {
-    margin: 0.7em 1em 0.1em 1em;
-    padding: 0;
-}
-.doc > p, .doc > h1, .doc > h2, .doc > h3, .doc > h4 {
-    margin: 0.7em 0 0.1em 0;
+<style media="all" type="text/css">
+#introduction-container > h2,
+.doc > h1,
+.doc > h2,
+.section > h1,
+.section > h2 {
+    margin-top: 4rem;
+    margin-bottom: 1rem;
+}
+.doc > h3, .section > h3 {
+    margin-top: 3rem;
+    margin-bottom: 1rem;
+}
+.doc > h4, .section > h4 {
+    margin-top: 2rem;
+    margin-bottom: 1rem;
+}
+.doc > p, .section > p {
+    margin-top: 1rem;
+    margin-bottom: 0.5rem;
 }
 .doc > *:first-child {
     margin-top: 0.1em;
 }
 .doc table {
-    border: 1px solid #ccc;
+    border: none;
     background: transparent;
     border-collapse: collapse;
     empty-cells: show;
     font-size: 0.9em;
+    overflow-y: auto;
+    display: block;
 }
 .doc table th, .doc table td {
-    border: 1px solid #ccc;
+    border: 1px solid var(--border-color);
     background: transparent;
     padding: 0.1em 0.3em;
     height: 1.2em;
 }
 .doc table th {
     text-align: center;
     letter-spacing: 0.1em;
 }
 .doc pre {
     font-size: 1.1em;
     letter-spacing: 0.05em;
-    background: #f4f4f4;
+    background: var(--light-background-color);
+    overflow-y: auto;
+    padding: 0.3rem;
+    border-radius: 3px;
 }
-.doc code {
-    padding: 0 0.2em;
+.doc code,
+.docutils.literal {
+    font-size: 1.1em;
     letter-spacing: 0.05em;
-    background: #eee;
+    background: var(--light-background-color);
+    padding: 1px;
+    border-radius: 3px;
 }
 .doc li {
     list-style-position: inside;
     list-style-type: square;
 }
 .doc img {
     border: 1px solid #ccc;
 }
 .doc hr {
     background: #ccc;
     height: 1px;
     border: 0;
 }
 </style>
-    <script type="text/javascript">
+<script type="text/javascript">
+storage = function () {
+    var prefix = 'robot-framework-';
+    var storage;
+    function init(user) {
+        prefix += user + '-';
+        storage = getStorage();
+    }
+    function getStorage() {
+        // Use localStorage if it's accessible, normal object otherwise.
+        // Inspired by https://stackoverflow.com/questions/11214404
+        try {
+            localStorage.setItem(prefix, prefix);
+            localStorage.removeItem(prefix);
+            return localStorage;
+        } catch (exception) {
+            return {};
+        }
+    }
+    function get(name, defaultValue) {
+        var value = storage[prefix + name];
+        if (typeof value === 'undefined')
+            return defaultValue;
+        return value;
+    }
+    function set(name, value) {
+        storage[prefix + name] = value;
+    }
+    return {init: init, get: get, set: set};
+}();
+</script>
+<script type="text/javascript">
 window.util = function () {
     function map(elems, func) {
         var ret = [];
         for (var i = 0, len = elems.length; i < len; i++) {
             ret[i] = func(elems[i]);
         }
         return ret;
@@ -513,400 +1156,693 @@
         timestamp: timestamp,
         createGeneratedString: createGeneratedString,
         createGeneratedAgoString: createGeneratedAgoString,
         parseQueryString: parseQueryString
     };
 }();
 </script>
-    <script type="text/javascript">
-/*! jQuery v3.3.1 | (c) JS Foundation and other contributors | jquery.org/license */
-!function(e,t){"use strict";"object"==typeof module&&"object"==typeof module.exports?module.exports=e.document?t(e,!0):function(e){if(!e.document)throw new Error("jQuery requires a window with a document");return t(e)}:t(e)}("undefined"!=typeof window?window:this,function(e,t){"use strict";var n=[],r=e.document,i=Object.getPrototypeOf,o=n.slice,a=n.concat,s=n.push,u=n.indexOf,l={},c=l.toString,f=l.hasOwnProperty,p=f.toString,d=p.call(Object),h={},g=function e(t){return"function"==typeof t&&"number"!=typeof t.nodeType},y=function e(t){return null!=t&&t===t.window},v={type:!0,src:!0,noModule:!0};function m(e,t,n){var i,o=(t=t||r).createElement("script");if(o.text=e,n)for(i in v)n[i]&&(o[i]=n[i]);t.head.appendChild(o).parentNode.removeChild(o)}function x(e){return null==e?e+"":"object"==typeof e||"function"==typeof e?l[c.call(e)]||"object":typeof e}var b="3.3.1",w=function(e,t){return new w.fn.init(e,t)},T=/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;w.fn=w.prototype={jquery:"3.3.1",constructor:w,length:0,toArray:function(){return o.call(this)},get:function(e){return null==e?o.call(this):e<0?this[e+this.length]:this[e]},pushStack:function(e){var t=w.merge(this.constructor(),e);return t.prevObject=this,t},each:function(e){return w.each(this,e)},map:function(e){return this.pushStack(w.map(this,function(t,n){return e.call(t,n,t)}))},slice:function(){return this.pushStack(o.apply(this,arguments))},first:function(){return this.eq(0)},last:function(){return this.eq(-1)},eq:function(e){var t=this.length,n=+e+(e<0?t:0);return this.pushStack(n>=0&&n<t?[this[n]]:[])},end:function(){return this.prevObject||this.constructor()},push:s,sort:n.sort,splice:n.splice},w.extend=w.fn.extend=function(){var e,t,n,r,i,o,a=arguments[0]||{},s=1,u=arguments.length,l=!1;for("boolean"==typeof a&&(l=a,a=arguments[s]||{},s++),"object"==typeof a||g(a)||(a={}),s===u&&(a=this,s--);s<u;s++)if(null!=(e=arguments[s]))for(t in e)n=a[t],a!==(r=e[t])&&(l&&r&&(w.isPlainObject(r)||(i=Array.isArray(r)))?(i?(i=!1,o=n&&Array.isArray(n)?n:[]):o=n&&w.isPlainObject(n)?n:{},a[t]=w.extend(l,o,r)):void 0!==r&&(a[t]=r));return a},w.extend({expando:"jQuery"+("3.3.1"+Math.random()).replace(/\D/g,""),isReady:!0,error:function(e){throw new Error(e)},noop:function(){},isPlainObject:function(e){var t,n;return!(!e||"[object Object]"!==c.call(e))&&(!(t=i(e))||"function"==typeof(n=f.call(t,"constructor")&&t.constructor)&&p.call(n)===d)},isEmptyObject:function(e){var t;for(t in e)return!1;return!0},globalEval:function(e){m(e)},each:function(e,t){var n,r=0;if(C(e)){for(n=e.length;r<n;r++)if(!1===t.call(e[r],r,e[r]))break}else for(r in e)if(!1===t.call(e[r],r,e[r]))break;return e},trim:function(e){return null==e?"":(e+"").replace(T,"")},makeArray:function(e,t){var n=t||[];return null!=e&&(C(Object(e))?w.merge(n,"string"==typeof e?[e]:e):s.call(n,e)),n},inArray:function(e,t,n){return null==t?-1:u.call(t,e,n)},merge:function(e,t){for(var n=+t.length,r=0,i=e.length;r<n;r++)e[i++]=t[r];return e.length=i,e},grep:function(e,t,n){for(var r,i=[],o=0,a=e.length,s=!n;o<a;o++)(r=!t(e[o],o))!==s&&i.push(e[o]);return i},map:function(e,t,n){var r,i,o=0,s=[];if(C(e))for(r=e.length;o<r;o++)null!=(i=t(e[o],o,n))&&s.push(i);else for(o in e)null!=(i=t(e[o],o,n))&&s.push(i);return a.apply([],s)},guid:1,support:h}),"function"==typeof Symbol&&(w.fn[Symbol.iterator]=n[Symbol.iterator]),w.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "),function(e,t){l["[object "+t+"]"]=t.toLowerCase()});function C(e){var t=!!e&&"length"in e&&e.length,n=x(e);return!g(e)&&!y(e)&&("array"===n||0===t||"number"==typeof t&&t>0&&t-1 in e)}var E=function(e){var t,n,r,i,o,a,s,u,l,c,f,p,d,h,g,y,v,m,x,b="sizzle"+1*new Date,w=e.document,T=0,C=0,E=ae(),k=ae(),S=ae(),D=function(e,t){return e===t&&(f=!0),0},N={}.hasOwnProperty,A=[],j=A.pop,q=A.push,L=A.push,H=A.slice,O=function(e,t){for(var n=0,r=e.length;n<r;n++)if(e[n]===t)return n;return-1},P="checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",M="[\\x20\\t\\r\\n\\f]",R="(?:\\\\.|[\\w-]|[^\0-\\xa0])+",I="\\["+M+"*("+R+")(?:"+M+"*([*^$|!~]?=)"+M+"*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|("+R+"))|)"+M+"*\\]",W=":("+R+")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|"+I+")*)|.*)\\)|)",$=new RegExp(M+"+","g"),B=new RegExp("^"+M+"+|((?:^|[^\\\\])(?:\\\\.)*)"+M+"+$","g"),F=new RegExp("^"+M+"*,"+M+"*"),_=new RegExp("^"+M+"*([>+~]|"+M+")"+M+"*"),z=new RegExp("="+M+"*([^\\]'\"]*?)"+M+"*\\]","g"),X=new RegExp(W),U=new RegExp("^"+R+"$"),V={ID:new RegExp("^#("+R+")"),CLASS:new RegExp("^\\.("+R+")"),TAG:new RegExp("^("+R+"|[*])"),ATTR:new RegExp("^"+I),PSEUDO:new RegExp("^"+W),CHILD:new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\("+M+"*(even|odd|(([+-]|)(\\d*)n|)"+M+"*(?:([+-]|)"+M+"*(\\d+)|))"+M+"*\\)|)","i"),bool:new RegExp("^(?:"+P+")$","i"),needsContext:new RegExp("^"+M+"*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\("+M+"*((?:-\\d)?\\d*)"+M+"*\\)|)(?=[^-]|$)","i")},G=/^(?:input|select|textarea|button)$/i,Y=/^h\d$/i,Q=/^[^{]+\{\s*\[native \w/,J=/^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,K=/[+~]/,Z=new RegExp("\\\\([\\da-f]{1,6}"+M+"?|("+M+")|.)","ig"),ee=function(e,t,n){var r="0x"+t-65536;return r!==r||n?t:r<0?String.fromCharCode(r+65536):String.fromCharCode(r>>10|55296,1023&r|56320)},te=/([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,ne=function(e,t){return t?"\0"===e?"\ufffd":e.slice(0,-1)+"\\"+e.charCodeAt(e.length-1).toString(16)+" ":"\\"+e},re=function(){p()},ie=me(function(e){return!0===e.disabled&&("form"in e||"label"in e)},{dir:"parentNode",next:"legend"});try{L.apply(A=H.call(w.childNodes),w.childNodes),A[w.childNodes.length].nodeType}catch(e){L={apply:A.length?function(e,t){q.apply(e,H.call(t))}:function(e,t){var n=e.length,r=0;while(e[n++]=t[r++]);e.length=n-1}}}function oe(e,t,r,i){var o,s,l,c,f,h,v,m=t&&t.ownerDocument,T=t?t.nodeType:9;if(r=r||[],"string"!=typeof e||!e||1!==T&&9!==T&&11!==T)return r;if(!i&&((t?t.ownerDocument||t:w)!==d&&p(t),t=t||d,g)){if(11!==T&&(f=J.exec(e)))if(o=f[1]){if(9===T){if(!(l=t.getElementById(o)))return r;if(l.id===o)return r.push(l),r}else if(m&&(l=m.getElementById(o))&&x(t,l)&&l.id===o)return r.push(l),r}else{if(f[2])return L.apply(r,t.getElementsByTagName(e)),r;if((o=f[3])&&n.getElementsByClassName&&t.getElementsByClassName)return L.apply(r,t.getElementsByClassName(o)),r}if(n.qsa&&!S[e+" "]&&(!y||!y.test(e))){if(1!==T)m=t,v=e;else if("object"!==t.nodeName.toLowerCase()){(c=t.getAttribute("id"))?c=c.replace(te,ne):t.setAttribute("id",c=b),s=(h=a(e)).length;while(s--)h[s]="#"+c+" "+ve(h[s]);v=h.join(","),m=K.test(e)&&ge(t.parentNode)||t}if(v)try{return L.apply(r,m.querySelectorAll(v)),r}catch(e){}finally{c===b&&t.removeAttribute("id")}}}return u(e.replace(B,"$1"),t,r,i)}function ae(){var e=[];function t(n,i){return e.push(n+" ")>r.cacheLength&&delete t[e.shift()],t[n+" "]=i}return t}function se(e){return e[b]=!0,e}function ue(e){var t=d.createElement("fieldset");try{return!!e(t)}catch(e){return!1}finally{t.parentNode&&t.parentNode.removeChild(t),t=null}}function le(e,t){var n=e.split("|"),i=n.length;while(i--)r.attrHandle[n[i]]=t}function ce(e,t){var n=t&&e,r=n&&1===e.nodeType&&1===t.nodeType&&e.sourceIndex-t.sourceIndex;if(r)return r;if(n)while(n=n.nextSibling)if(n===t)return-1;return e?1:-1}function fe(e){return function(t){return"input"===t.nodeName.toLowerCase()&&t.type===e}}function pe(e){return function(t){var n=t.nodeName.toLowerCase();return("input"===n||"button"===n)&&t.type===e}}function de(e){return function(t){return"form"in t?t.parentNode&&!1===t.disabled?"label"in t?"label"in t.parentNode?t.parentNode.disabled===e:t.disabled===e:t.isDisabled===e||t.isDisabled!==!e&&ie(t)===e:t.disabled===e:"label"in t&&t.disabled===e}}function he(e){return se(function(t){return t=+t,se(function(n,r){var i,o=e([],n.length,t),a=o.length;while(a--)n[i=o[a]]&&(n[i]=!(r[i]=n[i]))})})}function ge(e){return e&&"undefined"!=typeof e.getElementsByTagName&&e}n=oe.support={},o=oe.isXML=function(e){var t=e&&(e.ownerDocument||e).documentElement;return!!t&&"HTML"!==t.nodeName},p=oe.setDocument=function(e){var t,i,a=e?e.ownerDocument||e:w;return a!==d&&9===a.nodeType&&a.documentElement?(d=a,h=d.documentElement,g=!o(d),w!==d&&(i=d.defaultView)&&i.top!==i&&(i.addEventListener?i.addEventListener("unload",re,!1):i.attachEvent&&i.attachEvent("onunload",re)),n.attributes=ue(function(e){return e.className="i",!e.getAttribute("className")}),n.getElementsByTagName=ue(function(e){return e.appendChild(d.createComment("")),!e.getElementsByTagName("*").length}),n.getElementsByClassName=Q.test(d.getElementsByClassName),n.getById=ue(function(e){return h.appendChild(e).id=b,!d.getElementsByName||!d.getElementsByName(b).length}),n.getById?(r.filter.ID=function(e){var t=e.replace(Z,ee);return function(e){return e.getAttribute("id")===t}},r.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&g){var n=t.getElementById(e);return n?[n]:[]}}):(r.filter.ID=function(e){var t=e.replace(Z,ee);return function(e){var n="undefined"!=typeof e.getAttributeNode&&e.getAttributeNode("id");return n&&n.value===t}},r.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&g){var n,r,i,o=t.getElementById(e);if(o){if((n=o.getAttributeNode("id"))&&n.value===e)return[o];i=t.getElementsByName(e),r=0;while(o=i[r++])if((n=o.getAttributeNode("id"))&&n.value===e)return[o]}return[]}}),r.find.TAG=n.getElementsByTagName?function(e,t){return"undefined"!=typeof t.getElementsByTagName?t.getElementsByTagName(e):n.qsa?t.querySelectorAll(e):void 0}:function(e,t){var n,r=[],i=0,o=t.getElementsByTagName(e);if("*"===e){while(n=o[i++])1===n.nodeType&&r.push(n);return r}return o},r.find.CLASS=n.getElementsByClassName&&function(e,t){if("undefined"!=typeof t.getElementsByClassName&&g)return t.getElementsByClassName(e)},v=[],y=[],(n.qsa=Q.test(d.querySelectorAll))&&(ue(function(e){h.appendChild(e).innerHTML="<a id='"+b+"'></a><select id='"+b+"-\r\\' msallowcapture=''><option selected=''></option></select>",e.querySelectorAll("[msallowcapture^='']").length&&y.push("[*^$]="+M+"*(?:''|\"\")"),e.querySelectorAll("[selected]").length||y.push("\\["+M+"*(?:value|"+P+")"),e.querySelectorAll("[id~="+b+"-]").length||y.push("~="),e.querySelectorAll(":checked").length||y.push(":checked"),e.querySelectorAll("a#"+b+"+*").length||y.push(".#.+[+~]")}),ue(function(e){e.innerHTML="<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";var t=d.createElement("input");t.setAttribute("type","hidden"),e.appendChild(t).setAttribute("name","D"),e.querySelectorAll("[name=d]").length&&y.push("name"+M+"*[*^$|!~]?="),2!==e.querySelectorAll(":enabled").length&&y.push(":enabled",":disabled"),h.appendChild(e).disabled=!0,2!==e.querySelectorAll(":disabled").length&&y.push(":enabled",":disabled"),e.querySelectorAll("*,:x"),y.push(",.*:")})),(n.matchesSelector=Q.test(m=h.matches||h.webkitMatchesSelector||h.mozMatchesSelector||h.oMatchesSelector||h.msMatchesSelector))&&ue(function(e){n.disconnectedMatch=m.call(e,"*"),m.call(e,"[s!='']:x"),v.push("!=",W)}),y=y.length&&new RegExp(y.join("|")),v=v.length&&new RegExp(v.join("|")),t=Q.test(h.compareDocumentPosition),x=t||Q.test(h.contains)?function(e,t){var n=9===e.nodeType?e.documentElement:e,r=t&&t.parentNode;return e===r||!(!r||1!==r.nodeType||!(n.contains?n.contains(r):e.compareDocumentPosition&&16&e.compareDocumentPosition(r)))}:function(e,t){if(t)while(t=t.parentNode)if(t===e)return!0;return!1},D=t?function(e,t){if(e===t)return f=!0,0;var r=!e.compareDocumentPosition-!t.compareDocumentPosition;return r||(1&(r=(e.ownerDocument||e)===(t.ownerDocument||t)?e.compareDocumentPosition(t):1)||!n.sortDetached&&t.compareDocumentPosition(e)===r?e===d||e.ownerDocument===w&&x(w,e)?-1:t===d||t.ownerDocument===w&&x(w,t)?1:c?O(c,e)-O(c,t):0:4&r?-1:1)}:function(e,t){if(e===t)return f=!0,0;var n,r=0,i=e.parentNode,o=t.parentNode,a=[e],s=[t];if(!i||!o)return e===d?-1:t===d?1:i?-1:o?1:c?O(c,e)-O(c,t):0;if(i===o)return ce(e,t);n=e;while(n=n.parentNode)a.unshift(n);n=t;while(n=n.parentNode)s.unshift(n);while(a[r]===s[r])r++;return r?ce(a[r],s[r]):a[r]===w?-1:s[r]===w?1:0},d):d},oe.matches=function(e,t){return oe(e,null,null,t)},oe.matchesSelector=function(e,t){if((e.ownerDocument||e)!==d&&p(e),t=t.replace(z,"='$1']"),n.matchesSelector&&g&&!S[t+" "]&&(!v||!v.test(t))&&(!y||!y.test(t)))try{var r=m.call(e,t);if(r||n.disconnectedMatch||e.document&&11!==e.document.nodeType)return r}catch(e){}return oe(t,d,null,[e]).length>0},oe.contains=function(e,t){return(e.ownerDocument||e)!==d&&p(e),x(e,t)},oe.attr=function(e,t){(e.ownerDocument||e)!==d&&p(e);var i=r.attrHandle[t.toLowerCase()],o=i&&N.call(r.attrHandle,t.toLowerCase())?i(e,t,!g):void 0;return void 0!==o?o:n.attributes||!g?e.getAttribute(t):(o=e.getAttributeNode(t))&&o.specified?o.value:null},oe.escape=function(e){return(e+"").replace(te,ne)},oe.error=function(e){throw new Error("Syntax error, unrecognized expression: "+e)},oe.uniqueSort=function(e){var t,r=[],i=0,o=0;if(f=!n.detectDuplicates,c=!n.sortStable&&e.slice(0),e.sort(D),f){while(t=e[o++])t===e[o]&&(i=r.push(o));while(i--)e.splice(r[i],1)}return c=null,e},i=oe.getText=function(e){var t,n="",r=0,o=e.nodeType;if(o){if(1===o||9===o||11===o){if("string"==typeof e.textContent)return e.textContent;for(e=e.firstChild;e;e=e.nextSibling)n+=i(e)}else if(3===o||4===o)return e.nodeValue}else while(t=e[r++])n+=i(t);return n},(r=oe.selectors={cacheLength:50,createPseudo:se,match:V,attrHandle:{},find:{},relative:{">":{dir:"parentNode",first:!0}," ":{dir:"parentNode"},"+":{dir:"previousSibling",first:!0},"~":{dir:"previousSibling"}},preFilter:{ATTR:function(e){return e[1]=e[1].replace(Z,ee),e[3]=(e[3]||e[4]||e[5]||"").replace(Z,ee),"~="===e[2]&&(e[3]=" "+e[3]+" "),e.slice(0,4)},CHILD:function(e){return e[1]=e[1].toLowerCase(),"nth"===e[1].slice(0,3)?(e[3]||oe.error(e[0]),e[4]=+(e[4]?e[5]+(e[6]||1):2*("even"===e[3]||"odd"===e[3])),e[5]=+(e[7]+e[8]||"odd"===e[3])):e[3]&&oe.error(e[0]),e},PSEUDO:function(e){var t,n=!e[6]&&e[2];return V.CHILD.test(e[0])?null:(e[3]?e[2]=e[4]||e[5]||"":n&&X.test(n)&&(t=a(n,!0))&&(t=n.indexOf(")",n.length-t)-n.length)&&(e[0]=e[0].slice(0,t),e[2]=n.slice(0,t)),e.slice(0,3))}},filter:{TAG:function(e){var t=e.replace(Z,ee).toLowerCase();return"*"===e?function(){return!0}:function(e){return e.nodeName&&e.nodeName.toLowerCase()===t}},CLASS:function(e){var t=E[e+" "];return t||(t=new RegExp("(^|"+M+")"+e+"("+M+"|$)"))&&E(e,function(e){return t.test("string"==typeof e.className&&e.className||"undefined"!=typeof e.getAttribute&&e.getAttribute("class")||"")})},ATTR:function(e,t,n){return function(r){var i=oe.attr(r,e);return null==i?"!="===t:!t||(i+="","="===t?i===n:"!="===t?i!==n:"^="===t?n&&0===i.indexOf(n):"*="===t?n&&i.indexOf(n)>-1:"$="===t?n&&i.slice(-n.length)===n:"~="===t?(" "+i.replace($," ")+" ").indexOf(n)>-1:"|="===t&&(i===n||i.slice(0,n.length+1)===n+"-"))}},CHILD:function(e,t,n,r,i){var o="nth"!==e.slice(0,3),a="last"!==e.slice(-4),s="of-type"===t;return 1===r&&0===i?function(e){return!!e.parentNode}:function(t,n,u){var l,c,f,p,d,h,g=o!==a?"nextSibling":"previousSibling",y=t.parentNode,v=s&&t.nodeName.toLowerCase(),m=!u&&!s,x=!1;if(y){if(o){while(g){p=t;while(p=p[g])if(s?p.nodeName.toLowerCase()===v:1===p.nodeType)return!1;h=g="only"===e&&!h&&"nextSibling"}return!0}if(h=[a?y.firstChild:y.lastChild],a&&m){x=(d=(l=(c=(f=(p=y)[b]||(p[b]={}))[p.uniqueID]||(f[p.uniqueID]={}))[e]||[])[0]===T&&l[1])&&l[2],p=d&&y.childNodes[d];while(p=++d&&p&&p[g]||(x=d=0)||h.pop())if(1===p.nodeType&&++x&&p===t){c[e]=[T,d,x];break}}else if(m&&(x=d=(l=(c=(f=(p=t)[b]||(p[b]={}))[p.uniqueID]||(f[p.uniqueID]={}))[e]||[])[0]===T&&l[1]),!1===x)while(p=++d&&p&&p[g]||(x=d=0)||h.pop())if((s?p.nodeName.toLowerCase()===v:1===p.nodeType)&&++x&&(m&&((c=(f=p[b]||(p[b]={}))[p.uniqueID]||(f[p.uniqueID]={}))[e]=[T,x]),p===t))break;return(x-=i)===r||x%r==0&&x/r>=0}}},PSEUDO:function(e,t){var n,i=r.pseudos[e]||r.setFilters[e.toLowerCase()]||oe.error("unsupported pseudo: "+e);return i[b]?i(t):i.length>1?(n=[e,e,"",t],r.setFilters.hasOwnProperty(e.toLowerCase())?se(function(e,n){var r,o=i(e,t),a=o.length;while(a--)e[r=O(e,o[a])]=!(n[r]=o[a])}):function(e){return i(e,0,n)}):i}},pseudos:{not:se(function(e){var t=[],n=[],r=s(e.replace(B,"$1"));return r[b]?se(function(e,t,n,i){var o,a=r(e,null,i,[]),s=e.length;while(s--)(o=a[s])&&(e[s]=!(t[s]=o))}):function(e,i,o){return t[0]=e,r(t,null,o,n),t[0]=null,!n.pop()}}),has:se(function(e){return function(t){return oe(e,t).length>0}}),contains:se(function(e){return e=e.replace(Z,ee),function(t){return(t.textContent||t.innerText||i(t)).indexOf(e)>-1}}),lang:se(function(e){return U.test(e||"")||oe.error("unsupported lang: "+e),e=e.replace(Z,ee).toLowerCase(),function(t){var n;do{if(n=g?t.lang:t.getAttribute("xml:lang")||t.getAttribute("lang"))return(n=n.toLowerCase())===e||0===n.indexOf(e+"-")}while((t=t.parentNode)&&1===t.nodeType);return!1}}),target:function(t){var n=e.location&&e.location.hash;return n&&n.slice(1)===t.id},root:function(e){return e===h},focus:function(e){return e===d.activeElement&&(!d.hasFocus||d.hasFocus())&&!!(e.type||e.href||~e.tabIndex)},enabled:de(!1),disabled:de(!0),checked:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&!!e.checked||"option"===t&&!!e.selected},selected:function(e){return e.parentNode&&e.parentNode.selectedIndex,!0===e.selected},empty:function(e){for(e=e.firstChild;e;e=e.nextSibling)if(e.nodeType<6)return!1;return!0},parent:function(e){return!r.pseudos.empty(e)},header:function(e){return Y.test(e.nodeName)},input:function(e){return G.test(e.nodeName)},button:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&"button"===e.type||"button"===t},text:function(e){var t;return"input"===e.nodeName.toLowerCase()&&"text"===e.type&&(null==(t=e.getAttribute("type"))||"text"===t.toLowerCase())},first:he(function(){return[0]}),last:he(function(e,t){return[t-1]}),eq:he(function(e,t,n){return[n<0?n+t:n]}),even:he(function(e,t){for(var n=0;n<t;n+=2)e.push(n);return e}),odd:he(function(e,t){for(var n=1;n<t;n+=2)e.push(n);return e}),lt:he(function(e,t,n){for(var r=n<0?n+t:n;--r>=0;)e.push(r);return e}),gt:he(function(e,t,n){for(var r=n<0?n+t:n;++r<t;)e.push(r);return e})}}).pseudos.nth=r.pseudos.eq;for(t in{radio:!0,checkbox:!0,file:!0,password:!0,image:!0})r.pseudos[t]=fe(t);for(t in{submit:!0,reset:!0})r.pseudos[t]=pe(t);function ye(){}ye.prototype=r.filters=r.pseudos,r.setFilters=new ye,a=oe.tokenize=function(e,t){var n,i,o,a,s,u,l,c=k[e+" "];if(c)return t?0:c.slice(0);s=e,u=[],l=r.preFilter;while(s){n&&!(i=F.exec(s))||(i&&(s=s.slice(i[0].length)||s),u.push(o=[])),n=!1,(i=_.exec(s))&&(n=i.shift(),o.push({value:n,type:i[0].replace(B," ")}),s=s.slice(n.length));for(a in r.filter)!(i=V[a].exec(s))||l[a]&&!(i=l[a](i))||(n=i.shift(),o.push({value:n,type:a,matches:i}),s=s.slice(n.length));if(!n)break}return t?s.length:s?oe.error(e):k(e,u).slice(0)};function ve(e){for(var t=0,n=e.length,r="";t<n;t++)r+=e[t].value;return r}function me(e,t,n){var r=t.dir,i=t.next,o=i||r,a=n&&"parentNode"===o,s=C++;return t.first?function(t,n,i){while(t=t[r])if(1===t.nodeType||a)return e(t,n,i);return!1}:function(t,n,u){var l,c,f,p=[T,s];if(u){while(t=t[r])if((1===t.nodeType||a)&&e(t,n,u))return!0}else while(t=t[r])if(1===t.nodeType||a)if(f=t[b]||(t[b]={}),c=f[t.uniqueID]||(f[t.uniqueID]={}),i&&i===t.nodeName.toLowerCase())t=t[r]||t;else{if((l=c[o])&&l[0]===T&&l[1]===s)return p[2]=l[2];if(c[o]=p,p[2]=e(t,n,u))return!0}return!1}}function xe(e){return e.length>1?function(t,n,r){var i=e.length;while(i--)if(!e[i](t,n,r))return!1;return!0}:e[0]}function be(e,t,n){for(var r=0,i=t.length;r<i;r++)oe(e,t[r],n);return n}function we(e,t,n,r,i){for(var o,a=[],s=0,u=e.length,l=null!=t;s<u;s++)(o=e[s])&&(n&&!n(o,r,i)||(a.push(o),l&&t.push(s)));return a}function Te(e,t,n,r,i,o){return r&&!r[b]&&(r=Te(r)),i&&!i[b]&&(i=Te(i,o)),se(function(o,a,s,u){var l,c,f,p=[],d=[],h=a.length,g=o||be(t||"*",s.nodeType?[s]:s,[]),y=!e||!o&&t?g:we(g,p,e,s,u),v=n?i||(o?e:h||r)?[]:a:y;if(n&&n(y,v,s,u),r){l=we(v,d),r(l,[],s,u),c=l.length;while(c--)(f=l[c])&&(v[d[c]]=!(y[d[c]]=f))}if(o){if(i||e){if(i){l=[],c=v.length;while(c--)(f=v[c])&&l.push(y[c]=f);i(null,v=[],l,u)}c=v.length;while(c--)(f=v[c])&&(l=i?O(o,f):p[c])>-1&&(o[l]=!(a[l]=f))}}else v=we(v===a?v.splice(h,v.length):v),i?i(null,a,v,u):L.apply(a,v)})}function Ce(e){for(var t,n,i,o=e.length,a=r.relative[e[0].type],s=a||r.relative[" "],u=a?1:0,c=me(function(e){return e===t},s,!0),f=me(function(e){return O(t,e)>-1},s,!0),p=[function(e,n,r){var i=!a&&(r||n!==l)||((t=n).nodeType?c(e,n,r):f(e,n,r));return t=null,i}];u<o;u++)if(n=r.relative[e[u].type])p=[me(xe(p),n)];else{if((n=r.filter[e[u].type].apply(null,e[u].matches))[b]){for(i=++u;i<o;i++)if(r.relative[e[i].type])break;return Te(u>1&&xe(p),u>1&&ve(e.slice(0,u-1).concat({value:" "===e[u-2].type?"*":""})).replace(B,"$1"),n,u<i&&Ce(e.slice(u,i)),i<o&&Ce(e=e.slice(i)),i<o&&ve(e))}p.push(n)}return xe(p)}function Ee(e,t){var n=t.length>0,i=e.length>0,o=function(o,a,s,u,c){var f,h,y,v=0,m="0",x=o&&[],b=[],w=l,C=o||i&&r.find.TAG("*",c),E=T+=null==w?1:Math.random()||.1,k=C.length;for(c&&(l=a===d||a||c);m!==k&&null!=(f=C[m]);m++){if(i&&f){h=0,a||f.ownerDocument===d||(p(f),s=!g);while(y=e[h++])if(y(f,a||d,s)){u.push(f);break}c&&(T=E)}n&&((f=!y&&f)&&v--,o&&x.push(f))}if(v+=m,n&&m!==v){h=0;while(y=t[h++])y(x,b,a,s);if(o){if(v>0)while(m--)x[m]||b[m]||(b[m]=j.call(u));b=we(b)}L.apply(u,b),c&&!o&&b.length>0&&v+t.length>1&&oe.uniqueSort(u)}return c&&(T=E,l=w),x};return n?se(o):o}return s=oe.compile=function(e,t){var n,r=[],i=[],o=S[e+" "];if(!o){t||(t=a(e)),n=t.length;while(n--)(o=Ce(t[n]))[b]?r.push(o):i.push(o);(o=S(e,Ee(i,r))).selector=e}return o},u=oe.select=function(e,t,n,i){var o,u,l,c,f,p="function"==typeof e&&e,d=!i&&a(e=p.selector||e);if(n=n||[],1===d.length){if((u=d[0]=d[0].slice(0)).length>2&&"ID"===(l=u[0]).type&&9===t.nodeType&&g&&r.relative[u[1].type]){if(!(t=(r.find.ID(l.matches[0].replace(Z,ee),t)||[])[0]))return n;p&&(t=t.parentNode),e=e.slice(u.shift().value.length)}o=V.needsContext.test(e)?0:u.length;while(o--){if(l=u[o],r.relative[c=l.type])break;if((f=r.find[c])&&(i=f(l.matches[0].replace(Z,ee),K.test(u[0].type)&&ge(t.parentNode)||t))){if(u.splice(o,1),!(e=i.length&&ve(u)))return L.apply(n,i),n;break}}}return(p||s(e,d))(i,t,!g,n,!t||K.test(e)&&ge(t.parentNode)||t),n},n.sortStable=b.split("").sort(D).join("")===b,n.detectDuplicates=!!f,p(),n.sortDetached=ue(function(e){return 1&e.compareDocumentPosition(d.createElement("fieldset"))}),ue(function(e){return e.innerHTML="<a href='#'></a>","#"===e.firstChild.getAttribute("href")})||le("type|href|height|width",function(e,t,n){if(!n)return e.getAttribute(t,"type"===t.toLowerCase()?1:2)}),n.attributes&&ue(function(e){return e.innerHTML="<input/>",e.firstChild.setAttribute("value",""),""===e.firstChild.getAttribute("value")})||le("value",function(e,t,n){if(!n&&"input"===e.nodeName.toLowerCase())return e.defaultValue}),ue(function(e){return null==e.getAttribute("disabled")})||le(P,function(e,t,n){var r;if(!n)return!0===e[t]?t.toLowerCase():(r=e.getAttributeNode(t))&&r.specified?r.value:null}),oe}(e);w.find=E,w.expr=E.selectors,w.expr[":"]=w.expr.pseudos,w.uniqueSort=w.unique=E.uniqueSort,w.text=E.getText,w.isXMLDoc=E.isXML,w.contains=E.contains,w.escapeSelector=E.escape;var k=function(e,t,n){var r=[],i=void 0!==n;while((e=e[t])&&9!==e.nodeType)if(1===e.nodeType){if(i&&w(e).is(n))break;r.push(e)}return r},S=function(e,t){for(var n=[];e;e=e.nextSibling)1===e.nodeType&&e!==t&&n.push(e);return n},D=w.expr.match.needsContext;function N(e,t){return e.nodeName&&e.nodeName.toLowerCase()===t.toLowerCase()}var A=/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;function j(e,t,n){return g(t)?w.grep(e,function(e,r){return!!t.call(e,r,e)!==n}):t.nodeType?w.grep(e,function(e){return e===t!==n}):"string"!=typeof t?w.grep(e,function(e){return u.call(t,e)>-1!==n}):w.filter(t,e,n)}w.filter=function(e,t,n){var r=t[0];return n&&(e=":not("+e+")"),1===t.length&&1===r.nodeType?w.find.matchesSelector(r,e)?[r]:[]:w.find.matches(e,w.grep(t,function(e){return 1===e.nodeType}))},w.fn.extend({find:function(e){var t,n,r=this.length,i=this;if("string"!=typeof e)return this.pushStack(w(e).filter(function(){for(t=0;t<r;t++)if(w.contains(i[t],this))return!0}));for(n=this.pushStack([]),t=0;t<r;t++)w.find(e,i[t],n);return r>1?w.uniqueSort(n):n},filter:function(e){return this.pushStack(j(this,e||[],!1))},not:function(e){return this.pushStack(j(this,e||[],!0))},is:function(e){return!!j(this,"string"==typeof e&&D.test(e)?w(e):e||[],!1).length}});var q,L=/^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;(w.fn.init=function(e,t,n){var i,o;if(!e)return this;if(n=n||q,"string"==typeof e){if(!(i="<"===e[0]&&">"===e[e.length-1]&&e.length>=3?[null,e,null]:L.exec(e))||!i[1]&&t)return!t||t.jquery?(t||n).find(e):this.constructor(t).find(e);if(i[1]){if(t=t instanceof w?t[0]:t,w.merge(this,w.parseHTML(i[1],t&&t.nodeType?t.ownerDocument||t:r,!0)),A.test(i[1])&&w.isPlainObject(t))for(i in t)g(this[i])?this[i](t[i]):this.attr(i,t[i]);return this}return(o=r.getElementById(i[2]))&&(this[0]=o,this.length=1),this}return e.nodeType?(this[0]=e,this.length=1,this):g(e)?void 0!==n.ready?n.ready(e):e(w):w.makeArray(e,this)}).prototype=w.fn,q=w(r);var H=/^(?:parents|prev(?:Until|All))/,O={children:!0,contents:!0,next:!0,prev:!0};w.fn.extend({has:function(e){var t=w(e,this),n=t.length;return this.filter(function(){for(var e=0;e<n;e++)if(w.contains(this,t[e]))return!0})},closest:function(e,t){var n,r=0,i=this.length,o=[],a="string"!=typeof e&&w(e);if(!D.test(e))for(;r<i;r++)for(n=this[r];n&&n!==t;n=n.parentNode)if(n.nodeType<11&&(a?a.index(n)>-1:1===n.nodeType&&w.find.matchesSelector(n,e))){o.push(n);break}return this.pushStack(o.length>1?w.uniqueSort(o):o)},index:function(e){return e?"string"==typeof e?u.call(w(e),this[0]):u.call(this,e.jquery?e[0]:e):this[0]&&this[0].parentNode?this.first().prevAll().length:-1},add:function(e,t){return this.pushStack(w.uniqueSort(w.merge(this.get(),w(e,t))))},addBack:function(e){return this.add(null==e?this.prevObject:this.prevObject.filter(e))}});function P(e,t){while((e=e[t])&&1!==e.nodeType);return e}w.each({parent:function(e){var t=e.parentNode;return t&&11!==t.nodeType?t:null},parents:function(e){return k(e,"parentNode")},parentsUntil:function(e,t,n){return k(e,"parentNode",n)},next:function(e){return P(e,"nextSibling")},prev:function(e){return P(e,"previousSibling")},nextAll:function(e){return k(e,"nextSibling")},prevAll:function(e){return k(e,"previousSibling")},nextUntil:function(e,t,n){return k(e,"nextSibling",n)},prevUntil:function(e,t,n){return k(e,"previousSibling",n)},siblings:function(e){return S((e.parentNode||{}).firstChild,e)},children:function(e){return S(e.firstChild)},contents:function(e){return N(e,"iframe")?e.contentDocument:(N(e,"template")&&(e=e.content||e),w.merge([],e.childNodes))}},function(e,t){w.fn[e]=function(n,r){var i=w.map(this,t,n);return"Until"!==e.slice(-5)&&(r=n),r&&"string"==typeof r&&(i=w.filter(r,i)),this.length>1&&(O[e]||w.uniqueSort(i),H.test(e)&&i.reverse()),this.pushStack(i)}});var M=/[^\x20\t\r\n\f]+/g;function R(e){var t={};return w.each(e.match(M)||[],function(e,n){t[n]=!0}),t}w.Callbacks=function(e){e="string"==typeof e?R(e):w.extend({},e);var t,n,r,i,o=[],a=[],s=-1,u=function(){for(i=i||e.once,r=t=!0;a.length;s=-1){n=a.shift();while(++s<o.length)!1===o[s].apply(n[0],n[1])&&e.stopOnFalse&&(s=o.length,n=!1)}e.memory||(n=!1),t=!1,i&&(o=n?[]:"")},l={add:function(){return o&&(n&&!t&&(s=o.length-1,a.push(n)),function t(n){w.each(n,function(n,r){g(r)?e.unique&&l.has(r)||o.push(r):r&&r.length&&"string"!==x(r)&&t(r)})}(arguments),n&&!t&&u()),this},remove:function(){return w.each(arguments,function(e,t){var n;while((n=w.inArray(t,o,n))>-1)o.splice(n,1),n<=s&&s--}),this},has:function(e){return e?w.inArray(e,o)>-1:o.length>0},empty:function(){return o&&(o=[]),this},disable:function(){return i=a=[],o=n="",this},disabled:function(){return!o},lock:function(){return i=a=[],n||t||(o=n=""),this},locked:function(){return!!i},fireWith:function(e,n){return i||(n=[e,(n=n||[]).slice?n.slice():n],a.push(n),t||u()),this},fire:function(){return l.fireWith(this,arguments),this},fired:function(){return!!r}};return l};function I(e){return e}function W(e){throw e}function $(e,t,n,r){var i;try{e&&g(i=e.promise)?i.call(e).done(t).fail(n):e&&g(i=e.then)?i.call(e,t,n):t.apply(void 0,[e].slice(r))}catch(e){n.apply(void 0,[e])}}w.extend({Deferred:function(t){var n=[["notify","progress",w.Callbacks("memory"),w.Callbacks("memory"),2],["resolve","done",w.Callbacks("once memory"),w.Callbacks("once memory"),0,"resolved"],["reject","fail",w.Callbacks("once memory"),w.Callbacks("once memory"),1,"rejected"]],r="pending",i={state:function(){return r},always:function(){return o.done(arguments).fail(arguments),this},"catch":function(e){return i.then(null,e)},pipe:function(){var e=arguments;return w.Deferred(function(t){w.each(n,function(n,r){var i=g(e[r[4]])&&e[r[4]];o[r[1]](function(){var e=i&&i.apply(this,arguments);e&&g(e.promise)?e.promise().progress(t.notify).done(t.resolve).fail(t.reject):t[r[0]+"With"](this,i?[e]:arguments)})}),e=null}).promise()},then:function(t,r,i){var o=0;function a(t,n,r,i){return function(){var s=this,u=arguments,l=function(){var e,l;if(!(t<o)){if((e=r.apply(s,u))===n.promise())throw new TypeError("Thenable self-resolution");l=e&&("object"==typeof e||"function"==typeof e)&&e.then,g(l)?i?l.call(e,a(o,n,I,i),a(o,n,W,i)):(o++,l.call(e,a(o,n,I,i),a(o,n,W,i),a(o,n,I,n.notifyWith))):(r!==I&&(s=void 0,u=[e]),(i||n.resolveWith)(s,u))}},c=i?l:function(){try{l()}catch(e){w.Deferred.exceptionHook&&w.Deferred.exceptionHook(e,c.stackTrace),t+1>=o&&(r!==W&&(s=void 0,u=[e]),n.rejectWith(s,u))}};t?c():(w.Deferred.getStackHook&&(c.stackTrace=w.Deferred.getStackHook()),e.setTimeout(c))}}return w.Deferred(function(e){n[0][3].add(a(0,e,g(i)?i:I,e.notifyWith)),n[1][3].add(a(0,e,g(t)?t:I)),n[2][3].add(a(0,e,g(r)?r:W))}).promise()},promise:function(e){return null!=e?w.extend(e,i):i}},o={};return w.each(n,function(e,t){var a=t[2],s=t[5];i[t[1]]=a.add,s&&a.add(function(){r=s},n[3-e][2].disable,n[3-e][3].disable,n[0][2].lock,n[0][3].lock),a.add(t[3].fire),o[t[0]]=function(){return o[t[0]+"With"](this===o?void 0:this,arguments),this},o[t[0]+"With"]=a.fireWith}),i.promise(o),t&&t.call(o,o),o},when:function(e){var t=arguments.length,n=t,r=Array(n),i=o.call(arguments),a=w.Deferred(),s=function(e){return function(n){r[e]=this,i[e]=arguments.length>1?o.call(arguments):n,--t||a.resolveWith(r,i)}};if(t<=1&&($(e,a.done(s(n)).resolve,a.reject,!t),"pending"===a.state()||g(i[n]&&i[n].then)))return a.then();while(n--)$(i[n],s(n),a.reject);return a.promise()}});var B=/^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;w.Deferred.exceptionHook=function(t,n){e.console&&e.console.warn&&t&&B.test(t.name)&&e.console.warn("jQuery.Deferred exception: "+t.message,t.stack,n)},w.readyException=function(t){e.setTimeout(function(){throw t})};var F=w.Deferred();w.fn.ready=function(e){return F.then(e)["catch"](function(e){w.readyException(e)}),this},w.extend({isReady:!1,readyWait:1,ready:function(e){(!0===e?--w.readyWait:w.isReady)||(w.isReady=!0,!0!==e&&--w.readyWait>0||F.resolveWith(r,[w]))}}),w.ready.then=F.then;function _(){r.removeEventListener("DOMContentLoaded",_),e.removeEventListener("load",_),w.ready()}"complete"===r.readyState||"loading"!==r.readyState&&!r.documentElement.doScroll?e.setTimeout(w.ready):(r.addEventListener("DOMContentLoaded",_),e.addEventListener("load",_));var z=function(e,t,n,r,i,o,a){var s=0,u=e.length,l=null==n;if("object"===x(n)){i=!0;for(s in n)z(e,t,s,n[s],!0,o,a)}else if(void 0!==r&&(i=!0,g(r)||(a=!0),l&&(a?(t.call(e,r),t=null):(l=t,t=function(e,t,n){return l.call(w(e),n)})),t))for(;s<u;s++)t(e[s],n,a?r:r.call(e[s],s,t(e[s],n)));return i?e:l?t.call(e):u?t(e[0],n):o},X=/^-ms-/,U=/-([a-z])/g;function V(e,t){return t.toUpperCase()}function G(e){return e.replace(X,"ms-").replace(U,V)}var Y=function(e){return 1===e.nodeType||9===e.nodeType||!+e.nodeType};function Q(){this.expando=w.expando+Q.uid++}Q.uid=1,Q.prototype={cache:function(e){var t=e[this.expando];return t||(t={},Y(e)&&(e.nodeType?e[this.expando]=t:Object.defineProperty(e,this.expando,{value:t,configurable:!0}))),t},set:function(e,t,n){var r,i=this.cache(e);if("string"==typeof t)i[G(t)]=n;else for(r in t)i[G(r)]=t[r];return i},get:function(e,t){return void 0===t?this.cache(e):e[this.expando]&&e[this.expando][G(t)]},access:function(e,t,n){return void 0===t||t&&"string"==typeof t&&void 0===n?this.get(e,t):(this.set(e,t,n),void 0!==n?n:t)},remove:function(e,t){var n,r=e[this.expando];if(void 0!==r){if(void 0!==t){n=(t=Array.isArray(t)?t.map(G):(t=G(t))in r?[t]:t.match(M)||[]).length;while(n--)delete r[t[n]]}(void 0===t||w.isEmptyObject(r))&&(e.nodeType?e[this.expando]=void 0:delete e[this.expando])}},hasData:function(e){var t=e[this.expando];return void 0!==t&&!w.isEmptyObject(t)}};var J=new Q,K=new Q,Z=/^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,ee=/[A-Z]/g;function te(e){return"true"===e||"false"!==e&&("null"===e?null:e===+e+""?+e:Z.test(e)?JSON.parse(e):e)}function ne(e,t,n){var r;if(void 0===n&&1===e.nodeType)if(r="data-"+t.replace(ee,"-$&").toLowerCase(),"string"==typeof(n=e.getAttribute(r))){try{n=te(n)}catch(e){}K.set(e,t,n)}else n=void 0;return n}w.extend({hasData:function(e){return K.hasData(e)||J.hasData(e)},data:function(e,t,n){return K.access(e,t,n)},removeData:function(e,t){K.remove(e,t)},_data:function(e,t,n){return J.access(e,t,n)},_removeData:function(e,t){J.remove(e,t)}}),w.fn.extend({data:function(e,t){var n,r,i,o=this[0],a=o&&o.attributes;if(void 0===e){if(this.length&&(i=K.get(o),1===o.nodeType&&!J.get(o,"hasDataAttrs"))){n=a.length;while(n--)a[n]&&0===(r=a[n].name).indexOf("data-")&&(r=G(r.slice(5)),ne(o,r,i[r]));J.set(o,"hasDataAttrs",!0)}return i}return"object"==typeof e?this.each(function(){K.set(this,e)}):z(this,function(t){var n;if(o&&void 0===t){if(void 0!==(n=K.get(o,e)))return n;if(void 0!==(n=ne(o,e)))return n}else this.each(function(){K.set(this,e,t)})},null,t,arguments.length>1,null,!0)},removeData:function(e){return this.each(function(){K.remove(this,e)})}}),w.extend({queue:function(e,t,n){var r;if(e)return t=(t||"fx")+"queue",r=J.get(e,t),n&&(!r||Array.isArray(n)?r=J.access(e,t,w.makeArray(n)):r.push(n)),r||[]},dequeue:function(e,t){t=t||"fx";var n=w.queue(e,t),r=n.length,i=n.shift(),o=w._queueHooks(e,t),a=function(){w.dequeue(e,t)};"inprogress"===i&&(i=n.shift(),r--),i&&("fx"===t&&n.unshift("inprogress"),delete o.stop,i.call(e,a,o)),!r&&o&&o.empty.fire()},_queueHooks:function(e,t){var n=t+"queueHooks";return J.get(e,n)||J.access(e,n,{empty:w.Callbacks("once memory").add(function(){J.remove(e,[t+"queue",n])})})}}),w.fn.extend({queue:function(e,t){var n=2;return"string"!=typeof e&&(t=e,e="fx",n--),arguments.length<n?w.queue(this[0],e):void 0===t?this:this.each(function(){var n=w.queue(this,e,t);w._queueHooks(this,e),"fx"===e&&"inprogress"!==n[0]&&w.dequeue(this,e)})},dequeue:function(e){return this.each(function(){w.dequeue(this,e)})},clearQueue:function(e){return this.queue(e||"fx",[])},promise:function(e,t){var n,r=1,i=w.Deferred(),o=this,a=this.length,s=function(){--r||i.resolveWith(o,[o])};"string"!=typeof e&&(t=e,e=void 0),e=e||"fx";while(a--)(n=J.get(o[a],e+"queueHooks"))&&n.empty&&(r++,n.empty.add(s));return s(),i.promise(t)}});var re=/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,ie=new RegExp("^(?:([+-])=|)("+re+")([a-z%]*)$","i"),oe=["Top","Right","Bottom","Left"],ae=function(e,t){return"none"===(e=t||e).style.display||""===e.style.display&&w.contains(e.ownerDocument,e)&&"none"===w.css(e,"display")},se=function(e,t,n,r){var i,o,a={};for(o in t)a[o]=e.style[o],e.style[o]=t[o];i=n.apply(e,r||[]);for(o in t)e.style[o]=a[o];return i};function ue(e,t,n,r){var i,o,a=20,s=r?function(){return r.cur()}:function(){return w.css(e,t,"")},u=s(),l=n&&n[3]||(w.cssNumber[t]?"":"px"),c=(w.cssNumber[t]||"px"!==l&&+u)&&ie.exec(w.css(e,t));if(c&&c[3]!==l){u/=2,l=l||c[3],c=+u||1;while(a--)w.style(e,t,c+l),(1-o)*(1-(o=s()/u||.5))<=0&&(a=0),c/=o;c*=2,w.style(e,t,c+l),n=n||[]}return n&&(c=+c||+u||0,i=n[1]?c+(n[1]+1)*n[2]:+n[2],r&&(r.unit=l,r.start=c,r.end=i)),i}var le={};function ce(e){var t,n=e.ownerDocument,r=e.nodeName,i=le[r];return i||(t=n.body.appendChild(n.createElement(r)),i=w.css(t,"display"),t.parentNode.removeChild(t),"none"===i&&(i="block"),le[r]=i,i)}function fe(e,t){for(var n,r,i=[],o=0,a=e.length;o<a;o++)(r=e[o]).style&&(n=r.style.display,t?("none"===n&&(i[o]=J.get(r,"display")||null,i[o]||(r.style.display="")),""===r.style.display&&ae(r)&&(i[o]=ce(r))):"none"!==n&&(i[o]="none",J.set(r,"display",n)));for(o=0;o<a;o++)null!=i[o]&&(e[o].style.display=i[o]);return e}w.fn.extend({show:function(){return fe(this,!0)},hide:function(){return fe(this)},toggle:function(e){return"boolean"==typeof e?e?this.show():this.hide():this.each(function(){ae(this)?w(this).show():w(this).hide()})}});var pe=/^(?:checkbox|radio)$/i,de=/<([a-z][^\/\0>\x20\t\r\n\f]+)/i,he=/^$|^module$|\/(?:java|ecma)script/i,ge={option:[1,"<select multiple='multiple'>","</select>"],thead:[1,"<table>","</table>"],col:[2,"<table><colgroup>","</colgroup></table>"],tr:[2,"<table><tbody>","</tbody></table>"],td:[3,"<table><tbody><tr>","</tr></tbody></table>"],_default:[0,"",""]};ge.optgroup=ge.option,ge.tbody=ge.tfoot=ge.colgroup=ge.caption=ge.thead,ge.th=ge.td;function ye(e,t){var n;return n="undefined"!=typeof e.getElementsByTagName?e.getElementsByTagName(t||"*"):"undefined"!=typeof e.querySelectorAll?e.querySelectorAll(t||"*"):[],void 0===t||t&&N(e,t)?w.merge([e],n):n}function ve(e,t){for(var n=0,r=e.length;n<r;n++)J.set(e[n],"globalEval",!t||J.get(t[n],"globalEval"))}var me=/<|&#?\w+;/;function xe(e,t,n,r,i){for(var o,a,s,u,l,c,f=t.createDocumentFragment(),p=[],d=0,h=e.length;d<h;d++)if((o=e[d])||0===o)if("object"===x(o))w.merge(p,o.nodeType?[o]:o);else if(me.test(o)){a=a||f.appendChild(t.createElement("div")),s=(de.exec(o)||["",""])[1].toLowerCase(),u=ge[s]||ge._default,a.innerHTML=u[1]+w.htmlPrefilter(o)+u[2],c=u[0];while(c--)a=a.lastChild;w.merge(p,a.childNodes),(a=f.firstChild).textContent=""}else p.push(t.createTextNode(o));f.textContent="",d=0;while(o=p[d++])if(r&&w.inArray(o,r)>-1)i&&i.push(o);else if(l=w.contains(o.ownerDocument,o),a=ye(f.appendChild(o),"script"),l&&ve(a),n){c=0;while(o=a[c++])he.test(o.type||"")&&n.push(o)}return f}!function(){var e=r.createDocumentFragment().appendChild(r.createElement("div")),t=r.createElement("input");t.setAttribute("type","radio"),t.setAttribute("checked","checked"),t.setAttribute("name","t"),e.appendChild(t),h.checkClone=e.cloneNode(!0).cloneNode(!0).lastChild.checked,e.innerHTML="<textarea>x</textarea>",h.noCloneChecked=!!e.cloneNode(!0).lastChild.defaultValue}();var be=r.documentElement,we=/^key/,Te=/^(?:mouse|pointer|contextmenu|drag|drop)|click/,Ce=/^([^.]*)(?:\.(.+)|)/;function Ee(){return!0}function ke(){return!1}function Se(){try{return r.activeElement}catch(e){}}function De(e,t,n,r,i,o){var a,s;if("object"==typeof t){"string"!=typeof n&&(r=r||n,n=void 0);for(s in t)De(e,s,n,r,t[s],o);return e}if(null==r&&null==i?(i=n,r=n=void 0):null==i&&("string"==typeof n?(i=r,r=void 0):(i=r,r=n,n=void 0)),!1===i)i=ke;else if(!i)return e;return 1===o&&(a=i,(i=function(e){return w().off(e),a.apply(this,arguments)}).guid=a.guid||(a.guid=w.guid++)),e.each(function(){w.event.add(this,t,i,r,n)})}w.event={global:{},add:function(e,t,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,y=J.get(e);if(y){n.handler&&(n=(o=n).handler,i=o.selector),i&&w.find.matchesSelector(be,i),n.guid||(n.guid=w.guid++),(u=y.events)||(u=y.events={}),(a=y.handle)||(a=y.handle=function(t){return"undefined"!=typeof w&&w.event.triggered!==t.type?w.event.dispatch.apply(e,arguments):void 0}),l=(t=(t||"").match(M)||[""]).length;while(l--)d=g=(s=Ce.exec(t[l])||[])[1],h=(s[2]||"").split(".").sort(),d&&(f=w.event.special[d]||{},d=(i?f.delegateType:f.bindType)||d,f=w.event.special[d]||{},c=w.extend({type:d,origType:g,data:r,handler:n,guid:n.guid,selector:i,needsContext:i&&w.expr.match.needsContext.test(i),namespace:h.join(".")},o),(p=u[d])||((p=u[d]=[]).delegateCount=0,f.setup&&!1!==f.setup.call(e,r,h,a)||e.addEventListener&&e.addEventListener(d,a)),f.add&&(f.add.call(e,c),c.handler.guid||(c.handler.guid=n.guid)),i?p.splice(p.delegateCount++,0,c):p.push(c),w.event.global[d]=!0)}},remove:function(e,t,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,y=J.hasData(e)&&J.get(e);if(y&&(u=y.events)){l=(t=(t||"").match(M)||[""]).length;while(l--)if(s=Ce.exec(t[l])||[],d=g=s[1],h=(s[2]||"").split(".").sort(),d){f=w.event.special[d]||{},p=u[d=(r?f.delegateType:f.bindType)||d]||[],s=s[2]&&new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"),a=o=p.length;while(o--)c=p[o],!i&&g!==c.origType||n&&n.guid!==c.guid||s&&!s.test(c.namespace)||r&&r!==c.selector&&("**"!==r||!c.selector)||(p.splice(o,1),c.selector&&p.delegateCount--,f.remove&&f.remove.call(e,c));a&&!p.length&&(f.teardown&&!1!==f.teardown.call(e,h,y.handle)||w.removeEvent(e,d,y.handle),delete u[d])}else for(d in u)w.event.remove(e,d+t[l],n,r,!0);w.isEmptyObject(u)&&J.remove(e,"handle events")}},dispatch:function(e){var t=w.event.fix(e),n,r,i,o,a,s,u=new Array(arguments.length),l=(J.get(this,"events")||{})[t.type]||[],c=w.event.special[t.type]||{};for(u[0]=t,n=1;n<arguments.length;n++)u[n]=arguments[n];if(t.delegateTarget=this,!c.preDispatch||!1!==c.preDispatch.call(this,t)){s=w.event.handlers.call(this,t,l),n=0;while((o=s[n++])&&!t.isPropagationStopped()){t.currentTarget=o.elem,r=0;while((a=o.handlers[r++])&&!t.isImmediatePropagationStopped())t.rnamespace&&!t.rnamespace.test(a.namespace)||(t.handleObj=a,t.data=a.data,void 0!==(i=((w.event.special[a.origType]||{}).handle||a.handler).apply(o.elem,u))&&!1===(t.result=i)&&(t.preventDefault(),t.stopPropagation()))}return c.postDispatch&&c.postDispatch.call(this,t),t.result}},handlers:function(e,t){var n,r,i,o,a,s=[],u=t.delegateCount,l=e.target;if(u&&l.nodeType&&!("click"===e.type&&e.button>=1))for(;l!==this;l=l.parentNode||this)if(1===l.nodeType&&("click"!==e.type||!0!==l.disabled)){for(o=[],a={},n=0;n<u;n++)void 0===a[i=(r=t[n]).selector+" "]&&(a[i]=r.needsContext?w(i,this).index(l)>-1:w.find(i,this,null,[l]).length),a[i]&&o.push(r);o.length&&s.push({elem:l,handlers:o})}return l=this,u<t.length&&s.push({elem:l,handlers:t.slice(u)}),s},addProp:function(e,t){Object.defineProperty(w.Event.prototype,e,{enumerable:!0,configurable:!0,get:g(t)?function(){if(this.originalEvent)return t(this.originalEvent)}:function(){if(this.originalEvent)return this.originalEvent[e]},set:function(t){Object.defineProperty(this,e,{enumerable:!0,configurable:!0,writable:!0,value:t})}})},fix:function(e){return e[w.expando]?e:new w.Event(e)},special:{load:{noBubble:!0},focus:{trigger:function(){if(this!==Se()&&this.focus)return this.focus(),!1},delegateType:"focusin"},blur:{trigger:function(){if(this===Se()&&this.blur)return this.blur(),!1},delegateType:"focusout"},click:{trigger:function(){if("checkbox"===this.type&&this.click&&N(this,"input"))return this.click(),!1},_default:function(e){return N(e.target,"a")}},beforeunload:{postDispatch:function(e){void 0!==e.result&&e.originalEvent&&(e.originalEvent.returnValue=e.result)}}}},w.removeEvent=function(e,t,n){e.removeEventListener&&e.removeEventListener(t,n)},w.Event=function(e,t){if(!(this instanceof w.Event))return new w.Event(e,t);e&&e.type?(this.originalEvent=e,this.type=e.type,this.isDefaultPrevented=e.defaultPrevented||void 0===e.defaultPrevented&&!1===e.returnValue?Ee:ke,this.target=e.target&&3===e.target.nodeType?e.target.parentNode:e.target,this.currentTarget=e.currentTarget,this.relatedTarget=e.relatedTarget):this.type=e,t&&w.extend(this,t),this.timeStamp=e&&e.timeStamp||Date.now(),this[w.expando]=!0},w.Event.prototype={constructor:w.Event,isDefaultPrevented:ke,isPropagationStopped:ke,isImmediatePropagationStopped:ke,isSimulated:!1,preventDefault:function(){var e=this.originalEvent;this.isDefaultPrevented=Ee,e&&!this.isSimulated&&e.preventDefault()},stopPropagation:function(){var e=this.originalEvent;this.isPropagationStopped=Ee,e&&!this.isSimulated&&e.stopPropagation()},stopImmediatePropagation:function(){var e=this.originalEvent;this.isImmediatePropagationStopped=Ee,e&&!this.isSimulated&&e.stopImmediatePropagation(),this.stopPropagation()}},w.each({altKey:!0,bubbles:!0,cancelable:!0,changedTouches:!0,ctrlKey:!0,detail:!0,eventPhase:!0,metaKey:!0,pageX:!0,pageY:!0,shiftKey:!0,view:!0,"char":!0,charCode:!0,key:!0,keyCode:!0,button:!0,buttons:!0,clientX:!0,clientY:!0,offsetX:!0,offsetY:!0,pointerId:!0,pointerType:!0,screenX:!0,screenY:!0,targetTouches:!0,toElement:!0,touches:!0,which:function(e){var t=e.button;return null==e.which&&we.test(e.type)?null!=e.charCode?e.charCode:e.keyCode:!e.which&&void 0!==t&&Te.test(e.type)?1&t?1:2&t?3:4&t?2:0:e.which}},w.event.addProp),w.each({mouseenter:"mouseover",mouseleave:"mouseout",pointerenter:"pointerover",pointerleave:"pointerout"},function(e,t){w.event.special[e]={delegateType:t,bindType:t,handle:function(e){var n,r=this,i=e.relatedTarget,o=e.handleObj;return i&&(i===r||w.contains(r,i))||(e.type=o.origType,n=o.handler.apply(this,arguments),e.type=t),n}}}),w.fn.extend({on:function(e,t,n,r){return De(this,e,t,n,r)},one:function(e,t,n,r){return De(this,e,t,n,r,1)},off:function(e,t,n){var r,i;if(e&&e.preventDefault&&e.handleObj)return r=e.handleObj,w(e.delegateTarget).off(r.namespace?r.origType+"."+r.namespace:r.origType,r.selector,r.handler),this;if("object"==typeof e){for(i in e)this.off(i,t,e[i]);return this}return!1!==t&&"function"!=typeof t||(n=t,t=void 0),!1===n&&(n=ke),this.each(function(){w.event.remove(this,e,n,t)})}});var Ne=/<(?!area|br|col|embed|hr|img|input|link|meta|param)(([a-z][^\/\0>\x20\t\r\n\f]*)[^>]*)\/>/gi,Ae=/<script|<style|<link/i,je=/checked\s*(?:[^=]|=\s*.checked.)/i,qe=/^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;function Le(e,t){return N(e,"table")&&N(11!==t.nodeType?t:t.firstChild,"tr")?w(e).children("tbody")[0]||e:e}function He(e){return e.type=(null!==e.getAttribute("type"))+"/"+e.type,e}function Oe(e){return"true/"===(e.type||"").slice(0,5)?e.type=e.type.slice(5):e.removeAttribute("type"),e}function Pe(e,t){var n,r,i,o,a,s,u,l;if(1===t.nodeType){if(J.hasData(e)&&(o=J.access(e),a=J.set(t,o),l=o.events)){delete a.handle,a.events={};for(i in l)for(n=0,r=l[i].length;n<r;n++)w.event.add(t,i,l[i][n])}K.hasData(e)&&(s=K.access(e),u=w.extend({},s),K.set(t,u))}}function Me(e,t){var n=t.nodeName.toLowerCase();"input"===n&&pe.test(e.type)?t.checked=e.checked:"input"!==n&&"textarea"!==n||(t.defaultValue=e.defaultValue)}function Re(e,t,n,r){t=a.apply([],t);var i,o,s,u,l,c,f=0,p=e.length,d=p-1,y=t[0],v=g(y);if(v||p>1&&"string"==typeof y&&!h.checkClone&&je.test(y))return e.each(function(i){var o=e.eq(i);v&&(t[0]=y.call(this,i,o.html())),Re(o,t,n,r)});if(p&&(i=xe(t,e[0].ownerDocument,!1,e,r),o=i.firstChild,1===i.childNodes.length&&(i=o),o||r)){for(u=(s=w.map(ye(i,"script"),He)).length;f<p;f++)l=i,f!==d&&(l=w.clone(l,!0,!0),u&&w.merge(s,ye(l,"script"))),n.call(e[f],l,f);if(u)for(c=s[s.length-1].ownerDocument,w.map(s,Oe),f=0;f<u;f++)l=s[f],he.test(l.type||"")&&!J.access(l,"globalEval")&&w.contains(c,l)&&(l.src&&"module"!==(l.type||"").toLowerCase()?w._evalUrl&&w._evalUrl(l.src):m(l.textContent.replace(qe,""),c,l))}return e}function Ie(e,t,n){for(var r,i=t?w.filter(t,e):e,o=0;null!=(r=i[o]);o++)n||1!==r.nodeType||w.cleanData(ye(r)),r.parentNode&&(n&&w.contains(r.ownerDocument,r)&&ve(ye(r,"script")),r.parentNode.removeChild(r));return e}w.extend({htmlPrefilter:function(e){return e.replace(Ne,"<$1></$2>")},clone:function(e,t,n){var r,i,o,a,s=e.cloneNode(!0),u=w.contains(e.ownerDocument,e);if(!(h.noCloneChecked||1!==e.nodeType&&11!==e.nodeType||w.isXMLDoc(e)))for(a=ye(s),r=0,i=(o=ye(e)).length;r<i;r++)Me(o[r],a[r]);if(t)if(n)for(o=o||ye(e),a=a||ye(s),r=0,i=o.length;r<i;r++)Pe(o[r],a[r]);else Pe(e,s);return(a=ye(s,"script")).length>0&&ve(a,!u&&ye(e,"script")),s},cleanData:function(e){for(var t,n,r,i=w.event.special,o=0;void 0!==(n=e[o]);o++)if(Y(n)){if(t=n[J.expando]){if(t.events)for(r in t.events)i[r]?w.event.remove(n,r):w.removeEvent(n,r,t.handle);n[J.expando]=void 0}n[K.expando]&&(n[K.expando]=void 0)}}}),w.fn.extend({detach:function(e){return Ie(this,e,!0)},remove:function(e){return Ie(this,e)},text:function(e){return z(this,function(e){return void 0===e?w.text(this):this.empty().each(function(){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||(this.textContent=e)})},null,e,arguments.length)},append:function(){return Re(this,arguments,function(e){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||Le(this,e).appendChild(e)})},prepend:function(){return Re(this,arguments,function(e){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var t=Le(this,e);t.insertBefore(e,t.firstChild)}})},before:function(){return Re(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this)})},after:function(){return Re(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this.nextSibling)})},empty:function(){for(var e,t=0;null!=(e=this[t]);t++)1===e.nodeType&&(w.cleanData(ye(e,!1)),e.textContent="");return this},clone:function(e,t){return e=null!=e&&e,t=null==t?e:t,this.map(function(){return w.clone(this,e,t)})},html:function(e){return z(this,function(e){var t=this[0]||{},n=0,r=this.length;if(void 0===e&&1===t.nodeType)return t.innerHTML;if("string"==typeof e&&!Ae.test(e)&&!ge[(de.exec(e)||["",""])[1].toLowerCase()]){e=w.htmlPrefilter(e);try{for(;n<r;n++)1===(t=this[n]||{}).nodeType&&(w.cleanData(ye(t,!1)),t.innerHTML=e);t=0}catch(e){}}t&&this.empty().append(e)},null,e,arguments.length)},replaceWith:function(){var e=[];return Re(this,arguments,function(t){var n=this.parentNode;w.inArray(this,e)<0&&(w.cleanData(ye(this)),n&&n.replaceChild(t,this))},e)}}),w.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(e,t){w.fn[e]=function(e){for(var n,r=[],i=w(e),o=i.length-1,a=0;a<=o;a++)n=a===o?this:this.clone(!0),w(i[a])[t](n),s.apply(r,n.get());return this.pushStack(r)}});var We=new RegExp("^("+re+")(?!px)[a-z%]+$","i"),$e=function(t){var n=t.ownerDocument.defaultView;return n&&n.opener||(n=e),n.getComputedStyle(t)},Be=new RegExp(oe.join("|"),"i");!function(){function t(){if(c){l.style.cssText="position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0",c.style.cssText="position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%",be.appendChild(l).appendChild(c);var t=e.getComputedStyle(c);i="1%"!==t.top,u=12===n(t.marginLeft),c.style.right="60%",s=36===n(t.right),o=36===n(t.width),c.style.position="absolute",a=36===c.offsetWidth||"absolute",be.removeChild(l),c=null}}function n(e){return Math.round(parseFloat(e))}var i,o,a,s,u,l=r.createElement("div"),c=r.createElement("div");c.style&&(c.style.backgroundClip="content-box",c.cloneNode(!0).style.backgroundClip="",h.clearCloneStyle="content-box"===c.style.backgroundClip,w.extend(h,{boxSizingReliable:function(){return t(),o},pixelBoxStyles:function(){return t(),s},pixelPosition:function(){return t(),i},reliableMarginLeft:function(){return t(),u},scrollboxSize:function(){return t(),a}}))}();function Fe(e,t,n){var r,i,o,a,s=e.style;return(n=n||$e(e))&&(""!==(a=n.getPropertyValue(t)||n[t])||w.contains(e.ownerDocument,e)||(a=w.style(e,t)),!h.pixelBoxStyles()&&We.test(a)&&Be.test(t)&&(r=s.width,i=s.minWidth,o=s.maxWidth,s.minWidth=s.maxWidth=s.width=a,a=n.width,s.width=r,s.minWidth=i,s.maxWidth=o)),void 0!==a?a+"":a}function _e(e,t){return{get:function(){if(!e())return(this.get=t).apply(this,arguments);delete this.get}}}var ze=/^(none|table(?!-c[ea]).+)/,Xe=/^--/,Ue={position:"absolute",visibility:"hidden",display:"block"},Ve={letterSpacing:"0",fontWeight:"400"},Ge=["Webkit","Moz","ms"],Ye=r.createElement("div").style;function Qe(e){if(e in Ye)return e;var t=e[0].toUpperCase()+e.slice(1),n=Ge.length;while(n--)if((e=Ge[n]+t)in Ye)return e}function Je(e){var t=w.cssProps[e];return t||(t=w.cssProps[e]=Qe(e)||e),t}function Ke(e,t,n){var r=ie.exec(t);return r?Math.max(0,r[2]-(n||0))+(r[3]||"px"):t}function Ze(e,t,n,r,i,o){var a="width"===t?1:0,s=0,u=0;if(n===(r?"border":"content"))return 0;for(;a<4;a+=2)"margin"===n&&(u+=w.css(e,n+oe[a],!0,i)),r?("content"===n&&(u-=w.css(e,"padding"+oe[a],!0,i)),"margin"!==n&&(u-=w.css(e,"border"+oe[a]+"Width",!0,i))):(u+=w.css(e,"padding"+oe[a],!0,i),"padding"!==n?u+=w.css(e,"border"+oe[a]+"Width",!0,i):s+=w.css(e,"border"+oe[a]+"Width",!0,i));return!r&&o>=0&&(u+=Math.max(0,Math.ceil(e["offset"+t[0].toUpperCase()+t.slice(1)]-o-u-s-.5))),u}function et(e,t,n){var r=$e(e),i=Fe(e,t,r),o="border-box"===w.css(e,"boxSizing",!1,r),a=o;if(We.test(i)){if(!n)return i;i="auto"}return a=a&&(h.boxSizingReliable()||i===e.style[t]),("auto"===i||!parseFloat(i)&&"inline"===w.css(e,"display",!1,r))&&(i=e["offset"+t[0].toUpperCase()+t.slice(1)],a=!0),(i=parseFloat(i)||0)+Ze(e,t,n||(o?"border":"content"),a,r,i)+"px"}w.extend({cssHooks:{opacity:{get:function(e,t){if(t){var n=Fe(e,"opacity");return""===n?"1":n}}}},cssNumber:{animationIterationCount:!0,columnCount:!0,fillOpacity:!0,flexGrow:!0,flexShrink:!0,fontWeight:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,widows:!0,zIndex:!0,zoom:!0},cssProps:{},style:function(e,t,n,r){if(e&&3!==e.nodeType&&8!==e.nodeType&&e.style){var i,o,a,s=G(t),u=Xe.test(t),l=e.style;if(u||(t=Je(s)),a=w.cssHooks[t]||w.cssHooks[s],void 0===n)return a&&"get"in a&&void 0!==(i=a.get(e,!1,r))?i:l[t];"string"==(o=typeof n)&&(i=ie.exec(n))&&i[1]&&(n=ue(e,t,i),o="number"),null!=n&&n===n&&("number"===o&&(n+=i&&i[3]||(w.cssNumber[s]?"":"px")),h.clearCloneStyle||""!==n||0!==t.indexOf("background")||(l[t]="inherit"),a&&"set"in a&&void 0===(n=a.set(e,n,r))||(u?l.setProperty(t,n):l[t]=n))}},css:function(e,t,n,r){var i,o,a,s=G(t);return Xe.test(t)||(t=Je(s)),(a=w.cssHooks[t]||w.cssHooks[s])&&"get"in a&&(i=a.get(e,!0,n)),void 0===i&&(i=Fe(e,t,r)),"normal"===i&&t in Ve&&(i=Ve[t]),""===n||n?(o=parseFloat(i),!0===n||isFinite(o)?o||0:i):i}}),w.each(["height","width"],function(e,t){w.cssHooks[t]={get:function(e,n,r){if(n)return!ze.test(w.css(e,"display"))||e.getClientRects().length&&e.getBoundingClientRect().width?et(e,t,r):se(e,Ue,function(){return et(e,t,r)})},set:function(e,n,r){var i,o=$e(e),a="border-box"===w.css(e,"boxSizing",!1,o),s=r&&Ze(e,t,r,a,o);return a&&h.scrollboxSize()===o.position&&(s-=Math.ceil(e["offset"+t[0].toUpperCase()+t.slice(1)]-parseFloat(o[t])-Ze(e,t,"border",!1,o)-.5)),s&&(i=ie.exec(n))&&"px"!==(i[3]||"px")&&(e.style[t]=n,n=w.css(e,t)),Ke(e,n,s)}}}),w.cssHooks.marginLeft=_e(h.reliableMarginLeft,function(e,t){if(t)return(parseFloat(Fe(e,"marginLeft"))||e.getBoundingClientRect().left-se(e,{marginLeft:0},function(){return e.getBoundingClientRect().left}))+"px"}),w.each({margin:"",padding:"",border:"Width"},function(e,t){w.cssHooks[e+t]={expand:function(n){for(var r=0,i={},o="string"==typeof n?n.split(" "):[n];r<4;r++)i[e+oe[r]+t]=o[r]||o[r-2]||o[0];return i}},"margin"!==e&&(w.cssHooks[e+t].set=Ke)}),w.fn.extend({css:function(e,t){return z(this,function(e,t,n){var r,i,o={},a=0;if(Array.isArray(t)){for(r=$e(e),i=t.length;a<i;a++)o[t[a]]=w.css(e,t[a],!1,r);return o}return void 0!==n?w.style(e,t,n):w.css(e,t)},e,t,arguments.length>1)}});function tt(e,t,n,r,i){return new tt.prototype.init(e,t,n,r,i)}w.Tween=tt,tt.prototype={constructor:tt,init:function(e,t,n,r,i,o){this.elem=e,this.prop=n,this.easing=i||w.easing._default,this.options=t,this.start=this.now=this.cur(),this.end=r,this.unit=o||(w.cssNumber[n]?"":"px")},cur:function(){var e=tt.propHooks[this.prop];return e&&e.get?e.get(this):tt.propHooks._default.get(this)},run:function(e){var t,n=tt.propHooks[this.prop];return this.options.duration?this.pos=t=w.easing[this.easing](e,this.options.duration*e,0,1,this.options.duration):this.pos=t=e,this.now=(this.end-this.start)*t+this.start,this.options.step&&this.options.step.call(this.elem,this.now,this),n&&n.set?n.set(this):tt.propHooks._default.set(this),this}},tt.prototype.init.prototype=tt.prototype,tt.propHooks={_default:{get:function(e){var t;return 1!==e.elem.nodeType||null!=e.elem[e.prop]&&null==e.elem.style[e.prop]?e.elem[e.prop]:(t=w.css(e.elem,e.prop,""))&&"auto"!==t?t:0},set:function(e){w.fx.step[e.prop]?w.fx.step[e.prop](e):1!==e.elem.nodeType||null==e.elem.style[w.cssProps[e.prop]]&&!w.cssHooks[e.prop]?e.elem[e.prop]=e.now:w.style(e.elem,e.prop,e.now+e.unit)}}},tt.propHooks.scrollTop=tt.propHooks.scrollLeft={set:function(e){e.elem.nodeType&&e.elem.parentNode&&(e.elem[e.prop]=e.now)}},w.easing={linear:function(e){return e},swing:function(e){return.5-Math.cos(e*Math.PI)/2},_default:"swing"},w.fx=tt.prototype.init,w.fx.step={};var nt,rt,it=/^(?:toggle|show|hide)$/,ot=/queueHooks$/;function at(){rt&&(!1===r.hidden&&e.requestAnimationFrame?e.requestAnimationFrame(at):e.setTimeout(at,w.fx.interval),w.fx.tick())}function st(){return e.setTimeout(function(){nt=void 0}),nt=Date.now()}function ut(e,t){var n,r=0,i={height:e};for(t=t?1:0;r<4;r+=2-t)i["margin"+(n=oe[r])]=i["padding"+n]=e;return t&&(i.opacity=i.width=e),i}function lt(e,t,n){for(var r,i=(pt.tweeners[t]||[]).concat(pt.tweeners["*"]),o=0,a=i.length;o<a;o++)if(r=i[o].call(n,t,e))return r}function ct(e,t,n){var r,i,o,a,s,u,l,c,f="width"in t||"height"in t,p=this,d={},h=e.style,g=e.nodeType&&ae(e),y=J.get(e,"fxshow");n.queue||(null==(a=w._queueHooks(e,"fx")).unqueued&&(a.unqueued=0,s=a.empty.fire,a.empty.fire=function(){a.unqueued||s()}),a.unqueued++,p.always(function(){p.always(function(){a.unqueued--,w.queue(e,"fx").length||a.empty.fire()})}));for(r in t)if(i=t[r],it.test(i)){if(delete t[r],o=o||"toggle"===i,i===(g?"hide":"show")){if("show"!==i||!y||void 0===y[r])continue;g=!0}d[r]=y&&y[r]||w.style(e,r)}if((u=!w.isEmptyObject(t))||!w.isEmptyObject(d)){f&&1===e.nodeType&&(n.overflow=[h.overflow,h.overflowX,h.overflowY],null==(l=y&&y.display)&&(l=J.get(e,"display")),"none"===(c=w.css(e,"display"))&&(l?c=l:(fe([e],!0),l=e.style.display||l,c=w.css(e,"display"),fe([e]))),("inline"===c||"inline-block"===c&&null!=l)&&"none"===w.css(e,"float")&&(u||(p.done(function(){h.display=l}),null==l&&(c=h.display,l="none"===c?"":c)),h.display="inline-block")),n.overflow&&(h.overflow="hidden",p.always(function(){h.overflow=n.overflow[0],h.overflowX=n.overflow[1],h.overflowY=n.overflow[2]})),u=!1;for(r in d)u||(y?"hidden"in y&&(g=y.hidden):y=J.access(e,"fxshow",{display:l}),o&&(y.hidden=!g),g&&fe([e],!0),p.done(function(){g||fe([e]),J.remove(e,"fxshow");for(r in d)w.style(e,r,d[r])})),u=lt(g?y[r]:0,r,p),r in y||(y[r]=u.start,g&&(u.end=u.start,u.start=0))}}function ft(e,t){var n,r,i,o,a;for(n in e)if(r=G(n),i=t[r],o=e[n],Array.isArray(o)&&(i=o[1],o=e[n]=o[0]),n!==r&&(e[r]=o,delete e[n]),(a=w.cssHooks[r])&&"expand"in a){o=a.expand(o),delete e[r];for(n in o)n in e||(e[n]=o[n],t[n]=i)}else t[r]=i}function pt(e,t,n){var r,i,o=0,a=pt.prefilters.length,s=w.Deferred().always(function(){delete u.elem}),u=function(){if(i)return!1;for(var t=nt||st(),n=Math.max(0,l.startTime+l.duration-t),r=1-(n/l.duration||0),o=0,a=l.tweens.length;o<a;o++)l.tweens[o].run(r);return s.notifyWith(e,[l,r,n]),r<1&&a?n:(a||s.notifyWith(e,[l,1,0]),s.resolveWith(e,[l]),!1)},l=s.promise({elem:e,props:w.extend({},t),opts:w.extend(!0,{specialEasing:{},easing:w.easing._default},n),originalProperties:t,originalOptions:n,startTime:nt||st(),duration:n.duration,tweens:[],createTween:function(t,n){var r=w.Tween(e,l.opts,t,n,l.opts.specialEasing[t]||l.opts.easing);return l.tweens.push(r),r},stop:function(t){var n=0,r=t?l.tweens.length:0;if(i)return this;for(i=!0;n<r;n++)l.tweens[n].run(1);return t?(s.notifyWith(e,[l,1,0]),s.resolveWith(e,[l,t])):s.rejectWith(e,[l,t]),this}}),c=l.props;for(ft(c,l.opts.specialEasing);o<a;o++)if(r=pt.prefilters[o].call(l,e,c,l.opts))return g(r.stop)&&(w._queueHooks(l.elem,l.opts.queue).stop=r.stop.bind(r)),r;return w.map(c,lt,l),g(l.opts.start)&&l.opts.start.call(e,l),l.progress(l.opts.progress).done(l.opts.done,l.opts.complete).fail(l.opts.fail).always(l.opts.always),w.fx.timer(w.extend(u,{elem:e,anim:l,queue:l.opts.queue})),l}w.Animation=w.extend(pt,{tweeners:{"*":[function(e,t){var n=this.createTween(e,t);return ue(n.elem,e,ie.exec(t),n),n}]},tweener:function(e,t){g(e)?(t=e,e=["*"]):e=e.match(M);for(var n,r=0,i=e.length;r<i;r++)n=e[r],pt.tweeners[n]=pt.tweeners[n]||[],pt.tweeners[n].unshift(t)},prefilters:[ct],prefilter:function(e,t){t?pt.prefilters.unshift(e):pt.prefilters.push(e)}}),w.speed=function(e,t,n){var r=e&&"object"==typeof e?w.extend({},e):{complete:n||!n&&t||g(e)&&e,duration:e,easing:n&&t||t&&!g(t)&&t};return w.fx.off?r.duration=0:"number"!=typeof r.duration&&(r.duration in w.fx.speeds?r.duration=w.fx.speeds[r.duration]:r.duration=w.fx.speeds._default),null!=r.queue&&!0!==r.queue||(r.queue="fx"),r.old=r.complete,r.complete=function(){g(r.old)&&r.old.call(this),r.queue&&w.dequeue(this,r.queue)},r},w.fn.extend({fadeTo:function(e,t,n,r){return this.filter(ae).css("opacity",0).show().end().animate({opacity:t},e,n,r)},animate:function(e,t,n,r){var i=w.isEmptyObject(e),o=w.speed(t,n,r),a=function(){var t=pt(this,w.extend({},e),o);(i||J.get(this,"finish"))&&t.stop(!0)};return a.finish=a,i||!1===o.queue?this.each(a):this.queue(o.queue,a)},stop:function(e,t,n){var r=function(e){var t=e.stop;delete e.stop,t(n)};return"string"!=typeof e&&(n=t,t=e,e=void 0),t&&!1!==e&&this.queue(e||"fx",[]),this.each(function(){var t=!0,i=null!=e&&e+"queueHooks",o=w.timers,a=J.get(this);if(i)a[i]&&a[i].stop&&r(a[i]);else for(i in a)a[i]&&a[i].stop&&ot.test(i)&&r(a[i]);for(i=o.length;i--;)o[i].elem!==this||null!=e&&o[i].queue!==e||(o[i].anim.stop(n),t=!1,o.splice(i,1));!t&&n||w.dequeue(this,e)})},finish:function(e){return!1!==e&&(e=e||"fx"),this.each(function(){var t,n=J.get(this),r=n[e+"queue"],i=n[e+"queueHooks"],o=w.timers,a=r?r.length:0;for(n.finish=!0,w.queue(this,e,[]),i&&i.stop&&i.stop.call(this,!0),t=o.length;t--;)o[t].elem===this&&o[t].queue===e&&(o[t].anim.stop(!0),o.splice(t,1));for(t=0;t<a;t++)r[t]&&r[t].finish&&r[t].finish.call(this);delete n.finish})}}),w.each(["toggle","show","hide"],function(e,t){var n=w.fn[t];w.fn[t]=function(e,r,i){return null==e||"boolean"==typeof e?n.apply(this,arguments):this.animate(ut(t,!0),e,r,i)}}),w.each({slideDown:ut("show"),slideUp:ut("hide"),slideToggle:ut("toggle"),fadeIn:{opacity:"show"},fadeOut:{opacity:"hide"},fadeToggle:{opacity:"toggle"}},function(e,t){w.fn[e]=function(e,n,r){return this.animate(t,e,n,r)}}),w.timers=[],w.fx.tick=function(){var e,t=0,n=w.timers;for(nt=Date.now();t<n.length;t++)(e=n[t])()||n[t]!==e||n.splice(t--,1);n.length||w.fx.stop(),nt=void 0},w.fx.timer=function(e){w.timers.push(e),w.fx.start()},w.fx.interval=13,w.fx.start=function(){rt||(rt=!0,at())},w.fx.stop=function(){rt=null},w.fx.speeds={slow:600,fast:200,_default:400},w.fn.delay=function(t,n){return t=w.fx?w.fx.speeds[t]||t:t,n=n||"fx",this.queue(n,function(n,r){var i=e.setTimeout(n,t);r.stop=function(){e.clearTimeout(i)}})},function(){var e=r.createElement("input"),t=r.createElement("select").appendChild(r.createElement("option"));e.type="checkbox",h.checkOn=""!==e.value,h.optSelected=t.selected,(e=r.createElement("input")).value="t",e.type="radio",h.radioValue="t"===e.value}();var dt,ht=w.expr.attrHandle;w.fn.extend({attr:function(e,t){return z(this,w.attr,e,t,arguments.length>1)},removeAttr:function(e){return this.each(function(){w.removeAttr(this,e)})}}),w.extend({attr:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return"undefined"==typeof e.getAttribute?w.prop(e,t,n):(1===o&&w.isXMLDoc(e)||(i=w.attrHooks[t.toLowerCase()]||(w.expr.match.bool.test(t)?dt:void 0)),void 0!==n?null===n?void w.removeAttr(e,t):i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:(e.setAttribute(t,n+""),n):i&&"get"in i&&null!==(r=i.get(e,t))?r:null==(r=w.find.attr(e,t))?void 0:r)},attrHooks:{type:{set:function(e,t){if(!h.radioValue&&"radio"===t&&N(e,"input")){var n=e.value;return e.setAttribute("type",t),n&&(e.value=n),t}}}},removeAttr:function(e,t){var n,r=0,i=t&&t.match(M);if(i&&1===e.nodeType)while(n=i[r++])e.removeAttribute(n)}}),dt={set:function(e,t,n){return!1===t?w.removeAttr(e,n):e.setAttribute(n,n),n}},w.each(w.expr.match.bool.source.match(/\w+/g),function(e,t){var n=ht[t]||w.find.attr;ht[t]=function(e,t,r){var i,o,a=t.toLowerCase();return r||(o=ht[a],ht[a]=i,i=null!=n(e,t,r)?a:null,ht[a]=o),i}});var gt=/^(?:input|select|textarea|button)$/i,yt=/^(?:a|area)$/i;w.fn.extend({prop:function(e,t){return z(this,w.prop,e,t,arguments.length>1)},removeProp:function(e){return this.each(function(){delete this[w.propFix[e]||e]})}}),w.extend({prop:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return 1===o&&w.isXMLDoc(e)||(t=w.propFix[t]||t,i=w.propHooks[t]),void 0!==n?i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:e[t]=n:i&&"get"in i&&null!==(r=i.get(e,t))?r:e[t]},propHooks:{tabIndex:{get:function(e){var t=w.find.attr(e,"tabindex");return t?parseInt(t,10):gt.test(e.nodeName)||yt.test(e.nodeName)&&e.href?0:-1}}},propFix:{"for":"htmlFor","class":"className"}}),h.optSelected||(w.propHooks.selected={get:function(e){var t=e.parentNode;return t&&t.parentNode&&t.parentNode.selectedIndex,null},set:function(e){var t=e.parentNode;t&&(t.selectedIndex,t.parentNode&&t.parentNode.selectedIndex)}}),w.each(["tabIndex","readOnly","maxLength","cellSpacing","cellPadding","rowSpan","colSpan","useMap","frameBorder","contentEditable"],function(){w.propFix[this.toLowerCase()]=this});function vt(e){return(e.match(M)||[]).join(" ")}function mt(e){return e.getAttribute&&e.getAttribute("class")||""}function xt(e){return Array.isArray(e)?e:"string"==typeof e?e.match(M)||[]:[]}w.fn.extend({addClass:function(e){var t,n,r,i,o,a,s,u=0;if(g(e))return this.each(function(t){w(this).addClass(e.call(this,t,mt(this)))});if((t=xt(e)).length)while(n=this[u++])if(i=mt(n),r=1===n.nodeType&&" "+vt(i)+" "){a=0;while(o=t[a++])r.indexOf(" "+o+" ")<0&&(r+=o+" ");i!==(s=vt(r))&&n.setAttribute("class",s)}return this},removeClass:function(e){var t,n,r,i,o,a,s,u=0;if(g(e))return this.each(function(t){w(this).removeClass(e.call(this,t,mt(this)))});if(!arguments.length)return this.attr("class","");if((t=xt(e)).length)while(n=this[u++])if(i=mt(n),r=1===n.nodeType&&" "+vt(i)+" "){a=0;while(o=t[a++])while(r.indexOf(" "+o+" ")>-1)r=r.replace(" "+o+" "," ");i!==(s=vt(r))&&n.setAttribute("class",s)}return this},toggleClass:function(e,t){var n=typeof e,r="string"===n||Array.isArray(e);return"boolean"==typeof t&&r?t?this.addClass(e):this.removeClass(e):g(e)?this.each(function(n){w(this).toggleClass(e.call(this,n,mt(this),t),t)}):this.each(function(){var t,i,o,a;if(r){i=0,o=w(this),a=xt(e);while(t=a[i++])o.hasClass(t)?o.removeClass(t):o.addClass(t)}else void 0!==e&&"boolean"!==n||((t=mt(this))&&J.set(this,"__className__",t),this.setAttribute&&this.setAttribute("class",t||!1===e?"":J.get(this,"__className__")||""))})},hasClass:function(e){var t,n,r=0;t=" "+e+" ";while(n=this[r++])if(1===n.nodeType&&(" "+vt(mt(n))+" ").indexOf(t)>-1)return!0;return!1}});var bt=/\r/g;w.fn.extend({val:function(e){var t,n,r,i=this[0];{if(arguments.length)return r=g(e),this.each(function(n){var i;1===this.nodeType&&(null==(i=r?e.call(this,n,w(this).val()):e)?i="":"number"==typeof i?i+="":Array.isArray(i)&&(i=w.map(i,function(e){return null==e?"":e+""})),(t=w.valHooks[this.type]||w.valHooks[this.nodeName.toLowerCase()])&&"set"in t&&void 0!==t.set(this,i,"value")||(this.value=i))});if(i)return(t=w.valHooks[i.type]||w.valHooks[i.nodeName.toLowerCase()])&&"get"in t&&void 0!==(n=t.get(i,"value"))?n:"string"==typeof(n=i.value)?n.replace(bt,""):null==n?"":n}}}),w.extend({valHooks:{option:{get:function(e){var t=w.find.attr(e,"value");return null!=t?t:vt(w.text(e))}},select:{get:function(e){var t,n,r,i=e.options,o=e.selectedIndex,a="select-one"===e.type,s=a?null:[],u=a?o+1:i.length;for(r=o<0?u:a?o:0;r<u;r++)if(((n=i[r]).selected||r===o)&&!n.disabled&&(!n.parentNode.disabled||!N(n.parentNode,"optgroup"))){if(t=w(n).val(),a)return t;s.push(t)}return s},set:function(e,t){var n,r,i=e.options,o=w.makeArray(t),a=i.length;while(a--)((r=i[a]).selected=w.inArray(w.valHooks.option.get(r),o)>-1)&&(n=!0);return n||(e.selectedIndex=-1),o}}}}),w.each(["radio","checkbox"],function(){w.valHooks[this]={set:function(e,t){if(Array.isArray(t))return e.checked=w.inArray(w(e).val(),t)>-1}},h.checkOn||(w.valHooks[this].get=function(e){return null===e.getAttribute("value")?"on":e.value})}),h.focusin="onfocusin"in e;var wt=/^(?:focusinfocus|focusoutblur)$/,Tt=function(e){e.stopPropagation()};w.extend(w.event,{trigger:function(t,n,i,o){var a,s,u,l,c,p,d,h,v=[i||r],m=f.call(t,"type")?t.type:t,x=f.call(t,"namespace")?t.namespace.split("."):[];if(s=h=u=i=i||r,3!==i.nodeType&&8!==i.nodeType&&!wt.test(m+w.event.triggered)&&(m.indexOf(".")>-1&&(m=(x=m.split(".")).shift(),x.sort()),c=m.indexOf(":")<0&&"on"+m,t=t[w.expando]?t:new w.Event(m,"object"==typeof t&&t),t.isTrigger=o?2:3,t.namespace=x.join("."),t.rnamespace=t.namespace?new RegExp("(^|\\.)"+x.join("\\.(?:.*\\.|)")+"(\\.|$)"):null,t.result=void 0,t.target||(t.target=i),n=null==n?[t]:w.makeArray(n,[t]),d=w.event.special[m]||{},o||!d.trigger||!1!==d.trigger.apply(i,n))){if(!o&&!d.noBubble&&!y(i)){for(l=d.delegateType||m,wt.test(l+m)||(s=s.parentNode);s;s=s.parentNode)v.push(s),u=s;u===(i.ownerDocument||r)&&v.push(u.defaultView||u.parentWindow||e)}a=0;while((s=v[a++])&&!t.isPropagationStopped())h=s,t.type=a>1?l:d.bindType||m,(p=(J.get(s,"events")||{})[t.type]&&J.get(s,"handle"))&&p.apply(s,n),(p=c&&s[c])&&p.apply&&Y(s)&&(t.result=p.apply(s,n),!1===t.result&&t.preventDefault());return t.type=m,o||t.isDefaultPrevented()||d._default&&!1!==d._default.apply(v.pop(),n)||!Y(i)||c&&g(i[m])&&!y(i)&&((u=i[c])&&(i[c]=null),w.event.triggered=m,t.isPropagationStopped()&&h.addEventListener(m,Tt),i[m](),t.isPropagationStopped()&&h.removeEventListener(m,Tt),w.event.triggered=void 0,u&&(i[c]=u)),t.result}},simulate:function(e,t,n){var r=w.extend(new w.Event,n,{type:e,isSimulated:!0});w.event.trigger(r,null,t)}}),w.fn.extend({trigger:function(e,t){return this.each(function(){w.event.trigger(e,t,this)})},triggerHandler:function(e,t){var n=this[0];if(n)return w.event.trigger(e,t,n,!0)}}),h.focusin||w.each({focus:"focusin",blur:"focusout"},function(e,t){var n=function(e){w.event.simulate(t,e.target,w.event.fix(e))};w.event.special[t]={setup:function(){var r=this.ownerDocument||this,i=J.access(r,t);i||r.addEventListener(e,n,!0),J.access(r,t,(i||0)+1)},teardown:function(){var r=this.ownerDocument||this,i=J.access(r,t)-1;i?J.access(r,t,i):(r.removeEventListener(e,n,!0),J.remove(r,t))}}});var Ct=e.location,Et=Date.now(),kt=/\?/;w.parseXML=function(t){var n;if(!t||"string"!=typeof t)return null;try{n=(new e.DOMParser).parseFromString(t,"text/xml")}catch(e){n=void 0}return n&&!n.getElementsByTagName("parsererror").length||w.error("Invalid XML: "+t),n};var St=/\[\]$/,Dt=/\r?\n/g,Nt=/^(?:submit|button|image|reset|file)$/i,At=/^(?:input|select|textarea|keygen)/i;function jt(e,t,n,r){var i;if(Array.isArray(t))w.each(t,function(t,i){n||St.test(e)?r(e,i):jt(e+"["+("object"==typeof i&&null!=i?t:"")+"]",i,n,r)});else if(n||"object"!==x(t))r(e,t);else for(i in t)jt(e+"["+i+"]",t[i],n,r)}w.param=function(e,t){var n,r=[],i=function(e,t){var n=g(t)?t():t;r[r.length]=encodeURIComponent(e)+"="+encodeURIComponent(null==n?"":n)};if(Array.isArray(e)||e.jquery&&!w.isPlainObject(e))w.each(e,function(){i(this.name,this.value)});else for(n in e)jt(n,e[n],t,i);return r.join("&")},w.fn.extend({serialize:function(){return w.param(this.serializeArray())},serializeArray:function(){return this.map(function(){var e=w.prop(this,"elements");return e?w.makeArray(e):this}).filter(function(){var e=this.type;return this.name&&!w(this).is(":disabled")&&At.test(this.nodeName)&&!Nt.test(e)&&(this.checked||!pe.test(e))}).map(function(e,t){var n=w(this).val();return null==n?null:Array.isArray(n)?w.map(n,function(e){return{name:t.name,value:e.replace(Dt,"\r\n")}}):{name:t.name,value:n.replace(Dt,"\r\n")}}).get()}});var qt=/%20/g,Lt=/#.*$/,Ht=/([?&])_=[^&]*/,Ot=/^(.*?):[ \t]*([^\r\n]*)$/gm,Pt=/^(?:about|app|app-storage|.+-extension|file|res|widget):$/,Mt=/^(?:GET|HEAD)$/,Rt=/^\/\//,It={},Wt={},$t="*/".concat("*"),Bt=r.createElement("a");Bt.href=Ct.href;function Ft(e){return function(t,n){"string"!=typeof t&&(n=t,t="*");var r,i=0,o=t.toLowerCase().match(M)||[];if(g(n))while(r=o[i++])"+"===r[0]?(r=r.slice(1)||"*",(e[r]=e[r]||[]).unshift(n)):(e[r]=e[r]||[]).push(n)}}function _t(e,t,n,r){var i={},o=e===Wt;function a(s){var u;return i[s]=!0,w.each(e[s]||[],function(e,s){var l=s(t,n,r);return"string"!=typeof l||o||i[l]?o?!(u=l):void 0:(t.dataTypes.unshift(l),a(l),!1)}),u}return a(t.dataTypes[0])||!i["*"]&&a("*")}function zt(e,t){var n,r,i=w.ajaxSettings.flatOptions||{};for(n in t)void 0!==t[n]&&((i[n]?e:r||(r={}))[n]=t[n]);return r&&w.extend(!0,e,r),e}function Xt(e,t,n){var r,i,o,a,s=e.contents,u=e.dataTypes;while("*"===u[0])u.shift(),void 0===r&&(r=e.mimeType||t.getResponseHeader("Content-Type"));if(r)for(i in s)if(s[i]&&s[i].test(r)){u.unshift(i);break}if(u[0]in n)o=u[0];else{for(i in n){if(!u[0]||e.converters[i+" "+u[0]]){o=i;break}a||(a=i)}o=o||a}if(o)return o!==u[0]&&u.unshift(o),n[o]}function Ut(e,t,n,r){var i,o,a,s,u,l={},c=e.dataTypes.slice();if(c[1])for(a in e.converters)l[a.toLowerCase()]=e.converters[a];o=c.shift();while(o)if(e.responseFields[o]&&(n[e.responseFields[o]]=t),!u&&r&&e.dataFilter&&(t=e.dataFilter(t,e.dataType)),u=o,o=c.shift())if("*"===o)o=u;else if("*"!==u&&u!==o){if(!(a=l[u+" "+o]||l["* "+o]))for(i in l)if((s=i.split(" "))[1]===o&&(a=l[u+" "+s[0]]||l["* "+s[0]])){!0===a?a=l[i]:!0!==l[i]&&(o=s[0],c.unshift(s[1]));break}if(!0!==a)if(a&&e["throws"])t=a(t);else try{t=a(t)}catch(e){return{state:"parsererror",error:a?e:"No conversion from "+u+" to "+o}}}return{state:"success",data:t}}w.extend({active:0,lastModified:{},etag:{},ajaxSettings:{url:Ct.href,type:"GET",isLocal:Pt.test(Ct.protocol),global:!0,processData:!0,async:!0,contentType:"application/x-www-form-urlencoded; charset=UTF-8",accepts:{"*":$t,text:"text/plain",html:"text/html",xml:"application/xml, text/xml",json:"application/json, text/javascript"},contents:{xml:/\bxml\b/,html:/\bhtml/,json:/\bjson\b/},responseFields:{xml:"responseXML",text:"responseText",json:"responseJSON"},converters:{"* text":String,"text html":!0,"text json":JSON.parse,"text xml":w.parseXML},flatOptions:{url:!0,context:!0}},ajaxSetup:function(e,t){return t?zt(zt(e,w.ajaxSettings),t):zt(w.ajaxSettings,e)},ajaxPrefilter:Ft(It),ajaxTransport:Ft(Wt),ajax:function(t,n){"object"==typeof t&&(n=t,t=void 0),n=n||{};var i,o,a,s,u,l,c,f,p,d,h=w.ajaxSetup({},n),g=h.context||h,y=h.context&&(g.nodeType||g.jquery)?w(g):w.event,v=w.Deferred(),m=w.Callbacks("once memory"),x=h.statusCode||{},b={},T={},C="canceled",E={readyState:0,getResponseHeader:function(e){var t;if(c){if(!s){s={};while(t=Ot.exec(a))s[t[1].toLowerCase()]=t[2]}t=s[e.toLowerCase()]}return null==t?null:t},getAllResponseHeaders:function(){return c?a:null},setRequestHeader:function(e,t){return null==c&&(e=T[e.toLowerCase()]=T[e.toLowerCase()]||e,b[e]=t),this},overrideMimeType:function(e){return null==c&&(h.mimeType=e),this},statusCode:function(e){var t;if(e)if(c)E.always(e[E.status]);else for(t in e)x[t]=[x[t],e[t]];return this},abort:function(e){var t=e||C;return i&&i.abort(t),k(0,t),this}};if(v.promise(E),h.url=((t||h.url||Ct.href)+"").replace(Rt,Ct.protocol+"//"),h.type=n.method||n.type||h.method||h.type,h.dataTypes=(h.dataType||"*").toLowerCase().match(M)||[""],null==h.crossDomain){l=r.createElement("a");try{l.href=h.url,l.href=l.href,h.crossDomain=Bt.protocol+"//"+Bt.host!=l.protocol+"//"+l.host}catch(e){h.crossDomain=!0}}if(h.data&&h.processData&&"string"!=typeof h.data&&(h.data=w.param(h.data,h.traditional)),_t(It,h,n,E),c)return E;(f=w.event&&h.global)&&0==w.active++&&w.event.trigger("ajaxStart"),h.type=h.type.toUpperCase(),h.hasContent=!Mt.test(h.type),o=h.url.replace(Lt,""),h.hasContent?h.data&&h.processData&&0===(h.contentType||"").indexOf("application/x-www-form-urlencoded")&&(h.data=h.data.replace(qt,"+")):(d=h.url.slice(o.length),h.data&&(h.processData||"string"==typeof h.data)&&(o+=(kt.test(o)?"&":"?")+h.data,delete h.data),!1===h.cache&&(o=o.replace(Ht,"$1"),d=(kt.test(o)?"&":"?")+"_="+Et+++d),h.url=o+d),h.ifModified&&(w.lastModified[o]&&E.setRequestHeader("If-Modified-Since",w.lastModified[o]),w.etag[o]&&E.setRequestHeader("If-None-Match",w.etag[o])),(h.data&&h.hasContent&&!1!==h.contentType||n.contentType)&&E.setRequestHeader("Content-Type",h.contentType),E.setRequestHeader("Accept",h.dataTypes[0]&&h.accepts[h.dataTypes[0]]?h.accepts[h.dataTypes[0]]+("*"!==h.dataTypes[0]?", "+$t+"; q=0.01":""):h.accepts["*"]);for(p in h.headers)E.setRequestHeader(p,h.headers[p]);if(h.beforeSend&&(!1===h.beforeSend.call(g,E,h)||c))return E.abort();if(C="abort",m.add(h.complete),E.done(h.success),E.fail(h.error),i=_t(Wt,h,n,E)){if(E.readyState=1,f&&y.trigger("ajaxSend",[E,h]),c)return E;h.async&&h.timeout>0&&(u=e.setTimeout(function(){E.abort("timeout")},h.timeout));try{c=!1,i.send(b,k)}catch(e){if(c)throw e;k(-1,e)}}else k(-1,"No Transport");function k(t,n,r,s){var l,p,d,b,T,C=n;c||(c=!0,u&&e.clearTimeout(u),i=void 0,a=s||"",E.readyState=t>0?4:0,l=t>=200&&t<300||304===t,r&&(b=Xt(h,E,r)),b=Ut(h,b,E,l),l?(h.ifModified&&((T=E.getResponseHeader("Last-Modified"))&&(w.lastModified[o]=T),(T=E.getResponseHeader("etag"))&&(w.etag[o]=T)),204===t||"HEAD"===h.type?C="nocontent":304===t?C="notmodified":(C=b.state,p=b.data,l=!(d=b.error))):(d=C,!t&&C||(C="error",t<0&&(t=0))),E.status=t,E.statusText=(n||C)+"",l?v.resolveWith(g,[p,C,E]):v.rejectWith(g,[E,C,d]),E.statusCode(x),x=void 0,f&&y.trigger(l?"ajaxSuccess":"ajaxError",[E,h,l?p:d]),m.fireWith(g,[E,C]),f&&(y.trigger("ajaxComplete",[E,h]),--w.active||w.event.trigger("ajaxStop")))}return E},getJSON:function(e,t,n){return w.get(e,t,n,"json")},getScript:function(e,t){return w.get(e,void 0,t,"script")}}),w.each(["get","post"],function(e,t){w[t]=function(e,n,r,i){return g(n)&&(i=i||r,r=n,n=void 0),w.ajax(w.extend({url:e,type:t,dataType:i,data:n,success:r},w.isPlainObject(e)&&e))}}),w._evalUrl=function(e){return w.ajax({url:e,type:"GET",dataType:"script",cache:!0,async:!1,global:!1,"throws":!0})},w.fn.extend({wrapAll:function(e){var t;return this[0]&&(g(e)&&(e=e.call(this[0])),t=w(e,this[0].ownerDocument).eq(0).clone(!0),this[0].parentNode&&t.insertBefore(this[0]),t.map(function(){var e=this;while(e.firstElementChild)e=e.firstElementChild;return e}).append(this)),this},wrapInner:function(e){return g(e)?this.each(function(t){w(this).wrapInner(e.call(this,t))}):this.each(function(){var t=w(this),n=t.contents();n.length?n.wrapAll(e):t.append(e)})},wrap:function(e){var t=g(e);return this.each(function(n){w(this).wrapAll(t?e.call(this,n):e)})},unwrap:function(e){return this.parent(e).not("body").each(function(){w(this).replaceWith(this.childNodes)}),this}}),w.expr.pseudos.hidden=function(e){return!w.expr.pseudos.visible(e)},w.expr.pseudos.visible=function(e){return!!(e.offsetWidth||e.offsetHeight||e.getClientRects().length)},w.ajaxSettings.xhr=function(){try{return new e.XMLHttpRequest}catch(e){}};var Vt={0:200,1223:204},Gt=w.ajaxSettings.xhr();h.cors=!!Gt&&"withCredentials"in Gt,h.ajax=Gt=!!Gt,w.ajaxTransport(function(t){var n,r;if(h.cors||Gt&&!t.crossDomain)return{send:function(i,o){var a,s=t.xhr();if(s.open(t.type,t.url,t.async,t.username,t.password),t.xhrFields)for(a in t.xhrFields)s[a]=t.xhrFields[a];t.mimeType&&s.overrideMimeType&&s.overrideMimeType(t.mimeType),t.crossDomain||i["X-Requested-With"]||(i["X-Requested-With"]="XMLHttpRequest");for(a in i)s.setRequestHeader(a,i[a]);n=function(e){return function(){n&&(n=r=s.onload=s.onerror=s.onabort=s.ontimeout=s.onreadystatechange=null,"abort"===e?s.abort():"error"===e?"number"!=typeof s.status?o(0,"error"):o(s.status,s.statusText):o(Vt[s.status]||s.status,s.statusText,"text"!==(s.responseType||"text")||"string"!=typeof s.responseText?{binary:s.response}:{text:s.responseText},s.getAllResponseHeaders()))}},s.onload=n(),r=s.onerror=s.ontimeout=n("error"),void 0!==s.onabort?s.onabort=r:s.onreadystatechange=function(){4===s.readyState&&e.setTimeout(function(){n&&r()})},n=n("abort");try{s.send(t.hasContent&&t.data||null)}catch(e){if(n)throw e}},abort:function(){n&&n()}}}),w.ajaxPrefilter(function(e){e.crossDomain&&(e.contents.script=!1)}),w.ajaxSetup({accepts:{script:"text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"},contents:{script:/\b(?:java|ecma)script\b/},converters:{"text script":function(e){return w.globalEval(e),e}}}),w.ajaxPrefilter("script",function(e){void 0===e.cache&&(e.cache=!1),e.crossDomain&&(e.type="GET")}),w.ajaxTransport("script",function(e){if(e.crossDomain){var t,n;return{send:function(i,o){t=w("<script>").prop({charset:e.scriptCharset,src:e.url}).on("load error",n=function(e){t.remove(),n=null,e&&o("error"===e.type?404:200,e.type)}),r.head.appendChild(t[0])},abort:function(){n&&n()}}}});var Yt=[],Qt=/(=)\?(?=&|$)|\?\?/;w.ajaxSetup({jsonp:"callback",jsonpCallback:function(){var e=Yt.pop()||w.expando+"_"+Et++;return this[e]=!0,e}}),w.ajaxPrefilter("json jsonp",function(t,n,r){var i,o,a,s=!1!==t.jsonp&&(Qt.test(t.url)?"url":"string"==typeof t.data&&0===(t.contentType||"").indexOf("application/x-www-form-urlencoded")&&Qt.test(t.data)&&"data");if(s||"jsonp"===t.dataTypes[0])return i=t.jsonpCallback=g(t.jsonpCallback)?t.jsonpCallback():t.jsonpCallback,s?t[s]=t[s].replace(Qt,"$1"+i):!1!==t.jsonp&&(t.url+=(kt.test(t.url)?"&":"?")+t.jsonp+"="+i),t.converters["script json"]=function(){return a||w.error(i+" was not called"),a[0]},t.dataTypes[0]="json",o=e[i],e[i]=function(){a=arguments},r.always(function(){void 0===o?w(e).removeProp(i):e[i]=o,t[i]&&(t.jsonpCallback=n.jsonpCallback,Yt.push(i)),a&&g(o)&&o(a[0]),a=o=void 0}),"script"}),h.createHTMLDocument=function(){var e=r.implementation.createHTMLDocument("").body;return e.innerHTML="<form></form><form></form>",2===e.childNodes.length}(),w.parseHTML=function(e,t,n){if("string"!=typeof e)return[];"boolean"==typeof t&&(n=t,t=!1);var i,o,a;return t||(h.createHTMLDocument?((i=(t=r.implementation.createHTMLDocument("")).createElement("base")).href=r.location.href,t.head.appendChild(i)):t=r),o=A.exec(e),a=!n&&[],o?[t.createElement(o[1])]:(o=xe([e],t,a),a&&a.length&&w(a).remove(),w.merge([],o.childNodes))},w.fn.load=function(e,t,n){var r,i,o,a=this,s=e.indexOf(" ");return s>-1&&(r=vt(e.slice(s)),e=e.slice(0,s)),g(t)?(n=t,t=void 0):t&&"object"==typeof t&&(i="POST"),a.length>0&&w.ajax({url:e,type:i||"GET",dataType:"html",data:t}).done(function(e){o=arguments,a.html(r?w("<div>").append(w.parseHTML(e)).find(r):e)}).always(n&&function(e,t){a.each(function(){n.apply(this,o||[e.responseText,t,e])})}),this},w.each(["ajaxStart","ajaxStop","ajaxComplete","ajaxError","ajaxSuccess","ajaxSend"],function(e,t){w.fn[t]=function(e){return this.on(t,e)}}),w.expr.pseudos.animated=function(e){return w.grep(w.timers,function(t){return e===t.elem}).length},w.offset={setOffset:function(e,t,n){var r,i,o,a,s,u,l,c=w.css(e,"position"),f=w(e),p={};"static"===c&&(e.style.position="relative"),s=f.offset(),o=w.css(e,"top"),u=w.css(e,"left"),(l=("absolute"===c||"fixed"===c)&&(o+u).indexOf("auto")>-1)?(a=(r=f.position()).top,i=r.left):(a=parseFloat(o)||0,i=parseFloat(u)||0),g(t)&&(t=t.call(e,n,w.extend({},s))),null!=t.top&&(p.top=t.top-s.top+a),null!=t.left&&(p.left=t.left-s.left+i),"using"in t?t.using.call(e,p):f.css(p)}},w.fn.extend({offset:function(e){if(arguments.length)return void 0===e?this:this.each(function(t){w.offset.setOffset(this,e,t)});var t,n,r=this[0];if(r)return r.getClientRects().length?(t=r.getBoundingClientRect(),n=r.ownerDocument.defaultView,{top:t.top+n.pageYOffset,left:t.left+n.pageXOffset}):{top:0,left:0}},position:function(){if(this[0]){var e,t,n,r=this[0],i={top:0,left:0};if("fixed"===w.css(r,"position"))t=r.getBoundingClientRect();else{t=this.offset(),n=r.ownerDocument,e=r.offsetParent||n.documentElement;while(e&&(e===n.body||e===n.documentElement)&&"static"===w.css(e,"position"))e=e.parentNode;e&&e!==r&&1===e.nodeType&&((i=w(e).offset()).top+=w.css(e,"borderTopWidth",!0),i.left+=w.css(e,"borderLeftWidth",!0))}return{top:t.top-i.top-w.css(r,"marginTop",!0),left:t.left-i.left-w.css(r,"marginLeft",!0)}}},offsetParent:function(){return this.map(function(){var e=this.offsetParent;while(e&&"static"===w.css(e,"position"))e=e.offsetParent;return e||be})}}),w.each({scrollLeft:"pageXOffset",scrollTop:"pageYOffset"},function(e,t){var n="pageYOffset"===t;w.fn[e]=function(r){return z(this,function(e,r,i){var o;if(y(e)?o=e:9===e.nodeType&&(o=e.defaultView),void 0===i)return o?o[t]:e[r];o?o.scrollTo(n?o.pageXOffset:i,n?i:o.pageYOffset):e[r]=i},e,r,arguments.length)}}),w.each(["top","left"],function(e,t){w.cssHooks[t]=_e(h.pixelPosition,function(e,n){if(n)return n=Fe(e,t),We.test(n)?w(e).position()[t]+"px":n})}),w.each({Height:"height",Width:"width"},function(e,t){w.each({padding:"inner"+e,content:t,"":"outer"+e},function(n,r){w.fn[r]=function(i,o){var a=arguments.length&&(n||"boolean"!=typeof i),s=n||(!0===i||!0===o?"margin":"border");return z(this,function(t,n,i){var o;return y(t)?0===r.indexOf("outer")?t["inner"+e]:t.document.documentElement["client"+e]:9===t.nodeType?(o=t.documentElement,Math.max(t.body["scroll"+e],o["scroll"+e],t.body["offset"+e],o["offset"+e],o["client"+e])):void 0===i?w.css(t,n,s):w.style(t,n,i,s)},t,a?i:void 0,a)}})}),w.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "),function(e,t){w.fn[t]=function(e,n){return arguments.length>0?this.on(t,null,e,n):this.trigger(t)}}),w.fn.extend({hover:function(e,t){return this.mouseenter(e).mouseleave(t||e)}}),w.fn.extend({bind:function(e,t,n){return this.on(e,null,t,n)},unbind:function(e,t){return this.off(e,null,t)},delegate:function(e,t,n,r){return this.on(t,e,n,r)},undelegate:function(e,t,n){return 1===arguments.length?this.off(e,"**"):this.off(t,e||"**",n)}}),w.proxy=function(e,t){var n,r,i;if("string"==typeof t&&(n=e[t],t=e,e=n),g(e))return r=o.call(arguments,2),i=function(){return e.apply(t||this,r.concat(o.call(arguments)))},i.guid=e.guid=e.guid||w.guid++,i},w.holdReady=function(e){e?w.readyWait++:w.ready(!0)},w.isArray=Array.isArray,w.parseJSON=JSON.parse,w.nodeName=N,w.isFunction=g,w.isWindow=y,w.camelCase=G,w.type=x,w.now=Date.now,w.isNumeric=function(e){var t=w.type(e);return("number"===t||"string"===t)&&!isNaN(e-parseFloat(e))},"function"==typeof define&&define.amd&&define("jquery",[],function(){return w});var Jt=e.jQuery,Kt=e.$;return w.noConflict=function(t){return e.$===w&&(e.$=Kt),t&&e.jQuery===w&&(e.jQuery=Jt),w},t||(e.jQuery=e.$=w),w});
+<script type="text/javascript">
+/*! jQuery v3.5.1 | (c) JS Foundation and other contributors | jquery.org/license */
+!function(e,t){"use strict";"object"==typeof module&&"object"==typeof module.exports?module.exports=e.document?t(e,!0):function(e){if(!e.document)throw new Error("jQuery requires a window with a document");return t(e)}:t(e)}("undefined"!=typeof window?window:this,function(C,e){"use strict";var t=[],r=Object.getPrototypeOf,s=t.slice,g=t.flat?function(e){return t.flat.call(e)}:function(e){return t.concat.apply([],e)},u=t.push,i=t.indexOf,n={},o=n.toString,v=n.hasOwnProperty,a=v.toString,l=a.call(Object),y={},m=function(e){return"function"==typeof e&&"number"!=typeof e.nodeType},x=function(e){return null!=e&&e===e.window},E=C.document,c={type:!0,src:!0,nonce:!0,noModule:!0};function b(e,t,n){var r,i,o=(n=n||E).createElement("script");if(o.text=e,t)for(r in c)(i=t[r]||t.getAttribute&&t.getAttribute(r))&&o.setAttribute(r,i);n.head.appendChild(o).parentNode.removeChild(o)}function w(e){return null==e?e+"":"object"==typeof e||"function"==typeof e?n[o.call(e)]||"object":typeof e}var f="3.5.1",S=function(e,t){return new S.fn.init(e,t)};function p(e){var t=!!e&&"length"in e&&e.length,n=w(e);return!m(e)&&!x(e)&&("array"===n||0===t||"number"==typeof t&&0<t&&t-1 in e)}S.fn=S.prototype={jquery:f,constructor:S,length:0,toArray:function(){return s.call(this)},get:function(e){return null==e?s.call(this):e<0?this[e+this.length]:this[e]},pushStack:function(e){var t=S.merge(this.constructor(),e);return t.prevObject=this,t},each:function(e){return S.each(this,e)},map:function(n){return this.pushStack(S.map(this,function(e,t){return n.call(e,t,e)}))},slice:function(){return this.pushStack(s.apply(this,arguments))},first:function(){return this.eq(0)},last:function(){return this.eq(-1)},even:function(){return this.pushStack(S.grep(this,function(e,t){return(t+1)%2}))},odd:function(){return this.pushStack(S.grep(this,function(e,t){return t%2}))},eq:function(e){var t=this.length,n=+e+(e<0?t:0);return this.pushStack(0<=n&&n<t?[this[n]]:[])},end:function(){return this.prevObject||this.constructor()},push:u,sort:t.sort,splice:t.splice},S.extend=S.fn.extend=function(){var e,t,n,r,i,o,a=arguments[0]||{},s=1,u=arguments.length,l=!1;for("boolean"==typeof a&&(l=a,a=arguments[s]||{},s++),"object"==typeof a||m(a)||(a={}),s===u&&(a=this,s--);s<u;s++)if(null!=(e=arguments[s]))for(t in e)r=e[t],"__proto__"!==t&&a!==r&&(l&&r&&(S.isPlainObject(r)||(i=Array.isArray(r)))?(n=a[t],o=i&&!Array.isArray(n)?[]:i||S.isPlainObject(n)?n:{},i=!1,a[t]=S.extend(l,o,r)):void 0!==r&&(a[t]=r));return a},S.extend({expando:"jQuery"+(f+Math.random()).replace(/\D/g,""),isReady:!0,error:function(e){throw new Error(e)},noop:function(){},isPlainObject:function(e){var t,n;return!(!e||"[object Object]"!==o.call(e))&&(!(t=r(e))||"function"==typeof(n=v.call(t,"constructor")&&t.constructor)&&a.call(n)===l)},isEmptyObject:function(e){var t;for(t in e)return!1;return!0},globalEval:function(e,t,n){b(e,{nonce:t&&t.nonce},n)},each:function(e,t){var n,r=0;if(p(e)){for(n=e.length;r<n;r++)if(!1===t.call(e[r],r,e[r]))break}else for(r in e)if(!1===t.call(e[r],r,e[r]))break;return e},makeArray:function(e,t){var n=t||[];return null!=e&&(p(Object(e))?S.merge(n,"string"==typeof e?[e]:e):u.call(n,e)),n},inArray:function(e,t,n){return null==t?-1:i.call(t,e,n)},merge:function(e,t){for(var n=+t.length,r=0,i=e.length;r<n;r++)e[i++]=t[r];return e.length=i,e},grep:function(e,t,n){for(var r=[],i=0,o=e.length,a=!n;i<o;i++)!t(e[i],i)!==a&&r.push(e[i]);return r},map:function(e,t,n){var r,i,o=0,a=[];if(p(e))for(r=e.length;o<r;o++)null!=(i=t(e[o],o,n))&&a.push(i);else for(o in e)null!=(i=t(e[o],o,n))&&a.push(i);return g(a)},guid:1,support:y}),"function"==typeof Symbol&&(S.fn[Symbol.iterator]=t[Symbol.iterator]),S.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "),function(e,t){n["[object "+t+"]"]=t.toLowerCase()});var d=function(n){var e,d,b,o,i,h,f,g,w,u,l,T,C,a,E,v,s,c,y,S="sizzle"+1*new Date,p=n.document,k=0,r=0,m=ue(),x=ue(),A=ue(),N=ue(),D=function(e,t){return e===t&&(l=!0),0},j={}.hasOwnProperty,t=[],q=t.pop,L=t.push,H=t.push,O=t.slice,P=function(e,t){for(var n=0,r=e.length;n<r;n++)if(e[n]===t)return n;return-1},R="checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",M="[\\x20\\t\\r\\n\\f]",I="(?:\\\\[\\da-fA-F]{1,6}"+M+"?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",W="\\["+M+"*("+I+")(?:"+M+"*([*^$|!~]?=)"+M+"*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|("+I+"))|)"+M+"*\\]",F=":("+I+")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|"+W+")*)|.*)\\)|)",B=new RegExp(M+"+","g"),$=new RegExp("^"+M+"+|((?:^|[^\\\\])(?:\\\\.)*)"+M+"+$","g"),_=new RegExp("^"+M+"*,"+M+"*"),z=new RegExp("^"+M+"*([>+~]|"+M+")"+M+"*"),U=new RegExp(M+"|>"),X=new RegExp(F),V=new RegExp("^"+I+"$"),G={ID:new RegExp("^#("+I+")"),CLASS:new RegExp("^\\.("+I+")"),TAG:new RegExp("^("+I+"|[*])"),ATTR:new RegExp("^"+W),PSEUDO:new RegExp("^"+F),CHILD:new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\("+M+"*(even|odd|(([+-]|)(\\d*)n|)"+M+"*(?:([+-]|)"+M+"*(\\d+)|))"+M+"*\\)|)","i"),bool:new RegExp("^(?:"+R+")$","i"),needsContext:new RegExp("^"+M+"*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\("+M+"*((?:-\\d)?\\d*)"+M+"*\\)|)(?=[^-]|$)","i")},Y=/HTML$/i,Q=/^(?:input|select|textarea|button)$/i,J=/^h\d$/i,K=/^[^{]+\{\s*\[native \w/,Z=/^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,ee=/[+~]/,te=new RegExp("\\\\[\\da-fA-F]{1,6}"+M+"?|\\\\([^\\r\\n\\f])","g"),ne=function(e,t){var n="0x"+e.slice(1)-65536;return t||(n<0?String.fromCharCode(n+65536):String.fromCharCode(n>>10|55296,1023&n|56320))},re=/([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,ie=function(e,t){return t?"\0"===e?"\ufffd":e.slice(0,-1)+"\\"+e.charCodeAt(e.length-1).toString(16)+" ":"\\"+e},oe=function(){T()},ae=be(function(e){return!0===e.disabled&&"fieldset"===e.nodeName.toLowerCase()},{dir:"parentNode",next:"legend"});try{H.apply(t=O.call(p.childNodes),p.childNodes),t[p.childNodes.length].nodeType}catch(e){H={apply:t.length?function(e,t){L.apply(e,O.call(t))}:function(e,t){var n=e.length,r=0;while(e[n++]=t[r++]);e.length=n-1}}}function se(t,e,n,r){var i,o,a,s,u,l,c,f=e&&e.ownerDocument,p=e?e.nodeType:9;if(n=n||[],"string"!=typeof t||!t||1!==p&&9!==p&&11!==p)return n;if(!r&&(T(e),e=e||C,E)){if(11!==p&&(u=Z.exec(t)))if(i=u[1]){if(9===p){if(!(a=e.getElementById(i)))return n;if(a.id===i)return n.push(a),n}else if(f&&(a=f.getElementById(i))&&y(e,a)&&a.id===i)return n.push(a),n}else{if(u[2])return H.apply(n,e.getElementsByTagName(t)),n;if((i=u[3])&&d.getElementsByClassName&&e.getElementsByClassName)return H.apply(n,e.getElementsByClassName(i)),n}if(d.qsa&&!N[t+" "]&&(!v||!v.test(t))&&(1!==p||"object"!==e.nodeName.toLowerCase())){if(c=t,f=e,1===p&&(U.test(t)||z.test(t))){(f=ee.test(t)&&ye(e.parentNode)||e)===e&&d.scope||((s=e.getAttribute("id"))?s=s.replace(re,ie):e.setAttribute("id",s=S)),o=(l=h(t)).length;while(o--)l[o]=(s?"#"+s:":scope")+" "+xe(l[o]);c=l.join(",")}try{return H.apply(n,f.querySelectorAll(c)),n}catch(e){N(t,!0)}finally{s===S&&e.removeAttribute("id")}}}return g(t.replace($,"$1"),e,n,r)}function ue(){var r=[];return function e(t,n){return r.push(t+" ")>b.cacheLength&&delete e[r.shift()],e[t+" "]=n}}function le(e){return e[S]=!0,e}function ce(e){var t=C.createElement("fieldset");try{return!!e(t)}catch(e){return!1}finally{t.parentNode&&t.parentNode.removeChild(t),t=null}}function fe(e,t){var n=e.split("|"),r=n.length;while(r--)b.attrHandle[n[r]]=t}function pe(e,t){var n=t&&e,r=n&&1===e.nodeType&&1===t.nodeType&&e.sourceIndex-t.sourceIndex;if(r)return r;if(n)while(n=n.nextSibling)if(n===t)return-1;return e?1:-1}function de(t){return function(e){return"input"===e.nodeName.toLowerCase()&&e.type===t}}function he(n){return function(e){var t=e.nodeName.toLowerCase();return("input"===t||"button"===t)&&e.type===n}}function ge(t){return function(e){return"form"in e?e.parentNode&&!1===e.disabled?"label"in e?"label"in e.parentNode?e.parentNode.disabled===t:e.disabled===t:e.isDisabled===t||e.isDisabled!==!t&&ae(e)===t:e.disabled===t:"label"in e&&e.disabled===t}}function ve(a){return le(function(o){return o=+o,le(function(e,t){var n,r=a([],e.length,o),i=r.length;while(i--)e[n=r[i]]&&(e[n]=!(t[n]=e[n]))})})}function ye(e){return e&&"undefined"!=typeof e.getElementsByTagName&&e}for(e in d=se.support={},i=se.isXML=function(e){var t=e.namespaceURI,n=(e.ownerDocument||e).documentElement;return!Y.test(t||n&&n.nodeName||"HTML")},T=se.setDocument=function(e){var t,n,r=e?e.ownerDocument||e:p;return r!=C&&9===r.nodeType&&r.documentElement&&(a=(C=r).documentElement,E=!i(C),p!=C&&(n=C.defaultView)&&n.top!==n&&(n.addEventListener?n.addEventListener("unload",oe,!1):n.attachEvent&&n.attachEvent("onunload",oe)),d.scope=ce(function(e){return a.appendChild(e).appendChild(C.createElement("div")),"undefined"!=typeof e.querySelectorAll&&!e.querySelectorAll(":scope fieldset div").length}),d.attributes=ce(function(e){return e.className="i",!e.getAttribute("className")}),d.getElementsByTagName=ce(function(e){return e.appendChild(C.createComment("")),!e.getElementsByTagName("*").length}),d.getElementsByClassName=K.test(C.getElementsByClassName),d.getById=ce(function(e){return a.appendChild(e).id=S,!C.getElementsByName||!C.getElementsByName(S).length}),d.getById?(b.filter.ID=function(e){var t=e.replace(te,ne);return function(e){return e.getAttribute("id")===t}},b.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&E){var n=t.getElementById(e);return n?[n]:[]}}):(b.filter.ID=function(e){var n=e.replace(te,ne);return function(e){var t="undefined"!=typeof e.getAttributeNode&&e.getAttributeNode("id");return t&&t.value===n}},b.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&E){var n,r,i,o=t.getElementById(e);if(o){if((n=o.getAttributeNode("id"))&&n.value===e)return[o];i=t.getElementsByName(e),r=0;while(o=i[r++])if((n=o.getAttributeNode("id"))&&n.value===e)return[o]}return[]}}),b.find.TAG=d.getElementsByTagName?function(e,t){return"undefined"!=typeof t.getElementsByTagName?t.getElementsByTagName(e):d.qsa?t.querySelectorAll(e):void 0}:function(e,t){var n,r=[],i=0,o=t.getElementsByTagName(e);if("*"===e){while(n=o[i++])1===n.nodeType&&r.push(n);return r}return o},b.find.CLASS=d.getElementsByClassName&&function(e,t){if("undefined"!=typeof t.getElementsByClassName&&E)return t.getElementsByClassName(e)},s=[],v=[],(d.qsa=K.test(C.querySelectorAll))&&(ce(function(e){var t;a.appendChild(e).innerHTML="<a id='"+S+"'></a><select id='"+S+"-\r\\' msallowcapture=''><option selected=''></option></select>",e.querySelectorAll("[msallowcapture^='']").length&&v.push("[*^$]="+M+"*(?:''|\"\")"),e.querySelectorAll("[selected]").length||v.push("\\["+M+"*(?:value|"+R+")"),e.querySelectorAll("[id~="+S+"-]").length||v.push("~="),(t=C.createElement("input")).setAttribute("name",""),e.appendChild(t),e.querySelectorAll("[name='']").length||v.push("\\["+M+"*name"+M+"*="+M+"*(?:''|\"\")"),e.querySelectorAll(":checked").length||v.push(":checked"),e.querySelectorAll("a#"+S+"+*").length||v.push(".#.+[+~]"),e.querySelectorAll("\\\f"),v.push("[\\r\\n\\f]")}),ce(function(e){e.innerHTML="<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";var t=C.createElement("input");t.setAttribute("type","hidden"),e.appendChild(t).setAttribute("name","D"),e.querySelectorAll("[name=d]").length&&v.push("name"+M+"*[*^$|!~]?="),2!==e.querySelectorAll(":enabled").length&&v.push(":enabled",":disabled"),a.appendChild(e).disabled=!0,2!==e.querySelectorAll(":disabled").length&&v.push(":enabled",":disabled"),e.querySelectorAll("*,:x"),v.push(",.*:")})),(d.matchesSelector=K.test(c=a.matches||a.webkitMatchesSelector||a.mozMatchesSelector||a.oMatchesSelector||a.msMatchesSelector))&&ce(function(e){d.disconnectedMatch=c.call(e,"*"),c.call(e,"[s!='']:x"),s.push("!=",F)}),v=v.length&&new RegExp(v.join("|")),s=s.length&&new RegExp(s.join("|")),t=K.test(a.compareDocumentPosition),y=t||K.test(a.contains)?function(e,t){var n=9===e.nodeType?e.documentElement:e,r=t&&t.parentNode;return e===r||!(!r||1!==r.nodeType||!(n.contains?n.contains(r):e.compareDocumentPosition&&16&e.compareDocumentPosition(r)))}:function(e,t){if(t)while(t=t.parentNode)if(t===e)return!0;return!1},D=t?function(e,t){if(e===t)return l=!0,0;var n=!e.compareDocumentPosition-!t.compareDocumentPosition;return n||(1&(n=(e.ownerDocument||e)==(t.ownerDocument||t)?e.compareDocumentPosition(t):1)||!d.sortDetached&&t.compareDocumentPosition(e)===n?e==C||e.ownerDocument==p&&y(p,e)?-1:t==C||t.ownerDocument==p&&y(p,t)?1:u?P(u,e)-P(u,t):0:4&n?-1:1)}:function(e,t){if(e===t)return l=!0,0;var n,r=0,i=e.parentNode,o=t.parentNode,a=[e],s=[t];if(!i||!o)return e==C?-1:t==C?1:i?-1:o?1:u?P(u,e)-P(u,t):0;if(i===o)return pe(e,t);n=e;while(n=n.parentNode)a.unshift(n);n=t;while(n=n.parentNode)s.unshift(n);while(a[r]===s[r])r++;return r?pe(a[r],s[r]):a[r]==p?-1:s[r]==p?1:0}),C},se.matches=function(e,t){return se(e,null,null,t)},se.matchesSelector=function(e,t){if(T(e),d.matchesSelector&&E&&!N[t+" "]&&(!s||!s.test(t))&&(!v||!v.test(t)))try{var n=c.call(e,t);if(n||d.disconnectedMatch||e.document&&11!==e.document.nodeType)return n}catch(e){N(t,!0)}return 0<se(t,C,null,[e]).length},se.contains=function(e,t){return(e.ownerDocument||e)!=C&&T(e),y(e,t)},se.attr=function(e,t){(e.ownerDocument||e)!=C&&T(e);var n=b.attrHandle[t.toLowerCase()],r=n&&j.call(b.attrHandle,t.toLowerCase())?n(e,t,!E):void 0;return void 0!==r?r:d.attributes||!E?e.getAttribute(t):(r=e.getAttributeNode(t))&&r.specified?r.value:null},se.escape=function(e){return(e+"").replace(re,ie)},se.error=function(e){throw new Error("Syntax error, unrecognized expression: "+e)},se.uniqueSort=function(e){var t,n=[],r=0,i=0;if(l=!d.detectDuplicates,u=!d.sortStable&&e.slice(0),e.sort(D),l){while(t=e[i++])t===e[i]&&(r=n.push(i));while(r--)e.splice(n[r],1)}return u=null,e},o=se.getText=function(e){var t,n="",r=0,i=e.nodeType;if(i){if(1===i||9===i||11===i){if("string"==typeof e.textContent)return e.textContent;for(e=e.firstChild;e;e=e.nextSibling)n+=o(e)}else if(3===i||4===i)return e.nodeValue}else while(t=e[r++])n+=o(t);return n},(b=se.selectors={cacheLength:50,createPseudo:le,match:G,attrHandle:{},find:{},relative:{">":{dir:"parentNode",first:!0}," ":{dir:"parentNode"},"+":{dir:"previousSibling",first:!0},"~":{dir:"previousSibling"}},preFilter:{ATTR:function(e){return e[1]=e[1].replace(te,ne),e[3]=(e[3]||e[4]||e[5]||"").replace(te,ne),"~="===e[2]&&(e[3]=" "+e[3]+" "),e.slice(0,4)},CHILD:function(e){return e[1]=e[1].toLowerCase(),"nth"===e[1].slice(0,3)?(e[3]||se.error(e[0]),e[4]=+(e[4]?e[5]+(e[6]||1):2*("even"===e[3]||"odd"===e[3])),e[5]=+(e[7]+e[8]||"odd"===e[3])):e[3]&&se.error(e[0]),e},PSEUDO:function(e){var t,n=!e[6]&&e[2];return G.CHILD.test(e[0])?null:(e[3]?e[2]=e[4]||e[5]||"":n&&X.test(n)&&(t=h(n,!0))&&(t=n.indexOf(")",n.length-t)-n.length)&&(e[0]=e[0].slice(0,t),e[2]=n.slice(0,t)),e.slice(0,3))}},filter:{TAG:function(e){var t=e.replace(te,ne).toLowerCase();return"*"===e?function(){return!0}:function(e){return e.nodeName&&e.nodeName.toLowerCase()===t}},CLASS:function(e){var t=m[e+" "];return t||(t=new RegExp("(^|"+M+")"+e+"("+M+"|$)"))&&m(e,function(e){return t.test("string"==typeof e.className&&e.className||"undefined"!=typeof e.getAttribute&&e.getAttribute("class")||"")})},ATTR:function(n,r,i){return function(e){var t=se.attr(e,n);return null==t?"!="===r:!r||(t+="","="===r?t===i:"!="===r?t!==i:"^="===r?i&&0===t.indexOf(i):"*="===r?i&&-1<t.indexOf(i):"$="===r?i&&t.slice(-i.length)===i:"~="===r?-1<(" "+t.replace(B," ")+" ").indexOf(i):"|="===r&&(t===i||t.slice(0,i.length+1)===i+"-"))}},CHILD:function(h,e,t,g,v){var y="nth"!==h.slice(0,3),m="last"!==h.slice(-4),x="of-type"===e;return 1===g&&0===v?function(e){return!!e.parentNode}:function(e,t,n){var r,i,o,a,s,u,l=y!==m?"nextSibling":"previousSibling",c=e.parentNode,f=x&&e.nodeName.toLowerCase(),p=!n&&!x,d=!1;if(c){if(y){while(l){a=e;while(a=a[l])if(x?a.nodeName.toLowerCase()===f:1===a.nodeType)return!1;u=l="only"===h&&!u&&"nextSibling"}return!0}if(u=[m?c.firstChild:c.lastChild],m&&p){d=(s=(r=(i=(o=(a=c)[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]||[])[0]===k&&r[1])&&r[2],a=s&&c.childNodes[s];while(a=++s&&a&&a[l]||(d=s=0)||u.pop())if(1===a.nodeType&&++d&&a===e){i[h]=[k,s,d];break}}else if(p&&(d=s=(r=(i=(o=(a=e)[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]||[])[0]===k&&r[1]),!1===d)while(a=++s&&a&&a[l]||(d=s=0)||u.pop())if((x?a.nodeName.toLowerCase()===f:1===a.nodeType)&&++d&&(p&&((i=(o=a[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]=[k,d]),a===e))break;return(d-=v)===g||d%g==0&&0<=d/g}}},PSEUDO:function(e,o){var t,a=b.pseudos[e]||b.setFilters[e.toLowerCase()]||se.error("unsupported pseudo: "+e);return a[S]?a(o):1<a.length?(t=[e,e,"",o],b.setFilters.hasOwnProperty(e.toLowerCase())?le(function(e,t){var n,r=a(e,o),i=r.length;while(i--)e[n=P(e,r[i])]=!(t[n]=r[i])}):function(e){return a(e,0,t)}):a}},pseudos:{not:le(function(e){var r=[],i=[],s=f(e.replace($,"$1"));return s[S]?le(function(e,t,n,r){var i,o=s(e,null,r,[]),a=e.length;while(a--)(i=o[a])&&(e[a]=!(t[a]=i))}):function(e,t,n){return r[0]=e,s(r,null,n,i),r[0]=null,!i.pop()}}),has:le(function(t){return function(e){return 0<se(t,e).length}}),contains:le(function(t){return t=t.replace(te,ne),function(e){return-1<(e.textContent||o(e)).indexOf(t)}}),lang:le(function(n){return V.test(n||"")||se.error("unsupported lang: "+n),n=n.replace(te,ne).toLowerCase(),function(e){var t;do{if(t=E?e.lang:e.getAttribute("xml:lang")||e.getAttribute("lang"))return(t=t.toLowerCase())===n||0===t.indexOf(n+"-")}while((e=e.parentNode)&&1===e.nodeType);return!1}}),target:function(e){var t=n.location&&n.location.hash;return t&&t.slice(1)===e.id},root:function(e){return e===a},focus:function(e){return e===C.activeElement&&(!C.hasFocus||C.hasFocus())&&!!(e.type||e.href||~e.tabIndex)},enabled:ge(!1),disabled:ge(!0),checked:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&!!e.checked||"option"===t&&!!e.selected},selected:function(e){return e.parentNode&&e.parentNode.selectedIndex,!0===e.selected},empty:function(e){for(e=e.firstChild;e;e=e.nextSibling)if(e.nodeType<6)return!1;return!0},parent:function(e){return!b.pseudos.empty(e)},header:function(e){return J.test(e.nodeName)},input:function(e){return Q.test(e.nodeName)},button:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&"button"===e.type||"button"===t},text:function(e){var t;return"input"===e.nodeName.toLowerCase()&&"text"===e.type&&(null==(t=e.getAttribute("type"))||"text"===t.toLowerCase())},first:ve(function(){return[0]}),last:ve(function(e,t){return[t-1]}),eq:ve(function(e,t,n){return[n<0?n+t:n]}),even:ve(function(e,t){for(var n=0;n<t;n+=2)e.push(n);return e}),odd:ve(function(e,t){for(var n=1;n<t;n+=2)e.push(n);return e}),lt:ve(function(e,t,n){for(var r=n<0?n+t:t<n?t:n;0<=--r;)e.push(r);return e}),gt:ve(function(e,t,n){for(var r=n<0?n+t:n;++r<t;)e.push(r);return e})}}).pseudos.nth=b.pseudos.eq,{radio:!0,checkbox:!0,file:!0,password:!0,image:!0})b.pseudos[e]=de(e);for(e in{submit:!0,reset:!0})b.pseudos[e]=he(e);function me(){}function xe(e){for(var t=0,n=e.length,r="";t<n;t++)r+=e[t].value;return r}function be(s,e,t){var u=e.dir,l=e.next,c=l||u,f=t&&"parentNode"===c,p=r++;return e.first?function(e,t,n){while(e=e[u])if(1===e.nodeType||f)return s(e,t,n);return!1}:function(e,t,n){var r,i,o,a=[k,p];if(n){while(e=e[u])if((1===e.nodeType||f)&&s(e,t,n))return!0}else while(e=e[u])if(1===e.nodeType||f)if(i=(o=e[S]||(e[S]={}))[e.uniqueID]||(o[e.uniqueID]={}),l&&l===e.nodeName.toLowerCase())e=e[u]||e;else{if((r=i[c])&&r[0]===k&&r[1]===p)return a[2]=r[2];if((i[c]=a)[2]=s(e,t,n))return!0}return!1}}function we(i){return 1<i.length?function(e,t,n){var r=i.length;while(r--)if(!i[r](e,t,n))return!1;return!0}:i[0]}function Te(e,t,n,r,i){for(var o,a=[],s=0,u=e.length,l=null!=t;s<u;s++)(o=e[s])&&(n&&!n(o,r,i)||(a.push(o),l&&t.push(s)));return a}function Ce(d,h,g,v,y,e){return v&&!v[S]&&(v=Ce(v)),y&&!y[S]&&(y=Ce(y,e)),le(function(e,t,n,r){var i,o,a,s=[],u=[],l=t.length,c=e||function(e,t,n){for(var r=0,i=t.length;r<i;r++)se(e,t[r],n);return n}(h||"*",n.nodeType?[n]:n,[]),f=!d||!e&&h?c:Te(c,s,d,n,r),p=g?y||(e?d:l||v)?[]:t:f;if(g&&g(f,p,n,r),v){i=Te(p,u),v(i,[],n,r),o=i.length;while(o--)(a=i[o])&&(p[u[o]]=!(f[u[o]]=a))}if(e){if(y||d){if(y){i=[],o=p.length;while(o--)(a=p[o])&&i.push(f[o]=a);y(null,p=[],i,r)}o=p.length;while(o--)(a=p[o])&&-1<(i=y?P(e,a):s[o])&&(e[i]=!(t[i]=a))}}else p=Te(p===t?p.splice(l,p.length):p),y?y(null,t,p,r):H.apply(t,p)})}function Ee(e){for(var i,t,n,r=e.length,o=b.relative[e[0].type],a=o||b.relative[" "],s=o?1:0,u=be(function(e){return e===i},a,!0),l=be(function(e){return-1<P(i,e)},a,!0),c=[function(e,t,n){var r=!o&&(n||t!==w)||((i=t).nodeType?u(e,t,n):l(e,t,n));return i=null,r}];s<r;s++)if(t=b.relative[e[s].type])c=[be(we(c),t)];else{if((t=b.filter[e[s].type].apply(null,e[s].matches))[S]){for(n=++s;n<r;n++)if(b.relative[e[n].type])break;return Ce(1<s&&we(c),1<s&&xe(e.slice(0,s-1).concat({value:" "===e[s-2].type?"*":""})).replace($,"$1"),t,s<n&&Ee(e.slice(s,n)),n<r&&Ee(e=e.slice(n)),n<r&&xe(e))}c.push(t)}return we(c)}return me.prototype=b.filters=b.pseudos,b.setFilters=new me,h=se.tokenize=function(e,t){var n,r,i,o,a,s,u,l=x[e+" "];if(l)return t?0:l.slice(0);a=e,s=[],u=b.preFilter;while(a){for(o in n&&!(r=_.exec(a))||(r&&(a=a.slice(r[0].length)||a),s.push(i=[])),n=!1,(r=z.exec(a))&&(n=r.shift(),i.push({value:n,type:r[0].replace($," ")}),a=a.slice(n.length)),b.filter)!(r=G[o].exec(a))||u[o]&&!(r=u[o](r))||(n=r.shift(),i.push({value:n,type:o,matches:r}),a=a.slice(n.length));if(!n)break}return t?a.length:a?se.error(e):x(e,s).slice(0)},f=se.compile=function(e,t){var n,v,y,m,x,r,i=[],o=[],a=A[e+" "];if(!a){t||(t=h(e)),n=t.length;while(n--)(a=Ee(t[n]))[S]?i.push(a):o.push(a);(a=A(e,(v=o,m=0<(y=i).length,x=0<v.length,r=function(e,t,n,r,i){var o,a,s,u=0,l="0",c=e&&[],f=[],p=w,d=e||x&&b.find.TAG("*",i),h=k+=null==p?1:Math.random()||.1,g=d.length;for(i&&(w=t==C||t||i);l!==g&&null!=(o=d[l]);l++){if(x&&o){a=0,t||o.ownerDocument==C||(T(o),n=!E);while(s=v[a++])if(s(o,t||C,n)){r.push(o);break}i&&(k=h)}m&&((o=!s&&o)&&u--,e&&c.push(o))}if(u+=l,m&&l!==u){a=0;while(s=y[a++])s(c,f,t,n);if(e){if(0<u)while(l--)c[l]||f[l]||(f[l]=q.call(r));f=Te(f)}H.apply(r,f),i&&!e&&0<f.length&&1<u+y.length&&se.uniqueSort(r)}return i&&(k=h,w=p),c},m?le(r):r))).selector=e}return a},g=se.select=function(e,t,n,r){var i,o,a,s,u,l="function"==typeof e&&e,c=!r&&h(e=l.selector||e);if(n=n||[],1===c.length){if(2<(o=c[0]=c[0].slice(0)).length&&"ID"===(a=o[0]).type&&9===t.nodeType&&E&&b.relative[o[1].type]){if(!(t=(b.find.ID(a.matches[0].replace(te,ne),t)||[])[0]))return n;l&&(t=t.parentNode),e=e.slice(o.shift().value.length)}i=G.needsContext.test(e)?0:o.length;while(i--){if(a=o[i],b.relative[s=a.type])break;if((u=b.find[s])&&(r=u(a.matches[0].replace(te,ne),ee.test(o[0].type)&&ye(t.parentNode)||t))){if(o.splice(i,1),!(e=r.length&&xe(o)))return H.apply(n,r),n;break}}}return(l||f(e,c))(r,t,!E,n,!t||ee.test(e)&&ye(t.parentNode)||t),n},d.sortStable=S.split("").sort(D).join("")===S,d.detectDuplicates=!!l,T(),d.sortDetached=ce(function(e){return 1&e.compareDocumentPosition(C.createElement("fieldset"))}),ce(function(e){return e.innerHTML="<a href='#'></a>","#"===e.firstChild.getAttribute("href")})||fe("type|href|height|width",function(e,t,n){if(!n)return e.getAttribute(t,"type"===t.toLowerCase()?1:2)}),d.attributes&&ce(function(e){return e.innerHTML="<input/>",e.firstChild.setAttribute("value",""),""===e.firstChild.getAttribute("value")})||fe("value",function(e,t,n){if(!n&&"input"===e.nodeName.toLowerCase())return e.defaultValue}),ce(function(e){return null==e.getAttribute("disabled")})||fe(R,function(e,t,n){var r;if(!n)return!0===e[t]?t.toLowerCase():(r=e.getAttributeNode(t))&&r.specified?r.value:null}),se}(C);S.find=d,S.expr=d.selectors,S.expr[":"]=S.expr.pseudos,S.uniqueSort=S.unique=d.uniqueSort,S.text=d.getText,S.isXMLDoc=d.isXML,S.contains=d.contains,S.escapeSelector=d.escape;var h=function(e,t,n){var r=[],i=void 0!==n;while((e=e[t])&&9!==e.nodeType)if(1===e.nodeType){if(i&&S(e).is(n))break;r.push(e)}return r},T=function(e,t){for(var n=[];e;e=e.nextSibling)1===e.nodeType&&e!==t&&n.push(e);return n},k=S.expr.match.needsContext;function A(e,t){return e.nodeName&&e.nodeName.toLowerCase()===t.toLowerCase()}var N=/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;function D(e,n,r){return m(n)?S.grep(e,function(e,t){return!!n.call(e,t,e)!==r}):n.nodeType?S.grep(e,function(e){return e===n!==r}):"string"!=typeof n?S.grep(e,function(e){return-1<i.call(n,e)!==r}):S.filter(n,e,r)}S.filter=function(e,t,n){var r=t[0];return n&&(e=":not("+e+")"),1===t.length&&1===r.nodeType?S.find.matchesSelector(r,e)?[r]:[]:S.find.matches(e,S.grep(t,function(e){return 1===e.nodeType}))},S.fn.extend({find:function(e){var t,n,r=this.length,i=this;if("string"!=typeof e)return this.pushStack(S(e).filter(function(){for(t=0;t<r;t++)if(S.contains(i[t],this))return!0}));for(n=this.pushStack([]),t=0;t<r;t++)S.find(e,i[t],n);return 1<r?S.uniqueSort(n):n},filter:function(e){return this.pushStack(D(this,e||[],!1))},not:function(e){return this.pushStack(D(this,e||[],!0))},is:function(e){return!!D(this,"string"==typeof e&&k.test(e)?S(e):e||[],!1).length}});var j,q=/^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;(S.fn.init=function(e,t,n){var r,i;if(!e)return this;if(n=n||j,"string"==typeof e){if(!(r="<"===e[0]&&">"===e[e.length-1]&&3<=e.length?[null,e,null]:q.exec(e))||!r[1]&&t)return!t||t.jquery?(t||n).find(e):this.constructor(t).find(e);if(r[1]){if(t=t instanceof S?t[0]:t,S.merge(this,S.parseHTML(r[1],t&&t.nodeType?t.ownerDocument||t:E,!0)),N.test(r[1])&&S.isPlainObject(t))for(r in t)m(this[r])?this[r](t[r]):this.attr(r,t[r]);return this}return(i=E.getElementById(r[2]))&&(this[0]=i,this.length=1),this}return e.nodeType?(this[0]=e,this.length=1,this):m(e)?void 0!==n.ready?n.ready(e):e(S):S.makeArray(e,this)}).prototype=S.fn,j=S(E);var L=/^(?:parents|prev(?:Until|All))/,H={children:!0,contents:!0,next:!0,prev:!0};function O(e,t){while((e=e[t])&&1!==e.nodeType);return e}S.fn.extend({has:function(e){var t=S(e,this),n=t.length;return this.filter(function(){for(var e=0;e<n;e++)if(S.contains(this,t[e]))return!0})},closest:function(e,t){var n,r=0,i=this.length,o=[],a="string"!=typeof e&&S(e);if(!k.test(e))for(;r<i;r++)for(n=this[r];n&&n!==t;n=n.parentNode)if(n.nodeType<11&&(a?-1<a.index(n):1===n.nodeType&&S.find.matchesSelector(n,e))){o.push(n);break}return this.pushStack(1<o.length?S.uniqueSort(o):o)},index:function(e){return e?"string"==typeof e?i.call(S(e),this[0]):i.call(this,e.jquery?e[0]:e):this[0]&&this[0].parentNode?this.first().prevAll().length:-1},add:function(e,t){return this.pushStack(S.uniqueSort(S.merge(this.get(),S(e,t))))},addBack:function(e){return this.add(null==e?this.prevObject:this.prevObject.filter(e))}}),S.each({parent:function(e){var t=e.parentNode;return t&&11!==t.nodeType?t:null},parents:function(e){return h(e,"parentNode")},parentsUntil:function(e,t,n){return h(e,"parentNode",n)},next:function(e){return O(e,"nextSibling")},prev:function(e){return O(e,"previousSibling")},nextAll:function(e){return h(e,"nextSibling")},prevAll:function(e){return h(e,"previousSibling")},nextUntil:function(e,t,n){return h(e,"nextSibling",n)},prevUntil:function(e,t,n){return h(e,"previousSibling",n)},siblings:function(e){return T((e.parentNode||{}).firstChild,e)},children:function(e){return T(e.firstChild)},contents:function(e){return null!=e.contentDocument&&r(e.contentDocument)?e.contentDocument:(A(e,"template")&&(e=e.content||e),S.merge([],e.childNodes))}},function(r,i){S.fn[r]=function(e,t){var n=S.map(this,i,e);return"Until"!==r.slice(-5)&&(t=e),t&&"string"==typeof t&&(n=S.filter(t,n)),1<this.length&&(H[r]||S.uniqueSort(n),L.test(r)&&n.reverse()),this.pushStack(n)}});var P=/[^\x20\t\r\n\f]+/g;function R(e){return e}function M(e){throw e}function I(e,t,n,r){var i;try{e&&m(i=e.promise)?i.call(e).done(t).fail(n):e&&m(i=e.then)?i.call(e,t,n):t.apply(void 0,[e].slice(r))}catch(e){n.apply(void 0,[e])}}S.Callbacks=function(r){var e,n;r="string"==typeof r?(e=r,n={},S.each(e.match(P)||[],function(e,t){n[t]=!0}),n):S.extend({},r);var i,t,o,a,s=[],u=[],l=-1,c=function(){for(a=a||r.once,o=i=!0;u.length;l=-1){t=u.shift();while(++l<s.length)!1===s[l].apply(t[0],t[1])&&r.stopOnFalse&&(l=s.length,t=!1)}r.memory||(t=!1),i=!1,a&&(s=t?[]:"")},f={add:function(){return s&&(t&&!i&&(l=s.length-1,u.push(t)),function n(e){S.each(e,function(e,t){m(t)?r.unique&&f.has(t)||s.push(t):t&&t.length&&"string"!==w(t)&&n(t)})}(arguments),t&&!i&&c()),this},remove:function(){return S.each(arguments,function(e,t){var n;while(-1<(n=S.inArray(t,s,n)))s.splice(n,1),n<=l&&l--}),this},has:function(e){return e?-1<S.inArray(e,s):0<s.length},empty:function(){return s&&(s=[]),this},disable:function(){return a=u=[],s=t="",this},disabled:function(){return!s},lock:function(){return a=u=[],t||i||(s=t=""),this},locked:function(){return!!a},fireWith:function(e,t){return a||(t=[e,(t=t||[]).slice?t.slice():t],u.push(t),i||c()),this},fire:function(){return f.fireWith(this,arguments),this},fired:function(){return!!o}};return f},S.extend({Deferred:function(e){var o=[["notify","progress",S.Callbacks("memory"),S.Callbacks("memory"),2],["resolve","done",S.Callbacks("once memory"),S.Callbacks("once memory"),0,"resolved"],["reject","fail",S.Callbacks("once memory"),S.Callbacks("once memory"),1,"rejected"]],i="pending",a={state:function(){return i},always:function(){return s.done(arguments).fail(arguments),this},"catch":function(e){return a.then(null,e)},pipe:function(){var i=arguments;return S.Deferred(function(r){S.each(o,function(e,t){var n=m(i[t[4]])&&i[t[4]];s[t[1]](function(){var e=n&&n.apply(this,arguments);e&&m(e.promise)?e.promise().progress(r.notify).done(r.resolve).fail(r.reject):r[t[0]+"With"](this,n?[e]:arguments)})}),i=null}).promise()},then:function(t,n,r){var u=0;function l(i,o,a,s){return function(){var n=this,r=arguments,e=function(){var e,t;if(!(i<u)){if((e=a.apply(n,r))===o.promise())throw new TypeError("Thenable self-resolution");t=e&&("object"==typeof e||"function"==typeof e)&&e.then,m(t)?s?t.call(e,l(u,o,R,s),l(u,o,M,s)):(u++,t.call(e,l(u,o,R,s),l(u,o,M,s),l(u,o,R,o.notifyWith))):(a!==R&&(n=void 0,r=[e]),(s||o.resolveWith)(n,r))}},t=s?e:function(){try{e()}catch(e){S.Deferred.exceptionHook&&S.Deferred.exceptionHook(e,t.stackTrace),u<=i+1&&(a!==M&&(n=void 0,r=[e]),o.rejectWith(n,r))}};i?t():(S.Deferred.getStackHook&&(t.stackTrace=S.Deferred.getStackHook()),C.setTimeout(t))}}return S.Deferred(function(e){o[0][3].add(l(0,e,m(r)?r:R,e.notifyWith)),o[1][3].add(l(0,e,m(t)?t:R)),o[2][3].add(l(0,e,m(n)?n:M))}).promise()},promise:function(e){return null!=e?S.extend(e,a):a}},s={};return S.each(o,function(e,t){var n=t[2],r=t[5];a[t[1]]=n.add,r&&n.add(function(){i=r},o[3-e][2].disable,o[3-e][3].disable,o[0][2].lock,o[0][3].lock),n.add(t[3].fire),s[t[0]]=function(){return s[t[0]+"With"](this===s?void 0:this,arguments),this},s[t[0]+"With"]=n.fireWith}),a.promise(s),e&&e.call(s,s),s},when:function(e){var n=arguments.length,t=n,r=Array(t),i=s.call(arguments),o=S.Deferred(),a=function(t){return function(e){r[t]=this,i[t]=1<arguments.length?s.call(arguments):e,--n||o.resolveWith(r,i)}};if(n<=1&&(I(e,o.done(a(t)).resolve,o.reject,!n),"pending"===o.state()||m(i[t]&&i[t].then)))return o.then();while(t--)I(i[t],a(t),o.reject);return o.promise()}});var W=/^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;S.Deferred.exceptionHook=function(e,t){C.console&&C.console.warn&&e&&W.test(e.name)&&C.console.warn("jQuery.Deferred exception: "+e.message,e.stack,t)},S.readyException=function(e){C.setTimeout(function(){throw e})};var F=S.Deferred();function B(){E.removeEventListener("DOMContentLoaded",B),C.removeEventListener("load",B),S.ready()}S.fn.ready=function(e){return F.then(e)["catch"](function(e){S.readyException(e)}),this},S.extend({isReady:!1,readyWait:1,ready:function(e){(!0===e?--S.readyWait:S.isReady)||(S.isReady=!0)!==e&&0<--S.readyWait||F.resolveWith(E,[S])}}),S.ready.then=F.then,"complete"===E.readyState||"loading"!==E.readyState&&!E.documentElement.doScroll?C.setTimeout(S.ready):(E.addEventListener("DOMContentLoaded",B),C.addEventListener("load",B));var $=function(e,t,n,r,i,o,a){var s=0,u=e.length,l=null==n;if("object"===w(n))for(s in i=!0,n)$(e,t,s,n[s],!0,o,a);else if(void 0!==r&&(i=!0,m(r)||(a=!0),l&&(a?(t.call(e,r),t=null):(l=t,t=function(e,t,n){return l.call(S(e),n)})),t))for(;s<u;s++)t(e[s],n,a?r:r.call(e[s],s,t(e[s],n)));return i?e:l?t.call(e):u?t(e[0],n):o},_=/^-ms-/,z=/-([a-z])/g;function U(e,t){return t.toUpperCase()}function X(e){return e.replace(_,"ms-").replace(z,U)}var V=function(e){return 1===e.nodeType||9===e.nodeType||!+e.nodeType};function G(){this.expando=S.expando+G.uid++}G.uid=1,G.prototype={cache:function(e){var t=e[this.expando];return t||(t={},V(e)&&(e.nodeType?e[this.expando]=t:Object.defineProperty(e,this.expando,{value:t,configurable:!0}))),t},set:function(e,t,n){var r,i=this.cache(e);if("string"==typeof t)i[X(t)]=n;else for(r in t)i[X(r)]=t[r];return i},get:function(e,t){return void 0===t?this.cache(e):e[this.expando]&&e[this.expando][X(t)]},access:function(e,t,n){return void 0===t||t&&"string"==typeof t&&void 0===n?this.get(e,t):(this.set(e,t,n),void 0!==n?n:t)},remove:function(e,t){var n,r=e[this.expando];if(void 0!==r){if(void 0!==t){n=(t=Array.isArray(t)?t.map(X):(t=X(t))in r?[t]:t.match(P)||[]).length;while(n--)delete r[t[n]]}(void 0===t||S.isEmptyObject(r))&&(e.nodeType?e[this.expando]=void 0:delete e[this.expando])}},hasData:function(e){var t=e[this.expando];return void 0!==t&&!S.isEmptyObject(t)}};var Y=new G,Q=new G,J=/^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,K=/[A-Z]/g;function Z(e,t,n){var r,i;if(void 0===n&&1===e.nodeType)if(r="data-"+t.replace(K,"-$&").toLowerCase(),"string"==typeof(n=e.getAttribute(r))){try{n="true"===(i=n)||"false"!==i&&("null"===i?null:i===+i+""?+i:J.test(i)?JSON.parse(i):i)}catch(e){}Q.set(e,t,n)}else n=void 0;return n}S.extend({hasData:function(e){return Q.hasData(e)||Y.hasData(e)},data:function(e,t,n){return Q.access(e,t,n)},removeData:function(e,t){Q.remove(e,t)},_data:function(e,t,n){return Y.access(e,t,n)},_removeData:function(e,t){Y.remove(e,t)}}),S.fn.extend({data:function(n,e){var t,r,i,o=this[0],a=o&&o.attributes;if(void 0===n){if(this.length&&(i=Q.get(o),1===o.nodeType&&!Y.get(o,"hasDataAttrs"))){t=a.length;while(t--)a[t]&&0===(r=a[t].name).indexOf("data-")&&(r=X(r.slice(5)),Z(o,r,i[r]));Y.set(o,"hasDataAttrs",!0)}return i}return"object"==typeof n?this.each(function(){Q.set(this,n)}):$(this,function(e){var t;if(o&&void 0===e)return void 0!==(t=Q.get(o,n))?t:void 0!==(t=Z(o,n))?t:void 0;this.each(function(){Q.set(this,n,e)})},null,e,1<arguments.length,null,!0)},removeData:function(e){return this.each(function(){Q.remove(this,e)})}}),S.extend({queue:function(e,t,n){var r;if(e)return t=(t||"fx")+"queue",r=Y.get(e,t),n&&(!r||Array.isArray(n)?r=Y.access(e,t,S.makeArray(n)):r.push(n)),r||[]},dequeue:function(e,t){t=t||"fx";var n=S.queue(e,t),r=n.length,i=n.shift(),o=S._queueHooks(e,t);"inprogress"===i&&(i=n.shift(),r--),i&&("fx"===t&&n.unshift("inprogress"),delete o.stop,i.call(e,function(){S.dequeue(e,t)},o)),!r&&o&&o.empty.fire()},_queueHooks:function(e,t){var n=t+"queueHooks";return Y.get(e,n)||Y.access(e,n,{empty:S.Callbacks("once memory").add(function(){Y.remove(e,[t+"queue",n])})})}}),S.fn.extend({queue:function(t,n){var e=2;return"string"!=typeof t&&(n=t,t="fx",e--),arguments.length<e?S.queue(this[0],t):void 0===n?this:this.each(function(){var e=S.queue(this,t,n);S._queueHooks(this,t),"fx"===t&&"inprogress"!==e[0]&&S.dequeue(this,t)})},dequeue:function(e){return this.each(function(){S.dequeue(this,e)})},clearQueue:function(e){return this.queue(e||"fx",[])},promise:function(e,t){var n,r=1,i=S.Deferred(),o=this,a=this.length,s=function(){--r||i.resolveWith(o,[o])};"string"!=typeof e&&(t=e,e=void 0),e=e||"fx";while(a--)(n=Y.get(o[a],e+"queueHooks"))&&n.empty&&(r++,n.empty.add(s));return s(),i.promise(t)}});var ee=/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,te=new RegExp("^(?:([+-])=|)("+ee+")([a-z%]*)$","i"),ne=["Top","Right","Bottom","Left"],re=E.documentElement,ie=function(e){return S.contains(e.ownerDocument,e)},oe={composed:!0};re.getRootNode&&(ie=function(e){return S.contains(e.ownerDocument,e)||e.getRootNode(oe)===e.ownerDocument});var ae=function(e,t){return"none"===(e=t||e).style.display||""===e.style.display&&ie(e)&&"none"===S.css(e,"display")};function se(e,t,n,r){var i,o,a=20,s=r?function(){return r.cur()}:function(){return S.css(e,t,"")},u=s(),l=n&&n[3]||(S.cssNumber[t]?"":"px"),c=e.nodeType&&(S.cssNumber[t]||"px"!==l&&+u)&&te.exec(S.css(e,t));if(c&&c[3]!==l){u/=2,l=l||c[3],c=+u||1;while(a--)S.style(e,t,c+l),(1-o)*(1-(o=s()/u||.5))<=0&&(a=0),c/=o;c*=2,S.style(e,t,c+l),n=n||[]}return n&&(c=+c||+u||0,i=n[1]?c+(n[1]+1)*n[2]:+n[2],r&&(r.unit=l,r.start=c,r.end=i)),i}var ue={};function le(e,t){for(var n,r,i,o,a,s,u,l=[],c=0,f=e.length;c<f;c++)(r=e[c]).style&&(n=r.style.display,t?("none"===n&&(l[c]=Y.get(r,"display")||null,l[c]||(r.style.display="")),""===r.style.display&&ae(r)&&(l[c]=(u=a=o=void 0,a=(i=r).ownerDocument,s=i.nodeName,(u=ue[s])||(o=a.body.appendChild(a.createElement(s)),u=S.css(o,"display"),o.parentNode.removeChild(o),"none"===u&&(u="block"),ue[s]=u)))):"none"!==n&&(l[c]="none",Y.set(r,"display",n)));for(c=0;c<f;c++)null!=l[c]&&(e[c].style.display=l[c]);return e}S.fn.extend({show:function(){return le(this,!0)},hide:function(){return le(this)},toggle:function(e){return"boolean"==typeof e?e?this.show():this.hide():this.each(function(){ae(this)?S(this).show():S(this).hide()})}});var ce,fe,pe=/^(?:checkbox|radio)$/i,de=/<([a-z][^\/\0>\x20\t\r\n\f]*)/i,he=/^$|^module$|\/(?:java|ecma)script/i;ce=E.createDocumentFragment().appendChild(E.createElement("div")),(fe=E.createElement("input")).setAttribute("type","radio"),fe.setAttribute("checked","checked"),fe.setAttribute("name","t"),ce.appendChild(fe),y.checkClone=ce.cloneNode(!0).cloneNode(!0).lastChild.checked,ce.innerHTML="<textarea>x</textarea>",y.noCloneChecked=!!ce.cloneNode(!0).lastChild.defaultValue,ce.innerHTML="<option></option>",y.option=!!ce.lastChild;var ge={thead:[1,"<table>","</table>"],col:[2,"<table><colgroup>","</colgroup></table>"],tr:[2,"<table><tbody>","</tbody></table>"],td:[3,"<table><tbody><tr>","</tr></tbody></table>"],_default:[0,"",""]};function ve(e,t){var n;return n="undefined"!=typeof e.getElementsByTagName?e.getElementsByTagName(t||"*"):"undefined"!=typeof e.querySelectorAll?e.querySelectorAll(t||"*"):[],void 0===t||t&&A(e,t)?S.merge([e],n):n}function ye(e,t){for(var n=0,r=e.length;n<r;n++)Y.set(e[n],"globalEval",!t||Y.get(t[n],"globalEval"))}ge.tbody=ge.tfoot=ge.colgroup=ge.caption=ge.thead,ge.th=ge.td,y.option||(ge.optgroup=ge.option=[1,"<select multiple='multiple'>","</select>"]);var me=/<|&#?\w+;/;function xe(e,t,n,r,i){for(var o,a,s,u,l,c,f=t.createDocumentFragment(),p=[],d=0,h=e.length;d<h;d++)if((o=e[d])||0===o)if("object"===w(o))S.merge(p,o.nodeType?[o]:o);else if(me.test(o)){a=a||f.appendChild(t.createElement("div")),s=(de.exec(o)||["",""])[1].toLowerCase(),u=ge[s]||ge._default,a.innerHTML=u[1]+S.htmlPrefilter(o)+u[2],c=u[0];while(c--)a=a.lastChild;S.merge(p,a.childNodes),(a=f.firstChild).textContent=""}else p.push(t.createTextNode(o));f.textContent="",d=0;while(o=p[d++])if(r&&-1<S.inArray(o,r))i&&i.push(o);else if(l=ie(o),a=ve(f.appendChild(o),"script"),l&&ye(a),n){c=0;while(o=a[c++])he.test(o.type||"")&&n.push(o)}return f}var be=/^key/,we=/^(?:mouse|pointer|contextmenu|drag|drop)|click/,Te=/^([^.]*)(?:\.(.+)|)/;function Ce(){return!0}function Ee(){return!1}function Se(e,t){return e===function(){try{return E.activeElement}catch(e){}}()==("focus"===t)}function ke(e,t,n,r,i,o){var a,s;if("object"==typeof t){for(s in"string"!=typeof n&&(r=r||n,n=void 0),t)ke(e,s,n,r,t[s],o);return e}if(null==r&&null==i?(i=n,r=n=void 0):null==i&&("string"==typeof n?(i=r,r=void 0):(i=r,r=n,n=void 0)),!1===i)i=Ee;else if(!i)return e;return 1===o&&(a=i,(i=function(e){return S().off(e),a.apply(this,arguments)}).guid=a.guid||(a.guid=S.guid++)),e.each(function(){S.event.add(this,t,i,r,n)})}function Ae(e,i,o){o?(Y.set(e,i,!1),S.event.add(e,i,{namespace:!1,handler:function(e){var t,n,r=Y.get(this,i);if(1&e.isTrigger&&this[i]){if(r.length)(S.event.special[i]||{}).delegateType&&e.stopPropagation();else if(r=s.call(arguments),Y.set(this,i,r),t=o(this,i),this[i](),r!==(n=Y.get(this,i))||t?Y.set(this,i,!1):n={},r!==n)return e.stopImmediatePropagation(),e.preventDefault(),n.value}else r.length&&(Y.set(this,i,{value:S.event.trigger(S.extend(r[0],S.Event.prototype),r.slice(1),this)}),e.stopImmediatePropagation())}})):void 0===Y.get(e,i)&&S.event.add(e,i,Ce)}S.event={global:{},add:function(t,e,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,v=Y.get(t);if(V(t)){n.handler&&(n=(o=n).handler,i=o.selector),i&&S.find.matchesSelector(re,i),n.guid||(n.guid=S.guid++),(u=v.events)||(u=v.events=Object.create(null)),(a=v.handle)||(a=v.handle=function(e){return"undefined"!=typeof S&&S.event.triggered!==e.type?S.event.dispatch.apply(t,arguments):void 0}),l=(e=(e||"").match(P)||[""]).length;while(l--)d=g=(s=Te.exec(e[l])||[])[1],h=(s[2]||"").split(".").sort(),d&&(f=S.event.special[d]||{},d=(i?f.delegateType:f.bindType)||d,f=S.event.special[d]||{},c=S.extend({type:d,origType:g,data:r,handler:n,guid:n.guid,selector:i,needsContext:i&&S.expr.match.needsContext.test(i),namespace:h.join(".")},o),(p=u[d])||((p=u[d]=[]).delegateCount=0,f.setup&&!1!==f.setup.call(t,r,h,a)||t.addEventListener&&t.addEventListener(d,a)),f.add&&(f.add.call(t,c),c.handler.guid||(c.handler.guid=n.guid)),i?p.splice(p.delegateCount++,0,c):p.push(c),S.event.global[d]=!0)}},remove:function(e,t,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,v=Y.hasData(e)&&Y.get(e);if(v&&(u=v.events)){l=(t=(t||"").match(P)||[""]).length;while(l--)if(d=g=(s=Te.exec(t[l])||[])[1],h=(s[2]||"").split(".").sort(),d){f=S.event.special[d]||{},p=u[d=(r?f.delegateType:f.bindType)||d]||[],s=s[2]&&new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"),a=o=p.length;while(o--)c=p[o],!i&&g!==c.origType||n&&n.guid!==c.guid||s&&!s.test(c.namespace)||r&&r!==c.selector&&("**"!==r||!c.selector)||(p.splice(o,1),c.selector&&p.delegateCount--,f.remove&&f.remove.call(e,c));a&&!p.length&&(f.teardown&&!1!==f.teardown.call(e,h,v.handle)||S.removeEvent(e,d,v.handle),delete u[d])}else for(d in u)S.event.remove(e,d+t[l],n,r,!0);S.isEmptyObject(u)&&Y.remove(e,"handle events")}},dispatch:function(e){var t,n,r,i,o,a,s=new Array(arguments.length),u=S.event.fix(e),l=(Y.get(this,"events")||Object.create(null))[u.type]||[],c=S.event.special[u.type]||{};for(s[0]=u,t=1;t<arguments.length;t++)s[t]=arguments[t];if(u.delegateTarget=this,!c.preDispatch||!1!==c.preDispatch.call(this,u)){a=S.event.handlers.call(this,u,l),t=0;while((i=a[t++])&&!u.isPropagationStopped()){u.currentTarget=i.elem,n=0;while((o=i.handlers[n++])&&!u.isImmediatePropagationStopped())u.rnamespace&&!1!==o.namespace&&!u.rnamespace.test(o.namespace)||(u.handleObj=o,u.data=o.data,void 0!==(r=((S.event.special[o.origType]||{}).handle||o.handler).apply(i.elem,s))&&!1===(u.result=r)&&(u.preventDefault(),u.stopPropagation()))}return c.postDispatch&&c.postDispatch.call(this,u),u.result}},handlers:function(e,t){var n,r,i,o,a,s=[],u=t.delegateCount,l=e.target;if(u&&l.nodeType&&!("click"===e.type&&1<=e.button))for(;l!==this;l=l.parentNode||this)if(1===l.nodeType&&("click"!==e.type||!0!==l.disabled)){for(o=[],a={},n=0;n<u;n++)void 0===a[i=(r=t[n]).selector+" "]&&(a[i]=r.needsContext?-1<S(i,this).index(l):S.find(i,this,null,[l]).length),a[i]&&o.push(r);o.length&&s.push({elem:l,handlers:o})}return l=this,u<t.length&&s.push({elem:l,handlers:t.slice(u)}),s},addProp:function(t,e){Object.defineProperty(S.Event.prototype,t,{enumerable:!0,configurable:!0,get:m(e)?function(){if(this.originalEvent)return e(this.originalEvent)}:function(){if(this.originalEvent)return this.originalEvent[t]},set:function(e){Object.defineProperty(this,t,{enumerable:!0,configurable:!0,writable:!0,value:e})}})},fix:function(e){return e[S.expando]?e:new S.Event(e)},special:{load:{noBubble:!0},click:{setup:function(e){var t=this||e;return pe.test(t.type)&&t.click&&A(t,"input")&&Ae(t,"click",Ce),!1},trigger:function(e){var t=this||e;return pe.test(t.type)&&t.click&&A(t,"input")&&Ae(t,"click"),!0},_default:function(e){var t=e.target;return pe.test(t.type)&&t.click&&A(t,"input")&&Y.get(t,"click")||A(t,"a")}},beforeunload:{postDispatch:function(e){void 0!==e.result&&e.originalEvent&&(e.originalEvent.returnValue=e.result)}}}},S.removeEvent=function(e,t,n){e.removeEventListener&&e.removeEventListener(t,n)},S.Event=function(e,t){if(!(this instanceof S.Event))return new S.Event(e,t);e&&e.type?(this.originalEvent=e,this.type=e.type,this.isDefaultPrevented=e.defaultPrevented||void 0===e.defaultPrevented&&!1===e.returnValue?Ce:Ee,this.target=e.target&&3===e.target.nodeType?e.target.parentNode:e.target,this.currentTarget=e.currentTarget,this.relatedTarget=e.relatedTarget):this.type=e,t&&S.extend(this,t),this.timeStamp=e&&e.timeStamp||Date.now(),this[S.expando]=!0},S.Event.prototype={constructor:S.Event,isDefaultPrevented:Ee,isPropagationStopped:Ee,isImmediatePropagationStopped:Ee,isSimulated:!1,preventDefault:function(){var e=this.originalEvent;this.isDefaultPrevented=Ce,e&&!this.isSimulated&&e.preventDefault()},stopPropagation:function(){var e=this.originalEvent;this.isPropagationStopped=Ce,e&&!this.isSimulated&&e.stopPropagation()},stopImmediatePropagation:function(){var e=this.originalEvent;this.isImmediatePropagationStopped=Ce,e&&!this.isSimulated&&e.stopImmediatePropagation(),this.stopPropagation()}},S.each({altKey:!0,bubbles:!0,cancelable:!0,changedTouches:!0,ctrlKey:!0,detail:!0,eventPhase:!0,metaKey:!0,pageX:!0,pageY:!0,shiftKey:!0,view:!0,"char":!0,code:!0,charCode:!0,key:!0,keyCode:!0,button:!0,buttons:!0,clientX:!0,clientY:!0,offsetX:!0,offsetY:!0,pointerId:!0,pointerType:!0,screenX:!0,screenY:!0,targetTouches:!0,toElement:!0,touches:!0,which:function(e){var t=e.button;return null==e.which&&be.test(e.type)?null!=e.charCode?e.charCode:e.keyCode:!e.which&&void 0!==t&&we.test(e.type)?1&t?1:2&t?3:4&t?2:0:e.which}},S.event.addProp),S.each({focus:"focusin",blur:"focusout"},function(e,t){S.event.special[e]={setup:function(){return Ae(this,e,Se),!1},trigger:function(){return Ae(this,e),!0},delegateType:t}}),S.each({mouseenter:"mouseover",mouseleave:"mouseout",pointerenter:"pointerover",pointerleave:"pointerout"},function(e,i){S.event.special[e]={delegateType:i,bindType:i,handle:function(e){var t,n=e.relatedTarget,r=e.handleObj;return n&&(n===this||S.contains(this,n))||(e.type=r.origType,t=r.handler.apply(this,arguments),e.type=i),t}}}),S.fn.extend({on:function(e,t,n,r){return ke(this,e,t,n,r)},one:function(e,t,n,r){return ke(this,e,t,n,r,1)},off:function(e,t,n){var r,i;if(e&&e.preventDefault&&e.handleObj)return r=e.handleObj,S(e.delegateTarget).off(r.namespace?r.origType+"."+r.namespace:r.origType,r.selector,r.handler),this;if("object"==typeof e){for(i in e)this.off(i,t,e[i]);return this}return!1!==t&&"function"!=typeof t||(n=t,t=void 0),!1===n&&(n=Ee),this.each(function(){S.event.remove(this,e,n,t)})}});var Ne=/<script|<style|<link/i,De=/checked\s*(?:[^=]|=\s*.checked.)/i,je=/^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;function qe(e,t){return A(e,"table")&&A(11!==t.nodeType?t:t.firstChild,"tr")&&S(e).children("tbody")[0]||e}function Le(e){return e.type=(null!==e.getAttribute("type"))+"/"+e.type,e}function He(e){return"true/"===(e.type||"").slice(0,5)?e.type=e.type.slice(5):e.removeAttribute("type"),e}function Oe(e,t){var n,r,i,o,a,s;if(1===t.nodeType){if(Y.hasData(e)&&(s=Y.get(e).events))for(i in Y.remove(t,"handle events"),s)for(n=0,r=s[i].length;n<r;n++)S.event.add(t,i,s[i][n]);Q.hasData(e)&&(o=Q.access(e),a=S.extend({},o),Q.set(t,a))}}function Pe(n,r,i,o){r=g(r);var e,t,a,s,u,l,c=0,f=n.length,p=f-1,d=r[0],h=m(d);if(h||1<f&&"string"==typeof d&&!y.checkClone&&De.test(d))return n.each(function(e){var t=n.eq(e);h&&(r[0]=d.call(this,e,t.html())),Pe(t,r,i,o)});if(f&&(t=(e=xe(r,n[0].ownerDocument,!1,n,o)).firstChild,1===e.childNodes.length&&(e=t),t||o)){for(s=(a=S.map(ve(e,"script"),Le)).length;c<f;c++)u=e,c!==p&&(u=S.clone(u,!0,!0),s&&S.merge(a,ve(u,"script"))),i.call(n[c],u,c);if(s)for(l=a[a.length-1].ownerDocument,S.map(a,He),c=0;c<s;c++)u=a[c],he.test(u.type||"")&&!Y.access(u,"globalEval")&&S.contains(l,u)&&(u.src&&"module"!==(u.type||"").toLowerCase()?S._evalUrl&&!u.noModule&&S._evalUrl(u.src,{nonce:u.nonce||u.getAttribute("nonce")},l):b(u.textContent.replace(je,""),u,l))}return n}function Re(e,t,n){for(var r,i=t?S.filter(t,e):e,o=0;null!=(r=i[o]);o++)n||1!==r.nodeType||S.cleanData(ve(r)),r.parentNode&&(n&&ie(r)&&ye(ve(r,"script")),r.parentNode.removeChild(r));return e}S.extend({htmlPrefilter:function(e){return e},clone:function(e,t,n){var r,i,o,a,s,u,l,c=e.cloneNode(!0),f=ie(e);if(!(y.noCloneChecked||1!==e.nodeType&&11!==e.nodeType||S.isXMLDoc(e)))for(a=ve(c),r=0,i=(o=ve(e)).length;r<i;r++)s=o[r],u=a[r],void 0,"input"===(l=u.nodeName.toLowerCase())&&pe.test(s.type)?u.checked=s.checked:"input"!==l&&"textarea"!==l||(u.defaultValue=s.defaultValue);if(t)if(n)for(o=o||ve(e),a=a||ve(c),r=0,i=o.length;r<i;r++)Oe(o[r],a[r]);else Oe(e,c);return 0<(a=ve(c,"script")).length&&ye(a,!f&&ve(e,"script")),c},cleanData:function(e){for(var t,n,r,i=S.event.special,o=0;void 0!==(n=e[o]);o++)if(V(n)){if(t=n[Y.expando]){if(t.events)for(r in t.events)i[r]?S.event.remove(n,r):S.removeEvent(n,r,t.handle);n[Y.expando]=void 0}n[Q.expando]&&(n[Q.expando]=void 0)}}}),S.fn.extend({detach:function(e){return Re(this,e,!0)},remove:function(e){return Re(this,e)},text:function(e){return $(this,function(e){return void 0===e?S.text(this):this.empty().each(function(){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||(this.textContent=e)})},null,e,arguments.length)},append:function(){return Pe(this,arguments,function(e){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||qe(this,e).appendChild(e)})},prepend:function(){return Pe(this,arguments,function(e){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var t=qe(this,e);t.insertBefore(e,t.firstChild)}})},before:function(){return Pe(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this)})},after:function(){return Pe(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this.nextSibling)})},empty:function(){for(var e,t=0;null!=(e=this[t]);t++)1===e.nodeType&&(S.cleanData(ve(e,!1)),e.textContent="");return this},clone:function(e,t){return e=null!=e&&e,t=null==t?e:t,this.map(function(){return S.clone(this,e,t)})},html:function(e){return $(this,function(e){var t=this[0]||{},n=0,r=this.length;if(void 0===e&&1===t.nodeType)return t.innerHTML;if("string"==typeof e&&!Ne.test(e)&&!ge[(de.exec(e)||["",""])[1].toLowerCase()]){e=S.htmlPrefilter(e);try{for(;n<r;n++)1===(t=this[n]||{}).nodeType&&(S.cleanData(ve(t,!1)),t.innerHTML=e);t=0}catch(e){}}t&&this.empty().append(e)},null,e,arguments.length)},replaceWith:function(){var n=[];return Pe(this,arguments,function(e){var t=this.parentNode;S.inArray(this,n)<0&&(S.cleanData(ve(this)),t&&t.replaceChild(e,this))},n)}}),S.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(e,a){S.fn[e]=function(e){for(var t,n=[],r=S(e),i=r.length-1,o=0;o<=i;o++)t=o===i?this:this.clone(!0),S(r[o])[a](t),u.apply(n,t.get());return this.pushStack(n)}});var Me=new RegExp("^("+ee+")(?!px)[a-z%]+$","i"),Ie=function(e){var t=e.ownerDocument.defaultView;return t&&t.opener||(t=C),t.getComputedStyle(e)},We=function(e,t,n){var r,i,o={};for(i in t)o[i]=e.style[i],e.style[i]=t[i];for(i in r=n.call(e),t)e.style[i]=o[i];return r},Fe=new RegExp(ne.join("|"),"i");function Be(e,t,n){var r,i,o,a,s=e.style;return(n=n||Ie(e))&&(""!==(a=n.getPropertyValue(t)||n[t])||ie(e)||(a=S.style(e,t)),!y.pixelBoxStyles()&&Me.test(a)&&Fe.test(t)&&(r=s.width,i=s.minWidth,o=s.maxWidth,s.minWidth=s.maxWidth=s.width=a,a=n.width,s.width=r,s.minWidth=i,s.maxWidth=o)),void 0!==a?a+"":a}function $e(e,t){return{get:function(){if(!e())return(this.get=t).apply(this,arguments);delete this.get}}}!function(){function e(){if(l){u.style.cssText="position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0",l.style.cssText="position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%",re.appendChild(u).appendChild(l);var e=C.getComputedStyle(l);n="1%"!==e.top,s=12===t(e.marginLeft),l.style.right="60%",o=36===t(e.right),r=36===t(e.width),l.style.position="absolute",i=12===t(l.offsetWidth/3),re.removeChild(u),l=null}}function t(e){return Math.round(parseFloat(e))}var n,r,i,o,a,s,u=E.createElement("div"),l=E.createElement("div");l.style&&(l.style.backgroundClip="content-box",l.cloneNode(!0).style.backgroundClip="",y.clearCloneStyle="content-box"===l.style.backgroundClip,S.extend(y,{boxSizingReliable:function(){return e(),r},pixelBoxStyles:function(){return e(),o},pixelPosition:function(){return e(),n},reliableMarginLeft:function(){return e(),s},scrollboxSize:function(){return e(),i},reliableTrDimensions:function(){var e,t,n,r;return null==a&&(e=E.createElement("table"),t=E.createElement("tr"),n=E.createElement("div"),e.style.cssText="position:absolute;left:-11111px",t.style.height="1px",n.style.height="9px",re.appendChild(e).appendChild(t).appendChild(n),r=C.getComputedStyle(t),a=3<parseInt(r.height),re.removeChild(e)),a}}))}();var _e=["Webkit","Moz","ms"],ze=E.createElement("div").style,Ue={};function Xe(e){var t=S.cssProps[e]||Ue[e];return t||(e in ze?e:Ue[e]=function(e){var t=e[0].toUpperCase()+e.slice(1),n=_e.length;while(n--)if((e=_e[n]+t)in ze)return e}(e)||e)}var Ve=/^(none|table(?!-c[ea]).+)/,Ge=/^--/,Ye={position:"absolute",visibility:"hidden",display:"block"},Qe={letterSpacing:"0",fontWeight:"400"};function Je(e,t,n){var r=te.exec(t);return r?Math.max(0,r[2]-(n||0))+(r[3]||"px"):t}function Ke(e,t,n,r,i,o){var a="width"===t?1:0,s=0,u=0;if(n===(r?"border":"content"))return 0;for(;a<4;a+=2)"margin"===n&&(u+=S.css(e,n+ne[a],!0,i)),r?("content"===n&&(u-=S.css(e,"padding"+ne[a],!0,i)),"margin"!==n&&(u-=S.css(e,"border"+ne[a]+"Width",!0,i))):(u+=S.css(e,"padding"+ne[a],!0,i),"padding"!==n?u+=S.css(e,"border"+ne[a]+"Width",!0,i):s+=S.css(e,"border"+ne[a]+"Width",!0,i));return!r&&0<=o&&(u+=Math.max(0,Math.ceil(e["offset"+t[0].toUpperCase()+t.slice(1)]-o-u-s-.5))||0),u}function Ze(e,t,n){var r=Ie(e),i=(!y.boxSizingReliable()||n)&&"border-box"===S.css(e,"boxSizing",!1,r),o=i,a=Be(e,t,r),s="offset"+t[0].toUpperCase()+t.slice(1);if(Me.test(a)){if(!n)return a;a="auto"}return(!y.boxSizingReliable()&&i||!y.reliableTrDimensions()&&A(e,"tr")||"auto"===a||!parseFloat(a)&&"inline"===S.css(e,"display",!1,r))&&e.getClientRects().length&&(i="border-box"===S.css(e,"boxSizing",!1,r),(o=s in e)&&(a=e[s])),(a=parseFloat(a)||0)+Ke(e,t,n||(i?"border":"content"),o,r,a)+"px"}function et(e,t,n,r,i){return new et.prototype.init(e,t,n,r,i)}S.extend({cssHooks:{opacity:{get:function(e,t){if(t){var n=Be(e,"opacity");return""===n?"1":n}}}},cssNumber:{animationIterationCount:!0,columnCount:!0,fillOpacity:!0,flexGrow:!0,flexShrink:!0,fontWeight:!0,gridArea:!0,gridColumn:!0,gridColumnEnd:!0,gridColumnStart:!0,gridRow:!0,gridRowEnd:!0,gridRowStart:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,widows:!0,zIndex:!0,zoom:!0},cssProps:{},style:function(e,t,n,r){if(e&&3!==e.nodeType&&8!==e.nodeType&&e.style){var i,o,a,s=X(t),u=Ge.test(t),l=e.style;if(u||(t=Xe(s)),a=S.cssHooks[t]||S.cssHooks[s],void 0===n)return a&&"get"in a&&void 0!==(i=a.get(e,!1,r))?i:l[t];"string"===(o=typeof n)&&(i=te.exec(n))&&i[1]&&(n=se(e,t,i),o="number"),null!=n&&n==n&&("number"!==o||u||(n+=i&&i[3]||(S.cssNumber[s]?"":"px")),y.clearCloneStyle||""!==n||0!==t.indexOf("background")||(l[t]="inherit"),a&&"set"in a&&void 0===(n=a.set(e,n,r))||(u?l.setProperty(t,n):l[t]=n))}},css:function(e,t,n,r){var i,o,a,s=X(t);return Ge.test(t)||(t=Xe(s)),(a=S.cssHooks[t]||S.cssHooks[s])&&"get"in a&&(i=a.get(e,!0,n)),void 0===i&&(i=Be(e,t,r)),"normal"===i&&t in Qe&&(i=Qe[t]),""===n||n?(o=parseFloat(i),!0===n||isFinite(o)?o||0:i):i}}),S.each(["height","width"],function(e,u){S.cssHooks[u]={get:function(e,t,n){if(t)return!Ve.test(S.css(e,"display"))||e.getClientRects().length&&e.getBoundingClientRect().width?Ze(e,u,n):We(e,Ye,function(){return Ze(e,u,n)})},set:function(e,t,n){var r,i=Ie(e),o=!y.scrollboxSize()&&"absolute"===i.position,a=(o||n)&&"border-box"===S.css(e,"boxSizing",!1,i),s=n?Ke(e,u,n,a,i):0;return a&&o&&(s-=Math.ceil(e["offset"+u[0].toUpperCase()+u.slice(1)]-parseFloat(i[u])-Ke(e,u,"border",!1,i)-.5)),s&&(r=te.exec(t))&&"px"!==(r[3]||"px")&&(e.style[u]=t,t=S.css(e,u)),Je(0,t,s)}}}),S.cssHooks.marginLeft=$e(y.reliableMarginLeft,function(e,t){if(t)return(parseFloat(Be(e,"marginLeft"))||e.getBoundingClientRect().left-We(e,{marginLeft:0},function(){return e.getBoundingClientRect().left}))+"px"}),S.each({margin:"",padding:"",border:"Width"},function(i,o){S.cssHooks[i+o]={expand:function(e){for(var t=0,n={},r="string"==typeof e?e.split(" "):[e];t<4;t++)n[i+ne[t]+o]=r[t]||r[t-2]||r[0];return n}},"margin"!==i&&(S.cssHooks[i+o].set=Je)}),S.fn.extend({css:function(e,t){return $(this,function(e,t,n){var r,i,o={},a=0;if(Array.isArray(t)){for(r=Ie(e),i=t.length;a<i;a++)o[t[a]]=S.css(e,t[a],!1,r);return o}return void 0!==n?S.style(e,t,n):S.css(e,t)},e,t,1<arguments.length)}}),((S.Tween=et).prototype={constructor:et,init:function(e,t,n,r,i,o){this.elem=e,this.prop=n,this.easing=i||S.easing._default,this.options=t,this.start=this.now=this.cur(),this.end=r,this.unit=o||(S.cssNumber[n]?"":"px")},cur:function(){var e=et.propHooks[this.prop];return e&&e.get?e.get(this):et.propHooks._default.get(this)},run:function(e){var t,n=et.propHooks[this.prop];return this.options.duration?this.pos=t=S.easing[this.easing](e,this.options.duration*e,0,1,this.options.duration):this.pos=t=e,this.now=(this.end-this.start)*t+this.start,this.options.step&&this.options.step.call(this.elem,this.now,this),n&&n.set?n.set(this):et.propHooks._default.set(this),this}}).init.prototype=et.prototype,(et.propHooks={_default:{get:function(e){var t;return 1!==e.elem.nodeType||null!=e.elem[e.prop]&&null==e.elem.style[e.prop]?e.elem[e.prop]:(t=S.css(e.elem,e.prop,""))&&"auto"!==t?t:0},set:function(e){S.fx.step[e.prop]?S.fx.step[e.prop](e):1!==e.elem.nodeType||!S.cssHooks[e.prop]&&null==e.elem.style[Xe(e.prop)]?e.elem[e.prop]=e.now:S.style(e.elem,e.prop,e.now+e.unit)}}}).scrollTop=et.propHooks.scrollLeft={set:function(e){e.elem.nodeType&&e.elem.parentNode&&(e.elem[e.prop]=e.now)}},S.easing={linear:function(e){return e},swing:function(e){return.5-Math.cos(e*Math.PI)/2},_default:"swing"},S.fx=et.prototype.init,S.fx.step={};var tt,nt,rt,it,ot=/^(?:toggle|show|hide)$/,at=/queueHooks$/;function st(){nt&&(!1===E.hidden&&C.requestAnimationFrame?C.requestAnimationFrame(st):C.setTimeout(st,S.fx.interval),S.fx.tick())}function ut(){return C.setTimeout(function(){tt=void 0}),tt=Date.now()}function lt(e,t){var n,r=0,i={height:e};for(t=t?1:0;r<4;r+=2-t)i["margin"+(n=ne[r])]=i["padding"+n]=e;return t&&(i.opacity=i.width=e),i}function ct(e,t,n){for(var r,i=(ft.tweeners[t]||[]).concat(ft.tweeners["*"]),o=0,a=i.length;o<a;o++)if(r=i[o].call(n,t,e))return r}function ft(o,e,t){var n,a,r=0,i=ft.prefilters.length,s=S.Deferred().always(function(){delete u.elem}),u=function(){if(a)return!1;for(var e=tt||ut(),t=Math.max(0,l.startTime+l.duration-e),n=1-(t/l.duration||0),r=0,i=l.tweens.length;r<i;r++)l.tweens[r].run(n);return s.notifyWith(o,[l,n,t]),n<1&&i?t:(i||s.notifyWith(o,[l,1,0]),s.resolveWith(o,[l]),!1)},l=s.promise({elem:o,props:S.extend({},e),opts:S.extend(!0,{specialEasing:{},easing:S.easing._default},t),originalProperties:e,originalOptions:t,startTime:tt||ut(),duration:t.duration,tweens:[],createTween:function(e,t){var n=S.Tween(o,l.opts,e,t,l.opts.specialEasing[e]||l.opts.easing);return l.tweens.push(n),n},stop:function(e){var t=0,n=e?l.tweens.length:0;if(a)return this;for(a=!0;t<n;t++)l.tweens[t].run(1);return e?(s.notifyWith(o,[l,1,0]),s.resolveWith(o,[l,e])):s.rejectWith(o,[l,e]),this}}),c=l.props;for(!function(e,t){var n,r,i,o,a;for(n in e)if(i=t[r=X(n)],o=e[n],Array.isArray(o)&&(i=o[1],o=e[n]=o[0]),n!==r&&(e[r]=o,delete e[n]),(a=S.cssHooks[r])&&"expand"in a)for(n in o=a.expand(o),delete e[r],o)n in e||(e[n]=o[n],t[n]=i);else t[r]=i}(c,l.opts.specialEasing);r<i;r++)if(n=ft.prefilters[r].call(l,o,c,l.opts))return m(n.stop)&&(S._queueHooks(l.elem,l.opts.queue).stop=n.stop.bind(n)),n;return S.map(c,ct,l),m(l.opts.start)&&l.opts.start.call(o,l),l.progress(l.opts.progress).done(l.opts.done,l.opts.complete).fail(l.opts.fail).always(l.opts.always),S.fx.timer(S.extend(u,{elem:o,anim:l,queue:l.opts.queue})),l}S.Animation=S.extend(ft,{tweeners:{"*":[function(e,t){var n=this.createTween(e,t);return se(n.elem,e,te.exec(t),n),n}]},tweener:function(e,t){m(e)?(t=e,e=["*"]):e=e.match(P);for(var n,r=0,i=e.length;r<i;r++)n=e[r],ft.tweeners[n]=ft.tweeners[n]||[],ft.tweeners[n].unshift(t)},prefilters:[function(e,t,n){var r,i,o,a,s,u,l,c,f="width"in t||"height"in t,p=this,d={},h=e.style,g=e.nodeType&&ae(e),v=Y.get(e,"fxshow");for(r in n.queue||(null==(a=S._queueHooks(e,"fx")).unqueued&&(a.unqueued=0,s=a.empty.fire,a.empty.fire=function(){a.unqueued||s()}),a.unqueued++,p.always(function(){p.always(function(){a.unqueued--,S.queue(e,"fx").length||a.empty.fire()})})),t)if(i=t[r],ot.test(i)){if(delete t[r],o=o||"toggle"===i,i===(g?"hide":"show")){if("show"!==i||!v||void 0===v[r])continue;g=!0}d[r]=v&&v[r]||S.style(e,r)}if((u=!S.isEmptyObject(t))||!S.isEmptyObject(d))for(r in f&&1===e.nodeType&&(n.overflow=[h.overflow,h.overflowX,h.overflowY],null==(l=v&&v.display)&&(l=Y.get(e,"display")),"none"===(c=S.css(e,"display"))&&(l?c=l:(le([e],!0),l=e.style.display||l,c=S.css(e,"display"),le([e]))),("inline"===c||"inline-block"===c&&null!=l)&&"none"===S.css(e,"float")&&(u||(p.done(function(){h.display=l}),null==l&&(c=h.display,l="none"===c?"":c)),h.display="inline-block")),n.overflow&&(h.overflow="hidden",p.always(function(){h.overflow=n.overflow[0],h.overflowX=n.overflow[1],h.overflowY=n.overflow[2]})),u=!1,d)u||(v?"hidden"in v&&(g=v.hidden):v=Y.access(e,"fxshow",{display:l}),o&&(v.hidden=!g),g&&le([e],!0),p.done(function(){for(r in g||le([e]),Y.remove(e,"fxshow"),d)S.style(e,r,d[r])})),u=ct(g?v[r]:0,r,p),r in v||(v[r]=u.start,g&&(u.end=u.start,u.start=0))}],prefilter:function(e,t){t?ft.prefilters.unshift(e):ft.prefilters.push(e)}}),S.speed=function(e,t,n){var r=e&&"object"==typeof e?S.extend({},e):{complete:n||!n&&t||m(e)&&e,duration:e,easing:n&&t||t&&!m(t)&&t};return S.fx.off?r.duration=0:"number"!=typeof r.duration&&(r.duration in S.fx.speeds?r.duration=S.fx.speeds[r.duration]:r.duration=S.fx.speeds._default),null!=r.queue&&!0!==r.queue||(r.queue="fx"),r.old=r.complete,r.complete=function(){m(r.old)&&r.old.call(this),r.queue&&S.dequeue(this,r.queue)},r},S.fn.extend({fadeTo:function(e,t,n,r){return this.filter(ae).css("opacity",0).show().end().animate({opacity:t},e,n,r)},animate:function(t,e,n,r){var i=S.isEmptyObject(t),o=S.speed(e,n,r),a=function(){var e=ft(this,S.extend({},t),o);(i||Y.get(this,"finish"))&&e.stop(!0)};return a.finish=a,i||!1===o.queue?this.each(a):this.queue(o.queue,a)},stop:function(i,e,o){var a=function(e){var t=e.stop;delete e.stop,t(o)};return"string"!=typeof i&&(o=e,e=i,i=void 0),e&&this.queue(i||"fx",[]),this.each(function(){var e=!0,t=null!=i&&i+"queueHooks",n=S.timers,r=Y.get(this);if(t)r[t]&&r[t].stop&&a(r[t]);else for(t in r)r[t]&&r[t].stop&&at.test(t)&&a(r[t]);for(t=n.length;t--;)n[t].elem!==this||null!=i&&n[t].queue!==i||(n[t].anim.stop(o),e=!1,n.splice(t,1));!e&&o||S.dequeue(this,i)})},finish:function(a){return!1!==a&&(a=a||"fx"),this.each(function(){var e,t=Y.get(this),n=t[a+"queue"],r=t[a+"queueHooks"],i=S.timers,o=n?n.length:0;for(t.finish=!0,S.queue(this,a,[]),r&&r.stop&&r.stop.call(this,!0),e=i.length;e--;)i[e].elem===this&&i[e].queue===a&&(i[e].anim.stop(!0),i.splice(e,1));for(e=0;e<o;e++)n[e]&&n[e].finish&&n[e].finish.call(this);delete t.finish})}}),S.each(["toggle","show","hide"],function(e,r){var i=S.fn[r];S.fn[r]=function(e,t,n){return null==e||"boolean"==typeof e?i.apply(this,arguments):this.animate(lt(r,!0),e,t,n)}}),S.each({slideDown:lt("show"),slideUp:lt("hide"),slideToggle:lt("toggle"),fadeIn:{opacity:"show"},fadeOut:{opacity:"hide"},fadeToggle:{opacity:"toggle"}},function(e,r){S.fn[e]=function(e,t,n){return this.animate(r,e,t,n)}}),S.timers=[],S.fx.tick=function(){var e,t=0,n=S.timers;for(tt=Date.now();t<n.length;t++)(e=n[t])()||n[t]!==e||n.splice(t--,1);n.length||S.fx.stop(),tt=void 0},S.fx.timer=function(e){S.timers.push(e),S.fx.start()},S.fx.interval=13,S.fx.start=function(){nt||(nt=!0,st())},S.fx.stop=function(){nt=null},S.fx.speeds={slow:600,fast:200,_default:400},S.fn.delay=function(r,e){return r=S.fx&&S.fx.speeds[r]||r,e=e||"fx",this.queue(e,function(e,t){var n=C.setTimeout(e,r);t.stop=function(){C.clearTimeout(n)}})},rt=E.createElement("input"),it=E.createElement("select").appendChild(E.createElement("option")),rt.type="checkbox",y.checkOn=""!==rt.value,y.optSelected=it.selected,(rt=E.createElement("input")).value="t",rt.type="radio",y.radioValue="t"===rt.value;var pt,dt=S.expr.attrHandle;S.fn.extend({attr:function(e,t){return $(this,S.attr,e,t,1<arguments.length)},removeAttr:function(e){return this.each(function(){S.removeAttr(this,e)})}}),S.extend({attr:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return"undefined"==typeof e.getAttribute?S.prop(e,t,n):(1===o&&S.isXMLDoc(e)||(i=S.attrHooks[t.toLowerCase()]||(S.expr.match.bool.test(t)?pt:void 0)),void 0!==n?null===n?void S.removeAttr(e,t):i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:(e.setAttribute(t,n+""),n):i&&"get"in i&&null!==(r=i.get(e,t))?r:null==(r=S.find.attr(e,t))?void 0:r)},attrHooks:{type:{set:function(e,t){if(!y.radioValue&&"radio"===t&&A(e,"input")){var n=e.value;return e.setAttribute("type",t),n&&(e.value=n),t}}}},removeAttr:function(e,t){var n,r=0,i=t&&t.match(P);if(i&&1===e.nodeType)while(n=i[r++])e.removeAttribute(n)}}),pt={set:function(e,t,n){return!1===t?S.removeAttr(e,n):e.setAttribute(n,n),n}},S.each(S.expr.match.bool.source.match(/\w+/g),function(e,t){var a=dt[t]||S.find.attr;dt[t]=function(e,t,n){var r,i,o=t.toLowerCase();return n||(i=dt[o],dt[o]=r,r=null!=a(e,t,n)?o:null,dt[o]=i),r}});var ht=/^(?:input|select|textarea|button)$/i,gt=/^(?:a|area)$/i;function vt(e){return(e.match(P)||[]).join(" ")}function yt(e){return e.getAttribute&&e.getAttribute("class")||""}function mt(e){return Array.isArray(e)?e:"string"==typeof e&&e.match(P)||[]}S.fn.extend({prop:function(e,t){return $(this,S.prop,e,t,1<arguments.length)},removeProp:function(e){return this.each(function(){delete this[S.propFix[e]||e]})}}),S.extend({prop:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return 1===o&&S.isXMLDoc(e)||(t=S.propFix[t]||t,i=S.propHooks[t]),void 0!==n?i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:e[t]=n:i&&"get"in i&&null!==(r=i.get(e,t))?r:e[t]},propHooks:{tabIndex:{get:function(e){var t=S.find.attr(e,"tabindex");return t?parseInt(t,10):ht.test(e.nodeName)||gt.test(e.nodeName)&&e.href?0:-1}}},propFix:{"for":"htmlFor","class":"className"}}),y.optSelected||(S.propHooks.selected={get:function(e){var t=e.parentNode;return t&&t.parentNode&&t.parentNode.selectedIndex,null},set:function(e){var t=e.parentNode;t&&(t.selectedIndex,t.parentNode&&t.parentNode.selectedIndex)}}),S.each(["tabIndex","readOnly","maxLength","cellSpacing","cellPadding","rowSpan","colSpan","useMap","frameBorder","contentEditable"],function(){S.propFix[this.toLowerCase()]=this}),S.fn.extend({addClass:function(t){var e,n,r,i,o,a,s,u=0;if(m(t))return this.each(function(e){S(this).addClass(t.call(this,e,yt(this)))});if((e=mt(t)).length)while(n=this[u++])if(i=yt(n),r=1===n.nodeType&&" "+vt(i)+" "){a=0;while(o=e[a++])r.indexOf(" "+o+" ")<0&&(r+=o+" ");i!==(s=vt(r))&&n.setAttribute("class",s)}return this},removeClass:function(t){var e,n,r,i,o,a,s,u=0;if(m(t))return this.each(function(e){S(this).removeClass(t.call(this,e,yt(this)))});if(!arguments.length)return this.attr("class","");if((e=mt(t)).length)while(n=this[u++])if(i=yt(n),r=1===n.nodeType&&" "+vt(i)+" "){a=0;while(o=e[a++])while(-1<r.indexOf(" "+o+" "))r=r.replace(" "+o+" "," ");i!==(s=vt(r))&&n.setAttribute("class",s)}return this},toggleClass:function(i,t){var o=typeof i,a="string"===o||Array.isArray(i);return"boolean"==typeof t&&a?t?this.addClass(i):this.removeClass(i):m(i)?this.each(function(e){S(this).toggleClass(i.call(this,e,yt(this),t),t)}):this.each(function(){var e,t,n,r;if(a){t=0,n=S(this),r=mt(i);while(e=r[t++])n.hasClass(e)?n.removeClass(e):n.addClass(e)}else void 0!==i&&"boolean"!==o||((e=yt(this))&&Y.set(this,"__className__",e),this.setAttribute&&this.setAttribute("class",e||!1===i?"":Y.get(this,"__className__")||""))})},hasClass:function(e){var t,n,r=0;t=" "+e+" ";while(n=this[r++])if(1===n.nodeType&&-1<(" "+vt(yt(n))+" ").indexOf(t))return!0;return!1}});var xt=/\r/g;S.fn.extend({val:function(n){var r,e,i,t=this[0];return arguments.length?(i=m(n),this.each(function(e){var t;1===this.nodeType&&(null==(t=i?n.call(this,e,S(this).val()):n)?t="":"number"==typeof t?t+="":Array.isArray(t)&&(t=S.map(t,function(e){return null==e?"":e+""})),(r=S.valHooks[this.type]||S.valHooks[this.nodeName.toLowerCase()])&&"set"in r&&void 0!==r.set(this,t,"value")||(this.value=t))})):t?(r=S.valHooks[t.type]||S.valHooks[t.nodeName.toLowerCase()])&&"get"in r&&void 0!==(e=r.get(t,"value"))?e:"string"==typeof(e=t.value)?e.replace(xt,""):null==e?"":e:void 0}}),S.extend({valHooks:{option:{get:function(e){var t=S.find.attr(e,"value");return null!=t?t:vt(S.text(e))}},select:{get:function(e){var t,n,r,i=e.options,o=e.selectedIndex,a="select-one"===e.type,s=a?null:[],u=a?o+1:i.length;for(r=o<0?u:a?o:0;r<u;r++)if(((n=i[r]).selected||r===o)&&!n.disabled&&(!n.parentNode.disabled||!A(n.parentNode,"optgroup"))){if(t=S(n).val(),a)return t;s.push(t)}return s},set:function(e,t){var n,r,i=e.options,o=S.makeArray(t),a=i.length;while(a--)((r=i[a]).selected=-1<S.inArray(S.valHooks.option.get(r),o))&&(n=!0);return n||(e.selectedIndex=-1),o}}}}),S.each(["radio","checkbox"],function(){S.valHooks[this]={set:function(e,t){if(Array.isArray(t))return e.checked=-1<S.inArray(S(e).val(),t)}},y.checkOn||(S.valHooks[this].get=function(e){return null===e.getAttribute("value")?"on":e.value})}),y.focusin="onfocusin"in C;var bt=/^(?:focusinfocus|focusoutblur)$/,wt=function(e){e.stopPropagation()};S.extend(S.event,{trigger:function(e,t,n,r){var i,o,a,s,u,l,c,f,p=[n||E],d=v.call(e,"type")?e.type:e,h=v.call(e,"namespace")?e.namespace.split("."):[];if(o=f=a=n=n||E,3!==n.nodeType&&8!==n.nodeType&&!bt.test(d+S.event.triggered)&&(-1<d.indexOf(".")&&(d=(h=d.split(".")).shift(),h.sort()),u=d.indexOf(":")<0&&"on"+d,(e=e[S.expando]?e:new S.Event(d,"object"==typeof e&&e)).isTrigger=r?2:3,e.namespace=h.join("."),e.rnamespace=e.namespace?new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"):null,e.result=void 0,e.target||(e.target=n),t=null==t?[e]:S.makeArray(t,[e]),c=S.event.special[d]||{},r||!c.trigger||!1!==c.trigger.apply(n,t))){if(!r&&!c.noBubble&&!x(n)){for(s=c.delegateType||d,bt.test(s+d)||(o=o.parentNode);o;o=o.parentNode)p.push(o),a=o;a===(n.ownerDocument||E)&&p.push(a.defaultView||a.parentWindow||C)}i=0;while((o=p[i++])&&!e.isPropagationStopped())f=o,e.type=1<i?s:c.bindType||d,(l=(Y.get(o,"events")||Object.create(null))[e.type]&&Y.get(o,"handle"))&&l.apply(o,t),(l=u&&o[u])&&l.apply&&V(o)&&(e.result=l.apply(o,t),!1===e.result&&e.preventDefault());return e.type=d,r||e.isDefaultPrevented()||c._default&&!1!==c._default.apply(p.pop(),t)||!V(n)||u&&m(n[d])&&!x(n)&&((a=n[u])&&(n[u]=null),S.event.triggered=d,e.isPropagationStopped()&&f.addEventListener(d,wt),n[d](),e.isPropagationStopped()&&f.removeEventListener(d,wt),S.event.triggered=void 0,a&&(n[u]=a)),e.result}},simulate:function(e,t,n){var r=S.extend(new S.Event,n,{type:e,isSimulated:!0});S.event.trigger(r,null,t)}}),S.fn.extend({trigger:function(e,t){return this.each(function(){S.event.trigger(e,t,this)})},triggerHandler:function(e,t){var n=this[0];if(n)return S.event.trigger(e,t,n,!0)}}),y.focusin||S.each({focus:"focusin",blur:"focusout"},function(n,r){var i=function(e){S.event.simulate(r,e.target,S.event.fix(e))};S.event.special[r]={setup:function(){var e=this.ownerDocument||this.document||this,t=Y.access(e,r);t||e.addEventListener(n,i,!0),Y.access(e,r,(t||0)+1)},teardown:function(){var e=this.ownerDocument||this.document||this,t=Y.access(e,r)-1;t?Y.access(e,r,t):(e.removeEventListener(n,i,!0),Y.remove(e,r))}}});var Tt=C.location,Ct={guid:Date.now()},Et=/\?/;S.parseXML=function(e){var t;if(!e||"string"!=typeof e)return null;try{t=(new C.DOMParser).parseFromString(e,"text/xml")}catch(e){t=void 0}return t&&!t.getElementsByTagName("parsererror").length||S.error("Invalid XML: "+e),t};var St=/\[\]$/,kt=/\r?\n/g,At=/^(?:submit|button|image|reset|file)$/i,Nt=/^(?:input|select|textarea|keygen)/i;function Dt(n,e,r,i){var t;if(Array.isArray(e))S.each(e,function(e,t){r||St.test(n)?i(n,t):Dt(n+"["+("object"==typeof t&&null!=t?e:"")+"]",t,r,i)});else if(r||"object"!==w(e))i(n,e);else for(t in e)Dt(n+"["+t+"]",e[t],r,i)}S.param=function(e,t){var n,r=[],i=function(e,t){var n=m(t)?t():t;r[r.length]=encodeURIComponent(e)+"="+encodeURIComponent(null==n?"":n)};if(null==e)return"";if(Array.isArray(e)||e.jquery&&!S.isPlainObject(e))S.each(e,function(){i(this.name,this.value)});else for(n in e)Dt(n,e[n],t,i);return r.join("&")},S.fn.extend({serialize:function(){return S.param(this.serializeArray())},serializeArray:function(){return this.map(function(){var e=S.prop(this,"elements");return e?S.makeArray(e):this}).filter(function(){var e=this.type;return this.name&&!S(this).is(":disabled")&&Nt.test(this.nodeName)&&!At.test(e)&&(this.checked||!pe.test(e))}).map(function(e,t){var n=S(this).val();return null==n?null:Array.isArray(n)?S.map(n,function(e){return{name:t.name,value:e.replace(kt,"\r\n")}}):{name:t.name,value:n.replace(kt,"\r\n")}}).get()}});var jt=/%20/g,qt=/#.*$/,Lt=/([?&])_=[^&]*/,Ht=/^(.*?):[ \t]*([^\r\n]*)$/gm,Ot=/^(?:GET|HEAD)$/,Pt=/^\/\//,Rt={},Mt={},It="*/".concat("*"),Wt=E.createElement("a");function Ft(o){return function(e,t){"string"!=typeof e&&(t=e,e="*");var n,r=0,i=e.toLowerCase().match(P)||[];if(m(t))while(n=i[r++])"+"===n[0]?(n=n.slice(1)||"*",(o[n]=o[n]||[]).unshift(t)):(o[n]=o[n]||[]).push(t)}}function Bt(t,i,o,a){var s={},u=t===Mt;function l(e){var r;return s[e]=!0,S.each(t[e]||[],function(e,t){var n=t(i,o,a);return"string"!=typeof n||u||s[n]?u?!(r=n):void 0:(i.dataTypes.unshift(n),l(n),!1)}),r}return l(i.dataTypes[0])||!s["*"]&&l("*")}function $t(e,t){var n,r,i=S.ajaxSettings.flatOptions||{};for(n in t)void 0!==t[n]&&((i[n]?e:r||(r={}))[n]=t[n]);return r&&S.extend(!0,e,r),e}Wt.href=Tt.href,S.extend({active:0,lastModified:{},etag:{},ajaxSettings:{url:Tt.href,type:"GET",isLocal:/^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),global:!0,processData:!0,async:!0,contentType:"application/x-www-form-urlencoded; charset=UTF-8",accepts:{"*":It,text:"text/plain",html:"text/html",xml:"application/xml, text/xml",json:"application/json, text/javascript"},contents:{xml:/\bxml\b/,html:/\bhtml/,json:/\bjson\b/},responseFields:{xml:"responseXML",text:"responseText",json:"responseJSON"},converters:{"* text":String,"text html":!0,"text json":JSON.parse,"text xml":S.parseXML},flatOptions:{url:!0,context:!0}},ajaxSetup:function(e,t){return t?$t($t(e,S.ajaxSettings),t):$t(S.ajaxSettings,e)},ajaxPrefilter:Ft(Rt),ajaxTransport:Ft(Mt),ajax:function(e,t){"object"==typeof e&&(t=e,e=void 0),t=t||{};var c,f,p,n,d,r,h,g,i,o,v=S.ajaxSetup({},t),y=v.context||v,m=v.context&&(y.nodeType||y.jquery)?S(y):S.event,x=S.Deferred(),b=S.Callbacks("once memory"),w=v.statusCode||{},a={},s={},u="canceled",T={readyState:0,getResponseHeader:function(e){var t;if(h){if(!n){n={};while(t=Ht.exec(p))n[t[1].toLowerCase()+" "]=(n[t[1].toLowerCase()+" "]||[]).concat(t[2])}t=n[e.toLowerCase()+" "]}return null==t?null:t.join(", ")},getAllResponseHeaders:function(){return h?p:null},setRequestHeader:function(e,t){return null==h&&(e=s[e.toLowerCase()]=s[e.toLowerCase()]||e,a[e]=t),this},overrideMimeType:function(e){return null==h&&(v.mimeType=e),this},statusCode:function(e){var t;if(e)if(h)T.always(e[T.status]);else for(t in e)w[t]=[w[t],e[t]];return this},abort:function(e){var t=e||u;return c&&c.abort(t),l(0,t),this}};if(x.promise(T),v.url=((e||v.url||Tt.href)+"").replace(Pt,Tt.protocol+"//"),v.type=t.method||t.type||v.method||v.type,v.dataTypes=(v.dataType||"*").toLowerCase().match(P)||[""],null==v.crossDomain){r=E.createElement("a");try{r.href=v.url,r.href=r.href,v.crossDomain=Wt.protocol+"//"+Wt.host!=r.protocol+"//"+r.host}catch(e){v.crossDomain=!0}}if(v.data&&v.processData&&"string"!=typeof v.data&&(v.data=S.param(v.data,v.traditional)),Bt(Rt,v,t,T),h)return T;for(i in(g=S.event&&v.global)&&0==S.active++&&S.event.trigger("ajaxStart"),v.type=v.type.toUpperCase(),v.hasContent=!Ot.test(v.type),f=v.url.replace(qt,""),v.hasContent?v.data&&v.processData&&0===(v.contentType||"").indexOf("application/x-www-form-urlencoded")&&(v.data=v.data.replace(jt,"+")):(o=v.url.slice(f.length),v.data&&(v.processData||"string"==typeof v.data)&&(f+=(Et.test(f)?"&":"?")+v.data,delete v.data),!1===v.cache&&(f=f.replace(Lt,"$1"),o=(Et.test(f)?"&":"?")+"_="+Ct.guid+++o),v.url=f+o),v.ifModified&&(S.lastModified[f]&&T.setRequestHeader("If-Modified-Since",S.lastModified[f]),S.etag[f]&&T.setRequestHeader("If-None-Match",S.etag[f])),(v.data&&v.hasContent&&!1!==v.contentType||t.contentType)&&T.setRequestHeader("Content-Type",v.contentType),T.setRequestHeader("Accept",v.dataTypes[0]&&v.accepts[v.dataTypes[0]]?v.accepts[v.dataTypes[0]]+("*"!==v.dataTypes[0]?", "+It+"; q=0.01":""):v.accepts["*"]),v.headers)T.setRequestHeader(i,v.headers[i]);if(v.beforeSend&&(!1===v.beforeSend.call(y,T,v)||h))return T.abort();if(u="abort",b.add(v.complete),T.done(v.success),T.fail(v.error),c=Bt(Mt,v,t,T)){if(T.readyState=1,g&&m.trigger("ajaxSend",[T,v]),h)return T;v.async&&0<v.timeout&&(d=C.setTimeout(function(){T.abort("timeout")},v.timeout));try{h=!1,c.send(a,l)}catch(e){if(h)throw e;l(-1,e)}}else l(-1,"No Transport");function l(e,t,n,r){var i,o,a,s,u,l=t;h||(h=!0,d&&C.clearTimeout(d),c=void 0,p=r||"",T.readyState=0<e?4:0,i=200<=e&&e<300||304===e,n&&(s=function(e,t,n){var r,i,o,a,s=e.contents,u=e.dataTypes;while("*"===u[0])u.shift(),void 0===r&&(r=e.mimeType||t.getResponseHeader("Content-Type"));if(r)for(i in s)if(s[i]&&s[i].test(r)){u.unshift(i);break}if(u[0]in n)o=u[0];else{for(i in n){if(!u[0]||e.converters[i+" "+u[0]]){o=i;break}a||(a=i)}o=o||a}if(o)return o!==u[0]&&u.unshift(o),n[o]}(v,T,n)),!i&&-1<S.inArray("script",v.dataTypes)&&(v.converters["text script"]=function(){}),s=function(e,t,n,r){var i,o,a,s,u,l={},c=e.dataTypes.slice();if(c[1])for(a in e.converters)l[a.toLowerCase()]=e.converters[a];o=c.shift();while(o)if(e.responseFields[o]&&(n[e.responseFields[o]]=t),!u&&r&&e.dataFilter&&(t=e.dataFilter(t,e.dataType)),u=o,o=c.shift())if("*"===o)o=u;else if("*"!==u&&u!==o){if(!(a=l[u+" "+o]||l["* "+o]))for(i in l)if((s=i.split(" "))[1]===o&&(a=l[u+" "+s[0]]||l["* "+s[0]])){!0===a?a=l[i]:!0!==l[i]&&(o=s[0],c.unshift(s[1]));break}if(!0!==a)if(a&&e["throws"])t=a(t);else try{t=a(t)}catch(e){return{state:"parsererror",error:a?e:"No conversion from "+u+" to "+o}}}return{state:"success",data:t}}(v,s,T,i),i?(v.ifModified&&((u=T.getResponseHeader("Last-Modified"))&&(S.lastModified[f]=u),(u=T.getResponseHeader("etag"))&&(S.etag[f]=u)),204===e||"HEAD"===v.type?l="nocontent":304===e?l="notmodified":(l=s.state,o=s.data,i=!(a=s.error))):(a=l,!e&&l||(l="error",e<0&&(e=0))),T.status=e,T.statusText=(t||l)+"",i?x.resolveWith(y,[o,l,T]):x.rejectWith(y,[T,l,a]),T.statusCode(w),w=void 0,g&&m.trigger(i?"ajaxSuccess":"ajaxError",[T,v,i?o:a]),b.fireWith(y,[T,l]),g&&(m.trigger("ajaxComplete",[T,v]),--S.active||S.event.trigger("ajaxStop")))}return T},getJSON:function(e,t,n){return S.get(e,t,n,"json")},getScript:function(e,t){return S.get(e,void 0,t,"script")}}),S.each(["get","post"],function(e,i){S[i]=function(e,t,n,r){return m(t)&&(r=r||n,n=t,t=void 0),S.ajax(S.extend({url:e,type:i,dataType:r,data:t,success:n},S.isPlainObject(e)&&e))}}),S.ajaxPrefilter(function(e){var t;for(t in e.headers)"content-type"===t.toLowerCase()&&(e.contentType=e.headers[t]||"")}),S._evalUrl=function(e,t,n){return S.ajax({url:e,type:"GET",dataType:"script",cache:!0,async:!1,global:!1,converters:{"text script":function(){}},dataFilter:function(e){S.globalEval(e,t,n)}})},S.fn.extend({wrapAll:function(e){var t;return this[0]&&(m(e)&&(e=e.call(this[0])),t=S(e,this[0].ownerDocument).eq(0).clone(!0),this[0].parentNode&&t.insertBefore(this[0]),t.map(function(){var e=this;while(e.firstElementChild)e=e.firstElementChild;return e}).append(this)),this},wrapInner:function(n){return m(n)?this.each(function(e){S(this).wrapInner(n.call(this,e))}):this.each(function(){var e=S(this),t=e.contents();t.length?t.wrapAll(n):e.append(n)})},wrap:function(t){var n=m(t);return this.each(function(e){S(this).wrapAll(n?t.call(this,e):t)})},unwrap:function(e){return this.parent(e).not("body").each(function(){S(this).replaceWith(this.childNodes)}),this}}),S.expr.pseudos.hidden=function(e){return!S.expr.pseudos.visible(e)},S.expr.pseudos.visible=function(e){return!!(e.offsetWidth||e.offsetHeight||e.getClientRects().length)},S.ajaxSettings.xhr=function(){try{return new C.XMLHttpRequest}catch(e){}};var _t={0:200,1223:204},zt=S.ajaxSettings.xhr();y.cors=!!zt&&"withCredentials"in zt,y.ajax=zt=!!zt,S.ajaxTransport(function(i){var o,a;if(y.cors||zt&&!i.crossDomain)return{send:function(e,t){var n,r=i.xhr();if(r.open(i.type,i.url,i.async,i.username,i.password),i.xhrFields)for(n in i.xhrFields)r[n]=i.xhrFields[n];for(n in i.mimeType&&r.overrideMimeType&&r.overrideMimeType(i.mimeType),i.crossDomain||e["X-Requested-With"]||(e["X-Requested-With"]="XMLHttpRequest"),e)r.setRequestHeader(n,e[n]);o=function(e){return function(){o&&(o=a=r.onload=r.onerror=r.onabort=r.ontimeout=r.onreadystatechange=null,"abort"===e?r.abort():"error"===e?"number"!=typeof r.status?t(0,"error"):t(r.status,r.statusText):t(_t[r.status]||r.status,r.statusText,"text"!==(r.responseType||"text")||"string"!=typeof r.responseText?{binary:r.response}:{text:r.responseText},r.getAllResponseHeaders()))}},r.onload=o(),a=r.onerror=r.ontimeout=o("error"),void 0!==r.onabort?r.onabort=a:r.onreadystatechange=function(){4===r.readyState&&C.setTimeout(function(){o&&a()})},o=o("abort");try{r.send(i.hasContent&&i.data||null)}catch(e){if(o)throw e}},abort:function(){o&&o()}}}),S.ajaxPrefilter(function(e){e.crossDomain&&(e.contents.script=!1)}),S.ajaxSetup({accepts:{script:"text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"},contents:{script:/\b(?:java|ecma)script\b/},converters:{"text script":function(e){return S.globalEval(e),e}}}),S.ajaxPrefilter("script",function(e){void 0===e.cache&&(e.cache=!1),e.crossDomain&&(e.type="GET")}),S.ajaxTransport("script",function(n){var r,i;if(n.crossDomain||n.scriptAttrs)return{send:function(e,t){r=S("<script>").attr(n.scriptAttrs||{}).prop({charset:n.scriptCharset,src:n.url}).on("load error",i=function(e){r.remove(),i=null,e&&t("error"===e.type?404:200,e.type)}),E.head.appendChild(r[0])},abort:function(){i&&i()}}});var Ut,Xt=[],Vt=/(=)\?(?=&|$)|\?\?/;S.ajaxSetup({jsonp:"callback",jsonpCallback:function(){var e=Xt.pop()||S.expando+"_"+Ct.guid++;return this[e]=!0,e}}),S.ajaxPrefilter("json jsonp",function(e,t,n){var r,i,o,a=!1!==e.jsonp&&(Vt.test(e.url)?"url":"string"==typeof e.data&&0===(e.contentType||"").indexOf("application/x-www-form-urlencoded")&&Vt.test(e.data)&&"data");if(a||"jsonp"===e.dataTypes[0])return r=e.jsonpCallback=m(e.jsonpCallback)?e.jsonpCallback():e.jsonpCallback,a?e[a]=e[a].replace(Vt,"$1"+r):!1!==e.jsonp&&(e.url+=(Et.test(e.url)?"&":"?")+e.jsonp+"="+r),e.converters["script json"]=function(){return o||S.error(r+" was not called"),o[0]},e.dataTypes[0]="json",i=C[r],C[r]=function(){o=arguments},n.always(function(){void 0===i?S(C).removeProp(r):C[r]=i,e[r]&&(e.jsonpCallback=t.jsonpCallback,Xt.push(r)),o&&m(i)&&i(o[0]),o=i=void 0}),"script"}),y.createHTMLDocument=((Ut=E.implementation.createHTMLDocument("").body).innerHTML="<form></form><form></form>",2===Ut.childNodes.length),S.parseHTML=function(e,t,n){return"string"!=typeof e?[]:("boolean"==typeof t&&(n=t,t=!1),t||(y.createHTMLDocument?((r=(t=E.implementation.createHTMLDocument("")).createElement("base")).href=E.location.href,t.head.appendChild(r)):t=E),o=!n&&[],(i=N.exec(e))?[t.createElement(i[1])]:(i=xe([e],t,o),o&&o.length&&S(o).remove(),S.merge([],i.childNodes)));var r,i,o},S.fn.load=function(e,t,n){var r,i,o,a=this,s=e.indexOf(" ");return-1<s&&(r=vt(e.slice(s)),e=e.slice(0,s)),m(t)?(n=t,t=void 0):t&&"object"==typeof t&&(i="POST"),0<a.length&&S.ajax({url:e,type:i||"GET",dataType:"html",data:t}).done(function(e){o=arguments,a.html(r?S("<div>").append(S.parseHTML(e)).find(r):e)}).always(n&&function(e,t){a.each(function(){n.apply(this,o||[e.responseText,t,e])})}),this},S.expr.pseudos.animated=function(t){return S.grep(S.timers,function(e){return t===e.elem}).length},S.offset={setOffset:function(e,t,n){var r,i,o,a,s,u,l=S.css(e,"position"),c=S(e),f={};"static"===l&&(e.style.position="relative"),s=c.offset(),o=S.css(e,"top"),u=S.css(e,"left"),("absolute"===l||"fixed"===l)&&-1<(o+u).indexOf("auto")?(a=(r=c.position()).top,i=r.left):(a=parseFloat(o)||0,i=parseFloat(u)||0),m(t)&&(t=t.call(e,n,S.extend({},s))),null!=t.top&&(f.top=t.top-s.top+a),null!=t.left&&(f.left=t.left-s.left+i),"using"in t?t.using.call(e,f):("number"==typeof f.top&&(f.top+="px"),"number"==typeof f.left&&(f.left+="px"),c.css(f))}},S.fn.extend({offset:function(t){if(arguments.length)return void 0===t?this:this.each(function(e){S.offset.setOffset(this,t,e)});var e,n,r=this[0];return r?r.getClientRects().length?(e=r.getBoundingClientRect(),n=r.ownerDocument.defaultView,{top:e.top+n.pageYOffset,left:e.left+n.pageXOffset}):{top:0,left:0}:void 0},position:function(){if(this[0]){var e,t,n,r=this[0],i={top:0,left:0};if("fixed"===S.css(r,"position"))t=r.getBoundingClientRect();else{t=this.offset(),n=r.ownerDocument,e=r.offsetParent||n.documentElement;while(e&&(e===n.body||e===n.documentElement)&&"static"===S.css(e,"position"))e=e.parentNode;e&&e!==r&&1===e.nodeType&&((i=S(e).offset()).top+=S.css(e,"borderTopWidth",!0),i.left+=S.css(e,"borderLeftWidth",!0))}return{top:t.top-i.top-S.css(r,"marginTop",!0),left:t.left-i.left-S.css(r,"marginLeft",!0)}}},offsetParent:function(){return this.map(function(){var e=this.offsetParent;while(e&&"static"===S.css(e,"position"))e=e.offsetParent;return e||re})}}),S.each({scrollLeft:"pageXOffset",scrollTop:"pageYOffset"},function(t,i){var o="pageYOffset"===i;S.fn[t]=function(e){return $(this,function(e,t,n){var r;if(x(e)?r=e:9===e.nodeType&&(r=e.defaultView),void 0===n)return r?r[i]:e[t];r?r.scrollTo(o?r.pageXOffset:n,o?n:r.pageYOffset):e[t]=n},t,e,arguments.length)}}),S.each(["top","left"],function(e,n){S.cssHooks[n]=$e(y.pixelPosition,function(e,t){if(t)return t=Be(e,n),Me.test(t)?S(e).position()[n]+"px":t})}),S.each({Height:"height",Width:"width"},function(a,s){S.each({padding:"inner"+a,content:s,"":"outer"+a},function(r,o){S.fn[o]=function(e,t){var n=arguments.length&&(r||"boolean"!=typeof e),i=r||(!0===e||!0===t?"margin":"border");return $(this,function(e,t,n){var r;return x(e)?0===o.indexOf("outer")?e["inner"+a]:e.document.documentElement["client"+a]:9===e.nodeType?(r=e.documentElement,Math.max(e.body["scroll"+a],r["scroll"+a],e.body["offset"+a],r["offset"+a],r["client"+a])):void 0===n?S.css(e,t,i):S.style(e,t,n,i)},s,n?e:void 0,n)}})}),S.each(["ajaxStart","ajaxStop","ajaxComplete","ajaxError","ajaxSuccess","ajaxSend"],function(e,t){S.fn[t]=function(e){return this.on(t,e)}}),S.fn.extend({bind:function(e,t,n){return this.on(e,null,t,n)},unbind:function(e,t){return this.off(e,null,t)},delegate:function(e,t,n,r){return this.on(t,e,n,r)},undelegate:function(e,t,n){return 1===arguments.length?this.off(e,"**"):this.off(t,e||"**",n)},hover:function(e,t){return this.mouseenter(e).mouseleave(t||e)}}),S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "),function(e,n){S.fn[n]=function(e,t){return 0<arguments.length?this.on(n,null,e,t):this.trigger(n)}});var Gt=/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;S.proxy=function(e,t){var n,r,i;if("string"==typeof t&&(n=e[t],t=e,e=n),m(e))return r=s.call(arguments,2),(i=function(){return e.apply(t||this,r.concat(s.call(arguments)))}).guid=e.guid=e.guid||S.guid++,i},S.holdReady=function(e){e?S.readyWait++:S.ready(!0)},S.isArray=Array.isArray,S.parseJSON=JSON.parse,S.nodeName=A,S.isFunction=m,S.isWindow=x,S.camelCase=X,S.type=w,S.now=Date.now,S.isNumeric=function(e){var t=S.type(e);return("number"===t||"string"===t)&&!isNaN(e-parseFloat(e))},S.trim=function(e){return null==e?"":(e+"").replace(Gt,"")},"function"==typeof define&&define.amd&&define("jquery",[],function(){return S});var Yt=C.jQuery,Qt=C.$;return S.noConflict=function(e){return C.$===S&&(C.$=Qt),e&&C.jQuery===S&&(C.jQuery=Yt),S},"undefined"==typeof e&&(C.jQuery=C.$=S),S});
 </script>
-    <script type="text/javascript">
+<script type="text/javascript">
 /*
  * jQuery Templates Plugin 1.0.0pre
  * http://github.com/jquery/jquery-tmpl
  * Requires jQuery 1.4.2
  *
  * Copyright Software Freedom Conservancy, Inc.
  * Dual licensed under the MIT or GPL Version 2 licenses.
  * http://jquery.org/license
  */
 (function(a){var r=a.fn.domManip,d="_tmplitem",q=/^[^<]*(<[\w\W]+>)[^>]*$|\{\{\! /,b={},f={},e,p={key:0,data:{}},i=0,c=0,l=[];function g(g,d,h,e){var c={data:e||(e===0||e===false)?e:d?d.data:{},_wrap:d?d._wrap:null,tmpl:null,parent:d||null,nodes:[],calls:u,nest:w,wrap:x,html:v,update:t};g&&a.extend(c,g,{nodes:[],parent:d});if(h){c.tmpl=h;c._ctnt=c._ctnt||c.tmpl(a,c);c.key=++i;(l.length?f:b)[i]=c}return c}a.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(f,d){a.fn[f]=function(n){var g=[],i=a(n),k,h,m,l,j=this.length===1&&this[0].parentNode;e=b||{};if(j&&j.nodeType===11&&j.childNodes.length===1&&i.length===1){i[d](this[0]);g=this}else{for(h=0,m=i.length;h<m;h++){c=h;k=(h>0?this.clone(true):this).get();a(i[h])[d](k);g=g.concat(k)}c=0;g=this.pushStack(g,f,i.selector)}l=e;e=null;a.tmpl.complete(l);return g}});a.fn.extend({tmpl:function(d,c,b){return a.tmpl(this[0],d,c,b)},tmplItem:function(){return a.tmplItem(this[0])},template:function(b){return a.template(b,this[0])},domManip:function(d,m,k){if(d[0]&&a.isArray(d[0])){var g=a.makeArray(arguments),h=d[0],j=h.length,i=0,f;while(i<j&&!(f=a.data(h[i++],"tmplItem")));if(f&&c)g[2]=function(b){a.tmpl.afterManip(this,b,k)};r.apply(this,g)}else r.apply(this,arguments);c=0;!e&&a.tmpl.complete(b);return this}});a.extend({tmpl:function(d,h,e,c){var i,k=!c;if(k){c=p;d=a.template[d]||a.template(null,d);f={}}else if(!d){d=c.tmpl;b[c.key]=c;c.nodes=[];c.wrapped&&n(c,c.wrapped);return a(j(c,null,c.tmpl(a,c)))}if(!d)return[];if(typeof h==="function")h=h.call(c||{});e&&e.wrapped&&n(e,e.wrapped);i=a.isArray(h)?a.map(h,function(a){return a?g(e,c,d,a):null}):[g(e,c,d,h)];return k?a(j(c,null,i)):i},tmplItem:function(b){var c;if(b instanceof a)b=b[0];while(b&&b.nodeType===1&&!(c=a.data(b,"tmplItem"))&&(b=b.parentNode));return c||p},template:function(c,b){if(b){if(typeof b==="string")b=o(b);else if(b instanceof a)b=b[0]||{};if(b.nodeType)b=a.data(b,"tmpl")||a.data(b,"tmpl",o(b.innerHTML));return typeof c==="string"?(a.template[c]=b):b}return c?typeof c!=="string"?a.template(null,c):a.template[c]||a.template(null,q.test(c)?c:a(c)):null},encode:function(a){return(""+a).split("&").join("&amp;").split("<").join("&lt;").split(">").join("&gt;").split('"').join("&#34;").split("'").join("&#39;")}});a.extend(a.tmpl,{tag:{tmpl:{_default:{$2:"null"},open:"if($notnull_1){__=__.concat($item.nest($1,$2));}"},wrap:{_default:{$2:"null"},open:"$item.calls(__,$1,$2);__=[];",close:"call=$item.calls();__=call._.concat($item.wrap(call,__));"},each:{_default:{$2:"$index, $value"},open:"if($notnull_1){$.each($1a,function($2){with(this){",close:"}});}"},"if":{open:"if(($notnull_1) && $1a){",close:"}"},"else":{_default:{$1:"true"},open:"}else if(($notnull_1) && $1a){"},html:{open:"if($notnull_1){__.push($1a);}"},"=":{_default:{$1:"$data"},open:"if($notnull_1){__.push($.encode($1a));}"},"!":{open:""}},complete:function(){b={}},afterManip:function(f,b,d){var e=b.nodeType===11?a.makeArray(b.childNodes):b.nodeType===1?[b]:[];d.call(f,b);m(e);c++}});function j(e,g,f){var b,c=f?a.map(f,function(a){return typeof a==="string"?e.key?a.replace(/(<\w+)(?=[\s>])(?![^>]*_tmplitem)([^>]*)/g,"$1 "+d+'="'+e.key+'" $2'):a:j(a,e,a._ctnt)}):e;if(g)return c;c=c.join("");c.replace(/^\s*([^<\s][^<]*)?(<[\w\W]+>)([^>]*[^>\s])?\s*$/,function(f,c,e,d){b=a(e).get();m(b);if(c)b=k(c).concat(b);if(d)b=b.concat(k(d))});return b?b:k(c)}function k(c){var b=document.createElement("div");b.innerHTML=c;return a.makeArray(b.childNodes)}function o(b){return new Function("jQuery","$item","var $=jQuery,call,__=[],$data=$item.data;with($data){__.push('"+a.trim(b).replace(/([\\'])/g,"\\$1").replace(/[\r\t\n]/g," ").replace(/\$\{([^\}]*)\}/g,"{{= $1}}").replace(/\{\{(\/?)(\w+|.)(?:\(((?:[^\}]|\}(?!\}))*?)?\))?(?:\s+(.*?)?)?(\(((?:[^\}]|\}(?!\}))*?)\))?\s*\}\}/g,function(m,l,k,g,b,c,d){var j=a.tmpl.tag[k],i,e,f;if(!j)throw"Unknown template tag: "+k;i=j._default||[];if(c&&!/\w$/.test(b)){b+=c;c=""}if(b){b=h(b);d=d?","+h(d)+")":c?")":"";e=c?b.indexOf(".")>-1?b+h(c):"("+b+").call($item"+d:b;f=c?e:"(typeof("+b+")==='function'?("+b+").call($item):("+b+"))"}else f=e=i.$1||"null";g=h(g);return"');"+j[l?"close":"open"].split("$notnull_1").join(b?"typeof("+b+")!=='undefined' && ("+b+")!=null":"true").split("$1a").join(f).split("$1").join(e).split("$2").join(g||i.$2||"")+"__.push('"})+"');}return __;")}function n(c,b){c._wrap=j(c,true,a.isArray(b)?b:[q.test(b)?b:a(b).html()]).join("")}function h(a){return a?a.replace(/\\'/g,"'").replace(/\\\\/g,"\\"):null}function s(b){var a=document.createElement("div");a.appendChild(b.cloneNode(true));return a.innerHTML}function m(o){var n="_"+c,k,j,l={},e,p,h;for(e=0,p=o.length;e<p;e++){if((k=o[e]).nodeType!==1)continue;j=k.getElementsByTagName("*");for(h=j.length-1;h>=0;h--)m(j[h]);m(k)}function m(j){var p,h=j,k,e,m;if(m=j.getAttribute(d)){while(h.parentNode&&(h=h.parentNode).nodeType===1&&!(p=h.getAttribute(d)));if(p!==m){h=h.parentNode?h.nodeType===11?0:h.getAttribute(d)||0:0;if(!(e=b[m])){e=f[m];e=g(e,b[h]||f[h]);e.key=++i;b[i]=e}c&&o(m)}j.removeAttribute(d)}else if(c&&(e=a.data(j,"tmplItem"))){o(e.key);b[e.key]=e;h=a.data(j.parentNode,"tmplItem");h=h?h.key:0}if(e){k=e;while(k&&k.key!=h){k.nodes.push(j);k=k.parent}delete e._ctnt;delete e._wrap;a.data(j,"tmplItem",e)}function o(a){a=a+n;e=l[a]=l[a]||g(e,b[e.parent.key+n]||e.parent)}}}function u(a,d,c,b){if(!a)return l.pop();l.push({_:a,tmpl:d,item:this,data:c,options:b})}function w(d,c,b){return a.tmpl(a.template(d),c,b,this)}function x(b,d){var c=b.options||{};c.wrapped=d;return a.tmpl(a.template(b.tmpl),b.data,c,b.item)}function v(d,c){var b=this._wrap;return a.map(a(a.isArray(b)?b.join(""):b).filter(d||"*"),function(a){return c?a.innerText||a.textContent:a.outerHTML||s(a)})}function t(){var b=this.nodes;a.tmpl(null,null,null,this).insertBefore(b[0]);a(b).remove()}})(jQuery);
 </script>
-    <script type="text/javascript">
+<script type="text/javascript">
 /*
  * jQuery Highlight plugin
  *
  * Based on highlight v3 by Johann Burkard
  * http://johannburkard.de/blog/programming/javascript/highlight-javascript-text-higlighting-jquery-plugin.html
  *
  * Copyright (c) 2009 Bartek Szopka
  *
  * Licensed under MIT license.
  */
 jQuery.extend({highlight:function(e,t,n,r){if(e.nodeType===3){var i=e.data.match(t);if(i){var s=document.createElement(n||"span");s.className=r||"highlight";var o=e.splitText(i.index);o.splitText(i[0].length);var u=o.cloneNode(true);s.appendChild(u);o.parentNode.replaceChild(s,o);return 1}}else if(e.nodeType===1&&e.childNodes&&!/(script|style)/i.test(e.tagName)&&!(e.tagName===n.toUpperCase()&&e.className===r)){for(var a=0;a<e.childNodes.length;a++){a+=jQuery.highlight(e.childNodes[a],t,n,r)}}return 0}});jQuery.fn.unhighlight=function(e){var t={className:"highlight",element:"span"};jQuery.extend(t,e);return this.find(t.element+"."+t.className).each(function(){var e=this.parentNode;e.replaceChild(this.firstChild,this);e.normalize()}).end()};jQuery.fn.highlight=function(e,t){var n={className:"highlight",element:"span",caseSensitive:false,wordsOnly:false};jQuery.extend(n,t);if(e.constructor===String){e=[e]}e=jQuery.grep(e,function(e,t){return e!=""});e=jQuery.map(e,function(e,t){return e.replace(/[-[\]{}()*+?.,\\^$|#\s]/g,"\\$&")});if(e.length==0){return this}var r=n.caseSensitive?"":"i";var i="("+e.join("|")+")";if(n.wordsOnly){i="\\b"+i+"\\b"}var s=new RegExp(i,r);return this.each(function(){jQuery.highlight(this,s,n.element,n.className)})}
 </script>
-    <script type="text/javascript">
-libdoc = {"all_tags":[],"contains_tags":false,"doc":"<p>Robot Framework Library for generating a random BSN (Burger Service Nummer, i.e. a Dutch citizen service number) for test purposes.\x3c/p>\n<p>A BSN is used in Netherlands to identify a person for government organisations, see <a href=\"https://www.government.nl/topics/personal-data/citizen-service-number-bsn\">this information of the Dutch government\x3c/a>. The number consists of 9 digits and has to pass the eleven test.\x3c/p>\n<p>This test can be explained with the example 211551557. Each digit is multiplied with its position and the results are added up together:\x3c/p>\n<p><code>(9*2) + (8*1) + (7*1) + (6*5) + (5*5) + (4*1) + (3*5) + (2*5) - (1*7) = 110\x3c/code>\x3c/p>\n<p>Note that the digit in position 1 is subtracted from the other results. The total sum can be divided by 11, which means that this number has passed the eleven test.\x3c/p>\n<p>This library generates BSNs for test purposes in the sense that it generates random 9 digit numbers that pass the eleven test. By coincidence a generated number could be a real person's BSN. Yet this library cannot violate such a person's privacy, because it cannot tell you whether a number belongs to a real person or not, nor will it provide you with any personal data related to a BSN. Obviously you should only use this library in test environments.\x3c/p>\n<p>This library brings the following features to Robot Framework:\x3c/p>\n<ul>\n<li>generating a valid BSN\x3c/li>\n<li>generating a BSN that is unique within the current test run\x3c/li>\n<li>generating a number that will not pass the eleven test\x3c/li>\n<li>generating a BSN that starts with specific digits\x3c/li>\n<li>generating a BSN that is less than 9 digits long\x3c/li>\n<li>checking if a given number passes the eleven test\x3c/li>\n<li>returning a list of BSNs generated during the current test run\x3c/li>\n<li>specifying BSNs that should not be generated\x3c/li>\n\x3c/ul>\n<p>Possible use cases:\x3c/p>\n<ul>\n<li>A test message that is processed by one or more systems can be tracked by its unique BSN\x3c/li>\n<li>Creating messages with BSNs in a certain range that leads to a certain response from a system or stub\x3c/li>\n<li>Checking whether a test message contains a valid BSN\x3c/li>\n\x3c/ul>\n<h3 id=\"Backward compatibility\">Backward compatibility\x3c/h3>\n<p>BSNLibrary v1.0.0 and later is not compatible with previous versions in the sense that is does not allow you to validate a BSN with <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a>. You should use <a href=\"#Validate%20BSN\" class=\"name\">Validate BSN\x3c/a> instead. If your test suite still uses <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> for validation it will generate an error saying that the length of <code>given\x3c/code> exceeds the maximum value. In case you have test suites using <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> for validation you can install BSNLibrary v0.4.0 for a smooth transition:\x3c/p>\n<p><code>pip install robotframework-bsnlibrary==0.4.0\x3c/code>\x3c/p>\n<p>Your test suite will still run, but you will receive a warning of any deprecated use of <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> and a recommendation to replace it with the keyword <a href=\"#Validate%20BSN\" class=\"name\">Validate BSN\x3c/a>. This allows you to convert your test suites at your own pace.\x3c/p>\n<h3 id=\"Installation\">Installation\x3c/h3>\n<p><code>pip install robotframework-bsnlibrary\x3c/code>\x3c/p>\n<p>Apart from the library files, the following files are installed\x3c/p>\n<table border=\"1\">\n<tr>\n<td><b>File\x3c/b>\x3c/td>\n<td><b>Description\x3c/b>\x3c/td>\n\x3c/tr>\n<tr>\n<td>&lt;python dir&gt;/Lib/site-packages/BSNLibrary/docs/index.html\x3c/td>\n<td>Local copy of this keyword documentation\x3c/td>\n\x3c/tr>\n<tr>\n<td>&lt;python dir&gt;/Lib/site-packages/BSNLibrary/tests/BSNLibrary_test/\x3c/td>\n<td>Robot Framework (v3.1 or later) test suite for testing BSNLibrary\x3c/td>\n\x3c/tr>\n<tr>\n<td>&lt;python dir&gt;/Lib/site-packages/BSNLibrary/tests/BSNLibrary_test_old_syntax/\x3c/td>\n<td>Robot Framework (v3.1 or earlier) the same test suite for testing BSNLibrary with the old <code>:FOR\x3c/code> loop syntax\x3c/td>\n\x3c/tr>\n\x3c/table>\n<h3 id=\"General information\">General information\x3c/h3>\n<p><a href=\"https://pypi.org/project/robotframework-bsnlibrary/\">Installation package on PyPI\x3c/a>\x3c/p>\n<p><a href=\"https://github.com/HaaiHenkie/bsnlibrary\">GitHub repository\x3c/a>\x3c/p>\n<p><a href=\"https://github.com/HaaiHenkie/bsnlibrary/releases\">Release notes\x3c/a>\x3c/p>\n<p>Create date: 01-03-2020\x3c/p>\n<p>Author: Henk van den Akker\x3c/p>\n<p>License: GNU General Public License v3.0\x3c/p>\n<h2 id=\"Scope of uniqueness and exclusion\">Scope of uniqueness and exclusion\x3c/h2>\n<p><a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> will by default generate a unique BSN every time it is used throughout the test run. After using <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs\x3c/a> with a list of BSNs, <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> will exclude those BSNs every time it is used until the end of the test run. These are the normal scopes for uniqueness and exclusion and they are suitable for most purposes. The following information is relevant for the few cases that need a smaller or larger scope.\x3c/p>\n<h3 id=\"Reducing the scope\">Reducing the scope\x3c/h3>\n<p>Uniqueness is established by a list of generated BSNs. Every time <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> is used it will exclude the BSNs on this list and add the generated BSN to this list. The scope of uniqueness and exclusion can be ended by clearing the list of generated BSNs and the list of excluded BSNs respectively. So to limit, for example, the scope of uniqueness to a suite, use <a href=\"#Clear%20Generated%20BSNs\" class=\"name\">Clear Generated BSNs\x3c/a> in the teardown of the suite and of the previous suite. Suppose you need each test to have its own set of excluded BSNs, use <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs\x3c/a> in de setup of each test and <a href=\"#Clear%20Excluded%20BSNs\" class=\"name\">Clear Excluded BSNs\x3c/a> in the teardown of each test.\x3c/p>\n<h3 id=\"Extending the scope\">Extending the scope\x3c/h3>\n<p>It is possible to extend the scope of uniqueness of BSNs over test runs with <a href=\"#Get%20Generated%20BSNs\" class=\"name\">Get Generated BSNs\x3c/a> and <a href=\"#Get%20Excluded%20BSNs\" class=\"name\">Get Excluded BSNs\x3c/a> at the end of the test run and appending this list to a file. Then at the start of a test run read the list from the file and offer it as input to <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs\x3c/a>. However, you cannot do this infinitely, because after a certain amount of repetitions the list of excluded BSNs will be so large that it will lead to performance or other problems. The BSNLibary_test suite, see <a href=\"#Installation\" class=\"name\">Installation\x3c/a>, contains example 'Extending the scope of uniqueness beyond one test run' under '3 Demos'.\x3c/p>\n<h2 id=\"Troubleshooting\">Troubleshooting\x3c/h2>\n<p>Most exceptions are self-explanatory. The BSNLibary_test suite, see <a href=\"#Installation\" class=\"name\">Installation\x3c/a>, demonstrates how  BSNLibrary exceptions can be reproduced.\x3c/p>\n<p>The following exception (with example counts and arguments) needs more explanation:\x3c/p>\n<pre>\n'Generate BSN' was not able to generate a unique BSN after 1000 retries. You have generated 900 out of the 900 or\n901 unique BSNs that are permitted by 9 excluded BSNs and arguments given=12345 and length=9.\n\x3c/pre>\n<p>This means that all or more than 99% of all possible BSNs within the given restrictions have been generated. For further insight you could use <a href=\"#Get%20Generated%20BSNs\" class=\"name\">Get Generated BSNs\x3c/a> and <a href=\"#Get%20Excluded%20BSNs\" class=\"name\">Get Excluded BSNs\x3c/a> to log those lists just before this exception occurs. The exception only counts generated and excluded BSNs that could have been generated with the current arguments.\x3c/p>\n<p>Possible solutions are:\x3c/p>\n<ul>\n<li>Use <code>unique=False\x3c/code> if you do not need unique BSNs\x3c/li>\n<li>Use a smaller scope for uniqueness and exclusion, see <a href=\"#Reducing%20the%20scope\" class=\"name\">Reducing the scope\x3c/a>\x3c/li>\n<li>Limit the length of <code>given\x3c/code> and/or avoid using the same value for <code>given\x3c/code> repeatedly\x3c/li>\n<li>Reduce the list of excluded BSNs\x3c/li>\n\x3c/ul>\n<p><a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> generates numbers randomly and is not suitable for generating all possible numbers in a range of 10000 or more number. If you want to find all BSNs in a range, divide the range in smaller ranges of 100 numbers and loop through those ranges. The BSNLibary_test suite, see <a href=\"#Installation\" class=\"name\">Installation\x3c/a>, contains example 'Finding all BSNs in a range' under '3 Demos'.\x3c/p>\n<p>There is a similar second exception (again with example counts and arguments)\x3c/p>\n<pre>\n'Generate BSN' was not able to generate a BSN outside the list of excluded BSNs after 1000 retries. You have\nexcluded 909 out of the 909 or 910 BSNs that are permitted by arguments given=12345 and length=9.\n\x3c/pre>\n<p>In this case only the last two possible solutions apply. Unless your were intentionally trying to do the impossible, I would like you <a href=\"https://github.com/HaaiHenkie/bsnlibrary/issues/new\">to log\x3c/a> how you ended up with this last exception, so that I have anecdotal evidence that I did not include this exception for nothing.\x3c/p>\n<p>If you experience slow performance this is probably caused by a large number of both generated BSNs and excluded BSNs that have used a large percentage of all BSNs that are permitted by current arguments. The possible solutions are the same as for the exceptions above.\x3c/p>\n<p>When you are not able to resolve a problem regarding BSNLibrary, <a href=\"https://github.com/HaaiHenkie/bsnlibrary/issues/new\">register an issue\x3c/a>.\x3c/p>","generated":"2020-04-26 16:58:28","inits":[],"keywords":[{"args":[],"doc":"<p>Clears list of excluded BSNs and ends the scope of <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs\x3c/a>. See also <a href=\"#Scope%20of%20uniqueness%20and%20exclusion\" class=\"name\">Scope of uniqueness and exclusion\x3c/a>.\x3c/p>\n<p>Example:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>${bsnlist} =\x3c/td>\n<td>Create List\x3c/td>\n<td>469641459\x3c/td>\n<td>376670149\x3c/td>\n<td>671472847\x3c/td>\n\x3c/tr>\n<tr>\n<td>Exclude BSNs\x3c/td>\n<td>${bsnlist}\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>${excluded_bsns} =\x3c/td>\n<td>Get Excluded BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>Clear Excluded BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>${excluded_bsns} =\x3c/td>\n<td>Get Excluded BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\nINFO : ${bsnlist} = ['469641459', '376670149', '671472847']\nINFO : ${excluded_bsns} = ['469641459', '376670149', '671472847']\nINFO : The list of excluded BSNs has been cleared.\nINFO : ${excluded_bsns} = []\n\x3c/pre>","matched":true,"name":"Clear Excluded BSNs","shortdoc":"Clears list of excluded BSNs and ends the scope of `Exclude BSNs`. See also `Scope of uniqueness and exclusion`.","tags":[]},{"args":[],"doc":"<p>Clears the list of BSNs generated by <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> with argument <code>unique=True\x3c/code>. See in <a href=\"#Scope%20of%20uniqueness%20and%20exclusion\" class=\"name\">Scope of uniqueness and exclusion\x3c/a> how this can be used to reduce the scope of uniqueness.\x3c/p>\n<p>Example:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>FOR\x3c/td>\n<td>${i}\x3c/td>\n<td>IN RANGE\x3c/td>\n<td>3\x3c/td>\n\x3c/tr>\n<tr>\n<td>\x3c/td>\n<td>Generate BSN\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>END\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>${generated_bsns} =\x3c/td>\n<td>Get Generated BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>Clear Generated BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>${generated_bsns} =\x3c/td>\n<td>Get Generated BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\nINFO : ${generated_bsns} = ['514169138', '287516635', '715755407']\nINFO : List of 3 generated BSNs has been cleared.\nINFO : ${generated_bsns} = []\n\x3c/pre>","matched":true,"name":"Clear Generated BSNs","shortdoc":"Clears the list of BSNs generated by `Generate BSN` with argument ``unique=True``. See in `Scope of uniqueness and exclusion` how this can be used to reduce the scope of uniqueness.","tags":[]},{"args":["bsnlist"],"doc":"<p>Excludes BSNs from being generated from the moment it is used until the end of the test run or until <a href=\"#Clear%20Excluded%20BSNs\" class=\"name\">Clear Excluded BSNs\x3c/a> is used. It will combine <code>bsnlist\x3c/code> with previously excluded BSNs. If you need <code>bsnlist\x3c/code> to replace previously excluded BSNs, use <a href=\"#Clear%20Excluded%20BSNs\" class=\"name\">Clear Excluded BSNs\x3c/a> first.\x3c/p>\n<p><code>bsnlist\x3c/code> is a single BSN or a list of BSNs to be excluded\x3c/p>\n<p>Example:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>${bsnlist} =\x3c/td>\n<td>Create List\x3c/td>\n<td>267227607\x3c/td>\n<td>307684945\x3c/td>\n<td>643897100\x3c/td>\n\x3c/tr>\n<tr>\n<td>Exclude BSNs\x3c/td>\n<td>${bsnlist}\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>Exclude BSNs\x3c/td>\n<td>501840151\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>${excluded_bsns} =\x3c/td>\n<td>Get Excluded BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\nINFO : ${bsnlist} = ['267227607', '307684945', '643897100']\nINFO : ${excluded_bsns} = ['501840151', '307684945', '267227607', '643897100']\n\x3c/pre>","matched":true,"name":"Exclude BSNs","shortdoc":"Excludes BSNs from being generated from the moment it is used until the end of the test run or until `Clear Excluded BSNs` is used. It will combine ``bsnlist`` with previously excluded BSNs. If you need ``bsnlist`` to replace previously excluded BSNs, use `Clear Excluded BSNs` first.","tags":[]},{"args":["given=","length=9","unique=True"],"doc":"<p>Generates a number between 100000000 and 799999999 that passes the eleven test. By default this BSN is unique within a test run and is added to a list that can be accessed with <a href=\"#Get%20Generated%20BSNs\" class=\"name\">Get Generated BSNs\x3c/a>. It will not generate numbers specified with <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs\x3c/a>. As of BSNLibrary version 1.0.0 it is not possible to use this keyword for validation of BSNs anymore. Use <a href=\"#Validate%20BSN\" class=\"name\">Validate BSN\x3c/a> instead.\x3c/p>\n<p><code>given\x3c/code> argument can be used to specify the first digits of the number to be generated, thus restricting the range within which the number is generated.\x3c/p>\n<ul>\n<li>To generate a number outside the default range, specify 0, 8 or 9 as the first digit\x3c/li>\n<li>To generate an invalid number, specify '999' as the first three digits\x3c/li>\n<li>The <code>given\x3c/code> string can only contain digits\x3c/li>\n<li>The maximum number of digits is <code>length - 2\x3c/code>\x3c/li>\n\x3c/ul>\n<p><code>length\x3c/code> argument can be used to generate a number of less than 9 positions, for example to test a situation where it is permitted to leave out leading zeroes or a situation where this is not permitted.\x3c/p>\n<ul>\n<li>Only values 6, 7, 8 or 9 are allowed\x3c/li>\n\x3c/ul>\n<p>If <code>unique\x3c/code> is given a <code>False\x3c/code> value the keyword no longer enforces that the generated BSN is unique within a test run, nor will it add the generated number to the list of generated BSNs. Can be used in situations that uniqueness is not a requirement and enforcing it leads to problems.\x3c/p>\n<p>Examples:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>${bsn1} =\x3c/td>\n<td>Generate BSN\x3c/td>\n<td>\x3c/td>\n<td># Generates a valid BSN between 100000000 and 799999999.\x3c/td>\n\x3c/tr>\n<tr>\n<td>Validate BSN\x3c/td>\n<td>${bsn1}\x3c/td>\n<td>\x3c/td>\n<td># Validates the generated valid BSN.\x3c/td>\n\x3c/tr>\n<tr>\n<td>${bsn2} =\x3c/td>\n<td>Generate BSN\x3c/td>\n<td>85\x3c/td>\n<td># Generates a valid BSN with '85' as the first 2 digits.\x3c/td>\n\x3c/tr>\n<tr>\n<td>${bsn3} =\x3c/td>\n<td>Generate BSN\x3c/td>\n<td>9994\x3c/td>\n<td># Generates an invalid BSN.\x3c/td>\n\x3c/tr>\n<tr>\n<td>Validate BSN\x3c/td>\n<td>${bsn3}\x3c/td>\n<td>\x3c/td>\n<td># Validates the generated invalid BSN.\x3c/td>\n\x3c/tr>\n<tr>\n<td>${bsn4} =\x3c/td>\n<td>Generate BSN\x3c/td>\n<td>length=8\x3c/td>\n<td># Generates a BSN with 8 positions.\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\n${bsn1} = 771052066\nINFO : The BSN '771052066' is valid.\n${bsn2} = 853380107\n${bsn3} = 999450437\nFAIL : The given number '999450437' is not a valid BSN.\n${bsn4} = 30340731\n\x3c/pre>","matched":true,"name":"Generate BSN","shortdoc":"Generates a number between 100000000 and 799999999 that passes the eleven test. By default this BSN is unique within a test run and is added to a list that can be accessed with `Get Generated BSNs`. It will not generate numbers specified with `Exclude BSNs`. As of BSNLibrary version 1.0.0 it is not possible to use this keyword for validation of BSNs anymore. Use `Validate BSN` instead.","tags":[]},{"args":[],"doc":"<p>Gets the list of excluded BSNs to inspect it for troubleshooting purposes.\x3c/p>\n<p>Example:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>${bsnlist} =\x3c/td>\n<td>Create List\x3c/td>\n<td>423932020\x3c/td>\n<td>107004422\x3c/td>\n<td>233354773\x3c/td>\n\x3c/tr>\n<tr>\n<td>Exclude BSNs\x3c/td>\n<td>${bsnlist}\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>${excluded_bsns} =\x3c/td>\n<td>Get Excluded BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\nINFO : ${bsnlist} = ['423932020', '107004422', '233354773']\nINFO : ${excluded_bsns} = ['423932020', '107004422', '233354773']\n\x3c/pre>","matched":true,"name":"Get Excluded BSNs","shortdoc":"Gets the list of excluded BSNs to inspect it for troubleshooting purposes.","tags":[]},{"args":[],"doc":"<p>Returns a list of unique BSNs that are generated with <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN\x3c/a> within the current test run. It can be used to create such a list or to inspect the current list for troubleshooting purposes.\x3c/p>\n<p>Example:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>Clear Generated BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td># Clears BSNs generated so far\x3c/td>\n\x3c/tr>\n<tr>\n<td>FOR\x3c/td>\n<td>${i}\x3c/td>\n<td>IN RANGE\x3c/td>\n<td>3\x3c/td>\n<td>\x3c/td>\n\x3c/tr>\n<tr>\n<td>\x3c/td>\n<td>Generate BSN\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td># Do not use <code>unique=False\x3c/code>\x3c/td>\n\x3c/tr>\n<tr>\n<td>END\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td># for no list will be generated\x3c/td>\n\x3c/tr>\n<tr>\n<td>${generated_bsns} =\x3c/td>\n<td>Get Generated BSNs\x3c/td>\n<td>\x3c/td>\n<td>\x3c/td>\n<td># A list of 3 unique BSNs\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\nINFO : List of 0 generated BSNs has been cleared.\nINFO : ${generated_bsns} = ['143828654', '123095141', '189392307']\n\x3c/pre>","matched":true,"name":"Get Generated BSNs","shortdoc":"Returns a list of unique BSNs that are generated with `Generate BSN` within the current test run. It can be used to create such a list or to inspect the current list for troubleshooting purposes.","tags":[]},{"args":["bsn"],"doc":"<p>Validates the given BSN, i.e. checks if it passes the eleven test.\x3c/p>\n<p><code>bsn\x3c/code> argument is a string of 6, 7, 8 or 9 digits\x3c/p>\n<p>Examples:\x3c/p>\n<table border=\"1\">\n<tr>\n<td>Validate BSN\x3c/td>\n<td>627708195\x3c/td>\n<td># Validation of a valid BSN.\x3c/td>\n\x3c/tr>\n<tr>\n<td>Validate BSN\x3c/td>\n<td>566709883\x3c/td>\n<td># Validation of an invalid BSN.\x3c/td>\n\x3c/tr>\n\x3c/table>\n<p>=&gt;\x3c/p>\n<pre>\nINFO : The BSN '627708195' is valid.\nFAIL : The given number '566709883' is not a valid BSN.\n\x3c/pre>","matched":true,"name":"Validate BSN","shortdoc":"Validates the given BSN, i.e. checks if it passes the eleven test.","tags":[]}],"name":"BSNLibrary","named_args":true,"scope":"global","version":"1.0.0"};
+<script type="text/javascript">
+libdoc = {"specversion": 1, "name": "BSNLibrary", "doc": "<p>Robot Framework Library for generating a random BSN (Burger Service Nummer, i.e. a Dutch citizen service number) for test purposes.</p>\n<p>A BSN is used in Netherlands to identify a person for government organisations, see <a href=\"https://www.government.nl/topics/personal-data/citizen-service-number-bsn\">this information of the Dutch government</a>. The number consists of 9 digits and has to pass the eleven test.</p>\n<p>This test can be explained with the example 211551557. Each digit is multiplied with its position and the results are added up together:</p>\n<p><code>(9*2) + (8*1) + (7*1) + (6*5) + (5*5) + (4*1) + (3*5) + (2*5) - (1*7) = 110</code></p>\n<p>Note that the digit in position 1 is subtracted from the other results. The total sum can be divided by 11, which means that this number has passed the eleven test.</p>\n<p>This library generates BSNs for test purposes in the sense that it generates random 9 digit numbers that pass the eleven test. By coincidence a generated number could be a real person's BSN. Yet this library cannot violate such a person's privacy, because it cannot tell you whether a number belongs to a real person or not, nor will it provide you with any personal data related to a BSN. Obviously you should only use this library in test environments.</p>\n<p>This library brings the following features to Robot Framework:</p>\n<ul>\n<li>generating a valid BSN</li>\n<li>generating a BSN that is unique within the current test run</li>\n<li>generating a number that will not pass the eleven test</li>\n<li>generating a BSN that starts with specific digits</li>\n<li>generating a BSN that is less than 9 digits long</li>\n<li>checking if a given number passes the eleven test</li>\n<li>returning a list of BSNs generated during the current test run</li>\n<li>specifying BSNs that should not be generated</li>\n</ul>\n<p>Possible use cases:</p>\n<ul>\n<li>A test message that is processed by one or more systems can be tracked by its unique BSN</li>\n<li>Creating messages with BSNs in a certain range that leads to a certain response from a system or stub</li>\n<li>Checking whether a test message contains a valid BSN</li>\n</ul>\n<h3 id=\"Backward compatibility\">Backward compatibility</h3>\n<p>BSNLibrary v1.0.0 and later is not compatible with previous versions in the sense that is does not allow you to validate a BSN with <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a>. You should use <a href=\"#Validate%20BSN\" class=\"name\">Validate BSN</a> instead. If your test suite still uses <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> for validation it will generate an error saying that the length of <code>given</code> exceeds the maximum value. In case you have test suites using <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> for validation you can install BSNLibrary v0.4.0 for a smooth transition:</p>\n<p><code>pip install robotframework-bsnlibrary==0.4.0</code></p>\n<p>Your test suite will still run, but you will receive a warning of any deprecated use of <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> and a recommendation to replace it with the keyword <a href=\"#Validate%20BSN\" class=\"name\">Validate BSN</a>. This allows you to convert your test suites at your own pace.</p>\n<h3 id=\"Installation\">Installation</h3>\n<p><code>pip install robotframework-bsnlibrary</code></p>\n<p>Apart from the library files, the following files are installed</p>\n<table border=\"1\">\n<tr>\n<td><b>File</b></td>\n<td><b>Description</b></td>\n</tr>\n<tr>\n<td>&lt;python dir&gt;/Lib/site-packages/BSNLibrary/docs/index.html</td>\n<td>Local copy of this keyword documentation</td>\n</tr>\n<tr>\n<td>&lt;python dir&gt;/Lib/site-packages/BSNLibrary/tests/BSNLibrary_test/</td>\n<td>Robot Framework (v3.1 or later) test suite for testing BSNLibrary</td>\n</tr>\n<tr>\n<td>&lt;python dir&gt;/Lib/site-packages/BSNLibrary/tests/BSNLibrary_test_old_syntax/</td>\n<td>Robot Framework (v3.1 or earlier) the same test suite for testing BSNLibrary with the old <code>:FOR</code> loop syntax</td>\n</tr>\n</table>\n<h3 id=\"General information\">General information</h3>\n<p><a href=\"https://pypi.org/project/robotframework-bsnlibrary/\">Installation package on PyPI</a></p>\n<p><a href=\"https://github.com/HaaiHenkie/bsnlibrary\">GitHub repository</a></p>\n<p><a href=\"https://github.com/HaaiHenkie/bsnlibrary/releases\">Release notes</a></p>\n<p>Create date: 01-03-2020</p>\n<p>Author: Henk van den Akker</p>\n<p>License: MIT License (Expat)</p>\n<h2 id=\"Scope of uniqueness and exclusion\">Scope of uniqueness and exclusion</h2>\n<p><a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> will by default generate a unique BSN every time it is used throughout the test run. After using <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs</a> with a list of BSNs, <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> will exclude those BSNs every time it is used until the end of the test run. These are the normal scopes for uniqueness and exclusion and they are suitable for most purposes. The following information is relevant for the few cases that need a smaller or larger scope.</p>\n<h3 id=\"Reducing the scope\">Reducing the scope</h3>\n<p>Uniqueness is established by a list of generated BSNs. Every time <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> is used it will exclude the BSNs on this list and add the generated BSN to this list. The scope of uniqueness and exclusion can be ended by clearing the list of generated BSNs and the list of excluded BSNs respectively. So to limit, for example, the scope of uniqueness to a suite, use <a href=\"#Clear%20Generated%20BSNs\" class=\"name\">Clear Generated BSNs</a> in the teardown of the suite and of the previous suite. Suppose you need each test to have its own set of excluded BSNs, use <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs</a> in de setup of each test and <a href=\"#Clear%20Excluded%20BSNs\" class=\"name\">Clear Excluded BSNs</a> in the teardown of each test.</p>\n<h3 id=\"Extending the scope\">Extending the scope</h3>\n<p>It is possible to extend the scope of uniqueness of BSNs over test runs with <a href=\"#Get%20Generated%20BSNs\" class=\"name\">Get Generated BSNs</a> and <a href=\"#Get%20Excluded%20BSNs\" class=\"name\">Get Excluded BSNs</a> at the end of the test run and appending this list to a file. Then at the start of a test run read the list from the file and offer it as input to <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs</a>. However, you cannot do this infinitely, because after a certain amount of repetitions the list of excluded BSNs will be so large that it will lead to performance or other problems. The BSNLibary_test suite, see <a href=\"#Installation\" class=\"name\">Installation</a>, contains example 'Extending the scope of uniqueness beyond one test run' under '3 Demos'.</p>\n<h2 id=\"Troubleshooting\">Troubleshooting</h2>\n<p>Most exceptions are self-explanatory. The BSNLibary_test suite, see <a href=\"#Installation\" class=\"name\">Installation</a>, demonstrates how  BSNLibrary exceptions can be reproduced.</p>\n<p>The following exception (with example counts and arguments) needs more explanation:</p>\n<pre>\n'Generate BSN' was not able to generate a unique BSN after 1000 retries. You have generated 900 out of the 900 or\n901 unique BSNs that are permitted by 9 excluded BSNs and arguments given=12345 and length=9.\n</pre>\n<p>This means that all or more than 99% of all possible BSNs within the given restrictions have been generated. For further insight you could use <a href=\"#Get%20Generated%20BSNs\" class=\"name\">Get Generated BSNs</a> and <a href=\"#Get%20Excluded%20BSNs\" class=\"name\">Get Excluded BSNs</a> to log those lists just before this exception occurs. The exception only counts generated and excluded BSNs that could have been generated with the current arguments.</p>\n<p>Possible solutions are:</p>\n<ul>\n<li>Use <code>unique=False</code> if you do not need unique BSNs</li>\n<li>Use a smaller scope for uniqueness and exclusion, see <a href=\"#Reducing%20the%20scope\" class=\"name\">Reducing the scope</a></li>\n<li>Limit the length of <code>given</code> and/or avoid using the same value for <code>given</code> repeatedly</li>\n<li>Reduce the list of excluded BSNs</li>\n</ul>\n<p><a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> generates numbers randomly and is not suitable for generating all possible numbers in a range of 10000 or more number. If you want to find all BSNs in a range, divide the range in smaller ranges of 100 numbers and loop through those ranges. The BSNLibary_test suite, see <a href=\"#Installation\" class=\"name\">Installation</a>, contains example 'Finding all BSNs in a range' under '3 Demos'.</p>\n<p>There is a similar second exception (again with example counts and arguments)</p>\n<pre>\n'Generate BSN' was not able to generate a BSN outside the list of excluded BSNs after 1000 retries. You have\nexcluded 909 out of the 909 or 910 BSNs that are permitted by arguments given=12345 and length=9.\n</pre>\n<p>In this case only the last two possible solutions apply. Unless your were intentionally trying to do the impossible, I would like you <a href=\"https://github.com/HaaiHenkie/bsnlibrary/issues/new\">to log</a> how you ended up with this last exception, so that I have anecdotal evidence that I did not include this exception for nothing.</p>\n<p>If you experience slow performance this is probably caused by a large number of both generated BSNs and excluded BSNs that have used a large percentage of all BSNs that are permitted by current arguments. The possible solutions are the same as for the exceptions above.</p>\n<p>When you are not able to resolve a problem regarding BSNLibrary, <a href=\"https://github.com/HaaiHenkie/bsnlibrary/issues/new\">register an issue</a>.</p>", "version": "1.1.0", "generated": "2023-05-25T19:50:01+00:00", "type": "LIBRARY", "scope": "GLOBAL", "docFormat": "HTML", "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 1, "tags": [], "inits": [], "keywords": [{"name": "Clear Excluded BSNs", "args": [], "doc": "<p>Clears list of excluded BSNs and ends the scope of <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs</a>. See also <a href=\"#Scope%20of%20uniqueness%20and%20exclusion\" class=\"name\">Scope of uniqueness and exclusion</a>.</p>\n<p>Example:</p>\n<table border=\"1\">\n<tr>\n<td>${bsnlist} =</td>\n<td>Create List</td>\n<td>469641459</td>\n<td>376670149</td>\n<td>671472847</td>\n</tr>\n<tr>\n<td>Exclude BSNs</td>\n<td>${bsnlist}</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>${excluded_bsns} =</td>\n<td>Get Excluded BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>Clear Excluded BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>${excluded_bsns} =</td>\n<td>Get Excluded BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\nINFO : ${bsnlist} = ['469641459', '376670149', '671472847']\nINFO : ${excluded_bsns} = ['469641459', '376670149', '671472847']\nINFO : The list of excluded BSNs has been cleared.\nINFO : ${excluded_bsns} = []\n</pre>", "shortdoc": "Clears list of excluded BSNs and ends the scope of `Exclude BSNs`. See also `Scope of uniqueness and exclusion`.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 410}, {"name": "Clear Generated BSNs", "args": [], "doc": "<p>Clears the list of BSNs generated by <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> with argument <code>unique=True</code>. See in <a href=\"#Scope%20of%20uniqueness%20and%20exclusion\" class=\"name\">Scope of uniqueness and exclusion</a> how this can be used to reduce the scope of uniqueness.</p>\n<p>Example:</p>\n<table border=\"1\">\n<tr>\n<td>FOR</td>\n<td>${i}</td>\n<td>IN RANGE</td>\n<td>3</td>\n</tr>\n<tr>\n<td></td>\n<td>Generate BSN</td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>END</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>${generated_bsns} =</td>\n<td>Get Generated BSNs</td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>Clear Generated BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>${generated_bsns} =</td>\n<td>Get Generated BSNs</td>\n<td></td>\n<td></td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\nINFO : ${generated_bsns} = ['514169138', '287516635', '715755407']\nINFO : List of 3 generated BSNs has been cleared.\nINFO : ${generated_bsns} = []\n</pre>", "shortdoc": "Clears the list of BSNs generated by `Generate BSN` with argument ``unique=True``. See in `Scope of uniqueness and exclusion` how this can be used to reduce the scope of uniqueness.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 361}, {"name": "Exclude BSNs", "args": [{"name": "bsnlist", "types": [], "typedocs": {}, "defaultValue": null, "kind": "POSITIONAL_OR_NAMED", "required": true, "repr": "bsnlist"}], "doc": "<p>Excludes BSNs from being generated from the moment it is used until the end of the test run or until <a href=\"#Clear%20Excluded%20BSNs\" class=\"name\">Clear Excluded BSNs</a> is used. It will combine <code>bsnlist</code> with previously excluded BSNs. If you need <code>bsnlist</code> to replace previously excluded BSNs, use <a href=\"#Clear%20Excluded%20BSNs\" class=\"name\">Clear Excluded BSNs</a> first.</p>\n<p><code>bsnlist</code> is a single BSN or a list of BSNs to be excluded</p>\n<p>Example:</p>\n<table border=\"1\">\n<tr>\n<td>${bsnlist} =</td>\n<td>Create List</td>\n<td>267227607</td>\n<td>307684945</td>\n<td>643897100</td>\n</tr>\n<tr>\n<td>Exclude BSNs</td>\n<td>${bsnlist}</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>Exclude BSNs</td>\n<td>501840151</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>${excluded_bsns} =</td>\n<td>Get Excluded BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\nINFO : ${bsnlist} = ['267227607', '307684945', '643897100']\nINFO : ${excluded_bsns} = ['501840151', '307684945', '267227607', '643897100']\n</pre>", "shortdoc": "Excludes BSNs from being generated from the moment it is used until the end of the test run or until `Clear Excluded BSNs` is used. It will combine ``bsnlist`` with previously excluded BSNs. If you need ``bsnlist`` to replace previously excluded BSNs, use `Clear Excluded BSNs` first.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 385}, {"name": "Generate BSN", "args": [{"name": "given", "types": [], "typedocs": {}, "defaultValue": "", "kind": "POSITIONAL_OR_NAMED", "required": false, "repr": "given="}, {"name": "length", "types": [], "typedocs": {}, "defaultValue": "9", "kind": "POSITIONAL_OR_NAMED", "required": false, "repr": "length=9"}, {"name": "unique", "types": [], "typedocs": {}, "defaultValue": "True", "kind": "POSITIONAL_OR_NAMED", "required": false, "repr": "unique=True"}], "doc": "<p>Generates a number between 100000000 and 799999999 that passes the eleven test. By default this BSN is unique within a test run and is added to a list that can be accessed with <a href=\"#Get%20Generated%20BSNs\" class=\"name\">Get Generated BSNs</a>. It will not generate numbers specified with <a href=\"#Exclude%20BSNs\" class=\"name\">Exclude BSNs</a>. As of BSNLibrary version 1.0.0 it is not possible to use this keyword for validation of BSNs anymore. Use <a href=\"#Validate%20BSN\" class=\"name\">Validate BSN</a> instead.</p>\n<p><code>given</code> argument can be used to specify the first digits of the number to be generated, thus restricting the range within which the number is generated.</p>\n<ul>\n<li>To generate a number outside the default range, specify 0, 8 or 9 as the first digit</li>\n<li>To generate an invalid number, specify '999' as the first three digits</li>\n<li>The <code>given</code> string can only contain digits</li>\n<li>The maximum number of digits is <code>length - 2</code></li>\n</ul>\n<p><code>length</code> argument can be used to generate a number of less than 9 positions, for example to test a situation where it is permitted to leave out leading zeroes or a situation where this is not permitted.</p>\n<ul>\n<li>Only values 6, 7, 8 or 9 are allowed</li>\n</ul>\n<p>If <code>unique</code> is given a <code>False</code> value the keyword no longer enforces that the generated BSN is unique within a test run, nor will it add the generated number to the list of generated BSNs. Can be used in situations that uniqueness is not a requirement and enforcing it leads to problems.</p>\n<p>Examples:</p>\n<table border=\"1\">\n<tr>\n<td>${bsn1} =</td>\n<td>Generate BSN</td>\n<td></td>\n<td># Generates a valid BSN between 100000000 and 799999999.</td>\n</tr>\n<tr>\n<td>Validate BSN</td>\n<td>${bsn1}</td>\n<td></td>\n<td># Validates the generated valid BSN.</td>\n</tr>\n<tr>\n<td>${bsn2} =</td>\n<td>Generate BSN</td>\n<td>85</td>\n<td># Generates a valid BSN with '85' as the first 2 digits.</td>\n</tr>\n<tr>\n<td>${bsn3} =</td>\n<td>Generate BSN</td>\n<td>9994</td>\n<td># Generates an invalid BSN.</td>\n</tr>\n<tr>\n<td>Validate BSN</td>\n<td>${bsn3}</td>\n<td></td>\n<td># Validates the generated invalid BSN.</td>\n</tr>\n<tr>\n<td>${bsn4} =</td>\n<td>Generate BSN</td>\n<td>length=8</td>\n<td># Generates a BSN with 8 positions.</td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\n${bsn1} = 771052066\nINFO : The BSN '771052066' is valid.\n${bsn2} = 853380107\n${bsn3} = 999450437\nFAIL : The given number '999450437' is not a valid BSN.\n${bsn4} = 30340731\n</pre>", "shortdoc": "Generates a number between 100000000 and 799999999 that passes the eleven test. By default this BSN is unique within a test run and is added to a list that can be accessed with `Get Generated BSNs`. It will not generate numbers specified with `Exclude BSNs`. As of BSNLibrary version 1.0.0 it is not possible to use this keyword for validation of BSNs anymore. Use `Validate BSN` instead.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 151}, {"name": "Get Excluded BSNs", "args": [], "doc": "<p>Gets the list of excluded BSNs to inspect it for troubleshooting purposes.</p>\n<p>Example:</p>\n<table border=\"1\">\n<tr>\n<td>${bsnlist} =</td>\n<td>Create List</td>\n<td>423932020</td>\n<td>107004422</td>\n<td>233354773</td>\n</tr>\n<tr>\n<td>Exclude BSNs</td>\n<td>${bsnlist}</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n<tr>\n<td>${excluded_bsns} =</td>\n<td>Get Excluded BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\nINFO : ${bsnlist} = ['423932020', '107004422', '233354773']\nINFO : ${excluded_bsns} = ['423932020', '107004422', '233354773']\n</pre>", "shortdoc": "Gets the list of excluded BSNs to inspect it for troubleshooting purposes.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 432}, {"name": "Get Generated BSNs", "args": [], "doc": "<p>Returns a list of unique BSNs that are generated with <a href=\"#Generate%20BSN\" class=\"name\">Generate BSN</a> within the current test run. It can be used to create such a list or to inspect the current list for troubleshooting purposes.</p>\n<p>Example:</p>\n<table border=\"1\">\n<tr>\n<td>Clear Generated BSNs</td>\n<td></td>\n<td></td>\n<td></td>\n<td># Clears BSNs generated so far</td>\n</tr>\n<tr>\n<td>FOR</td>\n<td>${i}</td>\n<td>IN RANGE</td>\n<td>3</td>\n<td></td>\n</tr>\n<tr>\n<td></td>\n<td>Generate BSN</td>\n<td></td>\n<td></td>\n<td># Do not use <code>unique=False</code></td>\n</tr>\n<tr>\n<td>END</td>\n<td></td>\n<td></td>\n<td></td>\n<td># for no list will be generated</td>\n</tr>\n<tr>\n<td>${generated_bsns} =</td>\n<td>Get Generated BSNs</td>\n<td></td>\n<td></td>\n<td># A list of 3 unique BSNs</td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\nINFO : List of 0 generated BSNs has been cleared.\nINFO : ${generated_bsns} = ['143828654', '123095141', '189392307']\n</pre>", "shortdoc": "Returns a list of unique BSNs that are generated with `Generate BSN` within the current test run. It can be used to create such a list or to inspect the current list for troubleshooting purposes.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 342}, {"name": "Validate BSN", "args": [{"name": "bsn", "types": [], "typedocs": {}, "defaultValue": null, "kind": "POSITIONAL_OR_NAMED", "required": true, "repr": "bsn"}], "doc": "<p>Validates the given BSN, i.e. checks if it passes the eleven test.</p>\n<p><code>bsn</code> argument is a string of 6, 7, 8 or 9 digits</p>\n<p>Examples:</p>\n<table border=\"1\">\n<tr>\n<td>Validate BSN</td>\n<td>627708195</td>\n<td># Validation of a valid BSN.</td>\n</tr>\n<tr>\n<td>Validate BSN</td>\n<td>566709883</td>\n<td># Validation of an invalid BSN.</td>\n</tr>\n</table>\n<p>=&gt;</p>\n<pre>\nINFO : The BSN '627708195' is valid.\nFAIL : The given number '566709883' is not a valid BSN.\n</pre>", "shortdoc": "Validates the given BSN, i.e. checks if it passes the eleven test.", "tags": [], "source": "C:\\Users\\akkerhen\\PycharmProjects\\robotframework-bsnlibrary\\BSNLibrary\\__init__.py", "lineno": 320}], "dataTypes": {"enums": [], "typedDicts": []}, "typedocs": []}
 </script>
-    <title></title>
+<title></title>
 </head>
 <body>
 
 <div id="javascript-disabled">
-    <h1>Opening library documentation failed</h1>
-    <ul>
-        <li>Verify that you have <b>JavaScript enabled</b> in your browser.</li>
-        <li>Make sure you are using a <b>modern enough browser</b>. If using Internet Explorer, version 8 or newer is required.</li>
-        <li>Check are there messages in your browser's <b>JavaScript error log</b>. Please report the problem if you suspect you have encountered a bug.</li>
-    </ul>
+  <h1>Opening library documentation failed</h1>
+  <ul>
+    <li>Verify that you have <b>JavaScript enabled</b> in your browser.</li>
+    <li>Make sure you are using a <b>modern enough browser</b>. If using Internet Explorer, version 11 is required.</li>
+    <li>Check are there messages in your browser's <b>JavaScript error log</b>. Please report the problem if you suspect you have encountered a bug.</li>
+  </ul>
 </div>
 
 <script type="text/javascript">
     // Not using jQuery here for speed and to support ancient browsers.
     document.getElementById('javascript-disabled').style.display = 'none';
+    window.addEventListener("hashchange", function() {
+      document.getElementsByClassName("hamburger-menu")[0].checked = false;
+    }, false);
+    window.addEventListener("hashchange", function() {
+        if (window.location.hash.indexOf('#type-') == 0) {
+            const hash = '#type-modal-' + decodeURI(window.location.hash.slice(6));
+            const typeDoc = document.querySelector(".data-types").querySelector(hash);
+            if (typeDoc) {
+              showModal(typeDoc);
+            }
+        }
+    }, false);
 </script>
 
 <script type="text/javascript">
+
     $(document).ready(function() {
         parseTemplates();
         document.title = libdoc.name;
+        storage.init('libdoc');
+        setTheme();
         renderTemplate('base', libdoc, $('body'));
         if (libdoc.inits.length) {
+            libdoc.typedocs.map(function(type) {
+                var index = type.usages.indexOf('__init__');
+                if (index != -1) type.usages[index] = 'Importing';
+            });
             renderTemplate('importing', libdoc);
         }
         renderTemplate('shortcuts', libdoc);
-        if (libdoc.contains_tags) {
-            renderTemplate('tags', libdoc);
-        }
+        renderTemplate('keyword-shortcuts', libdoc);
         renderTemplate('keywords', libdoc);
+        renderTemplate('data-types', libdoc);
         renderTemplate('footer', libdoc);
+        const params = util.parseQueryString(window.location.search.slice(1));
+        let selectedTag = "";
+        if ("tag" in params) {
+            selectedTag = params["tag"];
+            tagSearch(selectedTag, window.location.hash);
+        }
+        if (libdoc.tags.length) {
+          libdoc.selectedTag = selectedTag;
+          renderTemplate('tags-shortcuts', libdoc);
+        }
         scrollToHash();
-        $(document).bind('keydown', handleKeydown);
+        setTimeout(function() {
+          document.getElementById("keyword-statistics-header").innerText = '' + libdoc.keywords.length;
+          if (storage.get('keyword-wall') === 'open') {
+            openKeywordWall();
+          }
+      }, 0);
+        createModal();
     });
 
+    function setTheme(theme) {
+        document.documentElement.setAttribute('data-theme', theme || getTheme());
+    }
+
+    function getTheme() {
+        if (libdoc['theme']) {
+            return libdoc['theme'];
+        } else if (window.matchMedia('(prefers-color-scheme: dark)').matches) {
+            return 'dark';
+        } else {
+            return 'light;'
+        }
+    }
+
     function parseTemplates() {
         $('script[type="text/x-jquery-tmpl"]').map(function (idx, elem) {
             $.template(elem.id, elem.text);
         });
     }
 
     function renderTemplate(name, arguments, container) {
-        if (!container) {
-            container = $('#' + name + '-container');
-            container.empty();
-        }
-        if (!arguments.search) {
-            arguments.search = false;
-        }
-        $.tmpl(name + '-template', arguments).appendTo(container);
-    }
-
-    function handleKeydown(event) {
-        event = event || window.event;
-        var keyCode = event.keyCode || event.which;
-        if (keyCode === 27)  // esc
-            setTimeout(closeSearch, 0);
-        if (keyCode === 83 && $('#search').is(':hidden'))  // s
-            setTimeout(openSearch, 0);
+      if (!container) {
+          container = $('#' + name + '-container');
+          container.empty();
+      }
+      if (!arguments.search) {
+          arguments.search = false;
+      }
+      $.tmpl(name + '-template', arguments).appendTo(container);
     }
 
     function scrollToHash() {
         if (window.location.hash) {
             var hash = window.location.hash.substring(1).replace('+', ' ');
             window.location.hash = '';
             window.location.hash = hash;
         }
     }
 
-    function tagSearch(tag) {
-        var include = {tags: true, tagsExact: true};
-        markMatches(tag, include);
-        highlightMatches(tag, include);
-        $('#keywords-container').find('.kw-row').addClass('hide-unmatched');
-    }
-
-    function doSearch() {
-        var string = $('#search-string').val();
-        var include = getIncludesAndDisableIfOnlyOneLeft();
-        if (string) {
-            markMatches(string, include);
-            highlightMatches(string, include);
-            setMatchVisibility();
-        } else {
-            resetKeywords();
-        }
-    }
-
-    function getIncludesAndDisableIfOnlyOneLeft() {
-        var name = $('#include-name');
-        var args = $('#include-args');
-        var doc = $('#include-doc');
-        var tags = $('#include-tags');
-        var include = {name: name.prop('checked'),
-                       args: args.prop('checked'),
-                       doc: doc.prop('checked'),
-                       tags: !!tags.prop('checked')};
-        if ((!include.name) && (!include.args) && (!include.doc)) {
-            tags.prop('disabled', true);
-        } else if ((!include.name) && (!include.args) && (!include.tags)) {
-            doc.prop('disabled', true);
-        } else if ((!include.name) && (!include.doc) && (!include.tags)) {
-            args.prop('disabled', true);
-        } else if ((!include.args) && (!include.doc) && (!include.tags)) {
-            name.prop('disabled', true);
-        } else {
-            name.prop('disabled', false);
-            args.prop('disabled', false);
-            doc.prop('disabled', false);
-            tags.prop('disabled', false);
-        }
-        return include;
-    }
-
-    function markMatches(pattern, include) {
-        pattern = util.regexpEscape(pattern);
+    function tagSearch(tag, hash) {
+      document.getElementsByClassName('search-input')[0].value = '';
+      const include = {tags: true, tagsExact: true};
+      const url = window.location.pathname + "?tag=" + tag + (hash || "");
+      markMatches(tag, include);
+      highlightMatches(tag, include);
+      history.replaceState && history.replaceState(null, '', url);
+      document.getElementById('keyword-shortcuts-container').scrollTop = 0;
+    }
+
+    function clearTagSearch() {
+      document.getElementsByClassName('search-input')[0].value = '';
+      history.replaceState && history.replaceState(null, '', window.location.pathname);
+      resetKeywords();
+    }
+
+    function closeMenu() {
+      document.getElementById('hamburger-menu-input').checked = false;
+    }
+
+    function markMatches(pattern, include, givenSearchTime, callback) {
+       if (givenSearchTime && givenSearchTime !== searchTime) {
+         return;
+       }
+        let patternRegexp = util.regexpEscape(pattern);
         if (include.tagsExact) {
-            pattern = '^' + pattern + '$';
+            patternRegexp = '^' + patternRegexp + '$';
         }
-        var regexp = new RegExp(pattern, 'i');
-        var test = regexp.test.bind(regexp);
-        var result = {contains_tags: libdoc.contains_tags};
-        var matchCount = 0;
+        let regexp = new RegExp(patternRegexp, 'i');
+        let test = regexp.test.bind(regexp);
+        let result = {};
+        let keywordMatchCount = 0;
         result.keywords = util.map(libdoc.keywords, function (kw) {
             kw = $.extend({}, kw);
-            kw.matched = (include.name && test(kw.name) ||
-                          include.args && test(kw.args) ||
-                          include.doc && test($(kw.doc).text()) ||
-                          include.tags && util.any(util.map(kw.tags, test)));
-            if (kw.matched)
-                matchCount++;
-            return kw
+            kw.hidden =  !(include.name && test(kw.name)) &&
+                         !(include.args && test(kw.args)) &&
+                          !(include.doc && test($(kw.doc).text())) &&
+                          !(include.tags && util.any(util.map(kw.tags, test)));
+            if (!kw.hidden)
+                keywordMatchCount++;
+            return kw;
         });
-        renderTemplate('shortcuts', result);
+        renderTemplate('keyword-shortcuts', result);
         renderTemplate('keywords', result);
-        if (libdoc.contains_tags) {
-            renderTemplate('tags', libdoc);
+        if (libdoc.tags.length) {
+          libdoc.selectedTag = include.tagsExact ? pattern : "";
+          renderTemplate('tags-shortcuts', libdoc);
         }
-        var ending = matchCount != 1 ? 's.' : '.';
-        $('#match-count').show().text(matchCount + ' matched keyword' + ending);
-        $('#altogether-count').hide();
-        if (matchCount == 0)
+        document.getElementById("keyword-statistics-header").innerText = keywordMatchCount + ' / ' + result.keywords.length;
+        if (keywordMatchCount === 0)
             $('#keywords-container').find('table').empty();
+        if (callback) {
+          requestAnimationFrame(callback);
+        }
     }
 
-    function highlightMatches(string, include) {
-        var shortcuts = $('#shortcuts-container').find('.match');
-        var keywords = $('#keywords-container').find('.match');
+    function highlightMatches(string, include, givenSearchTime) {
+       if (givenSearchTime && givenSearchTime !== searchTime) {
+         return;
+       }
+        const shortcuts = $('#shortcuts-container').find('.match');
+        const keywords = $('#keywords-container').find('.match');
         if (include.name) {
             shortcuts.highlight(string);
             keywords.find('.kw').highlight(string);
         }
         if (include.args) {
             keywords.find('.args').highlight(string);
         }
         if (include.doc) {
             keywords.find('.doc').highlight(string);
         }
         if (include.tags) {
             var matches = keywords.find('.tags').find('a').add(
-                    $('#tags-container').find('a'));
+                    $('#tags-shortcuts-container').find('a'));
             if (include.tagsExact) {
                 matches = matches.filter(function (index, tag) {
-                    return $(tag).text().toUpperCase() == string.toUpperCase();
+                    return $(tag).text().toUpperCase() === string.toUpperCase();
                 });
             }
             matches.highlight(string);
         }
     }
 
-    function openSearch() {
-        $('#search').show();
-        $('#open-search').hide();
-        $('#search-string').focus().select();
-        $(document).scrollTop($("#Shortcuts").offset().top);
-    }
-
-    function closeSearch() {
-        $('#search').hide();
-        $('#open-search').show();
-    }
-
-    function resetSearch() {
-        $('#search-string').val('');
-        $('#include-name').prop('checked', true);
-        $('#include-args').prop('checked', true);
-        $('#include-doc').prop('checked', true);
-        $('#hide-unmatched').prop('checked', false);
-        resetKeywords();
+    function clearSearch() {
+      document.getElementsByClassName('search-input')[0].value = '';
+      const tagsSelect = document.getElementById('tags-shortcuts-container');
+      if (tagsSelect) {
+        tagsSelect.selectedIndex = 0;
+      }
+      resetKeywords();
+    }
+
+    let searchTime = 0;
+
+    function searching() {
+      searchTime = Date.now();
+      const value = document.getElementsByClassName('search-input')[0].value;
+      const include = {name: true,
+                       args: true,
+                       doc: true,
+                       tags: true};
+      if (value) {
+        requestAnimationFrame(function () {
+          markMatches(value, include, searchTime,
+                  function () {
+                    highlightMatches(value, include, searchTime);
+                    document.getElementById('keyword-shortcuts-container').scrollTop = 0;
+                  }
+          );
+        });
+      } else {
+          resetKeywords();
+      }
+    }
+
+    function toggleShortcuts() {
+      const shortcuts = document.getElementsByClassName("shortcuts")[0];
+      if (shortcuts.classList.contains("keyword-wall")) {
+        closeKeywordWall();
+      } else {
+        openKeywordWall();
+      }
+    }
+
+    function openKeywordWall() {
+      const shortcuts = document.getElementsByClassName("shortcuts")[0];
+      shortcuts.classList.add("keyword-wall");
+      storage.set("keyword-wall", 'open');
+      const button = document.getElementById("toggle-keyword-shortcuts")
+      button.innerText = '-';
+    }
+
+    function closeKeywordWall() {
+      const shortcuts = document.getElementsByClassName("shortcuts")[0];
+      shortcuts.classList.remove("keyword-wall");
+      storage.set("keyword-wall", 'close');
+      const button = document.getElementById("toggle-keyword-shortcuts")
+      button.innerText = '+';
     }
 
     function resetKeywords() {
-        renderTemplate('shortcuts', libdoc);
+        renderTemplate('keyword-shortcuts', libdoc);
         renderTemplate('keywords', libdoc);
-        if (libdoc.contains_tags) {
+        renderTemplate('data-types', libdoc);
+        if (libdoc.tags.length) {
             renderTemplate('tags', libdoc);
         }
-        $('#match-count').hide();
-        $('#altogether-count').show();
-    }
-
-    function setMatchVisibility() {
-        var kws = $('#keywords-container').find('.kw-row');
-        var hide = $('#hide-unmatched').prop('checked');
-        kws.toggleClass('hide-unmatched', hide);
+        document.getElementById("keyword-statistics-header").innerText = ''+libdoc.keywords.length;
+        if (libdoc.typedocs.length) {
+            document.getElementById("type-statistics-header").innerText = '' + libdoc.typedocs.length;
+        }
+        history.replaceState && history.replaceState(null, '', location.pathname);
+    }
+
+    function createModal() {
+        const modalBackground = document.createElement('div');
+        modalBackground.id = 'modal-background';
+        modalBackground.classList.add('modal-background');
+        modalBackground.addEventListener('click', ({ target }) => {
+            if (target.id === 'modal-background') hideModal()
+        })
+
+        const modalCloseButton = document.createElement('button');
+        modalCloseButton.innerHTML = `<svg xmlns="
+      http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="2em" height="2em" className="block" data-v-2754030d="" data-v-512b0344="">
+              <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12 19 6.41z"
+                    data-v-2754030d="" fill="var(--text-color)"></path></svg>`;
+        modalCloseButton.classList.add('modal-close-button');
+        const modalCloseButtonContainer = document.createElement('div');
+        modalCloseButtonContainer.classList.add('modal-close-button-container');
+        modalCloseButtonContainer.appendChild(modalCloseButton);
+        modalCloseButton.addEventListener('click', () => {
+            hideModal()
+        })
+        modalBackground.appendChild(modalCloseButtonContainer);
+        modalCloseButtonContainer.addEventListener('click', () => {
+            hideModal()
+        })
+
+        const modal = document.createElement('div');
+        modal.id = 'modal';
+        modal.classList.add('modal');
+        modal.addEventListener('click', ({ target }) => {
+            if (target.tagName.toUpperCase() === 'A') hideModal()
+        })
+
+
+        const modalContent = document.createElement('div');
+        modalContent.id = 'modal-content';
+        modalContent.classList.add('modal-content');
+        modal.appendChild(modalContent);
+
+        modalBackground.appendChild(modal);
+        document.body.appendChild(modalBackground);
+        document.addEventListener('keydown', ({ key }) => {
+            if (key === 'Escape') hideModal()
+        })
+    }
+    function showModal(content) {
+        const modalBackground = document.getElementById('modal-background');
+        const modal = document.getElementById('modal');
+        const modalContent = document.getElementById('modal-content');
+        modalBackground.classList.add('visible');
+        modal.classList.add('visible');
+        modalContent.appendChild(content.cloneNode(true));
+        document.body.style.overflow = 'hidden';
+    }
+    function hideModal() {
+        const modalBackground = document.getElementById('modal-background');
+        const modal = document.getElementById('modal');
+        const modalContent = document.getElementById('modal-content');
+
+        modalBackground.classList.remove('visible');
+        modal.classList.remove('visible');
+        document.body.style.overflow = 'auto';
+        if (window.location.hash.indexOf('#type-') == 0)
+            history.pushState("", document.title, window.location.pathname);
+        // modal is hidden with a fading transition, timeout prevents premature emptying of modal
+        setTimeout(() => {
+            modalContent.innerHTML = '';
+        }, 200);
     }
 
     // http://stackoverflow.com/a/18484799
     var delay = (function () {
         var timer = 0;
         return function(callback, ms) {
             clearTimeout(timer);
             timer = setTimeout(callback, ms);
         };
     })();
-
 </script>
 
 <script type="text/x-jquery-tmpl" id="base-template">
-    <h1>${name}</h1>
-    <table class="metadata">
-        {{if version}}<tr><th>Library version:</th><td>${version}</td></tr>{{/if}}
-        {{if scope}}<tr><th>Library scope:</th><td>${scope}</td></tr>{{/if}}
-        <tr><th>Named arguments:</th><td>{{if named_args}}supported{{else}}not supported{{/if}}</td></tr>
-    </table>
-    <div id="introduction-container">
-        <h2 id="Introduction">Introduction</h2>
-        <div class="doc">{{html doc}}</div>
+  <div class="base-container">
+    <input id="hamburger-menu-input" class="hamburger-menu" type="checkbox" />
+    <span class="hamburger-menu hamburger-menu-1"></span>
+    <span class="hamburger-menu hamburger-menu-2"></span>
+    <span class="hamburger-menu hamburger-menu-3"></span>
+    <div class="libdoc-overview"><div id="shortcuts-container"></div></div>
+    <div class="libdoc-details">
+      <table class="metadata">
+          {{if version}}<tr><th>Library version:</th><td>${version}</td></tr>{{/if}}
+          {{if scope}}<tr><th>Library scope:</th><td>${scope}</td></tr>{{/if}}
+      </table>
+      <div id="introduction-container">
+          <h2 id="Introduction">Introduction</h2>
+          <div class="doc">{{html doc}}</div>
+      </div>
+      <div id="importing-container"></div>
+      <div id="keywords-container"></div>
+      <div id="data-types-container"></div>
+      <div id="footer-container"></div>
     </div>
-    <div id="importing-container"></div>
-    <div id="shortcuts-container"></div>
-    <div id="tags-container"></div>
-    <div id="keywords-container"></div>
-    <div id="footer-container"></div>
-    <form id="search" action="javascript:void(0)">
-        <fieldset>
-            <legend id="search-title">Search keywords</legend>
-            <input type="text" id="search-string" onkeyup="delay(doSearch, 500)">
-            <fieldset>
-                <legend>Search from</legend>
-                <input type="checkbox" id="include-name" onclick="doSearch()" checked>
-                <label for="include-name">Name</label>
-                <input type="checkbox" id="include-args" onclick="doSearch()" checked>
-                <label for="include-args">Arguments</label>
-                <input type="checkbox" id="include-doc" onclick="doSearch()" checked>
-                <label for="include-doc">Documentation</label>
-                {{if libdoc.contains_tags}}
-                <input type="checkbox" id="include-tags" onclick="doSearch()" checked>
-                <label for="include-tags">Tags</label>
-                {{/if}}
-            </fieldset>
-            <input type="checkbox" id="hide-unmatched" onclick="setMatchVisibility()" checked>
-            <label for="hide-unmatched">Hide unmatched keywords</label>
-            <div id="search-buttons">
-                <input type="button" value="Reset" onclick="resetSearch()"
-                       title="Reset search">
-                <input type="button" value="Close" onclick="closeSearch()"
-                       title="Close search (shortcut: <Esc>)">
-            </div>
-        </fieldset>
-    </form>
-    <div id="open-search" onclick="openSearch()" title="Search keywords (shortcut: s)"></div>
+    <a class="libdoc-title" href="#library-documentation-top">
+          <h1>${name}</h1>
+          <svg
+   xmlns:dc="http://purl.org/dc/elements/1.1/"
+   xmlns:cc="http://creativecommons.org/ns#"
+   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
+   xmlns:svg="http://www.w3.org/2000/svg"
+   xmlns="http://www.w3.org/2000/svg"
+   viewBox="0 0 202.4325 202.34125"
+   height="42"
+   width="42"
+   xml:space="preserve"
+   version="1.1"><metadata
+     id="metadata8"><rdf:RDF><cc:Work
+         rdf:about=""><dc:format>image/svg+xml</dc:format><dc:type
+           rdf:resource="http://purl.org/dc/dcmitype/StillImage" /></cc:Work></rdf:RDF></metadata><defs
+     id="defs6"><clipPath
+       id="clipPath16"
+       clipPathUnits="userSpaceOnUse"><path
+         id="path18"
+         d="m 0,161.873 161.946,0 L 161.946,0 0,0 0,161.873 Z" /></clipPath></defs><g
+     transform="matrix(1.25,0,0,-1.25,0,202.34125)"
+     id="g10"><g
+       id="g12"><g
+         clip-path="url(#clipPath16)"
+         id="g14"><g
+           transform="translate(52.4477,88.1268)"
+           id="g20"><path
+             id="robot-svg-path"
+             d="m 0,0 c 0,7.6 6.179,13.779 13.77,13.779 7.6,0 13.779,-6.179 13.779,-13.779 0,-2.769 -2.238,-5.007 -4.998,-5.007 -2.761,0 -4.999,2.238 -4.999,5.007 0,2.078 -1.695,3.765 -3.782,3.765 C 11.693,3.765 9.997,2.078 9.997,0 9.997,-2.769 7.76,-5.007 4.999,-5.007 2.238,-5.007 0,-2.769 0,0 m 57.05,-23.153 c 0,-2.771 -2.237,-5.007 -4.998,-5.007 l -46.378,0 c -2.761,0 -4.999,2.236 -4.999,5.007 0,2.769 2.238,5.007 4.999,5.007 l 46.378,0 c 2.761,0 4.998,-2.238 4.998,-5.007 M 35.379,-2.805 c -1.545,2.291 -0.941,5.398 1.35,6.943 l 11.594,7.83 c 2.273,1.58 5.398,0.941 6.943,-1.332 1.545,-2.29 0.941,-5.398 -1.35,-6.943 l -11.594,-7.83 c -0.852,-0.586 -1.829,-0.87 -2.788,-0.87 -1.607,0 -3.187,0.781 -4.155,2.202 m 31.748,-30.786 c 0,-0.945 -0.376,-1.852 -1.045,-2.522 l -8.617,-8.617 c -0.669,-0.668 -1.576,-1.045 -2.523,-1.045 l -52.833,0 c -0.947,0 -1.854,0.377 -2.523,1.045 l -8.617,8.617 c -0.669,0.67 -1.045,1.577 -1.045,2.522 l 0,52.799 c 0,0.947 0.376,1.854 1.045,2.522 l 8.617,8.619 c 0.669,0.668 1.576,1.044 2.523,1.044 l 52.833,0 c 0.947,0 1.854,-0.376 2.523,-1.044 l 8.617,-8.619 c 0.669,-0.668 1.045,-1.575 1.045,-2.522 l 0,-52.799 z m 7.334,61.086 -11.25,11.25 c -1.705,1.705 -4.018,2.663 -6.428,2.663 l -56.523,0 c -2.412,0 -4.725,-0.959 -6.43,-2.665 L -17.412,27.494 c -1.704,-1.705 -2.661,-4.016 -2.661,-6.427 l 0,-56.515 c 0,-2.411 0.958,-4.725 2.663,-6.428 l 11.25,-11.25 c 1.705,-1.705 4.017,-2.662 6.428,-2.662 l 56.515,0 c 2.41,0 4.723,0.957 6.428,2.662 l 11.25,11.25 c 1.705,1.703 2.663,4.017 2.663,6.428 l 0,56.514 c 0,2.412 -0.958,4.724 -2.663,6.429" /></g></g></g></g></svg>
+    </a>
+  </div>
 </script>
 
 <script type="text/x-jquery-tmpl" id="importing-template">
     <h2 id="Importing">Importing</h2>
-    <table border="1" class="keywords">
-        <tr>
-            <th class="args">Arguments</th>
-            <th class="doc">Documentation</th>
-        </tr>
+    <div class="keywords">
         {{each inits}}
-        <tr class="kw-row">
-            <td class="args">
-            {{each args}}
-              <span>${$value}</span>{{if $index < args.length-1}}, {{/if}}
-            {{/each}}
-            </td>
-            <td class="doc">{{html $value.doc}}</td>
-        </tr>
+        <div class="kw-row">
+          <div class="kw-overview">
+          {{if args.length}}
+              <div class="args">
+                <h4>Arguments</h4>
+                <div class="arguments-list-container">
+                  <div class="arguments-list">
+                  {{each args}}
+                    {{tmpl($value) 'argument-template'}}
+                  {{/each}}
+                  </div>
+                </div>
+              </div>
+          {{/if}}
+          {{if $value.doc}}
+            <div class="kw-docs">
+              <h4>Documentation</h4>
+              <div class="kwdoc doc">{{html $value.doc}}</div>
+            </div>
+          {{/if}}
+        </div>
         {{/each}}
-    </table>
+    </div>
 </script>
 
 <script type="text/x-jquery-tmpl" id="shortcuts-template">
-    <h2 id="Shortcuts">Shortcuts</h2>
-    <div class='shortcuts'>
-        {{each keywords}}
-        <a href="#${encodeURIComponent($value.name)}"
-           class="{{if $value.matched === false}}no-{{/if}}match"
-           title="${$value.shortdoc}">${$value.name}</a>
-        {{if $index < keywords.length-1}} &middot; {{/if}}
-        {{/each}}
+    <div class="keywords-overview">
+      <div class="keyword-search-box">
+        <input placeholder="Search" type="text" class="search-input" onkeydown="delay(searching, 150)"/>
+        <button class="clear-search" onclick="clearSearch()">&#10005;</button>
+      </div>
+      {{if tags.length}}
+      <select id="tags-shortcuts-container" onchange="location = this.value;">
+      </select>
+      {{/if}}
+      <div class="keywords-overview-header-row">
+      <h4>Keywords (<span id="keyword-statistics-header"></span>)
+      </h4>
+      <button id="toggle-keyword-shortcuts" onclick="toggleShortcuts()">+</button>
+      </div>
+      <ul class="shortcuts" id="keyword-shortcuts-container">
+      </ul>
     </div>
 </script>
 
-<script type="text/x-jquery-tmpl" id="tags-template">
-    <h2 id="Tags">Tags</h2>
-    <div class='shortcuts'>
-        {{each all_tags}}
-        <a href="javascript:tagSearch('${$value}')"
-           title="Show tests with this tag">${$value}</a> &middot;
-        {{/each}}
-        <a href="javascript:resetKeywords()" class="normal-first-letter"
-           title="Show all tests">[Reset]</a>
-    </div>
+<script id="keyword-shortcuts-template" type="text/x-jquery-tmpl">
+    {{each keywords}}
+    {{if !$value.hidden}}
+    <li>
+    <a href="#${encodeURIComponent($value.name)}"
+       onclick="closeMenu()"
+       class="match"
+       title="${$value.shortdoc}">${$value.name}</a>
+    </li>
+    {{/if}}
+    {{/each}}
+    {{each keywords}}
+    {{if $value.hidden}}
+    <li>
+    <a href="#${encodeURIComponent($value.name)}"
+       onclick="closeMenu()"
+       class="no-match"
+       title="${$value.shortdoc}">${$value.name}</a>
+    </li>
+    {{/if}}
+    {{/each}}
+</script>
+
+
+<script id="tags-shortcuts-template" type="text/x-jquery-tmpl">
+  <option value="javascript:clearTagSearch()" {{if selectedTag === ""}}selected{{/if}}>- Show all tags -</option>
+  {{each tags}}
+    <option value="javascript:tagSearch('${$value}')" {{if selectedTag === $value}}selected{{/if}}>${$value}</a>
+    </option>
+  {{/each}}
 </script>
 
 <script type="text/x-jquery-tmpl" id="keywords-template">
     <h2 id="Keywords">Keywords</h2>
-    <table border="1" class="keywords">
-        <tr>
-            <th class="kw">Keyword</th>
-            <th class="args">Arguments</th>
-            {{if libdoc.contains_tags}}
-            <th class="tags">Tags</th>
-            {{/if}}
-            <th class="doc">Documentation</th>
-        </tr>
+    <div class="keywords">
         {{each keywords}}
+        {{if !$value.hidden}}
             {{tmpl($value) 'keyword-template'}}
+        {{/if}}
+        {{/each}}
+        {{each keywords}}
+        {{if $value.hidden}}
+            {{tmpl($value) 'keyword-template'}}
+        {{/if}}
         {{/each}}
-    </table>
+    </div>
 </script>
 
 <script type="text/x-jquery-tmpl" id="keyword-template">
-    <tr class="kw-row {{if matched === false}}no-{{/if}}match">
-        <td class="kw">
-            <a name="${name}" href="#${encodeURIComponent(name)}"
+    <div class="keyword-container {{if hidden}}no-{{/if}}match" id="${name}">
+       <div class="keyword-name">
+            <h2>
+            <a class="kw-name" href="#${encodeURIComponent(name)}"
                title="Link to this keyword">${name}</a>
-        </td>
-        <td class="args">
-            {{each args}}
-            <span>${$value}</span>{{if $index < args.length-1}}, {{/if}}
-            {{/each}}
-        </td>
-        {{if libdoc.contains_tags}}
-        <td class="tags">
-            {{each tags}}
-            <a href="javascript:tagSearch('${$value}')"
-               title="Show tests with this tag">${$value}</a>{{if $index < tags.length-1}}, {{/if}}
-            {{/each}}
-        </td>
-        {{/if}}
-        <td class="doc">{{html doc}}</td>
-    </tr>
+            </h2>
+       </div>
+       <div class="keyword-content">
+          <div class="kw-overview">
+            {{if args.length}}
+              <div class="args">
+                <h4>Arguments</h4>
+                <div class="arguments-list-container">
+                  <div class="arguments-list">
+                  {{each args}}
+                    {{tmpl($value) 'argument-template'}}
+                  {{/each}}
+                  </div>
+                </div>
+              </div>
+            {{/if}}
+            {{if libdoc.tags.length && tags.length}}
+              <div class="tags">
+                <h4>Tags</h4>
+                {{each tags}}
+                  <a href="javascript:tagSearch('${$value}')"
+                    title="Show keywords with this tag">${$value}</a>{{if $index < tags.length-1}},<br>{{/if}}
+                {{/each}}
+              </div>
+            {{/if}}
+          </div>
+          {{if doc}}
+            <div class="kw-docs">
+              <h4>Documentation</h4>
+              <div class="kwdoc doc">{{html doc}}</div>
+            </div>
+          {{/if}}
+       </div>
+    </div>
 </script>
 
+<script id="argument-template" type="text/x-jquery-tmpl">
+<span class="arg-name {{if required}}arg-required{{else}}arg-optional{{/if}}" title="Argument name">
+{{if kind === 'VAR_POSITIONAL'}}<span class="arg-kind" title="Variable number of arguments">*</span>{{/if}}
+{{if kind === 'VAR_NAMED'}}<span class="arg-kind" title="Variable number of named arguments">**</span>{{/if}}
+{{if kind === 'NAMED_ONLY'}}<span class="arg-kind" title="Named only argument">&#x1F3F7;</span>{{/if}}
+{{if kind === 'POSITIONAL_ONLY'}}<span class="arg-kind" title="Positional only argument">&#x27F6;</span>{{/if}}
+${name}
+</span>
+
+{{if defaultValue !== null}}
+  <div class="arg-default-container">
+    <span class="arg-default-eq">=</span>
+    <span class="arg-default-value" title="Default value that is used if no value is given">${defaultValue}</span>
+  </div>
+{{/if}}
+
+{{if types.length}}
+  <span class="arg-type">
+    {{each types}}
+      {{if $value in $data.typedocs}}
+          &lt;<a style="cursor: pointer;" class="type" title="Click to show type information" onclick="showModal(document.querySelector('#type-modal-${$data.typedocs[$value]}'))">${$value}</a>&gt;
+      {{else}}
+          &lt;<span class="type">${$value}</span>&gt;
+      {{/if}}
+      <span class="or"></span>
+    {{/each}}
+  </span>
+{{/if}}
+</script>
+
+
+<script id="data-types-template" type="text/x-jquery-tmpl">
+  {{if typedocs.length}}
+    <h2 id="Data types">Data types</h2>
+    <div class="data-types">
+      {{each typedocs}}
+        {{tmpl($value) 'data-type-template'}}
+      {{/each}}
+    </div>
+  {{/if}}
+</script>
+
+<script id="data-type-template" type="text/x-jquery-tmpl">
+    <div class="data-type-container {{if hidden}}no-{{/if}}match" id="type-modal-${name}">
+       <div class="data-type-name">
+            <h2>${name} (${type})</h2>
+       </div>
+       <div class="data-type-content">
+          {{if doc}}
+            <div class="dt-docs">
+              <h4>Documentation</h4>
+              <div class="dtdoc doc">{{html doc}}</div>
+            </div>
+          {{/if}}
+          {{if members}}
+            <div class="dt-members">
+              <h4>Allowed Values</h4>
+              <ul class="enum-type-members">
+                {{each members}}
+                <li>
+                  <span class="enum-member">${$value.name}</span>
+                  {{if accepts.indexOf("integer") != -1}}
+                    &nbsp; (<span class="enum-member">${$value.value}</span>)
+                  {{/if}}
+                </li>
+                {{/each}}
+              </ul>
+            </div>
+          {{else items}}
+            <div class="dt-items">
+              <h4>Dictionary Structure</h4>
+                <div class="typed-dict-annotation">
+                <span class="typed-dict-item"
+                >{{{each items}}<br><span
+                  {{if required !== null}}
+                    class="td-item {{if required}}required-key{{else}}optional-key{{/if}}"
+                    title="{{if required}}required-key{{else}}optional-key{{/if}}"
+                  {{else}}
+                    class="td-item"
+                  {{/if}}
+                 >'${key}': </span>
+                   <span class="td-type">&lt;${type}&gt;</span>{{/each}}<br>}</span>
+                </div>
+            </div>
+          {{/if}}
+          {{if accepts.length}}
+            <div class="dt-docs">
+              <h4>Converted Types</h4>
+              <ul class="dt-usages-list">
+              {{each accepts}}
+                <li>${$value}</li>
+              {{/each}}
+              </ul>
+            </div>
+          {{/if}}
+          {{if usages.length}}
+            <div class="dt-usages">
+              <h4>Usages</h4>
+              <ul class="dt-usages-list">
+                {{each usages}}
+                  <li><a href="#${encodeURIComponent($value)}">${$value}</a></li>
+                {{/each}}
+              </ul>
+            </div>
+          {{/if}}
+       </div>
+    </div>
+</script>
 
 <script type="text/x-jquery-tmpl" id="footer-template">
     <p class="footer">
-        <span id="altogether-count">Altogether ${keywords.length} keywords.</span>
-        <span id="match-count"></span>
-        <br>
         Generated by <a href="http://robotframework.org/robotframework/#built-in-tools">Libdoc</a> on ${generated}.
     </p>
 </script>
 
 </body>
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 
 
 
 
 
+
 ****** Opening library documentation failed ******
     * Verify that you have JavaScript enabled in your browser.
     * Make sure you are using a modern enough browser. If using Internet
-      Explorer, version 8 or newer is required.
+      Explorer, version 11 is required.
     * Check are there messages in your browser's JavaScript error log. Please
       report the problem if you suspect you have encountered a bug.
```

### Comparing `robotframework-bsnlibrary-1.0.0/robotframework_bsnlibrary.egg-info/PKG-INFO` & `robotframework-bsnlibrary-1.1.0/robotframework_bsnlibrary.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 Metadata-Version: 2.1
 Name: robotframework-bsnlibrary
-Version: 1.0.0
+Version: 1.1.0
 Summary: Robot Framework library for generating BSNs (Dutch citizen service number)
 Home-page: https://github.com/HaaiHenkie/bsnlibrary
 Author: Henk van den Akker
 Author-email: haaihenkie@users.noreply.github.com
-License: GNU General Public License v3 (GPLv3)
+License: MIT License (Expat)
 Project-URL: Documentation, https://haaihenkie.github.io/bsnlibrary/
 Project-URL: Source, https://github.com/HaaiHenkie/bsnlibrary
 Project-URL: Tracker, https://github.com/HaaiHenkie/bsnlibrary/issues
-Description: # BSNLibrary for Robot Framework
-        
-        Robot Framework Library for generating a random BSN (Burger Service Nummer, i.e. a
-        Dutch citizen service number) for test purposes.
-        
-        A BSN is used in Netherlands to identify a person for government organisations, see
-        [this information of the Dutch government](https://www.government.nl/topics/personal-data/citizen-service-number-bsn).
-        The number consists of 9 digits and has to pass the eleven test.
-        
-        This test can be explained with the example 211551557. Each digit is multiplied with
-        its position and the results are added up together:
-        
-        ``(9*2) + (8*1) + (7*1) + (6*5) + (5*5) + (4*1) + (3*5) + (2*5) - (1*7) = 110``
-        
-        Note that the digit in position 1 is subtracted from the other results. The total
-        sum can be divided by 11, which means that this number has passed the eleven test.
-        
-        This library generates BSNs for test purposes in the sense that it generates random
-        9 digit numbers that pass the eleven test. By coincidence a generated number could
-        be a real person's BSN. Yet this library cannot violate such a person's privacy,
-        because it cannot tell you whether a number belongs to a real person or not, nor
-        will it provide you with any personal data related to a BSN. Obviously you should
-        only use this library in test environments.
-        
-        This library brings the following features to Robot Framework:
-        - generating a valid BSN
-        - generating a BSN that is unique within the current test run
-        - generating a number that will not pass the eleven test
-        - generating a BSN that starts with specific digits
-        - generating a BSN that is less than 9 digits long
-        - checking if a given number passes the eleven test
-        - returning a list of BSNs generated during the current test run
-        - specifying BSNs that should not be generated
-        
-        Possible use cases:
-        - A test message that is processed by one or more systems can be tracked by its unique BSN
-        - Creating messages with BSNs in a certain range that leads to a certain response from a system or stub
-        - Checking whether a test message contains a valid BSN
-        
-        ## Backward compatibility
-        BSNLibrary v1.0.0 and later is not compatible with previous versions in the sense that is does not allow you to 
-        validate a BSN with _Generate BSN_. You should use _Validate BSN_ instead. If your test suite still uses _Generate 
-        BSN_ for validation it will generate an error saying that the length of ``given`` exceeds the maximum value. In case 
-        you have test suites using _Generate BSN_ for validation you can install BSNLibrary v0.4.0 for a smooth transition: 
-        
-        ``pip install robotframework-bsnlibrary==0.4.0``
-        
-        Your test suite will still run, but you will receive a warning of any deprecated use of _Generate BSN_ and a 
-        recommendation to replace it with the keyword _Validate BSN_. This allows you to convert your test suites at your own 
-        pace. 
-        
-        ## Installation
-        ``pip install robotframework-bsnlibrary``
-        
-        ## General information
-        [Keyword documentation](https://haaihenkie.github.io/bsnlibrary/)
-        
-        [Installation package on PyPI](https://pypi.org/project/robotframework-bsnlibrary/)
-        
-        [Release notes](https://github.com/HaaiHenkie/bsnlibrary/releases)
-        
-        Create date: 01-03-2020
-        
-        Author: Henk van den Akker
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework :: Library
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2.7
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
+Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# BSNLibrary for Robot Framework
+
+Robot Framework Library for generating a random BSN (Burger Service Nummer, i.e. a
+Dutch citizen service number) for test purposes.
+
+A BSN is used in Netherlands to identify a person for government organisations, see
+[this information of the Dutch government](https://www.government.nl/topics/personal-data/citizen-service-number-bsn).
+The number consists of 9 digits and has to pass the eleven test.
+
+This test can be explained with the example 211551557. Each digit is multiplied with
+its position and the results are added up together:
+
+``(9*2) + (8*1) + (7*1) + (6*5) + (5*5) + (4*1) + (3*5) + (2*5) - (1*7) = 110``
+
+Note that the digit in position 1 is subtracted from the other results. The total
+sum can be divided by 11, which means that this number has passed the eleven test.
+
+This library generates BSNs for test purposes in the sense that it generates random
+9 digit numbers that pass the eleven test. By coincidence a generated number could
+be a real person's BSN. Yet this library cannot violate such a person's privacy,
+because it cannot tell you whether a number belongs to a real person or not, nor
+will it provide you with any personal data related to a BSN. Obviously you should
+only use this library in test environments.
+
+This library brings the following features to Robot Framework:
+- generating a valid BSN
+- generating a BSN that is unique within the current test run
+- generating a number that will not pass the eleven test
+- generating a BSN that starts with specific digits
+- generating a BSN that is less than 9 digits long
+- checking if a given number passes the eleven test
+- returning a list of BSNs generated during the current test run
+- specifying BSNs that should not be generated
+
+Possible use cases:
+- A test message that is processed by one or more systems can be tracked by its unique BSN
+- Creating messages with BSNs in a certain range that leads to a certain response from a system or stub
+- Checking whether a test message contains a valid BSN
+
+## Backward compatibility
+BSNLibrary v1.0.0 and later is not compatible with previous versions in the sense that is does not allow you to 
+validate a BSN with _Generate BSN_. You should use _Validate BSN_ instead. If your test suite still uses _Generate 
+BSN_ for validation it will generate an error saying that the length of ``given`` exceeds the maximum value. In case 
+you have test suites using _Generate BSN_ for validation you can install BSNLibrary v0.4.0 for a smooth transition: 
+
+``pip install robotframework-bsnlibrary==0.4.0``
+
+Your test suite will still run, but you will receive a warning of any deprecated use of _Generate BSN_ and a 
+recommendation to replace it with the keyword _Validate BSN_. This allows you to convert your test suites at your own 
+pace. 
+
+## Installation
+``pip install robotframework-bsnlibrary``
+
+## General information
+[Keyword documentation](https://haaihenkie.github.io/bsnlibrary/)
+
+[Installation package on PyPI](https://pypi.org/project/robotframework-bsnlibrary/)
+
+[Release notes](https://github.com/HaaiHenkie/bsnlibrary/releases)
+
+Create date: 01-03-2020
+
+Author: Henk van den Akker
```

### Comparing `robotframework-bsnlibrary-1.0.0/setup.py` & `robotframework-bsnlibrary-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='robotframework-bsnlibrary',
-    version='1.0.0',
+    version='1.1.0',
     packages=['BSNLibrary'],
     url='https://github.com/HaaiHenkie/bsnlibrary',
     project_urls={
         'Documentation': 'https://haaihenkie.github.io/bsnlibrary/',
         'Source': 'https://github.com/HaaiHenkie/bsnlibrary',
         'Tracker': 'https://github.com/HaaiHenkie/bsnlibrary/issues',
     },
-    license='GNU General Public License v3 (GPLv3)',
+    license='MIT License (Expat)',
     author='Henk van den Akker',
     author_email='haaihenkie@users.noreply.github.com',
     description='Robot Framework library for generating BSNs (Dutch citizen service number)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
         "Framework :: Robot Framework :: Library",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Programming Language :: Python :: 2.7",
+        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     data_files=[
         ('Lib/site-packages/BSNLibrary/docs', ['docs/index.html']),
+        ('Lib/site-packages/BSNLibrary/license', ['LICENSE.txt']),
         ('Lib/site-packages/BSNLibrary/tests/BSNLibrary_test', [
             'tests/BSNLibrary_test/__init__.robot',
             'tests/BSNLibrary_test/1_Functional_tests.robot',
             'tests/BSNLibrary_test/2_Error_handling.robot',
             'tests/BSNLibrary_test/3_Demos.robot',
-            'tests/BSNLibrary_test/Resource.robot']),
-        ('Lib/site-packages/BSNLibrary/tests/BSNLibrary_test_old_syntax', [
-            'tests/BSNLibrary_test_old_syntax/__init__.robot',
-            'tests/BSNLibrary_test_old_syntax/1_Functional_tests.robot',
-            'tests/BSNLibrary_test_old_syntax/2_Error_handling.robot',
-            'tests/BSNLibrary_test_old_syntax/3_Demos.robot',
-            'tests/BSNLibrary_test_old_syntax/Resource.robot'])
+            'tests/BSNLibrary_test/Resource.robot'])
     ],
     install_requires=['robotframework'],
-    python_requires='>=2.7'
+    python_requires='>=3'
 )
```

### Comparing `robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/1_Functional_tests.robot` & `robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/1_Functional_tests.robot`

 * *Files 1% similar despite different names*

```diff
@@ -151,33 +151,33 @@
     ...    - After generating the 9 BSNs the list of generated BSNs counts 9 BSNs
     ...    - Clearing the generated BSNs gives the right log message
     ...    - After clearing the generated BSNs the list of generated BSNs counts 0 BSNs
     ...    - After clearing the generated BSNs it is possible to generate the same 9 unique BSNs again
     ...
     ...    The following statements are used by ``statuschecker`` to check the messages of _Clear Generated BSNs_
     ...
-    ...    LOG 3.1.1.1.1 GLOB: List of * generated BSNs has been cleared.
+    ...    LOG 2.1.1.1.1 GLOB: List of * generated BSNs has been cleared.
     ...
-    ...    LOG 3.1.1.9 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.1.1.9 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.2.1.1.1 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.2.1.1.1 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.2.1.9 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.2.1.9 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.3.1.1.1 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.3.1.1.1 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.3.1.9 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.3.1.9 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.4.1.1.1 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.4.1.1.1 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.4.1.9 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.4.1.9 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.5.1.1.1 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.5.1.1.1 INFO List of 9 generated BSNs has been cleared.
     ...
-    ...    LOG 3.5.1.9 INFO List of 9 generated BSNs has been cleared.
+    ...    LOG 2.5.1.9 INFO List of 9 generated BSNs has been cleared.
     @{lengths}    Create List    ${None}    ${9}    ${8}    ${7}    ${6}
     FOR    ${length}    IN    @{lengths}
         Clear list of generated BSNs    ${length}
     END
 
 Clear list of excluded BSNs with variable length
     [Documentation]    Steps:
@@ -192,53 +192,53 @@
     ...    - After excluding the 9 BSNs the list of excluded BSNs counts 9 BSNs
     ...    - Clearing the excluded BSNs gives the right log message
     ...    - After clearing the excluded BSNs the list of excluded BSNs counts 0 BSNs
     ...    - After clearing the excluded BSNs it is possible to generate the same 9 unique BSNs again
     ...
     ...    The following statements are used by ``statuschecker`` to check the messages of _Clear Excluded BSNs_
     ...
-    ...    LOG 3.1.1.1.2 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.1.1.1.2 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.1.1.12 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.1.1.12 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.2.1.1.2 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.2.1.1.2 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.2.1.12 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.2.1.12 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.3.1.1.2 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.3.1.1.2 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.3.1.12 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.3.1.12 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.4.1.1.2 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.4.1.1.2 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.4.1.12 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.4.1.12 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.5.1.1.2 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.5.1.1.2 INFO The list of excluded BSNs has been cleared.
     ...
-    ...    LOG 3.5.1.12 INFO The list of excluded BSNs has been cleared.
+    ...    LOG 2.5.1.12 INFO The list of excluded BSNs has been cleared.
     @{lengths}    Create List    ${None}    ${9}    ${8}    ${7}    ${6}
     FOR    ${length}    IN    @{lengths}
         Clear list of excluded BSNs    ${length}
     END
 
 Validate a valid BSN with variable lengths
     [Documentation]    Validates a valid BSN for every possible ``length``: 6, 7, 8 or 9.
     ...
     ...    Checks:
     ...    - Validating a valid BSN gives the right log message
     ...
     ...    The following statements are used by ``statuschecker`` to check the messages of _Clear Generated BSNs_
     ...
-    ...    LOG 3.1.1 INFO The BSN '747359489' is valid.
+    ...    LOG 2.1.1 INFO The BSN '747359489' is valid.
     ...
-    ...    LOG 3.2.1 INFO The BSN '25221577' is valid.
+    ...    LOG 2.2.1 INFO The BSN '25221577' is valid.
     ...
-    ...    LOG 3.3.1 INFO The BSN '1763921' is valid.
+    ...    LOG 2.3.1 INFO The BSN '1763921' is valid.
     ...
-    ...    LOG 3.4.1 INFO The BSN '353000' is valid.
+    ...    LOG 2.4.1 INFO The BSN '353000' is valid.
     @{bsns}    Create List    747359489    25221577    1763921    353000
     FOR    ${bsn}    IN    @{bsns}
         Validate BSN    ${bsn}
     END
 
 Validate invalid BSNs with variable length
     [Documentation]    Validates an invalid BSN for every possible ``length``: 6, 7, 8 or 9.
```

### Comparing `robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/2_Error_handling.robot` & `robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/2_Error_handling.robot`

 * *Files identical despite different names*

### Comparing `robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/3_Demos.robot` & `robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/3_Demos.robot`

 * *Files identical despite different names*

### Comparing `robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/Resource.robot` & `robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/Resource.robot`

 * *Files identical despite different names*

### Comparing `robotframework-bsnlibrary-1.0.0/tests/BSNLibrary_test/__init__.robot` & `robotframework-bsnlibrary-1.1.0/tests/BSNLibrary_test/__init__.robot`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 *** Settings ***
 Documentation     Test suite to test BSNLibrary
 ...
-...               This test suite is suitable for Robot Framework v3.1 or later and contains the new ``FOR ... END`` loop syntax. If you need the old `:FOR`` loop syntax for earlier versions, use directory BSNLibrary_test_old_syntax.
+...               This test suite is suitable for Robot Framework v3.1 or later and contains the new ``FOR ... END`` loop syntax.
 ...
 ...               The primary use of this test suite is for the developer to test BSNLibrary before it is released.
 ...
 ...               Possible other uses:
 ...               - test whether BSNLibrary works on your system
 ...               - check out how certain errors can be reproduced under _2 Error handling_
 ...               - check test cases under _3 Demos_ as referred to by the keyword documentation
```

