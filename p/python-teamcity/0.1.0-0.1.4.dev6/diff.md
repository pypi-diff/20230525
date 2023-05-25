# Comparing `tmp/python-teamcity-0.1.0.tar.gz` & `tmp/python-teamcity-0.1.4.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-teamcity-0.1.0.tar", last modified: Thu Nov 24 14:43:35 2022, max compression
+gzip compressed data, was "python-teamcity-0.1.4.dev6.tar", last modified: Wed May 24 12:29:33 2023, max compression
```

## Comparing `python-teamcity-0.1.0.tar` & `python-teamcity-0.1.4.dev6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.048024 python-teamcity-0.1.0/
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.010522 python-teamcity-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.027001 python-teamcity-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     2852 2022-11-24 14:11:30.000000 python-teamcity-0.1.0/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0       68 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/AUTHORS
--rw-rw-rw-   0        0        0      243 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/ChangeLog
--rw-rw-rw-   0        0        0    35823 2022-11-22 12:21:06.000000 python-teamcity-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      985 2022-11-24 14:43:35.048024 python-teamcity-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       67 2022-11-22 12:21:06.000000 python-teamcity-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.028001 python-teamcity-0.1.0/examples/
--rw-rw-rw-   0        0        0        0 2022-11-22 12:26:55.000000 python-teamcity-0.1.0/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.039510 python-teamcity-0.1.0/python_teamcity.egg-info/
--rw-rw-rw-   0        0        0      985 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/python_teamcity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/python_teamcity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/python_teamcity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-24 14:43:26.000000 python-teamcity-0.1.0/python_teamcity.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/python_teamcity.egg-info/pbr.json
--rw-rw-rw-   0        0        0        9 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/python_teamcity.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-24 14:43:34.000000 python-teamcity-0.1.0/python_teamcity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        8 2022-11-22 12:28:41.000000 python-teamcity-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      838 2022-11-24 14:43:35.049024 python-teamcity-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      133 2022-11-24 14:11:30.000000 python-teamcity-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.045019 python-teamcity-0.1.0/teamcity/
--rw-rw-rw-   0        0        0       31 2022-11-24 14:11:30.000000 python-teamcity-0.1.0/teamcity/__init__.py
--rw-rw-rw-   0        0        0     6102 2022-11-24 14:43:07.000000 python-teamcity-0.1.0/teamcity/teamcity.py
--rw-rw-rw-   0        0        0      237 2022-11-24 14:11:30.000000 python-teamcity-0.1.0/teamcity/teamcity_const.py
-drwxrwxrwx   0        0        0        0 2022-11-24 14:43:35.046019 python-teamcity-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2022-11-22 12:27:14.000000 python-teamcity-0.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.663402 python-teamcity-0.1.4.dev6/
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.626193 python-teamcity-0.1.4.dev6/.github/
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.641824 python-teamcity-0.1.4.dev6/.github/workflows/
+-rw-rw-rw-   0        0        0     2852 2022-11-24 14:11:30.000000 python-teamcity-0.1.4.dev6/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0       68 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/AUTHORS
+-rw-rw-rw-   0        0        0      584 2023-05-24 12:29:32.000000 python-teamcity-0.1.4.dev6/ChangeLog
+-rw-rw-rw-   0        0        0     1088 2022-11-25 05:02:24.000000 python-teamcity-0.1.4.dev6/LICENSE
+-rw-rw-rw-   0        0        0     1025 2023-05-24 12:29:33.664403 python-teamcity-0.1.4.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2022-11-22 12:21:06.000000 python-teamcity-0.1.4.dev6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.644827 python-teamcity-0.1.4.dev6/examples/
+-rw-rw-rw-   0        0        0        0 2022-11-22 12:26:55.000000 python-teamcity-0.1.4.dev6/examples/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-26 07:17:43.000000 python-teamcity-0.1.4.dev6/examples/sample.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.655844 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/
+-rw-rw-rw-   0        0        0     1025 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-01 12:33:48.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/pbr.json
+-rw-rw-rw-   0        0        0        9 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 12:29:33.000000 python-teamcity-0.1.4.dev6/python_teamcity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        8 2022-11-22 12:28:41.000000 python-teamcity-0.1.4.dev6/requirements.txt
+-rw-rw-rw-   0        0        0      880 2023-05-24 12:29:33.664403 python-teamcity-0.1.4.dev6/setup.cfg
+-rw-rw-rw-   0        0        0      133 2022-11-24 14:11:30.000000 python-teamcity-0.1.4.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.660402 python-teamcity-0.1.4.dev6/teamcity/
+-rw-rw-rw-   0        0        0       31 2022-12-28 09:42:30.000000 python-teamcity-0.1.4.dev6/teamcity/__init__.py
+-rw-rw-rw-   0        0        0    12042 2023-05-24 12:25:33.000000 python-teamcity-0.1.4.dev6/teamcity/teamcity.py
+-rw-rw-rw-   0        0        0      237 2022-11-24 14:11:30.000000 python-teamcity-0.1.4.dev6/teamcity/teamcity_const.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:29:33.662411 python-teamcity-0.1.4.dev6/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-22 12:27:14.000000 python-teamcity-0.1.4.dev6/tests/__init__.py
```

### Comparing `python-teamcity-0.1.0/.github/workflows/codeql.yml` & `python-teamcity-0.1.4.dev6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.1.0/PKG-INFO` & `python-teamcity-0.1.4.dev6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.1.0
-Summary: Python API for triggering TeamCity by REST API
+Version: 0.1.4.dev6
+Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
-License: GPL
-Platform: UNKNOWN
+License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 # python-teamcity
 Python API for triggering TeamCity by REST API
 
-
-
```

### Comparing `python-teamcity-0.1.0/python_teamcity.egg-info/PKG-INFO` & `python-teamcity-0.1.4.dev6/python_teamcity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.1.0
-Summary: Python API for triggering TeamCity by REST API
+Version: 0.1.4.dev6
+Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
-License: GPL
-Platform: UNKNOWN
+License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 # python-teamcity
 Python API for triggering TeamCity by REST API
 
-
-
```

### Comparing `python-teamcity-0.1.0/setup.cfg` & `python-teamcity-0.1.4.dev6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 686f 6e2d 7465 616d 6369   = python-teamci
-00000020: 7479 0d0a 7665 7273 696f 6e20 3d20 312e  ty..version = 1.
-00000030: 312e 312e 3131 3232 0d0a 6175 7468 6f72  1.1.1122..author
-00000040: 203d 2059 756e 6c69 6e20 5461 6e0d 0a61   = Yunlin Tan..a
-00000050: 7574 686f 725f 656d 6169 6c20 3d20 7461  uthor_email = ta
-00000060: 6e79 756e 6c69 6e32 3030 3340 6e6f 7262  nyunlin2003@norb
-00000070: 7265 6164 2e63 6f6d 0d0a 7375 6d6d 6172  read.com..summar
-00000080: 7920 3d20 5079 7468 6f6e 2041 5049 2066  y = Python API f
-00000090: 6f72 2074 7269 6767 6572 696e 6720 5465  or triggering Te
-000000a0: 616d 4369 7479 2062 7920 5245 5354 2041  amCity by REST A
-000000b0: 5049 0d0a 6465 7363 7269 7074 696f 6e2d  PI..description-
-000000c0: 6669 6c65 203d 2052 4541 444d 452e 6d64  file = README.md
-000000d0: 0d0a 6c69 6365 6e73 6520 3d20 4750 4c0d  ..license = GPL.
-000000e0: 0a68 6f6d 652d 7061 6765 203d 2068 7474  .home-page = htt
-000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000100: 6e6f 7262 7265 6164 3230 3033 2f70 7974  norbread2003/pyt
-00000110: 686f 6e2d 7465 616d 6369 7479 0d0a 636c  hon-teamcity..cl
-00000120: 6173 7369 6669 6572 203d 200d 0a09 546f  assifier = ...To
-00000130: 7069 6320 3a3a 2055 7469 6c69 7469 6573  pic :: Utilities
-00000140: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-00000150: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000160: 7273 0d0a 0945 6e76 6972 6f6e 6d65 6e74  rs...Environment
-00000170: 203a 3a20 436f 6e73 6f6c 650d 0a09 4c69   :: Console...Li
-00000180: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000190: 726f 7665 6420 3a3a 2047 4e55 2047 656e  roved :: GNU Gen
-000001a0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-000001b0: 6e73 6520 7633 2028 4750 4c76 3329 0d0a  nse v3 (GPLv3)..
-000001c0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-000001d0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001e0: 656e 740d 0a09 5072 6f67 7261 6d6d 696e  ent...Programmin
-000001f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000200: 7468 6f6e 0d0a 0950 726f 6772 616d 6d69  thon...Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e20 3a3a 2033 2e35 0d0a 0950  ython :: 3.5...P
-00000230: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000240: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000250: 2033 2e36 0d0a 0950 726f 6772 616d 6d69   3.6...Programmi
-00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000270: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0950  ython :: 3.7...P
-00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002a0: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
-000002b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002c0: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0950  ython :: 3.9...P
-000002d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002f0: 2033 2e31 300d 0a0d 0a5b 6669 6c65 735d   3.10....[files]
-00000300: 0d0a 7061 636b 6167 6573 203d 200d 0a09  ..packages = ...
-00000310: 7465 616d 6369 7479 0d0a 0d0a 5b65 6767  teamcity....[egg
-00000320: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000330: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000340: 2030 0d0a 0d0a                            0....
+00000020: 7479 0d0a 7665 7273 696f 6e20 3d20 302e  ty..version = 0.
+00000030: 312e 340d 0a61 7574 686f 7220 3d20 5975  1.4..author = Yu
+00000040: 6e6c 696e 2054 616e 0d0a 6175 7468 6f72  nlin Tan..author
+00000050: 5f65 6d61 696c 203d 2074 616e 7975 6e6c  _email = tanyunl
+00000060: 696e 3230 3033 406e 6f72 6272 6561 642e  in2003@norbread.
+00000070: 636f 6d0d 0a73 756d 6d61 7279 203d 2050  com..summary = P
+00000080: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00000090: 7220 7472 6967 6765 7269 6e67 2054 6561  r triggering Tea
+000000a0: 6d43 6974 7920 6279 2052 4553 5420 4150  mCity by REST AP
+000000b0: 490d 0a64 6573 6372 6970 7469 6f6e 2d66  I..description-f
+000000c0: 696c 6520 3d20 5245 4144 4d45 2e6d 640d  ile = README.md.
+000000d0: 0a6c 6963 656e 7365 203d 2047 504c 7633  .license = GPLv3
+000000e0: 0d0a 686f 6d65 2d70 6167 6520 3d20 6874  ..home-page = ht
+000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000100: 2f6e 6f72 6272 6561 6432 3030 332f 7079  /norbread2003/py
+00000110: 7468 6f6e 2d74 6561 6d63 6974 790d 0a63  thon-teamcity..c
+00000120: 6c61 7373 6966 6965 7220 3d20 0d0a 0954  lassifier = ...T
+00000130: 6f70 6963 203a 3a20 5574 696c 6974 6965  opic :: Utilitie
+00000140: 730d 0a09 496e 7465 6e64 6564 2041 7564  s...Intended Aud
+00000150: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000160: 6572 730d 0a09 456e 7669 726f 6e6d 656e  ers...Environmen
+00000170: 7420 3a3a 2043 6f6e 736f 6c65 0d0a 094c  t :: Console...L
+00000180: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000190: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
+000001a0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+000001b0: 656e 7365 2076 3320 2847 504c 7633 290d  ense v3 (GPLv3).
+000001c0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000001d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000001e0: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
+000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000200: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
+00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000220: 5079 7468 6f6e 203a 3a20 332e 350d 0a09  Python :: 3.5...
+00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000250: 3a20 332e 360d 0a09 5072 6f67 7261 6d6d  : 3.6...Programm
+00000260: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000270: 5079 7468 6f6e 203a 3a20 332e 370d 0a09  Python :: 3.7...
+00000280: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000290: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002a0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002c0: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+000002d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002f0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
+00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000310: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
+00000320: 0a0d 0a5b 6669 6c65 735d 0d0a 7061 636b  ...[files]..pack
+00000330: 6167 6573 203d 200d 0a09 7465 616d 6369  ages = ...teamci
+00000340: 7479 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ty....[egg_info]
+00000350: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000360: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

