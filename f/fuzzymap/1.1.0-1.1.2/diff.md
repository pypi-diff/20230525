# Comparing `tmp/fuzzymap-1.1.0.tar.gz` & `tmp/fuzzymap-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzymap-1.1.0.tar", last modified: Fri Apr 28 09:35:37 2023, max compression
+gzip compressed data, was "fuzzymap-1.1.2.tar", last modified: Thu May 25 07:17:26 2023, max compression
```

## Comparing `fuzzymap-1.1.0.tar` & `fuzzymap-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/fuzzymap/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/fuzzymap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/fuzzymap/fuzzymap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/fuzzymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:17:26.847997 fuzzymap-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-25 07:16:51.000000 fuzzymap-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-25 07:17:26.847997 fuzzymap-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-25 07:17:19.000000 fuzzymap-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:17:26.843997 fuzzymap-1.1.2/fuzzymap/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-25 07:16:51.000000 fuzzymap-1.1.2/fuzzymap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-25 07:16:51.000000 fuzzymap-1.1.2/fuzzymap/fuzzymap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:17:26.847997 fuzzymap-1.1.2/fuzzymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-25 07:17:26.000000 fuzzymap-1.1.2/fuzzymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-25 07:17:26.000000 fuzzymap-1.1.2/fuzzymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:17:26.000000 fuzzymap-1.1.2/fuzzymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:17:26.000000 fuzzymap-1.1.2/fuzzymap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 07:17:26.000000 fuzzymap-1.1.2/fuzzymap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 07:17:26.000000 fuzzymap-1.1.2/fuzzymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 07:16:51.000000 fuzzymap-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 07:17:26.847997 fuzzymap-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 07:16:51.000000 fuzzymap-1.1.2/setup.py
```

### Comparing `fuzzymap-1.1.0/LICENSE` & `fuzzymap-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzymap-1.1.0/PKG-INFO` & `fuzzymap-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzymap
-Version: 1.1.0
+Version: 1.1.2
 Summary: The Fuzzy Map is a polymorph Python dictionary that always returns the value of the closest similar key.
 Home-page: https://github.com/pysnippet/fuzzymap
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: GPLv2
 Keywords: python,map,dict,match,fuzzy,matching,dictionary,fuzzywuzzy
 Platform: unix
@@ -29,22 +29,20 @@
 # Fuzzy Map <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/fuzzymap.svg)](https://pypi.org/project/fuzzymap/)
 [![License](https://img.shields.io/pypi/l/fuzzymap.svg?color=blue)](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap?ref=badge_shield)
 [![Tests](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml)
 
-## What is the Fuzzy Map?
-
 The Fuzzy Map is a polymorph Python dictionary that always returns the value of the closest similar key. This kind of
 dictionary returns the value of the exact key if there is such a key. Otherwise, it will return the value of the most
 similar key satisfying the given ratio. The exact mechanism works when setting a new or replacing an old key in the
 dictionary. If the key is not found and does not match any of the keys by the given ratio, it returns none.
 
-## Usage with a real-world example
+## A real-world example
 
 A live data parser collects the coefficients of sports games from different bookmakers at once, and then an analyzer
 tries to find the existing forks. Different bookmakers use different names for the same games. Some of them use the full
 names, and others use names with a partial abbreviation that makes the analyzer's job harder to find and compare the
 coefficients of the same game. Rather this could be hard without `FuzzyMap` that can find the game using the name used
 in one of the sources.
 
@@ -71,20 +69,12 @@
     handle_fork(odds1, odds2)
 ```
 
 In this code example, `source_1` and `source_2` are the dictionary of game and coefficients key-value pairs parsed from
 different sources. And converting the `source_2` dictionary to the `FuzzyMap` dictionary makes it able to find the
 corresponding game using the game's key used in the `source_1` dictionary.
 
-```mermaid
-graph LR
-    src1team1[Rapid Wien - First Vienna] --> src1coefs1["{'w1': 1.93, 'x': 2.32, 'w2': 7.44}"]
-    src1team2[Al Bourj - Al Nejmeh] --> src1coefs2["{'w1': 26, 'x': 11.5, 'w2': 1.05}"]
-    src2team1[SK Rapid Wien - First Vienna FC] --> src2coefs1["{'w1': 1.97, 'x': 2.3, 'w2': 8.2}"]
-    src2team2[Bourj FC - Nejmeh SC Beirut] --> src2coefs2["{'w1': 32, 'x': 12, 'w2': 1.05}"]
-    src1team1 --> src2coefs1
-    src1team2 --> src2coefs2
-```
+<p align="center"><img src="https://user-images.githubusercontent.com/44609997/205437148-4fb3d7bd-1fe9-4ce8-8321-d7aef9488e37.svg" height="400" /></p>
 
 ## License
 
 Copyright (C) 2022 Artyom Vancyan. [GPLv2](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
```

### Comparing `fuzzymap-1.1.0/README.md` & `fuzzymap-1.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # Fuzzy Map <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/fuzzymap.svg)](https://pypi.org/project/fuzzymap/)
 [![License](https://img.shields.io/pypi/l/fuzzymap.svg?color=blue)](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap?ref=badge_shield)
 [![Tests](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml)
 
-## What is the Fuzzy Map?
-
 The Fuzzy Map is a polymorph Python dictionary that always returns the value of the closest similar key. This kind of
 dictionary returns the value of the exact key if there is such a key. Otherwise, it will return the value of the most
 similar key satisfying the given ratio. The exact mechanism works when setting a new or replacing an old key in the
 dictionary. If the key is not found and does not match any of the keys by the given ratio, it returns none.
 
-## Usage with a real-world example
+## A real-world example
 
 A live data parser collects the coefficients of sports games from different bookmakers at once, and then an analyzer
 tries to find the existing forks. Different bookmakers use different names for the same games. Some of them use the full
 names, and others use names with a partial abbreviation that makes the analyzer's job harder to find and compare the
 coefficients of the same game. Rather this could be hard without `FuzzyMap` that can find the game using the name used
 in one of the sources.
 
@@ -43,20 +41,12 @@
     handle_fork(odds1, odds2)
 ```
 
 In this code example, `source_1` and `source_2` are the dictionary of game and coefficients key-value pairs parsed from
 different sources. And converting the `source_2` dictionary to the `FuzzyMap` dictionary makes it able to find the
 corresponding game using the game's key used in the `source_1` dictionary.
 
-```mermaid
-graph LR
-    src1team1[Rapid Wien - First Vienna] --> src1coefs1["{'w1': 1.93, 'x': 2.32, 'w2': 7.44}"]
-    src1team2[Al Bourj - Al Nejmeh] --> src1coefs2["{'w1': 26, 'x': 11.5, 'w2': 1.05}"]
-    src2team1[SK Rapid Wien - First Vienna FC] --> src2coefs1["{'w1': 1.97, 'x': 2.3, 'w2': 8.2}"]
-    src2team2[Bourj FC - Nejmeh SC Beirut] --> src2coefs2["{'w1': 32, 'x': 12, 'w2': 1.05}"]
-    src1team1 --> src2coefs1
-    src1team2 --> src2coefs2
-```
+<p align="center"><img src="https://user-images.githubusercontent.com/44609997/205437148-4fb3d7bd-1fe9-4ce8-8321-d7aef9488e37.svg" height="400" /></p>
 
 ## License
 
 Copyright (C) 2022 Artyom Vancyan. [GPLv2](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
```

### Comparing `fuzzymap-1.1.0/fuzzymap/__init__.py` & `fuzzymap-1.1.2/fuzzymap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 __all__ = ('FuzzyMap',)
-__version__ = '1.1.0'
+__version__ = '1.1.2'
```

### Comparing `fuzzymap-1.1.0/fuzzymap/fuzzymap.py` & `fuzzymap-1.1.2/fuzzymap/fuzzymap.py`

 * *Files identical despite different names*

### Comparing `fuzzymap-1.1.0/fuzzymap.egg-info/PKG-INFO` & `fuzzymap-1.1.2/fuzzymap.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzymap
-Version: 1.1.0
+Version: 1.1.2
 Summary: The Fuzzy Map is a polymorph Python dictionary that always returns the value of the closest similar key.
 Home-page: https://github.com/pysnippet/fuzzymap
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: GPLv2
 Keywords: python,map,dict,match,fuzzy,matching,dictionary,fuzzywuzzy
 Platform: unix
@@ -29,22 +29,20 @@
 # Fuzzy Map <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/fuzzymap.svg)](https://pypi.org/project/fuzzymap/)
 [![License](https://img.shields.io/pypi/l/fuzzymap.svg?color=blue)](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap?ref=badge_shield)
 [![Tests](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml)
 
-## What is the Fuzzy Map?
-
 The Fuzzy Map is a polymorph Python dictionary that always returns the value of the closest similar key. This kind of
 dictionary returns the value of the exact key if there is such a key. Otherwise, it will return the value of the most
 similar key satisfying the given ratio. The exact mechanism works when setting a new or replacing an old key in the
 dictionary. If the key is not found and does not match any of the keys by the given ratio, it returns none.
 
-## Usage with a real-world example
+## A real-world example
 
 A live data parser collects the coefficients of sports games from different bookmakers at once, and then an analyzer
 tries to find the existing forks. Different bookmakers use different names for the same games. Some of them use the full
 names, and others use names with a partial abbreviation that makes the analyzer's job harder to find and compare the
 coefficients of the same game. Rather this could be hard without `FuzzyMap` that can find the game using the name used
 in one of the sources.
 
@@ -71,20 +69,12 @@
     handle_fork(odds1, odds2)
 ```
 
 In this code example, `source_1` and `source_2` are the dictionary of game and coefficients key-value pairs parsed from
 different sources. And converting the `source_2` dictionary to the `FuzzyMap` dictionary makes it able to find the
 corresponding game using the game's key used in the `source_1` dictionary.
 
-```mermaid
-graph LR
-    src1team1[Rapid Wien - First Vienna] --> src1coefs1["{'w1': 1.93, 'x': 2.32, 'w2': 7.44}"]
-    src1team2[Al Bourj - Al Nejmeh] --> src1coefs2["{'w1': 26, 'x': 11.5, 'w2': 1.05}"]
-    src2team1[SK Rapid Wien - First Vienna FC] --> src2coefs1["{'w1': 1.97, 'x': 2.3, 'w2': 8.2}"]
-    src2team2[Bourj FC - Nejmeh SC Beirut] --> src2coefs2["{'w1': 32, 'x': 12, 'w2': 1.05}"]
-    src1team1 --> src2coefs1
-    src1team2 --> src2coefs2
-```
+<p align="center"><img src="https://user-images.githubusercontent.com/44609997/205437148-4fb3d7bd-1fe9-4ce8-8321-d7aef9488e37.svg" height="400" /></p>
 
 ## License
 
 Copyright (C) 2022 Artyom Vancyan. [GPLv2](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
```

### Comparing `fuzzymap-1.1.0/setup.cfg` & `fuzzymap-1.1.2/setup.cfg`

 * *Files identical despite different names*

