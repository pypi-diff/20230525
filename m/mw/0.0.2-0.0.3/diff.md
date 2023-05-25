# Comparing `tmp/mw-0.0.2.tar.gz` & `tmp/mw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mw-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mw-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mw-0.0.2.tar` & `mw-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      939 2023-05-22 20:52:54.059540 mw-0.0.2/README.md
--rw-r--r--   0        0        0      117 2023-05-22 20:52:54.059540 mw-0.0.2/mw/__init__.py
--rw-r--r--   0        0        0      559 2023-05-22 20:52:54.059540 mw-0.0.2/mw/__main__.py
--rw-r--r--   0        0        0     1811 2023-05-22 20:52:54.059540 mw-0.0.2/mw/app.py
--rw-r--r--   0        0        0     8154 2023-05-22 20:52:54.059540 mw-0.0.2/mw/command_handler.py
--rw-r--r--   0        0        0     3311 2023-05-22 20:52:54.059540 mw-0.0.2/mw/display.py
--rw-r--r--   0        0        0     4988 2023-05-22 20:52:54.059540 mw-0.0.2/mw/stack.py
--rw-r--r--   0        0        0       74 2023-05-22 20:52:54.059540 mw-0.0.2/mw/types.py
--rw-r--r--   0        0        0     1648 2023-05-22 20:52:54.059540 mw-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 mw-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1340 2023-05-24 06:29:49.850874 mw-0.0.3/README.md
+-rw-r--r--   0        0        0     4161 2023-05-24 06:29:49.850874 mw-0.0.3/data/share/man/man1/mw.1
+-rw-r--r--   0        0        0      117 2023-05-24 06:29:49.854874 mw-0.0.3/mw/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-24 06:29:49.854874 mw-0.0.3/mw/__main__.py
+-rw-r--r--   0        0        0     1811 2023-05-24 06:29:49.854874 mw-0.0.3/mw/app.py
+-rw-r--r--   0        0        0     8156 2023-05-24 06:29:49.854874 mw-0.0.3/mw/command_handler.py
+-rw-r--r--   0        0        0     3775 2023-05-24 06:29:49.854874 mw-0.0.3/mw/display.py
+-rw-r--r--   0        0        0     4988 2023-05-24 06:29:49.854874 mw-0.0.3/mw/stack.py
+-rw-r--r--   0        0        0       74 2023-05-24 06:29:49.854874 mw-0.0.3/mw/types.py
+-rw-r--r--   0        0        0     1694 2023-05-24 06:29:49.854874 mw-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2428 1970-01-01 00:00:00.000000 mw-0.0.3/PKG-INFO
```

### Comparing `mw-0.0.2/README.md` & `mw-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![](https://img.shields.io/github/license/iluvcapra/mw.svg) ![](https://img.shields.io/pypi/pyversions/mw.svg) [![](https://img.shields.io/pypi/v/mw.svg)](https://pypi.org/project/mw/) ![](https://img.shields.io/pypi/wheel/mw.svg)
+[![Lint and Test](https://github.com/iluvcapra/mw/actions/workflows/python-package.yml/badge.svg)](https://github.com/iluvcapra/mw/actions/workflows/python-package.yml)
+
 # mw
 
 `mw` is an audio sample editor for the terminal. If you're ever in a terminal/tmux
 session and just wanted to get a look at and maybe edit a sound file without
 having to open a window, this is a tool for you!
 
 # How to Use
```

### Comparing `mw-0.0.2/mw/__main__.py` & `mw-0.0.3/mw/__main__.py`

 * *Files identical despite different names*

### Comparing `mw-0.0.2/mw/app.py` & `mw-0.0.3/mw/app.py`

 * *Files identical despite different names*

### Comparing `mw-0.0.2/mw/command_handler.py` & `mw-0.0.3/mw/command_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,19 @@
             if len(argspec.parameters) == 1:
                 print(f"{f:15}: {m.__doc__}")
             else:
                 pnames = list(argspec.parameters)[1:] 
                 pnames = "[" + ",".join(pnames) + "]"
                 print(f"{f} {pnames}".ljust(15) + f": {m.__doc__}")
     
+    def license(self, app: 'mw.app.App'):
+        "Print the license"
+        print(app.license())
+
+  
     def stack(self, app: 'mw.app.App'):
         "Print the stack"
         app.display.print_stack(app.stack)
 
     def cmills(self, app: 'mw.app.App', pos: str = "0"):
         "Set/nudge cursor position in millis"
         if app.stack.top:
@@ -106,14 +111,27 @@
             new_time = app.stack.top.cursor
             if time:
                 new_time = parse_numeric(app.stack.top.out_point or 0, time)
             
             app.stack.top.out_point = Milliseconds(new_time)
             app.display.print_head(app.stack)
 
+    def ci(self, app: 'mw.app.App'):
+        "Clear in point"
+        if app.stack.top:
+            app.stack.top.in_point = None
+
+        app.display.print_head(app.stack)
+
+    def co(self, app:'mw.app.App'):
+        "Clear out point"
+        if app.stack.top:
+            app.stack.top.out_point = None
+
+        app.display.print_head(app.stack)
     def setw(self, app: 'mw.app.App', width = "80"):
         "Set columns width"
         app.display.display_width = int(width)
         app.display.print_head(app.stack)
     
     def dup(self, app: 'mw.app.App'):
         "Push a copy of the current sound onto the stack"
@@ -148,28 +166,14 @@
     def crop(self, app: 'mw.app.App',):
         "Crop the sound to the in and out points"
         if app.stack.top:
             app.stack.top.crop_to_selection()
         
         app.display.print_head(app.stack)
 
-    def ci(self, app: 'mw.app.App'):
-        "Clear in point"
-        if app.stack.top:
-            app.stack.top.in_point = None
-
-        app.display.print_head(app.stack)
-
-    def co(self, app:'mw.app.App'):
-        "Clear out point"
-        if app.stack.top:
-            app.stack.top.out_point = None
-
-        app.display.print_head(app.stack)
-
     def silence(self, app:'mw.app.App', dur: str):
         "Insert silence at cursor"
         if dur.isdigit():
             if app.stack.top:
                 at = app.stack.top.cursor
                 app.stack.top.insert_silence(Milliseconds(int(dur)), at)
             
@@ -198,18 +202,14 @@
         app.display.print_head(app.stack)
 
     def play(self, app:'mw.app.App'):
         "Play the sound"
         if app.stack.top:
             app.stack.top.play()
     
-    def license(self, app: 'mw.app.App'):
-        "Print the license"
-        print(app.license())
-
     def length(self, app:'mw.app.App'):
         "Print the length of the top sound"
         if app.stack.top:
             print(f"{len(app.stack.top.segment)} ms")
 
     def bounce(self, app: 'mw.app.App'):
         "Bounce (mix) the top sound in the stack with the sound below it"
```

### Comparing `mw-0.0.2/mw/display.py` & `mw-0.0.3/mw/display.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,20 +50,31 @@
                 self.print_frame(i, frame, session_length)
             print(f"Session length {stack.length() / 1000.0} sec")
         else:
             print("Stack empty")
 
     def print_head(self, stack: 'mw.stack.Stack'):
         if stack.top:
-            self.print_frame_single(stack.top)
             self.print_ruler(stack.top)
+            self.print_frame_single(stack.top)
+            self.print_selection(stack.top)
         else:
             print("Stack empty")
-
+    
     def print_ruler(self, entry: 'mw.stack.StackFrame'):
+        start_time = f"{entry.view_start}"
+        end_time = f"{entry.view_end} ms"
+        slug = list(" " * self.print_width_for_length(entry.view_length(),
+                                                      entry.view_length()))
+
+        slug[0:len(start_time)] = start_time
+        slug[-len(end_time):] = end_time
+        print("".join(slug))
+
+    def print_selection(self, entry: 'mw.stack.StackFrame'):
         slug = list(" " * self.display_width)
         in_pos = None
         out_pos = None
         view_length = Milliseconds(len(entry.clip_for_view()))
         if entry.in_point is not None:
             in_pos = self.print_width_for_length(entry.in_point, view_length) 
             slug[in_pos] = "["
@@ -72,15 +83,15 @@
             out_pos = self.print_width_for_length(entry.out_point, view_length)
             slug[out_pos] = "]"
 
         if in_pos is not None and out_pos is not None:
             for i in range(in_pos + 1, out_pos):
                 slug[i] = "⎯"
 
-        slug[self.print_width_for_length(entry.cursor, view_length)] = "^"
+        slug[self.print_width_for_length(entry.cursor, view_length)] = "⬆"
         print("".join(slug))
 
     def show_view_info(self):
         print(f"Display width: {self.display_width} cols")
         # print(f"View start: {self.view_start} ms")
         # print(f"View end: {self.view_end} ms")
         # print(f"ms/col: {(self.view_end - self.view_start) // self.display_width}")
```

### Comparing `mw-0.0.2/mw/stack.py` & `mw-0.0.3/mw/stack.py`

 * *Files identical despite different names*

### Comparing `mw-0.0.2/pyproject.toml` & `mw-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 keywords = [
     'waveform', 
     'metadata', 
     'audio', 
     'console'
 ]
 
+[tool.flit.external-data]
+directory = "data"
+
 [tool.flit.module]
 name = "mw"
 
 [project.optional-dependencies]
 doc = [
     'sphinx >= 5.3.0',
     'sphinx_rtd_theme >= 1.1.1',
```

### Comparing `mw-0.0.2/PKG-INFO` & `mw-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mw
-Version: 0.0.2
+Version: 0.0.3
 Summary: mw is an audio sample editor for the terminal.
 Keywords: waveform,metadata,audio,console
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -22,14 +22,17 @@
 Requires-Dist: sphinx >= 5.3.0 ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme >= 1.1.1 ; extra == "doc"
 Project-URL: Home, https://github.com/iluvcapra/mw
 Project-URL: Issues, https://github.com/iluvcapra/mw/issues
 Project-URL: Source, https://github.com/iluvcapra/mw.git
 Provides-Extra: doc
 
+![](https://img.shields.io/github/license/iluvcapra/mw.svg) ![](https://img.shields.io/pypi/pyversions/mw.svg) [![](https://img.shields.io/pypi/v/mw.svg)](https://pypi.org/project/mw/) ![](https://img.shields.io/pypi/wheel/mw.svg)
+[![Lint and Test](https://github.com/iluvcapra/mw/actions/workflows/python-package.yml/badge.svg)](https://github.com/iluvcapra/mw/actions/workflows/python-package.yml)
+
 # mw
 
 `mw` is an audio sample editor for the terminal. If you're ever in a terminal/tmux
 session and just wanted to get a look at and maybe edit a sound file without
 having to open a window, this is a tool for you!
 
 # How to Use
```

