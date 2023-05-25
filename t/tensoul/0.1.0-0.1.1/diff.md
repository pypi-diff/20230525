# Comparing `tmp/tensoul-0.1.0.tar.gz` & `tmp/tensoul-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensoul-0.1.0.tar", max compression
+gzip compressed data, was "tensoul-0.1.1.tar", max compression
```

## Comparing `tensoul-0.1.0.tar` & `tensoul-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      445 2023-05-25 07:38:45.749922 tensoul-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.0/README.md
--rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.0/tensoul/__init__.py
--rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.0/tensoul/cfg.json
--rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.0/tensoul/cfg.py
--rw-r--r--   0        0        0     2037 2023-05-24 15:36:27.100839 tensoul-0.1.0/tensoul/constants.py
--rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.0/tensoul/downloader.py
--rw-r--r--   0        0        0     9724 2023-05-25 04:10:00.181589 tensoul-0.1.0/tensoul/model.py
--rw-r--r--   0        0        0    14196 2023-05-25 03:22:05.532662 tensoul-0.1.0/tensoul/parser.py
--rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.0/tensoul/utils.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      445 2023-05-25 14:41:30.799701 tensoul-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.1/tensoul/__init__.py
+-rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.1/tensoul/cfg.json
+-rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.1/tensoul/cfg.py
+-rw-r--r--   0        0        0     2037 2023-05-24 15:36:27.100839 tensoul-0.1.1/tensoul/constants.py
+-rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.1/tensoul/downloader.py
+-rw-r--r--   0        0        0     9745 2023-05-25 14:38:55.766711 tensoul-0.1.1/tensoul/model.py
+-rw-r--r--   0        0        0    14196 2023-05-25 03:22:05.532662 tensoul-0.1.1/tensoul/parser.py
+-rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.1/tensoul/utils.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.1/PKG-INFO
```

### Comparing `tensoul-0.1.0/README.md` & `tensoul-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.0/tensoul/cfg.json` & `tensoul-0.1.1/tensoul/cfg.json`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.0/tensoul/constants.py` & `tensoul-0.1.1/tensoul/constants.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.0/tensoul/downloader.py` & `tensoul-0.1.1/tensoul/downloader.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.0/tensoul/model.py` & `tensoul-0.1.1/tensoul/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from enum import IntEnum
-from typing import NamedTuple, Union, Protocol, Optional, Sequence, runtime_checkable
+from typing import NamedTuple, Union, Protocol, Optional, Sequence
 
 from .cfg import cfg
 from .constants import TSUMOGIRI, RUNES, JPNAME
 from .utils import pad_list
 
 
 class TileType(IntEnum):
@@ -99,20 +99,17 @@
     """
     a: Tile
     b: Tile
     tile: Tile
     feeder_relative: int
 
     def encode_tenhou(self) -> str:
-        s = ""
-        for i in range(3):
-            if i == self.feeder_relative:
-                s += "p"
-            s += str(self[i].encode_tenhou())
-        return s
+        t = [str(self.a.encode_tenhou()), str(self.b.encode_tenhou())]
+        t.insert(self.feeder_relative, f"p{self.tile.encode_tenhou()}")
+        return "".join(t)
 
 
 class DaiminkanSymbol(NamedTuple):
     """
     a, b, c: 手里牌
     tile: 喂牌
     """
@@ -123,20 +120,17 @@
     feeder_relative: int
 
     def encode_tenhou(self) -> str:
         pos = self.feeder_relative
         if pos == 2:
             pos = 3
 
-        s = ""
-        for i in range(4):
-            if i == pos:
-                s += "m"
-            s += str(self[i].encode_tenhou())
-        return s
+        t = [str(self.a.encode_tenhou()), str(self.b.encode_tenhou()), str(self.c.encode_tenhou())]
+        t.insert(pos, f"m{self.tile.encode_tenhou()}")
+        return "".join(t)
 
 
 class AnkanSymbol(NamedTuple):
     tile: Tile
 
     def encode_tenhou(self) -> str:
         t = self.tile.encode_tenhou()
@@ -164,20 +158,17 @@
     feeder_relative: int
 
     def encode_tenhou(self) -> str:
         pos = self.feeder_relative
         if pos == 2:
             pos = 3
 
-        s = ""
-        for i in range(4):
-            if i == pos:
-                s += "k"
-            s += str(self[i].encode_tenhou())
-        return s
+        t = [str(self.a.encode_tenhou()), str(self.b.encode_tenhou()), str(self.c.encode_tenhou())]
+        t.insert(pos, f"k{self.tile.encode_tenhou()}")
+        return "".join(t)
 
 
 class Round(NamedTuple):
     kyoku: int
     honba: int
     riichi_sticks: int
```

### Comparing `tensoul-0.1.0/tensoul/parser.py` & `tensoul-0.1.1/tensoul/parser.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.0/PKG-INFO` & `tensoul-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensoul
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

