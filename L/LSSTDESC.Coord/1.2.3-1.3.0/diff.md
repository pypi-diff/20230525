# Comparing `tmp/LSSTDESC.Coord-1.2.3.tar.gz` & `tmp/LSSTDESC.Coord-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LSSTDESC.Coord-1.2.3.tar", last modified: Thu May 19 04:18:35 2022, max compression
+gzip compressed data, was "LSSTDESC.Coord-1.3.0.tar", last modified: Thu May 25 19:32:58 2023, max compression
```

## Comparing `LSSTDESC.Coord-1.2.3.tar` & `LSSTDESC.Coord-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.778602 LSSTDESC.Coord-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-05-19 04:18:35.000000 LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-19 04:18:35.000000 LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-19 04:18:35.000000 LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-19 04:18:35.000000 LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-19 04:18:35.000000 LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/coord/
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    19114 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/angle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5306 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/angleunit.py
--rw-r--r--   0 runner    (1001) docker     (121)    46157 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/celestial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/coord/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/include/Angle_C.h
--rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/coord/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/include/Angle_C.h
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-19 04:18:35.778602 LSSTDESC.Coord-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    17529 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/src/Angle.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/src/windows.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 04:18:35.774602 LSSTDESC.Coord-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/tests/helper_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    17903 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/tests/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (121)     7735 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/tests/test_angleunit.py
--rw-r--r--   0 runner    (1001) docker     (121)    13251 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/tests/test_astropy.py
--rw-r--r--   0 runner    (1001) docker     (121)    54214 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/tests/test_celestial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-05-19 04:18:15.000000 LSSTDESC.Coord-1.2.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:58.847133 LSSTDESC.Coord-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:58.843133 LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-25 19:32:58.000000 LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 19:32:58.000000 LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:58.000000 LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 19:32:58.000000 LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 19:32:58.000000 LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-25 19:32:58.847133 LSSTDESC.Coord-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:58.843133 LSSTDESC.Coord-1.3.0/coord/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/coord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/coord/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/coord/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/coord/angleunit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46157 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/coord/celestial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/coord/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:32:58.847133 LSSTDESC.Coord-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:58.847133 LSSTDESC.Coord-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/tests/helper_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18851 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/tests/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/tests/test_angleunit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/tests/test_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54214 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/tests/test_celestial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-25 19:32:46.000000 LSSTDESC.Coord-1.3.0/tests/test_util.py
```

### Comparing `LSSTDESC.Coord-1.2.3/LICENSE` & `LSSTDESC.Coord-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/LSSTDESC.Coord.egg-info/PKG-INFO` & `LSSTDESC.Coord-1.3.0/LSSTDESC.Coord.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: LSSTDESC.Coord
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python module for handling angles and celestial coordinates
 Home-page: https://github.com/LSSTDESC/Coord
-Download-URL: https://github.com/LSSTDESC/Coord/releases/tag/v1.2.3.zip
+Download-URL: https://github.com/LSSTDESC/Coord/releases/tag/v1.3.0.zip
 Author: LSST DESC (contact: Mike Jarvis)
 Author-email: michael@jarvis.net
 License: MIT License
 License-File: LICENSE
 
-.. image:: https://api.travis-ci.org/LSSTDESC/Coord.svg?branch=master
-        :target: https://travis-ci.org/LSSTDESC/Coord
-.. image:: https://codecov.io/gh/LSSTDESC/Coord/branch/master/graph/badge.svg
+.. image:: https://github.com/LSSTDESC/Coord/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/LSSTDESC/Coord/actions/workflows/ci.yml
+.. image:: https://codecov.io/gh/LSSTDESC/Coord/branch/main/graph/badge.svg
         :target: https://codecov.io/gh/LSSTDESC/Coord
 
 Coord is a Python module that provides basic functionality related to angles and
 celestial coordinates.
 
 It is similar in functionality to the astropy.coordinates module, but with more of an
 emphasis on efficiency.  Some functions are more than 100 times faster than the corresponding
@@ -50,58 +50,28 @@
 The code is licensed under the MIT License, which basically means you can use it in any way
 you want, so long as you keep the copyright notice at the top of each source file and/or include
 the accompanying LICENSE file with the distribution.
 
 Installation
 ============
 
-Installing libffi
------------------
-
-This module is mostly pure Python.  However, it does have a small bit of C++ code, which is
-wrapped with cffi.  This in turn depends on libffi, which is not itself pip installable.
-Most modern Python installations will have this already installed, so you probably don't have
-to do anything special to use it.  However, if not, installing libffi is fairly straightforward:
-
-On a Mac, you should only need to run the command::
-
-    $ xcode-select --install
-
-On Linux, if you have root access, then one of the following should work for you::
-
-    $ apt-get install libffi-dev
-    $ yum install libffi-devel
-
-If you don't have root access (and don't want to bother your sysadmin), then installing from
-source into a {prefix} directory where you have write access (e.g. your home directory) is also
-not very hard::
-
-    $ wget ftp://sourceware.org:/pub/libffi/libffi-3.2.1.tar.gz
-    $ tar xfz libffi-3.2.1.tar.gz
-    $ cd libffi-3.2.1
-    $ ./configure --prefix={prefix}
-    $ make
-    $ make install
-    $ cp */include/ffi*.h {prefix}/include
-    $ cd ..
-
-Installing Coord
-----------------
-
-Once you have done one of the above (or not if you already have libffi installed), you can
-install Coord with pip::
+You can install Coord with pip::
 
     $ pip install LSSTDESC.Coord --user
 
 or if you have root access, you might prefer::
 
     $ sudo pip install LSSTDESC.Coord
 
 or possibly with neither ``sudo`` nor ``--user`` if your Python distro is in a writable directory.
 
+If you use anaconda you can install from conda forge::
+
+    $ conda install -c conda-forge lsstdesc.coord
+
 If you prefer to download or clone the repo and install manually, you can install with
 setup.py using one of the usual variants::
 
     $ python setup.py install --prefix={prefix}
 
 or::
```

### Comparing `LSSTDESC.Coord-1.2.3/PKG-INFO` & `LSSTDESC.Coord-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: LSSTDESC.Coord
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python module for handling angles and celestial coordinates
 Home-page: https://github.com/LSSTDESC/Coord
-Download-URL: https://github.com/LSSTDESC/Coord/releases/tag/v1.2.3.zip
+Download-URL: https://github.com/LSSTDESC/Coord/releases/tag/v1.3.0.zip
 Author: LSST DESC (contact: Mike Jarvis)
 Author-email: michael@jarvis.net
 License: MIT License
 License-File: LICENSE
 
-.. image:: https://api.travis-ci.org/LSSTDESC/Coord.svg?branch=master
-        :target: https://travis-ci.org/LSSTDESC/Coord
-.. image:: https://codecov.io/gh/LSSTDESC/Coord/branch/master/graph/badge.svg
+.. image:: https://github.com/LSSTDESC/Coord/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/LSSTDESC/Coord/actions/workflows/ci.yml
+.. image:: https://codecov.io/gh/LSSTDESC/Coord/branch/main/graph/badge.svg
         :target: https://codecov.io/gh/LSSTDESC/Coord
 
 Coord is a Python module that provides basic functionality related to angles and
 celestial coordinates.
 
 It is similar in functionality to the astropy.coordinates module, but with more of an
 emphasis on efficiency.  Some functions are more than 100 times faster than the corresponding
@@ -50,58 +50,28 @@
 The code is licensed under the MIT License, which basically means you can use it in any way
 you want, so long as you keep the copyright notice at the top of each source file and/or include
 the accompanying LICENSE file with the distribution.
 
 Installation
 ============
 
-Installing libffi
------------------
-
-This module is mostly pure Python.  However, it does have a small bit of C++ code, which is
-wrapped with cffi.  This in turn depends on libffi, which is not itself pip installable.
-Most modern Python installations will have this already installed, so you probably don't have
-to do anything special to use it.  However, if not, installing libffi is fairly straightforward:
-
-On a Mac, you should only need to run the command::
-
-    $ xcode-select --install
-
-On Linux, if you have root access, then one of the following should work for you::
-
-    $ apt-get install libffi-dev
-    $ yum install libffi-devel
-
-If you don't have root access (and don't want to bother your sysadmin), then installing from
-source into a {prefix} directory where you have write access (e.g. your home directory) is also
-not very hard::
-
-    $ wget ftp://sourceware.org:/pub/libffi/libffi-3.2.1.tar.gz
-    $ tar xfz libffi-3.2.1.tar.gz
-    $ cd libffi-3.2.1
-    $ ./configure --prefix={prefix}
-    $ make
-    $ make install
-    $ cp */include/ffi*.h {prefix}/include
-    $ cd ..
-
-Installing Coord
-----------------
-
-Once you have done one of the above (or not if you already have libffi installed), you can
-install Coord with pip::
+You can install Coord with pip::
 
     $ pip install LSSTDESC.Coord --user
 
 or if you have root access, you might prefer::
 
     $ sudo pip install LSSTDESC.Coord
 
 or possibly with neither ``sudo`` nor ``--user`` if your Python distro is in a writable directory.
 
+If you use anaconda you can install from conda forge::
+
+    $ conda install -c conda-forge lsstdesc.coord
+
 If you prefer to download or clone the repo and install manually, you can install with
 setup.py using one of the usual variants::
 
     $ python setup.py install --prefix={prefix}
 
 or::
```

### Comparing `LSSTDESC.Coord-1.2.3/README.rst` & `LSSTDESC.Coord-1.3.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. image:: https://api.travis-ci.org/LSSTDESC/Coord.svg?branch=master
-        :target: https://travis-ci.org/LSSTDESC/Coord
-.. image:: https://codecov.io/gh/LSSTDESC/Coord/branch/master/graph/badge.svg
+.. image:: https://github.com/LSSTDESC/Coord/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/LSSTDESC/Coord/actions/workflows/ci.yml
+.. image:: https://codecov.io/gh/LSSTDESC/Coord/branch/main/graph/badge.svg
         :target: https://codecov.io/gh/LSSTDESC/Coord
 
 Coord is a Python module that provides basic functionality related to angles and
 celestial coordinates.
 
 It is similar in functionality to the astropy.coordinates module, but with more of an
 emphasis on efficiency.  Some functions are more than 100 times faster than the corresponding
@@ -39,58 +39,28 @@
 The code is licensed under the MIT License, which basically means you can use it in any way
 you want, so long as you keep the copyright notice at the top of each source file and/or include
 the accompanying LICENSE file with the distribution.
 
 Installation
 ============
 
-Installing libffi
------------------
-
-This module is mostly pure Python.  However, it does have a small bit of C++ code, which is
-wrapped with cffi.  This in turn depends on libffi, which is not itself pip installable.
-Most modern Python installations will have this already installed, so you probably don't have
-to do anything special to use it.  However, if not, installing libffi is fairly straightforward:
-
-On a Mac, you should only need to run the command::
-
-    $ xcode-select --install
-
-On Linux, if you have root access, then one of the following should work for you::
-
-    $ apt-get install libffi-dev
-    $ yum install libffi-devel
-
-If you don't have root access (and don't want to bother your sysadmin), then installing from
-source into a {prefix} directory where you have write access (e.g. your home directory) is also
-not very hard::
-
-    $ wget ftp://sourceware.org:/pub/libffi/libffi-3.2.1.tar.gz
-    $ tar xfz libffi-3.2.1.tar.gz
-    $ cd libffi-3.2.1
-    $ ./configure --prefix={prefix}
-    $ make
-    $ make install
-    $ cp */include/ffi*.h {prefix}/include
-    $ cd ..
-
-Installing Coord
-----------------
-
-Once you have done one of the above (or not if you already have libffi installed), you can
-install Coord with pip::
+You can install Coord with pip::
 
     $ pip install LSSTDESC.Coord --user
 
 or if you have root access, you might prefer::
 
     $ sudo pip install LSSTDESC.Coord
 
 or possibly with neither ``sudo`` nor ``--user`` if your Python distro is in a writable directory.
 
+If you use anaconda you can install from conda forge::
+
+    $ conda install -c conda-forge lsstdesc.coord
+
 If you prefer to download or clone the repo and install manually, you can install with
 setup.py using one of the usual variants::
 
     $ python setup.py install --prefix={prefix}
 
 or::
```

### Comparing `LSSTDESC.Coord-1.2.3/coord/_version.py` & `LSSTDESC.Coord-1.3.0/coord/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.2.3'
+__version__ = '1.3.0'
 __version_info__ = tuple(map(int, __version__.split('.')))
```

### Comparing `LSSTDESC.Coord-1.2.3/coord/angle.py` & `LSSTDESC.Coord-1.3.0/coord/angle.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,25 +258,18 @@
 
     def tan(self):
         """Return the tan of an Angle."""
         return math.tan(self._rad)
 
     def sincos(self):
         """Return both the sin and cos of an Angle as a numpy array [sint, cost].
-
-        (On some systems, this may be slightly faster than doing each separately.)
         """
-        # Note: This is admittedly pretty gratuitous.  We're writing Python after all, so the
-        # difference between this and two trig calls is probably neglible given all the normal
-        # Python overhead.  Mostly, I added this as an excuse to set up the C++ extension stuff
-        # to make sure people could see how to add further C++-layer optimizations as needed.
-        import coord
-        sc = np.empty(2)
-        coord._lib.coord_sincos(self._rad, coord._ffi.cast('double*', sc.ctypes.data))
-        return sc
+        sin = math.sin(self._rad)
+        cos = math.cos(self._rad)
+        return sin, cos
 
     def __str__(self):
         return str(self._rad) + ' radians'
 
     def __repr__(self):
         return 'coord.Angle(%r, coord.radians)'%self.rad
 
@@ -486,15 +479,15 @@
         return Angle._parse_dms(str) * degrees
 
     @staticmethod
     def _parse_dms(dms):
         """Convert a string of the form dd:mm:ss.decimal into decimal degrees.
         """
         import re
-        tokens = tuple(filter(None, re.split(r'([\.\d]+)', dms.strip())))
+        tokens = tuple(filter(None, re.split('([\.\d]+)', dms.strip())))
         if len(tokens) <= 1:
             raise ValueError("string is not of the expected format")
         sign = 1
         try:
             dd = float(tokens[0])
         except ValueError:
             if tokens[0].strip() == '-':
```

### Comparing `LSSTDESC.Coord-1.2.3/coord/angleunit.py` & `LSSTDESC.Coord-1.3.0/coord/angleunit.py`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/coord/celestial.py` & `LSSTDESC.Coord-1.3.0/coord/celestial.py`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/coord/util.py` & `LSSTDESC.Coord-1.3.0/coord/util.py`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/src/windows.cpp` & `LSSTDESC.Coord-1.3.0/coord/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-/* -*- c++ -*-
- * Copyright (c) 2013-2017 LSST Dark Energy Science Collaboration (DESC)
- *
- * Permission is hereby granted, free of charge, to any person obtaining a copy
- * of this software and associated documentation files (the "Software"), to deal
- * in the Software without restriction, including without limitation the rights
- * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- * copies of the Software, and to permit persons to whom the Software is
- * furnished to do so, subject to the following conditions:
- *
- * The above copyright notice and this permission notice shall be included in all
- * copies or substantial portions of the Software.
- *
- * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- * IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- * SOFTWARE.Copyright (c) 2013-2017 LSST Dark Energy Science Collaboration (DESC)
- */
+# Copyright (c) 2013-2017 LSST Dark Energy Science Collaboration (DESC)
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 
+# The version is stored in _version.py as recommended here:
+# http://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
+#
+# flake8: noqa
 
-// This contains hacks to get the installation on Windows working.
-// This fixes error LNK2001: unresolved external symbol PyInit__coord
-// cf. https://techoverflow.net/2022/01/23/how-to-fix-python-cffi-error-lnk2001-unresolved-external-symbol-pyinit__/
-void PyInit__coord(void) { }
+from ._version import __version__, __version_info__
+
+# Also let coord.version show the version.
+version = __version__
+
+# Explicitly import things that we want to be in the coord namespace
+from .angleunit import AngleUnit, arcsec, arcmin, degrees, hours, radians
+from .angle import Angle, _Angle
+from .celestial import CelestialCoord, _CelestialCoord
+
+# This isn't imported to the coord namespace.  You need to do coord.util.blah
+from . import util
```

### Comparing `LSSTDESC.Coord-1.2.3/tests/helper_util.py` & `LSSTDESC.Coord-1.3.0/tests/helper_util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from __future__ import print_function
 
 try:
     import cPickle as pickle
 except ImportError:
     import pickle
 import copy
-from collections import Counter
 try:
     from collections.abc import Hashable
 except ImportError:
     from collections import Hashable
+from collections import Counter
 import functools
 import time
 import coord
 
 # This file has some helper functions that are used by tests from multiple files to help
 # avoid code duplication.
```

### Comparing `LSSTDESC.Coord-1.2.3/tests/test_angle.py` & `LSSTDESC.Coord-1.3.0/tests/test_angle.py`

 * *Files 6% similar despite different names*

```diff
@@ -212,14 +212,28 @@
 
     # Have to explicitly wrap if you want it.
     assert theta2.wrap() < theta5.wrap()
     assert theta5.wrap() > theta2.wrap()
     assert theta3.wrap() > theta4.wrap()
     assert theta4.wrap() < theta3.wrap()
 
+    # Check invalid arithmetic
+    np.testing.assert_raises(TypeError, coord.Angle.__lt__, theta1, 23)
+    np.testing.assert_raises(TypeError, coord.Angle.__lt__, theta1, '23')
+    np.testing.assert_raises(TypeError, coord.Angle.__lt__, theta1, coord.degrees)
+    np.testing.assert_raises(TypeError, coord.Angle.__le__, theta1, 23)
+    np.testing.assert_raises(TypeError, coord.Angle.__le__, theta1, '23')
+    np.testing.assert_raises(TypeError, coord.Angle.__le__, theta1, coord.degrees)
+    np.testing.assert_raises(TypeError, coord.Angle.__gt__, theta1, 23)
+    np.testing.assert_raises(TypeError, coord.Angle.__gt__, theta1, '23')
+    np.testing.assert_raises(TypeError, coord.Angle.__gt__, theta1, coord.degrees)
+    np.testing.assert_raises(TypeError, coord.Angle.__ge__, theta1, 23)
+    np.testing.assert_raises(TypeError, coord.Angle.__ge__, theta1, '23')
+    np.testing.assert_raises(TypeError, coord.Angle.__ge__, theta1, coord.degrees)
+
 
 @timer
 def test_trig():
     """Test the various trig functions with Angles
     """
     theta1 = 45 * coord.degrees
     np.testing.assert_almost_equal(theta1.sin(), math.sqrt(0.5), decimal=12)
```

### Comparing `LSSTDESC.Coord-1.2.3/tests/test_angleunit.py` & `LSSTDESC.Coord-1.3.0/tests/test_angleunit.py`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/tests/test_astropy.py` & `LSSTDESC.Coord-1.3.0/tests/test_astropy.py`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/tests/test_celestial.py` & `LSSTDESC.Coord-1.3.0/tests/test_celestial.py`

 * *Files identical despite different names*

### Comparing `LSSTDESC.Coord-1.2.3/tests/test_util.py` & `LSSTDESC.Coord-1.3.0/tests/test_util.py`

 * *Files identical despite different names*

