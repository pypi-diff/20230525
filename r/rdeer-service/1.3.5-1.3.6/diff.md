# Comparing `tmp/rdeer-service-1.3.5.tar.gz` & `tmp/rdeer-service-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdeer-service-1.3.5.tar", last modified: Tue May 17 09:17:47 2022, max compression
+gzip compressed data, was "rdeer-service-1.3.6.tar", last modified: Thu May 25 15:09:07 2023, max compression
```

## Comparing `rdeer-service-1.3.5.tar` & `rdeer-service-1.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2022-05-17 09:17:47.838941 rdeer-service-1.3.5/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      201 2022-01-26 13:34:56.000000 rdeer-service-1.3.5/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     3970 2022-05-17 09:17:47.836510 rdeer-service-1.3.5/PKG-INFO
--rw-r--r--   0 benoit    (1017) bio2m     (1010)     2615 2022-01-26 13:34:56.000000 rdeer-service-1.3.5/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2022-05-17 09:17:47.768171 rdeer-service-1.3.5/rdeer/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      116 2022-01-26 13:34:56.000000 rdeer-service-1.3.5/rdeer/__init__.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10994 2022-05-16 18:50:05.000000 rdeer-service-1.3.5/rdeer/client.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      802 2022-05-16 06:15:32.000000 rdeer-service-1.3.5/rdeer/common.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      189 2022-05-17 09:16:13.000000 rdeer-service-1.3.5/rdeer/info.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    19637 2022-05-17 09:12:56.000000 rdeer-service-1.3.5/rdeer/server.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2022-05-17 09:17:47.823601 rdeer-service-1.3.5/rdeer_service.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     3970 2022-05-17 09:17:47.000000 rdeer-service-1.3.5/rdeer_service.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      298 2022-05-17 09:17:47.000000 rdeer-service-1.3.5/rdeer_service.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2022-05-17 09:17:47.000000 rdeer-service-1.3.5/rdeer_service.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       85 2022-05-17 09:17:47.000000 rdeer-service-1.3.5/rdeer_service.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        6 2022-05-17 09:17:47.000000 rdeer-service-1.3.5/rdeer_service.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2022-05-17 09:17:47.841047 rdeer-service-1.3.5/setup.cfg
--rw-r--r--   0 benoit    (1017) bio2m     (1010)     1064 2022-01-26 13:34:56.000000 rdeer-service-1.3.5/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-25 15:09:07.763462 rdeer-service-1.3.6/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      201 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     3970 2023-05-25 15:09:07.759097 rdeer-service-1.3.6/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     2615 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-25 15:09:07.668607 rdeer-service-1.3.6/rdeer/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      116 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/rdeer/__init__.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    10895 2023-05-25 14:58:05.000000 rdeer-service-1.3.6/rdeer/client.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      802 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/rdeer/common.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      189 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/rdeer/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    20226 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/rdeer/server.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-25 15:09:07.743079 rdeer-service-1.3.6/rdeer_service.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     3970 2023-05-25 15:09:07.000000 rdeer-service-1.3.6/rdeer_service.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      298 2023-05-25 15:09:07.000000 rdeer-service-1.3.6/rdeer_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-05-25 15:09:07.000000 rdeer-service-1.3.6/rdeer_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      111 2023-05-25 15:09:07.000000 rdeer-service-1.3.6/rdeer_service.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        6 2023-05-25 15:09:07.000000 rdeer-service-1.3.6/rdeer_service.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-05-25 15:09:07.765974 rdeer-service-1.3.6/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1085 2023-05-25 14:41:28.000000 rdeer-service-1.3.6/setup.py
```

### Comparing `rdeer-service-1.3.5/PKG-INFO` & `rdeer-service-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdeer-service
-Version: 1.3.5
+Version: 1.3.6
 Summary: Client-server to handle Reindeer in query mode.
 Home-page: https://github.com/Bio2M/rdeer-service
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Description: # RDEER-SERVICE
```

### Comparing `rdeer-service-1.3.5/README.md` & `rdeer-service-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `rdeer-service-1.3.5/rdeer/client.py` & `rdeer-service-1.3.6/rdeer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 """
 TODO
 In Transipedia, change type 'counts' by 'query' and 'indexes' by 'list'
 and in this file 'to_send({'type'='counts', .....})' by 'to_send({'type'=type, .....})'
 """
 
-""" Module doc """
 
 import sys
 import os
 import argparse
 import socket
 import pickle
 
-# sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 import info
 import common as stream
 
 
 
 def main():
     """ Function doc """
@@ -200,15 +198,15 @@
 
 def usage():
     """
     Help function with argument parser.
     https://docs.python.org/3/howto/argparse.html?highlight=argparse
     """
     ### build parser
-    parser = argparse.ArgumentParser(prog=info.APPNAME)
+    parser = argparse.ArgumentParser()
     global_parser = argparse.ArgumentParser(add_help=False)
     index_parser = argparse.ArgumentParser(add_help=False)
     subparsers = parser.add_subparsers()
     subparsers.dest = 'type'
     subparsers.required = True
     ### Hidden argument to send login name in requests
     parser.add_argument('--user',
```

### Comparing `rdeer-service-1.3.5/rdeer/common.py` & `rdeer-service-1.3.6/rdeer/common.py`

 * *Files identical despite different names*

### Comparing `rdeer-service-1.3.5/rdeer/server.py` & `rdeer-service-1.3.6/rdeer/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 - An instance of Rdeer is created
     - launch a thread scanning the root directory of indexes
     - received clients requests
 
 
 Starting a Reindeer socket
 - When index starting:
-    - lance un Reindeer query sur un port réseau distinct avec subprocess.Popen()
-    - ajoute dans un dictionnaire dict['nom de l'index'] = {'status': 'loading', 'port': 'n°'}
-    - qui scanne toute les secondes si le port réseau est ouvert
-    - lorsque le port réseau est ouvert
-        - se connecter en client sur l'index Reindeer
-            - vérifier si l'index fonctionne
-            - modifier l'entrée du dictionnaire dict['nom de l'index'] = {'status': 'running', 'port': 'n°'}
-            - rester en attente
+    - launch Reindeer query in waiting mode on specified port (default: 12800) using subprocess.Popen()
+    - add in a dictionnary dict['nom de l'index'] = {'status': 'loading', 'port': 'n°'}
+    - scan each second if port is open
+    - when port is open
+        - connect as client on the Reindeer index
+            - check running index
+            - update dictionnary entry dict['index name'] = {'status': 'running', 'port': 'n°'}
+            - wait to query from rdeer-client
 '''
 
 import os
 import sys
 import pathlib
 import socket
 import argparse
@@ -342,22 +342,19 @@
 
         ### check if Reindeer process running, otherwise, probably it is crashed
         # ~ cmd = f'Reindeer-socket --query -l {os.path.join(self.args.index_dir, index)} -q *{port}'
         # ~ proc = subprocess.run(f"ps -ef | grep '{cmd}'", shell=True, stdout=subprocess.PIPE)
         # ~ if proc.returncode:
             # ~ print(f'error: index {index} crashed during loading')
 
-
         ### try to connect
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        # ~ print(f'TRY TO CONNECT TO {index} on port {port}')
         try:
             s.settimeout(1)
             s.connect(('', int(port)))    # Connect to running Reindeer
-            # ~ s.settimeout(None)
             self.indexes[index]['status'] = 'running'
             self.sockets[index] = s
             ### evacuate WELCOME and INDEX message
             welcome = s.recv(1024)
             # ~ print(f"FIRST MESG: {welcome}")
             index = s.recv(1024)
             # ~ print(f"SECOND MESG: {index}")
@@ -411,25 +408,36 @@
                     for j,count in enumerate(counts):           # j --> sample/count
                         if count != '*':
                             counts[j] = [c.split(':')[1] for c in count.split(",")]
                             ### average of untigs counts - but stars  ('*') must be removed
                             counts[j] = sum([int(c) for c in counts[j] if c != '*']) // len(counts[j])
                             ### NORMALIZE if kmers counts are present in file of samples (fos.txt)
                             if normalize and kmers_found:
+                                if len(counts) != len(kmers_found):
+                                    msg = f"Error: check line counts in fos.txt."
+                                    response['status'] = 'error'
+                                    print(f"{timestamp()} Error: {msg}", file=sys.stdout)
+                                    return msg
                                 try:
                                     counts[j] = round(NORM * counts[j] / int(kmers_found[j]),2)
                                 except ValueError:
                                     self.indexes[index]['status'] = 'error'
                                     response['status'] = 'error'
                                     msg = f"File {FOS!r} malformed (index: {index})."
                                     print(f"{timestamp()} Error: {msg}", file=sys.stdout)
                                     return msg
+                                except IndexError:
+                                    response['status'] = 'error'
+                                    msg = f"unable to normalize (error: IndexError)."
+                                    print(f"{timestamp()} Error: {msg}", file=sys.stdout)
+                                    return msg
                             elif normalize and not kmers_found:
                                 response['status'] = 'error'
-                                return(f"unable to normalize counts on {index}, it could be that {FOS} does not contain counts.")
+                                return(f"unable to normalize counts on {index}, it could be that "
+                                       f"{FOS} does not contain counts.")
                             counts[j] = str(counts[j])
                         else:
                             counts[j] = '0'
                     data.append(seq_name + '\t' + '\t'.join(counts))
             data = '\n'.join(data) + '\n'
 
         ### join header and counts
```

### Comparing `rdeer-service-1.3.5/rdeer_service.egg-info/PKG-INFO` & `rdeer-service-1.3.6/rdeer_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdeer-service
-Version: 1.3.5
+Version: 1.3.6
 Summary: Client-server to handle Reindeer in query mode.
 Home-page: https://github.com/Bio2M/rdeer-service
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Description: # RDEER-SERVICE
```

### Comparing `rdeer-service-1.3.5/setup.py` & `rdeer-service-1.3.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
-# -*- coding:utf8 -*-
+
 
 import setuptools
 from rdeer import info
 
+
 setuptools.setup(
     name = 'rdeer-service',
     version = info.VERSION,
     author = info.AUTHOR,
     author_email = info.AUTHOR_EMAIL,
     description = info.SHORTDESC,
     long_description = open('README.md').read(),
@@ -21,14 +22,15 @@
         'Programming Language :: Python',
         'Natural Language :: English',
         'Intended Audience :: Science/Research',
     ],
     entry_points = {
         'console_scripts': [
             'rdeer-client = rdeer.client:main',
+            'rdeer = rdeer.client:main',
             'rdeer-server = rdeer.server:main',
         ],
     },
     include_package_data = True,
     # install_requires=['PyYAML'],
     python_requires = ">=3.6",
     licence = "GPLv3"
```

