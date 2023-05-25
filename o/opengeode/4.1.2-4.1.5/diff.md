# Comparing `tmp/opengeode-4.1.2.tar.gz` & `tmp/opengeode-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengeode-4.1.2.tar", last modified: Thu May 11 12:27:00 2023, max compression
+gzip compressed data, was "opengeode-4.1.5.tar", last modified: Thu May 25 08:53:30 2023, max compression
```

## Comparing `opengeode-4.1.2.tar` & `opengeode-4.1.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-11 12:27:00.366375 opengeode-4.1.2/
--rw-r--r--   0 taste     (1001) taste     (1001)     4673 2022-05-15 08:02:36.000000 opengeode-4.1.2/FONT-LICENCE.txt
--rw-r--r--   0 taste     (1001) taste     (1001)     7651 2022-05-15 08:02:36.000000 opengeode-4.1.2/LICENSE
--rw-r--r--   0 taste     (1001) taste     (1001)       54 2022-05-15 08:02:36.000000 opengeode-4.1.2/MANIFEST.in
--rw-r--r--   0 taste     (1001) taste     (1001)    43963 2023-05-11 12:27:00.366375 opengeode-4.1.2/PKG-INFO
--rw-r--r--   0 taste     (1001) taste     (1001)    34436 2023-05-11 12:26:51.000000 opengeode-4.1.2/README.md
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-11 12:27:00.362375 opengeode-4.1.2/opengeode/
--rw-r--r--   0 taste     (1001) taste     (1001)   157418 2023-05-09 20:41:05.000000 opengeode-4.1.2/opengeode/AdaGenerator.py
--rwxr-xr-x   0 taste     (1001) taste     (1001)    13962 2022-09-04 10:24:18.000000 opengeode-4.1.2/opengeode/Asn1scc.py
--rw-r--r--   0 taste     (1001) taste     (1001)   116013 2022-11-13 15:59:02.000000 opengeode-4.1.2/opengeode/CGenerator.py
--rw-r--r--   0 taste     (1001) taste     (1001)    11750 2023-05-09 20:41:05.000000 opengeode-4.1.2/opengeode/Clipboard.py
--rw-r--r--   0 taste     (1001) taste     (1001)    29689 2022-12-08 11:28:57.000000 opengeode-4.1.2/opengeode/Connectors.py
--rw-r--r--   0 taste     (1001) taste     (1001)    38631 2022-11-26 14:13:17.000000 opengeode-4.1.2/opengeode/Helper.py
--rw-r--r--   0 taste     (1001) taste     (1001)    12719 2023-04-14 16:02:15.000000 opengeode-4.1.2/opengeode/Lander.py
--rw-r--r--   0 taste     (1001) taste     (1001)    82924 2023-01-22 14:09:04.000000 opengeode-4.1.2/opengeode/LlvmGenerator.py
--rw-r--r--   0 taste     (1001) taste     (1001)    18655 2023-05-10 20:42:44.000000 opengeode-4.1.2/opengeode/Pr.py
--rw-r--r--   0 taste     (1001) taste     (1001)     2462 2022-05-15 08:02:36.000000 opengeode-4.1.2/opengeode/QGenSDL.py
--rw-r--r--   0 taste     (1001) taste     (1001)    15873 2023-01-03 10:27:29.000000 opengeode-4.1.2/opengeode/Renderer.py
--rw-r--r--   0 taste     (1001) taste     (1001)    36467 2022-08-25 09:25:42.000000 opengeode-4.1.2/opengeode/Statechart.py
--rw-r--r--   0 taste     (1001) taste     (1001)    73348 2022-07-25 21:01:25.000000 opengeode-4.1.2/opengeode/StgBackend.py
--rw-r--r--   0 taste     (1001) taste     (1001)    18658 2022-11-04 15:55:28.000000 opengeode-4.1.2/opengeode/TextInteraction.py
--rw-r--r--   0 taste     (1001) taste     (1001)     1058 2022-05-15 08:02:36.000000 opengeode-4.1.2/opengeode/__init__.py
--rw-r--r--   0 taste     (1001) taste     (1001)    57607 2023-05-10 20:42:44.000000 opengeode-4.1.2/opengeode/genericSymbols.py
--rw-r--r--   0 taste     (1001) taste     (1001) 21475752 2023-02-01 06:37:57.000000 opengeode-4.1.2/opengeode/icons.py
--rw-r--r--   0 taste     (1001) taste     (1001)    44934 2023-05-09 20:41:05.000000 opengeode-4.1.2/opengeode/ogAST.py
--rw-r--r--   0 taste     (1001) taste     (1001)   337829 2023-05-10 20:42:44.000000 opengeode-4.1.2/opengeode/ogParser.py
--rw-r--r--   0 taste     (1001) taste     (1001)   160196 2023-05-11 12:26:51.000000 opengeode-4.1.2/opengeode/opengeode.py
--rw-r--r--   0 taste     (1001) taste     (1001)   183270 2023-05-10 20:42:44.000000 opengeode-4.1.2/opengeode/sdl92Lexer.py
--rw-r--r--   0 taste     (1001) taste     (1001)  4922318 2023-05-10 20:42:44.000000 opengeode-4.1.2/opengeode/sdl92Parser.py
--rw-r--r--   0 taste     (1001) taste     (1001)     2077 2022-10-06 09:09:20.000000 opengeode-4.1.2/opengeode/sdlHelp.py
--rw-r--r--   0 taste     (1001) taste     (1001)    64900 2023-05-10 20:42:44.000000 opengeode-4.1.2/opengeode/sdlSymbols.py
--rw-r--r--   0 taste     (1001) taste     (1001)     9445 2022-07-25 21:01:25.000000 opengeode-4.1.2/opengeode/undoCommands.py
--rw-r--r--   0 taste     (1001) taste     (1001)      358 2023-05-11 12:26:51.000000 opengeode-4.1.2/opengeode/version.py
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-11 12:27:00.366375 opengeode-4.1.2/opengeode.egg-info/
--rw-r--r--   0 taste     (1001) taste     (1001)    43963 2023-05-11 12:27:00.000000 opengeode-4.1.2/opengeode.egg-info/PKG-INFO
--rw-r--r--   0 taste     (1001) taste     (1001)      818 2023-05-11 12:27:00.000000 opengeode-4.1.2/opengeode.egg-info/SOURCES.txt
--rw-r--r--   0 taste     (1001) taste     (1001)        1 2023-05-11 12:27:00.000000 opengeode-4.1.2/opengeode.egg-info/dependency_links.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       61 2023-05-11 12:27:00.000000 opengeode-4.1.2/opengeode.egg-info/entry_points.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       10 2023-05-11 12:27:00.000000 opengeode-4.1.2/opengeode.egg-info/top_level.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       38 2023-05-11 12:27:00.366375 opengeode-4.1.2/setup.cfg
--rwxr-xr-x   0 taste     (1001) taste     (1001)     1220 2023-01-22 14:13:21.000000 opengeode-4.1.2/setup.py
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-25 08:53:30.980527 opengeode-4.1.5/
+-rw-r--r--   0 taste     (1001) taste     (1001)     4673 2022-05-15 08:02:36.000000 opengeode-4.1.5/FONT-LICENCE.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)     7651 2022-05-15 08:02:36.000000 opengeode-4.1.5/LICENSE
+-rw-r--r--   0 taste     (1001) taste     (1001)       54 2022-05-15 08:02:36.000000 opengeode-4.1.5/MANIFEST.in
+-rw-r--r--   0 taste     (1001) taste     (1001)    44280 2023-05-25 08:53:30.980527 opengeode-4.1.5/PKG-INFO
+-rw-r--r--   0 taste     (1001) taste     (1001)    34681 2023-05-25 08:53:21.000000 opengeode-4.1.5/README.md
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-25 08:53:30.980527 opengeode-4.1.5/opengeode/
+-rw-r--r--   0 taste     (1001) taste     (1001)   158021 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/AdaGenerator.py
+-rwxr-xr-x   0 taste     (1001) taste     (1001)    13961 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/Asn1scc.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   116013 2022-11-13 15:59:02.000000 opengeode-4.1.5/opengeode/CGenerator.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    11750 2023-05-09 20:41:05.000000 opengeode-4.1.5/opengeode/Clipboard.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    29689 2022-12-08 11:28:57.000000 opengeode-4.1.5/opengeode/Connectors.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    38556 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/Helper.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    12719 2023-04-14 16:02:15.000000 opengeode-4.1.5/opengeode/Lander.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    82924 2023-01-22 14:09:04.000000 opengeode-4.1.5/opengeode/LlvmGenerator.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    18655 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/Pr.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     2462 2022-05-15 08:02:36.000000 opengeode-4.1.5/opengeode/QGenSDL.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    15873 2023-01-03 10:27:29.000000 opengeode-4.1.5/opengeode/Renderer.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    36467 2022-08-25 09:25:42.000000 opengeode-4.1.5/opengeode/Statechart.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    73348 2022-07-25 21:01:25.000000 opengeode-4.1.5/opengeode/StgBackend.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    18658 2022-11-04 15:55:28.000000 opengeode-4.1.5/opengeode/TextInteraction.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     1058 2022-05-15 08:02:36.000000 opengeode-4.1.5/opengeode/__init__.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    57607 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/genericSymbols.py
+-rw-r--r--   0 taste     (1001) taste     (1001) 21475752 2023-02-01 06:37:57.000000 opengeode-4.1.5/opengeode/icons.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    45021 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/ogAST.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     9297 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/ogASTDumper.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   340546 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/ogParser.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   160565 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/opengeode.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   183270 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/sdl92Lexer.py
+-rw-r--r--   0 taste     (1001) taste     (1001)  4922318 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/sdl92Parser.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     2077 2022-10-06 09:09:20.000000 opengeode-4.1.5/opengeode/sdlHelp.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    64900 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/sdlSymbols.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     9445 2022-07-25 21:01:25.000000 opengeode-4.1.5/opengeode/undoCommands.py
+-rw-r--r--   0 taste     (1001) taste     (1001)      358 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/version.py
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-25 08:53:30.980527 opengeode-4.1.5/opengeode.egg-info/
+-rw-r--r--   0 taste     (1001) taste     (1001)    44280 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/PKG-INFO
+-rw-r--r--   0 taste     (1001) taste     (1001)      843 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/SOURCES.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)        1 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/dependency_links.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       61 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/entry_points.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       10 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/top_level.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       38 2023-05-25 08:53:30.980527 opengeode-4.1.5/setup.cfg
+-rwxr-xr-x   0 taste     (1001) taste     (1001)     1220 2023-01-22 14:13:21.000000 opengeode-4.1.5/setup.py
```

### Comparing `opengeode-4.1.2/FONT-LICENCE.txt` & `opengeode-4.1.5/FONT-LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/LICENSE` & `opengeode-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/PKG-INFO` & `opengeode-4.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengeode
-Version: 4.1.2
+Version: 4.1.5
 Summary: A free SDL editor for TASTE
 Home-page: http://opengeode.net
 Author: Maxime Perrotin
 Author-email: maxime.perrotin@esa.int
 License: UNKNOWN
 Description: ![OpenGEODE Logo](icons/opengeode4.png)
         
@@ -129,14 +129,23 @@
         There is no runtime, and the generated code is not subject to any license.
         
         The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
         The background pattern was downloaded from www.subtlepatterns.com
         
         Changelog
         =========
+        **4.1.5 (05/2023)**
+        - Fix computation of modulo operator range
+        
+        **4.1.4 (05/2023)**
+        - Fix support for built-in operators (Val, To_Enum, etc) / Ada backend
+        
+        **4.1.3 (05/2023)**
+        - Fix type signed/unsigned potential mismatches when using syntypes
+        
         **4.1.2 (05/2023)**
         - Maintenance relaase - text search work cross-partitions
         
         **4.1.1 (05/2023)**
         - Maintenance relaase - minor bugfixes (placement of comments, partitions)
         
         **4.1.0 (05/2023)**
```

### Comparing `opengeode-4.1.2/README.md` & `opengeode-4.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,23 @@
 There is no runtime, and the generated code is not subject to any license.
 
 The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
 The background pattern was downloaded from www.subtlepatterns.com
 
 Changelog
 =========
+**4.1.5 (05/2023)**
+- Fix computation of modulo operator range
+
+**4.1.4 (05/2023)**
+- Fix support for built-in operators (Val, To_Enum, etc) / Ada backend
+
+**4.1.3 (05/2023)**
+- Fix type signed/unsigned potential mismatches when using syntypes
+
 **4.1.2 (05/2023)**
 - Maintenance relaase - text search work cross-partitions
 
 **4.1.1 (05/2023)**
 - Maintenance relaase - minor bugfixes (placement of comments, partitions)
 
 **4.1.0 (05/2023)**
```

### Comparing `opengeode-4.1.2/opengeode/AdaGenerator.py` & `opengeode-4.1.5/opengeode/AdaGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     ri_stub_ads = []
     ri_stub_adb = []
 
     # CHOICE selector types: we created an ASN.1 type to access them
     # (in Helper.generate_asn1_datamodel), but we need conversion functions
     choice_selections = []
     for sortname, sortdef in process.user_defined_types.items():
-        if sortdef.type.kind == "EnumeratedType":
+        if sortdef.type.kind == "EnumeratedType" and sortdef.AddedType == "True":
             choiceTypeModule = process.mapping_sort_module[sortdef.ChoiceTypeName].replace('-', '_')
             sortAda = sortname.replace('-', '_')
             fromMod = f'{choiceTypeModule}.{ASN1SCC}{sortAda}'
             toMod = f'{process.name}_Datamodel.{ASN1SCC}{process.name}_{sortAda}'
             choice_selections.append(
                     f"function To_{sortAda} (Src : {fromMod}) return {toMod} is ({toMod}'Enum_Val (Src'Enum_Rep));")
 
@@ -424,16 +424,15 @@
                 'begin',
                 'Startup;'])
 
     # Generate the TASTE template
     try:
         asn1_modules = '\n'.join([f"with {dv.replace('-', '_')};\nuse {dv.replace('-', '_')};"
                                   for dv in process.asn1Modules])
-        if process.asn1Modules:
-            asn1_modules += '\nwith adaasn1rtl;\nuse adaasn1rtl;'
+        asn1_modules += '\nwith adaasn1rtl;\nuse adaasn1rtl;'
     except TypeError:
         asn1_modules = '--  No ASN.1 data types are used in this model'
 
     taste_template = [f'''\
 -- This file was generated automatically by OpenGEODE: DO NOT MODIFY IT !
 
 {"with Text_IO; use Text_IO;" if process.dependencies["writeln"] else ""}
@@ -1722,14 +1721,20 @@
             error = f'{exp.inputString} is not a CHOICE'
             LOG.error(error)
             raise TypeError(error)
         param_stmts, param_str, local_var = expression(exp, readonly=1)
         stmts.extend(param_stmts)
         local_decl.extend(local_var)
         ada_string += f'To_{exp_typename}_Selection ({param_str}.Kind)'
+        # Finally we have to change the type name, because the
+        # function To_<type>_Selection function returns a type
+        # created by the Helper.generate_asn1_datamodel function
+        # and containing a prefix - not known by ogParser.
+        # No, this is now done properly in ogParser
+        #prim.exprType.ReferencedTypeName = f'{PROCESS_NAME}-{prim.exprType.ReferencedTypeName}'
 
     elif ident == 'choice_to_int':
         p1, p2 = params
         sort = find_basic_type (p1.exprType)
         assert (sort.kind == 'ChoiceType')  # normally checked by the parser
         param_stmts, varstr, local_var = expression(p1, readonly=1)
         stmts.extend(param_stmts)
@@ -1799,35 +1804,44 @@
         destSort = target_type.value[0]
         sortAda = destSort.replace('-', '_')
         sort_name = f'{PROCESS_NAME}_Datamodel.{ASN1SCC}{PROCESS_NAME}_{sortAda}_selection'
         if ident == 'to_selector':
             ada_string += f"{sort_name}'Val ({ASN1SCC}{var_typename}'Pos ({var_str}))"
         elif ident == 'to_enum':
             sort_name_val = f'{ASN1SCC}{sortAda}'
-            sort_name = f'{PROCESS_NAME}_Datamodel.{ASN1SCC}{PROCESS_NAME}_{var_typename}'
+            sort_name = f'{PROCESS_NAME}_Datamodel.{ASN1SCC}{var_typename}'
             ada_string += f"{sort_name_val}'Val ({sort_name}'Pos ({var_str}))"
 
     elif ident == 'val':
         variable, target_type = params
         var_typename = type_name (variable.exprType)
         var_stmts, var_str, var_decl = expression (variable, readonly=1)
         stmts.extend(var_stmts)
         local_decl.extend(var_decl)
         sort_name = ASN1SCC + target_type.value[0].replace('-', '_')
         ada_string += f"{sort_name}'Enum_Val ({var_str})"
 
     elif ident == 'num':
         # User wants to get an enumerated corresponding integer value
         exp = params[0]
-        exp_typename = type_name(exp.exprType)
         param_stmts, param_str, local_var = expression(exp, readonly=1)
+        # the type of the parameter may have been altered in case of
+        # the 'present' operator, so it is read only after the expression
+        # has been processed.
+        exp_typename = type_name(exp.exprType)
         # 'Enum_Rep gives directly the universal integer of an enumerated
         # (was in GNAT, now in Ada 2020)
         stmts.extend(param_stmts)
         local_decl.extend(local_var)
+        if not isinstance(exp, ogAST.PrimVariable):
+            # Enum_Rep only works on variables
+            tmp_id = f"tmp{exp.tmpVar}"
+            local_decl.append(f"{tmp_id} : {exp_typename};")
+            stmts.append(f"{tmp_id} := {param_str};")
+            param_str = tmp_id
         ada_string += f"{param_str}'Enum_Rep"
 
     elif ident == 'floor':
         exp = params[0]
         exp_typename = type_name(exp.exprType)
         param_stmts, param_str, local_var = expression(exp, readonly=1)
         stmts.extend(param_stmts)
@@ -2217,28 +2231,24 @@
             isinstance(expr.right, (ogAST.PrimOctetStringLiteral,
                                     ogAST.PrimBitStringLiteral)):
         # If right is an octet string or bit string literal, use the numerical
         # value directly.
         right_str = str(expr.right.numeric_value)
         strings.append(f"{left_str} := {right_str};")
     elif basic_left.kind.startswith('Integer'):
-#       print '\nASSIGN:', expr.inputString,
-#       print "Left type = ",type_name(find_basic_type (expr.left.exprType)),
-#       print "- Right type = ",type_name(find_basic_type (expr.right.exprType))
 
-        # Make sure that integers are cast to 64 bits
+        # Make sure that integers are cast if needed
         # It is possible that left and right are of different types
         # (signed vs unsigned and/or 32 bits vs 64 bits).
         # The parser should have ensured that the ranges are compatible.
         # We can therefore safely cast to the left type
         basic_right = find_basic_type (expr.right.exprType)
         cast_left, cast_right = type_name(basic_left), type_name(basic_right)
-        #print (cast_left, cast_right, right_str)
         if cast_left != cast_right:
-            res = f'{cast_left} ({right_str})'
+            res = f'{type_name(expr.left.exprType)} ({right_str})'
         else:
             if hasattr (expr.right, "expected_type") \
                     and expr.right.expected_type is not None:
 
                 cast_expected = type_name (expr.right.expected_type)
                 if cast_expected != cast_left:
                     res = f'{cast_left} ({right_str})'
```

### Comparing `opengeode-4.1.2/opengeode/Asn1scc.py` & `opengeode-4.1.5/opengeode/Asn1scc.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             #"IsStandardEnum" : False
             }) for key in each.type.Children.keys()
         }
         full_sort = \
                 type(new_sort_name, (object,), {
                     "Line": each.Line,
                     "CharPositionInLine": each.CharPositionInLine,
-                    "AddedType" : "False",
+                    "AddedType" : "True",
                     "ChoiceTypeName" : each.__name__,
                     "type": type(new_sort_name + "_type", (object,), {
                         "Line" : each.Line,
                         "CharPositionInLine": each.CharPositionInLine,
                         "kind": "EnumeratedType",
                         "Extensible": "False",
                         "ValuesAutoCalculated": "False",
```

### Comparing `opengeode-4.1.2/opengeode/CGenerator.py` & `opengeode-4.1.5/opengeode/CGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/Clipboard.py` & `opengeode-4.1.5/opengeode/Clipboard.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/Connectors.py` & `opengeode-4.1.5/opengeode/Connectors.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/Helper.py` & `opengeode-4.1.5/opengeode/Helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 import logging
 from itertools import chain
 from collections import defaultdict
 
 from functools import singledispatch
 
 from . import ogAST
+from . import ogParser
 
 LOG = logging.getLogger(__name__)
 DEFAULT_SEPARATOR='_0_'
 ASN1SCC = 'asn1Scc'
 
 __all__ = ['flatten', 'rename_everything', 'inner_labels_to_floating',
            'map_input_state', 'sorted_fields', 'state_aggregations',
@@ -258,15 +259,14 @@
             inp.transition_id += trans_idx
 
         process.mapping.update(state.mapping)
         process.cs_mapping.update(state.cs_mapping)
 
         # If composite state has entry procedures, add the call
         if state.entry_procedure:
-            #print(state.mapping)
             for each in (trans for trans in state.mapping.values()
                          if isinstance(trans, int)):
                 call_entry = ogAST.ProcedureCall()
                 call_entry.inputString = 'entry'
                 entryproc = f'{prefix}entry'
                 call_entry.output = [{'outputName': entryproc,
                                      'params': [], 'tmpVars': []}]
@@ -685,22 +685,15 @@
     return (x[0] for x in sorted(tmp, key=operator.itemgetter(1,2)))
 
 
 def find_basic_type(TYPES, a_type):
     ''' Return the ASN.1 basic type of a_type.
     TYPES is process.dataview
     '''
-    basic_type = a_type
-    while basic_type.kind == 'ReferenceType':
-        # Find type with proper case in the data view
-        for typename in TYPES.keys():
-            if typename.lower() == basic_type.ReferencedTypeName.lower():
-                basic_type = TYPES[typename].type
-                break
-    return basic_type
+    return ogParser.find_basic_type(a_type, TYPES)
 
 
 def generate_asn1_datamodel(process: ogAST.Process, SEPARATOR: str=DEFAULT_SEPARATOR) -> None:
     ''' Generate an ASN.1 model containing:
           - the state definition
           - a type describing the SDL context
           - all user-defined SDL type (NEWTYPEs, SYNTYPEs...)
@@ -782,14 +775,17 @@
 
     asn1_template.append(asn1_context)
 
     # Add user-defined NEWTYPEs, SYNTYPEs and CHOICE selector types
     choice_selections = []
     # a newtype may reuse another newtype, so we must update the list:
     types_with_proper_case.extend(process.user_defined_types.keys())
+    # We also add the newly created types for choice selectors to the
+    # visible list of types. they are needed a return types for the
+    # To_<type>_Selection functions in backends
     for sortname, sortdef in process.user_defined_types.items():
         if sortdef.type.kind == "SequenceOfType":
             rangeMin = sortdef.type.Min
             rangeMax = sortdef.type.Max
             refType  = sortdef.type.type.ReferencedTypeName
             for refTypeCase in types_with_proper_case:
                 if refTypeCase.lower().replace('-', '_') == \
@@ -797,22 +793,22 @@
                     break
             else:
                 LOG.error(f"Type not found: {refType}")
             asn1_template.append(
                     f'{sortname.replace("_", "-").capitalize()} ::= SEQUENCE '
                     f'(SIZE ({rangeMin} .. {rangeMax})) OF '
                     f'{refTypeCase.replace("_", "-")}')
-        elif sortdef.type.kind == "EnumeratedType":
+        elif sortdef.type.kind == "EnumeratedType" and sortdef.AddedType=="False":
             # At the moment, the only user-defined ENUMERATED types that are
             # supported are the ones generated for the CHOICE selectors
             # We can therefore safely rename them systematically here,
             # by using the process name as prefix, to avoid any risk of
             # duplicate type definition in case it exists in another SDL
             # process of the system.
-            prefixed_name = f'{process.name}_{sortdef.ChoiceTypeName}_selection '
+            prefixed_name = f'{process.name}_{sortdef.ChoiceTypeName}_selection'
             keys = []
             for idx, key in enumerate(sortdef.type.EnumValues.keys()):
                 # give an index to the enumerations to align with -selection
                 # types used in choice index
                 keys.append(f'{key}-present({idx+1})')
             asn1_template.append(
                     f'{prefixed_name.replace("_", "-").title()} ::= ENUMERATED {{' + ", ".join(keys) + '}')
@@ -823,15 +819,14 @@
     asn1_template.append('END\n')
 
     # Write the ASN.1 file
     with open(process.name.lower() + '_datamodel.asn', 'w') as asn1_file:
         asn1_file.write('\n'.join(asn1_template))
 
 
-
 def code_generation_preprocessing(process, separator=DEFAULT_SEPARATOR):
     ''' Do all sorts of preprocessing before invoking a code generator
         and update the AST of the process
     '''
     # In case model has nested states, flatten everything
     flatten(process, sep=separator)
```

### Comparing `opengeode-4.1.2/opengeode/Lander.py` & `opengeode-4.1.5/opengeode/Lander.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/LlvmGenerator.py` & `opengeode-4.1.5/opengeode/LlvmGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/Pr.py` & `opengeode-4.1.5/opengeode/Pr.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/QGenSDL.py` & `opengeode-4.1.5/opengeode/QGenSDL.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/Renderer.py` & `opengeode-4.1.5/opengeode/Renderer.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/Statechart.py` & `opengeode-4.1.5/opengeode/Statechart.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/StgBackend.py` & `opengeode-4.1.5/opengeode/StgBackend.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/TextInteraction.py` & `opengeode-4.1.5/opengeode/TextInteraction.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/__init__.py` & `opengeode-4.1.5/opengeode/__init__.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/genericSymbols.py` & `opengeode-4.1.5/opengeode/genericSymbols.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/icons.py` & `opengeode-4.1.5/opengeode/icons.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/ogAST.py` & `opengeode-4.1.5/opengeode/ogAST.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,14 +941,16 @@
 
 
 class Procedure:
     ''' Internal procedure definition '''
     def __init__(self):
         ''' Procedure AST default value '''
         self.inputString = ''
+        # keep track of the process name for the context
+        self.processName = ''
         self.line = None
         self.charPositionInLine = None
         # Set default coordinates and width/height
         self.pos_x = self.pos_y = None
         self.width = 70
         self.height = 35
         # Optional hyperlink
```

### Comparing `opengeode-4.1.2/opengeode/ogParser.py` & `opengeode-4.1.5/opengeode/ogParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
 lineno = lambda : currentframe().f_back.f_lineno
 
 # user may create SDL (non-asn1) types with the newtype keyword
 # they are stored in a dedicated dictionary with the same structure
 # as the ASN1SCC generated python AST
 USER_DEFINED_TYPES = dict()
 CHOICE_SELECTORS = dict()
+g_choice_selectors_ignore_list = list()
 
 
 def types():
     ''' Return all ASN.1 and user defined types '''
     ret = getattr(DV, 'types', {}).copy()
     ret.update(USER_DEFINED_TYPES)
     return ret
@@ -567,33 +568,33 @@
 def find_basic_type(a_type, pool=None):
     ''' Return the ASN.1 basic type of a_type '''
     basic_type = a_type or UNKNOWN_TYPE
     pool = pool or types()
     while basic_type.kind == 'ReferenceType':
         Min = getattr(basic_type, "Min", None)
         Max = getattr(basic_type, "Max", None)
+        name = basic_type.ReferencedTypeName.replace('_', '-').lower()
 
         # Find type with proper case in the data view
         for typename in pool.keys():
-            if typename.lower() == basic_type.ReferencedTypeName.lower():
+            if typename.replace('_', '-').lower() == name:
                 basic_type = pool[typename].type
                 if Min is not None and Max is not None \
                         and (is_numeric(basic_type, pool)
                                 or is_string(basic_type, pool)
                                 or is_sequenceof(basic_type, pool)):
                     # Subtypes may have defined subranges
                     new_type = type('Subtype',  basic_type.__bases__,
                             dict (basic_type.__dict__))
                     new_type.Min = Min
                     new_type.Max = Max
                     basic_type = new_type
                 break
         else:
-            raise TypeError('Type "' + type_name(basic_type) +
-                            '" was not found in Dataview')
+            raise TypeError(f'Type "{name}" was not found in Dataview')
     return basic_type
 
 def find_type_name(a_type, pool=None) -> str:
     ''' A Type may be an alias of another type, if it has a ReferencedTypeName
     and the same constraints as the referenced type. This function finds the
     name of the original type definition '''
     if a_type.kind != 'ReferenceType':
@@ -739,45 +740,51 @@
             if sort.lower().replace('-', '_') == \
                     sort_name.lower().replace('-', '_'):
                 break
         else:
             raise TypeError(name + ': type ' + sort_name + 'not found')
         # we could check if the range of the number is compatible with the
         # number of values...
-        return_type = types()[sort].type
+        return_type = new_ref_type(sort) #types()[sort].type
         return (return_type, warnings)
 
     elif name in ('to_selector', 'to_enum'):
         if len(params) != 2:
             raise TypeError(name + " takes 2 parameters: variable, type")
         variable, target_type = params
+        #breakpoint()
         variable_sort = find_basic_type(variable.exprType)
         if variable_sort.kind == 'UnknownType':
             raise TypeError(name + ': variable not found (parameter 1)')
         if variable_sort.kind != 'EnumeratedType':
             raise TypeError(name + ': First parameter is not an enumerated')
         sort_name = target_type.value[0]  #  raw string of the type to cast
+
         for sort in types().keys():
             if sort.lower().replace('-', '_') == \
                     sort_name.lower().replace('-', '_'):
                 break
         else:
             raise TypeError(name + ': type ' + sort_name + 'not found')
         # check that the list of enumerants are identical. unfortunately we
         # cannot check the ordering, as it is an unordered dict
         if name == 'to_selector':
             # if the sort is a subtype, it may not have a -selection suffix
             # and an exception may be raised. FIXME : check "present" operator
             # as the issue is already fixed there
-            return_type = types()[sort.title() + '-selection'].type
-        else:
-            return_type = types()[sort].type
-        if return_type.kind != 'EnumeratedType':
+            return_type = new_ref_type(f'{sort.title()}-selection')
+            #return_type = types()[sort.title() + '-selection'].type
+            base_sort = types()[sort.title() + '-selection'].type
+        else:
+            return_type = new_ref_type(sort)
+            #return_type = types()[sort].type
+            base_sort = types()[sort].type
+        if base_sort.kind != 'EnumeratedType':
             raise TypeError(name + ': Second parameter is incorrect')
-        return_type_keys = return_type.EnumValues.keys()
+        return_type_keys = base_sort.EnumValues.keys()
         variable_sort_keys = variable_sort.EnumValues.keys()
         if return_type_keys != variable_sort_keys:
             raise TypeError(name + ': Enumerated type are not equivalent')
         return (return_type, warnings)
     elif name == 'observer_status':
         if len(params) != 0:
             raise TypeError(f'{name} does not take any parameter')
@@ -937,15 +944,20 @@
         try:
             while sort.kind == "ReferenceType":
                 sort_name = sort.ReferencedTypeName
                 sort = types()[sort.ReferencedTypeName].type
         except AttributeError:
             # Native choice types don't have the kind field here
             pass
-        return (types()[sort_name.title() + "-selection"].type, warnings)
+        # we must return a referenced type, otherwise the present operator
+        # could not be used as the parameter of a function that needs to
+        # know the type of the parameter to cast or prefix it (e.g. to_enum)
+        selection_type = new_ref_type(f'{context.processName}-{sort_name.title()}-selection')
+        return (selection_type, warnings)
+        #return (types()[sort_name.title() + "-selection"].type, warnings)
 
     # choice_to_int: returns an integer corresponding to either the currently
     # selected choice value (e.g. foo in CHOICE { foo INTEGER (..), ... } when
     # foo is the current choice). or a default, user-defined value if the
     # current choice is not numerical. The first parameter is an instance of
     # a CHOICE type, and the second parameter is the default value.
     elif name == 'choice_to_int':
@@ -1552,35 +1564,48 @@
     else:
         raise TypeError('Incompatible types {} and {}'.format(
             type_name(type_a),
             type_name(type_b)
         ))
 
 def find_variable_type(var, context):
-    ''' Look for a variable name in the context and return its type '''
+    ''' Look for a variable name in the context and return its type
+    If the type is a choice selector (-selection), return the name
+    prefixed with the process name.
+    '''
+    def selector(sort):
+        ''' check if the type is defined in the CHOICE_SELECTORS
+        and return the type with the process name prefix if so '''
+        name = type_name(sort)
+        if name in CHOICE_SELECTORS.keys():
+            base_name = CHOICE_SELECTORS[name].ChoiceTypeName
+            for sortname, sortvalue in CHOICE_SELECTORS.items():
+                if sortvalue.ChoiceTypeName == base_name and sortvalue != CHOICE_SELECTORS[name]:
+                    return new_ref_type(sortname)
+        return sort
 
     # all DCL-variables
     all_visible_variables = dict(context.global_variables)
     all_visible_variables.update(context.variables)
     all_visible_variables.update(context.monitors)
     all_visible_variables.update(context.global_monitors)
 
     # First check locally, i.e. in FPAR
     try:
         for variable in context.fpar:
             if variable['name'].lower() == var.lower():
-                return variable['type']
+                return selector(variable['type'])
     except AttributeError:
         # No FPAR section
         pass
 
     for varname, (vartype, _) in all_visible_variables.items():
         # Case insensitive comparison with variables
         if var.lower() == varname.lower():
-            return vartype
+            return selector(vartype)
 
     for timer in chain(context.timers, context.global_timers):
         if var.lower() == timer.lower():
             return TIMER
 
     # check if it is an ASN.1 constant
     for varname, vartype in chain(DV.variables.items(),
@@ -2371,17 +2396,20 @@
                 msg = "Negative ranges and modulo don't fit well. " \
                         "Use with caution (check Wikipedia for details)"
                 warnings.append(warning(root, msg))
             if minR == 0 or maxR == 0:
                 msg = f'Modulo: range [{minR} .. {maxR}] allows division by zero'
                 errors.append(error(root, msg))
             else:
-                possible_values = [minL % minR, minL % maxR, maxL % minR, maxL % maxR]
-                bounds["Min"] = min(possible_values)
-                bounds["Max"] = max(possible_values)
+                # no the following is wrong
+                #possible_values = [minL % minR, minL % maxR, maxL % minR, maxL % maxR]
+                #bounds["Min"] = min(possible_values)
+                #bounds["Max"] = max(possible_values)
+                bounds["Min"] = min([minL, minR - 1])
+                bounds["Max"] = min([maxL, maxR - 1])
         else:
             bounds = find_bounds(expr.op, minL, maxL, minR, maxR)
 
         if is_number(basic_right) or is_number(basic_left):
             is_signed = (not is_number(basic_right))   and minR < 0.0 \
                         or (not is_number(basic_left)) and minL < 0.0
 
@@ -3423,14 +3451,15 @@
     if root.type == lexer.COMPOSITE_STATE:
         comp = ogAST.CompositeState()
     elif root.type == lexer.STATE_AGGREGATION:
         comp = ogAST.StateAggregation()
     errors, warnings = [], []
     # Create a list of all inherited data
     try:
+        comp.processName = context.processName
         comp.global_variables = dict(context.variables)
         comp.global_variables.update(context.global_variables)
         comp.global_monitors = dict(context.monitors)
         comp.global_monitors.update(context.global_monitors)
         comp.global_timers = list(context.timers)
         comp.global_timers.extend(list(context.global_timers))
         comp.input_signals = context.input_signals
@@ -3596,14 +3625,20 @@
 
 def procedure_pre(root, parent=None, context=None):
     ''' Parse a procedure interface - the content has to be parsed after
         all procedure interfaces are known, to prevent missing references '''
     errors = []
     warnings = []
     proc = ogAST.Procedure()
+    # propagate the process name if available
+    try:
+        proc.processName = context.processName
+    except AttributeError:
+        # no processname if procedure is declared at system level
+        pass
     content = []
 
     for child in root.getChildren():
         if child.type == lexer.CIF:
             # Get symbol coordinates
             proc.pos_x, proc.pos_y, proc.width, proc.height = cif(child)
         elif child.type == lexer.SYMBOLID:
@@ -4161,15 +4196,14 @@
     refbasic = find_basic_type(reftype)
     if hasattr(refbasic, "Min") and hasattr(refbasic, "Max") and \
        (int(refbasic.Min) > foundMin or int(refbasic.Max) < foundMax):
         errors.append(error(root, f"{line}:{char} Range [{foundMin}, {foundMax}] exceeds the capacity of the parent type"))
 
     LOG.debug(f"{line}:{char} Found range: for {newtypename}: [{foundMin}, {foundMax}]")
 
-
     asnName = newtypename.replace('_', '-')
     newtype = type(asnName, (object,), {
         "Line": -1,
         "CharPositionInLine": int(char),
         "CName": newtypename,
         "AddedType": "False",
         "type": type(f"{asnName}_type", (object,), {
@@ -4800,21 +4834,42 @@
     # we set or not the "self" variable)
     for child in root.getChildren():
         if child.type == lexer.ID:
             process.processName = child.text
             process.path = [f'PROCESS {process.processName}']
         elif child.type == lexer.TYPE:
             process.process_type = True
+        elif child.type == lexer.TYPE_INSTANCE:
+            # PROCESS Toto:ParentType;
+            process.instance_of_name = child.children[0].text
  
     # Create implicit "sender" identifier of type PID.
     if 'PID' in types().keys():
         parseSingleElement('content', 'dcl sender, offspring PID := env;', context=process)
 
+    # The choice selectors were added by the Asn1scc module. We need to duplicate
+    # these types but with the process name as a prefix. This is needed to support
+    # the num() and to_enum() operators, that allow user to access the choice
+    # selectors as enumerated types.
+    addedTypes = dict()
+    for name, sort in CHOICE_SELECTORS.items():
+        if name in g_choice_selectors_ignore_list or process.instance_of_name is not None:
+            # the function may be called multiple times, so avoid duplicates
+            continue
+        prefixed_name = f'{process.processName.title()}-{name}'
+        g_choice_selectors_ignore_list.append(prefixed_name)
+        newsort = type(prefixed_name, (sort,), sort.__dict__.copy())
+        newsort.AddedType = "False"
+        addedTypes[prefixed_name] = newsort
+    CHOICE_SELECTORS.update(addedTypes)
+
     # first look for all text areas to find NEWTYPE, SYNTYPE and SYNONYM declarations
+    global USER_DEFINED_TYPES
     USER_DEFINED_TYPES = CHOICE_SELECTORS.copy()
+
     process.user_defined_types = USER_DEFINED_TYPES
     tas = (x for x in root.getChildren() if x.type == lexer.TEXTAREA)
     for child in tas:
         content = (x for x in child.getChildren()
                    if x.type == lexer.TEXTAREA_CONTENT)
         for each in content:
             newtypes = (x for x in each.getChildren()
@@ -4962,16 +5017,16 @@
         elif child.type == lexer.REFERENCED:
             process.referenced = True
         elif child.type == lexer.TYPE:
             # Already set above
             pass
             #process.process_type = True
         elif child.type == lexer.TYPE_INSTANCE:
-            # PROCESS Toto:ParentType;
-            process.instance_of_name = child.children[0].text
+            # Already set above
+            pass
         elif child.type == lexer.COMMENT:
             process.comment, _, _ = end(child)
         else:
             warnings.append(['Unsupported process definition child: ' +
                              sdl92Parser.tokenNamesMap[child.type] +
                             ' - line ' + str(child.getLine()),
                             [proc_x, proc_y], []])
```

### Comparing `opengeode-4.1.2/opengeode/opengeode.py` & `opengeode-4.1.5/opengeode/opengeode.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
               sdl92Parser,  # NOQA
               genericSymbols,  # NOQA
               Asn1scc,  # NOQA
               sdlSymbols,
               AdaGenerator,
               ogParser,
               ogAST,
+              ogASTDumper,
               Renderer,
               Clipboard,
               Statechart,
               Lander,
               Helper,
               Pr,
               CGenerator,
@@ -111,14 +112,15 @@
 
 # Logging: ist of properly loaded modules that will use it
 LOG = logging.getLogger(__name__)
 MODULES : List[types.ModuleType] = [
     sdlSymbols,
     genericSymbols,
     ogAST,
+    ogASTDumper,
     ogParser,
     Lander,
     AdaGenerator,
     undoCommands,
     Renderer,
     Clipboard,
     Statechart,
@@ -2316,15 +2318,15 @@
 
         otherAsn1Files.append(f'code/{prj_name}_datamodel.asn')
         otherAsn = " ".join(otherAsn1Files)
 
         #  Template for the Makefile
         template_makefile = f'''all:
 \tmkdir -p code
-\tcd code && opengeode --toAda {first_pr} {other_pr}
+\tcd code && opengeode --toAda ../*.pr
 \tasn1scc -fp AUTO -typePrefix asn1Scc -o code -equal -Ada {firstAsn1File} {otherAsn}
 \tcd code && gnat make {prj_name}
 clean:
 \trm -rf code'''
         pr_data = str('\n'.join(pr_raw))
         try:
             pr_file.write(pr_data.encode('utf-8'))
@@ -3217,32 +3219,36 @@
 
         scene = self.view.scene()
         top_scene = self.view.top_scene()
 
         # check if the default partition is assigned to a process scene
         # already, and if not try to do it (if any such scene exists)
         default_part = partitions.child(0)
-        default_part_scene = default_part.data(0, SCENE)
-        if not default_part_scene:
+        if default_part:
+            default_part_scene = default_part.data(0, SCENE)
+        else:
+            default_part_scene = None
+        if default_part and not default_part_scene:
             for each in chain([top_scene], scene.all_nested_scenes):
                 if each.context == 'process':
                     default_part.setData(0, SCENE, each)
                     break
 
         # keep an up to date list of partition at the top-level scene
         # and update the partition name in each scene
         top_scene.partitions.clear()
         for idx in range(partitions.childCount()):
             part = partitions.child(idx)
             part_name = part.text(0)
             part_scene = part.data(0, SCENE)
-            top_scene.partitions[part_name] = part_scene
-            part_scene.partitions = top_scene.partitions
-            # Update the partition name for the scene
-            part_scene.partition_name = part_name
+            if part_scene:
+                top_scene.partitions[part_name] = part_scene
+                part_scene.partitions = top_scene.partitions
+                # Update the partition name for the scene
+                part_scene.partition_name = part_name
 
         if scene.context == 'block':
             for each in (in_sig, out_sig, states,
                          labels, dcl, timers, procedures):
                 change_state(each, True)
         elif scene.context == 'process':
             for each in (in_sig, out_sig, states,
@@ -3447,14 +3453,16 @@
 def parse_args():
     ''' Parse command line arguments '''
     parser = argparse.ArgumentParser()
     parser.add_argument('-v', '--version', action='version',
                         version=__version__)
     parser.add_argument('-g', '--debug', action='store_true', default=False,
             help='Display debug information')
+    parser.add_argument('--dumpAST', action='store_true', default=False,
+            help='Dump AST to the file')
     parser.add_argument('--simu', action='store_true', default=False,
             help='Generate additional code for the taste simulation mode')
     parser.add_argument('--stg', type=str, metavar='file',
             help='Generate code using a custom String Template file')
     parser.add_argument('--check', action='store_true', dest='check',
             help='Check a .pr file for syntax and semantics')
     parser.add_argument('--toAda', dest='toAda', action='store_true',
@@ -3636,14 +3644,17 @@
     try:
         ast, warnings, errors = parse(options.files)
     except IOError as err:
         LOG.error('Aborting due to parsing error')
         LOG.error(str(err))
         return 1
 
+    if options.dumpAST:
+        ogASTDumper.dump('ast.dump', ast)
+
     if len(ast.processes) != 1:
         LOG.error(f'Found {len(ast.processes)} process(es) instead of one')
         return 1
 
     if options.png or options.pdf or options.svg:
         export(ast, options)
 
@@ -3726,15 +3737,15 @@
     options = parse_args()
 
     init_logging(options)
 
     LOG.debug('Starting OpenGEODE version ' + __version__)
     if any((options.check, options.toAda, options.png, options.pdf,
             options.svg, options.llvm, options.simu, options.stg,
-            options.toC)):
+            options.toC, options.dumpAST)):
         return cli(options)
     else:
         return gui(options)
 
 
 if __name__ == '__main__':
     ''' Run main application '''
```

### Comparing `opengeode-4.1.2/opengeode/sdl92Lexer.py` & `opengeode-4.1.5/opengeode/sdl92Lexer.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/sdl92Parser.py` & `opengeode-4.1.5/opengeode/sdl92Parser.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/sdlHelp.py` & `opengeode-4.1.5/opengeode/sdlHelp.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/sdlSymbols.py` & `opengeode-4.1.5/opengeode/sdlSymbols.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode/undoCommands.py` & `opengeode-4.1.5/opengeode/undoCommands.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.2/opengeode.egg-info/PKG-INFO` & `opengeode-4.1.5/opengeode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengeode
-Version: 4.1.2
+Version: 4.1.5
 Summary: A free SDL editor for TASTE
 Home-page: http://opengeode.net
 Author: Maxime Perrotin
 Author-email: maxime.perrotin@esa.int
 License: UNKNOWN
 Description: ![OpenGEODE Logo](icons/opengeode4.png)
         
@@ -129,14 +129,23 @@
         There is no runtime, and the generated code is not subject to any license.
         
         The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
         The background pattern was downloaded from www.subtlepatterns.com
         
         Changelog
         =========
+        **4.1.5 (05/2023)**
+        - Fix computation of modulo operator range
+        
+        **4.1.4 (05/2023)**
+        - Fix support for built-in operators (Val, To_Enum, etc) / Ada backend
+        
+        **4.1.3 (05/2023)**
+        - Fix type signed/unsigned potential mismatches when using syntypes
+        
         **4.1.2 (05/2023)**
         - Maintenance relaase - text search work cross-partitions
         
         **4.1.1 (05/2023)**
         - Maintenance relaase - minor bugfixes (placement of comments, partitions)
         
         **4.1.0 (05/2023)**
```

### Comparing `opengeode-4.1.2/opengeode.egg-info/SOURCES.txt` & `opengeode-4.1.5/opengeode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 opengeode/Statechart.py
 opengeode/StgBackend.py
 opengeode/TextInteraction.py
 opengeode/__init__.py
 opengeode/genericSymbols.py
 opengeode/icons.py
 opengeode/ogAST.py
+opengeode/ogASTDumper.py
 opengeode/ogParser.py
 opengeode/opengeode.py
 opengeode/sdl92Lexer.py
 opengeode/sdl92Parser.py
 opengeode/sdlHelp.py
 opengeode/sdlSymbols.py
 opengeode/undoCommands.py
```

### Comparing `opengeode-4.1.2/setup.py` & `opengeode-4.1.5/setup.py`

 * *Files identical despite different names*

