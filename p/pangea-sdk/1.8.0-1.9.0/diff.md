# Comparing `tmp/pangea_sdk-1.8.0.tar.gz` & `tmp/pangea_sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_sdk-1.8.0.tar", max compression
+gzip compressed data, was "pangea_sdk-1.9.0.tar", max compression
```

## Comparing `pangea_sdk-1.8.0.tar` & `pangea_sdk-1.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     7767 2023-03-20 14:36:50.582052 pangea_sdk-1.8.0/README.md
--rw-r--r--   0        0        0      146 2023-04-21 21:23:31.675163 pangea_sdk-1.8.0/pangea/__init__.py
--rw-r--r--   0        0        0     3778 2023-03-14 20:29:54.979893 pangea_sdk-1.8.0/pangea/audit_logger.py
--rw-r--r--   0        0        0     1055 2023-03-30 18:28:00.245753 pangea_sdk-1.8.0/pangea/config.py
--rw-r--r--   0        0        0     8741 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/deep_verify.py
--rw-r--r--   0        0        0      604 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/deprecated.py
--rw-r--r--   0        0        0     6511 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/dump_audit.py
--rw-r--r--   0        0        0     4458 2023-04-10 12:19:13.490833 pangea_sdk-1.8.0/pangea/exceptions.py
--rw-r--r--   0        0        0     9874 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/request.py
--rw-r--r--   0        0        0     3891 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/response.py
--rw-r--r--   0        0        0      221 2023-04-18 15:23:55.985948 pangea_sdk-1.8.0/pangea/services/__init__.py
--rw-r--r--   0        0        0    24321 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/audit.py
--rw-r--r--   0        0        0      451 2023-03-14 20:29:54.979893 pangea_sdk-1.8.0/pangea/services/audit/exceptions.py
--rw-r--r--   0        0        0    12093 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/models.py
--rw-r--r--   0        0        0     5635 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/signing.py
--rw-r--r--   0        0        0     8533 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/util.py
--rw-r--r--   0        0        0    37620 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/authn/authn.py
--rw-r--r--   0        0        0    16741 2023-04-19 18:36:20.317300 pangea_sdk-1.8.0/pangea/services/authn/models.py
--rw-r--r--   0        0        0     1037 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/base.py
--rw-r--r--   0        0        0     5565 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/embargo.py
--rw-r--r--   0        0        0    33733 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/intel.py
--rw-r--r--   0        0        0     7253 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/redact.py
--rw-r--r--   0        0        0     1450 2023-03-14 20:29:54.983893 pangea_sdk-1.8.0/pangea/services/vault/models/asymmetric.py
--rw-r--r--   0        0        0     7847 2023-04-12 15:07:35.002848 pangea_sdk-1.8.0/pangea/services/vault/models/common.py
--rw-r--r--   0        0        0      481 2023-03-14 20:29:54.983893 pangea_sdk-1.8.0/pangea/services/vault/models/secret.py
--rw-r--r--   0        0        0     1260 2023-04-12 15:07:35.002848 pangea_sdk-1.8.0/pangea/services/vault/models/symmetric.py
--rw-r--r--   0        0        0    43335 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/vault/vault.py
--rw-r--r--   0        0        0     5472 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/tools.py
--rw-r--r--   0        0        0      554 2023-04-18 15:23:55.985948 pangea_sdk-1.8.0/pangea/utils.py
--rw-r--r--   0        0        0    10606 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/verify_audit.py
--rw-r--r--   0        0        0      840 2023-04-21 21:23:31.675163 pangea_sdk-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7767 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/README.md
+-rw-r--r--   0        0        0      146 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/__init__.py
+-rw-r--r--   0        0        0     3778 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/audit_logger.py
+-rw-r--r--   0        0        0     1059 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/config.py
+-rw-r--r--   0        0        0     8741 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/deep_verify.py
+-rw-r--r--   0        0        0      604 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/deprecated.py
+-rw-r--r--   0        0        0     6511 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/dump_audit.py
+-rw-r--r--   0        0        0     4458 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/exceptions.py
+-rw-r--r--   0        0        0    10052 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/request.py
+-rw-r--r--   0        0        0     3891 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/response.py
+-rw-r--r--   0        0        0      221 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/services/__init__.py
+-rw-r--r--   0        0        0    24530 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/audit.py
+-rw-r--r--   0        0        0      451 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/services/audit/exceptions.py
+-rw-r--r--   0        0        0    12093 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/models.py
+-rw-r--r--   0        0        0     5281 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/signing.py
+-rw-r--r--   0        0        0     7807 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/util.py
+-rw-r--r--   0        0        0    37055 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/authn/authn.py
+-rw-r--r--   0        0        0    16758 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/services/authn/models.py
+-rw-r--r--   0        0        0      956 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/base.py
+-rw-r--r--   0        0        0     4034 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/embargo.py
+-rw-r--r--   0        0        0    34640 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/intel.py
+-rw-r--r--   0        0        0     7440 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/redact.py
+-rw-r--r--   0        0        0     1450 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/services/vault/models/asymmetric.py
+-rw-r--r--   0        0        0     8463 2023-04-28 18:21:39.489966 pangea_sdk-1.9.0/pangea/services/vault/models/common.py
+-rw-r--r--   0        0        0      481 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/services/vault/models/secret.py
+-rw-r--r--   0        0        0     1330 2023-04-28 18:21:39.489966 pangea_sdk-1.9.0/pangea/services/vault/models/symmetric.py
+-rw-r--r--   0        0        0    44423 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/vault/vault.py
+-rw-r--r--   0        0        0     5472 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/tools.py
+-rw-r--r--   0        0        0      554 2023-05-23 13:45:34.331889 pangea_sdk-1.9.0/pangea/utils.py
+-rw-r--r--   0        0        0    10616 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/verify_audit.py
+-rw-r--r--   0        0        0      840 2023-05-25 20:04:02.236288 pangea_sdk-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.9.0/PKG-INFO
```

### Comparing `pangea_sdk-1.8.0/README.md` & `pangea_sdk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/audit_logger.py` & `pangea_sdk-1.9.0/pangea/audit_logger.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/config.py` & `pangea_sdk-1.9.0/pangea/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     request_retries: int = 3
 
     """'
     Backoff strategy passed to 'requests'
 
     """
-    request_backoff: int = 1
+    request_backoff: float = 0.5
 
     """
     Timeout used on initial request attempts
 
     """
     request_timeout: int = 5
```

### Comparing `pangea_sdk-1.8.0/pangea/deep_verify.py` & `pangea_sdk-1.9.0/pangea/deep_verify.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/deprecated.py` & `pangea_sdk-1.9.0/pangea/deprecated.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/dump_audit.py` & `pangea_sdk-1.9.0/pangea/dump_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/exceptions.py` & `pangea_sdk-1.9.0/pangea/exceptions.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/request.py` & `pangea_sdk-1.9.0/pangea/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 
     Wraps Get/Post calls to support both API requests. If `queued_retry_enabled`
     is enabled, the progress of long running Post requests will queried until
     completion or until the `queued_retries` limit is reached. Both values can
     be set in PangeaConfig.
     """
 
-    def __init__(self, config: PangeaConfig, token: str, version: str, service: str, logger: logging.Logger):
+    def __init__(self, config: PangeaConfig, token: str, service: str, logger: logging.Logger):
         self.config = copy.deepcopy(config)
         self.token = token
-        self.version = version
         self.service = service
 
         # Queued request retry support flag
         self._queued_retry_enabled = config.queued_retry_enabled
 
         # Custom headers
         self._extra_headers = {}
@@ -162,31 +161,37 @@
             else:
                 return pangea_response
 
     def _init_session(self) -> requests.Session:
         retry_config = Retry(
             total=self.config.request_retries,
             backoff_factor=self.config.request_backoff,
+            status_forcelist=[500, 502, 503, 504],
         )
 
         adapter = HTTPAdapter(max_retries=retry_config)
         session = requests.Session()
 
         if self.config.insecure:
             session.mount("http://", adapter)
         else:
             session.mount("https://", adapter)
 
         return session
 
     def _url(self, path: str) -> str:
-        protocol = "http://" if self.config.insecure else "https://"
-        domain = self.config.domain if self.config.environment == "local" else f"{self.service}.{self.config.domain}"
-
-        url = f"{protocol}{domain}/{ str(self.version) + '/' if self.version else '' }{path}"
+        if self.config.domain.startswith("http://") or self.config.domain.startswith("https://"):
+            # it's URL
+            url = f"{self.config.domain}/{path}"
+        else:
+            schema = "http://" if self.config.insecure else "https://"
+            domain = (
+                self.config.domain if self.config.environment == "local" else f"{self.service}.{self.config.domain}"
+            )
+            url = f"{schema}{domain}/{path}"
         return url
 
     def _headers(self) -> dict:
         headers = {
             "Content-Type": "application/json",
             "User-Agent": self._user_agent,
             "Authorization": f"Bearer {self.token}",
```

### Comparing `pangea_sdk-1.8.0/pangea/response.py` & `pangea_sdk-1.9.0/pangea/response.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/services/audit/audit.py` & `pangea_sdk-1.9.0/pangea/services/audit/audit.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         audit_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Audit service
         audit = Audit(token=PANGEA_TOKEN, config=audit_config)
     """
 
     service_name: str = "audit"
-    version: str = "v1"
 
     def __init__(
         self,
         token,
         config=None,
         private_key_file: str = "",
         public_key_info: Dict[str, str] = {},
@@ -104,14 +103,17 @@
         signing: EventSigning = EventSigning.NONE,
         verbose: Optional[bool] = None,
     ) -> PangeaResponse[LogResult]:
         """
         Log an entry
 
         Create a log entry in the Secure Audit Log.
+
+        OperationId: audit_post_v1_log
+
         Args:
             message (str, dict): A message describing a detailed account of what happened.
             actor (str, optional): Record who performed the auditable activity.
             action (str, optional): The auditable action that occurred.
             new (str, dict, optional): The value of a record after it was changed.
             old (str, dict, optional): The value of a record before it was changed.
             source (str, optional): Used to record the location from where an activity occurred.
@@ -125,28 +127,27 @@
         Raises:
             AuditException: If an audit based api exception happens
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the hash of event data and optional verbose
                 results are returned in the response.result field.
-                Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/audit#log-an-entry).
+                Available response fields can be found in our
+                [API documentation](https://pangea.cloud/docs/api/audit#log-an-entry).
 
         Examples:
             try:
                 log_response = audit.log(message="Hello world", verbose=False)
                 print(f"Response. Hash: {log_response.result.hash}")
             except pe.PangeaAPIException as e:
                 print(f"Request Error: {e.response.summary}")
                 for err in e.errors:
                     print(f"\\t{err.detail} \\n")
         """
 
-        endpoint_name = "log"
-
         event = Event(
             message=message,
             actor=actor,
             action=action,
             new=new,
             old=old,
             source=source,
@@ -159,29 +160,29 @@
         if signing == EventSigning.LOCAL and self.signer is None:
             raise AuditException("Error: the `signing` parameter set, but `signer` is not configured")
 
         input = LogRequest(event=event.get_stringified_copy(), verbose=verbose)
 
         if signing == EventSigning.LOCAL:
             data2sign = canonicalize_event(event)
-            signature = self.signer.signMessage(data2sign)
+            signature = self.signer.sign(data2sign)
             if signature is not None:
                 input.signature = signature
             else:
                 raise AuditException("Error: failure signing message")
 
             # Add public key value to public key info and serialize
             self.set_public_key(input, self.signer, self.public_key_info)
 
         if verify:
             input.verbose = True
             if self.prev_unpublished_root_hash:
                 input.prev_root = self.prev_unpublished_root_hash
 
-        response = self.request.post(endpoint_name, data=input.dict(exclude_none=True))
+        response = self.request.post("v1/log", data=input.dict(exclude_none=True))
         return self.handle_log_response(response, verify=verify)
 
     def handle_log_response(self, response: PangeaResponse, verify: bool) -> PangeaResponse[LogResult]:
         if not response.success:
             return response
 
         response.result = LogResult(**response.raw_result)
@@ -237,18 +238,20 @@
         max_results: Optional[int] = None,
         search_restriction: Optional[dict] = None,
         verbose: Optional[bool] = None,
         verify_consistency: bool = False,
         verify_events: bool = True,
     ) -> PangeaResponse[SearchOutput]:
         """
-        Search for events
+        Search the log
 
         Search for events that match the provided search criteria.
 
+        OperationId: audit_post_v1_search
+
         Args:
             query (str): Natural search string; list of keywords with optional
                 `<option>:<value>` qualifiers. The following optional qualifiers are supported:
                     - action
                     - actor
                     - message
                     - new
@@ -276,16 +279,14 @@
                 response.result field. Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/audit#search-for-events).
                 Pagination can be found in the [search results endpoint](https://pangea.cloud/docs/api/audit#search-results).
 
         Examples:
             response: PangeaResponse[SearchOutput] = audit.search(query="message:test", search_restriction={'source': ["monitor"]}, limit=1, verify_consistency=True, verify_events=True)
         """
 
-        endpoint_name = "search"
-
         if verify_consistency:
             verbose = True
 
         input = SearchRequest(
             query=query,
             order=order,
             order_by=order_by,
@@ -293,60 +294,68 @@
             end=format_datetime(end) if isinstance(end, datetime.datetime) else end,
             limit=limit,
             max_results=max_results,
             search_restriction=search_restriction,
             verbose=verbose,
         )
 
-        response = self.request.post(endpoint_name, data=input.dict(exclude_none=True))
+        response = self.request.post("v1/search", data=input.dict(exclude_none=True))
         return self.handle_search_response(response, verify_consistency, verify_events)
 
     def results(
         self,
         id: str,
         limit: Optional[int] = 20,
         offset: Optional[int] = 0,
         verify_consistency: bool = False,
         verify_events: bool = True,
     ) -> PangeaResponse[SearchResultOutput]:
         """
-        Results of a Search
+        Results of a search
 
-        Returns paginated results of a previous Search
+        Fetch paginated results of a previously executed search.
+
+        OperationId: audit_post_v1_results
 
         Args:
             id (string): the id of a search action, found in `response.result.id`
             limit (integer, optional): the maximum number of results to return, default is 20
             offset (integer, optional): the position of the first result to return, default is 0
             verify_consistency (bool): True to verify logs consistency
             verify_events (bool): True to verify hash events and signatures
         Raises:
             AuditException: If an audit based api exception happens
             PangeaAPIException: If an API Error happens
 
-        Example:
-
-            search_res: PangeaResponse[SearchOutput] = audit.search(query="message:test", search_restriction={'source': ["monitor"]}, limit=100, verify_consistency=True, verify_events=True)
-            result_res: PangeaResponse[SearchResultsOutput] = audit.results(id=search_res.result.id, limit=10, offset=0)
+        Examples:
+            search_res: PangeaResponse[SearchOutput] = audit.search(
+                query="message:test",
+                search_restriction={'source': ["monitor"]},
+                limit=100,
+                verify_consistency=True,
+                verify_events=True)
+
+            result_res: PangeaResponse[SearchResultsOutput] = audit.results(
+                id=search_res.result.id,
+                limit=10,
+                offset=0)
         """
 
-        endpoint_name = "results"
-
         if limit <= 0:
             raise AuditException("The 'limit' argument must be a positive integer > 0")
 
         if offset < 0:
             raise AuditException("The 'offset' argument must be a positive integer")
 
         input = SearchResultRequest(
             id=id,
             limit=limit,
             offset=offset,
         )
-        response = self.request.post(endpoint_name, data=input.dict(exclude_none=True))
+        response = self.request.post("v1/results", data=input.dict(exclude_none=True))
         return self.handle_results_response(response, verify_consistency, verify_events)
 
     def handle_results_response(
         self, response: PangeaResponse[SearchResultOutput], verify_consistency: bool = False, verify_events: bool = True
     ) -> PangeaResponse[SearchResultOutput]:
         if not response.success:
             return response
@@ -550,47 +559,49 @@
           EventVerification: PASS if success, FAIL if fail or NONE in case that there is not enough information to verify it
 
         """
         public_key = get_public_key(audit_envelope.public_key)
 
         if audit_envelope and audit_envelope.signature and public_key:
             v = Verifier()
-            verification = v.verifyMessage(
+            verification = v.verify_signature(
                 audit_envelope.signature, canonicalize_event(audit_envelope.event), public_key
             )
             if verification is not None:
                 return EventVerification.PASS if verification else EventVerification.FAIL
             else:
                 return EventVerification.NONE
         else:
             return EventVerification.NONE
 
     def set_public_key(self, input: LogRequest, signer: Signer, public_key_info: Dict[str, str]):
-        public_key_info["key"] = signer.getPublicKeyPEM()
+        public_key_info["key"] = signer.get_public_key_PEM()
+        public_key_info["algorithm"] = signer.get_algorithm()
         input.public_key = json.dumps(
             public_key_info, ensure_ascii=False, allow_nan=False, separators=(",", ":"), sort_keys=True
         )
 
     def root(self, tree_size: Optional[int] = None) -> PangeaResponse[RootResult]:
         """
-        Retrieve tamperproof verification
+        Tamperproof verification
 
         Returns current root hash and consistency proof.
 
+        OperationId: audit_post_v1_root
+
         Args:
-            tree_size (int, optional): The size of the tree (the number of records). If None endpoint will return last tree root.
+            tree_size (int, optional): The size of the tree (the number of records). If None, endpoint will return last tree root.
 
         Returns:
             PangeaResponse[RootOutput]
 
         Raises:
             AuditException: If an audit based api exception happens
             PangeaAPIException: If an API Error happens
 
         Examples:
             response = audit.root(tree_size=7)
         """
         input = RootRequest(tree_size=tree_size)
-        endpoint_name = "root"
-        response = self.request.post(endpoint_name, data=input.dict(exclude_none=True))
+        response = self.request.post("v1/root", data=input.dict(exclude_none=True))
         response.result = RootResult(**response.raw_result)
         return response
```

### Comparing `pangea_sdk-1.8.0/pangea/services/audit/models.py` & `pangea_sdk-1.9.0/pangea/services/audit/models.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/services/audit/signing.py` & `pangea_sdk-1.9.0/pangea/services/audit/signing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,164 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
+from abc import ABC, abstractmethod
 from base64 import b64decode, b64encode
-from typing import Dict, Optional, Union
+from typing import Optional
 
+from cryptography import exceptions
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519
-from cryptography.hazmat.primitives.asymmetric.types import PUBLIC_KEY_TYPES
-from pangea.services.audit.util import b64decode_ascii, canonicalize_json
+from cryptography.hazmat.primitives.asymmetric.types import PRIVATE_KEY_TYPES
+from pangea.exceptions import PangeaException
+from pangea.services.audit.util import b64decode_ascii
+from pangea.services.vault.models.common import AsymmetricAlgorithm
+
+
+class AlgorithmSigner(ABC):
+    def __init__(self, private_key):
+        self.private_key: PRIVATE_KEY_TYPES = private_key
+
+    @abstractmethod
+    def sign(self, message: bytes) -> str:
+        pass
+
+    @abstractmethod
+    def get_public_key_PEM(self) -> str:
+        pass
+
+    @abstractmethod
+    def get_algorithm(self) -> str:
+        pass
+
+
+class ED25519Signer(AlgorithmSigner):
+    def sign(self, message: bytes) -> str:
+        signature = self.private_key.sign(message)
+        return b64encode(signature).decode("ascii")
+
+    def get_public_key_PEM(self) -> str:
+        return (
+            self.private_key.public_key()
+            .public_bytes(encoding=serialization.Encoding.PEM, format=serialization.PublicFormat.SubjectPublicKeyInfo)
+            .decode("utf-8")
+        )
+
+    def get_algorithm(self) -> str:
+        return AsymmetricAlgorithm.Ed25519.value
+
+
+signers = {
+    ed25519.Ed25519PrivateKey: ED25519Signer,
+}
 
 
 class Signer:
-    def __init__(self, private_key_file: str) -> None:
-        self._private_key = None
-        self._private_key_filename = private_key_file
-
-    # Returns the private key
-    def _getPrivateKey(self) -> ed25519.Ed25519PrivateKey:
-        if self._private_key is None:
+    private_key_file: str
+    signer: Optional[AlgorithmSigner] = None
+
+    def __init__(self, private_key_file: str):
+        self.private_key_file = private_key_file
+
+    def sign(self, message: bytes) -> str:
+        self._load_signer()
+        return self.signer.sign(message=message)
+
+    def get_public_key_PEM(self) -> str:
+        self._load_signer()
+        return self.signer.get_public_key_PEM()
+
+    def get_algorithm(self) -> str:
+        self._load_signer()
+        return self.signer.get_algorithm()
+
+    def _load_signer(self):
+        if self.signer is not None:
+            return
+
+        if self.private_key_file:
             try:
-                with open(self._private_key_filename, "rb") as file:
+                with open(self.private_key_file, "rb") as file:
                     file_bytes = file.read()
             except FileNotFoundError:
-                raise Exception(f"Error: Failed opening private key file {self._private_key_filename}")
+                raise Exception(f"Error: Failed opening private key file {self.private_key_file}")
 
+            privkey = self._decode_private_key(file_bytes)
+            for cls, signer in signers.items():
+                if isinstance(privkey, cls):
+                    self.signer = signer(privkey)
+                    return
+
+            raise PangeaException(f"Private key is not supported: {type(privkey)}.")
+
+        raise PangeaException("Must pass a valid private key file name.")
+
+    def _decode_private_key(self, private_key: bytes):
+        """Parse a private key in PEM or ssh format"""
+
+        for func in (serialization.load_pem_private_key, serialization.load_ssh_private_key):
             try:
-                self._private_key = serialization.load_pem_private_key(file_bytes, None)
-            except Exception:
-                self._private_key = None
-                raise Exception("Error: Failed loading private key.")
-
-            if not isinstance(self._private_key, ed25519.Ed25519PrivateKey):
-                self._private_key = None
-                raise Exception("Private key is not using Ed25519 algorithm.")
+                return func(private_key, None)
+            except exceptions.UnsupportedAlgorithm as e:
+                raise e
+            except ValueError:
+                pass
 
-        return self._private_key
+        raise PangeaException("Unsupported key")
 
-    # Signs a message in bytes using Ed25519 algorithm
-    def _signMessageBytes(self, message_bytes: bytes, private_key: ed25519.Ed25519PrivateKey) -> str:
-        try:
-            signature = private_key.sign(message_bytes)
-            signature_b64 = b64encode(signature).decode("ascii")
-        except Exception:
-            return None
-
-        return signature_b64
-
-    # Signs a string message using Ed25519 algorithm
-    def _signMessageStr(self, message: str, private_key: ed25519.Ed25519PrivateKey) -> str:
-        message_bytes = bytes(message, "utf8")
-        return self._signMessageBytes(message_bytes, private_key)
-
-    # Signs a JSON message using Ed25519 algorithm
-    def _signMessageJSON(self, messageJSON: dict, private_key: ed25519.Ed25519PrivateKey) -> str:
-        message_bytes = canonicalize_json(messageJSON)
-        return self._signMessageBytes(message_bytes, private_key)
-
-    def signMessage(self, message: Union[str, Dict, bytes]) -> str:
-        private_key = self._getPrivateKey()
 
-        if isinstance(message, str):
-            return self._signMessageStr(message, private_key)
+class AlgorithmVerifier(ABC):
+    def __init__(self, public_key):
+        self.public_key = public_key
 
-        elif isinstance(message, dict):
-            return self._signMessageJSON(message, private_key)
+    @abstractmethod
+    def verify(self, message: bytes, signature: bytes) -> bool:
+        pass
 
-        elif isinstance(message, bytes):
-            return self._signMessageBytes(message, private_key)
-        else:
-            raise Exception("Error: Not supported instance")
 
-    def getPublicKeyBytes(self) -> bytes:
-        return (
-            self._getPrivateKey()
-            .public_key()
-            .public_bytes(encoding=serialization.Encoding.Raw, format=serialization.PublicFormat.Raw)
-        )
+class ED25519Verifier(AlgorithmVerifier):
+    def verify(self, message: bytes, signature: bytes) -> bool:
+        try:
+            self.public_key.verify(signature, message)
+            return True
+        except exceptions.InvalidSignature:
+            return False
 
-    def getPublicKeyPEM(self) -> str:
-        return (
-            self._getPrivateKey()
-            .public_key()
-            .public_bytes(encoding=serialization.Encoding.PEM, format=serialization.PublicFormat.SubjectPublicKeyInfo)
-            .decode("utf-8")
-        )
+
+verifiers = {
+    ed25519.Ed25519PublicKey: ED25519Verifier,
+}
 
 
 class Verifier:
     # verify message with signature and public key bytes
-    def verifyMessage(
-        self, signature_b64: str, message: Union[str, dict, bytes], public_key_input: str = None
+    def verify_signature(
+        self, signature_b64: str, message_bytes: bytes, public_key_input: str = None
     ) -> Optional[bool]:
-        if self._is_pem_format(public_key_input):
-            public_key = serialization.load_pem_public_key(bytes(public_key_input, "utf-8"))
-            if not isinstance(public_key, ed25519.Ed25519PublicKey):
-                # TODO: Add support for other public key formats
-                return None
+        if self._has_header(public_key_input):
+            pubkey = self._decode_public_key(bytes(public_key_input, "utf-8"))
         else:
             # To make backward compatible with original public keys send encoded bytes in base64
             public_key_bytes = b64decode_ascii(public_key_input)
-            public_key = ed25519.Ed25519PublicKey.from_public_bytes(public_key_bytes)
+            pubkey = ed25519.Ed25519PublicKey.from_public_bytes(public_key_bytes)
 
-        if isinstance(message, str):
-            return self._verifyMessageStr(signature_b64, message, public_key)
-        elif isinstance(message, dict):
-            return self._verifyMessageJSON(signature_b64, message, public_key)
-        elif isinstance(message, bytes):
-            return self._verifyMessageBytes(signature_b64, message, public_key)
+        signature_bytes = b64decode(signature_b64)
+        for cls, verifier in verifiers.items():
+            if isinstance(pubkey, cls):
+                return verifier(pubkey).verify(message_bytes, signature_bytes)
         else:
-            raise Exception("Error: Not supported instance")
+            raise PangeaException(f"Not supported public key type: {type(pubkey)}")
 
-    def _is_pem_format(self, key: str) -> bool:
-        return key.startswith("-----")
+    def _decode_public_key(self, public_key: bytes):
+        """Parse a public key in PEM or ssh format"""
 
-    # Verify a message in bytes using Ed25519 algorithm
-    def _verifyMessageBytes(self, signature_b64: str, message_bytes: bytes, public_key: PUBLIC_KEY_TYPES) -> bool:
-        try:
-            signature = b64decode(signature_b64)
-            public_key.verify(signature, message_bytes)
-            return True
-        except Exception:
-            return False
+        for func in (serialization.load_pem_public_key, serialization.load_ssh_public_key):
+            try:
+                return func(public_key)
+            except exceptions.UnsupportedAlgorithm as e:
+                raise e
+            except ValueError:
+                pass
+
+        raise PangeaException("Unsupported key")
 
-    # Verify a string message using Ed25519 algorithm
-    def _verifyMessageStr(self, signature_b64: str, message: str, public_key: PUBLIC_KEY_TYPES) -> bool:
-        message_bytes = bytes(message, "utf8")
-        return self._verifyMessageBytes(signature_b64, message_bytes, public_key)
-
-    # Verify a JSON message using Ed25519 algorithm
-    def _verifyMessageJSON(self, signature_b64: str, messageJSON: dict, public_key: PUBLIC_KEY_TYPES) -> bool:
-        message_bytes = canonicalize_json(messageJSON)
-        return self._verifyMessageBytes(signature_b64, message_bytes, public_key)
+    def _has_header(self, key: str) -> bool:
+        return key.startswith("----") or key.startswith("ssh-")
```

### Comparing `pangea_sdk-1.8.0/pangea/services/audit/util.py` & `pangea_sdk-1.9.0/pangea/services/audit/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,25 +150,14 @@
 def verify_membership_proof(node_hash: Hash, root_hash: Hash, proof: MembershipProof) -> bool:
     for proof_item in proof:
         proof_hash = proof_item.node_hash
         node_hash = hash_pair(proof_hash, node_hash) if proof_item.side == "left" else hash_pair(node_hash, proof_hash)
     return root_hash == node_hash
 
 
-def format_datetime(dt: datetime):
-    """
-    Format a datetime in ISO format, using Z instead of +00:00
-    """
-    ret = dt.isoformat()
-    if dt.tzinfo is not None:
-        return ret.replace("+00:00", "Z")
-    else:
-        return ret + "Z"
-
-
 def normalize_log(audit: dict) -> dict:
     ans = {}
     for key in audit:
         if type(audit[key]) == datetime:
             ans[key] = format_datetime(audit[key])
         elif type(audit[key]) == dict:
             ans[key] = normalize_log(audit[key])
@@ -295,24 +284,7 @@
 
     logger.debug("Verifying the proofs for the new root")
     for item in proof:
         if not verify_membership_proof(item.node_hash, new_root, item.proof):
             return False
 
     return True
-
-
-def get_public_key(public_key_info: Optional[str]) -> Optional[str]:
-    if not public_key_info:
-        return None
-
-    try:
-        # Try to parse key_info as a json
-        key_info: dict = json.loads(public_key_info)
-        # If it's a json, public key come in "key" field
-        key = key_info.pop("key", None)
-        return key
-    except json.JSONDecodeError:
-        pass
-
-    # If it's not a json, public key should be used as a string
-    return public_key_info
```

### Comparing `pangea_sdk-1.8.0/pangea/services/authn/authn.py` & `pangea_sdk-1.9.0/pangea/services/authn/authn.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Dict, List, Optional
 
 import pangea.services.authn.models as m
 from pangea.response import PangeaResponse
 from pangea.services.base import ServiceBase
 
 SERVICE_NAME = "authn"
-VERSION = "v1"
 
 
 class AuthN(ServiceBase):
     """AuthN service client.
 
     Provides methods to interact with the [Pangea AuthN Service](https://pangea.cloud/docs/api/authn).
 
@@ -31,15 +30,14 @@
         authn_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea AuthN service
         authn = AuthN(token=PANGEA_TOKEN, config=authn_config)
     """
 
     service_name: str = SERVICE_NAME
-    version: str = VERSION
 
     def __init__(
         self,
         token,
         config=None,
         logger_name="pangea",
     ):
@@ -47,29 +45,28 @@
         self.user = AuthN.User(token, config, logger_name=logger_name)
         self.flow = AuthN.Flow(token, config, logger_name=logger_name)
         self.client = AuthN.Client(token, config, logger_name=logger_name)
         self.session = AuthN.Session(token, config, logger_name=logger_name)
 
     class Session(ServiceBase):
         service_name: str = SERVICE_NAME
-        version: str = VERSION
 
         def __init__(
             self,
             token,
             config=None,
             logger_name="pangea",
         ):
             super().__init__(token, config, logger_name=logger_name)
 
         # https://dev.pangea.cloud/docs/api/authn#invalidate-a-session-by-session-id
         # - path: authn::/v1/session/invalidate
         def invalidate(self, session_id: str) -> PangeaResponse[m.SessionInvalidateResult]:
             input = m.SessionInvalidateRequest(session_id=session_id)
-            response = self.request.post("session/invalidate", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/session/invalidate", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.SessionInvalidateResult(**response.raw_result)
             return response
 
         # https://dev.pangea.cloud/docs/api/authn#list-sessions
         # - path: authn::/v1/session/list
         def list(
@@ -77,75 +74,73 @@
             filter: Optional[Dict] = None,
             last: Optional[str] = None,
             order: Optional[m.ItemOrder] = None,
             order_by: Optional[m.SessionListOrderBy] = None,
             size: Optional[int] = None,
         ) -> PangeaResponse[m.SessionListResults]:
             input = m.SessionListRequest(filter=filter, last=last, order=order, order_by=order_by, size=size)
-            response = self.request.post("session/list", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/session/list", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.SessionListResults(**response.raw_result)
             return response
 
         # https://dev.pangea.cloud/docs/api/authn#invalidate-all-sessions-belonging-to-a-user
         # - path: authn::/v1/session/logout
         def logout(self, user_id: str) -> PangeaResponse[m.SessionLogoutResult]:
             input = m.SessionLogoutRequest(user_id=user_id)
-            response = self.request.post("session/logout", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/session/logout", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.SessionLogoutResult(**response.raw_result)
             return response
 
     class Client(ServiceBase):
         service_name: str = SERVICE_NAME
-        version: str = VERSION
 
         def __init__(
             self,
             token,
             config=None,
             logger_name="pangea",
         ):
             super().__init__(token, config, logger_name=logger_name)
             self.session = AuthN.Client.Session(token, config, logger_name=logger_name)
             self.password = AuthN.Client.Password(token, config, logger_name=logger_name)
 
         # https://dev.pangea.cloud/docs/api/authn#complete-a-login
         def userinfo(self, code: str) -> PangeaResponse[m.ClientUserinfoResult]:
             input = m.ClientUserinfoRequest(code=code)
-            response = self.request.post("client/userinfo", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/client/userinfo", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.ClientUserinfoResult(**response.raw_result)
             return response
 
         def jwks(
             self,
         ) -> PangeaResponse[m.ClientJWKSResult]:
-            response = self.request.post("client/jwks", {})
+            response = self.request.post("v1/client/jwks", {})
             if response.raw_result is not None:
                 response.result = m.ClientJWKSResult(**response.raw_result)
             return response
 
         class Session(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
 
             # - path: authn::/v1/client/session/invalidate
             # https://dev.pangea.cloud/docs/api/authn?focus=authn#invalidate-a-session-by-session-id-using-a-client-token
             def invalidate(self, token: str, session_id: str) -> PangeaResponse[m.ClientSessionInvalidateResult]:
                 input = m.ClientSessionInvalidateRequest(token=token, session_id=session_id)
-                response = self.request.post("client/session/invalidate", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/client/session/invalidate", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.ClientSessionInvalidateResult(**response.raw_result)
                 return response
 
             # https://dev.pangea.cloud/docs/api/authn#list-sessions-using-a-client-token
             # - path: authn::/v1/client/session/list
             def list(
@@ -156,83 +151,80 @@
                 order: Optional[m.ItemOrder] = None,
                 order_by: Optional[m.SessionListOrderBy] = None,
                 size: Optional[int] = None,
             ) -> PangeaResponse[m.ClientSessionListResults]:
                 input = m.ClientSessionInvalidateRequest(
                     token=token, filter=filter, last=last, order=order, order_by=order_by, size=size
                 )
-                response = self.request.post("client/session/list", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/client/session/list", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.ClientSessionListResults(**response.raw_result)
                 return response
 
             # https://dev.pangea.cloud/docs/api/authn#log-out-the-current-users-session
             # - path: authn::/v1/client/session/logout
             def logout(self, token: str) -> PangeaResponse[m.ClientSessionLogoutResult]:
                 input = m.ClientSessionLogoutRequest(token=token)
-                response = self.request.post("client/session/logout", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/client/session/logout", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.ClientSessionLogoutResult(**response.raw_result)
                 return response
 
             # https://dev.pangea.cloud/docs/api/authn#refresh-a-session-token
             # - path: authn::/v1/client/session/refresh
             def refresh(
                 self, refresh_token: str, user_token: Optional[str] = None
             ) -> PangeaResponse[m.ClientSessionRefreshResult]:
                 input = m.ClientSessionRefreshRequest(refresh_token=refresh_token, user_token=user_token)
-                response = self.request.post("client/session/refresh", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/client/session/refresh", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.ClientSessionRefreshResult(**response.raw_result)
                 return response
 
         class Password(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
 
             # https://dev.pangea.cloud/docs/api/authn#change-a-users-password
             def change(
                 self, token: str, old_password: str, new_password: str
             ) -> PangeaResponse[m.ClientPasswordChangeResult]:
                 input = m.ClientPasswordChangeRequest(token=token, old_password=old_password, new_password=new_password)
-                response = self.request.post("client/password/change", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/client/password/change", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.ClientPasswordChangeResult(**response.raw_result)
                 return response
 
         class Token(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
 
         def check(self, token: str) -> PangeaResponse[m.ClientTokenCheckResult]:
             input = m.ClientTokenCheckRequest(token=token)
-            response = self.request.post("client/token/check", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/client/token/check", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.ClientTokenCheckResult(**response.raw_result)
             return response
 
     class User(ServiceBase):
         service_name: str = SERVICE_NAME
-        version: str = VERSION
 
         def __init__(
             self,
             token,
             config=None,
             logger_name="pangea",
         ):
@@ -260,24 +252,24 @@
                 authenticator=authenticator,
                 id_provider=id_provider,
                 verified=verified,
                 require_mfa=require_mfa,
                 profile=profile,
                 scopes=scopes,
             )
-            response = self.request.post("user/create", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/user/create", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.UserCreateResult(**response.raw_result)
             return response
 
         #   - path: authn::/v1/user/delete
         # https://dev.pangea.cloud/docs/api/authn#delete-a-user
         def delete(self, email: Optional[str] = None, id: Optional[str] = None) -> PangeaResponse[m.UserDeleteResult]:
             input = m.UserDeleteRequest(email=email, id=id)
-            response = self.request.post("user/delete", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/user/delete", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.UserDeleteResult(**response.raw_result)
             return response
 
         # https://dev.pangea.cloud/docs/api/authn/#administration-user-update
         def update(
             self,
@@ -293,15 +285,15 @@
                 email=email,
                 authenticator=authenticator,
                 disabled=disabled,
                 require_mfa=require_mfa,
                 verified=verified,
             )
 
-            response = self.request.post("user/update", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/user/update", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.UserUpdateResult(**response.raw_result)
             return response
 
         #   - path: authn::/v1/user/invite
         # https://dev.pangea.cloud/docs/api/authn#invite-a-user
         def invite(
@@ -315,15 +307,15 @@
             input = m.UserInviteRequest(
                 inviter=inviter,
                 email=email,
                 callback=callback,
                 state=state,
                 require_mfa=require_mfa,
             )
-            response = self.request.post("user/invite", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/user/invite", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.UserInviteResult(**response.raw_result)
             return response
 
         #   - path: authn::/v1/user/list
         # https://dev.pangea.cloud/docs/api/authn#list-users
         def list(
@@ -337,146 +329,142 @@
             input = m.UserListRequest(
                 filter=filter,
                 last=last,
                 order=order,
                 order_by=order_by,
                 size=size,
             )
-            response = self.request.post("user/list", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/user/list", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.UserListResult(**response.raw_result)
             return response
 
         #   - path: authn::/v1/user/verify
         # https://dev.pangea.cloud/docs/api/authn#verify-a-user
         def verify(
             self, id_provider: m.IDProvider, email: str, authenticator: str
         ) -> PangeaResponse[m.UserVerifyResult]:
             input = m.UserVerifyRequest(id_provider=id_provider, email=email, authenticator=authenticator)
-            response = self.request.post("user/verify", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/user/verify", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.UserVerifyResult(**response.raw_result)
             return response
 
         class Password(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
 
             #   - path: authn::/v1/password/update
             # https://dev.pangea.cloud/docs/api/authn#change-a-users-password
             def reset(self, user_id: str, new_password: str) -> PangeaResponse[m.UserPasswordResetResult]:
                 input = m.UserPasswordResetRequest(user_id=user_id, new_password=new_password)
-                response = self.request.post("user/password/reset", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/password/reset", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserPasswordResetResult(**response.raw_result)
                 return response
 
         class Login(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
 
             # https://dev.pangea.cloud/docs/api/authn#user-login-with-a-password
             def password(
                 self, email: str, password: str, extra_profile: Optional[m.Profile] = None
             ) -> PangeaResponse[m.UserLoginResult]:
                 input = m.UserLoginPasswordRequest(email=email, password=password, extra_profile=extra_profile)
-                response = self.request.post("user/login/password", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/login/password", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserLoginResult(**response.raw_result)
                 return response
 
             # https://dev.pangea.cloud/docs/api/authn#user-login-with-a-social-provider
             def social(
                 self, provider: m.IDProvider, email: str, social_id: str, extra_profile: Optional[m.Profile] = None
             ) -> PangeaResponse[m.UserLoginResult]:
                 input = m.UserLoginSocialRequest(
                     provider=provider, email=email, social_id=social_id, extra_profile=extra_profile
                 )
-                response = self.request.post("user/login/social", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/login/social", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserLoginResult(**response.raw_result)
                 return response
 
         class MFA(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
 
             #   - path: authn::/v1/user/mfa/delete
             # https://dev.pangea.cloud/docs/api/authn#delete-mfa-enrollment-for-a-user
             def delete(self, user_id: str, mfa_provider: m.MFAProvider) -> PangeaResponse[m.UserMFADeleteResult]:
                 input = m.UserMFADeleteRequest(user_id=user_id, mfa_provider=mfa_provider)
-                response = self.request.post("user/mfa/delete", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/mfa/delete", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserMFADeleteResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/user/mfa/enroll
             # https://dev.pangea.cloud/docs/api/authn#enroll-mfa-for-a-user
             def enroll(
                 self, user_id: str, mfa_provider: m.MFAProvider, code: str
             ) -> PangeaResponse[m.UserMFAEnrollResult]:
                 input = m.UserMFAEnrollRequest(user_id=user_id, mfa_provider=mfa_provider, code=code)
-                response = self.request.post("user/mfa/enroll", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/mfa/enroll", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserMFAEnrollResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/user/mfa/start
             # https://dev.pangea.cloud/docs/api/authn#start-mfa-verification-for-a-user
             def start(
                 self,
                 user_id: str,
                 mfa_provider: m.MFAProvider,
                 enroll: Optional[bool] = None,
                 phone: Optional[str] = None,
             ) -> PangeaResponse[m.UserMFAStartResult]:
                 input = m.UserMFAStartRequest(user_id=user_id, mfa_provider=mfa_provider, enroll=enroll, phone=phone)
-                response = self.request.post("user/mfa/start", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/mfa/start", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserMFAStartResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/user/mfa/verify
             # https://dev.pangea.cloud/docs/api/authn#verify-an-mfa-code
             def verify(
                 self, user_id: str, mfa_provider: m.MFAProvider, code: str
             ) -> PangeaResponse[m.UserMFAVerifyResult]:
                 input = m.UserMFAverifyRequest(user_id=user_id, mfa_provider=mfa_provider, code=code)
-                response = self.request.post("user/mfa/verify", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/mfa/verify", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserMFAVerifyResult(**response.raw_result)
                 return response
 
         class Profile(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
@@ -484,15 +472,15 @@
 
             #   - path: authn::/v1/user/profile/get
             # https://dev.pangea.cloud/docs/api/authn#get-user
             def get(
                 self, id: Optional[str] = None, email: Optional[str] = None
             ) -> PangeaResponse[m.UserProfileGetResult]:
                 input = m.UserProfileGetRequest(id=id, email=email)
-                response = self.request.post("user/profile/get", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/profile/get", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserProfileGetResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/user/profile/update
             # https://dev.pangea.cloud/docs/api/authn#update-user
             def update(
@@ -502,22 +490,21 @@
                 email: Optional[str] = None,
             ) -> PangeaResponse[m.UserProfileUpdateResult]:
                 input = m.UserProfileUpdateRequest(
                     id=id,
                     email=email,
                     profile=profile,
                 )
-                response = self.request.post("user/profile/update", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/profile/update", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserProfileUpdateResult(**response.raw_result)
                 return response
 
         class Invites(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
@@ -530,31 +517,30 @@
                 filter: Optional[Dict] = None,
                 last: Optional[str] = None,
                 order: Optional[m.ItemOrder] = None,
                 order_by: Optional[m.UserInviterOrderBy] = None,
                 size: Optional[int] = None,
             ) -> PangeaResponse[m.UserInviteListResult]:
                 input = m.UserInviteListRequest(filter=filter, last=last, order=order, order_by=order_by, size=size)
-                response = self.request.post("user/invite/list", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/invite/list", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserInviteListResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/user/invite/delete
             # https://dev.pangea.cloud/docs/api/authn#delete-an-invite
             def delete(self, id: str) -> PangeaResponse[m.UserInviteDeleteResult]:
                 input = m.UserInviteDeleteRequest(id=id)
-                response = self.request.post("user/invite/delete", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/user/invite/delete", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.UserInviteDeleteResult(**response.raw_result)
                 return response
 
     class Flow(ServiceBase):
         service_name: str = SERVICE_NAME
-        version: str = VERSION
 
         def __init__(
             self,
             token,
             config=None,
             logger_name="pangea",
         ):
@@ -564,37 +550,36 @@
             self.verify = AuthN.Flow.Verify(token, config, logger_name=logger_name)
             self.reset = AuthN.Flow.Reset(token, config, logger_name=logger_name)
 
         #   - path: authn::/v1/flow/complete
         # https://dev.pangea.cloud/docs/api/authn#complete-a-login-or-signup-flow
         def complete(self, flow_id: str) -> PangeaResponse[m.FlowCompleteResult]:
             input = m.FlowCompleteRequest(flow_id=flow_id)
-            response = self.request.post("flow/complete", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/flow/complete", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.FlowCompleteResult(**response.raw_result)
             return response
 
         #   - path: authn::/v1/flow/start
         # https://dev.pangea.cloud/docs/api/authn#start-a-new-signup-or-signin-flow
         def start(
             self,
             cb_uri: Optional[str] = None,
             email: Optional[str] = None,
             flow_types: Optional[List[m.FlowType]] = None,
             provider: Optional[m.MFAProvider] = None,
         ) -> PangeaResponse[m.FlowStartResult]:
             input = m.FlowStartRequest(cb_uri=cb_uri, email=email, flow_types=flow_types, provider=provider)
-            response = self.request.post("flow/start", data=input.dict(exclude_none=True))
+            response = self.request.post("v1/flow/start", data=input.dict(exclude_none=True))
             if response.raw_result is not None:
                 response.result = m.FlowStartResult(**response.raw_result)
             return response
 
         class Reset(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
@@ -609,35 +594,33 @@
                 cancel: Optional[bool] = None,
                 cb_state: Optional[str] = None,
                 cb_code: Optional[str] = None,
             ) -> PangeaResponse[m.FlowResetPasswordResult]:
                 input = m.FlowResetPasswordRequest(
                     flow_id=flow_id, password=password, cb_state=cb_state, cb_code=cb_code, cancel=cancel
                 )
-                response = self.request.post("flow/reset/password", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/reset/password", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowResetPasswordResult(**response.raw_result)
                 return response
 
         class Enroll(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
                 self.mfa = AuthN.Flow.Enroll.MFA(token, config, logger_name=logger_name)
 
             class MFA(ServiceBase):
                 service_name: str = SERVICE_NAME
-                version: str = VERSION
 
                 def __init__(
                     self,
                     token,
                     config=None,
                     logger_name="pangea",
                 ):
@@ -645,33 +628,32 @@
 
                 #   - path: authn::/v1/flow/enroll/mfa/complete
                 # https://dev.pangea.cloud/docs/api/authn#complete-mfa-enrollment-by-verifying-a-trial-mfa-code
                 def complete(
                     self, flow_id: str, code: Optional[str] = None, cancel: Optional[bool] = None
                 ) -> PangeaResponse[m.FlowEnrollMFAcompleteResult]:
                     input = m.FlowEnrollMFACompleteRequest(flow_id=flow_id, code=code, cancel=cancel)
-                    response = self.request.post("flow/enroll/mfa/complete", data=input.dict(exclude_none=True))
+                    response = self.request.post("v1/flow/enroll/mfa/complete", data=input.dict(exclude_none=True))
                     if response.raw_result is not None:
                         response.result = m.FlowEnrollMFAcompleteResult(**response.raw_result)
                     return response
 
                 #   - path: authn::/v1/flow/enroll/mfa/start
                 # https://dev.pangea.cloud/docs/api/authn#start-the-process-of-enrolling-an-mfa
                 def start(
                     self, flow_id: str, mfa_provider: m.MFAProvider, phone: Optional[str] = None
                 ) -> PangeaResponse[m.FlowEnrollMFAStartResult]:
                     input = m.FlowEnrollMFAStartRequest(flow_id=flow_id, mfa_provider=mfa_provider, phone=phone)
-                    response = self.request.post("flow/enroll/mfa/start", data=input.dict(exclude_none=True))
+                    response = self.request.post("v1/flow/enroll/mfa/start", data=input.dict(exclude_none=True))
                     if response.raw_result is not None:
                         response.result = m.FlowEnrollMFAStartResult(**response.raw_result)
                     return response
 
         class Signup(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
@@ -681,84 +663,82 @@
             # https://dev.pangea.cloud/docs/api/authn#signup-a-new-account-using-a-password
             def password(
                 self, flow_id: str, password: str, first_name: str, last_name: str
             ) -> PangeaResponse[m.FlowSignupPasswordResult]:
                 input = m.FlowSignupPasswordRequest(
                     flow_id=flow_id, password=password, first_name=first_name, last_name=last_name
                 )
-                response = self.request.post("flow/signup/password", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/signup/password", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowSignupPasswordResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/flow/signup/social
             # https://dev.pangea.cloud/docs/api/authn#signup-a-new-account-using-a-social-provider
             def social(self, flow_id: str, cb_state: str, cb_code: str) -> PangeaResponse[m.FlowSignupSocialResult]:
                 input = m.FlowSignupSocialRequest(flow_id=flow_id, cb_state=cb_state, cb_code=cb_code)
-                response = self.request.post("flow/signup/social", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/signup/social", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowSignupSocialResult(**response.raw_result)
                 return response
 
         class Verify(ServiceBase):
             service_name: str = SERVICE_NAME
-            version: str = VERSION
 
             def __init__(
                 self,
                 token,
                 config=None,
                 logger_name="pangea",
             ):
                 super().__init__(token, config, logger_name=logger_name)
                 self.mfa = AuthN.Flow.Verify.MFA(token, config, logger_name=logger_name)
 
             #   - path: authn::/v1/flow/verify/captcha
             # https://dev.pangea.cloud/docs/api/authn#verify-a-captcha-during-a-signup-or-signin-flow
             def captcha(self, flow_id: str, code: str) -> PangeaResponse[m.FlowVerifyCaptchaResult]:
                 input = m.FlowVerifyCaptchaRequest(flow_id=flow_id, code=code)
-                response = self.request.post("flow/verify/captcha", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/verify/captcha", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowVerifyCaptchaResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/flow/verify/email
             # https://dev.pangea.cloud/docs/api/authn#verify-an-email-address-during-a-signup-or-signin-flow
             def email(
                 self, flow_id: str, cb_state: Optional[str] = None, cb_code: Optional[str] = None
             ) -> PangeaResponse[m.FlowVerifyEmailResult]:
                 input = m.FlowVerifyEmailRequest(flow_id=flow_id, cb_state=cb_state, cb_code=cb_code)
-                response = self.request.post("flow/verify/email", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/verify/email", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowVerifyEmailResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/flow/verify/password
             # https://dev.pangea.cloud/docs/api/authn#sign-in-with-a-password
             def password(
                 self, flow_id: str, password: Optional[str] = None, cancel: Optional[bool] = None
             ) -> PangeaResponse[m.FlowVerifyPasswordResult]:
                 input = m.FlowVerifyPasswordRequest(flow_id=flow_id, password=password, cancel=cancel)
-                response = self.request.post("flow/verify/password", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/verify/password", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowVerifyPasswordResult(**response.raw_result)
                 return response
 
             #   - path: authn::/v1/flow/verify/social
             # https://dev.pangea.cloud/docs/api/authn#signin-with-a-social-provider
             def social(self, flow_id: str, cb_state: str, cb_code: str) -> PangeaResponse[m.FlowVerifySocialResult]:
                 input = m.FlowVerifySocialRequest(flow_id=flow_id, cb_state=cb_state, cb_code=cb_code)
-                response = self.request.post("flow/verify/social", data=input.dict(exclude_none=True))
+                response = self.request.post("v1/flow/verify/social", data=input.dict(exclude_none=True))
                 if response.raw_result is not None:
                     response.result = m.FlowVerifySocialResult(**response.raw_result)
                 return response
 
             class MFA(ServiceBase):
                 service_name: str = SERVICE_NAME
-                version: str = VERSION
 
                 def __init__(
                     self,
                     token,
                     config=None,
                     logger_name="pangea",
                 ):
@@ -766,42 +746,42 @@
 
                 #   - path: authn::/v1/flow/verify/mfa/complete
                 # https://dev.pangea.cloud/docs/api/authn#complete-mfa-verification
                 def complete(
                     self, flow_id: str, code: Optional[str] = None, cancel: Optional[bool] = None
                 ) -> PangeaResponse[m.FlowVerifyMFACompleteResult]:
                     input = m.FlowVerifyMFACompleteRequest(flow_id=flow_id, code=code, cancel=cancel)
-                    response = self.request.post("flow/verify/mfa/complete", data=input.dict(exclude_none=True))
+                    response = self.request.post("v1/flow/verify/mfa/complete", data=input.dict(exclude_none=True))
                     if response.raw_result is not None:
                         response.result = m.FlowVerifyMFACompleteResult(**response.raw_result)
                     return response
 
                 #   - path: authn::/v1/flow/verify/mfa/start
                 # https://dev.pangea.cloud/docs/api/authn#start-the-process-of-mfa-verification
                 def start(
                     self, flow_id: str, mfa_provider: m.MFAProvider
                 ) -> PangeaResponse[m.FlowVerifyMFAStartResult]:
                     input = m.FlowVerifyMFAStartRequest(flow_id=flow_id, mfa_provider=mfa_provider)
-                    response = self.request.post("flow/verify/mfa/start", data=input.dict(exclude_none=True))
+                    response = self.request.post("v1/flow/verify/mfa/start", data=input.dict(exclude_none=True))
                     if response.raw_result is not None:
                         response.result = m.FlowVerifyMFAStartResult(**response.raw_result)
                     return response
 
     # class Token(ServiceBase):
     #     service_name: str = SERVICE_NAME
-    #     version: str = VERSION
+    #
 
     #     def __init__(
     #         self,
     #         token,
     #         config=None,
     #       logger_name="pangea",
     #     ):
     #         super().__init__(token, config, logger_name=logger_name)
 
     #     # https://dev.pangea.cloud/docs/api/authn?focus=authn#invalidate-a-session-by-session-id-using-a-client-token
     #     def list(self, ) -> PangeaResponse[m.ClientSessionInvalidateResult]:
     #         input = m.ClientSessionInvalidateRequest(token=token, session_id=session_id)
-    #         response = self.request.post("client/session/invalidate", data=input.dict(exclude_none=True))
+    #         response = self.request.post("v1/client/session/invalidate", data=input.dict(exclude_none=True))
     #         if response.raw_result is not None:
     #             response.result = m.ClientSessionInvalidateResult(**response.raw_result)
     #         return response
```

### Comparing `pangea_sdk-1.8.0/pangea/services/authn/models.py` & `pangea_sdk-1.9.0/pangea/services/authn/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     disabled: bool
     last_login_at: Optional[str] = None
     created_at: str
 
 
 class UserListResult(PangeaResponseResult):
     users: List[User]
-    last: str
+    last: Optional[str] = None
     count: int
 
 
 class UserLoginPasswordRequest(APIRequestModel):
     email: str
     password: str
     extra_profile: Optional[Profile] = None
```

### Comparing `pangea_sdk-1.8.0/pangea/services/base.py` & `pangea_sdk-1.9.0/pangea/services/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 
 import copy
 import logging
 from typing import Optional
 
-from pangea import __version__
 from pangea.config import PangeaConfig
 from pangea.request import PangeaRequest
 
 
 class ServiceBase(object):
     service_name: str = "base"
-    version: str = "v1"
 
     def __init__(self, token, config: Optional[PangeaConfig] = None, logger_name: str = "pangea"):
         if not token:
             raise Exception("No token provided")
 
         self.config = config if copy.deepcopy(config) else PangeaConfig()
         self.logger = logging.getLogger(logger_name)
 
         self.request = PangeaRequest(
             self.config,
             token,
-            self.version,
             self.service_name,
             self.logger,
         )
 
         extra_headers = {}
         self.request.set_extra_headers(extra_headers)
```

### Comparing `pangea_sdk-1.8.0/pangea/services/embargo.py` & `pangea_sdk-1.9.0/pangea/services/embargo.py`

 * *Files 25% similar despite different names*

```diff
@@ -74,21 +74,22 @@
         embargo_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Embargo service
         embargo = Embargo(token=PANGEA_TOKEN, config=embargo_config)
     """
 
     service_name = "embargo"
-    version = "v1"
 
     def ip_check(self, ip: str) -> PangeaResponse[EmbargoResult]:
         """
         Check IP
 
-        Check this IP against known sanction and trade embargo lists.
+        Check an IP against known sanction and trade embargo lists.
+
+        OperationId: embargo_post_v1_ip_check
 
         Args:
             ip (str): Geolocate this IP and check the corresponding country
                 against the enabled embargo lists.  Accepts both IPV4 and IPV6 strings.
 
         Raises:
             EmbargoException: If an embargo based api exception happens
@@ -96,85 +97,43 @@
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found
                 in our [API Documentation](https://pangea.cloud/docs/api/embargo).
 
         Examples:
-            response = embargo.ip_check("1.1.1.1")
-
-            \"\"\"
-            response contains:
-            {
-                "request_id": "prq_lws4ldnnruaos2a4c2ohgw7ijodzqf52",
-                "request_time": "2022-07-06T23:37:36.952Z",
-                "response_time": "2022-07-06T23:37:37.104Z",
-                "status": "success",
-                "summary": "Found country in 1 embargo list(s)",
-                "result": {
-                    "sanctions": [
-                    {
-                        "list_name": "ITAR",
-                        "embargoed_country_name": "North Korea/Democratic Peoples Republic of Korea",
-                        "embargoed_country_iso_code": "KP",
-                        "issuing_country": "US",
-                        "annotations": {
-                        "reference": {
-                            "paragraph": "d1",
-                            "regulation": "CFR 126.1"
-                        },
-                        "restriction_name": "ITAR"
-                        }
-                    }
-                    ],
-                    "count": 1
-                }
-            }
-            \"\"\"
+            response = embargo.ip_check("190.6.64.94")
         """
         input = IPCheckRequest(ip=ip)
-        response = self.request.post("ip/check", data=input.dict())
+        response = self.request.post("v1/ip/check", data=input.dict())
         result = EmbargoResult(**response.raw_result)
         response.result = result
         return response
 
     def iso_check(self, iso_code: str) -> PangeaResponse[EmbargoResult]:
         """
         ISO Code Check
 
         Check this country against known sanction and trade embargo lists.
 
+        OperationId: embargo_post_v1_iso_check
+
         Args:
             iso_code (str): Check this two character country ISO-code against
                 the enabled embargo lists.
 
         Raises:
             EmbargoException: If an embargo based api exception happens
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found
                 in our [API Documentation](https://pangea.cloud/docs/api/embargo).
 
         Examples:
-            response = embargo.lookup("FR")
-
-            \"\"\"
-            response contains:
-            {
-                "request_id": "prq_fa6yqoztkfdyg655s6dut5e3bn3plmj5",
-                "request_time": "2022-07-06T23:44:29.248Z",
-                "response_time": "2022-07-06T23:44:29.357Z",
-                "status": "success",
-                "summary": "Found country in 0 embargo list(s)",
-                "result": {
-                    "sanctions": null,
-                    "count": 0
-                }
-            }
-            \"\"\"
+            response = embargo.iso_check("CU")
         """
         input = ISOCheckRequest(iso_code=iso_code)
-        response = self.request.post("iso/check", data=input.dict())
+        response = self.request.post("v1/iso/check", data=input.dict())
         response.result = EmbargoResult(**response.raw_result)
         return response
```

### Comparing `pangea_sdk-1.8.0/pangea/services/intel.py` & `pangea_sdk-1.9.0/pangea/services/intel.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,14 @@
         file_intel_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea File Intel service
         file_intel = FileIntel(token=PANGEA_TOKEN, config=file_intel_config)
     """
 
     service_name = "file-intel"
-    version = "v1"
 
     @pangea_deprecated(version="1.2.0", reason="Should use FileIntel.hashReputation()")
     def lookup(
         self,
         hash: str,
         hash_type: str,
         provider: Optional[str] = None,
@@ -328,15 +327,15 @@
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/file-intel).
 
         Examples:
             response = file_intel.lookup(hash="142b638c6a60b60c7f9928da4fb85a5a8e1422a9ffdc9ee49e17e56ccca9cf6e", hash_type="sha256", provider="reversinglabs")
         """
         input = FileReputationRequest(hash=hash, hash_type=hash_type, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = FileReputationResult(**response.raw_result)
         return response
 
     def hashReputation(
         self,
         hash: str,
         hash_type: str,
@@ -364,15 +363,15 @@
                 response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/file-intel).
 
         Examples:
             response = file_intel.hashReputation(hash="142b638c6a60b60c7f9928da4fb85a5a8e1422a9ffdc9ee49e17e56ccca9cf6e", hash_type="sha256", provider="reversinglabs")
 
         """
         input = FileReputationRequest(hash=hash, hash_type=hash_type, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = FileReputationResult(**response.raw_result)
         return response
 
     @pangea_deprecated(version="1.2.0", reason="Should use FileIntel.filepathReputation()")
     def lookupFilepath(
         self,
         filepath: str,
@@ -402,15 +401,15 @@
             response = file_intel.lookupFilepath(filepath="./myfile.exe", provider="reversinglabs"))
         """
 
         data = open(filepath, "rb")
         hash = hashlib.sha256(data.read()).hexdigest()
 
         input = FileReputationRequest(hash=hash, hash_type="sha256", verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = FileReputationResult(**response.raw_result)
         return response
 
     def filepathReputation(
         self,
         filepath: str,
         provider: Optional[str] = None,
@@ -419,36 +418,41 @@
     ) -> PangeaResponse[FileReputationResult]:
         """
         Reputation, from filepath
 
         Retrieve hash-based file reputation from a provider, including an optional detailed report.
         This function take care of calculate filepath hash and make the request to service
 
+        OperationId: file_intel_post_v1_reputation
+
         Args:
             filepath (str): The path to the file to be looked up
             provider (str, optional): Use reputation data from these providers: "reversinglabs" or "crowdstrike"
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/file-intel).
 
         Examples:
-            response = file_intel.filepathReputation(filepath="./myfile.exe", provider="reversinglabs"))
+            response = file_intel.filepathReputation(
+                filepath="./myfile.exe",
+                provider="reversinglabs",
+            )
         """
 
         data = open(filepath, "rb")
         hash = hashlib.sha256(data.read()).hexdigest()
 
         input = FileReputationRequest(hash=hash, hash_type="sha256", verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = FileReputationResult(**response.raw_result)
         return response
 
 
 class DomainIntel(ServiceBase):
     """Domain Intel service client
 
@@ -470,15 +474,14 @@
         domain_intel_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Domain Intel service
         domain_intel = DomainIntel(token=PANGEA_TOKEN, config=domain_intel_config)
     """
 
     service_name = "domain-intel"
-    version = "v1"
 
     @pangea_deprecated(version="1.2.0", reason="Should use DomainIntel.reputation()")
     def lookup(
         self, domain: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[DomainReputationResult]:
         """
         Reputation check
@@ -498,44 +501,49 @@
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/domain-intel).
 
         Examples:
             response = domain_intel.lookup(domain="737updatesboeing.com", provider="domaintools")
         """
         input = DomainReputationRequest(domain=domain, verbose=verbose, provider=provider, raw=raw)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = DomainReputationResult(**response.raw_result)
         return response
 
     def reputation(
         self, domain: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[DomainReputationResult]:
         """
-        Reputation check
+        Reputation
 
         Retrieve reputation for a domain from a provider, including an optional detailed report.
 
+        OperationId: domain_intel_post_v1_reputation
+
         Args:
             domain (str): The domain to be looked up
             provider (str, optional): Use reputation data from these providers: "domaintools" or "crowdstrike"
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/domain-intel).
 
         Examples:
-            response = domain_intel.lookup(domain="737updatesboeing.com", provider="domaintools")
+            response = domain_intel.lookup(
+                domain="737updatesboeing.com",
+                provider="domaintools",
+            )
         """
         input = DomainReputationRequest(domain=domain, verbose=verbose, provider=provider, raw=raw)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = DomainReputationResult(**response.raw_result)
         return response
 
 
 class IpIntel(ServiceBase):
     """IP Intel service client
 
@@ -557,15 +565,14 @@
         ip_intel_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea IP Intel service
         ip_intel = IpIntel(token=PANGEA_TOKEN, config=ip_intel_config)
     """
 
     service_name = "ip-intel"
-    version = "v1"
 
     @pangea_deprecated(version="1.2.0", reason="Should use IpIntel.reputation()")
     def lookup(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPReputationResult]:
         """
         Reputation
@@ -586,160 +593,185 @@
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
 
         Examples:
             response = ip_intel.lookup(ip="93.231.182.110", provider="crowdstrike")
 
         """
         input = IPRepurationRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = IPReputationResult(**response.raw_result)
         return response
 
     def reputation(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPReputationResult]:
         """
         Reputation
 
         Retrieve a reputation score for an IP address from a provider, including an optional detailed report.
 
+        OperationId: ip_intel_post_v1_reputation
+
         Args:
             ip (str): The IP to be looked up
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
             provider (str, optional): Use reputation data from this provider: "crowdstrike"
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
 
         Examples:
-            response = ip_intel.reputation(ip="93.231.182.110", provider="crowdstrike")
+            response = ip_intel.reputation(
+                ip="93.231.182.110",
+                provider="crowdstrike",
+            )
         """
         input = IPRepurationRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = IPReputationResult(**response.raw_result)
         return response
 
     def geolocate(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPGeolocateResult]:
         """
         Geolocate
 
         Retrieve information about the location of an IP address.
 
+        OperationId: ip_intel_post_v1_geolocate
+
         Args:
             ip (str): IP address to be geolocated
             provider (str, optional): Use geolocation data from this provider ("digitalelement"). Default provider defined by the configuration.
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the IP information is in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
 
         Examples:
-            response = ip_intel.geolocate(ip="93.231.182.110", provider="digitalelement")
+            response = ip_intel.geolocate(
+                ip="93.231.182.110",
+                provider="digitalelement",
+            )
         """
         input = IPGeolocateRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("geolocate", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/geolocate", data=input.dict(exclude_none=True))
         response.result = IPGeolocateResult(**response.raw_result)
         return response
 
     def get_domain(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPDomainResult]:
         """
         Domain
 
         Retrieve the domain name associated with an IP address.
 
+        OperationId: ip_intel_post_v1_domain
+
         Args:
-            ip (str): IP address to be geolocated
+            ip (str): The IP to be looked up
             provider (str, optional): Use geolocation data from this provider ("digitalelement"). Default provider defined by the configuration.
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the IP information is in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
 
         Examples:
-            response = ip_intel.get_domain(ip="93.231.182.110", provider="digitalelement")
+            response = ip_intel.get_domain(
+                ip="93.231.182.110",
+                provider="digitalelement",
+            )
         """
         input = IPDomainRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("domain", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/domain", data=input.dict(exclude_none=True))
         response.result = IPDomainResult(**response.raw_result)
         return response
 
     def is_vpn(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPVPNResult]:
         """
         VPN
 
         Determine if an IP address is provided by a VPN service.
 
+        OperationId: ip_intel_post_v1_vpn
+
         Args:
-            ip (str): IP address to be geolocated
+            ip (str): The IP to be looked up
             provider (str, optional): Use geolocation data from this provider ("digitalelement"). Default provider defined by the configuration.
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the IP information is in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
 
         Examples:
-            response = ip_intel.is_vpn(ip="93.231.182.110", provider="digitalelement")
+            response = ip_intel.is_vpn(
+                ip="93.231.182.110",
+                provider="digitalelement",
+            )
         """
         input = IPVPNRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("vpn", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/vpn", data=input.dict(exclude_none=True))
         response.result = IPVPNResult(**response.raw_result)
         return response
 
     def is_proxy(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPProxyResult]:
         """
         Proxy
 
         Determine if an IP address is provided by a proxy service.
 
+        OperationId: ip_intel_post_v1_proxy
+
         Args:
-            ip (str): IP address to be geolocated
+            ip (str): The IP to be looked up
             provider (str, optional): Use geolocation data from this provider ("digitalelement"). Default provider defined by the configuration.
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the IP information is in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
 
         Examples:
-            response = ip_intel.is_proxy(ip="93.231.182.110", provider="digitalelement")
+            response = ip_intel.is_proxy(
+                ip="93.231.182.110",
+                provider="digitalelement",
+            )
         """
         input = IPProxyRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("proxy", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/proxy", data=input.dict(exclude_none=True))
         response.result = IPProxyResult(**response.raw_result)
         return response
 
 
 class UrlIntel(ServiceBase):
     """URL Intel service client.
 
@@ -761,15 +793,14 @@
         url_intel_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea URL Intel service
         url_intel = UrlIntel(token=PANGEA_TOKEN, config=url_intel_config)
     """
 
     service_name = "url-intel"
-    version = "v1"
 
     @pangea_deprecated(version="1.2.0", reason="Should use UrlIntel.reputation()")
     def lookup(
         self, url: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[URLReputationResult]:
         """
         Reputation check
@@ -790,45 +821,50 @@
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
 
         Examples:
             response = url_intel.lookup(url="http://113.235.101.11:54384", provider="crowdstrike")
         """
 
         input = URLReputationRequest(url=url, provider=provider, verbose=verbose, raw=raw)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = URLReputationResult(**response.raw_result)
         return response
 
     def reputation(
         self, url: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[URLReputationResult]:
         """
-        Reputation check
+        Reputation
 
         Retrieve URL address reputation from a provider.
 
+        OperationId: url_intel_post_v1_reputation
+
         Args:
             url (str): The URL to be looked up
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
             provider (str, optional): Use reputation data from this provider: "crowdstrike"
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
 
         Examples:
-            response = url_intel.reputation(url="http://113.235.101.11:54384", provider="crowdstrike")
+            response = url_intel.reputation(
+                url="http://113.235.101.11:54384",
+                provider="crowdstrike",
+            )
         """
 
         input = URLReputationRequest(url=url, provider=provider, verbose=verbose, raw=raw)
-        response = self.request.post("reputation", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
         response.result = URLReputationResult(**response.raw_result)
         return response
 
 
 class UserBreachedRequest(IntelCommonRequest):
     """
     User breached common request data
@@ -923,15 +959,14 @@
         user_intel_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea User Intel service
         user_intel = UserIntel(token=PANGEA_TOKEN, config=user_intel_config)
     """
 
     service_name = "user-intel"
-    version = "v1"
 
     def user_breached(
         self,
         email: Optional[str] = None,
         username: Optional[str] = None,
         ip: Optional[str] = None,
         phone_number: Optional[str] = None,
@@ -942,14 +977,16 @@
         provider: Optional[str] = None,
     ) -> PangeaResponse[UserBreachedResult]:
         """
         Look up breached users
 
         Find out if an email address, username, phone number, or IP address was exposed in a security breach.
 
+        OperationId: user_intel_post_v1_user_breached
+
         Args:
             email (str): An email address to search for
             username (str): An username to search for
             ip (str): An ip to search for
             phone_number (str): A phone number to search for. minLength: 7, maxLength: 15.
             start (str): Earliest date for search
             end (str): Latest date for search
@@ -961,31 +998,34 @@
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
 
         Examples:
-            response = self.intel_user.user_breached(
-                phone_number="8005550123", provider="spycloud", verbose=True, raw=True
+            response = user_intel.user_breached(
+                phone_number="8005550123",
+                provider="spycloud",
+                verbose=True,
+                raw=True,
             )
         """
 
         input = UserBreachedRequest(
             email=email,
             phone_number=phone_number,
             username=username,
             ip=ip,
             provider=provider,
             start=start,
             end=end,
             verbose=verbose,
             raw=raw,
         )
-        response = self.request.post("user/breached", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/user/breached", data=input.dict(exclude_none=True))
         response.result = UserBreachedResult(**response.raw_result)
         return response
 
     def password_breached(
         self,
         hash_type: HashType,
         hash_prefix: str,
@@ -994,14 +1034,16 @@
         provider: Optional[str] = None,
     ) -> PangeaResponse[UserPasswordBreachedResult]:
         """
         Look up breached passwords
 
         Find out if a password has been exposed in security breaches by providing a 5 character prefix of the password hash.
 
+        OperationId: user_intel_post_v1_password_breached
+
         Args:
             hash_type (str): Hash type to be looked up
             hash_prefix (str): The prefix of the hash to be looked up.
             verbose (bool, optional): Echo the API parameters in the response
             raw (bool, optional): Include raw data from this provider
             provider (str, optional): Use reputation data from this provider: "crowdstrike"
 
@@ -1009,16 +1051,20 @@
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the sanctioned source(s) are in the
                 response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
 
         Examples:
-            response = self.intel_user.password_breached(hash_prefix="5baa6", hash_type=HashType.SHA256, provider="spycloud")
+            response = user_intel.password_breached(
+                hash_prefix="5baa6",
+                hash_type=HashType.SHA256,
+                provider="spycloud",
+            )
         """
 
         input = UserPasswordBreachedRequest(
             hash_type=hash_type, hash_prefix=hash_prefix, provider=provider, verbose=verbose, raw=raw
         )
-        response = self.request.post("password/breached", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/password/breached", data=input.dict(exclude_none=True))
         response.result = UserPasswordBreachedResult(**response.raw_result)
         return response
```

### Comparing `pangea_sdk-1.8.0/pangea/services/redact.py` & `pangea_sdk-1.9.0/pangea/services/redact.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,14 @@
         redact_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Redact service client
         redact = Redact(token=PANGEA_TOKEN, config=redact_config)
     """
 
     service_name = "redact"
-    version = "v1"
 
     def __init__(
         self,
         token,
         config=None,
         logger_name="pangea",
     ):
@@ -147,37 +146,39 @@
         debug: Optional[bool] = None,
         rules: Optional[List[str]] = None,
         return_result: Optional[bool] = None,
     ) -> PangeaResponse[RedactResult]:
         """
         Redact
 
-        Redacts the content of a single text string
+        Redact sensitive information from provided text.
+
+        OperationId: redact_post_v1_redact
 
         Args:
-            text (str): The text to be redacted
+            text (str): The text data to redact
             debug (bool, optional): Setting this value to true will provide a detailed analysis of
                 the redacted data and the rules that caused redaction
             rules (list[str], optional): An array of redact rule short names
             return_result(bool, optional): Setting this value to false will omit the redacted result only returning count
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             Pangea Response with redacted text in the response.result property,
                 available response fields can be found in our
                 [API Documentation](https://pangea.cloud/docs/api/redact#redact).
 
         Examples:
-            response = redact.redact(text="Jenny Jenny... 415-867-5309")
+            response = redact.redact(text="Jenny Jenny... 555-867-5309")
         """
 
         input = RedactRequest(text=text, debug=debug, rules=rules, return_result=return_result)
-        response = self.request.post("redact", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/redact", data=input.dict(exclude_none=True))
         response.result = RedactResult(**response.raw_result)
         return response
 
     def redact_structured(
         self,
         data: Union[Dict, str],
         jsonp: Optional[List[str]] = None,
@@ -185,15 +186,17 @@
         debug: Optional[bool] = None,
         rules: Optional[List[str]] = None,
         return_result: Optional[bool] = None,
     ) -> PangeaResponse[StructuredResult]:
         """
         Redact structured
 
-        Redacts text within a structured object
+        Redact sensitive information from structured data (e.g., JSON).
+
+        OperationId: redact_post_v1_redact_structured
 
         Args:
             data (dict, str): Structured data to redact
             jsonp (list[str]): JSON path(s) used to identify the specific JSON fields to redact in
                 the structured data. Note: If jsonp parameter is used, the data parameter must be
                 in JSON format.
             format (RedactFormat, optional): The format of the passed data. Default: "json"
@@ -207,16 +210,21 @@
 
         Returns:
             Pangea Response with redacted data in the response.result field,
                 available response fields can be found in our
                 [API Documentation](https://pangea.cloud/docs/api/redact#redact-structured)
 
         Examples:
-            response = redact.redact_structured(data={"number": "415-867-5309", "ip": "1.1.1.1"}, redact_format="json")
+            data = {
+                "number": "555-867-5309",
+                "ip": "1.1.1.1",
+            }
+
+            response = redact.redact_structured(data=data, redact_format="json")
         """
 
         input = StructuredRequest(
             data=data, jsonp=jsonp, format=format, debug=debug, rules=rules, return_result=return_result
         )
-        response = self.request.post("redact_structured", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/redact_structured", data=input.dict(exclude_none=True))
         response.result = StructuredResult(**response.raw_result)
         return response
```

### Comparing `pangea_sdk-1.8.0/pangea/services/vault/models/asymmetric.py` & `pangea_sdk-1.9.0/pangea/services/vault/models/asymmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/services/vault/models/common.py` & `pangea_sdk-1.9.0/pangea/services/vault/models/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import datetime
 import enum
-from typing import Any, Dict, List, NewType, Optional, Union
+from typing import Dict, List, NewType, Optional, Union
 
 from pangea.response import APIRequestModel, PangeaResponseResult
 
 # EncodedPublicKey is a PEM public key, with no further encoding (i.e. no base64)
 # It may be used for example in openssh with no further processing
 EncodedPublicKey = NewType("EncodedPublicKey", str)
 
@@ -33,14 +33,27 @@
 class AsymmetricAlgorithm(str, enum.Enum):
     Ed25519 = "ED25519"
     RSA2048_PKCS1V15_SHA256 = "RSA-PKCS1V15-2048-SHA256"
     RSA2048_OAEP_SHA256 = "RSA-OAEP-2048-SHA256"
     ES256 = "ES256"
     ES384 = "ES384"
     ES512 = "ES512"
+    ES256K = "ES256K"
+    RSA2048_OAEP_SHA1 = "RSA-OAEP-2048-SHA1"
+    RSA2048_OAEP_SHA512 = "RSA-OAEP-2048-SHA512"
+    RSA3072_OAEP_SHA1 = "RSA-OAEP-3072-SHA1"
+    RSA3072_OAEP_SHA256 = "RSA-OAEP-3072-SHA256"
+    RSA3072_OAEP_SHA512 = "RSA-OAEP-3072-SHA512"
+    RSA4096_OAEP_SHA1 = "RSA-OAEP-4096-SHA1"
+    RSA4096_OAEP_SHA256 = "RSA-OAEP-4096-SHA256"
+    RSA4096_OAEP_SHA512 = "RSA-OAEP-4096-SHA512"
+    RSA2048_PSS_SHA256 = "RSA-PSS-2048-SHA256"
+    RSA3072_PSS_SHA256 = "RSA-PSS-3072-SHA256"
+    RSA4096_PSS_SHA256 = "RSA-PSS-4096-SHA256"
+    RSA4096_PSS_SHA512 = "RSA-PSS-4096-SHA512"
     RSA = "RSA-PKCS1V15-2048-SHA256"  # deprecated, use RSA2048_PKCS1V15_SHA256 instead
 
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return str(self.value)
@@ -48,14 +61,15 @@
 
 class SymmetricAlgorithm(str, enum.Enum):
     HS256 = "HS256"
     HS384 = "HS384"
     HS512 = "HS512"
     AES128_CFB = "AES-CFB-128"
     AES256_CFB = "AES-CFB-256"
+    AES256_GCM = "AES-GCM-256"
     AES = "AES-CFB-128"  # deprecated, use AES128_CFB instead
 
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return str(self.value)
```

### Comparing `pangea_sdk-1.8.0/pangea/services/vault/models/symmetric.py` & `pangea_sdk-1.9.0/pangea/services/vault/models/symmetric.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,27 +35,29 @@
     purpose: str
 
 
 class EncryptRequest(APIRequestModel):
     id: str
     plain_text: str
     version: Optional[int] = None
+    additional_data: Optional[str]
 
 
 class EncryptResult(PangeaResponseResult):
     id: str
     version: int
     algorithm: str
     cipher_text: str
 
 
 class DecryptRequest(APIRequestModel):
     id: str
     cipher_text: str
     version: Optional[int] = None
+    additional_data: Optional[str]
 
 
 class DecryptResult(PangeaResponseResult):
     id: str
     version: int
     algorithm: str
     plain_text: str
```

### Comparing `pangea_sdk-1.8.0/pangea/services/vault/vault.py` & `pangea_sdk-1.9.0/pangea/services/vault/vault.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         vault_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea Vault service
         vault = Vault(token=PANGEA_VAULT_TOKEN, config=audit_config)
     """
 
     service_name: str = "vault"
-    version: str = "v1"
 
     def __init__(
         self,
         token,
         config=None,
         logger_name="pangea",
     ):
@@ -102,15 +101,17 @@
 
     # Delete endpoint
     def delete(self, id: str) -> PangeaResponse[DeleteResult]:
         """
         Delete
 
         Delete a secret or key
-        
+
+        OperationId: vault_post_v1_delete
+
         Args:
             id (str): The item ID
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the id of the deleted secret or key
@@ -119,15 +120,15 @@
 
         Examples:
             vault.delete(id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5")
         """
         input = DeleteRequest(
             id=id,
         )
-        response = self.request.post("delete", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/delete", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = DeleteResult(**response.raw_result)
         return response
 
     # Get endpoint
     def get(
         self,
@@ -136,46 +137,48 @@
         version_state: Optional[ItemVersionState] = None,
         verbose: Optional[bool] = None,
     ) -> PangeaResponse[GetResult]:
         """
         Retrieve
 
         Retrieve a secret or key, and any associated information
-        
+
+        OperationId: vault_post_v1_get
+
         Args:
             id (str): The item ID
-            version (str, int, optional): The key version(s). 
+            version (str, int, optional): The key version(s).
                 - `all` for all versions
                 - `num` for a specific version
                 - `-num` for the `num` latest versions
             version_state (ItemVersionState, optional): The state of the item version
             verbose (bool, optional): Return metadata and extra fields. Default is `False`.
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the secret or key
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#retrieve).
 
         Examples:
-            vault.get(
+            response = vault.get(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 version=1,
                 version_state=ItemVersionState.ACTIVE,
                 verbose=True,
             )
         """
         input = GetRequest(
             id=id,
             version=version,
             verbose=verbose,
             version_state=version_state,
         )
-        response = self.request.post("get", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/get", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = GetResult(**response.raw_result)
         return response
 
     # List endpoint
     def list(
         self,
@@ -185,15 +188,17 @@
         order_by: Optional[ItemOrderBy] = None,
         size: Optional[int] = None,
     ) -> PangeaResponse[ListResult]:
         """
         List
 
         Look up a list of secrets, keys and folders, and their associated information
-        
+
+        OperationId: vault_post_v1_list
+
         Args:
             filter (dict, optional): A set of filters to help you customize your search. Examples:
                 - "folder": "/tmp"
                 - "tags": "personal"
                 - "name__contains": "xxx"
                 - "created_at__gt": "2020-02-05T10:00:00Z"
 
@@ -209,30 +214,30 @@
 
         Returns:
             A PangeaResponse where a list of secrets or keys
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#list).
 
         Examples:
-            vault.list(
+            response = vault.list(
                 filter={
                     "folder": "/",
                     "type": "asymmetric_key",
                     "name__contains": "test",
                     "metadata_key1": "value1",
                     "created_at__lt": "2023-12-12T00:00:00Z"
                 },
                 last="WyIvdGVzdF8yMDdfc3ltbWV0cmljLyJd",
                 order=ItemOrder.ASC,
                 order_by=ItemOrderBy.NAME,
                 size=20,
             )
         """
         input = ListRequest(filter=filter, last=last, order=order, order_by=order_by, size=size)
-        response = self.request.post("list", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/list", data=input.dict(exclude_none=True))
 
         if response.raw_result is not None:
             response.result = ListResult(**response.raw_result)
         return response
 
     # Update endpoint
     def update(
@@ -248,15 +253,17 @@
         expiration: Optional[datetime.datetime] = None,
         item_state: Optional[ItemState] = None,
     ) -> PangeaResponse[UpdateResult]:
         """
         Update
 
         Update information associated with a secret or key.
-        
+
+        OperationId: vault_post_v1_update
+
         Args:
             id (str): The item ID
             name (str, optional): The name of this item
             folder (string, optional): The folder where this item is stored
             metadata (dict, optional): User-provided metadata
             tags (list[str], optional): A list of user-defined tags
             rotation_frequency (str, optional): Period of time between item rotations
@@ -276,15 +283,15 @@
 
         Returns:
             A PangeaResponse where the item ID
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#update).
 
         Examples:
-            vault.update(
+            response = vault.update(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
                     "created_by": "John Doe",
                     "used_in": "Google products"
                 },
@@ -307,15 +314,15 @@
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             rotation_grace_period=rotation_grace_period,
             expiration=expiration,
             item_state=item_state,
         )
-        response = self.request.post("update", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/update", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = UpdateResult(**response.raw_result)
         return response
 
     def secret_store(
         self,
         secret: str,
@@ -327,15 +334,17 @@
         rotation_state: Optional[ItemVersionState] = None,
         expiration: Optional[datetime.datetime] = None,
     ) -> PangeaResponse[SecretStoreResult]:
         """
         Secret store
 
         Import a secret
-        
+
+        OperationId: vault_post_v1_secret_store 1
+
         Args:
             secret (str): The secret value
             name (str): The name of this item
             folder (str, optional): The folder where this item is stored
             metadata (dict, optional): User-provided metadata
             tags (list[str], optional): A list of user-defined tags
             rotation_frequency (str, optional): Period of time between item rotations
@@ -350,15 +359,15 @@
 
         Returns:
             A PangeaResponse where the secret
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#import-a-secret).
 
         Examples:
-            vault.secret_store(
+            response = vault.secret_store(
                 secret="12sdfgs4543qv@#%$casd",
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
                     "created_by": "John Doe",
                     "used_in": "Google products"
                 },
@@ -378,15 +387,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("secret/store", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/secret/store", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SecretStoreResult(**response.raw_result)
         return response
 
     def pangea_token_store(
         self,
         pangea_token: str,
@@ -398,38 +407,40 @@
         rotation_state: Optional[ItemVersionState] = None,
         expiration: Optional[datetime.datetime] = None,
     ) -> PangeaResponse[SecretStoreResult]:
         """
         Pangea token store
 
         Import a secret
-        
+
+        OperationId: vault_post_v1_secret_store 2
+
         Args:
             pangea_token (str): The pangea token to store
             name (str): the name of this item
             folder (str, optional): The folder where this item is stored
             metadata (dict, optional): User-provided metadata
             tags (list[str], optional): A list of user-defined tags
             rotation_frequency (str, optional): Period of time between item rotations
-            rotation_state (ItemVersionState, optional): State to which the previous version should 
+            rotation_state (ItemVersionState, optional): State to which the previous version should
                 transition upon rotation. Supported options:
                 - `deactivated`
                 - `destroyed`
             expiration (str, optional): Expiration timestamp
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the token
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#import-a-secret).
 
         Examples:
-            vault.pangea_token_store(
+            response = vault.pangea_token_store(
                 pangea_token="ptv_x6fdiizbon6j3bsdvnpmwxsz2aan7fqd",
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
                     "created_by": "John Doe",
                     "used_in": "Google products"
                 },
@@ -449,28 +460,30 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("secret/store", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/secret/store", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SecretStoreResult(**response.raw_result)
         return response
 
     # Rotate endpoint
     def secret_rotate(
         self, id: str, secret: str, rotation_state: Optional[ItemVersionState] = None
     ) -> PangeaResponse[SecretRotateResult]:
         """
         Secret rotate
 
         Rotate a secret
-        
+
+        OperationId: vault_post_v1_secret_rotate 1
+
         Args:
             id (str): The item ID
             secret (str): The secret value
             rotation_state (ItemVersionState, optional): State to which the previous version should transition upon rotation.
                 Supported options:
                 - `deactivated`
                 - `suspended`
@@ -483,51 +496,53 @@
 
         Returns:
             A PangeaResponse where the secret
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#rotate-a-secret).
 
         Examples:
-            vault.secret_rotate(
+            response = vault.secret_rotate(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 secret="12sdfgs4543qv@#%$casd",
                 rotation_state=ItemVersionState.DEACTIVATED,
             )
         """
         input = SecretRotateRequest(id=id, secret=secret, rotation_state=rotation_state)
-        response = self.request.post("secret/rotate", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/secret/rotate", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SecretRotateResult(**response.raw_result)
         return response
 
     # Rotate endpoint
     def pangea_token_rotate(self, id: str) -> PangeaResponse[SecretRotateResult]:
         """
         Token rotate
 
         Rotate a Pangea token
-        
+
+        OperationId: vault_post_v1_secret_rotate 2
+
         Args:
             id (str): The item ID
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the token
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#rotate-a-secret).
 
         Examples:
-            vault.pangea_token_rotate(
+            response = vault.pangea_token_rotate(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
             )
         """
         input = SecretRotateRequest(id=id)
-        response = self.request.post("secret/rotate", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/secret/rotate", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SecretRotateResult(**response.raw_result)
         return response
 
     def symmetric_generate(
         self,
         algorithm: SymmetricAlgorithm,
@@ -540,15 +555,17 @@
         rotation_state: Optional[ItemVersionState] = None,
         expiration: Optional[datetime.datetime] = None,
     ) -> PangeaResponse[SymmetricGenerateResult]:
         """
         Symmetric generate
 
         Generate a symmetric key
-        
+
+        OperationId: vault_post_v1_key_generate 1
+
         Args:
             algorithm (SymmetricAlgorithm): The algorithm of the key
             purpose (KeyPurpose): The purpose of this key
             name (str): The name of this item
             folder (str, optional): The folder where this item is stored
             metadata (dict, optional): User-provided metadata
             tags (list[str], optional): A list of user-defined tags
@@ -564,15 +581,15 @@
 
         Returns:
             A PangeaResponse where the ID of the key
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#generate).
 
         Examples:
-            vault.symmetric_generate(
+            response = vault.symmetric_generate(
                 algorithm=SymmetricAlgorithm.AES,
                 purpose=KeyPurpose.ENCRYPTION,
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
                     "created_by": "John Doe",
                     "used_in": "Google products"
@@ -594,15 +611,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("key/generate", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/generate", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SymmetricGenerateResult(**response.raw_result)
         return response
 
     def asymmetric_generate(
         self,
         algorithm: AsymmetricAlgorithm,
@@ -615,15 +632,17 @@
         rotation_state: Optional[ItemVersionState] = None,
         expiration: Optional[datetime.datetime] = None,
     ) -> PangeaResponse[AsymmetricGenerateResult]:
         """
         Asymmetric generate
 
         Generate an asymmetric key
-        
+
+        OperationId: vault_post_v1_key_generate 2
+
         Args:
             algorithm (AsymmetricAlgorithm): The algorithm of the key
             purpose (KeyPurpose): The purpose of this key
             name (str): The name of this item
             folder (str, optional): The folder where this item is stored
             metadata (dict, optional): User-provided metadata
             tags (list[str], optional): A list of user-defined tags
@@ -639,15 +658,15 @@
 
         Returns:
             A PangeaResponse where the ID of the key
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#generate).
 
         Examples:
-            vault.asymmetric_generate(
+            response = vault.asymmetric_generate(
                 algorithm=AsymmetricAlgorithm.RSA,
                 purpose=KeyPurpose.SIGNING,
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
                     "created_by": "John Doe",
                     "used_in": "Google products"
@@ -669,15 +688,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("key/generate", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/generate", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = AsymmetricGenerateResult(**response.raw_result)
         return response
 
     # Store endpoints
     def asymmetric_store(
         self,
@@ -693,15 +712,17 @@
         rotation_state: Optional[ItemVersionState] = None,
         expiration: Optional[datetime.datetime] = None,
     ) -> PangeaResponse[AsymmetricStoreResult]:
         """
         Asymmetric store
 
         Import an asymmetric key
-        
+
+        OperationId: vault_post_v1_key_store 1
+
         Args:
             private_key (EncodedPrivateKey): The private key in PEM format
             public_key (EncodedPublicKey): The public key in PEM format
             algorithm (AsymmetricAlgorithm): The algorithm of the key
             purpose (KeyPurpose): The purpose of this key. `signing`, `encryption`, or `jwt`.
             name (str): The name of this item
             folder (str, optional): The folder where this item is stored
@@ -719,15 +740,15 @@
 
         Returns:
             A PangeaResponse where the ID and public key
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#import-a-key).
 
         Examples:
-            vault.asymmetric_store(
+            response = vault.asymmetric_store(
                 private_key="private key example",
                 public_key="-----BEGIN PUBLIC KEY-----\\nMCowBQYDK2VwAyEA8s5JopbEPGBylPBcMK+L5PqHMqPJW/5KYPgBHzZGncc=\\n-----END PUBLIC KEY-----",
                 algorithm="AsymmetricAlgorithm.RSA,
                 purpose=KeyPurpose.SIGNING,
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
@@ -753,15 +774,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("key/store", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/store", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = AsymmetricStoreResult(**response.raw_result)
         return response
 
     def symmetric_store(
         self,
         key: str,
@@ -775,15 +796,17 @@
         rotation_state: Optional[ItemVersionState] = None,
         expiration: Optional[datetime.datetime] = None,
     ) -> PangeaResponse[SymmetricStoreResult]:
         """
         Symmetric store
 
         Import a symmetric key
-        
+
+        OperationId: vault_post_v1_key_store 2
+
         Args:
             key (str): The key material (in base64)
             algorithm (SymmetricAlgorithm): The algorithm of the key
             purpose (KeyPurpose): The purpose of this key. `encryption` or `jwt`
             name (str): The name of this item
             folder (str, optional): The folder where this item is stored
             metadata (dict, optional): User-provided metadata
@@ -800,15 +823,15 @@
 
         Returns:
             A PangeaResponse where the ID
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#import-a-key).
 
         Examples:
-            vault.symmetric_store(
+            response = vault.symmetric_store(
                 key="lJkk0gCLux+Q+rPNqLPEYw==",
                 algorithm=SymmetricAlgorithm.AES,
                 purpose=KeyPurpose.ENCRYPTION,
                 name="my-very-secret-secret",
                 folder="/personal",
                 metadata={
                     "created_by": "John Doe",
@@ -832,15 +855,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("key/store", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/store", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SymmetricStoreResult(**response.raw_result)
         return response
 
     # Rotate endpoint
     def key_rotate(
         self,
@@ -850,15 +873,17 @@
         private_key: Optional[EncodedPrivateKey] = None,
         key: Optional[EncodedSymmetricKey] = None,
     ) -> PangeaResponse[KeyRotateResult]:
         """
         Key rotate
 
         Manually rotate a symmetric or asymmetric key
-        
+
+        OperationId: vault_post_v1_key_rotate
+
         Args:
             id (str): The ID of the item
             rotation_state (ItemVersionState, optional): State to which the previous version should transition upon rotation.
                 Supported options:
                 - `deactivated`
                 - `suspended`
                 - `destroyed`
@@ -873,136 +898,144 @@
 
         Returns:
             A PangeaResponse where the ID
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#rotate).
 
         Examples:
-            vault.key_rotate(
+            response = vault.key_rotate(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 rotation_state=ItemVersionState.DEACTIVATED,
                 key="lJkk0gCLux+Q+rPNqLPEYw==",
             )
         """
         input = KeyRotateRequest(
             id=id, public_key=public_key, private_key=private_key, key=key, rotation_state=rotation_state
         )
-        response = self.request.post("key/rotate", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/rotate", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = KeyRotateResult(**response.raw_result)
         return response
 
     # Encrypt
     def encrypt(self, id: str, plain_text: str, version: Optional[int] = None) -> PangeaResponse[EncryptResult]:
         """
         Encrypt
 
         Encrypt a message using a key
-        
+
+        OperationId: vault_post_v1_key_encrypt
+
         Args:
             id (str): The item ID
             plain_text (str): A message to be in encrypted (in base64)
             version (int, optional): The item version
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the encrypted message in base64
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#encrypt).
 
         Examples:
-            vault.encrypt(
+            response = vault.encrypt(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 plain_text="lJkk0gCLux+Q+rPNqLPEYw==",
                 version=1,
             )
         """
         input = EncryptRequest(id=id, plain_text=plain_text, version=version)
-        response = self.request.post("key/encrypt", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/encrypt", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = EncryptResult(**response.raw_result)
         return response
 
     # Decrypt
     def decrypt(self, id: str, cipher_text: str, version: Optional[int] = None) -> PangeaResponse[DecryptResult]:
         """
         Decrypt
 
         Decrypt a message using a key
-        
+
+        OperationId: vault_post_v1_key_decrypt
+
         Args:
             id (str): The item ID
             cipher_text (str): A message encrypted by Vault (in base64)
             version (int, optional): The item version
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the decrypted message in base64
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#decrypt).
 
         Examples:
-            vault.decrypt(
+            response = vault.decrypt(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 cipher_text="lJkk0gCLux+Q+rPNqLPEYw==",
                 version=1,
             )
         """
         input = DecryptRequest(id=id, cipher_text=cipher_text, version=version)
-        response = self.request.post("key/decrypt", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/decrypt", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = DecryptResult(**response.raw_result)
         return response
 
     # Sign
     def sign(self, id: str, message: str, version: Optional[int] = None) -> PangeaResponse[SignResult]:
         """
         Sign
 
         Sign a message using a key
-        
+
+        OperationId: vault_post_v1_key_sign
+
         Args:
             id (str): The item ID
             message (str): The message to be signed, in base64
             version (int, optional): The item version
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the signature of the message in base64
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#sign).
 
         Examples:
-            vault.sign(
+            response = vault.sign(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 message="lJkk0gCLux+Q+rPNqLPEYw==",
                 version=1,
             )
         """
         input = SignRequest(id=id, message=message, version=version)
-        response = self.request.post("key/sign", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/sign", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = SignResult(**response.raw_result)
         return response
 
     # Verify
     def verify(
         self, id: str, message: str, signature: str, version: Optional[int] = None
     ) -> PangeaResponse[VerifyResult]:
         """
         Verify
 
         Verify a signature using a key
-        
+
+        OperationId: vault_post_v1_key_verify
+
         Args:
             id (str): The item ID
             message (str): A message to be verified (in base64)
             signature (str): The message signature (in base64)
             version (int, optional): The item version
 
         Raises:
@@ -1010,97 +1043,103 @@
 
         Returns:
             A PangeaResponse where the signature is valid
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#verify).
 
         Examples:
-            vault.verify(
+            response = vault.verify(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 message="lJkk0gCLux+Q+rPNqLPEYw==",
                 signature="FfWuT2Mq/+cxa7wIugfhzi7ktZxVf926idJNgBDCysF/knY9B7M6wxqHMMPDEBs86D8OsEGuED21y3J7IGOpCQ==",
                 version=1,
             )
         """
         input = VerifyRequest(
             id=id,
             message=message,
             signature=signature,
             version=version,
         )
-        response = self.request.post("key/verify", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/verify", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = VerifyResult(**response.raw_result)
         return response
 
     def jwt_verify(self, jws: str) -> PangeaResponse[JWTVerifyResult]:
         """
         JWT Verify
 
         Verify the signature of a JSON Web Token (JWT)
-        
+
+        OperationId: vault_post_v1_key_verify_jwt
+
         Args:
             jws (str): The signed JSON Web Token (JWS)
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the signature is valid
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#verify-jwt).
 
         Examples:
-            vault.jwt_verify(
-                jws="ewogICJhbGciO..."
+            response = vault.jwt_verify(
+                jws="ewogICJhbGciO...",
             )
         """
         input = JWTVerifyRequest(jws=jws)
-        response = self.request.post("key/verify/jwt", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/verify/jwt", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = JWTVerifyResult(**response.raw_result)
         return response
 
     def jwt_sign(self, id: str, payload: str) -> PangeaResponse[JWTSignResult]:
         """
         JWT Sign
 
         Sign a JSON Web Token (JWT) using a key
-        
+
+        OperationId: vault_post_v1_key_sign_jwt
+
         Args:
             id (str): The item ID
             payload (str): The JWT payload (in JSON)
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the signed JSON Web Token (JWS)
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#sign-a-jwt).
 
         Examples:
-            vault.jwt_sign(
+            response = vault.jwt_sign(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 payload="{\\"sub\\": \\"1234567890\\",\\"name\\": \\"John Doe\\",\\"admin\\": true}"
             )
         """
         input = JWTSignRequest(id=id, payload=payload)
-        response = self.request.post("key/sign/jwt", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/key/sign/jwt", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = JWTSignResult(**response.raw_result)
         return response
 
     # Get endpoint
     def jwk_get(self, id: str, version: Optional[str] = None) -> PangeaResponse[JWKGetResult]:
         """
         JWT Retrieve
 
         Retrieve a key in JWK format
-        
+
+        OperationId: vault_post_v1_get_jwk
+
         Args:
             id (str): The item ID
             version (str, optional): The key version(s).
                 - `all` for all versions
                 - `num` for a specific version
                 - `-num` for the `num` latest versions
         Raises:
@@ -1108,56 +1147,58 @@
 
         Returns:
             A PangeaResponse where the JSON Web Key Set (JWKS) object
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#retrieve-jwk").
 
         Examples:
-            vault.jwk_get(
+            response = vault.jwk_get(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
             )
         """
         input = JWKGetRequest(id=id, version=version)
-        response = self.request.post("get/jwk", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/get/jwk", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = JWKGetResult(**response.raw_result)
         return response
 
     # State change
     def state_change(
         self, id: str, state: ItemVersionState, version: Optional[int] = None, destroy_period: Optional[str] = None
     ) -> PangeaResponse[StateChangeResult]:
         """
         State change
 
         Change the state of a specific version of a secret or key
-        
+
+        OperationId: vault_post_v1_state_change
+
         Args:
             id (str): The item ID
             state (ItemVersionState): The new state of the item version. Supported options:
                 - `active`
                 - `deactivated`
                 - `suspended`
                 - `compromised`
                 - `destroyed`
             version (int, optional): the item version
-            destroy_period (str, optional): Period of time for the destruction of a compromised key. 
+            destroy_period (str, optional): Period of time for the destruction of a compromised key.
                 Only valid if state=`compromised`
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             A PangeaResponse where the state change object
                 is returned in the response.result field.
                 Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/vault#change-state").
 
         Examples:
-            vault.state_change(
+            response = vault.state_change(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 state=ItemVersionState.DEACTIVATED,
             )
         """
         input = StateChangeRequest(id=id, state=state, version=version, destroy_period=destroy_period)
-        response = self.request.post("state/change", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/state/change", data=input.dict(exclude_none=True))
         if response.raw_result is not None:
             response.result = StateChangeResult(**response.raw_result)
         return response
```

### Comparing `pangea_sdk-1.8.0/pangea/tools.py` & `pangea_sdk-1.9.0/pangea/tools.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/utils.py` & `pangea_sdk-1.9.0/pangea/utils.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.8.0/pangea/verify_audit.py` & `pangea_sdk-1.9.0/pangea/verify_audit.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,31 +194,31 @@
             logger.debug(str(e))
 
     log_result("Consistency proof verification", succeeded)
     logger.info("")
     return succeeded
 
 
-def create_signed_envelope(event: t.Dict) -> t.Dict:
+def create_signed_event(event: t.Dict) -> t.Dict:
     return {k: v for k, v in event.items() if v is not None}
 
 
 def _verify_signature(data: t.Dict) -> t.Optional[bool]:
     log_section("Checking signature")
     if "signature" not in data:
         logger.debug("Signature is not present")
         succeeded = None
     else:
         try:
             logger.debug("Obtaining signature and public key from the event")
-            sign_envelope = create_signed_envelope(data["event"])
+            sign_event = create_signed_event(data["event"])
             public_key = get_public_key(data["public_key"])
             sign_verifier = Verifier()
             logger.debug("Checking the signature")
-            if not sign_verifier.verifyMessage(data["signature"], sign_envelope, public_key):
+            if not sign_verifier.verify_signature(data["signature"], canonicalize_json(sign_event), public_key):
                 raise ValueError("Signature is invalid")
             succeeded = True
         except Exception:
             succeeded = False
 
     log_result("Data signature verification", succeeded)
     logger.info("")
```

### Comparing `pangea_sdk-1.8.0/pyproject.toml` & `pangea_sdk-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pangea-sdk"
-version = "1.8.0"
+version = "1.9.0"
 description = "Pangea API SDK"
 authors = ["Glenn Gallien <glenn.gallien@pangea.cloud>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = ""
 keywords = ["Pangea", "SDK", "Audit"]
```

### Comparing `pangea_sdk-1.8.0/PKG-INFO` & `pangea_sdk-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangea-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Pangea API SDK
 License: MIT
 Keywords: Pangea,SDK,Audit
 Author: Glenn Gallien
 Author-email: glenn.gallien@pangea.cloud
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

