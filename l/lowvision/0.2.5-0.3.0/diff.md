# Comparing `tmp/lowvision-0.2.5.tar.gz` & `tmp/lowvision-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowvision-0.2.5.tar", last modified: Thu May 25 02:13:05 2023, max compression
+gzip compressed data, was "lowvision-0.3.0.tar", last modified: Thu May 25 03:39:45 2023, max compression
```

## Comparing `lowvision-0.2.5.tar` & `lowvision-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 02:13:05.505445 lowvision-0.2.5/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2104 2023-05-25 02:13:05.505286 lowvision-0.2.5/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)     1902 2023-05-24 03:53:26.000000 lowvision-0.2.5/README.md
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 02:13:05.504291 lowvision-0.2.5/lowvision/
--rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.5/lowvision/__init__.py
--rw-r--r--   0 danielpcox   (502) staff       (20)     5749 2023-05-25 02:11:50.000000 lowvision-0.2.5/lowvision/chat.py
--rwxr-xr-x   0 danielpcox   (502) staff       (20)     4578 2023-05-25 02:07:29.000000 lowvision-0.2.5/lowvision/shell.py
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 02:13:05.505077 lowvision-0.2.5/lowvision.egg-info/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2104 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/SOURCES.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/dependency_links.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)        7 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/requires.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-25 02:13:05.000000 lowvision-0.2.5/lowvision.egg-info/top_level.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)      395 2023-05-25 02:12:35.000000 lowvision-0.2.5/pyproject.toml
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-25 02:13:05.505481 lowvision-0.2.5/setup.cfg
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.5/setup.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 03:39:45.372037 lowvision-0.3.0/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     3052 2023-05-25 03:39:45.371893 lowvision-0.3.0/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2849 2023-05-25 03:39:28.000000 lowvision-0.3.0/README.md
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 03:39:45.370518 lowvision-0.3.0/lowvision/
+-rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.3.0/lowvision/__init__.py
+-rw-r--r--   0 danielpcox   (502) staff       (20)     6037 2023-05-25 03:12:55.000000 lowvision-0.3.0/lowvision/chat.py
+-rw-r--r--   0 danielpcox   (502) staff       (20)      128 2023-05-25 02:47:36.000000 lowvision-0.3.0/lowvision/chat_mode_trigger.py
+-rwxr-xr-x   0 danielpcox   (502) staff       (20)     4602 2023-05-25 02:28:11.000000 lowvision-0.3.0/lowvision/shell.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-25 03:39:45.371706 lowvision-0.3.0/lowvision.egg-info/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     3052 2023-05-25 03:39:45.000000 lowvision-0.3.0/lowvision.egg-info/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)      323 2023-05-25 03:39:45.000000 lowvision-0.3.0/lowvision.egg-info/SOURCES.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-25 03:39:45.000000 lowvision-0.3.0/lowvision.egg-info/dependency_links.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       65 2023-05-25 03:39:45.000000 lowvision-0.3.0/lowvision.egg-info/entry_points.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)        7 2023-05-25 03:39:45.000000 lowvision-0.3.0/lowvision.egg-info/requires.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-25 03:39:45.000000 lowvision-0.3.0/lowvision.egg-info/top_level.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)      463 2023-05-25 03:14:03.000000 lowvision-0.3.0/pyproject.toml
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-25 03:39:45.372073 lowvision-0.3.0/setup.cfg
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.3.0/setup.py
```

### Comparing `lowvision-0.2.5/PKG-INFO` & `lowvision-0.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-Metadata-Version: 2.1
-Name: lowvision
-Version: 0.2.5
-Summary: Tools for low-vision coders
-Author-email: Daniel Cox <danielpcox@gmail.com>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # Tools for low-vision coders
 
 ## Shell Chat
 
 A wrapper for your shell that lets you talk to ChatGPT about the recent interactions.
 
 1. Wraps bash or another shell you pass in, so that it behaves exactly like what you'd expect.
 2. Except that when you run the `chat` command, it switches into a separate mode where you're talking to ChatGPT about the past 3k (configurable) characters of interaction.
 3. You have a back and forth conversation, and all of ChatGPT's responses are read aloud.
 4. You can `Ctrl-C` to interrupt and go back to the chat prompt.
 5. You type `exit` to go back to your shell.
 
 ### Installation
 
+From the Python environment _that will be activated when your chosen shell starts_, run
+
 ```bash
 pip install lowvision
 ```
 
 Then set [your OpenAI API key](https://platform.openai.com/account/api-keys)
 ```bash
 export OPENAI_API_KEY='whatever'
 ```
 
+NOTE: The reason for installing in the Python environment active when your shell starts is because a `chat` command is
+installed by `lowvision` that activates chat mode, and it must be available inside your wrapped shell.
+if you've installed in a virtualenv instead, you'll need to activate that virtualenv after running the shell wrapper,
+or `chat` won't properly activate chat mode.
+
 ### Usage
 
 See the help with 
 
 ```bash
 python -m lowvision.shell -h
 ```
@@ -61,7 +60,20 @@
 sh-3.2$ chat     
 ?> what happened?
 The user performed a ping test to google.com by sending 3 packets, and received a reply from one packet. The response shows the IP address of google.com and the round-trip time for the packet. The test was interrupted with ^C after receiving one response.
 ?> exit
 sh-3.2$
 ```
 
+### Installing as the default shell
+
+If you want to use this as your default shell, you could create a script like this (replacing the path to the Python
+environment where you installed `lowvision`) and then set your default shell to that script.
+
+```bash
+#!/bin/sh
+
+export OPENAI_API_KEY="whatever"
+/opt/homebrew/Caskroom/mambaforge/base/bin/python3 -m lowvision.shell
+```
+
+Then make it executable, and set it as your default shell with `chsh -s /path/to/your/script.sh`.
```

### Comparing `lowvision-0.2.5/lowvision/chat.py` & `lowvision-0.3.0/lowvision/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,50 +5,55 @@
 import sys
 import termios
 import textwrap
 from datetime import datetime, timezone
 
 import openai
 
+from lowvision.chat_mode_trigger import chat_mode_trigger
 
 class ChatLogger:
     def __init__(self, config: argparse.Namespace, old_term_settings: list):
         self.config = config
         self.old_settings = old_term_settings
         self.line_buffer = ''
         self.scrollback = ''
         self.max_chars = config.scrollback
         self.conversation = []
         self.interrupt_response = False
 
         # We only care about the input so we can watch for the "chat" command
         self.input_buffer = ''
-        self.trigger_chat_mode = False
+        self.chat_in_input = False
+        chat_mode_trigger.unlink(missing_ok=True)
 
     async def watch_for_trigger(self, message: bytes):
         message = message.decode('utf-8', errors='ignore').replace('\r', '')
         self.input_buffer += message
         if '\n' in self.input_buffer:
             lines = self.input_buffer.split('\n')
             self.input_buffer = lines.pop()
             for line in lines:
-                if line == "chat":
-                    self.trigger_chat_mode = True
+                if "chat" in line:
+                    self.chat_in_input = True
 
     async def log(self, message: bytes):
 
         message = message.decode('utf-8', errors='ignore').replace('\r', '')
         self.line_buffer += message
         if '\n' in self.line_buffer:
             lines = self.line_buffer.split('\n')
             self.line_buffer = lines.pop()
             for line in lines:
-                if line.endswith("chat") and self.trigger_chat_mode:
-                    self.trigger_chat_mode = False
-                    await self.chat_mode()
+                if "chat" in line and self.chat_in_input:
+                    await asyncio.sleep(0.2) # wait for trigger file to exist
+                    if chat_mode_trigger.exists():
+                        self.chat_in_input = False
+                        chat_mode_trigger.unlink(missing_ok=True)
+                        await self.chat_mode()
                 new_line = line + '\n'
                 self.scrollback += new_line
                 while len(self.scrollback) > self.max_chars:
                     pos = self.scrollback.find('\n') + 1
                     self.scrollback = self.scrollback[pos:]
 
     def reset_conversation(self):
```

### Comparing `lowvision-0.2.5/lowvision/shell.py` & `lowvision-0.3.0/lowvision/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 async def main(config):
     pid, master_fd = pty.fork()
 
     if pid == 0:
         # Child process
         os.execv(config.shell, [config.shell])
     else:
+        # Parent process
         print(f"\nStarting chat-aware shell wrapper around {config.shell}. "
               "Run `chat` to enter chat mode. Exit with `exit`. "
               "Ctrl-C interrupts text-to-speech. "
               "Exit and re-run with `-h` to see options.")
         print("Option values: ", config.__dict__, "\n")
-        # Parent process
-        shell_pid = pid
 
-        def handle_signals(signal_number, frame):
-            os.kill(shell_pid, signal_number)
+        def handle_signals(signum, frame):
+            foreground_pgrp = os.tcgetpgrp(master_fd)
+            os.killpg(foreground_pgrp, signum)
 
         def handle_window_resize(signum, frame):
             size = get_terminal_size()
             set_terminal_size(master_fd, size)
 
         signal.signal(signal.SIGWINCH, handle_window_resize)
         signal.signal(signal.SIGINT, handle_signals)
```

### Comparing `lowvision-0.2.5/lowvision.egg-info/PKG-INFO` & `lowvision-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
 
@@ -16,23 +16,30 @@
 2. Except that when you run the `chat` command, it switches into a separate mode where you're talking to ChatGPT about the past 3k (configurable) characters of interaction.
 3. You have a back and forth conversation, and all of ChatGPT's responses are read aloud.
 4. You can `Ctrl-C` to interrupt and go back to the chat prompt.
 5. You type `exit` to go back to your shell.
 
 ### Installation
 
+From the Python environment _that will be activated when your chosen shell starts_, run
+
 ```bash
 pip install lowvision
 ```
 
 Then set [your OpenAI API key](https://platform.openai.com/account/api-keys)
 ```bash
 export OPENAI_API_KEY='whatever'
 ```
 
+NOTE: The reason for installing in the Python environment active when your shell starts is because a `chat` command is
+installed by `lowvision` that activates chat mode, and it must be available inside your wrapped shell.
+if you've installed in a virtualenv instead, you'll need to activate that virtualenv after running the shell wrapper,
+or `chat` won't properly activate chat mode.
+
 ### Usage
 
 See the help with 
 
 ```bash
 python -m lowvision.shell -h
 ```
@@ -61,7 +68,20 @@
 sh-3.2$ chat     
 ?> what happened?
 The user performed a ping test to google.com by sending 3 packets, and received a reply from one packet. The response shows the IP address of google.com and the round-trip time for the packet. The test was interrupted with ^C after receiving one response.
 ?> exit
 sh-3.2$
 ```
 
+### Installing as the default shell
+
+If you want to use this as your default shell, you could create a script like this (replacing the path to the Python
+environment where you installed `lowvision`) and then set your default shell to that script.
+
+```bash
+#!/bin/sh
+
+export OPENAI_API_KEY="whatever"
+/opt/homebrew/Caskroom/mambaforge/base/bin/python3 -m lowvision.shell
+```
+
+Then make it executable, and set it as your default shell with `chsh -s /path/to/your/script.sh`.
```

