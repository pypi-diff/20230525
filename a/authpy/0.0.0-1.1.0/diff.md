# Comparing `tmp/authpy-0.0.0.tar.gz` & `tmp/authpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authpy-0.0.0.tar", last modified: Wed May 24 06:19:30 2023, max compression
+gzip compressed data, was "authpy-1.1.0.tar", last modified: Thu May 25 02:25:15 2023, max compression
```

## Comparing `authpy-0.0.0.tar` & `authpy-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 06:19:30.728050 authpy-0.0.0/
--rw-rw-rw-   0        0        0      561 2023-05-24 06:19:30.728050 authpy-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 06:19:30.711997 authpy-0.0.0/authpy/
--rw-rw-rw-   0        0        0       35 2023-05-24 06:51:10.000000 authpy-0.0.0/authpy/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-05-24 06:51:09.000000 authpy-0.0.0/authpy/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-24 06:19:30.726071 authpy-0.0.0/authpy.egg-info/
--rw-rw-rw-   0        0        0      561 2023-05-24 06:19:30.000000 authpy-0.0.0/authpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-24 06:19:30.000000 authpy-0.0.0/authpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 06:19:30.000000 authpy-0.0.0/authpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 06:19:30.000000 authpy-0.0.0/authpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 06:19:30.729035 authpy-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      638 2023-05-24 06:19:18.000000 authpy-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:25:15.724774 authpy-1.1.0/
+-rw-rw-rw-   0        0        0     1176 2023-05-25 02:15:23.000000 authpy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1961 2023-05-25 02:25:15.723692 authpy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1334 2023-05-25 02:21:36.000000 authpy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 02:25:15.697646 authpy-1.1.0/authpy/
+-rw-rw-rw-   0        0        0       70 2023-05-25 02:11:31.000000 authpy-1.1.0/authpy/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-05-25 01:16:49.000000 authpy-1.1.0/authpy/auth.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:25:15.720836 authpy-1.1.0/authpy.egg-info/
+-rw-rw-rw-   0        0        0     1961 2023-05-25 02:25:15.000000 authpy-1.1.0/authpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-05-25 02:25:15.000000 authpy-1.1.0/authpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 02:25:15.000000 authpy-1.1.0/authpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 02:25:15.000000 authpy-1.1.0/authpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 02:25:15.724774 authpy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-05-25 02:24:38.000000 authpy-1.1.0/setup.py
```

### Comparing `authpy-0.0.0/authpy/auth.py` & `authpy-1.1.0/authpy/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,57 @@
 import csv
+import bcrypt
+import os
+
+def create_db():
+    with open("db.csv", "w", newline='') as database:
+        writer = csv.writer(database)
+        writer.writerow(["username", "password"])
 
 def signup(username, password):
     if len(username) == 0:
         raise ValueError("Please enter a valid username with characters")
     elif len(username) > 30:
         raise ValueError("The username has to be less than 30 characters")
     elif username == "username" or username == "admin":
         raise ValueError("Don't use a forbidden username")
 
-    with open("database.json", "r") as database:
+    if not os.path.isfile("db.csv"):
+        create_db()
+
+    with open("db.csv", "r") as database:
         reader = csv.reader(database)
         for u, _ in reader:
             if username == u:
                 raise ValueError("This username has already been taken")
 
     if len(password) < 4:
         raise ValueError("Please make sure your password is more than 4 characters")
     if password == "Password" or password == "password":
         raise ValueError("Choose a stronger password")
 
-    with open("database.json", "a", newline="") as database:
-        writer = csv.writer(database)
-        writer.writerow([username, password])
+    # Hash the password using bcrypt
+    salt = bcrypt.gensalt()
+    hashed_password = bcrypt.hashpw(password.encode(), salt)
 
-    return "Your username and password have been successfully saved"
+    # Store the username and hashed password in the database
+    with open("db.csv", "a", newline='') as database:
+        writer = csv.writer(database)
+        writer.writerow([username, hashed_password.decode()])
 
 
 def login(username, password):
-    with open("database.json", "r") as database:
+    if not os.path.isfile("db.csv"):
+        create_db()
+
+    with open("db.csv", "r") as database:
         reader = csv.reader(database)
         for u, p in reader:
             if username == u:
-                if password == p:
+                if bcrypt.checkpw(password.encode(), p.encode()):
                     return "Login successful"
                 else:
                     return "The password is incorrect"
 
     return "Sorry, username or password doesn't exist"
 
 # Example usage when the library is imported
@@ -44,8 +60,8 @@
     password_input = input("Enter your password: ")
     signup_result = signup(username_input, password_input)
     print(signup_result)
 
     username_input = input("What is your username: ")
     password_input = input("Enter your password: ")
     login_result = login(username_input, password_input)
-    print(login_result)
+    print(login_result)
```

