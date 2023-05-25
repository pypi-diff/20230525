# Comparing `tmp/suddendeath-0.5.1.tar.gz` & `tmp/suddendeath-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suddendeath-0.5.1.tar", last modified: Thu May 25 04:39:14 2023, max compression
+gzip compressed data, was "suddendeath-0.5.2.tar", last modified: Thu May 25 06:06:11 2023, max compression
```

## Comparing `suddendeath-0.5.1.tar` & `suddendeath-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 04:39:14.521827 suddendeath-0.5.1/
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)    11356 2023-05-25 00:37:03.000000 suddendeath-0.5.1/LICENSE
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)       59 2023-05-25 04:14:49.000000 suddendeath-0.5.1/MANIFEST.in
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)    14244 2023-05-25 04:39:14.521593 suddendeath-0.5.1/PKG-INFO
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      504 2023-05-25 04:35:59.000000 suddendeath-0.5.1/README.rst
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      997 2023-05-25 04:31:14.000000 suddendeath-0.5.1/pyproject.toml
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)       38 2023-05-25 04:39:14.521873 suddendeath-0.5.1/setup.cfg
-drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 04:39:14.520602 suddendeath-0.5.1/suddendeath/
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)     2070 2023-05-25 04:38:11.000000 suddendeath-0.5.1/suddendeath/__init__.py
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      586 2023-05-25 04:35:08.000000 suddendeath-0.5.1/suddendeath/__main__.py
-drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 04:39:14.521192 suddendeath-0.5.1/suddendeath.egg-info/
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)    14244 2023-05-25 04:39:14.000000 suddendeath-0.5.1/suddendeath.egg-info/PKG-INFO
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      252 2023-05-25 04:39:14.000000 suddendeath-0.5.1/suddendeath.egg-info/SOURCES.txt
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)        1 2023-05-25 04:39:14.000000 suddendeath-0.5.1/suddendeath.egg-info/dependency_links.txt
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)       12 2023-05-25 04:39:14.000000 suddendeath-0.5.1/suddendeath.egg-info/top_level.txt
-drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 04:39:14.521331 suddendeath-0.5.1/tests/
--rw-r--r--   0 yoshifumi (135160) primarygroup (89939)     1712 2023-05-25 00:37:03.000000 suddendeath-0.5.1/tests/test_init.py
+drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 06:06:11.030782 suddendeath-0.5.2/
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)    11356 2023-05-25 00:37:03.000000 suddendeath-0.5.2/LICENSE
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)       59 2023-05-25 04:14:49.000000 suddendeath-0.5.2/MANIFEST.in
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)    14244 2023-05-25 06:06:11.030574 suddendeath-0.5.2/PKG-INFO
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      504 2023-05-25 04:35:59.000000 suddendeath-0.5.2/README.rst
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      997 2023-05-25 04:31:14.000000 suddendeath-0.5.2/pyproject.toml
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)       38 2023-05-25 06:06:11.030832 suddendeath-0.5.2/setup.cfg
+drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 06:06:11.029250 suddendeath-0.5.2/suddendeath/
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)     1818 2023-05-25 06:01:06.000000 suddendeath-0.5.2/suddendeath/__init__.py
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      811 2023-05-25 06:05:59.000000 suddendeath-0.5.2/suddendeath/__main__.py
+drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 06:06:11.030079 suddendeath-0.5.2/suddendeath.egg-info/
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)    14244 2023-05-25 06:06:11.000000 suddendeath-0.5.2/suddendeath.egg-info/PKG-INFO
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)      252 2023-05-25 06:06:11.000000 suddendeath-0.5.2/suddendeath.egg-info/SOURCES.txt
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)        1 2023-05-25 06:06:11.000000 suddendeath-0.5.2/suddendeath.egg-info/dependency_links.txt
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)       12 2023-05-25 06:06:11.000000 suddendeath-0.5.2/suddendeath.egg-info/top_level.txt
+drwxr-xr-x   0 yoshifumi (135160) primarygroup (89939)        0 2023-05-25 06:06:11.030240 suddendeath-0.5.2/tests/
+-rw-r--r--   0 yoshifumi (135160) primarygroup (89939)     1712 2023-05-25 00:37:03.000000 suddendeath-0.5.2/tests/test_init.py
```

### Comparing `suddendeath-0.5.1/LICENSE` & `suddendeath-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `suddendeath-0.5.1/PKG-INFO` & `suddendeath-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suddendeath
-Version: 0.5.1
+Version: 0.5.2
 Summary: suddendeath generates 突然の死 message.
 Author-email: Yoshi Yamaguchi <ymotongpoo@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `suddendeath-0.5.1/pyproject.toml` & `suddendeath-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `suddendeath-0.5.1/suddendeath/__init__.py` & `suddendeath-0.5.2/suddendeath/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 suddendeath module generates "突然の死" like messages.
 """
 
 import sys
 from itertools import cycle
 from unicodedata import east_asian_width
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 CODEC = "utf-8"
 if sys.platform == "win32":
     CODEC = "mbcs"
 
 DEFAULT_MESSAGE = "突然の死"
 
@@ -60,16 +60,7 @@
         footer += next(footer_pattern)
     footer += "￣"
 
     middle = "＞　" + message + "　＜"
     return "\n".join([header, middle, footer])
 
 
-def main():
-    if len(sys.argv) < 2:
-        message = DEFAULT_MESSAGE
-    else:
-        message = sys.argv[1]
-        if sys.version_info.major == 2:
-            message = message.decode(CODEC)
-
-    print((suddendeathmessage(message).encode(CODEC)))
```

### Comparing `suddendeath-0.5.1/suddendeath/__main__.py` & `suddendeath-0.5.2/suddendeath/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,8 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+
+from . import CODEC, DEFAULT_MESSAGE, suddendeathmessage
+
+
+def main():
+    if len(sys.argv) < 2:
+        message = DEFAULT_MESSAGE
+    else:
+        message = sys.argv[1]
+
+    print(suddendeathmessage(message))
+
+
 main()
```

### Comparing `suddendeath-0.5.1/suddendeath.egg-info/PKG-INFO` & `suddendeath-0.5.2/suddendeath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suddendeath
-Version: 0.5.1
+Version: 0.5.2
 Summary: suddendeath generates 突然の死 message.
 Author-email: Yoshi Yamaguchi <ymotongpoo@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `suddendeath-0.5.1/tests/test_init.py` & `suddendeath-0.5.2/tests/test_init.py`

 * *Files identical despite different names*

