# Comparing `tmp/tap_rest_api_msdk-1.1.2.tar.gz` & `tmp/tap_rest_api_msdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_rest_api_msdk-1.1.2.tar", max compression
+gzip compressed data, was "tap_rest_api_msdk-1.2.0.tar", max compression
```

## Comparing `tap_rest_api_msdk-1.1.2.tar` & `tap_rest_api_msdk-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-18 16:18:59.062102 tap_rest_api_msdk-1.1.2/LICENSE
--rw-r--r--   0        0        0     8564 2023-05-18 16:18:59.062102 tap_rest_api_msdk-1.1.2/README.md
--rw-r--r--   0        0        0     1209 2023-05-18 16:18:59.066102 tap_rest_api_msdk-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-18 16:18:59.066102 tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/__init__.py
--rw-r--r--   0        0        0      506 2023-05-18 16:18:59.066102 tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/client.py
--rw-r--r--   0        0        0     7676 2023-05-18 16:18:59.066102 tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/streams.py
--rw-r--r--   0        0        0    10608 2023-05-18 16:18:59.066102 tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/tap.py
--rw-r--r--   0        0        0     1969 2023-05-18 16:18:59.066102 tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/utils.py
--rw-r--r--   0        0        0     9760 1970-01-01 00:00:00.000000 tap_rest_api_msdk-1.1.2/setup.py
--rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 tap_rest_api_msdk-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8564 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/README.md
+-rw-r--r--   0        0        0     1209 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/__init__.py
+-rw-r--r--   0        0        0      506 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/client.py
+-rw-r--r--   0        0        0     7756 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/streams.py
+-rw-r--r--   0        0        0    10608 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/tap.py
+-rw-r--r--   0        0        0     1989 2023-05-25 20:33:40.700172 tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/utils.py
+-rw-r--r--   0        0        0     9760 1970-01-01 00:00:00.000000 tap_rest_api_msdk-1.2.0/setup.py
+-rw-r--r--   0        0        0     9489 1970-01-01 00:00:00.000000 tap_rest_api_msdk-1.2.0/PKG-INFO
```

### Comparing `tap_rest_api_msdk-1.1.2/LICENSE` & `tap_rest_api_msdk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_rest_api_msdk-1.1.2/README.md` & `tap_rest_api_msdk-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_rest_api_msdk-1.1.2/pyproject.toml` & `tap_rest_api_msdk-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-rest-api-msdk"
-version = "1.1.2"
+version = "1.2.0"
 description = "`tap-rest-api-msdk` is a Singer tap for REST APIs, built with the Meltano SDK for Singer Taps."
 authors = ["Josh Lloyd", "Fred Reimer"]
 keywords = [
     "ELT",
     "rest-api-msdk",
     "Meltano",
     "Singer",
@@ -14,30 +14,30 @@
 ]
 license = "Apache 2.0"
 homepage = "https://github.com/Widen/tap-rest-api-msdk"
 repository = "https://github.com/Widen/tap-rest-api-msdk"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "<3.10,>=3.7.1"
+python = "<3.12,>=3.7.1"
 requests = "^2.25.1"
 singer-sdk = "^0.26.0"
 genson = "^1.2.2"
 atomicwrites = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 tox = "^3.24.4"
 flake8 = "^3.9.2"
-black = "^21.9b0"
+black = "^23.3.0"
 pydocstyle = "^6.1.1"
-mypy = "^0.910"
+mypy = "^1.3.0"
 types-requests = "^2.25.8"
 requests-mock = "^1.9.3"
-isort = "^5.10.1"
+isort = "^5.11.5"
 
 [tool.black]
 exclude = ".*simpleeval.*"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
```

### Comparing `tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/streams.py` & `tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/streams.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
     def __init__(
         self,
         tap: Any,
         name: str,
         records_path: str,
         path: str,
-        params: dict = None,
-        headers: dict = None,
-        primary_keys: list = None,
-        replication_key: str = None,
-        except_keys: list = None,
-        next_page_token_path: str = None,
-        schema: dict = None,
+        params: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        primary_keys: Optional[list] = None,
+        replication_key: Optional[str] = None,
+        except_keys: Optional[list] = None,
+        next_page_token_path: Optional[str] = None,
+        schema: Optional[dict] = None,
         pagination_request_style: str = "default",
         pagination_response_style: str = "default",
-        pagination_page_size: int = None,
+        pagination_page_size: Optional[int] = None,
     ) -> None:
         """Class initialization.
 
         Args:
             tap: see tap.py
             name: see tap.py
             path: see tap.py
```

### Comparing `tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/tap.py` & `tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/tap.py`

 * *Files identical despite different names*

### Comparing `tap_rest_api_msdk-1.1.2/tap_rest_api_msdk/utils.py` & `tap_rest_api_msdk-1.2.0/tap_rest_api_msdk/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Basic utility functions."""
 
 import json
-from typing import Any
+from typing import Any, Optional
 
 
-def flatten_json(obj: dict, except_keys: list = None) -> dict:
+def flatten_json(obj: dict, except_keys: Optional[list] = None) -> dict:
     """Flattens a json object by appending the patch as a key in the returned object.
 
     Automatically converts arrays and any provided keys into json strings to prevent
     flattening further into those branches.
 
     Args:
         obj: the json object to be flattened.
```

### Comparing `tap_rest_api_msdk-1.1.2/setup.py` & `tap_rest_api_msdk-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 entry_points = \
 {'console_scripts': ['tap-rest-api-msdk = '
                      'tap_rest_api_msdk.tap:TapRestApiMsdk.cli']}
 
 setup_kwargs = {
     'name': 'tap-rest-api-msdk',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': '`tap-rest-api-msdk` is a Singer tap for REST APIs, built with the Meltano SDK for Singer Taps.',
     'long_description': '# tap-rest-api-msdk\n\n`tap-rest-api-msdk` is a Singer tap for generic rest-apis. The novelty of this particular tap\nis that it will auto-discover the stream\'s schema.\n\nThis is particularly useful if you have a stream with a very large and complex schema or\na stream that outputs records with varying schemas for each record. Can also be used for\nsimpler more reliable streams.\n\nPlease note that authentication capabilities have not yet been developed for this tap,\nunless you are able to pass the authentication through the header.\nIf you are interested in contributing this, please fork and make a pull request.\n\nBuilt with the Meltano [SDK](https://gitlab.com/meltano/sdk) for Singer Taps.\n\nGratitude goes to [anelendata](https://github.com/anelendata/tap-rest-api) for inspiring this "SDK-ized" version of their tap.\n\n## Installation\nIf using via Meltano, add the following lines to your `meltano.yml` file and run the following command:\n\n```yaml\nplugins:\n  extractors:\n    - name: tap-rest-api-msdk\n      namespace: tap_rest_api_msdk\n      pip_url: tap-rest-api-msdk\n      executable: tap-rest-api-msdk\n      capabilities:\n        - state\n        - catalog\n        - discover\n      settings:\n        - name: api_url\n        - name: name\n        - name: path\n        - name: params\n        - name: headers\n        - name: records_path\n        - name: next_page_token_path\n        - name: pagination_request_style\n        - name: pagination_response_style\n        - name: pagination_page_size\n        - name: primary_keys\n        - name: replication_key\n        - name: except_keys\n        - name: num_inference_records\n        - name: pagination_request_style\n        - name: pagination_response_style\n        - name: pagination_page_size\n        - name: next_page_token_path\n```\n\n```bash\nmeltano install extractor tap-rest-api-msdk\n```\n\n## Configuration\n\n### Accepted Config Options\n\n\nA full list of supported settings and capabilities for this\ntap is available by running:\n\n```bash\ntap-rest-api-msdk --about\n```\n\n#### Top-level config options. \nParameters that appear at the stream-level will overwrite their top-level \ncounterparts except where noted in the stream-level params. Otherwise, the values\nprovided at the top-level will be the default values for each stream.:\n- `api_url`: required: the base url/endpoint for the desired api.\n- `pagination_request_style`: optional: style for requesting pagination, defaults to `default`, see Pagination below.\n- `pagination_response_style`: optional: style of pagination results, defaults to `default`, see Pagination below.\n- `pagination_page_size`: optional: limit for size of page, defaults to None.\n- `next_page_token_path`: optional: a jsonpath string representing the path to the "next page" token. Defaults to `$.next_page`.\n- `streams`: required: a list of objects that contain the configuration of each stream. See stream-level params below.\n- `path`: optional: see stream-level params below.\n- `params`: optional: see stream-level params below.\n- `headers`: optional: see stream-level params below.\n- `records_path`: optional: see stream-level params below.\n- `primary_keys`: optional: see stream-level params below.\n- `replication_key`: optional: see stream-level params below.\n- `except_keys`: optional: see stream-level params below.\n- `num_inference_keys`: optional:  see stream-level params below.\n\n#### Stream level config options. \nParameters that appear at the stream-level\nwill overwrite their top-level counterparts except where noted below:\n- `name`: required: name of the stream.\n- `path`: optional: the path appended to the `api_url`.\n- `params`: optional: an object of objects that provide the `params` in a `requests.get` method.\n  Stream level params will be merged with top-level params with stream level params overwriting \n  top-level params with the same key.\n- `headers`: optional: an object of headers to pass into the api calls. Stream level\n  headers will be merged with top-level params with stream level params overwriting \n  top-level params with the same key\n- `records_path`: optional: a jsonpath string representing the path in the requests response that contains the records to process. Defaults to `$[*]`.\n- `primary_keys`: required: a list of the json keys of the primary key for the stream.\n- `replication_key`: optional: the json key of the replication key. Note that this should be an incrementing integer or datetime object.\n- `except_keys`: This tap automatically flattens the entire json structure and builds keys based on the corresponding paths.\n  Keys, whether composite or otherwise, listed in this dictionary will not be recursively flattened, but instead their values will be\n  turned into a json string and processed in that format. This is also automatically done for any lists within the records; therefore,\n  records are not duplicated for each item in lists.\n- `num_inference_keys`: optional: number of records used to infer the stream\'s schema. Defaults to 50.\n- `scheam`: optional: A valid Singer schema or a path-like string that provides\n  the path to a `.json` file that contains a valid Singer schema. If provided, \n  the schema will not be inferred from the results of an api call.\n\n## Pagination\nPagination is a complex topic as there is no real single standard, and many different implementations.  Unless options are provided, both the request and results stype default to the `default`, which is the pagination style originally implemented.\n\n### Default Request Style\nThe default request style for pagination is described below:\n- Use next_page_token_path if provided to extract the token from response if found; otherwise\n- use X-Next-Page header from response\n\n### Default Response Style\nThe default response style for pagination is described below:\n- If there is a token, add that as a `page` URL parameter.\n\n### Additional Request Styles\nThere are additional request styles supported as follows.\n- `style1` - This style uses URL parameters named offset and limit\n  - `offset` is calculated from the previous response, or not set if there is no previous response\n  - `limit` is set to the `pagination_page_size` value, if specified, or not set\n\n### Additional Response Styles\nThere are additional response styles supported as follows.\n- `style1` - This style retrieves pagination information from the `pagination` top-level element in the response.  Expected format is as follows:\n    ```json\n    "pagination": {\n        "total": 136,\n        "limit": 2,\n        "offset": 2\n    }\n    ```\n  The next page token, which in this case is really the next starting record number, is calculated by the limit, current offset, or None is returned to indicate no more data.  For this style, the response style _must_ include the limit in the response, even if none is specified in the request, as well as total and offset to calculate the next token value.\n\n## Usage\n\nYou can easily run `tap-rest-api-msdk` by itself or in a pipeline using [Meltano](www.meltano.com).\n\n### Executing the Tap Directly\n\n```bash\ntap-rest-api-msdk --version\ntap-rest-api-msdk --help\ntap-rest-api-msdk --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tests/` directory and\nthen run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-rest-api-msdk` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-rest-api-msdk --help\n```\n\n### Continuous Integration\nRun through the full suite of tests and linters by running\n\n```bash\npoetry run tox -e py\n```\n\nThese must pass in order for PR\'s to be merged.\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nThis project comes with an example `meltano.yml` project file already created.\n\nNext, install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-rest-api-msdk\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-rest-api-msdk --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-rest-api-msdk target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n',
     'author': 'Josh Lloyd',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Widen/tap-rest-api-msdk',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.10',
+    'python_requires': '>=3.7.1,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tap_rest_api_msdk-1.1.2/PKG-INFO` & `tap_rest_api_msdk-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: tap-rest-api-msdk
-Version: 1.1.2
+Version: 1.2.0
 Summary: `tap-rest-api-msdk` is a Singer tap for REST APIs, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/Widen/tap-rest-api-msdk
 License: Apache 2.0
 Keywords: ELT,rest-api-msdk,Meltano,Singer,REST,API,tap
 Author: Josh Lloyd
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atomicwrites (>=1.4.0,<2.0.0)
 Requires-Dist: genson (>=1.2.2,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: singer-sdk (>=0.26.0,<0.27.0)
 Project-URL: Repository, https://github.com/Widen/tap-rest-api-msdk
 Description-Content-Type: text/markdown
```

