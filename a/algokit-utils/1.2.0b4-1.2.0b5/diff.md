# Comparing `tmp/algokit_utils-1.2.0b4-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 34345 bytes, number of entries: 15
+Zip file size: 34605 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    54130 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    54567 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
--rw-r--r--  2.0 unx     2000 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
+-rw-r--r--  2.0 unx     2475 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2038 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/RECORD
-15 files, 132380 bytes uncompressed, 32253 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2038 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/RECORD
+15 files, 133292 bytes uncompressed, 32513 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b4.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b5.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b4.dist-info/METADATA
+Filename: algokit_utils-1.2.0b5.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b4.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b5.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b4.dist-info/RECORD
+Filename: algokit_utils-1.2.0b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -158,18 +158,18 @@
         """
         self.algod_client = algod_client
         self.app_spec = (
             au_spec.ApplicationSpecification.from_json(app_spec.read_text()) if isinstance(app_spec, Path) else app_spec
         )
         self._app_name = app_name
         self._approval_program: Program | None = None
+        self._approval_source_map: SourceMap | None = None
         self._clear_program: Program | None = None
 
         self.template_values: au_deploy.TemplateValueMapping = template_values or {}
-        self.approval_source_map: SourceMap | None = None
         self.existing_deployments = existing_deployments
         self._indexer_client = indexer_client
         if creator is not None:
             if not self.existing_deployments and not self._indexer_client:
                 raise Exception(
                     "If using the creator parameter either existing_deployments or indexer_client must also be provided"
                 )
@@ -211,14 +211,26 @@
         return get_application_address(self.app_id)
 
     @property
     def approval(self) -> Program | None:
         return self._approval_program
 
     @property
+    def approval_source_map(self) -> SourceMap | None:
+        if self._approval_source_map:
+            return self._approval_source_map
+        if self._approval_program:
+            return self._approval_program.source_map
+        return None
+
+    @approval_source_map.setter
+    def approval_source_map(self, value: SourceMap) -> None:
+        self._approval_source_map = value
+
+    @property
     def clear(self) -> Program | None:
         return self._clear_program
 
     def prepare(
         self,
         signer: TransactionSigner | Account | None = None,
         sender: str | None = None,
@@ -296,15 +308,15 @@
         has increased beyond the current allocation
         :param dict[str, int|str|bytes] template_values: Values to use for `TMPL_*` template variables, dictionary keys
         should *NOT* include the TMPL_ prefix
         :param ABICreateCallArgs create_args: Arguments used when creating an application
         :param ABICallArgs | ABICallArgsDict update_args: Arguments used when updating an application
         :param ABICallArgs | ABICallArgsDict delete_args: Arguments used when deleting an application
         :return DeployResponse: details action taken and relevant transactions
-        :raises DeploymentError: If the deployment failed due
+        :raises DeploymentError: If the deployment failed
         """
         # check inputs
         if self.app_id:
             raise au_deploy.DeploymentFailedError(
                 f"Attempt to deploy app which already has an app index of {self.app_id}"
             )
         try:
@@ -606,17 +618,17 @@
             **abi_kwargs,
         )
 
         method = self._resolve_method(
             call_abi_method, abi_kwargs, _parameters.on_complete or transaction.OnComplete.NoOpOC
         )
         if method:
-            response = self._try_simulate_call(method, atc)
-            if response:
-                return response
+            hints = self._method_hints(method)
+            if hints and hints.read_only:
+                return self._simulate_readonly_call(method, atc)
 
         return self._execute_atc_tr(atc)
 
     def compose_opt_in(
         self,
         atc: AtomicTransactionComposer,
         /,
@@ -845,31 +857,28 @@
     def _check_is_compiled(self) -> tuple[Program, Program]:
         if self._approval_program is None or self._clear_program is None:
             self._approval_program, self._clear_program = substitute_template_and_compile(
                 self.algod_client, self.app_spec, self.template_values
             )
         return self._approval_program, self._clear_program
 
-    def _try_simulate_call(
+    def _simulate_readonly_call(
         self, method: Method, atc: AtomicTransactionComposer
-    ) -> ABITransactionResponse | TransactionResponse | None:
-        hints = self._method_hints(method)
-        if hints and hints.read_only:
-            simulate_response = atc.simulate(self.algod_client)
-            if not simulate_response.would_succeed:
-                raise _try_convert_to_logic_error(
-                    simulate_response.failure_message,
-                    self.app_spec.approval_program,
-                    self._get_approval_source_map(),
-                ) or Exception(
-                    f"Simulate failed for readonly method {method.get_signature()}: {simulate_response.failure_message}"
-                )
+    ) -> ABITransactionResponse | TransactionResponse:
+        simulate_response = atc.simulate(self.algod_client)
+        if simulate_response.failure_message:
+            raise _try_convert_to_logic_error(
+                simulate_response.failure_message,
+                self.app_spec.approval_program,
+                self._get_approval_source_map,
+            ) or Exception(
+                f"Simulate failed for readonly method {method.get_signature()}: {simulate_response.failure_message}"
+            )
 
-            return TransactionResponse.from_atr(simulate_response)
-        return None
+        return TransactionResponse.from_atr(simulate_response)
 
     def _load_reference_and_check_app_id(self) -> None:
         self._load_app_reference()
         self._check_app_id()
 
     def _load_app_reference(self) -> au_deploy.AppReference | au_deploy.AppMetaData:
         if not self.existing_deployments and self._creator:
@@ -928,18 +937,22 @@
             )
         else:  # no match
             raise Exception(
                 f"Could not find any methods to use for {on_complete.name} with call_config of {call_config.name}"
             )
 
     def _get_approval_source_map(self) -> SourceMap | None:
-        if self.approval:
-            return self.approval.source_map
+        if self.approval_source_map:
+            return self.approval_source_map
 
-        return self.approval_source_map
+        try:
+            approval, _ = self._check_is_compiled()
+        except au_deploy.DeploymentFailedError:
+            return None
+        return approval.source_map
 
     def add_method_call(
         self,
         atc: AtomicTransactionComposer,
         abi_method: ABIMethod | bool | None = None,
         *,
         abi_args: ABIArgsDict | None = None,
@@ -1100,15 +1113,15 @@
         return TransactionResponse.from_atr(result)
 
     def execute_atc(self, atc: AtomicTransactionComposer) -> AtomicTransactionResponse:
         return execute_atc_with_logic_error(
             atc,
             self.algod_client,
             approval_program=self.app_spec.approval_program,
-            approval_source_map=self._get_approval_source_map(),
+            approval_source_map=self._get_approval_source_map,
         )
 
     def get_signer_sender(
         self, signer: TransactionSigner | None = None, sender: str | None = None
     ) -> tuple[TransactionSigner | None, str | None]:
         """Return signer and sender, using default values on client if not specified
 
@@ -1183,37 +1196,37 @@
     raise au_deploy.DeploymentFailedError(
         f"Could not auto increment {current_version}, please specify the next version using the version parameter"
     )
 
 
 def _try_convert_to_logic_error(
     source_ex: Exception | str,
-    approval_program: str | None = None,
-    approval_source_map: SourceMap | None = None,
+    approval_program: str,
+    approval_source_map: SourceMap | typing.Callable[[], SourceMap | None] | None = None,
 ) -> Exception | None:
-    if approval_source_map and approval_program:
-        source_ex_str = str(source_ex)
-        logic_error_data = parse_logic_error(source_ex_str)
-        if logic_error_data is not None:
-            return LogicError(
-                logic_error_str=source_ex_str,
-                logic_error=source_ex if isinstance(source_ex, Exception) else None,
-                program=approval_program,
-                source_map=approval_source_map,
-                **logic_error_data,
-            )
+    source_ex_str = str(source_ex)
+    logic_error_data = parse_logic_error(source_ex_str)
+    if logic_error_data:
+        return LogicError(
+            logic_error_str=source_ex_str,
+            logic_error=source_ex if isinstance(source_ex, Exception) else None,
+            program=approval_program,
+            source_map=approval_source_map() if callable(approval_source_map) else approval_source_map,
+            **logic_error_data,
+        )
+
     return None
 
 
 def execute_atc_with_logic_error(
     atc: AtomicTransactionComposer,
     algod_client: "AlgodClient",
+    approval_program: str,
     wait_rounds: int = 4,
-    approval_program: str | None = None,
-    approval_source_map: SourceMap | None = None,
+    approval_source_map: SourceMap | typing.Callable[[], SourceMap | None] | None = None,
 ) -> AtomicTransactionResponse:
     """Calls {py:meth}`AtomicTransactionComposer.execute` on provided `atc`, but will parse any errors
     and raise a {py:class}`LogicError` if possible
 
     ```{note}
     `approval_program` and `approval_source_map` are required to be able to parse any errors into a
     {py:class}`LogicError`
```

## algokit_utils/logic_error.py

```diff
@@ -38,37 +38,44 @@
 
 class LogicError(Exception):
     def __init__(
         self,
         *,
         logic_error_str: str,
         program: str,
-        source_map: "AlgoSourceMap",
+        source_map: "AlgoSourceMap | None",
         transaction_id: str,
         message: str,
         pc: int,
         logic_error: Exception | None = None,
     ):
         self.logic_error = logic_error
         self.logic_error_str = logic_error_str
         self.program = program
         self.source_map = source_map
         self.lines = program.split("\n")
         self.transaction_id = transaction_id
         self.message = message
         self.pc = pc
 
-        line = self.source_map.get_line_for_pc(self.pc)
-        self.line_no = line if line is not None else 0
+        self.line_no = self.source_map.get_line_for_pc(self.pc) if self.source_map else None
 
     def __str__(self) -> str:
         return (
-            f"Txn {self.transaction_id} had error '{self.message}' at PC {self.pc} and Source Line {self.line_no}: "
-            f"\n\n\t{self.trace()}"
+            f"Txn {self.transaction_id} had error '{self.message}' at PC {self.pc}"
+            + (":" if self.line_no is None else f" and Source Line {self.line_no}:")
+            + f"\n{self.trace()}"
         )
 
     def trace(self, lines: int = 5) -> str:
+        if self.line_no is None:
+            return """
+Could not determine TEAL source line for the error as no approval source map was provided, to receive a trace of the
+error please provide an approval SourceMap. Either by:
+    1.) Providing template_values when creating the ApplicationClient, so a SourceMap can be obtained automatically OR
+    2.) Set approval_source_map from a previously compiled approval program"""
+
         program_lines = copy(self.lines)
         program_lines[self.line_no] += "\t\t<-- Error"
         lines_before = max(0, self.line_no - lines)
         lines_after = min(len(program_lines), self.line_no + lines)
-        return "\n\t".join(program_lines[lines_before:lines_after])
+        return "\n\t" + "\n\t".join(program_lines[lines_before:lines_after])
```

## Comparing `algokit_utils-1.2.0b4.dist-info/LICENSE` & `algokit_utils-1.2.0b5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b4.dist-info/METADATA` & `algokit_utils-1.2.0b5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b4
+Version: 1.2.0b5
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.2.0b4.dist-info/RECORD` & `algokit_utils-1.2.0b5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 algokit_utils/__init__.py,sha256=wuh-p9PubCj9Bj2tpxP3tQ5qZPs_nUHzB16BHi9Aq2c,4091
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
-algokit_utils/application_client.py,sha256=zeoPAIYhUq2PLrWzRmLFGjVyFFcpYiXekJ3t_sPqlpM,54130
+algokit_utils/application_client.py,sha256=EH3UoVoo56Vmg6_ji96IvYIJSzFAe96OfeGsDzI1T1w,54567
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
-algokit_utils/logic_error.py,sha256=IxsAGS11kuFhPhEHvhheZamQ2KQxb3LQdxiTOvnKKAA,2000
+algokit_utils/logic_error.py,sha256=-04aGw8OG4wY3T42mKU6TezNlkxjtMr6CtHVDWLpS5s,2475
 algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b4.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b4.dist-info/METADATA,sha256=2QI6lw0DKnJwcJhTw-E51sTmgmbS8L4foQbexmhKMo0,2038
-algokit_utils-1.2.0b4.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_utils-1.2.0b4.dist-info/RECORD,,
+algokit_utils-1.2.0b5.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b5.dist-info/METADATA,sha256=hOL2d9pwN66F9-5THnKOveGrHd2GRhznRUaU3M7UwTw,2038
+algokit_utils-1.2.0b5.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_utils-1.2.0b5.dist-info/RECORD,,
```

