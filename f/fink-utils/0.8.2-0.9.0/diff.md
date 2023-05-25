# Comparing `tmp/fink-utils-0.8.2.tar.gz` & `tmp/fink-utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fink-utils-0.8.2.tar", last modified: Fri Jan 13 07:37:14 2023, max compression
+gzip compressed data, was "fink-utils-0.9.0.tar", last modified: Thu Feb  2 08:26:26 2023, max compression
```

## Comparing `fink-utils-0.8.2.tar` & `fink-utils-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.277114 fink-utils-0.8.2/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    11357 2022-07-18 11:52:48.000000 fink-utils-0.8.2/LICENSE
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     1280 2023-01-13 07:37:14.273114 fink-utils-0.8.2/PKG-INFO
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      621 2022-08-17 13:03:39.000000 fink-utils-0.8.2/README.md
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      628 2023-01-13 07:36:57.000000 fink-utils-0.8.2/fink_utils/__init__.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/broker/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/broker/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     3278 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/broker/avroUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    17398 2023-01-11 12:43:48.000000 fink-utils-0.8.2/fink_utils/broker/distributionUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    14241 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/broker/hbaseUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     2759 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/broker/loggingUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     7089 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/broker/slackUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    12551 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/broker/sparkUtils.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/data/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/data/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     6132 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/data/utils.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/hbase/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/hbase/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     3009 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/hbase/utils.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/photometry/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/photometry/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     4856 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/photometry/conversion.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     3396 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/photometry/test.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     5435 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/photometry/vect_conversion.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/science/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/science/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     3535 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/science/utils.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/spark/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/spark/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     4481 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/spark/partitioning.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     7526 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/spark/utils.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/sso/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:36:57.000000 fink-utils-0.8.2/fink_utils/sso/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     6360 2023-01-13 07:36:57.000000 fink-utils-0.8.2/fink_utils/sso/spins.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     5592 2023-01-13 07:36:57.000000 fink-utils-0.8.2/fink_utils/sso/utils.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/test/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/test/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     5819 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/test/tester.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils/xmatch/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/xmatch/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     8770 2022-07-18 11:52:48.000000 fink-utils-0.8.2/fink_utils/xmatch/otypes.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     7798 2022-09-23 12:03:20.000000 fink-utils-0.8.2/fink_utils/xmatch/simbad.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:37:14.273114 fink-utils-0.8.2/fink_utils.egg-info/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     1280 2023-01-13 07:37:13.000000 fink-utils-0.8.2/fink_utils.egg-info/PKG-INFO
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     1027 2023-01-13 07:37:14.000000 fink-utils-0.8.2/fink_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        1 2023-01-13 07:37:13.000000 fink-utils-0.8.2/fink_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)       11 2023-01-13 07:37:14.000000 fink-utils-0.8.2/fink_utils.egg-info/top_level.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)       38 2023-01-13 07:37:14.277114 fink-utils-0.8.2/setup.cfg
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     1542 2022-09-23 12:03:20.000000 fink-utils-0.8.2/setup.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.722568 fink-utils-0.9.0/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    11357 2022-07-18 11:52:48.000000 fink-utils-0.9.0/LICENSE
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     1280 2023-02-02 08:26:26.722568 fink-utils-0.9.0/PKG-INFO
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      621 2022-08-17 13:03:39.000000 fink-utils-0.9.0/README.md
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      628 2023-02-02 08:26:01.000000 fink-utils-0.9.0/fink_utils/__init__.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/broker/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/broker/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     3278 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/broker/avroUtils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    17398 2023-01-11 12:43:48.000000 fink-utils-0.9.0/fink_utils/broker/distributionUtils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    14241 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/broker/hbaseUtils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     2759 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/broker/loggingUtils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     7089 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/broker/slackUtils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    12551 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/broker/sparkUtils.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/data/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/data/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     6132 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/data/utils.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/hbase/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/hbase/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     3009 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/hbase/utils.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/photometry/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/photometry/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     4856 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/photometry/conversion.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     3396 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/photometry/test.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     5435 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/photometry/vect_conversion.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/science/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/science/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     3535 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/science/utils.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/spark/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/spark/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     4481 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/spark/partitioning.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     7526 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/spark/utils.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils/sso/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2023-01-13 07:36:57.000000 fink-utils-0.9.0/fink_utils/sso/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     6360 2023-01-13 07:36:57.000000 fink-utils-0.9.0/fink_utils/sso/spins.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     9352 2023-02-02 08:25:34.000000 fink-utils-0.9.0/fink_utils/sso/utils.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.722568 fink-utils-0.9.0/fink_utils/test/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/test/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     5819 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/test/tester.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.722568 fink-utils-0.9.0/fink_utils/xmatch/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        0 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/xmatch/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     8770 2022-07-18 11:52:48.000000 fink-utils-0.9.0/fink_utils/xmatch/otypes.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     7798 2022-09-23 12:03:20.000000 fink-utils-0.9.0/fink_utils/xmatch/simbad.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-02 08:26:26.718568 fink-utils-0.9.0/fink_utils.egg-info/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     1280 2023-02-02 08:26:26.000000 fink-utils-0.9.0/fink_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     1027 2023-02-02 08:26:26.000000 fink-utils-0.9.0/fink_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        1 2023-02-02 08:26:26.000000 fink-utils-0.9.0/fink_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)       11 2023-02-02 08:26:26.000000 fink-utils-0.9.0/fink_utils.egg-info/top_level.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)       38 2023-02-02 08:26:26.722568 fink-utils-0.9.0/setup.cfg
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     1542 2022-09-23 12:03:20.000000 fink-utils-0.9.0/setup.py
```

### Comparing `fink-utils-0.8.2/LICENSE` & `fink-utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/PKG-INFO` & `fink-utils-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fink-utils
-Version: 0.8.2
+Version: 0.9.0
 Summary:  Collection of useful functionalities used across the Fink ecosystem.
 Home-page: https://github.com/astrolabsoftware/fink-utils
 Author: JulienPeloton
 Author-email: peloton@lal.in2p3.fr
 License: UNKNOWN
 Project-URL: Source, https://github.com/astrolabsoftware/fink-utils
 Platform: UNKNOWN
```

### Comparing `fink-utils-0.8.2/README.md` & `fink-utils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/__init__.py` & `fink-utils-0.9.0/fink_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.8.2"
+__version__ = "0.9.0"
```

### Comparing `fink-utils-0.8.2/fink_utils/broker/avroUtils.py` & `fink-utils-0.9.0/fink_utils/broker/avroUtils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/broker/distributionUtils.py` & `fink-utils-0.9.0/fink_utils/broker/distributionUtils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/broker/hbaseUtils.py` & `fink-utils-0.9.0/fink_utils/broker/hbaseUtils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/broker/loggingUtils.py` & `fink-utils-0.9.0/fink_utils/broker/loggingUtils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/broker/slackUtils.py` & `fink-utils-0.9.0/fink_utils/broker/slackUtils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/broker/sparkUtils.py` & `fink-utils-0.9.0/fink_utils/broker/sparkUtils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/data/utils.py` & `fink-utils-0.9.0/fink_utils/data/utils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/hbase/utils.py` & `fink-utils-0.9.0/fink_utils/hbase/utils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/photometry/conversion.py` & `fink-utils-0.9.0/fink_utils/photometry/conversion.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/photometry/test.py` & `fink-utils-0.9.0/fink_utils/photometry/test.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/photometry/vect_conversion.py` & `fink-utils-0.9.0/fink_utils/photometry/vect_conversion.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/science/utils.py` & `fink-utils-0.9.0/fink_utils/science/utils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/spark/partitioning.py` & `fink-utils-0.9.0/fink_utils/spark/partitioning.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/spark/utils.py` & `fink-utils-0.9.0/fink_utils/spark/utils.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/sso/spins.py` & `fink-utils-0.9.0/fink_utils/sso/spins.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/sso/utils.py` & `fink-utils-0.9.0/fink_utils/sso/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-# Copyright 2022 AstroLab Software
+# Copyright 2022-2023 AstroLab Software
 # Author: Julien Peloton
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import requests
+import subprocess
+import json
+import os
 
 import pandas as pd
 import numpy as np
 
 from astropy.coordinates import SkyCoord
+from astropy.time import Time
 import astropy.units as u
 
 def query_miriade(ident, jd, observer='I41', rplane='1', tcoor=5, shift=15.):
     """ Gets asteroid or comet ephemerides from IMCCE Miriade for a suite of JD for a single SSO
 
     Original function by M. Mahlke, adapted for Fink usage.
 
@@ -92,15 +96,97 @@
     try:
         ephem = pd.DataFrame.from_dict(j['data'])
     except KeyError:
         return pd.DataFrame()
 
     return ephem
 
-def get_miriade_data(pdf, observer='I41', rplane='1', tcoor=5, withecl=True):
+def query_miriade_epehemcc(ident, jd, observer='I41', rplane='1', tcoor=5, shift=15., parameters={}):
+    """ Gets asteroid or comet ephemerides from IMCCE Miriade for a suite of JD for a single SSO
+
+    This uses local installation of ephemcc instead of the REST API.
+
+    Limitations:
+        - Color ephemerides are returned only for asteroids
+        - Temporary designations (C/... or YYYY...) do not have ephemerides available
+
+    Parameters
+    ----------
+    ident: int, float, str
+        asteroid or comet identifier
+    jd: array
+        dates to query
+    observer: str
+        IAU Obs code - default to ZTF: https://minorplanetcenter.net//iau/lists/ObsCodesF.html
+    rplane: str
+        Reference plane: equator ('1'), ecliptic ('2').
+        If rplane = '2', then tcoor is automatically set to 1 (spherical)
+    tcoor: int
+        See https://ssp.imcce.fr/webservices/miriade/api/ephemcc/
+        Default is 5 (dedicated to observation)
+    shift: float
+        Time shift to center exposure times, in second.
+        Default is 15 seconds which is half of the exposure time for ZTF.
+    parameters: dict
+        runner_path, userconf, iofile, outdir
+
+    Returns
+    ----------
+    pd.DataFrame
+        Input dataframe with ephemerides columns
+        appended False if query failed somehow
+
+    """
+    # write tmp files on disk
+    date_path = '{}/dates_{}.txt'.format(parameters['outdir'], ident)
+    ephem_path = '{}/ephem_{}.json'.format(parameters['outdir'], ident)
+
+    pdf = pd.DataFrame(jd)
+
+    shift_hour = shift / 24.0 / 3600.0
+    pdf\
+        .apply(lambda epoch: Time(epoch + shift_hour, format='jd').iso)\
+        .to_csv(date_path, index=False, header=False)
+
+    # launch the processing
+    cmd = [
+        parameters['runner_path'],
+        str(ident),
+        str(rplane),
+        str(tcoor),
+        observer,
+        "UTC",
+        parameters['userconf'],
+        parameters['iofile'],
+        parameters['outdir']
+    ]
+
+    # subprocess.run(cmd, capture_output=True)
+    out = subprocess.run(cmd)
+
+    if out.returncode != 0:
+        print("Error code {}".format(out.returncode))
+
+        # clean date file
+        os.remove(date_path)
+
+        return pd.DataFrame()
+
+    # read the data from disk and return
+    with open(ephem_path, 'r') as f:
+        data = json.load(f)
+    ephem = pd.DataFrame(data['data'], columns=data['datacol'].keys())
+
+    # clean tmp files
+    os.remove(ephem_path)
+    os.remove(date_path)
+
+    return ephem
+
+def get_miriade_data(pdf, observer='I41', rplane='1', tcoor=5, withecl=True, method='rest', parameters={}):
     """ Add ephemerides information from Miriade to a Pandas DataFrame with SSO lightcurve
 
     Parameters
     ----------
     pdf: pd.DataFrame
         Pandas DataFrame containing Fink alert data for a (or several) SSO
     observer: str
@@ -111,50 +197,77 @@
         If rplane = '2', then tcoor is automatically set to 1 (spherical)
     tcoor: int
         See https://ssp.imcce.fr/webservices/miriade/api/ephemcc/
         Default is 5 (dedicated to observation)
     withecl: bool
         If True, query for also for ecliptic Longitude & Latitude (extra call to miriade).
         Default is True.
+    method: str
+        Use the REST API (`rest`), or a local installation of miriade (`ephemcc`)
+    parameters: dict
+        If method == `ephemcc`, specify the mapping of extra parameters here.
 
     Returns
     ----------
     out: pd.DataFrame
         DataFrame of the same length, but with new columns from the ephemerides service.
     """
     ssnamenrs = np.unique(pdf['i:ssnamenr'].values)
 
     infos = []
     for ssnamenr in ssnamenrs:
         mask = pdf['i:ssnamenr'] == ssnamenr
         pdf_sub = pdf[mask]
 
-        eph = query_miriade(
-            str(ssnamenr),
-            pdf_sub['i:jd'],
-            observer=observer,
-            rplane=rplane,
-            tcoor=tcoor
-        )
+        if method == 'rest':
+            eph = query_miriade(
+                str(ssnamenr),
+                pdf_sub['i:jd'],
+                observer=observer,
+                rplane=rplane,
+                tcoor=tcoor
+            )
+        elif method == 'ephemcc':
+            eph = query_miriade_epehemcc(
+                str(ssnamenr),
+                pdf_sub['i:jd'],
+                observer=observer,
+                rplane=rplane,
+                tcoor=tcoor,
+                parameters=parameters
+            )
+        else:
+            raise AssertionError('Method must be `rest` or `ephemcc`. {} not supported'.format(method))
 
         if not eph.empty:
             sc = SkyCoord(eph['RA'], eph['DEC'], unit=(u.deg, u.deg))
 
             eph = eph.drop(columns=['RA', 'DEC'])
             eph['RA'] = sc.ra.value * 15
             eph['Dec'] = sc.dec.value
 
             if withecl:
                 # Add Ecliptic coordinates
-                eph_ec = query_miriade(
-                    str(ssnamenr),
-                    pdf_sub['i:jd'],
-                    observer=observer,
-                    rplane='2'
-                )
+                if method == 'rest':
+                    eph_ec = query_miriade(
+                        str(ssnamenr),
+                        pdf_sub['i:jd'],
+                        observer=observer,
+                        rplane='2'
+                    )
+                elif method == 'ephemcc':
+                    eph_ec = query_miriade_epehemcc(
+                        str(ssnamenr),
+                        pdf_sub['i:jd'],
+                        observer=observer,
+                        rplane='2',
+                        parameters=parameters
+                    )
+                else:
+                    raise AssertionError('Method must be `rest` or `ephemcc`. {} not supported'.format(method))
 
                 sc = SkyCoord(eph_ec['Longitude'], eph_ec['Latitude'], unit=(u.deg, u.deg))
                 eph['Longitude'] = sc.ra.value
                 eph['Latitude'] = sc.dec.value
 
             # Merge fink & Eph
             info = pd.concat([eph.reset_index(), pdf_sub.reset_index()], axis=1)
```

### Comparing `fink-utils-0.8.2/fink_utils/test/tester.py` & `fink-utils-0.9.0/fink_utils/test/tester.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/xmatch/otypes.txt` & `fink-utils-0.9.0/fink_utils/xmatch/otypes.txt`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils/xmatch/simbad.py` & `fink-utils-0.9.0/fink_utils/xmatch/simbad.py`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/fink_utils.egg-info/PKG-INFO` & `fink-utils-0.9.0/fink_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fink-utils
-Version: 0.8.2
+Version: 0.9.0
 Summary:  Collection of useful functionalities used across the Fink ecosystem.
 Home-page: https://github.com/astrolabsoftware/fink-utils
 Author: JulienPeloton
 Author-email: peloton@lal.in2p3.fr
 License: UNKNOWN
 Project-URL: Source, https://github.com/astrolabsoftware/fink-utils
 Platform: UNKNOWN
```

### Comparing `fink-utils-0.8.2/fink_utils.egg-info/SOURCES.txt` & `fink-utils-0.9.0/fink_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fink-utils-0.8.2/setup.py` & `fink-utils-0.9.0/setup.py`

 * *Files identical despite different names*

