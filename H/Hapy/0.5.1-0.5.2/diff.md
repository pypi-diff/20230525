# Comparing `tmp/Hapy-0.5.1.tar.gz` & `tmp/Hapy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hapy-0.5.1.tar", last modified: Tue May 16 20:35:23 2023, max compression
+gzip compressed data, was "Hapy-0.5.2.tar", last modified: Wed May 24 23:49:27 2023, max compression
```

## Comparing `Hapy-0.5.1.tar` & `Hapy-0.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:35:23.543567 Hapy-0.5.1/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:35:23.491159 Hapy-0.5.1/Hapy.egg-info/
--rw-rw-rw-   0        0        0     6575 2023-05-16 20:35:23.000000 Hapy-0.5.1/Hapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-16 20:35:23.000000 Hapy-0.5.1/Hapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:35:23.000000 Hapy-0.5.1/Hapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-16 20:35:23.000000 Hapy-0.5.1/Hapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 20:35:23.000000 Hapy-0.5.1/Hapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 20:35:23.000000 Hapy-0.5.1/Hapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1140 2021-10-19 14:31:36.000000 Hapy-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0      138 2021-11-08 15:33:44.000000 Hapy-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6575 2023-05-16 20:35:23.543567 Hapy-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     5814 2023-05-16 20:10:35.000000 Hapy-0.5.1/README.md
--rw-rw-rw-   0        0        0        7 2021-11-27 23:37:20.000000 Hapy-0.5.1/VERSION.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 20:35:23.521382 Hapy-0.5.1/hapy/
--rw-rw-rw-   0        0        0      373 2021-11-27 23:37:20.000000 Hapy-0.5.1/hapy/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-05-16 15:40:24.000000 Hapy-0.5.1/hapy/exector.py
--rw-rw-rw-   0        0        0    13601 2023-05-16 15:40:24.000000 Hapy-0.5.1/hapy/generate_py.py
--rw-rw-rw-   0        0        0       63 2023-05-16 15:42:28.000000 Hapy-0.5.1/hapy/hello.hapy
--rw-rw-rw-   0        0        0     4695 2023-05-16 15:40:24.000000 Hapy-0.5.1/hapy/importer.py
--rw-rw-rw-   0        0        0     4466 2021-10-16 21:38:52.000000 Hapy-0.5.1/hapy/indent.py
--rw-rw-rw-   0        0        0     2113 2023-05-16 15:40:24.000000 Hapy-0.5.1/hapy/input_stream.py
--rw-rw-rw-   0        0        0     1146 2021-11-16 14:21:34.000000 Hapy-0.5.1/hapy/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:35:23.525379 Hapy-0.5.1/hapy/modules/
--rw-rw-rw-   0        0        0      138 2021-10-15 16:38:34.000000 Hapy-0.5.1/hapy/modules/popo_module.py
--rw-rw-rw-   0        0        0      334 2021-10-15 16:38:34.000000 Hapy-0.5.1/hapy/modules/test_module.py
--rw-rw-rw-   0        0        0     1174 2021-11-16 14:21:34.000000 Hapy-0.5.1/hapy/something.hapy
--rw-rw-rw-   0        0        0    17152 2023-05-16 20:10:09.000000 Hapy-0.5.1/hapy/token_parser.py
--rw-rw-rw-   0        0        0     6394 2023-05-16 15:40:24.000000 Hapy-0.5.1/hapy/token_stream.py
--rw-rw-rw-   0        0        0     2157 2023-04-06 08:31:55.000000 Hapy-0.5.1/hapy/translations.py
--rw-rw-rw-   0        0        0     2376 2021-11-16 14:21:34.000000 Hapy-0.5.1/hapy/transpiler.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:35:23.529380 Hapy-0.5.1/scripts/
--rw-rw-rw-   0        0        0      219 2021-11-08 15:33:44.000000 Hapy-0.5.1/scripts/__init__.py
--rw-rw-rw-   0        0        0     9101 2023-05-16 15:40:24.000000 Hapy-0.5.1/scripts/hapy_cli.py
--rw-rw-rw-   0        0        0       90 2023-05-16 20:35:23.549563 Hapy-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1039 2023-05-16 20:18:59.000000 Hapy-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:35:23.541486 Hapy-0.5.1/tests/
--rw-rw-rw-   0        0        0        0 2021-11-14 20:49:44.000000 Hapy-0.5.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1152 2023-05-16 15:40:24.000000 Hapy-0.5.1/tests/test_generatepy.py
--rw-rw-rw-   0        0        0     1548 2023-05-16 15:40:24.000000 Hapy-0.5.1/tests/test_input_stream.py
--rw-rw-rw-   0        0        0    20600 2021-11-14 20:49:44.000000 Hapy-0.5.1/tests/test_parser.py
--rw-rw-rw-   0        0        0     4345 2021-11-14 20:49:44.000000 Hapy-0.5.1/tests/test_token_stream.py
+drwxrwxrwx   0        0        0        0 2023-05-24 23:49:27.325513 Hapy-0.5.2/
+drwxrwxrwx   0        0        0        0 2023-05-24 23:49:27.269762 Hapy-0.5.2/Hapy.egg-info/
+-rw-rw-rw-   0        0        0     6552 2023-05-24 23:49:27.000000 Hapy-0.5.2/Hapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-24 23:49:27.000000 Hapy-0.5.2/Hapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 23:49:27.000000 Hapy-0.5.2/Hapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-24 23:49:27.000000 Hapy-0.5.2/Hapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-24 23:49:27.000000 Hapy-0.5.2/Hapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-24 23:49:27.000000 Hapy-0.5.2/Hapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1140 2021-10-19 14:31:36.000000 Hapy-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      138 2021-11-08 15:33:44.000000 Hapy-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6552 2023-05-24 23:49:27.325513 Hapy-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5814 2023-05-16 20:10:35.000000 Hapy-0.5.2/README.md
+-rw-rw-rw-   0        0        0        6 2023-05-24 23:49:05.000000 Hapy-0.5.2/VERSION.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 23:49:27.301480 Hapy-0.5.2/hapy/
+-rw-rw-rw-   0        0        0      360 2023-05-24 23:49:05.000000 Hapy-0.5.2/hapy/__init__.py
+-rw-rw-rw-   0        0        0     1860 2023-05-16 15:40:24.000000 Hapy-0.5.2/hapy/exector.py
+-rw-rw-rw-   0        0        0    13601 2023-05-16 15:40:24.000000 Hapy-0.5.2/hapy/generate_py.py
+-rw-rw-rw-   0        0        0       63 2023-05-16 15:42:28.000000 Hapy-0.5.2/hapy/hello.hapy
+-rw-rw-rw-   0        0        0     4695 2023-05-16 15:40:24.000000 Hapy-0.5.2/hapy/importer.py
+-rw-rw-rw-   0        0        0     4466 2021-10-16 21:38:52.000000 Hapy-0.5.2/hapy/indent.py
+-rw-rw-rw-   0        0        0     2113 2023-05-24 23:46:18.000000 Hapy-0.5.2/hapy/input_stream.py
+-rw-rw-rw-   0        0        0     1146 2021-11-16 14:21:34.000000 Hapy-0.5.2/hapy/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 23:49:27.306475 Hapy-0.5.2/hapy/modules/
+-rw-rw-rw-   0        0        0      138 2021-10-15 16:38:34.000000 Hapy-0.5.2/hapy/modules/popo_module.py
+-rw-rw-rw-   0        0        0      334 2021-10-15 16:38:34.000000 Hapy-0.5.2/hapy/modules/test_module.py
+-rw-rw-rw-   0        0        0     1174 2021-11-16 14:21:34.000000 Hapy-0.5.2/hapy/something.hapy
+-rw-rw-rw-   0        0        0    17014 2023-05-23 13:00:03.000000 Hapy-0.5.2/hapy/token_parser.py
+-rw-rw-rw-   0        0        0     6394 2023-05-16 15:40:24.000000 Hapy-0.5.2/hapy/token_stream.py
+-rw-rw-rw-   0        0        0     2157 2023-04-06 08:31:55.000000 Hapy-0.5.2/hapy/translations.py
+-rw-rw-rw-   0        0        0     2376 2021-11-16 14:21:34.000000 Hapy-0.5.2/hapy/transpiler.py
+drwxrwxrwx   0        0        0        0 2023-05-24 23:49:27.310475 Hapy-0.5.2/scripts/
+-rw-rw-rw-   0        0        0      219 2021-11-08 15:33:44.000000 Hapy-0.5.2/scripts/__init__.py
+-rw-rw-rw-   0        0        0     9101 2023-05-16 15:40:24.000000 Hapy-0.5.2/scripts/hapy_cli.py
+-rw-rw-rw-   0        0        0       90 2023-05-24 23:49:27.331800 Hapy-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2023-05-24 23:49:05.000000 Hapy-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 23:49:27.322514 Hapy-0.5.2/tests/
+-rw-rw-rw-   0        0        0        0 2021-11-14 20:49:44.000000 Hapy-0.5.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1168 2023-05-23 13:00:03.000000 Hapy-0.5.2/tests/test_generatepy.py
+-rw-rw-rw-   0        0        0     1548 2023-05-16 15:40:24.000000 Hapy-0.5.2/tests/test_input_stream.py
+-rw-rw-rw-   0        0        0    18978 2023-05-23 13:00:03.000000 Hapy-0.5.2/tests/test_parser.py
+-rw-rw-rw-   0        0        0     4369 2023-05-24 23:46:04.000000 Hapy-0.5.2/tests/test_token_stream.py
```

### Comparing `Hapy-0.5.1/Hapy.egg-info/PKG-INFO` & `Hapy-0.5.2/Hapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: Hapy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Basic Python using Hausa vocabulary
 Home-page: https://github.com/hapy-lang/hapy
 Author: Emmanuel Segun-Lean
 Author-email: emmanuel.segunlean@proton.me
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -208,9 +207,7 @@
 @software{segunlean2021,
   author = {Segun-Lean, Emmanuel and Wuta, Shugaba},
   title = {Hapy: Hausa Programming Language},
   month = December,
   year = 2021,
   url = {https://github.com/hapy-lang/hapy}
 }
-
-
```

### Comparing `Hapy-0.5.1/Hapy.egg-info/SOURCES.txt` & `Hapy-0.5.2/Hapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/LICENSE.txt` & `Hapy-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/PKG-INFO` & `Hapy-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: Hapy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Basic Python using Hausa vocabulary
 Home-page: https://github.com/hapy-lang/hapy
 Author: Emmanuel Segun-Lean
 Author-email: emmanuel.segunlean@proton.me
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -208,9 +207,7 @@
 @software{segunlean2021,
   author = {Segun-Lean, Emmanuel and Wuta, Shugaba},
   title = {Hapy: Hausa Programming Language},
   month = December,
   year = 2021,
   url = {https://github.com/hapy-lang/hapy}
 }
-
-
```

### Comparing `Hapy-0.5.1/README.md` & `Hapy-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/exector.py` & `Hapy-0.5.2/hapy/exector.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/generate_py.py` & `Hapy-0.5.2/hapy/generate_py.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/importer.py` & `Hapy-0.5.2/hapy/importer.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/indent.py` & `Hapy-0.5.2/hapy/indent.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/input_stream.py` & `Hapy-0.5.2/hapy/input_stream.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/main.py` & `Hapy-0.5.2/hapy/main.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/something.hapy` & `Hapy-0.5.2/hapy/something.hapy`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/token_parser.py` & `Hapy-0.5.2/hapy/token_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from .translations import keywords, operator_words, builtin_functions
 
 FALSE = {"type": "bool", "value": False}
 PASS = {"type": "var", "value": "pass"}
 
 
 def any_fulfill(collection, condition):
-    """checks if any element of collection returns true for condition """
+    """checks if any element of collection returns true for condition"""
     a = False
     index = 0
     while not a and index < len(collection):
         a = condition(collection[index])
         index += 1
     return a
 
+
 def parse(input: TokenStream):
     """parse input to AST tokens"""
 
     PRECEDENCE = {
         "=": 1,
         ":": 1,
         operator_words[input.settings["lang"]]["is"]: 1,
@@ -56,87 +57,84 @@
         if operation.lower() == "get":
             return expecting_non_dict_block
         elif operation.lower() == "set":
             expecting_non_dict_block = True
 
     def is_punc(ch):
         tok = input.peek()
-        return tok and tok["type"] == "punc" and (not ch or tok["value"]
-                                                  == ch) and tok
+        return tok and tok["type"] == "punc" and (not ch or tok["value"] == ch) and tok
 
     def is_kw(kw):
         tok = input.peek()
-        return tok and tok["type"] == "kw" and (not kw
-                                                or tok["value"] == kw) and tok
+        return tok and tok["type"] == "kw" and (not kw or tok["value"] == kw) and tok
 
     def is_op(op):
         tok = input.peek()
-        return tok and tok["type"] == "op" and (not op
-                                                or tok["value"] == op) and tok
+        return tok and tok["type"] == "op" and (not op or tok["value"] == op) and tok
 
     def skip_punc(ch):
         if is_punc(ch):
             input.next()
         else:
 
             # if the punc we are meant to skip is ';' then there's probs
             # something wrong with the syntax :|
             if ch == ";":
                 return unexpected(
-                    "Check your syntax! You might have made an error at %s")
+                    "Check your syntax! You might have made an error at %s"
+                )
 
-            input.croak(f"Expecting punctuation got: \"{ch}\"")
+            input.croak(f'Expecting punctuation got: "{ch}"')
 
     def skip_kw(kw):
         if is_kw(kw):
             input.next()
         else:
-            input.croak(f"Expecting keyword got: \"{kw}\"")
+            input.croak(f'Expecting keyword got: "{kw}"')
 
     def skip_op(op):
         if is_op(op):
             input.next()
         else:
-            input.croak(f"Expecting operator got: \"{op}\"")
+            input.croak(f'Expecting operator got: "{op}"')
 
     def unexpected(msg="unexpected token: %s "):
         input.croak(msg % json.dumps(input.peek()))
 
     def maybe_binary(left, my_prec):
         tok = is_op(None)
         # tbh, I'm not 100% sure what's going on here, but I'll find out!
         binary_type = {  # noqa: F841
             operator_words[input.settings["lang"]]["is"]: "assign",
             "=": "assign",
             ".": "access",
             operator_words[input.settings["lang"]]["in"]: "membership",
-            ":": "dict-elem"  # Wuta added this line.
+            ":": "dict-elem",  # Wuta added this line.
         }
         if tok:
             their_prec = PRECEDENCE[tok["value"]]
             if their_prec > my_prec:
                 input.next()
 
                 return maybe_binary(
                     {
-                        "type":
-                        binary_type.get(tok["value"], "binary"),
-                        "operator":
-                        tok["value"],
-                        "left" if tok["value"] != ":" else "key":
-                        left,
-                        "right" if tok["value"] != ":" else "value":
-                        maybe_binary(parse_atom(), their_prec)
-                    }, my_prec
+                        "type": binary_type.get(tok["value"], "binary"),
+                        "operator": tok["value"],
+                        "left" if tok["value"] != ":" else "key": left,
+                        "right"
+                        if tok["value"] != ":"
+                        else "value": maybe_binary(parse_atom(), their_prec),
+                    },
+                    my_prec,
                 )  # made a mistake here initially, put their_prec instead :|
 
         return left
 
     def delimited(start, stop, separator, parser):
-        """ get all the args for example """
+        """get all the args for example"""
 
         args, first = [], True
 
         skip_punc(start)
         while not input.eof():
             if is_punc(stop):
                 break
@@ -151,15 +149,15 @@
         skip_punc(stop)
         return args
 
     def parse_call(func):
         return {
             "type": "call",
             "func": func,
-            "args": delimited("(", ")", ",", parse_expression)
+            "args": delimited("(", ")", ",", parse_expression),
         }
 
     def parse_varname():
         name = input.next()
         if name["type"] != "var":
             input.croak("Expecting variable name")
         return {"type": "var", "value": name["value"]}
@@ -202,40 +200,39 @@
         # if is_kw("else_if"):
         #   input.next()
         #   ret["else"] = parse_expression()
 
         return ret
 
     def parse_while():
-        """ parse while"""
+        """parse while"""
         block_kw("set")
 
-        '''
+        """
         Basically this creates a block of code. However a dictionary sysntax is quite similar "{}".
         So once it sees a block, it should set expecting_non_dict_block to True and the next '{}' is called as a block.
-        '''
+        """
         block_kw("set")
 
         skip_kw(keywords[input.settings["lang"]]["while"])
 
         cond = parse_expression()
 
         then = parse_expression()
 
         ret = {
             "type": "while",
             "cond": cond,
-            "then":
-            then  # TODO: probably rename this to 'body' to match functions
+            "then": then,  # TODO: probably rename this to 'body' to match functions
         }
 
         return ret
 
     def parse_forloop():
-        """ read a for-loop expression """
+        """read a for-loop expression"""
         block_kw("set")
 
         skip_kw(keywords[input.settings["lang"]]["for"])
 
         header = parse_expression()  # the iterator...
 
         body = parse_expression()
@@ -269,15 +266,15 @@
 
         ret = {
             # get variable name, that should be the next thing!
             # we are using parse_expression because the args could actually
             # be expressions like assingment def foo(b=1) {...}
             **ret,
             "vars": delimited("(", ")", ",", parse_expression),
-            "body": parse_expression()
+            "body": parse_expression(),
         }
 
         return ret
 
     def parse_class():
         """
         read a class definition.
@@ -330,16 +327,15 @@
                 ret["class_special_methods"].append(e)
             elif e["type"] == "function":
                 ret["class_methods"].append(e)
             # this is to initialize the parent class
             elif e["type"] == "use_class":
                 ret["init_parent"] = e
                 # make sure classes are the same!
-                if ret["init_parent"]["func"]["value"] != ret["inherits"][
-                        "value"]:
+                if ret["init_parent"]["func"]["value"] != ret["inherits"]["value"]:
                     input.croak("Parent class not initialized!")
 
         return ret
 
     def parse_modulename():
         name = input.next()
         if name["type"] != "var":
@@ -394,15 +390,18 @@
         elif p["type"] == "var":
             ret = {**ret, **p}
         # TODO: maybe throw an error here...
 
         return p
 
     def parse_bool():
-        return {"type": "bool", "value": input.next()["value"] == keywords[input.settings["lang"]]["True"]}
+        return {
+            "type": "bool",
+            "value": input.next()["value"] == keywords[input.settings["lang"]]["True"],
+        }
 
     def maybe_call(expr):
         expr = expr()
         return parse_call(expr) if is_punc("(") else expr
 
     def parse_atom():
         def doer():
@@ -440,25 +439,30 @@
                 return parse_import()
             if is_kw(keywords[input.settings["lang"]]["return"]):
                 return parse_return()
             if is_kw(keywords[input.settings["lang"]]["has"]):
                 return parse_classprop()
             if is_kw(keywords[input.settings["lang"]]["use"]):
                 return parse_class_use()
-            if is_kw(keywords[input.settings["lang"]]["True"]) or is_kw(keywords[input.settings["lang"]]["False"]):
+            if is_kw(keywords[input.settings["lang"]]["True"]) or is_kw(
+                keywords[input.settings["lang"]]["False"]
+            ):
                 return parse_bool()
             if is_kw(keywords[input.settings["lang"]]["def"]):
                 return parse_function()
 
             # NOTE: If you don't handle tokens they will raise an error
 
             tok = input.next()
 
-            if (tok["type"] == "var") or (tok["type"] == "num") or (tok["type"]
-                                                                    == "str"):
+            if (
+                (tok["type"] == "var")
+                or (tok["type"] == "num")
+                or (tok["type"] == "str")
+            ):
                 return tok
 
             unexpected()
 
         return maybe_call(doer)
 
     def parse_list():
```

### Comparing `Hapy-0.5.1/hapy/token_stream.py` & `Hapy-0.5.2/hapy/token_stream.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/translations.py` & `Hapy-0.5.2/hapy/translations.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/hapy/transpiler.py` & `Hapy-0.5.2/hapy/transpiler.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/scripts/hapy_cli.py` & `Hapy-0.5.2/scripts/hapy_cli.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/setup.py` & `Hapy-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name='Hapy',
-    version='0.5.1',
+    version='0.5.2',
     author='Emmanuel Segun-Lean',
     author_email='emmanuel.segunlean@proton.me',
     license='MIT',
     description='Basic Python using Hausa vocabulary',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/hapy-lang/hapy',
```

### Comparing `Hapy-0.5.1/tests/test_generatepy.py` & `Hapy-0.5.2/tests/test_generatepy.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from hapy.token_stream import TokenStream
 from hapy.token_parser import parse
 from hapy.generate_py import make_py
 
 # TODO: ADD MORE TESTS OOO! TEST OTHER CONSTRUCTS!
 class TestGeneratePy(unittest.TestCase):
     def test_binary_ops_1(self):
-        """ test the binary ops bro """
+        """test the binary ops bro"""
         code = """
 				age = 20;
 				age > 10;
 				"""
 
         inputs = InputStream(code)
         tokens = TokenStream(inputs)
@@ -22,16 +22,17 @@
         expected = """age = 20;\n(age > 10)"""
 
         actual = make_py(ast)
 
         self.assertEqual(expected, actual, "This is a binary operator!")
 
     def test_binary_ops_words(self):
-        """ test the binary ops bro """
+        """test the binary ops bro"""
         code = """
+        #! lang=eng
 				bola_age is 20;
 				tolu_age is 30 minus 10;
 				"""
 
         inputs = InputStream(code)
         tokens = TokenStream(inputs)
         ast = parse(tokens)
```

### Comparing `Hapy-0.5.1/tests/test_input_stream.py` & `Hapy-0.5.2/tests/test_input_stream.py`

 * *Files identical despite different names*

### Comparing `Hapy-0.5.1/tests/test_token_stream.py` & `Hapy-0.5.2/tests/test_token_stream.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,159 @@
-import unittest
-
-from hapy.input_stream import InputStream
-from hapy.token_stream import TokenStream
-
-
-class TestTokenStream(unittest.TestCase):
-    def test_read_next_number(self):
-        """test read number function"""
-
-        stream = InputStream("30.034")
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "num", "value": 30.034}
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual, "the stream is a number")
-
-    def test_read_next_string(self):
-        """test read number function"""
-
-        stream = InputStream('"Thank you Jesus"')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "str", "value": "Thank you Jesus"}
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual, "the stream is a string")
-
-    def test_skip_comment(self):
-        """test read number function"""
-
-        stream = InputStream('#this is a comment!\n"Hello my friend!"')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "str", "value": "Hello my friend!"}
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual,
-                         "the stream is a comment, whitespace & string")
-
-    def test_read_identifier_keywords(self):
-        """test identifier function"""
-
-        stream = InputStream('return "goat"')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "kw", "value": "return"}
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual, "the stream is a keyword")
-
-    def test_read_identifier_varnames1(self):
-        """test identifier function to identify variable names"""
-
-        stream = InputStream('cow = "animal"')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "var", "value": "cow"}
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual, "the stream is an identifier")
-
-    def test_read_operator(self):
-        """test identifier function"""
-
-        stream1 = InputStream('>=')
-
-        ts1 = TokenStream(stream1)
-
-        expected1 = {"type": "op", "value": ">="}
-
-        actual1 = ts1.read_next()
-
-        # test multi character operator: => //
-        stream2 = InputStream('and')
-
-        ts2 = TokenStream(stream2)
-
-        expected2 = {"type": "op", "value": "and"}
-
-        actual2 = ts2.read_next()
-
-        self.assertEqual([expected1, expected2], [actual1, actual2],
-                         "the stream is a operation char")
-
-    def test_read_punctuation(self):
-        """test identifier function to identify variable names"""
-
-        stream = InputStream('{"cow": "animal"}')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "punc", "value": "{"}
-
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual, "the stream is a punctuation mark")
-
-    def test_read_dot(self):
-        """test identifier function to identify dot operator"""
-        # we are treeating the '.' as a binary operator in a sense
-
-        stream = InputStream('"hello".upper()')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "op", "value": "."}
-
-        ts.read_next() # first token
-        actual = ts.read_next() # 2nd...
-
-        self.assertEqual(expected, actual, "Expected a dot token")
-
-    def test_import_statement_1(self):
-        """test token stream reading import tokens"""
-
-        stream = InputStream('import names;')
-
-        ts = TokenStream(stream)
-
-        expected = [{"type": "kw", "value": "import"}, {"type": "var", "value": "names"}]
-
-        actual = [ts.read_next(), ts.read_next()] # 2nd...
-
-        self.assertEqual(expected, actual, "Expected import and names keywords")
-
-    def test_forloop_statement_1(self):
-        """test token stream reading forloop statement"""
-
-        stream = InputStream('for (a in b) {\n print(a); };')
-
-        ts = TokenStream(stream)
-
-        expected = {"type": "kw", "value": "for"}
-
-        actual = ts.read_next()
-
-        self.assertEqual(expected, actual, "Expected for loop keyword")
-
-
-if __name__ == "__main__":
-    # NOTE: You have to set the env to "set HAPY_LANG=eng" if you want to
-    # test these in english.
-
-    # we should probably create a Hausa version of the tests :)
-    unittest.main()
+import os
+from unittest import main, mock, TestCase
+
+from hapy.input_stream import InputStream
+from hapy.token_stream import TokenStream
+
+class TestTokenStream(TestCase):
+    # TODO: doesn't work idk why. You have to set Env Variables yourself
+    @mock.patch.dict(os.environ, {"HAPY_LANG": "eng"})
+    def test_read_next_number(self):
+        """test read number function"""
+
+        stream = InputStream("30.034")
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "num", "value": 30.034}
+        actual = ts.read_next()
+
+        self.assertEqual(expected, actual, "the stream is a number")
+
+    def test_read_next_string(self):
+        """test read number function"""
+
+        stream = InputStream('"Thank you Jesus"')
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "str", "value": "Thank you Jesus"}
+        actual = ts.read_next()
+
+        self.assertEqual(expected, actual, "the stream is a string")
+
+    def test_skip_comment(self):
+        """test read number function"""
+
+        stream = InputStream('#this is a comment!\n"Hello my friend!"')
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "str", "value": "Hello my friend!"}
+        actual = ts.read_next()
+
+        self.assertEqual(
+            expected, actual, "the stream is a comment, whitespace & string"
+        )
+
+    def test_read_identifier_keywords(self):
+        """test identifier function"""
+
+        stream = InputStream('return "goat"')
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "kw", "value": "return"}
+        actual = ts.read_next()
+
+        self.assertEqual(expected, actual, "the stream is a keyword")
+
+    def test_read_identifier_varnames1(self):
+        """test identifier function to identify variable names"""
+
+        stream = InputStream('cow = "animal"')
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "var", "value": "cow"}
+        actual = ts.read_next()
+
+        self.assertEqual(expected, actual, "the stream is an identifier")
+
+    def test_read_operator(self):
+        """test identifier function"""
+
+        stream1 = InputStream(">=")
+
+        ts1 = TokenStream(stream1)
+
+        expected1 = {"type": "op", "value": ">="}
+
+        actual1 = ts1.read_next()
+
+        # test multi character operator: => //
+        stream2 = InputStream("and")
+
+        ts2 = TokenStream(stream2)
+
+        expected2 = {"type": "op", "value": "and"}
+
+        actual2 = ts2.read_next()
+
+        self.assertEqual(
+            [expected1, expected2], [actual1, actual2], "the stream is a operation char"
+        )
+
+    def test_read_punctuation(self):
+        """test identifier function to identify variable names"""
+
+        stream = InputStream('{"cow": "animal"}')
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "punc", "value": "{"}
+
+        actual = ts.read_next()
+
+        self.assertEqual(expected, actual, "the stream is a punctuation mark")
+
+    def test_read_dot(self):
+        """test identifier function to identify dot operator"""
+        # we are treating the '.' as a binary operator in a sense
+
+        stream = InputStream('"hello".upper()')
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "op", "value": "."}
+
+        ts.read_next()  # first token
+        actual = ts.read_next()  # 2nd...
+
+        self.assertEqual(expected, actual, "Expected a dot token")
+
+    def test_import_statement_1(self):
+        """test token stream reading import tokens"""
+
+        stream = InputStream("import names;")
+
+        ts = TokenStream(stream)
+
+        expected = [
+            {"type": "kw", "value": "import"},
+            {"type": "var", "value": "names"},
+        ]
+
+        actual = [ts.read_next(), ts.read_next()]  # 2nd...
+
+        self.assertEqual(expected, actual, "Expected import and names keywords")
+
+    def test_forloop_statement_1(self):
+        """test token stream reading forloop statement"""
+
+        stream = InputStream("for (a in b) {\n print(a); };")
+
+        ts = TokenStream(stream)
+
+        expected = {"type": "kw", "value": "for"}
+
+        actual = ts.read_next()
+
+        self.assertEqual(expected, actual, "Expected for loop keyword")
+
+
+if __name__ == "__main__":
+    # NOTE: You have to set the env to "set HAPY_LANG=eng" if you want to
+    # test these in english.
+
+    # we should probably create a Hausa version of the tests :)
+    main()
```

