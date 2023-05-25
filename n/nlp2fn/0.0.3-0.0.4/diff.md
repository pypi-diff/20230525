# Comparing `tmp/nlp2fn-0.0.3.tar.gz` & `tmp/nlp2fn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp2fn-0.0.3.tar", last modified: Wed May 24 13:25:17 2023, max compression
+gzip compressed data, was "nlp2fn-0.0.4.tar", last modified: Thu May 25 20:51:53 2023, max compression
```

## Comparing `nlp2fn-0.0.3.tar` & `nlp2fn-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.316139 nlp2fn-0.0.3/
--rw-r--r--   0 jennie     (502) staff       (20)     2742 2023-05-24 13:25:17.315969 nlp2fn-0.0.3/PKG-INFO
--rw-r--r--   0 jennie     (502) staff       (20)     2208 2023-05-24 13:22:33.000000 nlp2fn-0.0.3/README.md
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.312805 nlp2fn-0.0.3/nlp2fn/
--rw-r--r--   0 jennie     (502) staff       (20)     2038 2023-05-24 13:17:43.000000 nlp2fn-0.0.3/nlp2fn/__init__.py
--rw-r--r--   0 jennie     (502) staff       (20)      810 2023-05-24 13:20:40.000000 nlp2fn-0.0.3/nlp2fn/clonefromgit.py
--rw-r--r--   0 jennie     (502) staff       (20)        0 2023-05-20 21:04:58.000000 nlp2fn-0.0.3/nlp2fn/constants.py
--rw-r--r--   0 jennie     (502) staff       (20)     2732 2023-05-20 22:48:22.000000 nlp2fn-0.0.3/nlp2fn/fncloader.py
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.314212 nlp2fn-0.0.3/nlp2fn/git/
--rw-r--r--   0 jennie     (502) staff       (20)       25 2023-05-24 12:25:45.000000 nlp2fn-0.0.3/nlp2fn/git/__init__.py
--rw-r--r--   0 jennie     (502) staff       (20)     3994 2023-05-24 12:18:57.000000 nlp2fn-0.0.3/nlp2fn/git/repo.py
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.315564 nlp2fn-0.0.3/nlp2fn/utils/
--rw-r--r--   0 jennie     (502) staff       (20)     1950 2023-05-24 13:20:25.000000 nlp2fn-0.0.3/nlp2fn/utils/__init__.py
--rw-r--r--   0 jennie     (502) staff       (20)      542 2023-05-20 22:26:48.000000 nlp2fn-0.0.3/nlp2fn/utils/colorpriniting.py
--rw-r--r--   0 jennie     (502) staff       (20)      687 2023-05-24 13:16:04.000000 nlp2fn-0.0.3/nlp2fn/utils/commands.py
--rw-r--r--   0 jennie     (502) staff       (20)     2143 2023-05-19 22:37:53.000000 nlp2fn-0.0.3/nlp2fn/utils/configparser.py
--rw-r--r--   0 jennie     (502) staff       (20)     3395 2023-05-19 22:40:17.000000 nlp2fn-0.0.3/nlp2fn/utils/detectenv.py
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.313812 nlp2fn-0.0.3/nlp2fn.egg-info/
--rw-r--r--   0 jennie     (502) staff       (20)     2742 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/PKG-INFO
--rw-r--r--   0 jennie     (502) staff       (20)      460 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/SOURCES.txt
--rw-r--r--   0 jennie     (502) staff       (20)        1 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/dependency_links.txt
--rw-r--r--   0 jennie     (502) staff       (20)       42 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/entry_points.txt
--rw-r--r--   0 jennie     (502) staff       (20)        9 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/requires.txt
--rw-r--r--   0 jennie     (502) staff       (20)       14 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/top_level.txt
--rw-r--r--   0 jennie     (502) staff       (20)       38 2023-05-24 13:25:17.316205 nlp2fn-0.0.3/setup.cfg
--rw-r--r--   0 jennie     (502) staff       (20)     1000 2023-05-24 13:25:12.000000 nlp2fn-0.0.3/setup.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-25 20:51:53.017938 nlp2fn-0.0.4/
+-rw-r--r--   0 jennie     (502) staff       (20)     3046 2023-05-25 20:51:53.017767 nlp2fn-0.0.4/PKG-INFO
+-rw-r--r--   0 jennie     (502) staff       (20)     2512 2023-05-25 20:51:36.000000 nlp2fn-0.0.4/README.md
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-25 20:51:53.013435 nlp2fn-0.0.4/nlp2fn/
+-rw-r--r--   0 jennie     (502) staff       (20)     1027 2023-05-25 20:47:23.000000 nlp2fn-0.0.4/nlp2fn/__init__.py
+-rw-r--r--   0 jennie     (502) staff       (20)      810 2023-05-24 13:20:40.000000 nlp2fn-0.0.4/nlp2fn/clonefromgit.py
+-rw-r--r--   0 jennie     (502) staff       (20)     4998 2023-05-25 20:47:23.000000 nlp2fn-0.0.4/nlp2fn/interface.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-25 20:51:53.015175 nlp2fn-0.0.4/nlp2fn/sourcehandler/
+-rw-r--r--   0 jennie     (502) staff       (20)       56 2023-05-25 19:33:11.000000 nlp2fn-0.0.4/nlp2fn/sourcehandler/__init__.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-25 20:51:53.015676 nlp2fn-0.0.4/nlp2fn/sourcehandler/git/
+-rw-r--r--   0 jennie     (502) staff       (20)       34 2023-05-25 16:16:17.000000 nlp2fn-0.0.4/nlp2fn/sourcehandler/git/__init__.py
+-rw-r--r--   0 jennie     (502) staff       (20)     4051 2023-05-25 17:17:49.000000 nlp2fn-0.0.4/nlp2fn/sourcehandler/git/repo.py
+-rw-r--r--   0 jennie     (502) staff       (20)     4545 2023-05-25 20:20:59.000000 nlp2fn-0.0.4/nlp2fn/sourcehandler/helper.py
+-rw-r--r--   0 jennie     (502) staff       (20)     5692 2023-05-25 20:47:23.000000 nlp2fn-0.0.4/nlp2fn/sourcehandler/sourcemodel.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-25 20:51:53.017458 nlp2fn-0.0.4/nlp2fn/utils/
+-rw-r--r--   0 jennie     (502) staff       (20)     2083 2023-05-24 19:47:32.000000 nlp2fn-0.0.4/nlp2fn/utils/__init__.py
+-rw-r--r--   0 jennie     (502) staff       (20)      542 2023-05-20 22:26:48.000000 nlp2fn-0.0.4/nlp2fn/utils/colorpriniting.py
+-rw-r--r--   0 jennie     (502) staff       (20)      681 2023-05-25 20:47:23.000000 nlp2fn-0.0.4/nlp2fn/utils/commands.py
+-rw-r--r--   0 jennie     (502) staff       (20)     2143 2023-05-19 22:37:53.000000 nlp2fn-0.0.4/nlp2fn/utils/configparser.py
+-rw-r--r--   0 jennie     (502) staff       (20)     3395 2023-05-19 22:40:17.000000 nlp2fn-0.0.4/nlp2fn/utils/detectenv.py
+-rw-r--r--   0 jennie     (502) staff       (20)      726 2023-05-25 20:16:47.000000 nlp2fn-0.0.4/nlp2fn/utils/fncloader.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-25 20:51:53.014500 nlp2fn-0.0.4/nlp2fn.egg-info/
+-rw-r--r--   0 jennie     (502) staff       (20)     3046 2023-05-25 20:51:53.000000 nlp2fn-0.0.4/nlp2fn.egg-info/PKG-INFO
+-rw-r--r--   0 jennie     (502) staff       (20)      594 2023-05-25 20:51:53.000000 nlp2fn-0.0.4/nlp2fn.egg-info/SOURCES.txt
+-rw-r--r--   0 jennie     (502) staff       (20)        1 2023-05-25 20:51:53.000000 nlp2fn-0.0.4/nlp2fn.egg-info/dependency_links.txt
+-rw-r--r--   0 jennie     (502) staff       (20)       42 2023-05-25 20:51:53.000000 nlp2fn-0.0.4/nlp2fn.egg-info/entry_points.txt
+-rw-r--r--   0 jennie     (502) staff       (20)        9 2023-05-25 20:51:53.000000 nlp2fn-0.0.4/nlp2fn.egg-info/requires.txt
+-rw-r--r--   0 jennie     (502) staff       (20)       14 2023-05-25 20:51:53.000000 nlp2fn-0.0.4/nlp2fn.egg-info/top_level.txt
+-rw-r--r--   0 jennie     (502) staff       (20)       38 2023-05-25 20:51:53.017985 nlp2fn-0.0.4/setup.cfg
+-rw-r--r--   0 jennie     (502) staff       (20)     1000 2023-05-25 20:50:26.000000 nlp2fn-0.0.4/setup.py
```

### Comparing `nlp2fn-0.0.3/PKG-INFO` & `nlp2fn-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp2fn
-Version: 0.0.3
+Version: 0.0.4
 Summary: With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together.
 Home-page: https://github.com/dextrop/nlp2fn
 Author: Jennie Developers <saurabh@ask-jennie.com>
 Author-email: Jennie Developers <saurabh@ask-jennie.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -19,15 +19,15 @@
 
 A typical function for `nlp2fn` follows this format:
 
 ```python
 # Write you execute statement, this shall be an 
 # input by user to execute your events, make sure all the 
 # parameters that are required by event is properly captured with {param_name}.
-statement = "download {link} to {output_dir}"
+STATEMENT = "download {link} to {output_dir}"
 
 
 # This shall be the main function for your event. once 
 def execute(args):
     file = args[0]
     output_dir = args[1]
     
@@ -44,21 +44,21 @@
 ```bash
 pip install nlp2fn
 ```
 
 Next, add the source directory where your Python functions are located:
 
 ```bash
-nlp2fn set-source local /path/to/directory
+nlp2fn add-source /path/to/directory
 ```
 
 or 
 
 ```bash
-nlp2fn set-source git https://github.com/{githubid}/{repo}
+nlp2fn add-source https://github.com/{githubid}/{repo}
 ```
 
 make sure repo is public.
 
 
 Ready to launch `nlp2fn` as a chatbot? Use this command:
 
@@ -74,18 +74,34 @@
 
 If you need to reset your sources, simply use the `reset` command:
 
 ```bash
 nlp2fn reset
 ```
 
+If you need to remove any source your sources, simply use the `delete ` command:
+
+```bash
+nlp2fn delete
+```
+
+If you need to update the source, both remote or local use `update` command
+
+```bash
+nlp2fn update
+```
+
 ## Join the Development
 
 We welcome your contributions! Feel free to submit pull requests and create issues on our [GitHub page](https://github.com/dextrop/nlp2fn/issues).
 
+## View ChangeLog
+
+[GitHub Release page](https://github.com/dextrop/nlp2fn/blob/main/CHANGELOG.md).
+
 ## Contact
 
 For questions, suggestions, or any kind of discussion, feel free to open an issue on our GitHub page.
 
 Embrace the simplification of Python automation with `nlp2fn`.
 
 ## Events
```

### Comparing `nlp2fn-0.0.3/README.md` & `nlp2fn-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 A typical function for `nlp2fn` follows this format:
 
 ```python
 # Write you execute statement, this shall be an 
 # input by user to execute your events, make sure all the 
 # parameters that are required by event is properly captured with {param_name}.
-statement = "download {link} to {output_dir}"
+STATEMENT = "download {link} to {output_dir}"
 
 
 # This shall be the main function for your event. once 
 def execute(args):
     file = args[0]
     output_dir = args[1]
     
@@ -32,21 +32,21 @@
 ```bash
 pip install nlp2fn
 ```
 
 Next, add the source directory where your Python functions are located:
 
 ```bash
-nlp2fn set-source local /path/to/directory
+nlp2fn add-source /path/to/directory
 ```
 
 or 
 
 ```bash
-nlp2fn set-source git https://github.com/{githubid}/{repo}
+nlp2fn add-source https://github.com/{githubid}/{repo}
 ```
 
 make sure repo is public.
 
 
 Ready to launch `nlp2fn` as a chatbot? Use this command:
 
@@ -62,18 +62,34 @@
 
 If you need to reset your sources, simply use the `reset` command:
 
 ```bash
 nlp2fn reset
 ```
 
+If you need to remove any source your sources, simply use the `delete ` command:
+
+```bash
+nlp2fn delete
+```
+
+If you need to update the source, both remote or local use `update` command
+
+```bash
+nlp2fn update
+```
+
 ## Join the Development
 
 We welcome your contributions! Feel free to submit pull requests and create issues on our [GitHub page](https://github.com/dextrop/nlp2fn/issues).
 
+## View ChangeLog
+
+[GitHub Release page](https://github.com/dextrop/nlp2fn/blob/main/CHANGELOG.md).
+
 ## Contact
 
 For questions, suggestions, or any kind of discussion, feel free to open an issue on our GitHub page.
 
 Embrace the simplification of Python automation with `nlp2fn`.
 
 ## Events
```

### Comparing `nlp2fn-0.0.3/nlp2fn/clonefromgit.py` & `nlp2fn-0.0.4/nlp2fn/clonefromgit.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.3/nlp2fn/git/repo.py` & `nlp2fn-0.0.4/nlp2fn/sourcehandler/git/repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import subprocess
 
 
 class Repo:
-    def __init__(self, path):
+    def __init__(self, working_dir):
         """
         Initializes a Repo object with the given path to the repository.
         """
-        self.path = path
+        self.working_dir = working_dir
 
     def run_command(self, command):
         """
         Runs the specified command as a subprocess in the repository's working directory.
 
         Args:
             command (list): A list containing the command and its arguments.
 
         Returns:
             str: The output of the command as a string.
         """
-        result = subprocess.run(command, cwd=self.path, capture_output=True, text=True)
+        result = subprocess.run(command, cwd=self.working_dir, capture_output=True, text=True)
         return result.stdout.strip()
 
     def clone(self, url):
         """
         Clones a Git repository from the specified URL into the repository's working directory.
 
         Args:
             url (str): The URL of the repository to clone.
 
         Returns:
             str: The output of the clone command.
         """
-        return self.run_command(['git', 'clone', url, self.path])
+        name = url.split("/")[-1]
+        return self.run_command(['git', 'clone', url, name])
 
     def commit(self, message):
         """
         Commits the changes in the repository with the specified commit message.
 
         Args:
             message (str): The commit message.
```

### Comparing `nlp2fn-0.0.3/nlp2fn/utils/__init__.py` & `nlp2fn-0.0.4/nlp2fn/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,21 +42,27 @@
         directory (str): The directory to add. Can be a local filesystem path or a URL.
     """
 
     # If the directory doesn't start with "http", assume it's a filesystem path.
     if not os.path.exists(directory):
         raise ValueError(f"Directory {directory} does not exits")
 
+    if not os.path.exists(TOKEN_PATH):
+        open(TOKEN_PATH, "w").write("")
+
     lines = open(TOKEN_PATH).read().splitlines()
     if directory in lines:
         error("Source Already Exits")
         return
 
     with open(TOKEN_PATH, 'a') as file:
         file.write(f"{directory}\n")
 
     return get_py_fnc_dir()
 
 def delete_py_fnc_dir_info():
-    os.remove(TOKEN_PATH)
+    try:
+        os.remove(TOKEN_PATH)
+    except Exception as e:
+        pass
```

### Comparing `nlp2fn-0.0.3/nlp2fn/utils/colorpriniting.py` & `nlp2fn-0.0.4/nlp2fn/utils/colorpriniting.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.3/nlp2fn/utils/configparser.py` & `nlp2fn-0.0.4/nlp2fn/utils/configparser.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.3/nlp2fn/utils/detectenv.py` & `nlp2fn-0.0.4/nlp2fn/utils/detectenv.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.3/nlp2fn.egg-info/PKG-INFO` & `nlp2fn-0.0.4/nlp2fn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp2fn
-Version: 0.0.3
+Version: 0.0.4
 Summary: With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together.
 Home-page: https://github.com/dextrop/nlp2fn
 Author: Jennie Developers <saurabh@ask-jennie.com>
 Author-email: Jennie Developers <saurabh@ask-jennie.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -19,15 +19,15 @@
 
 A typical function for `nlp2fn` follows this format:
 
 ```python
 # Write you execute statement, this shall be an 
 # input by user to execute your events, make sure all the 
 # parameters that are required by event is properly captured with {param_name}.
-statement = "download {link} to {output_dir}"
+STATEMENT = "download {link} to {output_dir}"
 
 
 # This shall be the main function for your event. once 
 def execute(args):
     file = args[0]
     output_dir = args[1]
     
@@ -44,21 +44,21 @@
 ```bash
 pip install nlp2fn
 ```
 
 Next, add the source directory where your Python functions are located:
 
 ```bash
-nlp2fn set-source local /path/to/directory
+nlp2fn add-source /path/to/directory
 ```
 
 or 
 
 ```bash
-nlp2fn set-source git https://github.com/{githubid}/{repo}
+nlp2fn add-source https://github.com/{githubid}/{repo}
 ```
 
 make sure repo is public.
 
 
 Ready to launch `nlp2fn` as a chatbot? Use this command:
 
@@ -74,18 +74,34 @@
 
 If you need to reset your sources, simply use the `reset` command:
 
 ```bash
 nlp2fn reset
 ```
 
+If you need to remove any source your sources, simply use the `delete ` command:
+
+```bash
+nlp2fn delete
+```
+
+If you need to update the source, both remote or local use `update` command
+
+```bash
+nlp2fn update
+```
+
 ## Join the Development
 
 We welcome your contributions! Feel free to submit pull requests and create issues on our [GitHub page](https://github.com/dextrop/nlp2fn/issues).
 
+## View ChangeLog
+
+[GitHub Release page](https://github.com/dextrop/nlp2fn/blob/main/CHANGELOG.md).
+
 ## Contact
 
 For questions, suggestions, or any kind of discussion, feel free to open an issue on our GitHub page.
 
 Embrace the simplification of Python automation with `nlp2fn`.
 
 ## Events
```

### Comparing `nlp2fn-0.0.3/setup.py` & `nlp2fn-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __description__ = 'With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together.'
 __author__ = 'Jennie Developers <saurabh@ask-jennie.com>'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

