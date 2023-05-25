# Comparing `tmp/flake8_tkinter-0.5.4.tar.gz` & `tmp/flake8_tkinter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_tkinter-0.5.4.tar", last modified: Tue Aug 16 15:35:19 2022, max compression
+gzip compressed data, was "flake8_tkinter-0.6.0.tar", last modified: Thu May 25 20:48:41 2023, max compression
```

## Comparing `flake8_tkinter-0.5.4.tar` & `flake8_tkinter-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:35:19.319581 flake8_tkinter-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7760 2022-08-16 15:35:19.319581 flake8_tkinter-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6826 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:35:19.319581 flake8_tkinter-0.5.4/flake8_tkinter/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:35:19.319581 flake8_tkinter-0.5.4/flake8_tkinter/rules/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_call.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_import.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_import_from.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/flake8_tkinter/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:35:19.319581 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7760 2022-08-16 15:35:19.000000 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-08-16 15:35:19.000000 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 15:35:19.000000 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-16 15:35:19.000000 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-16 15:35:19.000000 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-16 15:35:19.000000 flake8_tkinter-0.5.4/flake8_tkinter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 15:35:19.319581 flake8_tkinter-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-08-16 15:35:11.000000 flake8_tkinter-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:41.189312 flake8_tkinter-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-25 20:48:41.189312 flake8_tkinter-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:41.189312 flake8_tkinter-0.6.0/flake8_tkinter/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:41.189312 flake8_tkinter-0.6.0/flake8_tkinter/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_import_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/flake8_tkinter/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:41.189312 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-25 20:48:41.000000 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 20:48:41.000000 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:48:41.000000 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:48:41.000000 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 20:48:41.000000 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 20:48:41.000000 flake8_tkinter-0.6.0/flake8_tkinter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:48:41.193313 flake8_tkinter-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-25 20:48:28.000000 flake8_tkinter-0.6.0/setup.py
```

### Comparing `flake8_tkinter-0.5.4/LICENSE` & `flake8_tkinter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_tkinter-0.5.4/PKG-INFO` & `flake8_tkinter-0.6.0/flake8_tkinter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
-Name: flake8_tkinter
-Version: 0.5.4
-Summary: Flake8 plugin to detect (too) common mistakes and bad practices in Tkinter projects
+Name: flake8-tkinter
+Version: 0.6.0
+Summary: A flake8 plugin that helps you write better Tkinter code
 Home-page: https://github.com/rdbende/flake8-tkinter
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
+Project-URL: Tracker, https://github.com/rdbende/flake8-tkinter/issues
 Platform: UNKNOWN
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-tkinter
 
-A flake8 plugin that helps you detect (too) common mistakes and bad practices in you Tkinter project
+A [flake8](https://github.com/PyCQA/flake8) plugin that helps you write better Tkinter code
 
 _Project idea by [@insolor](https://github.com/insolor)_
 
 
 ## Installation
 
 ```
@@ -41,21 +43,21 @@
 Common mistakes
 - **`TK102`**: Using multiple mainloop calls is unnecessary. One call is perfectly enough. ([example](#tk102))
 - **`TK111`**: Calling `callback_handler()` instead of passing the reference for on-click or binding callback. ([example](#tk111))
 - **`TK112`**: Calling `callback_handler()` with arguments instead of passing the reference for on-click or binding callback. If you need to call `callback_handler` with arguments, use lambda or functools.partial. ([example](#tk112))
 - **`TK131`**: Assigning result of geometry manager call to a variable. ([example](#tk131))
 
 Best practices
+- **`TK141`**: Using bind without `add=True` will overwrite any existing bindings to this sequence on this widget. Either overwrite them explicitly with `add=False` or use `add=True` to keep existing bindings. ([example](#tk141))
+- **`TK142`**: Creating tag bindings in a loop can lead to memory leaks. Store the returned command names in a list to clean them up later. ([example](#tk142))
 - **`TK201`**: Using `from tkinter import *` is generally a bad practice and discouraged. Use `import tkinter as tk` or simply `import tkinter` instead. ([example](#tk201))
 - **`TK202`**: Using `from tkinter.ttk import *` is generally a bad practice and discouraged. Use `from tkinter import ttk` instead. ([example](#tk202))
 - **`TK211`**: Using `import tkinter.ttk as ttk` is pointless. Use `from tkinter import ttk` instead. ([example](#tk211))
 - **`TK221`**: Using tkinter.TRUE, tkinter.FALSE, etc. is pointless. Use an appropriate Python boolean instead. ([example](#tk221))
-- **`TK231`**: Using bind without `add=True` will overwrite any existing bindings to this sequence on this widget. Either overwrite them explicitly with `add=False` or use `add=True` to keep existing bindings. ([example](#tk231))
-- **`TK232`**: Creating tag bindings in a loop can lead to memory leaks. Store the returned command names in a list to clean them up later. ([example](#tk232))
-- **`TK251`**: Using `tkinter.Message` widget. It's redundant since `tkinter.Label` provides the same functionality.. ([example](#tk251)
+- **`TK251`**: Using `tkinter.Message` widget. It's redundant since `tkinter.Label` provides the same functionality. ([example](#tk251))
 
 Code quality
 - **`TK304`**: Value for `add` in bind methods should be a boolean. ([example](#tk304))
 
 Opinionated warnings
 - **`TK504`**: Using a tkinter constant. Use a string literal instead (disabled by default). ([example](#tk504))
 
@@ -155,41 +157,39 @@
 w.pack(expand=tk.OFF)
 
 # Good
 w.pack(expand=True)
 w.pack(expand=False)
 ```
 
-### TK231
-_Will be renamed to TK141 in v1.0.0_
+### TK141
 ```python
 # Bad
 w.bind("<Button-1>", foo)
 
 # Good
 w.bind("<Button-1>", foo, add=True)
 # OR
 w.bind("<Button-1>", foo, add=False)
 ```
 
-### TK232
-_Will be renamed to TK142 in v1.0.0_
+### TK142
 ```python
 # Bad
 for index, foo in enumerate(foos):
     w.tag_bind(f"bar_{index}", "<Button-1>", baz)
     
 # Good
 for index, foo in enumerate(foos):
     tcl_command = w.tag_bind(f"bar_{index}", "<Button-1>", baz)
     bindings.append(tcl_command)  # Clean them up later with `.deletecommand()`
 ```
 
 ### TK251
-_Yes, there's some minor diffrence in text wrapping difference, but that can be adjusted_
+_Yes, there's some minor diffrence in text wrapping, but that can be easily fixed
 ```python
 # Bad
 w = tkinter.Message()
 
 # Good
 w = tkinter.Label()
 ```
@@ -213,39 +213,47 @@
 ```
 
 ## Planned warnings
 
 - Common mistakes (TK101-TK179)
     - `TK101`: Using multiple `tkinter.Tk` instances. Child windows must be created from `tkinter.Toplevel`.
     - `TK103`: Suggest refactoring code that uses `.update()`, as it's usually pointless, [potentially harmful](https://wiki.tcl-lang.org/page/Update+considered+harmful), and considered a code smell.
-    - `TK113`: Callback handler should be a callable ([lol](https://www.reddit.com/r/Tkinter/comments/w84lt0/does_tkinter_button_command_only_accept_functions))
+    - `TK113`: Callback handler should be a callable
     - `TK121`: Using `time.sleep()` in tkinter code. Use `.after()` in some form instead.
     - `TK122`: Using an infinite loop in callback handler. Propose to use recursive function with `.after()`.
-    - `TK141`: Suggest keeping reference of local `PhotoImage` instance to avoid GC.
+    - `TK???`: Suggest keeping reference of local `PhotoImage` instance to avoid GC.
+    - `TK151`: Don't use `w.setup()` directly. Use init args, or `w.configure()`.
+    - Extend `TK111` and `Tk112` to check in `w.after()` calls.
 
 - Cross platform (TK181-TK199)
-    - `TK181`: Using `<Shift-Tab>` binding. It doesn't work on Linux.
+    - `TK181`: Using `<MouseWheel>` binding. It doesn't work on Linux with Tk 8.6 (use button4-5 instead)
+    - `TK182`: Using `<Shift-Tab>` binding. It doesn't work on Linux (use `<ISO_Left_Tab>` instead)
+    - `TK183`: Using `<Menu>` binding. It doesn't work on Windows (use `<App>` instead)
+    - `TK184`: Binding to control or alt with constant values. It probably won't work on macOS.
+    - `TK191`: Not calling `wait_visibility` before `wm_attributes("-alpha")`.
+    - `TK192`: Using `w.state("zoomed")`. It throws an error on Linux (and on mac too?). Use `wm_attributes("-zoomed", True)`
 
 - Best practices (TK201-TK299)
     - `TK222`: Using `tk.N+tk.S+tk.E+tk.W` and combinations like that. Use `tk.NSEW`, or some other constant instead.
     - `TK241`: Creating a widget without parent specified, and there is a container in the same scope.
+    - `TK252`: Using `tkinter.Menu` without `tearoff=False`
     - `TK261`: Using subsequent `wm_attributes` calls. It can take value pairs.
 
 - Code quality (TK301-TK399)
     - `TK301`: Suggest using more clear binding sequences, like `<Button-1>` instead of `<1>` and `<Key-a>` instead of `<a>`.
     - `TK302`: Suggest using more clear `tkinter.Text` indexes, like `end - 1 chars` instead of `end-1c`.
     - `TK303`: Using a float as `tkinter.Text` index. It works because how Tkinter translates Python objects to Tcl, but it shouldn't.
 
 - OO (TK401-TK499)
     - `TK401`: Consider refactoring a huge app with OOP.
     - `TK402`: Consider refactoring widget into separate class.
     
 - Opinionated rules (TK501-TK599)
     - `TK501`: Calling `mainloop()` on something other than the root window.
-    - `TK502`: Using things like `root.wm_title()`. Use `root.title()`. (But there should be exceptions, like `wm_attributes`)
+    - `TK502`: Using things like `root.wm_title()`. Use `root.title()`. (But there should be exceptions, like `wm_attributes`, and instead warn on plain `attributes`)
     - `TK503`: Using subscripting for widget cget and configure. Use `.cget()` and `.configure()` instead.
 
 
 ## Development
 1. Clone the repo
 2. Set up a virtual environment, activate, and install `flake8` and `pytest` in it
 3. Run `pip install -e .` to install `flake8-tkinter` in editable format
```

### Comparing `flake8_tkinter-0.5.4/README.md` & `flake8_tkinter-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,36 @@
+Metadata-Version: 2.1
+Name: flake8_tkinter
+Version: 0.6.0
+Summary: A flake8 plugin that helps you write better Tkinter code
+Home-page: https://github.com/rdbende/flake8-tkinter
+Author: rdbende
+Author-email: rdbende@gmail.com
+License: MIT license
+Project-URL: Tracker, https://github.com/rdbende/flake8-tkinter/issues
+Platform: UNKNOWN
+Classifier: Framework :: Flake8
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # flake8-tkinter
 
-A flake8 plugin that helps you detect (too) common mistakes and bad practices in you Tkinter project
+A [flake8](https://github.com/PyCQA/flake8) plugin that helps you write better Tkinter code
 
 _Project idea by [@insolor](https://github.com/insolor)_
 
 
 ## Installation
 
 ```
@@ -17,21 +43,21 @@
 Common mistakes
 - **`TK102`**: Using multiple mainloop calls is unnecessary. One call is perfectly enough. ([example](#tk102))
 - **`TK111`**: Calling `callback_handler()` instead of passing the reference for on-click or binding callback. ([example](#tk111))
 - **`TK112`**: Calling `callback_handler()` with arguments instead of passing the reference for on-click or binding callback. If you need to call `callback_handler` with arguments, use lambda or functools.partial. ([example](#tk112))
 - **`TK131`**: Assigning result of geometry manager call to a variable. ([example](#tk131))
 
 Best practices
+- **`TK141`**: Using bind without `add=True` will overwrite any existing bindings to this sequence on this widget. Either overwrite them explicitly with `add=False` or use `add=True` to keep existing bindings. ([example](#tk141))
+- **`TK142`**: Creating tag bindings in a loop can lead to memory leaks. Store the returned command names in a list to clean them up later. ([example](#tk142))
 - **`TK201`**: Using `from tkinter import *` is generally a bad practice and discouraged. Use `import tkinter as tk` or simply `import tkinter` instead. ([example](#tk201))
 - **`TK202`**: Using `from tkinter.ttk import *` is generally a bad practice and discouraged. Use `from tkinter import ttk` instead. ([example](#tk202))
 - **`TK211`**: Using `import tkinter.ttk as ttk` is pointless. Use `from tkinter import ttk` instead. ([example](#tk211))
 - **`TK221`**: Using tkinter.TRUE, tkinter.FALSE, etc. is pointless. Use an appropriate Python boolean instead. ([example](#tk221))
-- **`TK231`**: Using bind without `add=True` will overwrite any existing bindings to this sequence on this widget. Either overwrite them explicitly with `add=False` or use `add=True` to keep existing bindings. ([example](#tk231))
-- **`TK232`**: Creating tag bindings in a loop can lead to memory leaks. Store the returned command names in a list to clean them up later. ([example](#tk232))
-- **`TK251`**: Using `tkinter.Message` widget. It's redundant since `tkinter.Label` provides the same functionality.. ([example](#tk251)
+- **`TK251`**: Using `tkinter.Message` widget. It's redundant since `tkinter.Label` provides the same functionality. ([example](#tk251))
 
 Code quality
 - **`TK304`**: Value for `add` in bind methods should be a boolean. ([example](#tk304))
 
 Opinionated warnings
 - **`TK504`**: Using a tkinter constant. Use a string literal instead (disabled by default). ([example](#tk504))
 
@@ -131,41 +157,39 @@
 w.pack(expand=tk.OFF)
 
 # Good
 w.pack(expand=True)
 w.pack(expand=False)
 ```
 
-### TK231
-_Will be renamed to TK141 in v1.0.0_
+### TK141
 ```python
 # Bad
 w.bind("<Button-1>", foo)
 
 # Good
 w.bind("<Button-1>", foo, add=True)
 # OR
 w.bind("<Button-1>", foo, add=False)
 ```
 
-### TK232
-_Will be renamed to TK142 in v1.0.0_
+### TK142
 ```python
 # Bad
 for index, foo in enumerate(foos):
     w.tag_bind(f"bar_{index}", "<Button-1>", baz)
     
 # Good
 for index, foo in enumerate(foos):
     tcl_command = w.tag_bind(f"bar_{index}", "<Button-1>", baz)
     bindings.append(tcl_command)  # Clean them up later with `.deletecommand()`
 ```
 
 ### TK251
-_Yes, there's some minor diffrence in text wrapping difference, but that can be adjusted_
+_Yes, there's some minor diffrence in text wrapping, but that can be easily fixed
 ```python
 # Bad
 w = tkinter.Message()
 
 # Good
 w = tkinter.Label()
 ```
@@ -189,40 +213,50 @@
 ```
 
 ## Planned warnings
 
 - Common mistakes (TK101-TK179)
     - `TK101`: Using multiple `tkinter.Tk` instances. Child windows must be created from `tkinter.Toplevel`.
     - `TK103`: Suggest refactoring code that uses `.update()`, as it's usually pointless, [potentially harmful](https://wiki.tcl-lang.org/page/Update+considered+harmful), and considered a code smell.
-    - `TK113`: Callback handler should be a callable ([lol](https://www.reddit.com/r/Tkinter/comments/w84lt0/does_tkinter_button_command_only_accept_functions))
+    - `TK113`: Callback handler should be a callable
     - `TK121`: Using `time.sleep()` in tkinter code. Use `.after()` in some form instead.
     - `TK122`: Using an infinite loop in callback handler. Propose to use recursive function with `.after()`.
-    - `TK141`: Suggest keeping reference of local `PhotoImage` instance to avoid GC.
+    - `TK???`: Suggest keeping reference of local `PhotoImage` instance to avoid GC.
+    - `TK151`: Don't use `w.setup()` directly. Use init args, or `w.configure()`.
+    - Extend `TK111` and `Tk112` to check in `w.after()` calls.
 
 - Cross platform (TK181-TK199)
-    - `TK181`: Using `<Shift-Tab>` binding. It doesn't work on Linux.
+    - `TK181`: Using `<MouseWheel>` binding. It doesn't work on Linux with Tk 8.6 (use button4-5 instead)
+    - `TK182`: Using `<Shift-Tab>` binding. It doesn't work on Linux (use `<ISO_Left_Tab>` instead)
+    - `TK183`: Using `<Menu>` binding. It doesn't work on Windows (use `<App>` instead)
+    - `TK184`: Binding to control or alt with constant values. It probably won't work on macOS.
+    - `TK191`: Not calling `wait_visibility` before `wm_attributes("-alpha")`.
+    - `TK192`: Using `w.state("zoomed")`. It throws an error on Linux (and on mac too?). Use `wm_attributes("-zoomed", True)`
 
 - Best practices (TK201-TK299)
     - `TK222`: Using `tk.N+tk.S+tk.E+tk.W` and combinations like that. Use `tk.NSEW`, or some other constant instead.
     - `TK241`: Creating a widget without parent specified, and there is a container in the same scope.
+    - `TK252`: Using `tkinter.Menu` without `tearoff=False`
     - `TK261`: Using subsequent `wm_attributes` calls. It can take value pairs.
 
 - Code quality (TK301-TK399)
     - `TK301`: Suggest using more clear binding sequences, like `<Button-1>` instead of `<1>` and `<Key-a>` instead of `<a>`.
     - `TK302`: Suggest using more clear `tkinter.Text` indexes, like `end - 1 chars` instead of `end-1c`.
     - `TK303`: Using a float as `tkinter.Text` index. It works because how Tkinter translates Python objects to Tcl, but it shouldn't.
 
 - OO (TK401-TK499)
     - `TK401`: Consider refactoring a huge app with OOP.
     - `TK402`: Consider refactoring widget into separate class.
     
 - Opinionated rules (TK501-TK599)
     - `TK501`: Calling `mainloop()` on something other than the root window.
-    - `TK502`: Using things like `root.wm_title()`. Use `root.title()`. (But there should be exceptions, like `wm_attributes`)
+    - `TK502`: Using things like `root.wm_title()`. Use `root.title()`. (But there should be exceptions, like `wm_attributes`, and instead warn on plain `attributes`)
     - `TK503`: Using subscripting for widget cget and configure. Use `.cget()` and `.configure()` instead.
 
 
 ## Development
 1. Clone the repo
 2. Set up a virtual environment, activate, and install `flake8` and `pytest` in it
 3. Run `pip install -e .` to install `flake8-tkinter` in editable format
 4. Run `python3 -m pytest` to test your changes
+
+
```

### Comparing `flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_assign.py` & `flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_assign.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
 import ast
 
 from flake8_tkinter.constants import GM_METHODS
-from flake8_tkinter.utils import Error, is_attr_call, is_tkinter_namespace
-
-TK131 = "TK131 Assigning result of .{func}() call to a variable. {func}() returns None, not the widget object itself."
+from flake8_tkinter.utils import is_attr_call, is_tkinter_namespace
+from flake8_tkinter.messages import Error
 
 
 def detect_assign_to_gm_return(node: ast.Assign) -> list[Error] | None:
     for element in node.value.elts if isinstance(node.value, ast.Tuple) else [node.value]:
         if (
             is_attr_call(element)
             and is_attr_call(element.func.value)
             and isinstance(element.func.value.func.value, ast.Name)
             and is_tkinter_namespace(element.func.value.func.value.id)
             and element.func.attr in GM_METHODS
         ):
-            return [Error(node.lineno, node.col_offset, TK131.format(func=element.func.attr))]
+            return [Error(131, node.lineno, node.col_offset, func=element.func.attr)]
```

### Comparing `flake8_tkinter-0.5.4/flake8_tkinter/rules/ast_loop.py` & `flake8_tkinter-0.6.0/flake8_tkinter/rules/ast_loop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 from __future__ import annotations
 
 import ast
 
-from flake8_tkinter.utils import Error, is_attr_call, is_func
-
-TK232 = (
-    "TK232 "
-    "Creating tag bindings in a loop can lead to memory leaks. "
-    "Store the returned command names in a list to clean them up later."
-)
+from flake8_tkinter.utils import is_attr_call, is_func
+from flake8_tkinter.messages import Error
 
 
 def detect_tag_bind_in_loop_badly(node: ast.For | ast.While) -> list[Error] | None:
     tag_bind = False
     appended = False
-    tag_bind_pos = (0, 0)
-
-    elems = [
-        el for el in node.body if isinstance(el, (ast.Assign, ast.Expr)) and is_attr_call(el.value)
-    ]
+    line = col = 0
+    elems = [x for x in node.body if isinstance(x, (ast.Assign, ast.Expr)) and is_attr_call(x.value)]
 
     for expr in elems:
         if is_func(expr, "tag_bind"):
             tag_bind = True
-            tag_bind_pos = (expr.value.lineno, expr.value.col_offset)
+            line, col = expr.value.lineno, expr.value.col_offset
             variable = expr.targets[0].id if isinstance(expr, ast.Assign) else None
         elif tag_bind and is_func(expr, "append"):
             arg = expr.value.args[0] if len(expr.value.args) != 0 else None
             appended = isinstance(arg, ast.Name) and arg.id == variable
 
     if tag_bind and not appended:
-        return [Error(*tag_bind_pos, TK232)]
+        return [Error(142, line, col)]
```

### Comparing `flake8_tkinter-0.5.4/flake8_tkinter/utils.py` & `flake8_tkinter-0.6.0/flake8_tkinter/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from __future__ import annotations
 
 import ast
 from dataclasses import dataclass
 
 
 @dataclass
-class Error:
-    line: int
-    col: int
-    msg: str
-
-
-@dataclass
-class _Settings:
+class _State:
     mainloop_already_called: bool = False
     tkinter_used: bool = False
     tkinter_as: str = ""
     ttk_as: str = ""
 
+    def reset(self):
+        for field in self.__dataclass_fields__.values():
+            setattr(self, field.name, field.default)
+
 
-Settings = _Settings()
+State = _State()
 
 
 def is_tkinter_namespace(thing: str) -> bool:
-    return thing in {Settings.tkinter_as, Settings.ttk_as}
+    return thing in {State.tkinter_as, State.ttk_as}
 
 
 def is_functools_partial(node: ast.Call) -> bool:
     func = node.func
     if isinstance(func, ast.Name):
         return func.id in {"partial", "partialmethod"}
     elif isinstance(func, ast.Attribute):
```

### Comparing `flake8_tkinter-0.5.4/flake8_tkinter/visitor.py` & `flake8_tkinter-0.6.0/flake8_tkinter/visitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 )
 from flake8_tkinter.rules.ast_import import detect_import_tkinter_dot_ttk_as_ttk
 from flake8_tkinter.rules.ast_import_from import (
     detect_from_tkinter_dot_ttk_import_star,
     detect_from_tkinter_import_star,
 )
 from flake8_tkinter.rules.ast_loop import detect_tag_bind_in_loop_badly
-from flake8_tkinter.utils import Error, Settings, get_ancestors
+from flake8_tkinter.utils import State, get_ancestors
+from flake8_tkinter.messages import Error
 
 
 class Visitor(ast.NodeVisitor):
     def __init__(self) -> None:
         self.errors: list[Error] = []
 
     def visit_Assign(self, node: ast.Assign) -> None:
@@ -37,51 +38,46 @@
     def visit_Attribute(self, node: ast.Attribute) -> None:
         self.extend(detect_use_of_dumb_constant(node))
         self.extend(detect_use_of_tkinter_constant(node))
         self.extend(detect_use_of_tkinter_dot_message(node))
 
         self.generic_visit(node)
 
-    def visit_BindMethod(self, node: ast.Call) -> None:
-        self.extend(detect_bind_add_is_not_boolean(node))
-        self.extend(detect_bind_add_missing(node))
-        self.extend(detect_called_func_bind(node))
-
     def visit_Call(self, node: ast.Call) -> None:
         self.extend(detect_called_func_command_arg(node))
         self.extend(detect_multiple_mainloop_calls(node))
 
         if (
             isinstance(node.func, ast.Attribute)
             and isinstance(node.func.value, ast.Name)  # TODO: can it be something else?
             and node.func.attr in BIND_METHODS | {"tag_bind"}
         ):
-            self.visit_BindMethod(node)
+            self.visit_tkinter_bind_method(node)
 
         self.generic_visit(node)
 
     def visit_Import(self, node: ast.Import) -> None:
         for name in node.names:
             if name.name == "tkinter":
-                Settings.tkinter_used = True
-                Settings.tkinter_as = name.asname or name.name
+                State.tkinter_used = True
+                State.tkinter_as = name.asname or name.name
             elif name.name == "tkinter.ttk":
-                Settings.tkinter_used = True
-                Settings.ttk_as = name.asname or name.name
+                State.tkinter_used = True
+                State.ttk_as = name.asname or name.name
 
         self.extend(detect_import_tkinter_dot_ttk_as_ttk(node))
 
         self.generic_visit(node)
 
     def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
-        if node.module == "tkinter":
-            Settings.tkinter_used = True
+        if node.module in ("tkinter", "tkinter.ttk"):
+            State.tkinter_used = True
             for name in node.names:
                 if name.name == "ttk":
-                    Settings.ttk_as = name.asname or name.name
+                    State.ttk_as = name.asname or name.name
 
         self.extend(detect_from_tkinter_dot_ttk_import_star(node))
         self.extend(detect_from_tkinter_import_star(node))
 
         self.generic_visit(node)
 
     def visit_For(self, node: ast.For) -> None:
@@ -111,10 +107,15 @@
     def visit_Try(self, node: ast.Try) -> None:
         ancestors = get_ancestors(node)
         if ast.For in ancestors or ast.While in ancestors:
             self.extend(detect_tag_bind_in_loop_badly(node))
 
         self.generic_visit(node)
 
+    def visit_tkinter_bind_method(self, node: ast.Call) -> None:
+        self.extend(detect_bind_add_is_not_boolean(node))
+        self.extend(detect_bind_add_missing(node))
+        self.extend(detect_called_func_bind(node))
+
     def extend(self, error: list[Error] | None) -> None:
-        if Settings.tkinter_used and error:
+        if State.tkinter_used and error:
             self.errors += error
```

### Comparing `flake8_tkinter-0.5.4/flake8_tkinter.egg-info/PKG-INFO` & `flake8_tkinter-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-Metadata-Version: 2.1
-Name: flake8-tkinter
-Version: 0.5.4
-Summary: Flake8 plugin to detect (too) common mistakes and bad practices in Tkinter projects
-Home-page: https://github.com/rdbende/flake8-tkinter
-Author: rdbende
-Author-email: rdbende@gmail.com
-License: MIT license
-Platform: UNKNOWN
-Classifier: Framework :: Flake8
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # flake8-tkinter
 
-A flake8 plugin that helps you detect (too) common mistakes and bad practices in you Tkinter project
+A [flake8](https://github.com/PyCQA/flake8) plugin that helps you write better Tkinter code
 
 _Project idea by [@insolor](https://github.com/insolor)_
 
 
 ## Installation
 
 ```
@@ -41,21 +17,21 @@
 Common mistakes
 - **`TK102`**: Using multiple mainloop calls is unnecessary. One call is perfectly enough. ([example](#tk102))
 - **`TK111`**: Calling `callback_handler()` instead of passing the reference for on-click or binding callback. ([example](#tk111))
 - **`TK112`**: Calling `callback_handler()` with arguments instead of passing the reference for on-click or binding callback. If you need to call `callback_handler` with arguments, use lambda or functools.partial. ([example](#tk112))
 - **`TK131`**: Assigning result of geometry manager call to a variable. ([example](#tk131))
 
 Best practices
+- **`TK141`**: Using bind without `add=True` will overwrite any existing bindings to this sequence on this widget. Either overwrite them explicitly with `add=False` or use `add=True` to keep existing bindings. ([example](#tk141))
+- **`TK142`**: Creating tag bindings in a loop can lead to memory leaks. Store the returned command names in a list to clean them up later. ([example](#tk142))
 - **`TK201`**: Using `from tkinter import *` is generally a bad practice and discouraged. Use `import tkinter as tk` or simply `import tkinter` instead. ([example](#tk201))
 - **`TK202`**: Using `from tkinter.ttk import *` is generally a bad practice and discouraged. Use `from tkinter import ttk` instead. ([example](#tk202))
 - **`TK211`**: Using `import tkinter.ttk as ttk` is pointless. Use `from tkinter import ttk` instead. ([example](#tk211))
 - **`TK221`**: Using tkinter.TRUE, tkinter.FALSE, etc. is pointless. Use an appropriate Python boolean instead. ([example](#tk221))
-- **`TK231`**: Using bind without `add=True` will overwrite any existing bindings to this sequence on this widget. Either overwrite them explicitly with `add=False` or use `add=True` to keep existing bindings. ([example](#tk231))
-- **`TK232`**: Creating tag bindings in a loop can lead to memory leaks. Store the returned command names in a list to clean them up later. ([example](#tk232))
-- **`TK251`**: Using `tkinter.Message` widget. It's redundant since `tkinter.Label` provides the same functionality.. ([example](#tk251)
+- **`TK251`**: Using `tkinter.Message` widget. It's redundant since `tkinter.Label` provides the same functionality. ([example](#tk251))
 
 Code quality
 - **`TK304`**: Value for `add` in bind methods should be a boolean. ([example](#tk304))
 
 Opinionated warnings
 - **`TK504`**: Using a tkinter constant. Use a string literal instead (disabled by default). ([example](#tk504))
 
@@ -155,41 +131,39 @@
 w.pack(expand=tk.OFF)
 
 # Good
 w.pack(expand=True)
 w.pack(expand=False)
 ```
 
-### TK231
-_Will be renamed to TK141 in v1.0.0_
+### TK141
 ```python
 # Bad
 w.bind("<Button-1>", foo)
 
 # Good
 w.bind("<Button-1>", foo, add=True)
 # OR
 w.bind("<Button-1>", foo, add=False)
 ```
 
-### TK232
-_Will be renamed to TK142 in v1.0.0_
+### TK142
 ```python
 # Bad
 for index, foo in enumerate(foos):
     w.tag_bind(f"bar_{index}", "<Button-1>", baz)
     
 # Good
 for index, foo in enumerate(foos):
     tcl_command = w.tag_bind(f"bar_{index}", "<Button-1>", baz)
     bindings.append(tcl_command)  # Clean them up later with `.deletecommand()`
 ```
 
 ### TK251
-_Yes, there's some minor diffrence in text wrapping difference, but that can be adjusted_
+_Yes, there's some minor diffrence in text wrapping, but that can be easily fixed
 ```python
 # Bad
 w = tkinter.Message()
 
 # Good
 w = tkinter.Label()
 ```
@@ -213,42 +187,48 @@
 ```
 
 ## Planned warnings
 
 - Common mistakes (TK101-TK179)
     - `TK101`: Using multiple `tkinter.Tk` instances. Child windows must be created from `tkinter.Toplevel`.
     - `TK103`: Suggest refactoring code that uses `.update()`, as it's usually pointless, [potentially harmful](https://wiki.tcl-lang.org/page/Update+considered+harmful), and considered a code smell.
-    - `TK113`: Callback handler should be a callable ([lol](https://www.reddit.com/r/Tkinter/comments/w84lt0/does_tkinter_button_command_only_accept_functions))
+    - `TK113`: Callback handler should be a callable
     - `TK121`: Using `time.sleep()` in tkinter code. Use `.after()` in some form instead.
     - `TK122`: Using an infinite loop in callback handler. Propose to use recursive function with `.after()`.
-    - `TK141`: Suggest keeping reference of local `PhotoImage` instance to avoid GC.
+    - `TK???`: Suggest keeping reference of local `PhotoImage` instance to avoid GC.
+    - `TK151`: Don't use `w.setup()` directly. Use init args, or `w.configure()`.
+    - Extend `TK111` and `Tk112` to check in `w.after()` calls.
 
 - Cross platform (TK181-TK199)
-    - `TK181`: Using `<Shift-Tab>` binding. It doesn't work on Linux.
+    - `TK181`: Using `<MouseWheel>` binding. It doesn't work on Linux with Tk 8.6 (use button4-5 instead)
+    - `TK182`: Using `<Shift-Tab>` binding. It doesn't work on Linux (use `<ISO_Left_Tab>` instead)
+    - `TK183`: Using `<Menu>` binding. It doesn't work on Windows (use `<App>` instead)
+    - `TK184`: Binding to control or alt with constant values. It probably won't work on macOS.
+    - `TK191`: Not calling `wait_visibility` before `wm_attributes("-alpha")`.
+    - `TK192`: Using `w.state("zoomed")`. It throws an error on Linux (and on mac too?). Use `wm_attributes("-zoomed", True)`
 
 - Best practices (TK201-TK299)
     - `TK222`: Using `tk.N+tk.S+tk.E+tk.W` and combinations like that. Use `tk.NSEW`, or some other constant instead.
     - `TK241`: Creating a widget without parent specified, and there is a container in the same scope.
+    - `TK252`: Using `tkinter.Menu` without `tearoff=False`
     - `TK261`: Using subsequent `wm_attributes` calls. It can take value pairs.
 
 - Code quality (TK301-TK399)
     - `TK301`: Suggest using more clear binding sequences, like `<Button-1>` instead of `<1>` and `<Key-a>` instead of `<a>`.
     - `TK302`: Suggest using more clear `tkinter.Text` indexes, like `end - 1 chars` instead of `end-1c`.
     - `TK303`: Using a float as `tkinter.Text` index. It works because how Tkinter translates Python objects to Tcl, but it shouldn't.
 
 - OO (TK401-TK499)
     - `TK401`: Consider refactoring a huge app with OOP.
     - `TK402`: Consider refactoring widget into separate class.
     
 - Opinionated rules (TK501-TK599)
     - `TK501`: Calling `mainloop()` on something other than the root window.
-    - `TK502`: Using things like `root.wm_title()`. Use `root.title()`. (But there should be exceptions, like `wm_attributes`)
+    - `TK502`: Using things like `root.wm_title()`. Use `root.title()`. (But there should be exceptions, like `wm_attributes`, and instead warn on plain `attributes`)
     - `TK503`: Using subscripting for widget cget and configure. Use `.cget()` and `.configure()` instead.
 
 
 ## Development
 1. Clone the repo
 2. Set up a virtual environment, activate, and install `flake8` and `pytest` in it
 3. Run `pip install -e .` to install `flake8-tkinter` in editable format
 4. Run `python3 -m pytest` to test your changes
-
-
```

### Comparing `flake8_tkinter-0.5.4/flake8_tkinter.egg-info/SOURCES.txt` & `flake8_tkinter-0.6.0/flake8_tkinter.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 flake8_tkinter/__init__.py
 flake8_tkinter/constants.py
+flake8_tkinter/messages.py
 flake8_tkinter/utils.py
 flake8_tkinter/visitor.py
 flake8_tkinter.egg-info/PKG-INFO
 flake8_tkinter.egg-info/SOURCES.txt
 flake8_tkinter.egg-info/dependency_links.txt
 flake8_tkinter.egg-info/entry_points.txt
 flake8_tkinter.egg-info/requires.txt
```

### Comparing `flake8_tkinter-0.5.4/setup.py` & `flake8_tkinter-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from setuptools import setup
-from flake8_tkinter import __version__
 
+from flake8_tkinter import __version__
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 flake8_entry_point = "TK = flake8_tkinter:Plugin"
 
 
 setup(
     name="flake8_tkinter",
     version=__version__,
-    description="Flake8 plugin to detect (too) common mistakes and bad practices in Tkinter projects",
+    description="A flake8 plugin that helps you write better Tkinter code",
     author="rdbende",
     author_email="rdbende@gmail.com",
     url="https://github.com/rdbende/flake8-tkinter",
+    project_urls={
+        "Tracker": "https://github.com/rdbende/flake8-tkinter/issues",
+    },
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
     install_requires=["flake8>=3.7"],
     packages=["flake8_tkinter", "flake8_tkinter/rules"],
     entry_points={"flake8.extension": ["TK = flake8_tkinter:Plugin"]},
     license="MIT license",
@@ -29,11 +32,12 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Quality Assurance",
     ],
 )
```

