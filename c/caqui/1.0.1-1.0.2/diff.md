# Comparing `tmp/caqui-1.0.1.tar.gz` & `tmp/caqui-1.0.2.tar.gz`

## Comparing `caqui-1.0.1.tar` & `caqui-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 caqui-1.0.1/publish.sh
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 caqui-1.0.1/sample.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.1/caqui/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 caqui-1.0.1/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.1/caqui/constants.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 caqui-1.0.1/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/constants.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/sniffer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/doubles/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/doubles/fake_responses.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/feature/test_functions.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/html/playground.html
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/unit/__initi__.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 caqui-1.0.1/tests/unit/test_sync_unit.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 caqui-1.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.1/LICENSE
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 caqui-1.0.1/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 caqui-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 caqui-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 caqui-1.0.2/publish.sh
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 caqui-1.0.2/sample.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 caqui-1.0.2/test-requirements.txt
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.2/caqui/__init__.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 caqui-1.0.2/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.2/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.2/caqui/exceptions.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 caqui-1.0.2/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/constants.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/sniffer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/doubles/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/doubles/fake_responses.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/feature/test_functions.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/html/playground.html
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 caqui-1.0.2/tests/unit/test_sync_unit.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 caqui-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.2/LICENSE
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 caqui-1.0.2/README.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 caqui-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 caqui-1.0.2/PKG-INFO
```

### Comparing `caqui-1.0.1/sample.py` & `caqui-1.0.2/sample.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/caqui/__init__.py` & `caqui-1.0.2/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/caqui/asynchronous.py` & `caqui-1.0.2/caqui/asynchronous.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,99 @@
 import aiohttp
 import json
 from caqui.constants import HEADERS
+from caqui.exceptions import WebDriverError
 
 
 async def __post(url, payload):
-    async with aiohttp.ClientSession() as session:
-        async with session.post(url, data=payload, headers=HEADERS) as resp:
-            response = await resp.json()
-            return response
+    try:
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, data=payload, headers=HEADERS) as resp:
+                response = await resp.json()
+                return response
+    except Exception as error:
+        raise WebDriverError("'POST' request failed.") from error
 
 
 async def get_property_value(driver_url, session, element):
-    url = f"{driver_url}/session/{session}/element/{element}/property/value"
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url, headers=HEADERS) as resp:
-            response = await resp.json()
-            return response.get("value")
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/property/value"
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, headers=HEADERS) as resp:
+                response = await resp.json()
+                return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get value from element.") from error
 
 
 async def get_text(driver_url, session, element):
-    url = f"{driver_url}/session/{session}/element/{element}/text"
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url, headers=HEADERS) as resp:
-            response = await resp.json()
-            return response.get("value")
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/text"
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, headers=HEADERS) as resp:
+                response = await resp.json()
+                return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get text from element.") from error
 
 
 async def close_session(driver_url, session):
-    url = f"{driver_url}/session/{session}"
-    async with aiohttp.ClientSession() as session:
-        async with session.delete(url, headers=HEADERS) as resp:
-            response = await resp.json()
-            return response.get("sessionId")
+    try:
+        url = f"{driver_url}/session/{session}"
+        async with aiohttp.ClientSession() as session:
+            async with session.delete(url, headers=HEADERS) as resp:
+                response = await resp.json()
+                return response.get("sessionId")
+    except Exception as error:
+        raise WebDriverError("Failed to close session.") from error
 
 
 async def go_to_page(driver_url, session, page_url):
-    url = f"{driver_url}/session/{session}/url"
-    payload = json.dumps({"url": page_url})
-    response = await __post(url, payload)
-    return response.get("sessionId")
+    try:
+        url = f"{driver_url}/session/{session}/url"
+        payload = json.dumps({"url": page_url})
+        response = await __post(url, payload)
+        return response.get("sessionId")
+    except Exception as error:
+        raise WebDriverError(f"Failed to navigate to page '{page_url}'.") from error
 
 
 async def send_keys(driver_url, session, element, text):
-    url = f"{driver_url}/session/{session}/element/{element}/value"
-    payload = json.dumps({"text": text, "value": [*text], "id": element})
-    response = await __post(url, payload)
-    return response.get("sessionId")
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/value"
+        payload = json.dumps({"text": text, "value": [*text], "id": element})
+        response = await __post(url, payload)
+        return response.get("sessionId")
+    except Exception as error:
+        raise WebDriverError(f"Failed to send key '{text}'.") from error
 
 
 async def click(driver_url, session, element):
-    payload = json.dumps({"id": element})
-    url = f"{driver_url}/session/{session}/element/{element}/click"
-    response = await __post(url, payload)
-    return response.get("sessionId")
+    try:
+        payload = json.dumps({"id": element})
+        url = f"{driver_url}/session/{session}/element/{element}/click"
+        response = await __post(url, payload)
+        return response.get("sessionId")
+    except Exception as error:
+        raise WebDriverError("Failed to click on element.") from error
 
 
 async def find_element(driver_url, session, locator_type, locator_value):
-    payload = json.dumps({"using": locator_type, "value": locator_value})
-    url = f"{driver_url}/session/{session}/element"
-    response = await __post(url, payload)
-    return response.get("value").get("ELEMENT")
+    try:
+        payload = json.dumps({"using": locator_type, "value": locator_value})
+        url = f"{driver_url}/session/{session}/element"
+        response = await __post(url, payload)
+        return response.get("value").get("ELEMENT")
+    except Exception as error:
+        raise WebDriverError(
+            f"Failed to find element by '{locator_type}'-'{locator_value}'."
+        ) from error
 
 
 async def get_session(driver_url, capabilities):
-    payload = json.dumps(capabilities)
-    url = f"{driver_url}/session"
-    response = await __post(payload, url)
-    return response.get("sessionId")
+    try:
+        payload = json.dumps(capabilities)
+        url = f"{driver_url}/session"
+        response = await __post(url, payload)
+        return response.get("sessionId")
+    except Exception as error:
+        raise WebDriverError("Failed to open session.") from error
```

### Comparing `caqui-1.0.1/tests/sniffer.py` & `caqui-1.0.2/tests/sniffer.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/tests/doubles/fake_responses.py` & `caqui-1.0.2/tests/doubles/fake_responses.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/tests/feature/test_functions.py` & `caqui-1.0.2/tests/feature/test_functions.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/tests/html/playground.html` & `caqui-1.0.2/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/tests/integration/test_async_scenarios.py` & `caqui-1.0.2/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/tests/integration/test_sync_scenarios.py` & `caqui-1.0.2/tests/integration/test_sync_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/tests/unit/test_async_unit.py` & `caqui-1.0.2/tests/unit/test_sync_unit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,127 +1,101 @@
-from pytest import mark, fixture
-from caqui.asynchronous import (
-    get_session,
+import json
+from unittest.mock import patch
+from caqui.synchronous import (
     find_element,
+    get_session,
     click,
     send_keys,
-    go_to_page,
-    close_session,
     get_text,
+    close_session,
+    go_to_page,
     get_property_value,
 )
-from unittest.mock import patch
 from tests.doubles.fake_responses import (
-    GET_SESSION,
     FIND_ELEMENT,
+    GET_SESSION,
     CLICK,
-    SEND_KEYS,
-    GO_TO_PAGE,
     GET_TEXT,
+    CLOSE_SESSION,
+    GO_TO_PAGE,
+    GET_PROPERTY_VALUE,
+    SEND_KEYS,
 )
 
 
-class Request:
-    def __init__(self, return_value) -> None:
-        self.__return_value = return_value
-
-    def release(*args):
-        pass
-
-    async def session(self, *args):
-        return self.__return_value
-
-    def json(self, *args):
-        return self.session(*args)
-
-
-def request_mock(*args):
-    return Request(*args)
-
-
-@fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     session = "4358a5b53794586af59678fc1653dc40"
     element = "0.8851292311864847-1"
-
     return driver_url, session, element
 
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(GET_TEXT))
-async def test_get_property_value(mock, __setup):
-    driver_url, session, element = __setup
-    text = "any"
-
-    assert await get_property_value(driver_url, session, element) == text
+@patch("requests.request", return_value=GET_PROPERTY_VALUE)
+def test_get_property_value(*args):
+    driver_url, session, _ = __setup()
+    element = "any"
+    expected = "any_value"
+
+    assert get_property_value(driver_url, session, element) == expected
 
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(GET_TEXT))
-async def test_get_text(mock, __setup):
-    driver_url, session, element = __setup
-    text = "any"
+@patch("requests.request", return_value=GO_TO_PAGE)
+def test_go_to_page(*args):
+    driver_url, session, _ = __setup()
+    url = "http://any.com"
 
-    assert await get_text(driver_url, session, element) == text
+    assert go_to_page(driver_url, session, url) == session
 
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(GET_SESSION))
-async def test_close_session(mock, __setup):
-    driver_url, session, _ = __setup
+@patch("requests.request", return_value=CLOSE_SESSION)
+def test_close_session(*args):
+    driver_url, session, _ = __setup()
 
-    assert await close_session(driver_url, session) == session
+    assert close_session(driver_url, session) == session
 
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(GO_TO_PAGE))
-async def test_go_to_page(mock, __setup):
-    driver_url, session, _ = __setup
-    url = "http://any.com"
+@patch("requests.request", return_value=GET_TEXT)
+def test_get_text(*args):
+    driver_url, session, element = __setup()
+    expected = "any"
 
-    assert await go_to_page(driver_url, session, url) == session
+    assert get_text(driver_url, session, element) == expected
 
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(SEND_KEYS))
-async def test_send_keys(mock, __setup):
-    driver_url, session, element = __setup
+@patch("requests.request", return_value=SEND_KEYS)
+def test_send_keys(*args):
+    driver_url, session, element = __setup()
     text = "any"
 
-    assert await send_keys(driver_url, session, element, text) == session
-
+    assert send_keys(driver_url, session, element, text) == session
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(CLICK))
-async def test_click(mock, __setup):
-    driver_url, session, element = __setup
 
-    assert await click(driver_url, session, element) == session
+@patch("requests.request", return_value=CLICK)
+def test_click(*args):
+    driver_url, session, element = __setup()
 
+    assert click(driver_url, session, element) == session
 
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(FIND_ELEMENT))
-async def test_find_element(mock, __setup):
-    driver_url, session, element = __setup
-    locator_type = "xpath"
-    locator_value = "//input"
-
-    assert (
-        await find_element(driver_url, session, locator_type, locator_value) == element
-    )
 
-
-@mark.asyncio
-@patch("aiohttp.ClientSession._request", return_value=request_mock(GET_SESSION))
-async def test_get_session(*args):
+@patch("requests.request", return_value=GET_SESSION)
+def test_get_session(*args):
     driver_url = "http://127.0.0.1:9999"
-    capabilities = {
+    payload = {
         "desiredCapabilities": {
             "browserName": "firefox",
             "marionette": True,
             "acceptInsecureCerts": True,
         }
     }
     expected = "4358a5b53794586af59678fc1653dc40"
 
-    assert await get_session(driver_url, capabilities) == expected
+    assert get_session(driver_url, payload) == expected
+
+
+@patch("requests.request", return_value=FIND_ELEMENT)
+def test_find_element(*args):
+    driver_url, session, _ = __setup()
+    locator_type = "xpath"
+    locator_value = "//input"
+    expected = "0.8851292311864847-1"
+
+    assert find_element(driver_url, session, locator_type, locator_value) == expected
```

### Comparing `caqui-1.0.1/.gitignore` & `caqui-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/LICENSE` & `caqui-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.1/README.md` & `caqui-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -222,7 +222,25 @@
   --version                       print the version number and exit
   --url-base                      base URL path prefix for commands, e.g. wd/url
   --readable-timestamp            add readable timestamps to log
   --enable-chrome-logs            show logs from the browser (overrides other logging options)
   --disable-dev-shm-usage         do not use /dev/shm (add this switch if seeing errors related to shared memory)
   --allowed-ips                   comma-separated allowlist of remote IP addresses which are allowed to connect to ChromeDriver
 ```
+# Contributing
+Install the dependencies (Python >= 3.7)
+```
+python3 -m venv venv
+pip install -e .
+pip install -r test-requirements.txt
+```
+Fork this repository, make the changes into the forked repository and push a new Merge Request to 'main' branch.
+Open an issue in case of big MRs.
+# Testing
+To run the tests, start a new Driver as server on port `9999`, for example:
+```
+./chromedriver --port=9999
+```
+And execute the tests
+```
+python -m pytest
+```
```

#### html2text {}

```diff
@@ -90,8 +90,13 @@
 (experimental) log verbosely and don't truncate long strings so that the log
 can be replayed. --version print the version number and exit --url-base base
 URL path prefix for commands, e.g. wd/url --readable-timestamp add readable
 timestamps to log --enable-chrome-logs show logs from the browser (overrides
 other logging options) --disable-dev-shm-usage do not use /dev/shm (add this
 switch if seeing errors related to shared memory) --allowed-ips comma-separated
 allowlist of remote IP addresses which are allowed to connect to ChromeDriver
-```
+``` # Contributing Install the dependencies (Python >= 3.7) ``` python3 -m venv
+venv pip install -e . pip install -r test-requirements.txt ``` Fork this
+repository, make the changes into the forked repository and push a new Merge
+Request to 'main' branch. Open an issue in case of big MRs. # Testing To run
+the tests, start a new Driver as server on port `9999`, for example: ``` ./
+chromedriver --port=9999 ``` And execute the tests ``` python -m pytest ```
```

### Comparing `caqui-1.0.1/pyproject.toml` & `caqui-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "caqui"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `caqui-1.0.1/PKG-INFO` & `caqui-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 1.0.1
+Version: 1.0.2
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -239,7 +239,25 @@
   --version                       print the version number and exit
   --url-base                      base URL path prefix for commands, e.g. wd/url
   --readable-timestamp            add readable timestamps to log
   --enable-chrome-logs            show logs from the browser (overrides other logging options)
   --disable-dev-shm-usage         do not use /dev/shm (add this switch if seeing errors related to shared memory)
   --allowed-ips                   comma-separated allowlist of remote IP addresses which are allowed to connect to ChromeDriver
 ```
+# Contributing
+Install the dependencies (Python >= 3.7)
+```
+python3 -m venv venv
+pip install -e .
+pip install -r test-requirements.txt
+```
+Fork this repository, make the changes into the forked repository and push a new Merge Request to 'main' branch.
+Open an issue in case of big MRs.
+# Testing
+To run the tests, start a new Driver as server on port `9999`, for example:
+```
+./chromedriver --port=9999
+```
+And execute the tests
+```
+python -m pytest
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.0.1 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 1.0.2 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
 noemail.com> License-File: LICENSE Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
@@ -98,8 +98,13 @@
 (experimental) log verbosely and don't truncate long strings so that the log
 can be replayed. --version print the version number and exit --url-base base
 URL path prefix for commands, e.g. wd/url --readable-timestamp add readable
 timestamps to log --enable-chrome-logs show logs from the browser (overrides
 other logging options) --disable-dev-shm-usage do not use /dev/shm (add this
 switch if seeing errors related to shared memory) --allowed-ips comma-separated
 allowlist of remote IP addresses which are allowed to connect to ChromeDriver
-```
+``` # Contributing Install the dependencies (Python >= 3.7) ``` python3 -m venv
+venv pip install -e . pip install -r test-requirements.txt ``` Fork this
+repository, make the changes into the forked repository and push a new Merge
+Request to 'main' branch. Open an issue in case of big MRs. # Testing To run
+the tests, start a new Driver as server on port `9999`, for example: ``` ./
+chromedriver --port=9999 ``` And execute the tests ``` python -m pytest ```
```

