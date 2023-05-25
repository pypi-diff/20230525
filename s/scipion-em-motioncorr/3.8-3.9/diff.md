# Comparing `tmp/scipion-em-motioncorr-3.8.tar.gz` & `tmp/scipion-em-motioncorr-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-motioncorr-3.8.tar", last modified: Sat Oct  8 15:49:35 2022, max compression
+gzip compressed data, was "scipion-em-motioncorr-3.9.tar", last modified: Sun Nov 27 15:34:00 2022, max compression
```

## Comparing `scipion-em-motioncorr-3.8.tar` & `scipion-em-motioncorr-3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:49:35.170938 scipion-em-motioncorr-3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5530 2022-10-08 15:49:35.166938 scipion-em-motioncorr-3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3989 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:49:35.166938 scipion-em-motioncorr-3.8/motioncorr/
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:49:35.166938 scipion-em-motioncorr-3.8/motioncorr/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34554 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/protocols/protocol_motioncorr.py
--rw-r--r--   0 runner    (1001) docker     (121)    16856 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/protocols/protocol_ts_motioncor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:49:35.166938 scipion-em-motioncorr-3.8/motioncorr/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6099 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/tests/test_protocols_motioncor2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/tests/test_protocols_tomo.py
--rw-r--r--   0 runner    (1001) docker     (121)     7292 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/motioncorr/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:49:35.166938 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5530 2022-10-08 15:49:35.000000 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-10-08 15:49:35.000000 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 15:49:35.000000 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-08 15:49:35.000000 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-08 15:49:35.000000 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-08 15:49:35.000000 scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-08 15:49:35.170938 scipion-em-motioncorr-3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8684 2022-10-08 15:47:56.000000 scipion-em-motioncorr-3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5530 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/motioncorr/
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/motioncorr/protocols/
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34554 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/protocols/protocol_motioncorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16890 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/protocols/protocol_ts_motioncor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5492 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/motioncorr/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/tests/test_protocols_motioncor2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/tests/test_protocols_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7292 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/motioncorr/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5530 2022-11-27 15:34:00.000000 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-27 15:34:00.000000 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 15:34:00.000000 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2022-11-27 15:34:00.000000 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-27 15:34:00.000000 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-27 15:34:00.000000 scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 15:34:00.153531 scipion-em-motioncorr-3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     8684 2022-11-27 15:32:02.000000 scipion-em-motioncorr-3.9/setup.py
```

### Comparing `scipion-em-motioncorr-3.8/CHANGES.txt` & `scipion-em-motioncorr-3.9/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.9: remove MOTIONCOR2_PROGRAM, improve validation msg
 3.8:
     - guess cuda binary version
     - set gain to output optics table if input movies had one
 3.7: update mc2 to 1.5.0
 3.6 - implement odd/even sums for SPA
 3.5:
     - use weakImport for tomo
```

### Comparing `scipion-em-motioncorr-3.8/LICENSE` & `scipion-em-motioncorr-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/PKG-INFO` & `scipion-em-motioncorr-3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-motioncorr
-Version: 3.8
+Version: 3.9
 Summary: Plugin to use motioncorr programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-motioncorr
 Author: Grigory Sharov, J.M. De la Rosa Trevin
 Author-email: sharov.grigory@gmail.com, delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-motioncorr/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-motioncorr/
```

### Comparing `scipion-em-motioncorr-3.8/README.rst` & `scipion-em-motioncorr-3.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/__init__.py` & `scipion-em-motioncorr-3.9/motioncorr/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,42 +28,56 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.8'
+__version__ = '3.9'
 _references = ['Zheng2017']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = MOTIONCOR2_HOME
-    _pathVars = [MOTIONCOR2_PROGRAM, MOTIONCOR2_CUDA_LIB]
+    _pathVars = [MOTIONCOR2_CUDA_LIB]
     _supportedVersions = ['1.4.0', '1.4.2', '1.4.4', '1.4.5', '1.4.7', '1.5.0']
     _url = "https://github.com/scipion-em/scipion-em-motioncorr"
 
     @classmethod
     def _defineVariables(cls):
         cls._defineEmVar(MOTIONCOR2_HOME, 'motioncor2-1.5.0')
         cls._defineVar(MOTIONCOR2_CUDA_LIB, pwem.Config.CUDA_LIB)
 
         # Define the variable default value based on the guessed cuda version
         cudaVersion = cls.guessCudaVersion(MOTIONCOR2_CUDA_LIB)
         cls._defineVar(MOTIONCOR2_BIN, 'MotionCor2_1.5.0_Cuda%s%s_05-31-2022' % (
             cudaVersion.major, cudaVersion.minor))
 
-        # Final program to use
-        defaultProgram = os.path.join(cls.getHome('bin'),
-                                      os.path.basename(cls.getVar(MOTIONCOR2_BIN)))
-        cls._defineVar(MOTIONCOR2_PROGRAM, defaultProgram)
 
     @classmethod
     def getProgram(cls):
-        return cls.getVar(MOTIONCOR2_PROGRAM)
+        return os.path.join(cls.getHome('bin'),
+                            os.path.basename(cls.getVar(MOTIONCOR2_BIN)))
+
+    @classmethod
+    def validateInstallation(cls):
+        """ Check if the binaries are properly installed. """
+        try:
+            if not os.path.exists(cls.getProgram()):
+                return [f"{cls.getProgram()} does not exist, please verify "
+                        "the following variables or edit the config file:\n\n"
+                        f"{MOTIONCOR2_HOME}: {cls.getVar(MOTIONCOR2_HOME)}\n"
+                        f"{MOTIONCOR2_BIN}: {cls.getVar(MOTIONCOR2_BIN)}"]
+
+            if not os.path.exists(cls.getVar(MOTIONCOR2_CUDA_LIB)):
+                return [f"{cls.getVar(MOTIONCOR2_CUDA_LIB)} does not exist, "
+                        f"please verify {MOTIONCOR2_CUDA_LIB} variable."]
+
+        except Exception as e:
+            return ["validateInstallation fails: %s" % e]
 
     @classmethod
     def versionGE(cls, version):
         """ Return True if current version of motioncor2 is greater
          or equal than the input argument.
          Params:
             version: string version (semantic version, e.g 1.0.1)
```

### Comparing `scipion-em-motioncorr-3.8/motioncorr/bibtex.py` & `scipion-em-motioncorr-3.9/motioncorr/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/constants.py` & `scipion-em-motioncorr-3.9/motioncorr/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/convert.py` & `scipion-em-motioncorr-3.9/motioncorr/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/protocols/__init__.py` & `scipion-em-motioncorr-3.9/motioncorr/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/protocols/protocol_motioncorr.py` & `scipion-em-motioncorr-3.9/motioncorr/protocols/protocol_motioncorr.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/protocols/protocol_ts_motioncor.py` & `scipion-em-motioncorr-3.9/motioncorr/protocols/protocol_ts_motioncor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *
 # * Authors:     J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [1]
 # *
 # * [1] SciLifeLab, Stockholm University
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
@@ -98,15 +98,15 @@
         form.addParam('tol', params.FloatParam, default='0.5',
                       expertLevel=cons.LEVEL_ADVANCED,
                       label='Tolerance (px)',
                       help='Tolerance for iterative alignment, default *0.5px*.')
 
         form.addParam('doSaveUnweightedMic', params.BooleanParam, default=True,
                       condition='doApplyDoseFilter',
-                      label="Save unweighted micrographs?",
+                      label="Save unweighted tilt-series?",
                       help="Aligned but non-dose weighted images are sometimes "
                            "useful in CTF estimation, although there is no "
                            "difference in most cases.")
 
         form.addParam('extraParams2', params.StringParam, default='',
                       expertLevel=cons.LEVEL_ADVANCED,
                       label='Additional parameters',
@@ -295,16 +295,16 @@
             self.tsMList.append(tiltImageM)
 
             # Update even and odd average lists
             self.evenAvgFrameList.append(evenName)
             self.oddAvgFrameList.append(oddName)
 
         tiFn, tiFnDW = self._getOutputTiltImagePaths(tiltImageM)
-        if not os.path.exists(tiFn):
-            raise Exception("Expected output file '%s' not produced!" % tiFn)
+        if not os.path.exists(tiFn) and not os.path.exists(tiFnDW):
+            raise Exception("Expected output file(s) '%s' not produced!" % tiFn)
 
         if not pwutils.envVarOn('SCIPION_DEBUG_NOCLEAN'):
             pwutils.cleanPath(workingFolder)
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
         summary = []
```

### Comparing `scipion-em-motioncorr-3.8/motioncorr/protocols.conf` & `scipion-em-motioncorr-3.9/motioncorr/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/tests/test_protocols_motioncor2.py` & `scipion-em-motioncorr-3.9/motioncorr/tests/test_protocols_motioncor2.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/motioncorr/tests/test_protocols_tomo.py` & `scipion-em-motioncorr-3.9/motioncorr/tests/test_protocols_tomo.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # * Authors: Yunior C. Fonseca Reyna    (cfonseca@cnb.csic.es)
 # *
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
```

### Comparing `scipion-em-motioncorr-3.8/motioncorr/viewers.py` & `scipion-em-motioncorr-3.9/motioncorr/viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/PKG-INFO` & `scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-motioncorr
-Version: 3.8
+Version: 3.9
 Summary: Plugin to use motioncorr programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-motioncorr
 Author: Grigory Sharov, J.M. De la Rosa Trevin
 Author-email: sharov.grigory@gmail.com, delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-motioncorr/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-motioncorr/
```

### Comparing `scipion-em-motioncorr-3.8/scipion_em_motioncorr.egg-info/SOURCES.txt` & `scipion-em-motioncorr-3.9/scipion_em_motioncorr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-motioncorr-3.8/setup.py` & `scipion-em-motioncorr-3.9/setup.py`

 * *Files identical despite different names*

