# Comparing `tmp/rzpipe-0.5.0.tar.gz` & `tmp/rzpipe-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rzpipe-0.5.0.tar", last modified: Wed May 24 16:30:56 2023, max compression
+gzip compressed data, was "rzpipe-0.5.1.tar", last modified: Thu May 25 17:32:49 2023, max compression
```

## Comparing `rzpipe-0.5.0.tar` & `rzpipe-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:30:56.270512 rzpipe-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-24 16:23:58.000000 rzpipe-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-24 16:23:58.000000 rzpipe-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-24 16:30:56.270512 rzpipe-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-24 16:23:58.000000 rzpipe-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:30:56.270512 rzpipe-0.5.0/rzpipe/
--rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/native.py
--rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/open_async.py
--rw-r--r--   0 runner    (1001) docker     (122)    10191 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/open_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/open_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:30:56.270512 rzpipe-0.5.0/rzpipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 16:30:56.270512 rzpipe-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      876 2023-05-24 16:23:58.000000 rzpipe-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:32:49.324274 rzpipe-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-25 17:26:20.000000 rzpipe-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-25 17:26:20.000000 rzpipe-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-05-25 17:32:49.324274 rzpipe-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-25 17:26:20.000000 rzpipe-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:32:49.324274 rzpipe-0.5.1/rzpipe/
+-rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-05-25 17:26:20.000000 rzpipe-0.5.1/rzpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-05-25 17:26:20.000000 rzpipe-0.5.1/rzpipe/native.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-05-25 17:26:20.000000 rzpipe-0.5.1/rzpipe/open_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10805 2023-05-25 17:26:20.000000 rzpipe-0.5.1/rzpipe/open_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4893 2023-05-25 17:26:20.000000 rzpipe-0.5.1/rzpipe/open_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:32:49.324274 rzpipe-0.5.1/rzpipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-05-25 17:32:49.000000 rzpipe-0.5.1/rzpipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 17:32:49.000000 rzpipe-0.5.1/rzpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:32:49.000000 rzpipe-0.5.1/rzpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-25 17:32:49.000000 rzpipe-0.5.1/rzpipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 17:32:49.324274 rzpipe-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      876 2023-05-25 17:26:20.000000 rzpipe-0.5.1/setup.py
```

### Comparing `rzpipe-0.5.0/LICENSE` & `rzpipe-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rzpipe-0.5.0/PKG-INFO` & `rzpipe-0.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rzpipe
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pipe interface for rizin
 Home-page: https://rizin.re
 Author: rizinorg
 Author-email: info@rizin.re
 License: MIT
 Description: # rzpipe for Python
         
@@ -27,16 +27,16 @@
         
         ```python
         import rzpipe
         
         pipe = rzpipe.open("/bin/ls")
         pipe.cmd('aa')
         print(pipe.cmd("afl"))
-        print(pipe.cmdj("aflj"))            # evaluates JSON and returns an object
-        print(pipe.cmdj("ij").core.format)  # shows file format
+        print(pipe.cmdj("aflj"))            # parses the JSON and returns a dict (note the lowercase j)
+        print(pipe.cmdJ("ij").core.format)  # parses the JSON and returns a namedtuple (note the uppercase J)
         pipe.quit()
         ```
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `rzpipe-0.5.0/rzpipe/__init__.py` & `rzpipe-0.5.1/rzpipe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import time
 
 try:
     import rzlang
 except ImportError:
     rzlang = None
 
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 
 from .open_sync import open
 from shutil import which
 
 
 def version():
     """Return string with the version of the rzpipe library"""
```

### Comparing `rzpipe-0.5.0/rzpipe/native.py` & `rzpipe-0.5.1/rzpipe/native.py`

 * *Files identical despite different names*

### Comparing `rzpipe-0.5.0/rzpipe/open_async.py` & `rzpipe-0.5.1/rzpipe/open_async.py`

 * *Files identical despite different names*

### Comparing `rzpipe-0.5.0/rzpipe/open_base.py` & `rzpipe-0.5.1/rzpipe/open_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 """
 
 import json
 import os
 import platform
 import sys
-import signal
 import functools
+import signal
 from contextlib import contextmanager
+import threading
 from shutil import which
 from subprocess import Popen, PIPE
 
 try:
     import rzlang
 except ImportError:
     rzlang = None
@@ -77,31 +78,52 @@
             bin_file = "/usr/bin/rizin"
 
         if os.path.isfile(bin_file):
             return bin_file
         else:
             raise IOError("rizin can't be found in your system")
 
-@contextmanager
-def timeout_callback(timeout_s, callback):
-    signal.signal(signal.SIGALRM, callback)
 
+class TimerTimeout(Exception):
+    pass
+
+
+def raise_exception_on_thread(target_tid):
+    import ctypes
+    tid = ctypes.c_long(target_tid)
+    pyo = ctypes.py_object(TimerTimeout)
+    ret = ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, pyo)
+    if ret == 0:
+        raise ValueError(f"invalid thread id ({target_tid})")
+    elif ret > 1:
+        ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, 0)
+        raise SystemError("PyThreadState_SetAsyncExc failed")
+
+
+@contextmanager
+def timeout_callback(timeout_secs):
+    timer = None
+    if timeout_secs > 0:
+        tid = threading.current_thread().ident
+        timer = threading.Timer(timeout_secs, raise_exception_on_thread, args=(tid,))
     try:
-        signal.alarm(timeout_s)
+        if timer is not None:
+            timer.start()
         yield
     finally:
-        signal.alarm(0)
+        if timer is not None:
+            timer.cancel()
 
 class OpenBase(object):
     """
     Class representing an rzpipe connection with a running rizin instance
     Class body derived from __init__.py "open" class.
     """
 
-    def __init__(self, filename="", flags=None, cmd_timeout_s=-1):
+    def __init__(self, filename="", flags=None, cmd_timeout_secs=-1):
         """
         Open a new rizin pipe
         The 'filename' can be one of the following:
 
         * absolute or relative path to file
         * http://<host>:<port> to connect to an rizin webserver
         * tcp://<host>:<port> to connect to an rizin tcp server
@@ -113,15 +135,15 @@
                 ("-wdn") or separated by commas ("-w","-d","-n")
         Returns:
             Returns an object with methods to interact with rizin via commands
         """
         if not flags:
             flags = []
 
-        self.cmd_timeout_s = cmd_timeout_s
+        self._cmd_timeout_secs = cmd_timeout_secs
 
         self._async = False
 
         # Set cmd native as default
         self.uri = filename
         self._cmd = self._cmd_native
 
@@ -171,18 +193,16 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.quit()
 
-    def _handle_killswitch_timeout(self, context, *args):
-        self._quit_process()
-
-        raise TimeoutError(f"Timeout of {self.cmd_timeout_s} seconds reached on '{context}'")
+    def set_timeout(self, timeout_secs):
+        self._cmd_timeout_secs = timeout_secs
 
     def _cmd_pipe(self, cmd):
         out = b""
         cmd = cmd.strip().replace("\n", ";")
         if os.name == "nt":
             cmd = cmd.encode("utf-8")
             windll.kernel32.WriteFile(
@@ -233,15 +253,15 @@
             import subprocess
 
             is_async = not isinstance(self.process, subprocess.Popen)
             if not is_async:
                 for f in [self.process.stdin, self.process.stdout]:
                     if f is not None:
                         f.close()
-            self.process.terminate()
+            self.process.kill()
             self.process.wait()
             delattr(self, "process")
 
             if is_async:
                 import asyncio
 
                 asyncio.get_event_loop().run_until_complete(asyncio.sleep(0.1))
@@ -258,25 +278,25 @@
             Returns an string with the results of the command
 
         res = self._cmd(cmd)
         if res is not None:
             return res.strip()
         return None
         """
+        with timeout_callback(self._cmd_timeout_secs):
+            try:
+                res = self._cmd(cmd, **kwargs)
+                if res is not None:
+                    if os.name == "nt":
+                        res = res.replace("\r\n", "\n")
+                    return res
+            except TimerTimeout:
+                raise TimeoutError(f"Timeout reached on cmd: '{cmd}'") from None
 
-        with timeout_callback(
-            self.cmd_timeout_s,
-            functools.partial(self._handle_killswitch_timeout, f"rzpipe.cmd: {cmd}")
-        ):
-            res = self._cmd(cmd, **kwargs)
-            if res is not None:
-                if os.name == "nt":
-                    res = res.replace("\r\n", "\n")
-                return res
-            return None
+        return None
 
     def cmdj(self, cmd, **kwargs):
         """Same as cmd() but evaluates JSONs and returns an object
         Args:
             cmdj (str): rizin command
         Returns:
             Returns a JSON object respresenting the parsed JSON
```

### Comparing `rzpipe-0.5.0/rzpipe/open_sync.py` & `rzpipe-0.5.1/rzpipe/open_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             self.conn = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.conn.connect((r.group(1), int(r.group(2))))
         elif filename:
             self._cmd = self._cmd_process
             if rizin_home is not None:
                 if not os.path.isdir(rizin_home):
                     raise Exception(
-                        "`rizinhome` passed is invalid, leave it None or put a valid path to rizin folder"
+                        "`rizin_home` passed is invalid, leave it None or put a valid path to rizin folder"
                     )
                 rze = os.path.join(rizin_home, "rizin")
             else:
                 rze = "rizin"
             if os.name == "nt":
                 # avoid errors on Windows when subprocess messes with name
                 rze += ".exe"
```

### Comparing `rzpipe-0.5.0/rzpipe.egg-info/PKG-INFO` & `rzpipe-0.5.1/rzpipe.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rzpipe
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pipe interface for rizin
 Home-page: https://rizin.re
 Author: rizinorg
 Author-email: info@rizin.re
 License: MIT
 Description: # rzpipe for Python
         
@@ -27,16 +27,16 @@
         
         ```python
         import rzpipe
         
         pipe = rzpipe.open("/bin/ls")
         pipe.cmd('aa')
         print(pipe.cmd("afl"))
-        print(pipe.cmdj("aflj"))            # evaluates JSON and returns an object
-        print(pipe.cmdj("ij").core.format)  # shows file format
+        print(pipe.cmdj("aflj"))            # parses the JSON and returns a dict (note the lowercase j)
+        print(pipe.cmdJ("ij").core.format)  # parses the JSON and returns a namedtuple (note the uppercase J)
         pipe.quit()
         ```
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `rzpipe-0.5.0/setup.py` & `rzpipe-0.5.1/setup.py`

 * *Files identical despite different names*

