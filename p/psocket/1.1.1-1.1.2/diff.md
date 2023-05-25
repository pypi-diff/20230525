# Comparing `tmp/psocket-1.1.1.tar.gz` & `tmp/psocket-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psocket-1.1.1.tar", last modified: Wed Aug  3 21:38:20 2022, max compression
+gzip compressed data, was "psocket-1.1.2.tar", last modified: Thu May 25 17:28:55 2023, max compression
```

## Comparing `psocket-1.1.1.tar` & `psocket-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-08-03 21:38:20.420682 psocket-1.1.1/
--rw-rw-rw-   0        0        0     1095 2022-08-03 20:54:54.000000 psocket-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3868 2022-08-03 21:38:20.388871 psocket-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3044 2022-08-03 21:36:34.000000 psocket-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-03 21:38:20.372941 psocket-1.1.1/psocket/
--rw-rw-rw-   0        0        0     5546 2022-08-03 21:35:11.000000 psocket-1.1.1/psocket/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-03 21:38:20.388871 psocket-1.1.1/psocket.egg-info/
--rw-rw-rw-   0        0        0     3868 2022-08-03 21:38:20.000000 psocket-1.1.1/psocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2022-08-03 21:38:20.000000 psocket-1.1.1/psocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-03 21:38:20.000000 psocket-1.1.1/psocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-08-03 21:38:20.000000 psocket-1.1.1/psocket.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-03 21:38:20.000000 psocket-1.1.1/psocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-03 21:38:20.420682 psocket-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1229 2022-08-03 21:31:11.000000 psocket-1.1.1/setup.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-25 17:28:55.520525 psocket-1.1.2/
+-rw-r--r--   0 c-pher     (502) staff       (20)     1074 2023-05-25 16:06:10.000000 psocket-1.1.2/LICENSE
+-rw-r--r--   0 c-pher     (502) staff       (20)     3800 2023-05-25 17:28:55.520400 psocket-1.1.2/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)     2997 2023-05-25 17:28:50.000000 psocket-1.1.2/README.md
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-25 17:28:55.519646 psocket-1.1.2/psocket/
+-rw-r--r--   0 c-pher     (502) staff       (20)     6222 2023-05-25 17:28:50.000000 psocket-1.1.2/psocket/__init__.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-25 17:28:55.520231 psocket-1.1.2/psocket.egg-info/
+-rw-r--r--   0 c-pher     (502) staff       (20)     3800 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)      200 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/SOURCES.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        1 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/dependency_links.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       15 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/requires.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        8 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/top_level.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       38 2023-05-25 17:28:55.520566 psocket-1.1.2/setup.cfg
+-rw-r--r--   0 c-pher     (502) staff       (20)     1194 2023-05-25 17:28:50.000000 psocket-1.1.2/setup.py
```

### Comparing `psocket-1.1.1/PKG-INFO` & `psocket-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,142 +1,146 @@
-Metadata-Version: 2.1
-Name: psocket
-Version: 1.1.1
-Summary: The cross-platform tool to work with remote connection using sockets
-Home-page: https://github.com/c-pher/PSocket.git
-Author: Andrey Komissarov
-Author-email: a.komisssarov@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI version](https://badge.fury.io/py/psocket.svg)](https://badge.fury.io/py/psocket)
-[![Build Status](https://travis-ci.org/c-pher/PSocket.svg?branch=master)](https://travis-ci.org/c-pher/PSocket)
-[![Coverage Status](https://coveralls.io/repos/github/c-pher/PSocket/badge.svg?branch=master)](https://coveralls.io/github/c-pher/PSocket?branch=master)
-
-
-# PSocket
-The cross-platform simple tool to work with remote server through sockets. 
-It can establish socket connection to a remote host:port, send commands and receive response.
-No need to send byte-string. Use usual strings to send command.
-
-## Installation
-For most users, the recommended method to install is via pip:
-```cmd
-pip install psocket
-```
-
-or from source:
-
-```cmd
-python setup.py install
-```
-
-## Import
-```python
-from psocket import SocketClient
-```
----
-## Usage
-```python
-from psocket import SocketClient
-
-client = SocketClient(host='172.16.0.48', port=3261)
-print(client)
-```
-```python
-from psocket import SocketClient
-
-client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
-print(client.send_command('<commands>'))
-```
-
----
-
-## Changelog
-
-##### 1.1.1 (04.08.2022)
-
-- Detect command is completed by \n\n
-
-##### 1.1.0 (23.07.2022)
-
-- log format changed
-
-##### 1.0.9 (4.06.2022)
-
-- response now split lines (instead of .split('\n'))
-- logger now is static `SocketClient`
-- "greeting" class attr added
-- minor changes in logging format
-- socket timeout log level changed from debug to warning
-
-##### 1.0.8 (22.04.2022)
-
-- Set blocking after command send with it
-
-##### 1.0.7 (18.04.2022)
-
-- ._socket_response() renamed to ._receive_all() and changed to read huge amount of data from socket
-- buffer size changed to 4k (instead of 64k)
-- .send_command() extended with "timeout=None" param
-
-##### 1.0.6 (17.04.2022)
-
-- refactored to manage logger state
-
-##### 1.0.5 (6.04.2022)
-
-- logger moved inside class as attr in order to get access to it from outside
-- unknown attr access handling added
--
-
-##### 1.0.4 (14.06.2021)
-
-Added host address logging
-
-##### 1.0.3 (12.03.2021)
-
-- Added ability to disable logs
-- "timeout connection" added as parameter with None default value
-
-##### 1.0.2 (15.01.2020)
-
-Added "initialize" param to the constructor
-
-##### 1.0.1 (15.01.2020)
-
-- "is_host_available()" renamed to "is_socket_available()" and updated
-- used external logger from "plogger" package
-
-##### 1.0.0a4 (15.01.2020)
-- added init docstring
-- init notation changed:
-  - host is string
-  - port is integer
-
-##### 1.0.0a3 (14.01.2020)
-- removed timeout from socket connection
-- greeting and socket_response now are private methods
-
-##### 1.0.0a2 (13.01.2020)
-Reverted "client". Now it is an attribute again to keep session alive 
-
-##### 1.0.0a1 (13.01.2020)
-- Now connection creates with client property
-- New methods added:
-    - is_host_available() 
-    - get_sock_name()
-    - get_peer_name()
-
-##### 1.0.0a0 (13.01.2020)
-- initial commit
+Metadata-Version: 2.1
+Name: psocket
+Version: 1.1.2
+Summary: The cross-platform tool to work with remote connection using sockets
+Home-page: https://github.com/c-pher/PSocket.git
+Author: Andrey Komissarov
+Author-email: a.komisssarov@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/psocket.svg)](https://badge.fury.io/py/psocket)
+[![Build Status](https://travis-ci.org/c-pher/PSocket.svg?branch=master)](https://travis-ci.org/c-pher/PSocket)
+[![Coverage Status](https://coveralls.io/repos/github/c-pher/PSocket/badge.svg?branch=master)](https://coveralls.io/github/c-pher/PSocket?branch=master)
+
+
+# PSocket
+The cross-platform simple tool to work with remote server through sockets. 
+It can establish socket connection to a remote host:port, send commands and receive response.
+No need to send byte-string. Use usual strings to send command.
+
+## Installation
+For most users, the recommended method to install is via pip:
+```cmd
+pip install psocket
+```
+
+or from source:
+
+```cmd
+python setup.py install
+```
+
+## Import
+```python
+from psocket import SocketClient
+```
+---
+## Usage
+```python
+from psocket import SocketClient
+
+client = SocketClient(host='172.16.0.48', port=3261)
+print(client)
+```
+```python
+from psocket import SocketClient
+
+client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
+print(client.send_command('<commands>'))
+```
+
+---
+
+## Changelog
+
+##### 1.1.2 (25.05.2023)
+- buffer size increased to 8k
+- debug log added
+
+##### 1.1.1 (04.08.2022)
+
+- Detect command is completed by \n\n
+
+##### 1.1.0 (23.07.2022)
+
+- log format changed
+
+##### 1.0.9 (4.06.2022)
+
+- response now split lines (instead of .split('\n'))
+- logger now is static `SocketClient`
+- "greeting" class attr added
+- minor changes in logging format
+- socket timeout log level changed from debug to warning
+
+##### 1.0.8 (22.04.2022)
+
+- Set blocking after command send with it
+
+##### 1.0.7 (18.04.2022)
+
+- ._socket_response() renamed to ._receive_all() and changed to read huge amount of data from socket
+- buffer size changed to 4k (instead of 64k)
+- .send_command() extended with "timeout=None" param
+
+##### 1.0.6 (17.04.2022)
+
+- refactored to manage logger state
+
+##### 1.0.5 (6.04.2022)
+
+- logger moved inside class as attr in order to get access to it from outside
+- unknown attr access handling added
+-
+
+##### 1.0.4 (14.06.2021)
+
+Added host address logging
+
+##### 1.0.3 (12.03.2021)
+
+- Added ability to disable logs
+- "timeout connection" added as parameter with None default value
+
+##### 1.0.2 (15.01.2020)
+
+Added "initialize" param to the constructor
+
+##### 1.0.1 (15.01.2020)
+
+- "is_host_available()" renamed to "is_socket_available()" and updated
+- used external logger from "plogger" package
+
+##### 1.0.0a4 (15.01.2020)
+- added init docstring
+- init notation changed:
+  - host is string
+  - port is integer
+
+##### 1.0.0a3 (14.01.2020)
+- removed timeout from socket connection
+- greeting and socket_response now are private methods
+
+##### 1.0.0a2 (13.01.2020)
+Reverted "client". Now it is an attribute again to keep session alive 
+
+##### 1.0.0a1 (13.01.2020)
+- Now connection creates with client property
+- New methods added:
+    - is_host_available() 
+    - get_sock_name()
+    - get_peer_name()
+
+##### 1.0.0a0 (13.01.2020)
+- initial commit
```

### Comparing `psocket-1.1.1/README.md` & `psocket-1.1.2/psocket.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,146 @@
-[![PyPI version](https://badge.fury.io/py/psocket.svg)](https://badge.fury.io/py/psocket)
-[![Build Status](https://travis-ci.org/c-pher/PSocket.svg?branch=master)](https://travis-ci.org/c-pher/PSocket)
-[![Coverage Status](https://coveralls.io/repos/github/c-pher/PSocket/badge.svg?branch=master)](https://coveralls.io/github/c-pher/PSocket?branch=master)
-
-
-# PSocket
-The cross-platform simple tool to work with remote server through sockets. 
-It can establish socket connection to a remote host:port, send commands and receive response.
-No need to send byte-string. Use usual strings to send command.
-
-## Installation
-For most users, the recommended method to install is via pip:
-```cmd
-pip install psocket
-```
-
-or from source:
-
-```cmd
-python setup.py install
-```
-
-## Import
-```python
-from psocket import SocketClient
-```
----
-## Usage
-```python
-from psocket import SocketClient
-
-client = SocketClient(host='172.16.0.48', port=3261)
-print(client)
-```
-```python
-from psocket import SocketClient
-
-client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
-print(client.send_command('<commands>'))
-```
-
----
-
-## Changelog
-
-##### 1.1.1 (04.08.2022)
-
-- Detect command is completed by \n\n
-
-##### 1.1.0 (23.07.2022)
-
-- log format changed
-
-##### 1.0.9 (4.06.2022)
-
-- response now split lines (instead of .split('\n'))
-- logger now is static `SocketClient`
-- "greeting" class attr added
-- minor changes in logging format
-- socket timeout log level changed from debug to warning
-
-##### 1.0.8 (22.04.2022)
-
-- Set blocking after command send with it
-
-##### 1.0.7 (18.04.2022)
-
-- ._socket_response() renamed to ._receive_all() and changed to read huge amount of data from socket
-- buffer size changed to 4k (instead of 64k)
-- .send_command() extended with "timeout=None" param
-
-##### 1.0.6 (17.04.2022)
-
-- refactored to manage logger state
-
-##### 1.0.5 (6.04.2022)
-
-- logger moved inside class as attr in order to get access to it from outside
-- unknown attr access handling added
--
-
-##### 1.0.4 (14.06.2021)
-
-Added host address logging
-
-##### 1.0.3 (12.03.2021)
-
-- Added ability to disable logs
-- "timeout connection" added as parameter with None default value
-
-##### 1.0.2 (15.01.2020)
-
-Added "initialize" param to the constructor
-
-##### 1.0.1 (15.01.2020)
-
-- "is_host_available()" renamed to "is_socket_available()" and updated
-- used external logger from "plogger" package
-
-##### 1.0.0a4 (15.01.2020)
-- added init docstring
-- init notation changed:
-  - host is string
-  - port is integer
-
-##### 1.0.0a3 (14.01.2020)
-- removed timeout from socket connection
-- greeting and socket_response now are private methods
-
-##### 1.0.0a2 (13.01.2020)
-Reverted "client". Now it is an attribute again to keep session alive 
-
-##### 1.0.0a1 (13.01.2020)
-- Now connection creates with client property
-- New methods added:
-    - is_host_available() 
-    - get_sock_name()
-    - get_peer_name()
-
-##### 1.0.0a0 (13.01.2020)
-- initial commit
+Metadata-Version: 2.1
+Name: psocket
+Version: 1.1.2
+Summary: The cross-platform tool to work with remote connection using sockets
+Home-page: https://github.com/c-pher/PSocket.git
+Author: Andrey Komissarov
+Author-email: a.komisssarov@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/psocket.svg)](https://badge.fury.io/py/psocket)
+[![Build Status](https://travis-ci.org/c-pher/PSocket.svg?branch=master)](https://travis-ci.org/c-pher/PSocket)
+[![Coverage Status](https://coveralls.io/repos/github/c-pher/PSocket/badge.svg?branch=master)](https://coveralls.io/github/c-pher/PSocket?branch=master)
+
+
+# PSocket
+The cross-platform simple tool to work with remote server through sockets. 
+It can establish socket connection to a remote host:port, send commands and receive response.
+No need to send byte-string. Use usual strings to send command.
+
+## Installation
+For most users, the recommended method to install is via pip:
+```cmd
+pip install psocket
+```
+
+or from source:
+
+```cmd
+python setup.py install
+```
+
+## Import
+```python
+from psocket import SocketClient
+```
+---
+## Usage
+```python
+from psocket import SocketClient
+
+client = SocketClient(host='172.16.0.48', port=3261)
+print(client)
+```
+```python
+from psocket import SocketClient
+
+client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
+print(client.send_command('<commands>'))
+```
+
+---
+
+## Changelog
+
+##### 1.1.2 (25.05.2023)
+- buffer size increased to 8k
+- debug log added
+
+##### 1.1.1 (04.08.2022)
+
+- Detect command is completed by \n\n
+
+##### 1.1.0 (23.07.2022)
+
+- log format changed
+
+##### 1.0.9 (4.06.2022)
+
+- response now split lines (instead of .split('\n'))
+- logger now is static `SocketClient`
+- "greeting" class attr added
+- minor changes in logging format
+- socket timeout log level changed from debug to warning
+
+##### 1.0.8 (22.04.2022)
+
+- Set blocking after command send with it
+
+##### 1.0.7 (18.04.2022)
+
+- ._socket_response() renamed to ._receive_all() and changed to read huge amount of data from socket
+- buffer size changed to 4k (instead of 64k)
+- .send_command() extended with "timeout=None" param
+
+##### 1.0.6 (17.04.2022)
+
+- refactored to manage logger state
+
+##### 1.0.5 (6.04.2022)
+
+- logger moved inside class as attr in order to get access to it from outside
+- unknown attr access handling added
+-
+
+##### 1.0.4 (14.06.2021)
+
+Added host address logging
+
+##### 1.0.3 (12.03.2021)
+
+- Added ability to disable logs
+- "timeout connection" added as parameter with None default value
+
+##### 1.0.2 (15.01.2020)
+
+Added "initialize" param to the constructor
+
+##### 1.0.1 (15.01.2020)
+
+- "is_host_available()" renamed to "is_socket_available()" and updated
+- used external logger from "plogger" package
+
+##### 1.0.0a4 (15.01.2020)
+- added init docstring
+- init notation changed:
+  - host is string
+  - port is integer
+
+##### 1.0.0a3 (14.01.2020)
+- removed timeout from socket connection
+- greeting and socket_response now are private methods
+
+##### 1.0.0a2 (13.01.2020)
+Reverted "client". Now it is an attribute again to keep session alive 
+
+##### 1.0.0a1 (13.01.2020)
+- Now connection creates with client property
+- New methods added:
+    - is_host_available() 
+    - get_sock_name()
+    - get_peer_name()
+
+##### 1.0.0a0 (13.01.2020)
+- initial commit
```

### Comparing `psocket-1.1.1/setup.py` & `psocket-1.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from os import path
-
-from setuptools import setup
-
-INSTALL_REQUIRES = ['plogger>=1.0.6']
-
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='psocket',
-    version='1.1.1',
-    packages=['psocket'],
-    url='https://github.com/c-pher/PSocket.git',
-    license='MIT',
-    author='Andrey Komissarov',
-    author_email='a.komisssarov@gmail.com',
-    description='The cross-platform tool to work with remote connection using sockets',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Intended Audience :: System Administrators',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: System :: Systems Administration',
-        'Topic :: Software Development :: Libraries :: Python Modules'
-    ],
-    install_requires=INSTALL_REQUIRES,
-    python_requires='>=3.6',
-)
+from os import path
+
+from setuptools import setup
+
+INSTALL_REQUIRES = ['plogger>=1.0.6']
+
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='psocket',
+    version='1.1.2',
+    packages=['psocket'],
+    url='https://github.com/c-pher/PSocket.git',
+    license='MIT',
+    author='Andrey Komissarov',
+    author_email='a.komisssarov@gmail.com',
+    description='The cross-platform tool to work with remote connection using sockets',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Intended Audience :: System Administrators',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3.6',
+        'Topic :: System :: Systems Administration',
+        'Topic :: Software Development :: Libraries :: Python Modules'
+    ],
+    install_requires=INSTALL_REQUIRES,
+    python_requires='>=3.6',
+)
```

