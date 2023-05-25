# Comparing `tmp/all-fives-domino-1.0.3.tar.gz` & `tmp/all-fives-domino-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all-fives-domino-1.0.3.tar", last modified: Thu May 25 20:40:20 2023, max compression
+gzip compressed data, was "all-fives-domino-1.0.4.tar", last modified: Thu May 25 21:11:03 2023, max compression
```

## Comparing `all-fives-domino-1.0.3.tar` & `all-fives-domino-1.0.4.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-25 20:40:02.000000 all-fives-domino-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.176983 all-fives-domino-1.0.3/all_fives_domino.egg-info/
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-25 20:40:20.000000 all-fives-domino-1.0.3/all_fives_domino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-25 20:40:20.000000 all-fives-domino-1.0.3/all_fives_domino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 20:40:20.000000 all-fives-domino-1.0.3/all_fives_domino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-25 20:40:20.000000 all-fives-domino-1.0.3/all_fives_domino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.176983 all-fives-domino-1.0.3/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.176983 all-fives-domino-1.0.3/src/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.176983 all-fives-domino-1.0.3/src/main/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.176983 all-fives-domino-1.0.3/src/main/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/main/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.176983 all-fives-domino-1.0.3/src/main/game/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/main/game/DominoRound.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/main/game/Piece.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/main/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/src/main/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     3474 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/main/game/__pycache__/Piece.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/main/game/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/src/main/player/
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/main/player/Player.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/main/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/src/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/src/test/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/test/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/src/test/game/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/test/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:40:20.180983 all-fives-domino-1.0.3/src/test/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/test/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 20:34:42.000000 all-fives-domino-1.0.3/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 20:33:44.000000 all-fives-domino-1.0.3/src/test/game/test_pieces.py
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-25 20:40:03.000000 all-fives-domino-1.0.3/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.141143 all-fives-domino-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      814 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-25 21:10:49.000000 all-fives-domino-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/all_fives_domino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      814 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 21:11:03.141143 all-fives-domino-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/main/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/main/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/main/game/
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/game/DominoRound.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/game/Piece.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/main/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/main/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-25 21:10:48.000000 all-fives-domino-1.0.4/src/main/game/__pycache__/Piece.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/main/game/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/main/player/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/player/Brain.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/player/Hand.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/player/Player.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/main/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/test/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/game/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/test/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/test/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/test/game/test_pieces.py
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-25 21:10:50.000000 all-fives-domino-1.0.4/version.txt
```

### Comparing `all-fives-domino-1.0.3/LICENSE` & `all-fives-domino-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.3/PKG-INFO` & `all-fives-domino-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.3
+Version: 1.0.4
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
 ![image](https://img.shields.io/static/v1?label=pytest&message=1+failed%2C+1+tests&color=critical&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=63%25&color=yellow&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=32%25&color=orange&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.3/all_fives_domino.egg-info/PKG-INFO` & `all-fives-domino-1.0.4/all_fives_domino.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.3
+Version: 1.0.4
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
 ![image](https://img.shields.io/static/v1?label=pytest&message=1+failed%2C+1+tests&color=critical&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=63%25&color=yellow&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=32%25&color=orange&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.3/all_fives_domino.egg-info/SOURCES.txt` & `all-fives-domino-1.0.4/all_fives_domino.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 src/main/__init__.py
 src/main/__pycache__/__init__.cpython-311.pyc
 src/main/game/DominoRound.py
 src/main/game/Piece.py
 src/main/game/__init__.py
 src/main/game/__pycache__/Piece.cpython-311.pyc
 src/main/game/__pycache__/__init__.cpython-311.pyc
+src/main/player/Brain.py
+src/main/player/Hand.py
 src/main/player/Player.py
 src/main/player/__init__.py
 src/test/__init__.py
 src/test/__pycache__/__init__.cpython-311.pyc
 src/test/game/__init__.py
 src/test/game/test_pieces.py
 src/test/game/__pycache__/__init__.cpython-311.pyc
```

### Comparing `all-fives-domino-1.0.3/setup.py` & `all-fives-domino-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.3/src/main/game/Piece.py` & `all-fives-domino-1.0.4/src/main/game/Piece.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,27 +7,26 @@
         Constructor
 
         a: int                  -> First number on the piece
         b: int                  -> Second number on the piece
 
         linked: List[Piece]     -> Pieces played from this Piece
         is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece
+        is_double: Bool         -> Whether both sides of the piece show the same number
+        points: int             -> Point value of the piece, which is the combined value of both sides
         """
         self.sides = sorted([a, b])
         self.linked: List[Piece] = []
         self.is_crossing = False
+        self.is_double = self.sides[0] == self.sides[1]
+        self.points = sum(self.sides)
 
     def append(self, piece):
         self.linked.append(piece)
 
-    @property
-    def points(self):
-        """Returns the point value of the piece, which is the combined value of both sides"""
-        return sum(self.sides)
-
     def __repr__(self):
         """Simple visual representation, e.g. [4|6]"""
         return f"[{self.sides[0]}|{self.sides[1]}]"
 
     def __hash__(self):
         """Integer representation, e.g. 64 for a [4|6] piece"""
         return self.sides[1] * 10 + self.sides[0]
@@ -48,11 +47,7 @@
 def domino_set():
     pieces = set()
     for i in range(7):
         for j in range(7):
             if i <= j:
                 pieces.add(Piece(i, j))
     return sorted(pieces)
-
-
-if __name__ == '__main__':
-    print(domino_set())
```

### Comparing `all-fives-domino-1.0.3/src/main/game/__pycache__/Piece.cpython-311.pyc` & `all-fives-domino-1.0.4/src/main/game/__pycache__/Piece.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,18 @@
 magic:    0xa70d0d0a
-moddate:  0x28c66f64 (Thu May 25 20:33:44 2023 UTC)
-files sz: 1671
+moddate:  0xd1ce6f64 (Thu May 25 21:10:41 2023 UTC)
+files sz: 1741
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a01010002004700640284006403a6020000ab
-      0200000000000000005a02640484005a03650464056b0200000000721502
-      00650502006503a6000000ab000000000000000000a6010000ab01000000
-      000000000001006406530064065300
+      0200000000000000005a02640484005a0364055300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('List',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
                 10 STORE_NAME               1 (List)
@@ -25,49 +23,31 @@
                 18 LOAD_CONST               2 (<code object Piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('Piece')
                 24 PRECALL                  2
                 28 CALL                     2
                 38 STORE_NAME               2 (Piece)
    
-    48          40 LOAD_CONST               4 (<code object domino_set, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 48>)
+    47          40 LOAD_CONST               4 (<code object domino_set, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 47>)
                 42 MAKE_FUNCTION            0
                 44 STORE_NAME               3 (domino_set)
-   
-    57          46 LOAD_NAME                4 (__name__)
-                48 LOAD_CONST               5 ('__main__')
-                50 COMPARE_OP               2 (==)
-                56 POP_JUMP_FORWARD_IF_FALSE    21 (to 100)
-   
-    58          58 PUSH_NULL
-                60 LOAD_NAME                5 (print)
-                62 PUSH_NULL
-                64 LOAD_NAME                3 (domino_set)
-                66 PRECALL                  0
-                70 CALL                     0
-                80 PRECALL                  1
-                84 CALL                     1
-                94 POP_TOP
-                96 LOAD_CONST               6 (None)
-                98 RETURN_VALUE
-   
-    57     >>  100 LOAD_CONST               6 (None)
-               102 RETURN_VALUE
+                46 LOAD_CONST               5 (None)
+                48 RETURN_VALUE
    consts
       0
       ('List',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264016503640265036604640384045a04640484
-            005a05650664058400a6000000ab0000000000000000005a07640684005a
-            08640784005a09640884005a0a640984005a0b640a84005a0c640b5300
+            005a05640584005a06640684005a07640784005a08640884005a09640984
+            005a0a640a5300
            4           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Piece')
                        8 STORE_NAME               2 (__qualname__)
          
            5          10 LOAD_CONST               1 ('a')
@@ -75,105 +55,121 @@
                       14 LOAD_CONST               2 ('b')
                       16 LOAD_NAME                3 (int)
                       18 BUILD_TUPLE              4
                       20 LOAD_CONST               3 (<code object __init__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 5>)
                       22 MAKE_FUNCTION            4 (annotations)
                       24 STORE_NAME               4 (__init__)
          
-          19          26 LOAD_CONST               4 (<code object append, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 19>)
+          23          26 LOAD_CONST               4 (<code object append, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 23>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (append)
          
-          22          32 LOAD_NAME                6 (property)
-         
-          23          34 LOAD_CONST               5 (<code object points, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 22>)
-                      36 MAKE_FUNCTION            0
-         
-          22          38 PRECALL                  0
-                      42 CALL                     0
-         
-          23          52 STORE_NAME               7 (points)
-         
-          27          54 LOAD_CONST               6 (<code object __repr__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 27>)
-                      56 MAKE_FUNCTION            0
-                      58 STORE_NAME               8 (__repr__)
-         
-          31          60 LOAD_CONST               7 (<code object __hash__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 31>)
-                      62 MAKE_FUNCTION            0
-                      64 STORE_NAME               9 (__hash__)
-         
-          35          66 LOAD_CONST               8 (<code object __eq__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 35>)
-                      68 MAKE_FUNCTION            0
-                      70 STORE_NAME              10 (__eq__)
-         
-          39          72 LOAD_CONST               9 (<code object __lt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 39>)
-                      74 MAKE_FUNCTION            0
-                      76 STORE_NAME              11 (__lt__)
-         
-          43          78 LOAD_CONST              10 (<code object __gt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 43>)
-                      80 MAKE_FUNCTION            0
-                      82 STORE_NAME              12 (__gt__)
-                      84 LOAD_CONST              11 (None)
-                      86 RETURN_VALUE
+          26          32 LOAD_CONST               5 (<code object __repr__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 26>)
+                      34 MAKE_FUNCTION            0
+                      36 STORE_NAME               6 (__repr__)
+         
+          30          38 LOAD_CONST               6 (<code object __hash__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 30>)
+                      40 MAKE_FUNCTION            0
+                      42 STORE_NAME               7 (__hash__)
+         
+          34          44 LOAD_CONST               7 (<code object __eq__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 34>)
+                      46 MAKE_FUNCTION            0
+                      48 STORE_NAME               8 (__eq__)
+         
+          38          50 LOAD_CONST               8 (<code object __lt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 38>)
+                      52 MAKE_FUNCTION            0
+                      54 STORE_NAME               9 (__lt__)
+         
+          42          56 LOAD_CONST               9 (<code object __gt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 42>)
+                      58 MAKE_FUNCTION            0
+                      60 STORE_NAME              10 (__gt__)
+                      62 LOAD_CONST              10 (None)
+                      64 RETURN_VALUE
          consts
             'Piece'
             'a'
             'b'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c017c026702a6010000ab01000000
                   00000000007c005f01000000000000000067007c005f0200000000000000
-                  0064017c005f03000000000000000064025300
+                  0064017c005f0300000000000000007c006a010000000000000000640219
+                  0000000000000000007c006a010000000000000000640319000000000000
+                  0000006b02000000007c005f040000000000000000740b00000000000000
+                  0000007c006a010000000000000000a6010000ab0100000000000000007c
+                  005f06000000000000000064045300
                  5           0 RESUME                   0
                
-                15           2 LOAD_GLOBAL              1 (NULL + sorted)
+                17           2 LOAD_GLOBAL              1 (NULL + sorted)
                             14 LOAD_FAST                1 (a)
                             16 LOAD_FAST                2 (b)
                             18 BUILD_LIST               2
                             20 PRECALL                  1
                             24 CALL                     1
                             34 LOAD_FAST                0 (self)
                             36 STORE_ATTR               1 (sides)
                
-                16          46 BUILD_LIST               0
+                18          46 BUILD_LIST               0
                             48 LOAD_FAST                0 (self)
                             50 STORE_ATTR               2 (linked)
                
-                17          60 LOAD_CONST               1 (False)
+                19          60 LOAD_CONST               1 (False)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               3 (is_crossing)
-                            74 LOAD_CONST               2 (None)
-                            76 RETURN_VALUE
+               
+                20          74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                1 (sides)
+                            86 LOAD_CONST               2 (0)
+                            88 BINARY_SUBSCR
+                            98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                1 (sides)
+                           110 LOAD_CONST               3 (1)
+                           112 BINARY_SUBSCR
+                           122 COMPARE_OP               2 (==)
+                           128 LOAD_FAST                0 (self)
+                           130 STORE_ATTR               4 (is_double)
+               
+                21         140 LOAD_GLOBAL             11 (NULL + sum)
+                           152 LOAD_FAST                0 (self)
+                           154 LOAD_ATTR                1 (sides)
+                           164 PRECALL                  1
+                           168 CALL                     1
+                           178 LOAD_FAST                0 (self)
+                           180 STORE_ATTR               6 (points)
+                           190 LOAD_CONST               4 (None)
+                           192 RETURN_VALUE
                consts
-                  '\n        Constructor\n\n        a: int                  -> First number on the piece\n        b: int                  -> Second number on the piece\n\n        linked: List[Piece]     -> Pieces played from this Piece\n        is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece\n        '
+                  '\n        Constructor\n\n        a: int                  -> First number on the piece\n        b: int                  -> Second number on the piece\n\n        linked: List[Piece]     -> Pieces played from this Piece\n        is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece\n        is_double: Bool         -> Whether both sides of the piece show the same number\n        points: int             -> Point value of the piece, which is the combined value of both sides\n        '
                   False
+                  0
+                  1
                   None
-               names      ('sorted', 'sides', 'linked', 'is_crossing')
+               names      ('sorted', 'sides', 'linked', 'is_crossing', 'is_double', 'sum', 'points')
                varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__init__'
                firstlineno 5
-               lnotab 0x020a2c010e01
+               lnotab 0x020c2c010e010e014201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-                19           0 RESUME                   0
+                23           0 RESUME                   0
                
-                20           2 LOAD_FAST                0 (self)
+                24           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (linked)
                             14 LOAD_METHOD              1 (append)
                             36 LOAD_FAST                1 (piece)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
@@ -182,54 +178,28 @@
                   None
                names      ('linked', 'append')
                varnames   ('self', 'piece')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       'append'
-               firstlineno 19
+               firstlineno 23
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 3
-               flags     : 3
-               code
-                  0x97007401000000000000000000007c006a010000000000000000a60100
-                  00ab0100000000000000005300
-                22           0 RESUME                   0
-               
-                25           2 LOAD_GLOBAL              1 (NULL + sum)
-                            14 LOAD_FAST                0 (self)
-                            16 LOAD_ATTR                1 (sides)
-                            26 PRECALL                  1
-                            30 CALL                     1
-                            40 RETURN_VALUE
-               consts
-                  'Returns the point value of the piece, which is the combined value of both sides'
-               names      ('sum', 'sides')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
-               name       'points'
-               firstlineno 22
-               lnotab 0x0203
-            code
-               argcount  : 1
-               nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x970064017c006a0000000000000000006402190000000000000000009b
                   0064037c006a0000000000000000006404190000000000000000009b0064
                   059d055300
-                27           0 RESUME                   0
+                26           0 RESUME                   0
                
-                29           2 LOAD_CONST               1 ('[')
+                28           2 LOAD_CONST               1 ('[')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (sides)
                             16 LOAD_CONST               2 (0)
                             18 BINARY_SUBSCR
                             28 FORMAT_VALUE             0
                             30 LOAD_CONST               3 ('|')
                             32 LOAD_FAST                0 (self)
@@ -249,28 +219,28 @@
                   ']'
                names      ('sides',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__repr__'
-               firstlineno 27
+               firstlineno 26
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a00000000000000000064011900000000000000000064027a
                   0500007c006a0000000000000000006403190000000000000000007a0000
                   005300
-                31           0 RESUME                   0
+                30           0 RESUME                   0
                
-                33           2 LOAD_FAST                0 (self)
+                32           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sides)
                             14 LOAD_CONST               1 (1)
                             16 BINARY_SUBSCR
                             26 LOAD_CONST               2 (10)
                             28 BINARY_OP                5 (*)
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                0 (sides)
@@ -285,28 +255,28 @@
                   0
                names      ('sides',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__hash__'
-               firstlineno 31
+               firstlineno 30
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   007401000000000000000000007c01a6010000ab0100000000000000006b
                   02000000005300
-                35           0 RESUME                   0
+                34           0 RESUME                   0
                
-                37           2 LOAD_GLOBAL              1 (NULL + hash)
+                36           2 LOAD_GLOBAL              1 (NULL + hash)
                             14 LOAD_FAST                0 (self)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_GLOBAL              1 (NULL + hash)
                             42 LOAD_FAST                1 (other)
                             44 PRECALL                  1
                             48 CALL                     1
@@ -316,77 +286,77 @@
                   'Returns whether the pieces are equal based on their hash'
                names      ('hash',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__eq__'
-               firstlineno 35
+               firstlineno 34
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a0000000000000000006b0000
                   0000005300
-                39           0 RESUME                   0
+                38           0 RESUME                   0
                
-                41           2 LOAD_FAST                0 (self)
+                40           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (points)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_ATTR                0 (points)
                             26 COMPARE_OP               0 (<)
                             32 RETURN_VALUE
                consts
                   'Returns whether a piece is bigger based on point value'
                names      ('points',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__lt__'
-               firstlineno 39
+               firstlineno 38
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a0000000000000000006b0400
                   0000005300
-                43           0 RESUME                   0
+                42           0 RESUME                   0
                
-                45           2 LOAD_FAST                0 (self)
+                44           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (points)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_ATTR                0 (points)
                             26 COMPARE_OP               4 (>)
                             32 RETURN_VALUE
                consts
                   'Returns whether a piece is smaller based on point value'
                names      ('points',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__gt__'
-               firstlineno 43
+               firstlineno 42
                lnotab 0x0202
             None
-         names      ('__name__', '__module__', '__qualname__', 'int', '__init__', 'append', 'property', 'points', '__repr__', '__hash__', '__eq__', '__lt__', '__gt__')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__init__', 'append', '__repr__', '__hash__', '__eq__', '__lt__', '__gt__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
          name       'Piece'
          firstlineno 4
-         lnotab 0x0a01100e0603020104ff0e0102040604060406040604
+         lnotab 0x0a01101206030604060406040604
       'Piece'
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 8
          flags     : 3
          code
@@ -394,75 +364,74 @@
             007403000000000000000000006401a6010000ab01000000000000000044
             005d3d7d017403000000000000000000006401a6010000ab010000000000
             00000044005d2b7d027c017c026b010000000072237c00a0020000000000
             0000000000000000000000000000007407000000000000000000007c017c
             02a6020000ab020000000000000000a6010000ab01000000000000000001
             008c2c8c3e7409000000000000000000007c00a6010000ab010000000000
             0000005300
-          48           0 RESUME                   0
+          47           0 RESUME                   0
          
-          49           2 LOAD_GLOBAL              1 (NULL + set)
+          48           2 LOAD_GLOBAL              1 (NULL + set)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               0 (pieces)
          
-          50          30 LOAD_GLOBAL              3 (NULL + range)
+          49          30 LOAD_GLOBAL              3 (NULL + range)
                       42 LOAD_CONST               1 (7)
                       44 PRECALL                  1
                       48 CALL                     1
                       58 GET_ITER
                  >>   60 FOR_ITER                61 (to 184)
                       62 STORE_FAST               1 (i)
          
-          51          64 LOAD_GLOBAL              3 (NULL + range)
+          50          64 LOAD_GLOBAL              3 (NULL + range)
                       76 LOAD_CONST               1 (7)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 GET_ITER
                  >>   94 FOR_ITER                43 (to 182)
                       96 STORE_FAST               2 (j)
          
-          52          98 LOAD_FAST                1 (i)
+          51          98 LOAD_FAST                1 (i)
                      100 LOAD_FAST                2 (j)
                      102 COMPARE_OP               1 (<=)
                      108 POP_JUMP_FORWARD_IF_FALSE    35 (to 180)
          
-          53         110 LOAD_FAST                0 (pieces)
+          52         110 LOAD_FAST                0 (pieces)
                      112 LOAD_METHOD              2 (add)
                      134 LOAD_GLOBAL              7 (NULL + Piece)
                      146 LOAD_FAST                1 (i)
                      148 LOAD_FAST                2 (j)
                      150 PRECALL                  2
                      154 CALL                     2
                      164 PRECALL                  1
                      168 CALL                     1
                      178 POP_TOP
                  >>  180 JUMP_BACKWARD           44 (to 94)
          
-          51     >>  182 JUMP_BACKWARD           62 (to 60)
+          50     >>  182 JUMP_BACKWARD           62 (to 60)
          
-          54     >>  184 LOAD_GLOBAL              9 (NULL + sorted)
+          53     >>  184 LOAD_GLOBAL              9 (NULL + sorted)
                      196 LOAD_FAST                0 (pieces)
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RETURN_VALUE
          consts
             None
             7
          names      ('set', 'range', 'add', 'Piece', 'sorted')
          varnames   ('pieces', 'i', 'j')
          freevars   ()
          cellvars   ()
          filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
          name       'domino_set'
-         firstlineno 48
+         firstlineno 47
          lnotab 0x02011c01220122010c0148fe0203
-      '__main__'
       None
-   names      ('typing', 'List', 'Piece', 'domino_set', '__name__', 'print')
+   names      ('typing', 'List', 'Piece', 'domino_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c031a2c06090c012aff
+   lnotab 0x00ff02010c031a2b
```

### Comparing `all-fives-domino-1.0.3/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.4/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

