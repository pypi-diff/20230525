# Comparing `tmp/flask_matomo2-0.2.6.tar.gz` & `tmp/flask_matomo2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_matomo2-0.2.6.tar", max compression
+gzip compressed data, was "flask_matomo2-0.3.0.tar", max compression
```

## Comparing `flask_matomo2-0.2.6.tar` & `flask_matomo2-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/LICENSE
--rw-r--r--   0        0        0     4756 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/README.md
--rw-r--r--   0        0        0      114 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/flask_matomo2/__init__.py
--rw-r--r--   0        0        0     8650 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/flask_matomo2/core.py
--rw-r--r--   0        0        0     1250 2023-05-22 10:52:36.890973 flask_matomo2-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5893 1970-01-01 00:00:00.000000 flask_matomo2-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4928 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/README.md
+-rw-r--r--   0        0        0      161 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/flask_matomo2/__init__.py
+-rw-r--r--   0        0        0     8348 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/flask_matomo2/core.py
+-rw-r--r--   0        0        0        0 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/flask_matomo2/py.typed
+-rw-r--r--   0        0        0     1099 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/flask_matomo2/trackers.py
+-rw-r--r--   0        0        0     1250 2023-05-25 07:36:32.878024 flask_matomo2-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5775 1970-01-01 00:00:00.000000 flask_matomo2-0.3.0/setup.py
+-rw-r--r--   0        0        0     6065 1970-01-01 00:00:00.000000 flask_matomo2-0.3.0/PKG-INFO
```

### Comparing `flask_matomo2-0.2.6/LICENSE` & `flask_matomo2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_matomo2-0.2.6/README.md` & `flask_matomo2-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,19 @@
 Lucas Hild - [https://lucas-hild.de](https://lucas.hild.de)
 This project is licensed under the MIT License - see the LICENSE file for details
 
 # Release Notes
 
 ## Latest Changes
 
+## 0.3.0 - 2023-05-25
+
+### Added
+
+- Add PerfMsTracker. PR [#33](https://github.com/spraakbanken/flask-matomo2/pull/33) by [@kod-kristoff](https://github.com/kod-kristoff).
 
 ## 0.2.0 - 2023-05-22
 ### Changed
 
 - Track original IP address if request was forwarded by proxy. [Tanikai/flask-matomo](https://github.com/Tanikai/flask-matomo) by [@Tanakai](https://github.com/Tanakai).
 - Change ignored routes to compare against rules instead of endpoint. [MSU-Libraries/flask-matomo](https://github.com/MSU-Libraries/flask-matomo) by [@meganschanz](https://github.com/meganschanz).
 - Add ignored UserAgent prefix; set action to be url_rule. [MSU-Libraries/flask-matomo](https://github.com/MSU-Libraries/flask-matomo) by [@natecollins](https://github.com/natecollins).
```

### Comparing `flask_matomo2-0.2.6/flask_matomo2/core.py` & `flask_matomo2-0.3.0/flask_matomo2/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,14 @@
         self.routes_details: typing.Dict[str, typing.Dict[str, str]] = routes_details or {}
         self.client = client or httpx.Client()
         if ignored_patterns:
             self._ignored_patterns = [re.compile(pattern) for pattern in ignored_patterns]
 
         if not matomo_url:
             raise ValueError("matomo_url has to be set")
-        if type(id_site) != int:
-            raise ValueError("id_site has to be an integer")
         if not self.token_auth:
             logger.warning("'token_auth' not given, NOT tracking ip-address")
 
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app):
@@ -83,24 +81,16 @@
             str(request.user_agent).startswith(ua_prefix)
             for ua_prefix in self.ignored_ua_prefixes
         ):
             return
         if any(pattern.match(url_rule) for pattern in self._ignored_patterns):
             return
 
-        if self.base_url:
-            url = self.base_url + request.path
-        else:
-            url = request.url
-
-        if request.url_rule:
-            action_name = url_rule
-        else:
-            action_name = "Not Found"
-
+        url = self.base_url + request.path if self.base_url else request.url
+        action_name = url_rule if request.url_rule else "Not Found"
         user_agent = request.user_agent
         # If request was forwarded (e.g. by a proxy), then get origin IP from
         # HTTP_X_FORWARDED_FOR. If this header field doesn't exist, return
         # remote_addr.
         ip_address = request.environ.get("HTTP_X_FORWARDED_FOR", request.remote_addr)
 
         data = {
@@ -130,16 +120,14 @@
 
         # Overwrite action_name, if it was configured with details()
         if self.routes_details.get(action_name) and self.routes_details.get(action_name, {}).get(
             "action_name"
         ):
             data["action_name"] = self.routes_details.get(action_name, {}).get("action_name")
 
-        # Create new thread with request, because otherwise the original request will be blocked
-        # Thread(target=self.track, kwargs=keyword_arguments).start()
         g.flask_matomo2 = {
             "tracking": True,
             "start_ns": time.perf_counter_ns(),
             "tracking_data": data,
         }
 
     def after_request(self, response: flask.Response):
@@ -155,15 +143,15 @@
 
         return response
 
     def teardown_request(self, exc: typing.Optional[Exception] = None) -> None:
         tracking_state = g.get("flask_matomo2", {})
         if not tracking_state.get("tracking", False):
             return
-
+        logger.debug(f"{tracking_state=}")
         tracking_data = tracking_state["tracking_data"]
         for key, value in tracking_state.get("custom_tracking_data", {}).items():
             if key == "cvar" and "cvar" in tracking_data:
                 tracking_data["cvar"].update(value)
             else:
                 tracking_data[key] = value
 
@@ -193,15 +181,15 @@
         """
         if "cvar" in tracking_data:
             cvar = tracking_data.pop("cvar")
             tracking_data["cvar"] = json.dumps(cvar)
         tracking_params = urllib.parse.urlencode(tracking_data)
 
         tracking_url = f"{self.matomo_url}?{tracking_params}"
-        print(f"calling {tracking_url}")
+        logger.debug(f"calling {tracking_url}")
         try:
             r = self.client.get(tracking_url)
 
             if r.status_code >= 300:
                 logger.error(
                     "Tracking call failed (status_code=%d)",
                     r.status_code,
```

### Comparing `flask_matomo2-0.2.6/pyproject.toml` & `flask_matomo2-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-matomo2"
-version = "0.2.6"
+version = "0.3.0"
 description = "Track requests to your Flask server with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "flask_matomo2"}]
 classifiers=[
     "Environment :: Web Environment",
```

### Comparing `flask_matomo2-0.2.6/PKG-INFO` & `flask_matomo2-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-matomo2
-Version: 0.2.6
+Version: 0.3.0
 Summary: Track requests to your Flask server with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
@@ -141,14 +141,19 @@
 Lucas Hild - [https://lucas-hild.de](https://lucas.hild.de)
 This project is licensed under the MIT License - see the LICENSE file for details
 
 # Release Notes
 
 ## Latest Changes
 
+## 0.3.0 - 2023-05-25
+
+### Added
+
+- Add PerfMsTracker. PR [#33](https://github.com/spraakbanken/flask-matomo2/pull/33) by [@kod-kristoff](https://github.com/kod-kristoff).
 
 ## 0.2.0 - 2023-05-22
 ### Changed
 
 - Track original IP address if request was forwarded by proxy. [Tanikai/flask-matomo](https://github.com/Tanikai/flask-matomo) by [@Tanakai](https://github.com/Tanakai).
 - Change ignored routes to compare against rules instead of endpoint. [MSU-Libraries/flask-matomo](https://github.com/MSU-Libraries/flask-matomo) by [@meganschanz](https://github.com/meganschanz).
 - Add ignored UserAgent prefix; set action to be url_rule. [MSU-Libraries/flask-matomo](https://github.com/MSU-Libraries/flask-matomo) by [@natecollins](https://github.com/natecollins).
```

