# Comparing `tmp/olympipe-1.1.8.tar.gz` & `tmp/olympipe-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympipe-1.1.8.tar", max compression
+gzip compressed data, was "olympipe-1.1.9.tar", max compression
```

## Comparing `olympipe-1.1.8.tar` & `olympipe-1.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-05-23 07:04:07.327230 olympipe-1.1.8/LICENSE
--rw-r--r--   0        0        0     3887 2023-05-23 07:04:07.330230 olympipe-1.1.8/README.md
--rw-r--r--   0        0        0    10513 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/dispatcher.py
--rw-r--r--   0        0        0        0 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/__init__.py
--rw-r--r--   0        0        0     1718 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/batch.py
--rw-r--r--   0        0        0      530 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/explode.py
--rw-r--r--   0        0        0      524 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/filter.py
--rw-r--r--   0        0        0     2428 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/generic.py
--rw-r--r--   0        0        0     1649 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/instance.py
--rw-r--r--   0        0        0     1180 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/reduce.py
--rw-r--r--   0        0        0      408 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/task.py
--rw-r--r--   0        0        0     1899 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/timebatch.py
--rw-r--r--   0        0        0        0 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/py.typed
--rw-r--r--   0        0        0      646 2023-05-23 07:04:07.330230 olympipe-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-23 20:52:54.717589 olympipe-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3887 2023-05-23 20:52:54.719590 olympipe-1.1.9/README.md
+-rw-r--r--   0        0        0    10652 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/dispatcher.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/__init__.py
+-rw-r--r--   0        0        0     1718 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/batch.py
+-rw-r--r--   0        0        0      530 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/explode.py
+-rw-r--r--   0        0        0      524 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/filter.py
+-rw-r--r--   0        0        0     2508 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/generic.py
+-rw-r--r--   0        0        0     1649 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/instance.py
+-rw-r--r--   0        0        0     1180 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/reduce.py
+-rw-r--r--   0        0        0      408 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/task.py
+-rw-r--r--   0        0        0     1899 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/timebatch.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/py.typed
+-rw-r--r--   0        0        0      646 2023-05-23 20:52:54.720589 olympipe-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.9/PKG-INFO
```

### Comparing `olympipe-1.1.8/LICENSE` & `olympipe-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/README.md` & `olympipe-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/__init__.py` & `olympipe-1.1.9/olympipe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __version__ = "1.1.1"
 
 from multiprocessing import Process, Queue, TimeoutError
+from queue import Empty, Full
 from threading import Timer
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
@@ -248,14 +249,18 @@
                     packet = output_queue.get(timeout=0.1)
                     if GenericPipe.is_death_packet(packet):
                         output_queues[i] = None
                     else:
                         outputs[i].append(packet)
                 except TimeoutError:
                     pass
+                except Full:
+                    pass
+                except Empty:
+                    pass
                 except Exception as e:
                     print("Error waiting:", e)
 
         return outputs
 
     def wait_for_completion(
         self, other_pipes: List["Pipeline[Any]"] = [], debug_graph: Optional[str] = None
```

### Comparing `olympipe-1.1.8/olympipe/dispatcher.py` & `olympipe-1.1.9/olympipe/dispatcher.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/pipes/batch.py` & `olympipe-1.1.9/olympipe/pipes/batch.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/pipes/explode.py` & `olympipe-1.1.9/olympipe/pipes/explode.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/pipes/filter.py` & `olympipe-1.1.9/olympipe/pipes/filter.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/pipes/generic.py` & `olympipe-1.1.9/olympipe/pipes/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import multiprocessing
-import queue
 import time
 from multiprocessing import Process, Queue
-from queue import Empty
+from queue import Empty, Full
 from threading import Timer
 from typing import Any, Generic, Optional, Tuple, TypeVar, cast
 
 R = TypeVar("R")
 S = TypeVar("S")
 
 
@@ -58,25 +57,29 @@
     def _send_to_next(self, processed: S):
         while True:
             try:
                 self._target.put(processed, timeout=self._timeout)
                 break
             except multiprocessing.TimeoutError:
                 pass
+            except Full:
+                pass
+            except Empty:
+                pass
             except Exception as e:
                 print("Error sending:", e)
 
     def run(self):
         while True:
             try:
                 data = self._source.get(timeout=self._timeout)
                 if GenericPipe.is_death_packet(data):
                     self._kill(data)
                     return
                 processed = self._perform_task(data)
                 self._send_to_next(processed)
-            except queue.Empty:
+            except Empty:
                 continue
             except Exception as e:
                 self._kill(GenericPipe.get_kill_word(), True)
                 print(f"Error_{e.__class__.__name__}_{e.args}")
                 return
```

### Comparing `olympipe-1.1.8/olympipe/pipes/instance.py` & `olympipe-1.1.9/olympipe/pipes/instance.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/pipes/reduce.py` & `olympipe-1.1.9/olympipe/pipes/reduce.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/olympipe/pipes/timebatch.py` & `olympipe-1.1.9/olympipe/pipes/timebatch.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.8/pyproject.toml` & `olympipe-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olympipe"
-version = "1.1.8"
+version = "1.1.9"
 description = "A powerful parallel pipelining tool"
 readme = "README.md"
 license = "MIT"
 homepage = "https://gitlab.com/gabraken/olympipe"
 repository = "https://gitlab.com/gabraken/olympipe"
 authors = ["Gabriel Kasser <gabriel.kasser@gmail.com>"]
 keywords = ["pipeline", "multiprocessing"]
```

### Comparing `olympipe-1.1.8/PKG-INFO` & `olympipe-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympipe
-Version: 1.1.8
+Version: 1.1.9
 Summary: A powerful parallel pipelining tool
 Home-page: https://gitlab.com/gabraken/olympipe
 License: MIT
 Keywords: pipeline,multiprocessing
 Author: Gabriel Kasser
 Author-email: gabriel.kasser@gmail.com
 Requires-Python: >=3.7.2,<4.0
```

