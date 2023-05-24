# Comparing `tmp/pychuck-1.0.0.tar.gz` & `tmp/pychuck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychuck-1.0.0.tar", last modified: Fri May 19 01:28:41 2023, max compression
+gzip compressed data, was "pychuck-1.0.1.tar", last modified: Wed May 24 22:04:34 2023, max compression
```

## Comparing `pychuck-1.0.0.tar` & `pychuck-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.121923 pychuck-1.0.0/
--rw-r--r--   0 ykli       (501) staff       (20)     1073 2023-05-18 08:14:19.000000 pychuck-1.0.0/LICENSE
--rw-r--r--   0 ykli       (501) staff       (20)     2267 2023-05-19 01:28:41.121818 pychuck-1.0.0/PKG-INFO
--rw-r--r--   0 ykli       (501) staff       (20)      501 2023-05-18 21:41:10.000000 pychuck-1.0.0/README.md
--rw-r--r--   0 ykli       (501) staff       (20)     1175 2023-05-19 01:28:28.000000 pychuck-1.0.0/pyproject.toml
--rw-r--r--   0 ykli       (501) staff       (20)       38 2023-05-19 01:28:41.121952 pychuck-1.0.0/setup.cfg
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.119338 pychuck-1.0.0/src/
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.120853 pychuck-1.0.0/src/pychuck/
--rw-r--r--   0 ykli       (501) staff       (20)      278 2023-05-18 10:21:13.000000 pychuck-1.0.0/src/pychuck/__init__.py
--rw-r--r--   0 ykli       (501) staff       (20)     3908 2023-05-18 21:30:14.000000 pychuck-1.0.0/src/pychuck/core.py
--rw-r--r--   0 ykli       (501) staff       (20)     4176 2023-05-18 10:25:46.000000 pychuck-1.0.0/src/pychuck/unit.py
--rw-r--r--   0 ykli       (501) staff       (20)     3439 2023-05-18 10:15:01.000000 pychuck-1.0.0/src/pychuck/util.py
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.121685 pychuck-1.0.0/src/pychuck.egg-info/
--rw-r--r--   0 ykli       (501) staff       (20)     2267 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/PKG-INFO
--rw-r--r--   0 ykli       (501) staff       (20)      328 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/SOURCES.txt
--rw-r--r--   0 ykli       (501) staff       (20)        1 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/dependency_links.txt
--rw-r--r--   0 ykli       (501) staff       (20)       99 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/entry_points.txt
--rw-r--r--   0 ykli       (501) staff       (20)       47 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/requires.txt
--rw-r--r--   0 ykli       (501) staff       (20)        8 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/top_level.txt
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-24 22:04:34.587978 pychuck-1.0.1/
+-rw-r--r--   0 ykli       (501) staff       (20)     1073 2023-05-18 08:14:19.000000 pychuck-1.0.1/LICENSE
+-rw-r--r--   0 ykli       (501) staff       (20)     2337 2023-05-24 22:04:34.587862 pychuck-1.0.1/PKG-INFO
+-rw-r--r--   0 ykli       (501) staff       (20)      501 2023-05-18 21:41:10.000000 pychuck-1.0.1/README.md
+-rw-r--r--   0 ykli       (501) staff       (20)     1185 2023-05-24 22:04:03.000000 pychuck-1.0.1/pyproject.toml
+-rw-r--r--   0 ykli       (501) staff       (20)       38 2023-05-24 22:04:34.588014 pychuck-1.0.1/setup.cfg
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-24 22:04:34.585898 pychuck-1.0.1/src/
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-24 22:04:34.586835 pychuck-1.0.1/src/pychuck/
+-rw-r--r--   0 ykli       (501) staff       (20)      278 2023-05-18 10:21:13.000000 pychuck-1.0.1/src/pychuck/__init__.py
+-rw-r--r--   0 ykli       (501) staff       (20)     6104 2023-05-24 21:49:42.000000 pychuck-1.0.1/src/pychuck/core.py
+-rw-r--r--   0 ykli       (501) staff       (20)    22107 2023-05-24 21:47:37.000000 pychuck-1.0.1/src/pychuck/gui.py
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-24 22:04:34.587718 pychuck-1.0.1/src/pychuck/ui/
+-rw-r--r--   0 ykli       (501) staff       (20)    10302 2023-05-24 21:43:50.000000 pychuck-1.0.1/src/pychuck/ui/main.py
+-rw-r--r--   0 ykli       (501) staff       (20)    12005 2023-05-22 23:09:31.000000 pychuck-1.0.1/src/pychuck/ui/pyaudicle.py
+-rw-r--r--   0 ykli       (501) staff       (20)     4335 2023-05-23 01:13:50.000000 pychuck-1.0.1/src/pychuck/unit.py
+-rw-r--r--   0 ykli       (501) staff       (20)     5647 2023-05-22 23:48:10.000000 pychuck-1.0.1/src/pychuck/util.py
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-24 22:04:34.587502 pychuck-1.0.1/src/pychuck.egg-info/
+-rw-r--r--   0 ykli       (501) staff       (20)     2337 2023-05-24 22:04:34.000000 pychuck-1.0.1/src/pychuck.egg-info/PKG-INFO
+-rw-r--r--   0 ykli       (501) staff       (20)      398 2023-05-24 22:04:34.000000 pychuck-1.0.1/src/pychuck.egg-info/SOURCES.txt
+-rw-r--r--   0 ykli       (501) staff       (20)        1 2023-05-24 22:04:34.000000 pychuck-1.0.1/src/pychuck.egg-info/dependency_links.txt
+-rw-r--r--   0 ykli       (501) staff       (20)       99 2023-05-24 22:04:34.000000 pychuck-1.0.1/src/pychuck.egg-info/entry_points.txt
+-rw-r--r--   0 ykli       (501) staff       (20)       58 2023-05-24 22:04:34.000000 pychuck-1.0.1/src/pychuck.egg-info/requires.txt
+-rw-r--r--   0 ykli       (501) staff       (20)        8 2023-05-24 22:04:34.000000 pychuck-1.0.1/src/pychuck.egg-info/top_level.txt
```

### Comparing `pychuck-1.0.0/LICENSE` & `pychuck-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychuck-1.0.0/PKG-INFO` & `pychuck-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychuck
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python implementation of music programming language Chuck
 Author-email: Yikai Li <yikaili@stanford.edu>
 Maintainer-email: Yikai Li <yikaili@stanford.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -19,14 +19,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Project-URL: documentation, https://pychuck.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/42x00/pychuck.git
 Keywords: chuck,music,programming,sound,synthesis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gui
```

### Comparing `pychuck-1.0.0/pyproject.toml` & `pychuck-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pychuck"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python implementation of music programming language Chuck"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["chuck", "music", "programming", "sound", "synthesis"]
 authors = [
     { name = "Yikai Li", email = "yikaili@stanford.edu" },
@@ -26,20 +26,20 @@
     "networkx",
     "sounddevice",
 ]
 
 # dynamic = ["version", "description"]
 
 [project.optional-dependencies]
-gui = ["PyQt6"]
+gui = ["PyQt6-QScintilla"]
 cli = []
 
 [project.urls]
 #homepage = "https://example.com"
-#documentation = "https://pychuck.readthedocs.io/en/latest/"
+documentation = "https://pychuck.readthedocs.io/en/latest/"
 repository = "https://github.com/42x00/pychuck.git"
 #changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 [project.scripts]
 pychuck = "pychuck.core:main_cli"
 
 [project.gui-scripts]
```

### Comparing `pychuck-1.0.0/src/pychuck/unit.py` & `pychuck-1.0.1/src/pychuck/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,20 @@
     def __init__(self, *args, **kwargs):
         super().__init__(add_to_shred=False, *args, **kwargs)
 
     def _compute(self, samples: int):
         pass
 
 
+class Gain(UGen):
+    def _compute(self, samples: int):
+        self._aggregate_input(samples)
+        self.buffered = self._in_buffer[:samples] * self.gain
+
+
 class SinOsc(UGen):
     def __init__(self, freq: float = 440.0, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.freq: float = freq
         self._phase: float = -np.pi / 2
         self._sample_rate: int = pychuck.VM._sample_rate
```

### Comparing `pychuck-1.0.0/src/pychuck.egg-info/PKG-INFO` & `pychuck-1.0.1/src/pychuck.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychuck
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python implementation of music programming language Chuck
 Author-email: Yikai Li <yikaili@stanford.edu>
 Maintainer-email: Yikai Li <yikaili@stanford.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -19,14 +19,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Project-URL: documentation, https://pychuck.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/42x00/pychuck.git
 Keywords: chuck,music,programming,sound,synthesis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gui
```

