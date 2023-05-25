# Comparing `tmp/hdcc-0.6.3.tar.gz` & `tmp/hdcc-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcc-0.6.3.tar", max compression
+gzip compressed data, was "hdcc-0.6.4.tar", max compression
```

## Comparing `hdcc-0.6.3.tar` & `hdcc-0.6.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       90 2023-04-27 19:50:34.511536 hdcc-0.6.3/README.md
--rw-r--r--   0        0        0    19811 2023-05-18 20:05:24.076365 hdcc-0.6.3/hdcc/HDProg.py
--rw-r--r--   0        0        0    17423 2023-05-18 21:43:21.092307 hdcc-0.6.3/hdcc/HDTypes.py
--rw-r--r--   0        0        0        0 2023-04-27 19:50:34.512471 hdcc-0.6.3/hdcc/__init__.py
--rw-r--r--   0        0        0      330 2023-05-18 21:43:37.710350 hdcc-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.6.4/README.md
+-rw-r--r--   0        0        0    19728 2023-05-25 03:31:51.475701 hdcc-0.6.4/hdcc/HDProg.py
+-rw-r--r--   0        0        0    17423 2023-05-24 22:57:38.914478 hdcc-0.6.4/hdcc/HDTypes.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.6.4/hdcc/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-25 03:32:04.579243 hdcc-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.6.4/PKG-INFO
```

### Comparing `hdcc-0.6.3/hdcc/HDProg.py` & `hdcc-0.6.4/hdcc/HDProg.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,20 @@
     Operator.FRAC_BIND: ((str, Types.HyperVector), (str, int, float), Types.HyperVector)
 }
 
 
 class Expression:
     # a: Expression | str | int | float | Types.HyperVector
     # aType: type
-    op: Operator
+    # op: Operator
     # b: Expression | str | int | float | Types.HyperVector
     # bType: type
-    outType: type
-    operands: list[Expression | str | int | float | Types.HyperVector]
-    types: list[type]
+    # outType: type
+    # operands: list[Expression | str | int | float | Types.HyperVector]
+    # types: list[type]
 
     def __init__(self, op: Operator, operands: list[Expression | str | int | float | Types.HyperVector], program: HDProg = None):
         self.op = op
         self.operands = operands
         self.types = []
         # parse types
         for i in range(len(operands)):
@@ -88,41 +88,42 @@
         return "Expression(" + str(self.op) + ", " + str(self.operands) + ")"
     
     def typecheck(self):
         self.outType = self.op.support(self.types)
         pass
 
     def eval(self, state: HDProgState):
+        vals = [0 for _ in range(len(self.operands))]
         if not self.op == Operator.BUNDlE:
             if isinstance(self.operands[0], Expression):
-                self.operands[0] = self.operands[0].eval(state)
+                vals[0] = self.operands[0].eval(state)
             elif isinstance(self.operands[0], str):
                 # type check
                 if self.operands[0] not in state.val_table:
                     raise Exception("Symbol " + self.operands[0] + " not found")
                 if not issubclass(state.val_table[self.operands[0]][1], self.types[0]):
                     raise Exception("Symbol " + self.operands[0] + " is not of type " + str(self.types[0]))
-                self.operands[0] = state.val_table[self.operands[0]][3]
+                vals[0] = state.val_table[self.operands[0]][3]
             if isinstance(self.operands[1], Expression):
-                self.operands[1] = self.operands[1].eval(state)
+                vals[1] = self.operands[1].eval(state)
             elif isinstance(self.operands[1], str):
                 # type check
                 if self.operands[1] not in state.val_table:
                     raise Exception("Symbol " + self.operands[1] + " not found")
                 if not issubclass(state.val_table[self.operands[1]][1], self.types[1]):
                     raise Exception("Symbol " + self.operands[1] + " is not of type " + str(self.types[1]))
-                self.operands[1] = state.val_table[self.operands[1]][3]
+                vals[1] = state.val_table[self.operands[1]][3]
             if self.op == Operator.BIND:
-                return self.operands[0].bind(self.operands[1])
+                return vals[0].bind(vals[1])
             elif self.op == Operator.UNBIND:
-                return self.operands[0].unbind(self.operands[1])
+                return vals[0].unbind(vals[1])
             elif self.op == Operator.PERMUTATION:
-                return self.operands[0].permutation(self.operands[1])
+                return vals[0].permutation(vals[1])
             elif self.op == Operator.FRAC_BIND:
-                return self.operands[0].frac_bind(self.operands[1])
+                return vals[0].frac_bind(vals[1])
             else:
                 raise Exception("Unsupported operator " + str(self.op))
         else:
             vals = []
             for i in range(len(self.operands)):
                 if isinstance(self.operands[i], Expression):
                     vals.append(self.operands[i].eval(state))
@@ -141,17 +142,14 @@
 
 Operand = Union[Expression, str, int, float, Types.HyperVector]
 
 
 # Definition of HDProg class
 
 class HDProgState:
-    val_table: dict = {}
-    pc = 0
-
     def __init__(self, val_table: dict = None, pc: int = 0):
         if val_table is not None:
             self.val_table = val_table
         self.pc = pc
         pass
     pass
```

### Comparing `hdcc-0.6.3/hdcc/HDTypes.py` & `hdcc-0.6.4/hdcc/HDTypes.py`

 * *Files identical despite different names*

### Comparing `hdcc-0.6.3/PKG-INFO` & `hdcc-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcc
-Version: 0.6.3
+Version: 0.6.4
 Summary: 
 Author: Yifan Yang
 Author-email: yyang29@stanford.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

