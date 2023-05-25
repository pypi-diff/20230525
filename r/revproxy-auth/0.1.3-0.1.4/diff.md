# Comparing `tmp/revproxy_auth-0.1.3.tar.gz` & `tmp/revproxy_auth-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.1.3.tar", last modified: Tue May 23 14:55:12 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.4.tar", last modified: Thu May 25 07:01:10 2023, max compression
```

## Comparing `revproxy_auth-0.1.3.tar` & `revproxy_auth-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.553099 revproxy_auth-0.1.3/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.553099 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/test_001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.767554 revproxy_auth-0.1.4/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.767554 revproxy_auth-0.1.4/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.767554 revproxy_auth-0.1.4/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-25 07:01:10.000000 revproxy_auth-0.1.4/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 07:01:10.000000 revproxy_auth-0.1.4/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:01:10.000000 revproxy_auth-0.1.4/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 07:01:10.000000 revproxy_auth-0.1.4/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 07:01:10.000000 revproxy_auth-0.1.4/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:01:10.771554 revproxy_auth-0.1.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-25 07:00:58.000000 revproxy_auth-0.1.4/tests/test_001.py
```

### Comparing `revproxy_auth-0.1.3/PKG-INFO` & `revproxy_auth-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy_auth
-Version: 0.1.3
+Version: 0.1.4
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.3/README.md` & `revproxy_auth-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.3/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.4/revproxy_auth/revproxy_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,25 +212,24 @@
 
     def _credentials_valid(self, form):
         token = form.get('revproxy_auth', None)
         if token:
             user = form.get('user', '').strip(' \t\n\r')
             password = form.get('password', '').strip(' \t\n\r')
             otp = form.get('OTP', '').strip(' \t\n\r')
-            testing_credentials = self._config['testing_credentials']
-            if not testing_credentials:
-                url = (f'{self._config["NAS"]}/webapi/entry.cgi?api=SYNO.API.Auth&version=6&method=login'
-                       f'&account={user}&passwd={password}&otp_code={otp}')
-                auth_response = requests.get(url, timeout=10)
-                # Verify authentication
-                return auth_response.json()['success']
-            else: # Testing credentiales
-                return user == testing_credentials['user'] and \
-                       password == testing_credentials['password'] and \
-                       otp == testing_credentials['OTP']
+            for credential in self._config['credentials']:
+                if credential['user'] == user and credential['password'] == password and credential['OTP'] == otp:
+                    print('Validating credentials by user/password...')
+                    return True
+            print('Validating credentials Synology Auth...')
+            url = (f'{self._config["NAS"]}/webapi/entry.cgi?api=SYNO.API.Auth&version=6&method=login'
+                   f'&account={user}&passwd={password}&otp_code={otp}')
+            auth_response = requests.get(url, timeout=10)
+            # Verify authentication
+            return auth_response.json()['success']
         return False
 
     def _call_inner_get(self, host, endpoint, params, headers) -> Response:
         fullpath = parse.urljoin(host, endpoint)
         resp = requests.get(fullpath,
                             params=params,
                             headers = headers,
@@ -286,15 +285,15 @@
 
     def _first_auth_and_redirect(self, req: Request) -> Response:
         cookie_name = req.form.get('revproxy_auth', None)
         cookie = self._get_local_auth_cookie(cookie_name)
         if cookie:
             print(f'Local cookie {cookie_name} still alive')
             if self._credentials_valid(req.form):
-                print('Credentials validated by synology NAS')
+                print('Credentials validated.')
                 # Search for the cookie and redirect to related URL if present
                 if cookie['method'] == 'GET':
                     response = self._call_inner_get(cookie['host'], cookie['endpoint'], cookie['params'], cookie['headers'])
                 else:
                     response = self._call_inner_post(cookie['host'], cookie['endpoint'], cookie['content'], cookie['headers'])
                 response.set_cookie('token', cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else: # We come from the auth popup, but credentials are invalid --> ask again for credentials
```

### Comparing `revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.4/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.3/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.4/revproxy_auth/templates/form.html`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.3/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.4/revproxy_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy-auth
-Version: 0.1.3
+Version: 0.1.4
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.3/setup.py` & `revproxy_auth-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.1.3",
+    version="0.1.4",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
```

### Comparing `revproxy_auth-0.1.3/tests/test_000.py` & `revproxy_auth-0.1.4/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.3/tests/test_001.py` & `revproxy_auth-0.1.4/tests/test_001.py`

 * *Files identical despite different names*

