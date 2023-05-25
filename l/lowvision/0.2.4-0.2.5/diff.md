# Comparing `tmp/lowvision-0.2.4.tar.gz` & `tmp/lowvision-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowvision-0.2.4.tar", last modified: Wed May 24 03:54:42 2023, max compression
+gzip compressed data, was "lowvision-0.2.5.tar", last modified: Thu May 25 02:13:05 2023, max compression
```

## Comparing `lowvision-0.2.4.tar` & `lowvision-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:54:42.024641 lowvision-0.2.4/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2104 2023-05-24 03:54:42.024507 lowvision-0.2.4/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)     1902 2023-05-24 03:53:26.000000 lowvision-0.2.4/README.md
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:54:42.023595 lowvision-0.2.4/lowvision/
--rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.4/lowvision/__init__.py
--rw-r--r--   0 danielpcox   (502) staff       (20)     5103 2023-05-24 03:30:09.000000 lowvision-0.2.4/lowvision/chat.py
--rwxr-xr-x   0 danielpcox   (502) staff       (20)     4511 2023-05-24 03:48:42.000000 lowvision-0.2.4/lowvision/shell.py
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:54:42.024335 lowvision-0.2.4/lowvision.egg-info/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2104 2023-05-24 03:54:41.000000 lowvision-0.2.4/lowvision.egg-info/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-24 03:54:42.000000 lowvision-0.2.4/lowvision.egg-info/SOURCES.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-24 03:54:41.000000 lowvision-0.2.4/lowvision.egg-info/dependency_links.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:54:41.000000 lowvision-0.2.4/lowvision.egg-info/requires.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:54:41.000000 lowvision-0.2.4/lowvision.egg-info/top_level.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)      413 2023-05-24 03:54:30.000000 lowvision-0.2.4/pyproject.toml
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-24 03:54:42.024678 lowvision-0.2.4/setup.cfg
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.4/setup.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 02:13:05.505445 lowvision-0.2.5/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2104 2023-05-25 02:13:05.505286 lowvision-0.2.5/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)     1902 2023-05-24 03:53:26.000000 lowvision-0.2.5/README.md
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 02:13:05.504291 lowvision-0.2.5/lowvision/
+-rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.5/lowvision/__init__.py
+-rw-r--r--   0 danielpcox   (502) staff       (20)     5749 2023-05-25 02:11:50.000000 lowvision-0.2.5/lowvision/chat.py
+-rwxr-xr-x   0 danielpcox   (502) staff       (20)     4578 2023-05-25 02:07:29.000000 lowvision-0.2.5/lowvision/shell.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 02:13:05.505077 lowvision-0.2.5/lowvision.egg-info/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2104 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/SOURCES.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/dependency_links.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)        7 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/requires.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/top_level.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)      395 2023-05-25 02:12:35.000000 lowvision-0.2.5/pyproject.toml
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-25 02:13:05.505481 lowvision-0.2.5/setup.cfg
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.5/setup.py
```

### Comparing `lowvision-0.2.4/PKG-INFO` & `lowvision-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
```

### Comparing `lowvision-0.2.4/README.md` & `lowvision-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `lowvision-0.2.4/lowvision/chat.py` & `lowvision-0.2.5/lowvision/chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,22 +16,38 @@
         self.old_settings = old_term_settings
         self.line_buffer = ''
         self.scrollback = ''
         self.max_chars = config.scrollback
         self.conversation = []
         self.interrupt_response = False
 
+        # We only care about the input so we can watch for the "chat" command
+        self.input_buffer = ''
+        self.trigger_chat_mode = False
+
+    async def watch_for_trigger(self, message: bytes):
+        message = message.decode('utf-8', errors='ignore').replace('\r', '')
+        self.input_buffer += message
+        if '\n' in self.input_buffer:
+            lines = self.input_buffer.split('\n')
+            self.input_buffer = lines.pop()
+            for line in lines:
+                if line == "chat":
+                    self.trigger_chat_mode = True
+
     async def log(self, message: bytes):
+
         message = message.decode('utf-8', errors='ignore').replace('\r', '')
         self.line_buffer += message
         if '\n' in self.line_buffer:
             lines = self.line_buffer.split('\n')
             self.line_buffer = lines.pop()
             for line in lines:
-                if line.endswith("chat"):
+                if line.endswith("chat") and self.trigger_chat_mode:
+                    self.trigger_chat_mode = False
                     await self.chat_mode()
                 new_line = line + '\n'
                 self.scrollback += new_line
                 while len(self.scrollback) > self.max_chars:
                     pos = self.scrollback.find('\n') + 1
                     self.scrollback = self.scrollback[pos:]
```

### Comparing `lowvision-0.2.4/lowvision/shell.py` & `lowvision-0.2.5/lowvision/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                 try:
                     r_fd, _, _ = select([sys.stdin, master_fd], [], [])
 
                     if sys.stdin in r_fd:
                         input_data = os.read(sys.stdin.fileno(), 1024)
                         if not input_data:
                             break
+                        await logger.watch_for_trigger(input_data)
                         os.write(master_fd, input_data)
 
                     if master_fd in r_fd:
                         output_data = os.read(master_fd, 1024)
                         if not output_data:
                             break
```

### Comparing `lowvision-0.2.4/lowvision.egg-info/PKG-INFO` & `lowvision-0.2.5/lowvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
```

