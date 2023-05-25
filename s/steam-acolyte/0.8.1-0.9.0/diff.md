# Comparing `tmp/steam-acolyte-0.8.1.tar.gz` & `tmp/steam-acolyte-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-acolyte-0.8.1.tar", last modified: Sun Oct  9 21:41:34 2022, max compression
+gzip compressed data, was "steam-acolyte-0.9.0.tar", last modified: Thu May 25 15:00:35 2023, max compression
```

## Comparing `steam-acolyte-0.8.1.tar` & `steam-acolyte-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 21:41:34.011769 steam-acolyte-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13212 2022-10-09 21:41:34.011769 steam-acolyte-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/UNLICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/acolyte.desktop
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-10-09 21:41:34.011769 steam-acolyte-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 21:41:34.011769 steam-acolyte-0.8.1/steam_acolyte/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/acolyte.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/async_.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/delete.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/funcwrap.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/logout.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/plus.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10252 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/steam.py
--rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/steam_linux.py
--rw-r--r--   0 runner    (1001) docker     (121)     6428 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/steam_win32.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/theme.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/user.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/window.css
--rw-r--r--   0 runner    (1001) docker     (121)    12862 2022-10-09 21:41:24.000000 steam-acolyte-0.8.1/steam_acolyte/window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 21:41:34.011769 steam-acolyte-0.8.1/steam_acolyte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13212 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-09 21:41:33.000000 steam-acolyte-0.8.1/steam_acolyte.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:00:35.955056 steam-acolyte-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-25 15:00:35.955056 steam-acolyte-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/UNLICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/acolyte.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 15:00:35.955056 steam-acolyte-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:00:35.951056 steam-acolyte-0.9.0/steam_acolyte/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/acolyte.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/funcwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/steam_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/steam_win32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/user.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/window.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-05-25 15:00:25.000000 steam-acolyte-0.9.0/steam_acolyte/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:00:35.955056 steam-acolyte-0.9.0/steam_acolyte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:00:35.000000 steam-acolyte-0.9.0/steam_acolyte.egg-info/zip-safe
```

### Comparing `steam-acolyte-0.8.1/PKG-INFO` & `steam-acolyte-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-acolyte
-Version: 0.8.1
+Version: 0.9.0
 Summary: Lightweight user account switcher/login keeper for steam
 Home-page: https://github.com/coldfix/steam-acolyte
 Author: Thomas Gläßle
 Author-email: thomas@coldfix.de
 License: Unlicense
 Description: Steam Acolyte
         =============
@@ -68,42 +68,44 @@
         
         Optionally, modify your steam launchers to execute ``steam-acolyte``.
         
         
         How it works
         ------------
         
-        *acolyte* works dead-simple by saving the login token for the last active
-        steam account upon program start. When the user clicks on a particular account
-        it simply restores the corresponding token and then starts steam. *acolyte*
-        only stores login tokes, but never any passwords! This has the following
-        implications:
+        *acolyte* does not inspect or store any password or login tokens at all. It
+        only tells steam which user to login when starting. Steam uses its own
+        mechanism to store login information. This has the following consequences:
         
         - the login token can be used to login without having to re-enter 2FA
-          (whereas for password-based logins you would need to redo 2FA)
-        - the login token can only be used for a single login
-        - after a successful login, steam will create a fresh token which acolyte can
-          save for the next cycle when steam exits or when acolyte is started the next
-          time
-        - it is no problem to start and exit steam several times without acolyte
-          running (as long as you always sign on with the same account), because
-          acolyte will always pick up the most recent login token when it starts
-        - the token expires if unused for a several weeks
+          (whereas for password-based login manager you would need to redo 2FA)
+        - you can mix using steam with or without acolyte
+        - active logins expire if unused for a several weeks
         - selecting "Change Account" from the steam menu or "Log Out User" in Big
           Picture mode UI invalidates the login and you will have to reenter your
           password for the logged out user
         
         
         .. |Screenshot| image:: https://raw.githubusercontent.com/coldfix/steam-acolyte/master/screenshot.png
            :target:             https://raw.githubusercontent.com/coldfix/steam-acolyte/master/screenshot.png
            :alt:                Screenshot (usernames were changed)
         
         CHANGES
         -------
         
+        0.9.0
+        ~~~~~
+        Date: 25.05.2023
+        
+        - no longer modify/replace config.vdf (see #28)
+        - remove obsolete "logout" button
+        - the files in ``steam/acolyte/*/config.vdf`` that were created by
+          previous versions of the program no longer have any purposes
+        
+        
         0.8.1
         ~~~~~
         Date: 09.10.2022
         
         - new build to trigger PyPI/AUR deployment…
           It turns out, using ``schedule:`` in a GitHub Actions seems to prevent
           it from being run on push (or at least that seems to be the case after
```

### Comparing `steam-acolyte-0.8.1/UNLICENSE` & `steam-acolyte-0.9.0/UNLICENSE`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/setup.cfg` & `steam-acolyte-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 	vdf
 	docopt
 	importlib_resources; python_version < '3.7'
 include_package_data = true
 zip_safe = true
 
 [options.entry_points]
-console-scripts = 
+console_scripts = 
 	steam-acolyte = steam_acolyte.app:main
 
 [metadata]
 name = steam-acolyte
 description = Lightweight user account switcher/login keeper for steam
 url = https://github.com/coldfix/steam-acolyte
 long_description = file: README.rst, CHANGES.rst
```

### Comparing `steam-acolyte-0.8.1/steam_acolyte/acolyte.svg` & `steam-acolyte-0.9.0/steam_acolyte/acolyte.svg`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/app.py` & `steam-acolyte-0.9.0/steam_acolyte/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,33 +85,29 @@
         if not first:
             print("Acolyte is already running. Terminating.")
             return 0
         if cli_mode:
             if not locked:
                 print("Waiting for steam to exit.")
                 steam.wait_for_lock()
-            if opts['store']:
-                steam.store_login_cookie()
-            elif opts['switch']:
+            if opts['switch']:
                 steam.switch_user(opts['<USER>'])
             elif opts['start']:
                 steam.switch_user(opts['<USER>'])
                 steam.unlock()
                 steam.run().waitForFinished(-1)
                 steam.lock()
-                steam.store_login_cookie()
         else:
             from steam_acolyte.window import LoginDialog
             from steam_acolyte.theme import load_theme
             init_app()
             window = LoginDialog(steam, load_theme())
             window.show_trayicon()
             try:
                 if locked:
-                    steam.store_login_cookie()
                     window.show()
                 else:
                     print("Waiting for steam to exit.")
                     window.show_waiting_message()
                     window.wait_for_lock()
                 return app.exec_()
             finally:
```

### Comparing `steam-acolyte-0.8.1/steam_acolyte/funcwrap.py` & `steam-acolyte-0.9.0/steam_acolyte/funcwrap.py`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/plus.svg` & `steam-acolyte-0.9.0/steam_acolyte/plus.svg`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/steam.py` & `steam-acolyte-0.9.0/steam_acolyte/steam.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from PyQt5.QtCore import QObject, pyqtSignal, QProcess
 import vdf
 
 import os
 import sys
 import shlex
 from time import sleep
-from shutil import copyfile
 from abc import abstractmethod
 
 if sys.platform == 'win32':
     from .steam_win32 import SteamWin32 as SteamImpl
 else:
     from .steam_linux import SteamLinux as SteamImpl
 
@@ -191,74 +190,36 @@
         users = subkey_lookup(config, r'users')
         return [
             SteamUser(uid, u['AccountName'], u['PersonaName'], u['Timestamp'])
             for uid, u in users.items()
         ]
 
     @trace.method
-    def store_login_cookie(self):
-        """Save the login token from the last active steam account."""
-        username = self.get_last_user()
-        userpath = os.path.join(self.acolyte_data, username, 'config.vdf')
-        configpath = os.path.join(self.steam_config, 'config.vdf')
-        config = self.read_config('config.vdf')
-        accounts = subkey_lookup(
-            config, r'InstallConfigStore\Software\Valve\Steam\Accounts')
-        if accounts.get(username):
-            os.makedirs(os.path.dirname(userpath), exist_ok=True)
-            copyfile(configpath, userpath)
-        else:
-            print("Not replacing login data for logged out user: {!r}"
-                  .format(username))
-
-    @trace.method
-    def remove_login_cookie(self, username):
-        """Delete saved login token."""
-        userpath = os.path.join(self.acolyte_data, username, 'config.vdf')
-        if os.path.isfile(userpath):
-            os.remove(userpath)
-
-    @trace.method
     def remove_user(self, username):
         """Delete login token and remove account from the list of saved
         accounts."""
-        self.remove_login_cookie(username)
         loginusers = self.read_config('loginusers.vdf')
         loginusers['users'] = {
             uid: info
             for uid, info in subkey_lookup(loginusers, r'users').items()
             if info['AccountName'] != username
         }
         self.write_config('loginusers.vdf', loginusers)
 
         config = self.read_config('config.vdf')
         accounts = subkey_lookup(
             config, r'InstallConfigStore\Software\Valve\Steam\Accounts')
         accounts.pop(username, None)
         self.write_config('config.vdf', config)
 
-    def has_cookie(self, username):
-        """Check if there is a saved login cookie."""
-        userpath = os.path.join(self.acolyte_data, username, 'config.vdf')
-        return bool(username) and os.path.isfile(userpath)
-
     @trace.method
     def switch_user(self, username):
         """Switch login config to given user. Do not use this while steam is
         running."""
         self.set_last_user(username)
-        if not username:
-            return True
-        userpath = os.path.join(self.acolyte_data, username, 'config.vdf')
-        configpath = os.path.join(self.steam_config, 'config.vdf')
-        if not os.path.isfile(userpath):
-            print("No stored config found for {!r}".format(username),
-                  file=sys.stderr)
-            return False
-        copyfile(userpath, configpath)
         return True
 
     @trace.method
     def run(self):
         """Run steam."""
         process = self._process = QProcess()
         process.setInputChannelMode(QProcess.ForwardedInputChannel)
@@ -275,19 +236,19 @@
     def stop(self):
         """Signal steam to exit."""
         if not self.has_steam_lock():
             if self._is_steam_pid_valid() and self._connect():
                 self._send([self.exe, '-shutdown'])
 
     @trace.method
-    def read_config(self, filename='config.vdf'):
-        """Read steam config.vdf file."""
+    def read_config(self, filename):
+        """Read a steam .vdf config file."""
         conf = os.path.join(self.steam_config, filename)
         text = read_file(conf)
         return vdf.loads(text) if text else {}
 
     @trace.method
     def write_config(self, filename, data):
-        """Write steam config.vdf file."""
+        """Write a steam .vdf config file."""
         conf = os.path.join(self.steam_config, filename)
         text = vdf.dumps(data, pretty=True)
         write_file(conf, text)
```

### Comparing `steam-acolyte-0.8.1/steam_acolyte/steam_linux.py` & `steam-acolyte-0.9.0/steam_acolyte/steam_linux.py`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/steam_win32.py` & `steam-acolyte-0.9.0/steam_acolyte/steam_win32.py`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/theme.py` & `steam-acolyte-0.9.0/steam_acolyte/theme.py`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/user.svg` & `steam-acolyte-0.9.0/steam_acolyte/user.svg`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/util.py` & `steam-acolyte-0.9.0/steam_acolyte/util.py`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/window.css` & `steam-acolyte-0.9.0/steam_acolyte/window.css`

 * *Files identical despite different names*

### Comparing `steam-acolyte-0.8.1/steam_acolyte/window.py` & `steam-acolyte-0.9.0/steam_acolyte/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         login command, or activates the user list widget if no command was
         queued."""
         if self._exit:
             self.close()
             return
         self.stopAction.setEnabled(False)
         self.wait_task = None
-        self.steam.store_login_cookie()
         self.update_userlist()
         if self._login:
             self.run_steam(self._login)
             self._login = None
             return
         self.show()
 
@@ -302,52 +301,36 @@
         bot_label.setObjectName("AccountName")
         top_font = top_label.font()
         top_font.setBold(True)
         top_font.setPointSize(top_font.pointSize() + 2)
         top_label.setFont(top_font)
         labels.addWidget(top_label)
         labels.addWidget(bot_label)
-        self.logout_action = QAction()
-        self.logout_action.triggered.connect(self.logout_clicked)
-        self.logout_action.setIcon(self.theme.logout_icon)
-        self.logout_action.setToolTip("Delete saved login")
-        self.logout_action.setWhatsThis(
-            "Logout user by deleting the saved login token.\n"
-            "The user will stay visible on this list.")
         self.delete_action = QAction()
         self.delete_action.triggered.connect(self.delete_clicked)
         self.delete_action.setIcon(theme.delete_icon)
         self.delete_action.setToolTip("Delete user from list")
-        self.delete_action.setWhatsThis(
-            "Logout and remove user from this list.")
-        self.logout_button = QToolButton()
-        self.logout_button.setDefaultAction(self.logout_action)
+        self.delete_action.setWhatsThis("Remove user from this list.")
         self.delete_button = QToolButton()
         self.delete_button.setDefaultAction(self.delete_action)
         layout.setSpacing(0)
         layout.addWidget(ico_label)
         layout.addSpacing(10)
         layout.addLayout(labels)
         layout.addStretch()
         layout.addSpacing(10)
-        layout.addWidget(self.logout_button)
         layout.addWidget(self.delete_button)
         self.setLayout(layout)
         self.clicked.connect(self.login_clicked)
         self.update_ui()
 
     def login_clicked(self):
         self.window().login(self.user.account_name)
 
-    def logout_clicked(self):
-        self.steam.remove_login_cookie(self.user.account_name)
-        self.update_ui()
-
     def delete_clicked(self):
         self.steam.remove_user(self.user.account_name)
         self.hide()
         self.window().adjustSize()
 
     def update_ui(self):
         username = self.user.account_name
-        self.logout_button.setVisible(self.steam.has_cookie(username))
         self.delete_button.setVisible(bool(username))
```

### Comparing `steam-acolyte-0.8.1/steam_acolyte.egg-info/PKG-INFO` & `steam-acolyte-0.9.0/steam_acolyte.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-acolyte
-Version: 0.8.1
+Version: 0.9.0
 Summary: Lightweight user account switcher/login keeper for steam
 Home-page: https://github.com/coldfix/steam-acolyte
 Author: Thomas Gläßle
 Author-email: thomas@coldfix.de
 License: Unlicense
 Description: Steam Acolyte
         =============
@@ -68,42 +68,44 @@
         
         Optionally, modify your steam launchers to execute ``steam-acolyte``.
         
         
         How it works
         ------------
         
-        *acolyte* works dead-simple by saving the login token for the last active
-        steam account upon program start. When the user clicks on a particular account
-        it simply restores the corresponding token and then starts steam. *acolyte*
-        only stores login tokes, but never any passwords! This has the following
-        implications:
+        *acolyte* does not inspect or store any password or login tokens at all. It
+        only tells steam which user to login when starting. Steam uses its own
+        mechanism to store login information. This has the following consequences:
         
         - the login token can be used to login without having to re-enter 2FA
-          (whereas for password-based logins you would need to redo 2FA)
-        - the login token can only be used for a single login
-        - after a successful login, steam will create a fresh token which acolyte can
-          save for the next cycle when steam exits or when acolyte is started the next
-          time
-        - it is no problem to start and exit steam several times without acolyte
-          running (as long as you always sign on with the same account), because
-          acolyte will always pick up the most recent login token when it starts
-        - the token expires if unused for a several weeks
+          (whereas for password-based login manager you would need to redo 2FA)
+        - you can mix using steam with or without acolyte
+        - active logins expire if unused for a several weeks
         - selecting "Change Account" from the steam menu or "Log Out User" in Big
           Picture mode UI invalidates the login and you will have to reenter your
           password for the logged out user
         
         
         .. |Screenshot| image:: https://raw.githubusercontent.com/coldfix/steam-acolyte/master/screenshot.png
            :target:             https://raw.githubusercontent.com/coldfix/steam-acolyte/master/screenshot.png
            :alt:                Screenshot (usernames were changed)
         
         CHANGES
         -------
         
+        0.9.0
+        ~~~~~
+        Date: 25.05.2023
+        
+        - no longer modify/replace config.vdf (see #28)
+        - remove obsolete "logout" button
+        - the files in ``steam/acolyte/*/config.vdf`` that were created by
+          previous versions of the program no longer have any purposes
+        
+        
         0.8.1
         ~~~~~
         Date: 09.10.2022
         
         - new build to trigger PyPI/AUR deployment…
           It turns out, using ``schedule:`` in a GitHub Actions seems to prevent
           it from being run on push (or at least that seems to be the case after
```

### Comparing `steam-acolyte-0.8.1/steam_acolyte.egg-info/SOURCES.txt` & `steam-acolyte-0.9.0/steam_acolyte.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 steam_acolyte/__init__.py
 steam_acolyte/__main__.py
 steam_acolyte/acolyte.svg
 steam_acolyte/app.py
 steam_acolyte/async_.py
 steam_acolyte/delete.svg
 steam_acolyte/funcwrap.py
-steam_acolyte/logout.svg
 steam_acolyte/plus.svg
 steam_acolyte/steam.py
 steam_acolyte/steam_linux.py
 steam_acolyte/steam_win32.py
 steam_acolyte/theme.py
 steam_acolyte/user.svg
 steam_acolyte/util.py
```

