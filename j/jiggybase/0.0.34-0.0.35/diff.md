# Comparing `tmp/jiggybase-0.0.34.tar.gz` & `tmp/jiggybase-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.34.tar", last modified: Sat May 20 00:43:09 2023, max compression
+gzip compressed data, was "jiggybase-0.0.35.tar", last modified: Thu May 25 02:08:18 2023, max compression
```

## Comparing `jiggybase-0.0.34.tar` & `jiggybase-0.0.35.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.325658 jiggybase-0.0.34/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.34/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-20 00:43:09.325201 jiggybase-0.0.34/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.34/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.316613 jiggybase-0.0.34/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.34/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.34/jiggybase/chat_stream.py
--rw-r--r--   0 wsk        (501) staff       (20)     2317 2023-05-16 01:07:05.000000 jiggybase-0.0.34/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)    11142 2023-05-19 02:24:06.000000 jiggybase-0.0.34/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.319562 jiggybase-0.0.34/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.34/jiggybase/examples/chat_completion.py
--rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-15 15:35:06.000000 jiggybase-0.0.34/jiggybase/examples/chat_completion_stream.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.34/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.34/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     5705 2023-05-15 15:27:23.000000 jiggybase-0.0.34/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.34/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.324322 jiggybase-0.0.34/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.34/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.34/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2767 2023-05-15 16:07:13.000000 jiggybase-0.0.34/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.34/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.34/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.34/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.34/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.34/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.34/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3206 2023-05-20 00:39:05.000000 jiggybase-0.0.34/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.34/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.34/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.34/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.34/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.34/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.318302 jiggybase-0.0.34/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      960 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-20 00:39:32.000000 jiggybase-0.0.34/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-20 00:43:09.325782 jiggybase-0.0.34/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.324625 jiggybase-0.0.34/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.34/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.427770 jiggybase-0.0.35/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.35/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-25 02:08:18.427331 jiggybase-0.0.35/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.35/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.417723 jiggybase-0.0.35/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.35/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.35/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4078 2023-05-25 02:03:37.000000 jiggybase-0.0.35/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)    11142 2023-05-25 02:00:12.000000 jiggybase-0.0.35/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.420574 jiggybase-0.0.35/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.35/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-25 02:00:08.000000 jiggybase-0.0.35/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.35/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.35/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)      449 2023-05-21 02:08:21.000000 jiggybase-0.0.35/jiggybase/ipython.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.0.35/jiggybase/jiggybase_ipython.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5681 2023-05-25 01:30:49.000000 jiggybase-0.0.35/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.35/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.425932 jiggybase-0.0.35/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.35/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.35/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.0.35/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.35/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.35/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.35/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.35/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.35/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.35/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3206 2023-05-20 00:39:05.000000 jiggybase-0.0.35/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.35/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.35/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.35/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.35/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.35/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.419414 jiggybase-0.0.35/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     1050 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-25 02:06:37.000000 jiggybase-0.0.35/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-25 02:08:18.427891 jiggybase-0.0.35/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.426801 jiggybase-0.0.35/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.35/test/test.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.0.35/test/test_extract_typed_completion.py
```

### Comparing `jiggybase-0.0.34/LICENSE` & `jiggybase-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/PKG-INFO` & `jiggybase-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.34
+Version: 0.0.35
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.34/README.md` & `jiggybase-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/chat_stream.py` & `jiggybase-0.0.35/jiggybase/chat_stream.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/collection.py` & `jiggybase-0.0.35/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/examples/chat_completion.py` & `jiggybase-0.0.35/jiggybase/examples/chat_completion.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.35/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.35/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/jiggybase_session.py` & `jiggybase-0.0.35/jiggybase/jiggybase_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,39 +28,38 @@
 class ServerError(Exception):
     """
     API returned 5xx Server error
     """
 
     
 class JiggyBaseSession(requests.Session):
-    def __init__(self, host=JIGGYBASE_HOST, api='gpt-gateway-v1',  *args, **kwargs):
+    def __init__(self, host=JIGGYBASE_HOST, api='gpt-gateway-v1', bearer_token=None, *args, **kwargs):
         """
         Extend requests.Session with common GPTG authentication, retry, and exceptions.
 
         host: The url host prefix of the form "https:/api.gpt-gateway.com"
               if host arg is not set, will use 
                     JIGGYBASE_HOST environment variable or "api.gpt-gateway.com" as final default.
 
         api:  The api & version to use. defaults to 'gpt-gateway-v1'
-                
+
+        bearer_token:  usually None, but can be specified if this is used by an endpoint has already has one handy
+        
         final url prefix are of the form "https://{host}/{api}"
         """
         super(JiggyBaseSession, self).__init__(*args, **kwargs)
         if not host.startswith('http'):
             host = f"https://{host}" if not host.startswith('localhost') else f'http://{host}'
         self.host = host
         if api:
             self.prefix_url = f"{host}/{api}"
         else:
-            self.prefix_url = host            
-        test_url = f"{self.prefix_url}/docs"
-        if requests.head(test_url).status_code != 200:
-            raise Exception(f"Invalid or unreachable api: {self.prefix_url}")
+            self.prefix_url = host          
             
-        self.bearer_token = None
+        self.bearer_token = bearer_token
         super(JiggyBaseSession, self).mount('https://',
                                             HTTPAdapter(max_retries=Retry(connect=5,
                                                                           read=5,
                                                                           status=5,
                                                                           redirect=2,
                                                                           backoff_factor=.001,
                                                                           status_forcelist=None)))
@@ -79,15 +78,15 @@
             raise ServerError(resp.content)
 
     def _auth(self):
         if 'JIGGYBASE_API_KEY' in os.environ:
             self._getjwt(os.environ['JIGGYBASE_API_KEY'])
         elif os.path.exists(JB_KEY_FILE):
             self._getjwt(open(JB_KEY_FILE).read())
-        else:
+        else: ## check interactive?
             while True:
                 window_open("https://jiggy.ai/authorize")
                 key_input = input("Enter your JiggyBase API Key: ")
                 if key_input[:4] == "jgy-":
                     # try using the key to see if it is valid
                     try:
                         self._getjwt(key_input)
```

### Comparing `jiggybase-0.0.34/jiggybase/login.py` & `jiggybase-0.0.35/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/auth.py` & `jiggybase-0.0.35/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/chat.py` & `jiggybase-0.0.35/jiggybase/models/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     model: str
     messages: list[Message]
     max_tokens: Optional[int] = None
     temperature: float
     stream: bool
 
 
+class TypedCompletionRequest(CompletionRequest):
+    json_schema : str
 
 
 class Choice(BaseModel):
     finish_reason: str
     index: int
     message: Message
 
@@ -69,10 +71,11 @@
     model:           str           = Field(description="The name of the model used to generate the completion")
     user_message:    str           = Field(description="The user's input message")
     input_tokens:    int           = Field(description="The number of input tokens sent to the model")
     output_tokens:   int           = Field(description="The number of output tokens generated by the model")
     messages_json:   Optional[str] = Field(description="JSON representation of the input messages sent to model endpoint")    
     completion:      Optional[str] = Field(description="The completion text returned by the model")
     created_at:      float         = Field(description="The epoch timestamp associated with the completion.")
+    endpoint:        str           = Field(description="The JiggyBase endpoint that requested the model completion")
     
     def __str__(self):
         return self.completion
```

### Comparing `jiggybase-0.0.34/jiggybase/models/chunk.py` & `jiggybase-0.0.35/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/collection.py` & `jiggybase-0.0.35/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/metadata.py` & `jiggybase-0.0.35/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/org.py` & `jiggybase-0.0.35/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/plugin.py` & `jiggybase-0.0.35/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/plugin_config.py` & `jiggybase-0.0.35/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/prompt.py` & `jiggybase-0.0.35/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/providers.py` & `jiggybase-0.0.35/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/models/user.py` & `jiggybase-0.0.35/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase/org.py` & `jiggybase-0.0.35/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.34/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.35/jiggybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.34
+Version: 0.0.35
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.34/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.35/jiggybase.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 jiggybase/__init__.py
 jiggybase/chat_stream.py
 jiggybase/client.py
 jiggybase/collection.py
+jiggybase/ipython.py
+jiggybase/jiggybase_ipython.py
 jiggybase/jiggybase_session.py
 jiggybase/login.py
 jiggybase/org.py
 jiggybase.egg-info/PKG-INFO
 jiggybase.egg-info/SOURCES.txt
 jiggybase.egg-info/dependency_links.txt
 jiggybase.egg-info/entry_points.txt
@@ -28,8 +30,9 @@
 jiggybase/models/metadata.py
 jiggybase/models/org.py
 jiggybase/models/plugin.py
 jiggybase/models/plugin_config.py
 jiggybase/models/prompt.py
 jiggybase/models/providers.py
 jiggybase/models/user.py
-test/test.py
+test/test.py
+test/test_extract_typed_completion.py
```

### Comparing `jiggybase-0.0.34/pyproject.toml` & `jiggybase-0.0.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.34"
+version = "0.0.35"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.34/test/test.py` & `jiggybase-0.0.35/test/test.py`

 * *Files identical despite different names*

