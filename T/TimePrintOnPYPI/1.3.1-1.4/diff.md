# Comparing `tmp/TimePrintOnPYPI-1.3.1.tar.gz` & `tmp/TimePrintOnPYPI-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.3.1.tar", last modified: Thu May 25 21:01:32 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.4.tar", last modified: Thu May 25 21:04:59 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.3.1.tar` & `TimePrintOnPYPI-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 21:01:32.841004 TimePrintOnPYPI-1.3.1/
--rw-rw-rw-   0        0        0     1201 2023-05-25 21:01:32.839998 TimePrintOnPYPI-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-05-25 21:00:58.000000 TimePrintOnPYPI-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 21:01:32.820229 TimePrintOnPYPI-1.3.1/TimePrint/
--rw-rw-rw-   0        0        0     1687 2023-05-25 21:01:16.000000 TimePrintOnPYPI-1.3.1/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:01:32.838996 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     1201 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 21:01:32.841997 TimePrintOnPYPI-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-05-25 21:01:12.000000 TimePrintOnPYPI-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:04:59.578278 TimePrintOnPYPI-1.4/
+-rw-rw-rw-   0        0        0     1262 2023-05-25 21:04:59.577278 TimePrintOnPYPI-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-05-25 21:04:36.000000 TimePrintOnPYPI-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 21:04:59.560213 TimePrintOnPYPI-1.4/TimePrint/
+-rw-rw-rw-   0        0        0     1685 2023-05-25 21:04:41.000000 TimePrintOnPYPI-1.4/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:04:59.574269 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     1262 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 21:04:59.578278 TimePrintOnPYPI-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-05-25 21:04:45.000000 TimePrintOnPYPI-1.4/setup.py
```

### Comparing `TimePrintOnPYPI-1.3.1/PKG-INFO` & `TimePrintOnPYPI-1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.3.1
+Version: 1.4
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# TIME PRINT README FILE
-This is a python package to use write effect and more in your texts !
+# TIME PRINT V1.4
+This is a python package to use write effect and more in your texts !<br>
 
 ## TP(seconds,"text")
-You want to write "your_text" in 5 seconds? just use;
-TP(5,"your_text") !
-formats: seconds: int,"text":str
+You want to write "your_text" in 5 seconds? just use;<br>
+TP(5,"your_text") !<br>
+formats: seconds: int,"text":str<br>
 ## P("text")
-You don't want to wait until it writes bla bla seconds ?
-it just goes write effect and its fast (very fast)
+You don't want to wait until it writes bla bla seconds ?<br>
+it just goes write effect and its fast (very fast)<br>
 
-format: "text":str
+format: "text":str<br>
 ## timetag(format:str)
-Its not very cool thing but i added
-don't have to talk just look ex.
-format usages;
-"%H:%M" Returns --> 12:56 = (Hours:Minutes)
-"%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
-"%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
+Its not very cool thing but i added,Don't have to much talk just look ex.<br>
 
-It uses strftime package.
+Example format usages;<br>
+"%H:%M" Returns --> 12:56 = (Hours:Minutes)<br>
+"%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)<br>
+"%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)<br>
+
+It uses strftime package.<br>
 ## info()
-just info about package.
+just info about package.<br>
```

### Comparing `TimePrintOnPYPI-1.3.1/README.md` & `TimePrintOnPYPI-1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# TIME PRINT README FILE
-This is a python package to use write effect and more in your texts !
+# TIME PRINT V1.4
+This is a python package to use write effect and more in your texts !<br>
 
 ## TP(seconds,"text")
-You want to write "your_text" in 5 seconds? just use;
-TP(5,"your_text") !
-formats: seconds: int,"text":str
+You want to write "your_text" in 5 seconds? just use;<br>
+TP(5,"your_text") !<br>
+formats: seconds: int,"text":str<br>
 ## P("text")
-You don't want to wait until it writes bla bla seconds ?
-it just goes write effect and its fast (very fast)
+You don't want to wait until it writes bla bla seconds ?<br>
+it just goes write effect and its fast (very fast)<br>
 
-format: "text":str
+format: "text":str<br>
 ## timetag(format:str)
-Its not very cool thing but i added
-don't have to talk just look ex.
-format usages;
-"%H:%M" Returns --> 12:56 = (Hours:Minutes)
-"%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
-"%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
+Its not very cool thing but i added,Don't have to much talk just look ex.<br>
 
-It uses strftime package.
+Example format usages;<br>
+"%H:%M" Returns --> 12:56 = (Hours:Minutes)<br>
+"%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)<br>
+"%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)<br>
+
+It uses strftime package.<br>
 ## info()
-just info about package.
+just info about package.<br>
```

### Comparing `TimePrintOnPYPI-1.3.1/TimePrint/__init__.py` & `TimePrintOnPYPI-1.4/TimePrint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.3.1")
+    print("Version: 1.4")
 def timetag(format: str):
     """
     Example Usages;
 
     "%H:%M" Returns --> 12:56 = (Hours:Minutes)
     "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
     "%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
```

### Comparing `TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/PKG-INFO` & `TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.3.1
+Version: 1.4
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# TIME PRINT README FILE
-This is a python package to use write effect and more in your texts !
+# TIME PRINT V1.4
+This is a python package to use write effect and more in your texts !<br>
 
 ## TP(seconds,"text")
-You want to write "your_text" in 5 seconds? just use;
-TP(5,"your_text") !
-formats: seconds: int,"text":str
+You want to write "your_text" in 5 seconds? just use;<br>
+TP(5,"your_text") !<br>
+formats: seconds: int,"text":str<br>
 ## P("text")
-You don't want to wait until it writes bla bla seconds ?
-it just goes write effect and its fast (very fast)
+You don't want to wait until it writes bla bla seconds ?<br>
+it just goes write effect and its fast (very fast)<br>
 
-format: "text":str
+format: "text":str<br>
 ## timetag(format:str)
-Its not very cool thing but i added
-don't have to talk just look ex.
-format usages;
-"%H:%M" Returns --> 12:56 = (Hours:Minutes)
-"%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
-"%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
+Its not very cool thing but i added,Don't have to much talk just look ex.<br>
 
-It uses strftime package.
+Example format usages;<br>
+"%H:%M" Returns --> 12:56 = (Hours:Minutes)<br>
+"%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)<br>
+"%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)<br>
+
+It uses strftime package.<br>
 ## info()
-just info about package.
+just info about package.<br>
```

### Comparing `TimePrintOnPYPI-1.3.1/setup.py` & `TimePrintOnPYPI-1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='TimePrintOnPYPI',
-    version='1.3.1',
+    version='1.4',
     description='A package for printing text with time delay between characters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
```

