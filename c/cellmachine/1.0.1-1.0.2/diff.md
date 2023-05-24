# Comparing `tmp/cellmachine-1.0.1.tar.gz` & `tmp/cellmachine-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmachine-1.0.1.tar", max compression
+gzip compressed data, was "cellmachine-1.0.2.tar", max compression
```

## Comparing `cellmachine-1.0.1.tar` & `cellmachine-1.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    35149 2023-05-24 01:51:33.719818 cellmachine-1.0.1/LICENSE
--rw-r--r--   0        0        0       60 2023-05-24 01:51:33.719818 cellmachine-1.0.1/README.md
--rw-r--r--   0        0        0      339 2023-05-24 01:51:33.719818 cellmachine-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       57 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/__init__.py
--rw-r--r--   0        0        0      271 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__init__.py
--rw-r--r--   0        0        0      476 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      890 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
--rw-r--r--   0        0        0     2034 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
--rw-r--r--   0        0        0      885 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
--rw-r--r--   0        0        0      747 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
--rw-r--r--   0        0        0     1229 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
--rw-r--r--   0        0        0      851 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
--rw-r--r--   0        0        0      917 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
--rw-r--r--   0        0        0      561 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
--rw-r--r--   0        0        0      766 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
--rw-r--r--   0        0        0      719 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
--rw-r--r--   0        0        0      538 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/ccw.py
--rw-r--r--   0        0        0     2025 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/cell.py
--rw-r--r--   0        0        0      536 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/cw.py
--rw-r--r--   0        0        0      341 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/enemy.py
--rw-r--r--   0        0        0     1266 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/generator.py
--rw-r--r--   0        0        0      294 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/immobile.py
--rw-r--r--   0        0        0      456 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/mover.py
--rw-r--r--   0        0        0      155 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/push.py
--rw-r--r--   0        0        0      354 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/slide.py
--rw-r--r--   0        0        0      277 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/cells/trash.py
--rw-r--r--   0        0        0     3652 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/level.py
--rw-r--r--   0        0        0      417 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/__init__.py
--rw-r--r--   0        0        0      528 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2145 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
--rw-r--r--   0        0        0     2371 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
--rw-r--r--   0        0        0     2481 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/v1.py
--rw-r--r--   0        0        0     3173 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/v2.py
--rw-r--r--   0        0        0     3528 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/levelstring/v3.py
--rw-r--r--   0        0        0     6148 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/.DS_Store
--rwxr-xr-x   0        0        0      165 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/0.png
--rwxr-xr-x   0        0        0      127 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/BGDefault.png
--rwxr-xr-x   0        0        0      494 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/ccw.png
--rwxr-xr-x   0        0        0      437 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/cw.png
--rwxr-xr-x   0        0        0      429 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/enemy.png
--rwxr-xr-x   0        0        0      522 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/generator.png
--rwxr-xr-x   0        0        0      171 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/immobile.png
--rwxr-xr-x   0        0        0      467 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/mover.png
--rwxr-xr-x   0        0        0      527 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/push.png
--rwxr-xr-x   0        0        0      481 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/slide.png
--rwxr-xr-x   0        0        0      469 2023-05-24 01:51:33.719818 cellmachine-1.0.1/src/cellmachine/textures/trash.png
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-24 22:11:08.716144 cellmachine-1.0.2/LICENSE
+-rw-r--r--   0        0        0       60 2023-05-24 22:11:08.716144 cellmachine-1.0.2/README.md
+-rw-r--r--   0        0        0      339 2023-05-24 22:11:08.716144 cellmachine-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/__init__.py
+-rw-r--r--   0        0        0      271 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__init__.py
+-rw-r--r--   0        0        0      476 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      890 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
+-rw-r--r--   0        0        0      885 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
+-rw-r--r--   0        0        0      747 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
+-rw-r--r--   0        0        0     1229 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
+-rw-r--r--   0        0        0      917 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
+-rw-r--r--   0        0        0      561 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
+-rw-r--r--   0        0        0      766 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
+-rw-r--r--   0        0        0      719 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/ccw.py
+-rw-r--r--   0        0        0     2025 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/cell.py
+-rw-r--r--   0        0        0      536 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/cw.py
+-rw-r--r--   0        0        0      341 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/enemy.py
+-rw-r--r--   0        0        0     1266 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/generator.py
+-rw-r--r--   0        0        0      294 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/immobile.py
+-rw-r--r--   0        0        0      456 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/mover.py
+-rw-r--r--   0        0        0      155 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/push.py
+-rw-r--r--   0        0        0      354 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/slide.py
+-rw-r--r--   0        0        0      277 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/cells/trash.py
+-rw-r--r--   0        0        0     3652 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/level.py
+-rw-r--r--   0        0        0      417 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/levelstring/__init__.py
+-rw-r--r--   0        0        0      528 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2145 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
+-rw-r--r--   0        0        0     2371 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
+-rw-r--r--   0        0        0     2481 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-05-24 22:11:08.716144 cellmachine-1.0.2/src/cellmachine/levelstring/v1.py
+-rw-r--r--   0        0        0     3173 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/levelstring/v2.py
+-rw-r--r--   0        0        0     3528 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/levelstring/v3.py
+-rw-r--r--   0        0        0     6148 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/.DS_Store
+-rwxr-xr-x   0        0        0      165 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/0.png
+-rwxr-xr-x   0        0        0      127 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/BGDefault.png
+-rwxr-xr-x   0        0        0      494 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/ccw.png
+-rwxr-xr-x   0        0        0      437 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/cw.png
+-rwxr-xr-x   0        0        0      429 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/enemy.png
+-rwxr-xr-x   0        0        0      522 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/generator.png
+-rwxr-xr-x   0        0        0      171 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/immobile.png
+-rwxr-xr-x   0        0        0      467 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/mover.png
+-rwxr-xr-x   0        0        0      527 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/push.png
+-rwxr-xr-x   0        0        0      481 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/slide.png
+-rwxr-xr-x   0        0        0      469 2023-05-24 22:11:08.720144 cellmachine-1.0.2/src/cellmachine/textures/trash.png
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.0.2/PKG-INFO
```

### Comparing `cellmachine-1.0.1/LICENSE` & `cellmachine-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/push.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/push.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/ccw.py` & `cellmachine-1.0.2/src/cellmachine/cells/ccw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/cell.py` & `cellmachine-1.0.2/src/cellmachine/cells/cell.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/cw.py` & `cellmachine-1.0.2/src/cellmachine/cells/cw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/cells/generator.py` & `cellmachine-1.0.2/src/cellmachine/cells/generator.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/level.py` & `cellmachine-1.0.2/src/cellmachine/level.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc` & `cellmachine-1.0.2/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/v1.py` & `cellmachine-1.0.2/src/cellmachine/levelstring/v1.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/v2.py` & `cellmachine-1.0.2/src/cellmachine/levelstring/v2.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/levelstring/v3.py` & `cellmachine-1.0.2/src/cellmachine/levelstring/v3.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/textures/.DS_Store` & `cellmachine-1.0.2/src/cellmachine/textures/.DS_Store`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/textures/generator.png` & `cellmachine-1.0.2/src/cellmachine/textures/generator.png`

 * *Files identical despite different names*

### Comparing `cellmachine-1.0.1/src/cellmachine/textures/push.png` & `cellmachine-1.0.2/src/cellmachine/textures/push.png`

 * *Files identical despite different names*

