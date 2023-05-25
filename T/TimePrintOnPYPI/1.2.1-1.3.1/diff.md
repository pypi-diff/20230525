# Comparing `tmp/TimePrintOnPYPI-1.2.1.tar.gz` & `tmp/TimePrintOnPYPI-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.2.1.tar", last modified: Thu May 25 20:49:22 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.3.1.tar", last modified: Thu May 25 21:01:32 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.2.1.tar` & `TimePrintOnPYPI-1.3.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 20:49:22.602265 TimePrintOnPYPI-1.2.1/
--rw-rw-rw-   0        0        0      445 2023-05-25 20:49:22.601254 TimePrintOnPYPI-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 20:49:22.586219 TimePrintOnPYPI-1.2.1/TimePrint/
--rw-rw-rw-   0        0        0     1444 2023-05-25 20:48:51.000000 TimePrintOnPYPI-1.2.1/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:49:22.599741 TimePrintOnPYPI-1.2.1/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0      445 2023-05-25 20:49:22.000000 TimePrintOnPYPI-1.2.1/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-05-25 20:49:22.000000 TimePrintOnPYPI-1.2.1/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 20:49:22.000000 TimePrintOnPYPI-1.2.1/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 20:49:22.000000 TimePrintOnPYPI-1.2.1/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 20:49:22.603269 TimePrintOnPYPI-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-05-25 20:49:11.000000 TimePrintOnPYPI-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:01:32.841004 TimePrintOnPYPI-1.3.1/
+-rw-rw-rw-   0        0        0     1201 2023-05-25 21:01:32.839998 TimePrintOnPYPI-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-05-25 21:00:58.000000 TimePrintOnPYPI-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 21:01:32.820229 TimePrintOnPYPI-1.3.1/TimePrint/
+-rw-rw-rw-   0        0        0     1687 2023-05-25 21:01:16.000000 TimePrintOnPYPI-1.3.1/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:01:32.838996 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     1201 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 21:01:32.000000 TimePrintOnPYPI-1.3.1/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 21:01:32.841997 TimePrintOnPYPI-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      735 2023-05-25 21:01:12.000000 TimePrintOnPYPI-1.3.1/setup.py
```

### Comparing `TimePrintOnPYPI-1.2.1/TimePrint/__init__.py` & `TimePrintOnPYPI-1.3.1/TimePrint/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 import time
 import sys
-def TP(saniye, metin):
+def TP(saniye: int, metin: str):
+    """
+    Usage;
+    TimePrint.TP(seconds,"text")
+    Example TimePrint.TP(1,"Hello") 
+    Writes Hello In 1 Seconds
+
+    """
     for karakter in metin:
         sys.stdout.write(karakter)
         sys.stdout.flush()
         time.sleep(int(saniye)/len(metin))
     print("")
-def P(metin):
+def P(metin:str):
+    """
+    Usage;
+    TimePrint.P("text")
+    Example TimePrint.P("Hello") writes
+    Hello in 0.001 seconds
+    You can use this for just
+    write effect.
+    
+    """
     for karakter in metin:
         sys.stdout.write(karakter)
         sys.stdout.flush()
         time.sleep(0.001)
     print("")    
 def info():
     print("      _______ _____ __  __ ______     _____  _____  _____ _   _ _______  ")
@@ -18,17 +34,18 @@
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.2.1")
+    print("Version: 1.3.1")
 def timetag(format: str):
     """
     Example Usages;
-    %H:%M Returns --> 12:56 = (Hours:Minutes)
-    %H:%M:%S Returns --> 12:56:24 = (Hours:Minutes:Seconds)
-    %d.%m.%y Returns --> 10.02.2023 = (Day.Month.Year)
-    %d.%m.%y %H:%M:%S Returns --> 10.02.2023 12:56:24 = (Day.Month.Year Hours:Minutes:Seconds)
+
+    "%H:%M" Returns --> 12:56 = (Hours:Minutes)
+    "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
+    "%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
+
     """
     return time.strftime(format, time.localtime())
```

