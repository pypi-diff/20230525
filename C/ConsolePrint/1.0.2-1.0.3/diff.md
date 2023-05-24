# Comparing `tmp/consoleprint-1.0.2.tar.gz` & `tmp/consoleprint-1.0.3.tar.gz`

## Comparing `consoleprint-1.0.2.tar` & `consoleprint-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.0.2/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 consoleprint-1.0.2/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 consoleprint-1.0.2/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.0.2/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 consoleprint-1.0.2/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.0.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.0.2/LICENSE
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 consoleprint-1.0.2/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 consoleprint-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 consoleprint-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 consoleprint-1.0.3/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 consoleprint-1.0.3/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 consoleprint-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 consoleprint-1.0.3/PKG-INFO
```

### Comparing `consoleprint-1.0.2/src/ConsolePrint/console2file.py` & `consoleprint-1.0.3/src/ConsolePrint/console2file.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
             subprocess.Popen(["start", "", filename], shell=True)
         except FileNotFoundError:
             print("File not found.")
         except OSError:
             print("Error opening file.")
 
 
-
 if __name__ == "__main__":
     print("Running module test")
     import calendar
     
     startConsoleSave()
     
     print("Printing Calendar")
```

### Comparing `consoleprint-1.0.2/src/ConsolePrint/loading.py` & `consoleprint-1.0.3/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.0.2/LICENSE` & `consoleprint-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.0.2/README.md` & `consoleprint-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 # ConsolePrint
 This module making printing to the terminal more exciting by animating the text output.
 You can also save routine console output to a file using the console2file module.
 Created using python 3.11
 
 # Installation
 You may install it form PyPI.org using the pip command.
+
 pip install ConsolePrint
 
 # Usage
-Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output with IDLE.
-You may change the arguments as desired
+Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output on some terminals.
+
+import ConsolePrint.animate as prt    
 
-import ConsolePrint.animate as prt       
 import ConsolePrint.console2file as file  
+
 import ConsolePrint.loading as load        
 
 # Test Cases
+You may change the arguments as desired
+
 file.startConsoleSave()
+
 'Saves all output between the start and end functions to file.'
+
 from calendar import calendar
+
 print(calendar(2023))
+
 file.endConsoleSave()
 
 prt.printing("hello this should print letter by letter", delay=0.05, style="letter", new_line=True, rev=False)
+
 prt.printing("hello this should print word by word but in reverse", delay=0.05, style="word", new_line=True, rev=True)
+
 prt.flashprint("The entire text should flash", flashes=5, delay=0.2, stay=True)
+
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2)
+
 prt.animate1("This text is animated with #", symbol="#")
+
 prt.animate2("Prints letter by letter but masked with # first", symbol="#", delay=0.05)
+
 prt.text_box("M O N E Y  M A K E R", symbol="$", padding=True, wall=True)
+
 load.countdown(5)
+
 load.loading1(10)
+
 print()
+
 load.loading2(5)
+
 print()
+
 load.loading3(5)
 
 # License
 This project is given free for use and download under the MIT license.
 
 # Project Status
 Still undergoing enhancements.
```

### Comparing `consoleprint-1.0.2/pyproject.toml` & `consoleprint-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate print output to console"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `consoleprint-1.0.2/PKG-INFO` & `consoleprint-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package to animate print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,43 +15,63 @@
 # ConsolePrint
 This module making printing to the terminal more exciting by animating the text output.
 You can also save routine console output to a file using the console2file module.
 Created using python 3.11
 
 # Installation
 You may install it form PyPI.org using the pip command.
+
 pip install ConsolePrint
 
 # Usage
-Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output with IDLE.
-You may change the arguments as desired
+Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output on some terminals.
+
+import ConsolePrint.animate as prt    
 
-import ConsolePrint.animate as prt       
 import ConsolePrint.console2file as file  
+
 import ConsolePrint.loading as load        
 
 # Test Cases
+You may change the arguments as desired
+
 file.startConsoleSave()
+
 'Saves all output between the start and end functions to file.'
+
 from calendar import calendar
+
 print(calendar(2023))
+
 file.endConsoleSave()
 
 prt.printing("hello this should print letter by letter", delay=0.05, style="letter", new_line=True, rev=False)
+
 prt.printing("hello this should print word by word but in reverse", delay=0.05, style="word", new_line=True, rev=True)
+
 prt.flashprint("The entire text should flash", flashes=5, delay=0.2, stay=True)
+
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2)
+
 prt.animate1("This text is animated with #", symbol="#")
+
 prt.animate2("Prints letter by letter but masked with # first", symbol="#", delay=0.05)
+
 prt.text_box("M O N E Y  M A K E R", symbol="$", padding=True, wall=True)
+
 load.countdown(5)
+
 load.loading1(10)
+
 print()
+
 load.loading2(5)
+
 print()
+
 load.loading3(5)
 
 # License
 This project is given free for use and download under the MIT license.
 
 # Project Status
 Still undergoing enhancements.
```

