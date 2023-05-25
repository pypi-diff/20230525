# Comparing `tmp/pytket_qir-0.2.0rc6-py3-none-any.whl.zip` & `tmp/pytket_qir-0.2.0rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17668 bytes, number of entries: 12
--rw-r--r--  2.0 unx      862 b- defN 23-May-24 09:31 pytket/qir/__init__.py
--rw-r--r--  2.0 unx       69 b- defN 23-May-24 09:32 pytket/qir/_metadata.py
--rw-r--r--  2.0 unx      715 b- defN 23-May-24 09:31 pytket/qir/conversion/__init__.py
--rw-r--r--  2.0 unx     2519 b- defN 23-May-24 09:31 pytket/qir/conversion/api.py
--rw-r--r--  2.0 unx    27612 b- defN 23-May-24 09:31 pytket/qir/conversion/conversion.py
--rw-r--r--  2.0 unx     4082 b- defN 23-May-24 09:31 pytket/qir/conversion/gatesets.py
--rw-r--r--  2.0 unx     1481 b- defN 23-May-24 09:31 pytket/qir/conversion/module.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-24 09:32 pytket_qir-0.2.0rc6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4183 b- defN 23-May-24 09:32 pytket_qir-0.2.0rc6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 09:32 pytket_qir-0.2.0rc6.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-24 09:32 pytket_qir-0.2.0rc6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1017 b- defN 23-May-24 09:32 pytket_qir-0.2.0rc6.dist-info/RECORD
-12 files, 53996 bytes uncompressed, 15946 bytes compressed:  70.5%
+Zip file size: 17967 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      858 b- defN 23-May-25 11:19 pytket/qir/__init__.py
+-rw-r--r--  2.0 unx       69 b- defN 23-May-25 11:19 pytket/qir/_metadata.py
+-rw-r--r--  2.0 unx      711 b- defN 23-May-25 11:19 pytket/qir/conversion/__init__.py
+-rw-r--r--  2.0 unx     3352 b- defN 23-May-25 11:19 pytket/qir/conversion/api.py
+-rw-r--r--  2.0 unx    28971 b- defN 23-May-25 11:19 pytket/qir/conversion/conversion.py
+-rw-r--r--  2.0 unx     4082 b- defN 23-May-25 11:19 pytket/qir/conversion/gatesets.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-May-25 11:19 pytket/qir/conversion/module.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4183 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1017 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/RECORD
+12 files, 56180 bytes uncompressed, 16245 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pytket/qir/conversion/gatesets.py
 Comment: 
 
 Filename: pytket/qir/conversion/module.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc6.dist-info/LICENSE
+Filename: pytket_qir-0.2.0rc7.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qir-0.2.0rc6.dist-info/METADATA
+Filename: pytket_qir-0.2.0rc7.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qir-0.2.0rc6.dist-info/WHEEL
+Filename: pytket_qir-0.2.0rc7.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_qir-0.2.0rc6.dist-info/top_level.txt
+Filename: pytket_qir-0.2.0rc7.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_qir-0.2.0rc6.dist-info/RECORD
+Filename: pytket_qir-0.2.0rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/qir/__init__.py

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 
 """Backends for processing pytket circuits with Quantinuum devices
 """
 
 # _metadata.py is copied to the folder after installation.
 from ._metadata import __extension_version__, __extension_name__  # type: ignore
-from .conversion import pytket_to_qir, ReturnTypeQIR
+from .conversion import pytket_to_qir, QIRFormat
```

## pytket/qir/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.2.0rc6"
+__extension_version__ = "0.2.0rc7"
 __extension_name__ = "pytket-qir"
```

## pytket/qir/conversion/__init__.py

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Backends for processing pytket circuits with Quantinuum devices
 """
 
-from .api import pytket_to_qir, ReturnTypeQIR
+from .api import pytket_to_qir, QIRFormat
```

## pytket/qir/conversion/api.py

```diff
@@ -15,55 +15,59 @@
 """
 public api for qir conversion from pytket
 """
 
 from enum import Enum
 from typing import Union
 
+import pyqir
+
 from pytket.circuit import Circuit
 
 from .conversion import QirGenerator
 from .module import tketqirModule
 
 
-class ReturnTypeQIR(Enum):
+class QIRFormat(Enum):
     """Return types qir, options are BINARY for a binary
     output and STRING for a string output
     """
 
     BINARY = 0
     STRING = 1
 
 
 def pytket_to_qir(
     circ: Circuit,
     name: str = "Generated from input pytket circuit",
-    returntype: ReturnTypeQIR = ReturnTypeQIR.BINARY,
+    qir_format: QIRFormat = QIRFormat.BINARY,
+    pyqir_0_7_compatibility: bool = False,
 ) -> Union[str, bytes, None]:
     """converts given pytket circuit to qir
     :param circ: given circuit
     :type circ: pytket circuit
     :param name: name for the qir module created
     :type name: str
-    :param returntype: format of the generated qir, defaut value is binary
-    :type returntype: ReturnTypeQIR
+    :param qir_format: format of the generated qir, default value is binary
+    :type qir_format: QIRFormat
+    :param pyqir_0_7_compatibility: converts the output to be compatible with
+    pyqir 0.7, default value false
+    :type pyqir_0_7_compatibility: bool
     """
 
-    if len(circ.q_registers) > 1:
+    if len(circ.q_registers) > 1 or circ.q_registers[0].name != "q":
         raise ValueError(
-            """The circuit that should be converted should only have one
-            quantum register, you can convert it with using the pytket
-              compilerpass `FlattenRelabelRegistersPass`"""
+            """The circuit that should be converted should only have the default
+            quantum register. You can convert it using the pytket
+            compiler pass `FlattenRelabelRegistersPass`."""
         )
 
     for creg in circ.c_registers:
         if creg.size > 64:
-            raise ValueError(
-                "each of the classical register must not have more than 64 bits"
-            )
+            raise ValueError("classical registers must not have more than 64 bits")
 
     m = tketqirModule(
         name=name,
         num_qubits=circ.n_qubits,
         num_results=circ.n_qubits,
     )
 
@@ -73,13 +77,30 @@
         wasm_int_type=32,
         qir_int_type=64,
     )
 
     populated_module = qir_generator.circuit_to_module(
         qir_generator.circuit, qir_generator.module, True
     )
-    if returntype == ReturnTypeQIR.BINARY:
-        return populated_module.module.bitcode()
-    elif returntype == ReturnTypeQIR.STRING:
-        return populated_module.module.ir()
+
+    if pyqir_0_7_compatibility:
+
+        initial_result = str(populated_module.module.ir())  # type: ignore
+
+        result = initial_result.replace("entry_point", "EntryPoint").replace("num_required_qubits", "requiredQubits").replace("num_required_results", "requiredResults")  # type: ignore
+
+        bitcode = pyqir.Module.from_ir(pyqir.Context(), result).bitcode  # type: ignore
+
+        if qir_format == QIRFormat.BINARY:
+            return bitcode  # type: ignore
+        elif qir_format == QIRFormat.STRING:
+            return result  # type: ignore
+        else:
+            assert not "unsupported return type"
+
     else:
-        raise ValueError("unsupported return type")
+        if qir_format == QIRFormat.BINARY:
+            return populated_module.module.bitcode()
+        elif qir_format == QIRFormat.STRING:
+            return populated_module.module.ir()
+        else:
+            assert not "unsupported return type"
```

## pytket/qir/conversion/conversion.py

```diff
@@ -489,38 +489,40 @@
                         self.ssa_vars[registername],
                         pyqir.const(self.qir_int_type, condition_bit_index),
                         result,
                     ],
                 )
 
             elif isinstance(op, Conditional):
-                assert op.width == 1  # only one conditional bit
+
                 conditional_circuit = self._rebase_op_to_gateset(
                     op.op, command.args[op.width :]
                 )
-                condition_bit_index = command.args[0].index[0]
                 condition_name = command.args[0].reg_name
 
-                def condition_block_true() -> None:
-                    """
-                    Populate recursively the module with the contents of the conditional
-                    sub-circuit when the condition is True.
-                    """
-                    if op.value == 1:
-                        self.circuit_to_module(conditional_circuit, module)
+                if op.width == 1:  # only one conditional bit
+                    condition_bit_index = command.args[0].index[0]
 
-                def condition_block_false() -> None:
-                    """
-                    Populate recursively the module with the contents of the conditional
-                    sub-circuit when the condition is False.
-                    """
-                    if op.value == 0:
-                        self.circuit_to_module(conditional_circuit, module)
+                    def condition_block_true() -> None:
+                        """
+                        Populate recursively the module with the contents of the
+                        conditional sub-circuit when the condition is True.
+                        """
+                        if op.value == 1:
+                            self.circuit_to_module(conditional_circuit, module)
+
+                    def condition_block_false() -> None:
+                        """
+                        Populate recursively the module with the contents of the
+                        conditional sub-circuit when the condition is False.
+                        """
+                        if op.value == 0:
+                            self.circuit_to_module(conditional_circuit, module)
 
-                if condition_name in self.ssa_vars:
+                    assert condition_name in self.ssa_vars
 
                     ssabool = module.builder.call(
                         self.read_bit_from_reg,
                         [
                             self.ssa_vars[condition_name],
                             pyqir.const(self.qir_int_type, condition_bit_index),
                         ],
@@ -529,23 +531,52 @@
                     module.module.builder.if_(
                         ssabool,
                         true=lambda: condition_block_true(),  # type: ignore
                         false=lambda: condition_block_false(),  # type: ignore
                     )
 
                 else:
-                    ValueError(
-                        "circuit contruction with special condition not yet supported"
+
+                    for i in range(op.width):
+                        if command.args[i].reg_name != condition_name:
+                            raise ValueError(
+                                "conditional can only work with one entire register"
+                            )
+
+                    for i in range(op.width - 1):
+                        if command.args[i].index[0] >= command.args[i + 1].index[0]:
+                            raise ValueError(
+                                "conditional can only work with one entire register"
+                            )
+
+                    if self.circuit.get_c_register(condition_name).size != op.width:
+                        raise ValueError(
+                            "conditional can only work with one entire register"
+                        )
+
+                    def condition_block() -> None:
+                        """
+                        Populate recursively the module with the contents of the
+                        conditional sub-circuit when the condition is True.
+                        """
+                        self.circuit_to_module(conditional_circuit, module)
+
+                    ssabool = module.module.builder.icmp(
+                        pyqir.IntPredicate.EQ,
+                        pyqir.const(self.qir_int_type, op.value),
+                        self.ssa_vars[condition_name],
+                    )
+
+                    module.module.builder.if_(
+                        ssabool,
+                        true=lambda: condition_block(),  # type: ignore
                     )
-                    # this should be an assertion when working
 
             elif isinstance(op, WASMOp):
-                raise ValueError(
-                    "WASM not supported yet, support expected with pytket-qir==0.3.0"
-                )
+                raise ValueError("WASM not supported yet")
             elif op.type == OpType.Measure:
 
                 assert len(command.bits) == 1
                 assert len(command.qubits) == 1
                 assert command.qubits[0].reg_name == "q"
 
                 module.qis.mz(
```

## Comparing `pytket_qir-0.2.0rc6.dist-info/LICENSE` & `pytket_qir-0.2.0rc7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_qir-0.2.0rc6.dist-info/METADATA` & `pytket_qir-0.2.0rc7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qir
-Version: 0.2.0rc6
+Version: 0.2.0rc7
 Summary: Extension for pytket, providing functions for conversion into to qir
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-qir/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-qir
 Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
```

## Comparing `pytket_qir-0.2.0rc6.dist-info/RECORD` & `pytket_qir-0.2.0rc7.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pytket/qir/__init__.py,sha256=bVQc7W5vFNKJ_hnMPYiFaYnU6NPJAMaYMY_m3rZ4Jgs,862
-pytket/qir/_metadata.py,sha256=kaJz0Mi4P3mb_Q3Rl0rlewezOwpT-Bzu_sMktT6l3vE,69
-pytket/qir/conversion/__init__.py,sha256=FTpNgzkF_dlwlu67zaPKHX5y2_v_jGmTnViJ8IbiX8w,715
-pytket/qir/conversion/api.py,sha256=q1A4dphwvSCe0Yf0eUEPs-mGc9rR2lePhng7pIWHoMI,2519
-pytket/qir/conversion/conversion.py,sha256=T0IJh5NPDYnhY9kC0TYF3zFQ4XKuoJ4q3NdR2ETEVhc,27612
+pytket/qir/__init__.py,sha256=3AXz2dN6Yg20zM3YYtMAPf6ZCidAG-opHomVhmU93w4,858
+pytket/qir/_metadata.py,sha256=Q72S2KNuOD41_lqKXljKX1mo5gC5O05w_ibxpNJ3AN4,69
+pytket/qir/conversion/__init__.py,sha256=kKuV2wCn6cMf_iVQhlsu28cH8K4dDCUqwUXlHF_FpUg,711
+pytket/qir/conversion/api.py,sha256=FznzHIsaAJCAbhQxc3iudc173sWYI9bz1i8dJJtl9L0,3352
+pytket/qir/conversion/conversion.py,sha256=ppjPAhsBEfBtnAe-8u-izrW4zpG5O_11X6rt7rbTekc,28971
 pytket/qir/conversion/gatesets.py,sha256=Ix1KkLlFoyE1LkoUs0J7wFikZXT9w5jYs8mnTQnZURM,4082
 pytket/qir/conversion/module.py,sha256=fj8iHNh27_-wbjKkO9JdnKkExiRAhMWXTzjVP9kCwtA,1481
-pytket_qir-0.2.0rc6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytket_qir-0.2.0rc6.dist-info/METADATA,sha256=vwQ8oYOBrvdr_p4hUsvHExjDB_46W7AKoG1_lKX1WzI,4183
-pytket_qir-0.2.0rc6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytket_qir-0.2.0rc6.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_qir-0.2.0rc6.dist-info/RECORD,,
+pytket_qir-0.2.0rc7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_qir-0.2.0rc7.dist-info/METADATA,sha256=_qbFKZ4Y-huQLdPB_A9e1EOCjcPfOotglGJgrg5G6X4,4183
+pytket_qir-0.2.0rc7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytket_qir-0.2.0rc7.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_qir-0.2.0rc7.dist-info/RECORD,,
```

