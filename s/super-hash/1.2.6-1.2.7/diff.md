# Comparing `tmp/super_hash-1.2.6.tar.gz` & `tmp/super_hash-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_hash-1.2.6.tar", last modified: Mon Nov 28 02:53:48 2022, max compression
+gzip compressed data, was "super_hash-1.2.7.tar", last modified: Thu May 25 20:21:01 2023, max compression
```

## Comparing `super_hash-1.2.6.tar` & `super_hash-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.065168 super_hash-1.2.6/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2022-11-28 02:53:48.065025 super_hash-1.2.6/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-11-28 02:53:48.065210 super_hash-1.2.6/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2022-11-20 16:13:35.000000 super_hash-1.2.6/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.063311 super_hash-1.2.6/super_hash/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.063902 super_hash-1.2.6/super_hash/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3435 2022-11-18 16:09:06.000000 super_hash-1.2.6/super_hash/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.063020 super_hash-1.2.6/super_hash/__dependencies__/simple_namespace/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.064238 super_hash-1.2.6/super_hash/__dependencies__/simple_namespace/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      821 2022-11-18 16:35:23.000000 super_hash-1.2.6/super_hash/__dependencies__/simple_namespace/main/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.064787 super_hash-1.2.6/super_hash/__dependencies__/simple_namespace/main/simple_namespace/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2022-11-18 16:35:23.000000 super_hash-1.2.6/super_hash/__dependencies__/simple_namespace/main/simple_namespace/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      656 2022-11-18 16:35:23.000000 super_hash-1.2.6/super_hash/__dependencies__/simple_namespace/main/simple_namespace/main.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    11162 2022-11-28 02:53:19.000000 super_hash-1.2.6/super_hash/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:53:48.063763 super_hash-1.2.6/super_hash.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2022-11-28 02:53:47.000000 super_hash-1.2.6/super_hash.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2022-11-28 02:53:47.000000 super_hash-1.2.6/super_hash.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-11-28 02:53:47.000000 super_hash-1.2.6/super_hash.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2022-11-28 02:53:47.000000 super_hash-1.2.6/super_hash.egg-info/top_level.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:21:01.584510 super_hash-1.2.7/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-25 20:21:01.584343 super_hash-1.2.7/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-25 20:21:01.584561 super_hash-1.2.7/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2022-11-20 16:13:35.000000 super_hash-1.2.7/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:21:01.583281 super_hash-1.2.7/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12054 2023-05-25 20:20:06.000000 super_hash-1.2.7/super_hash/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    74569 2023-05-25 19:39:10.000000 super_hash-1.2.7/super_hash/instuctions.ignore.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:21:01.584160 super_hash-1.2.7/super_hash.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/top_level.txt
```

### Comparing `super_hash-1.2.6/PKG-INFO` & `super_hash-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super_hash
-Version: 1.2.6
+Version: 1.2.7
 Summary: hash the unhashable, hash everything
 Home-page: https://github.com/jeff-hykin/super_hash.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `super_hash-1.2.6/setup.py` & `super_hash-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `super_hash-1.2.6/super_hash/__init__.py` & `super_hash-1.2.7/super_hash/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-from .__dependencies__ import simple_namespace
 import collections
 from hashlib import md5 
 import pickle
+import dis
 
-namespace = simple_namespace.namespace
+LOAD_GLOBAL_CODE = 116
 code = type(compile('1','','single'))
 
 def consistent_hash(value):
     if isinstance(value, bytes):
         return md5(value).hexdigest()
     
     if isinstance(value, str):
         return md5(("@"+value).encode('utf-8')).hexdigest()
     
     if isinstance(value, (bool, int, float, type(None))):
-        return md5(str(value).encode('utf-8')).hexdigest()
+        return md5(("#"+str(value)).encode('utf-8')).hexdigest()
         
     else:
         return md5(pickle.dumps(value, protocol=4)).hexdigest()
 
+def shallow_instruction_hash(value):
+    instructions = value if type(value) == tuple else dis.get_instructions(value)
+    to_hash = tuple(str((each.opcode, each.argval)) for each in instructions) + (getattr(value, "__name__", ""), )
+    hash_str = str(' '.join(to_hash).encode('utf-8'))
+    return consistent_hash(hash_str)
+
 import os
 file_doesnt_exist_key = "pGVQDVYZAVeUb9oOPvWn3QbHmnpw/MGu43pI8a+Gss+QKgnbo36NfRGmMtY0PXyBCg0MyG91Ey5aEQbZxzRp5sxQ"
 file_exists_key       = "xeWLFUZaurvdgqQA524lqQZ6BOSv+OBpQUmsSV4AmbRQG31JuMkhCZNz+XVN1HoU9wU3gezpusflZkd3kdKRwYBw"
+using_id_based        = "xeWLFUZaurvdgqQA524lqQZ6BOSv+OBpQUmsSV4AmbRQG31JuMkhCZNz+XVN1HoU9wU3gezpusflZkd3kdKRwYBw"
+hash_salt             = md5(("|"+str(-24979514859357)).encode('utf-8')).hexdigest()
 def hash_file(filepath=None, *, file=None, _block_read_size=1024):
     if filepath:
         if os.path.isdir(filepath):
             raise Exception(f'''filepath_hash("{filepath}") is not (yet) designed to work on folders''')
         # if file itself doesnt exist
         if not os.path.exists(filepath):
             return super_hash((file_doesnt_exist_key, filepath))
@@ -47,115 +55,111 @@
             hash_value = consistent_hash(bytes(hash_value, "utf-8")+block)
             block = file.read(_block_read_size)
         return hash_value
     
     # if filepath was only arg and was None
     return super_hash(None)
 
-@namespace
-def helpers():
-    
+class helpers:
     # yup this is how to detect iterables in python
+    @staticmethod
     def is_iterable(thing):
         # https://stackoverflow.com/questions/1952464/in-python-how-do-i-determine-if-an-object-is-iterable
         try:
             iter(thing)
         except TypeError:
             return False
         else:
             return True
-            
-    def shallow_instruction_hash(value):
-        import dis
-        instructions = dis.get_instructions(value)
-        to_hash = [str((each.opcode, each.argval)) for each in instructions]
-        hash_str = str(' '.join(to_hash).encode('utf-8')) + str(value.__name__ if hasattr(value, "__name__") else "")
-        return consistent_hash(hash_str)
     
+    shallow_instruction_hash = shallow_instruction_hash
+    
+    @staticmethod
     def source_hash(value):
         import inspect
         source = inspect.getsource(value)
         return consistent_hash(f"{hash_salt}{source}")
     
-    return locals()
-    
-@namespace
-def function_hashers():
-    def smart(value):
+class function_hashers:
+    @staticmethod
+    def smart(value, debug=False):
         # if defined in a proper module
         try:
-            return deep(value)
+            return function_hashers.deep(value)
         except Exception as error:
+            if debug: print("couldn't do deep", error)
             pass
         
         # if user defined
         try:
-            return shallow(value)
+            return function_hashers.shallow(value)
         except Exception as error:
+            if debug: print("couldn't do shallow", error)
             pass
         
         # if file defined, but actually a class
         try:
             return helpers.source_hash(value)
         except Exception as error:
+            if debug: print("couldn't do source_hash", error)
             pass
         
         # if has documentation (e.g. builtin)
         if type(value.__doc__) == str and len(value.__doc__) > 0 and type(value.__name__) == str:
+            if debug: print("couldn't do __doc__ hash")
             return consistent_hash(f'{hash_salt}{value.__doc__}{value.__name__}')
         
         # if all this fails, use the object id
         return id(value)
     
-    def shallow(value):
-        return helpers.shallow_instruction_hash(value)
+    shallow = shallow_instruction_hash
     
     # from https://github.com/andrewgazelka/smart-cache/blob/master/smart_cache/__init__.py
+    @staticmethod
     def instructions_to_hash(instructions):
-        to_hash = [str((each.opcode, super_hash(each.argval))) for each in instructions]
+        to_hash = tuple(str((each.opcode, super_hash(each.argval))) for each in instructions)
         hash_str = ' '.join(to_hash).encode('utf-8')
         return consistent_hash(hash_str)
     
+    @staticmethod
     def get_referenced_function_names(instructions):
-        return [ins.argval for ins in instructions if ins.opcode == 116]
+        return tuple(ins.argval for ins in instructions if ins.opcode == LOAD_GLOBAL_CODE)
     
+    @staticmethod
     def deep(input_func):
         import inspect
-        import dis
         module = inspect.getmodule(input_func)
         closed_set = set()
         instruction_hashes = [] if not hasattr(input_func, "__name__") else [ input_func.__name__ ]
         frontier = set()
         
-        base_instructions = list(dis.get_instructions(input_func))
-        child_names = get_referenced_function_names(base_instructions)
-        instruction_hashes.append(str(instructions_to_hash(base_instructions)))
+        base_instructions = tuple(dis.get_instructions(input_func))
+        child_names = function_hashers.get_referenced_function_names(base_instructions)
+        instruction_hashes.append(function_hashers.instructions_to_hash(base_instructions))
         for name in child_names:
             frontier.add(name)
         
         while len(frontier) > 0:
             function_name = frontier.pop()
             closed_set.add(function_name)
             function_reference = getattr(module, function_name, None)
             if function_reference is None:
                 continue
             try:
                 instructions = dis.get_instructions(function_reference)
             except TypeError as error:
                 continue
-            instruction_hashes.append(str(instructions_to_hash(instructions)))
+            instruction_hashes.append(function_hashers.instructions_to_hash(instructions))
             child_names = get_referenced_function_names(instructions)
             for child_name in child_names:
                 if child_name not in closed_set:
                     frontier.add(child_name)
         hash_str = ' '.join(instruction_hashes).encode('utf-8')
         return consistent_hash(hash_str)
     
-    return locals()
-
 try:
     mapping = collections.Mapping
 except Exception as error:
     try:
         import collections.abc
         mapping = collections.abc.Mapping
     except Exception as error:
@@ -204,37 +208,37 @@
     
     super_hash_method = getattr(value, "__super_hash__", None)
     if callable(super_hash_method):
         return consistent_hash(value.__super_hash__())
     
     if type(value) == code:
         try:
-            import dis
-            instructions = dis.get_instructions(value)
-            return consistent_hash(str([str((each.opcode, super_hash(each.argval))) for each in instructions]))
+            return shallow_instruction_hash(value)
         except Exception as error:
             return consistent_hash(code.co_code)
     # 
     # fallback 1: attempt consistent hash
     # 
     try:
         return consistent_hash(value)
     except Exception as error:
         # ignore the "TypeError: unhashable type:" errors and go to the next fallback method
         pass
     # 
     # generic fallback methods
     # 
-    hash_salt = -24979514859357
     value_id = id(value)
     if helpers.is_iterable(value):
         if value_id in already_seen:
             # seen but not yet computed
             if already_seen[value_id] is None:
-                return hash_salt
+                # FIXME: this is a problem when dealing with sets or lists, as two already-seen items in two different orders will result in the same parent hash
+                #        however this problem is equivlent (technially "bijective") to the problem of hashing an unlabelled graph
+                #        at the theory level, there is no proven method for hashing an unlabelled graph, although there are some not-proven-incorrect methods
+                return hash_salt # hash of something that is pending
             else:
                 return already_seen[value_id]
         else:
             already_seen[value_id] = None
         
         # dict is a special case, switch to using all its keys
         if isinstance(value, dict):
@@ -291,12 +295,14 @@
             super_hash._non_iterable_cache[value_id] = consistent_hash(f'{hash_salt}{value.__doc__}{value.__name__}')
             return super_hash._non_iterable_cache[value_id]
         
         # if all this fails, use the object id
         super_hash._non_iterable_cache[value_id] = value_id
         return super_hash._non_iterable_cache[value_id]
 
+from collections import OrderedDict
 super_hash._non_iterable_cache = {}
-super_hash.conversion_table = {
+super_hash.conversion_table = OrderedDict()
+super_hash.conversion_table[
     # have functions default to deep hashing
-    (lambda each: callable(each) and not isinstance(each, type)): function_hashers.smart
-}
+    (lambda each: callable(each) and not isinstance(each, type))
+] = function_hashers.smart
```

### Comparing `super_hash-1.2.6/super_hash.egg-info/PKG-INFO` & `super_hash-1.2.7/super_hash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-hash
-Version: 1.2.6
+Version: 1.2.7
 Summary: hash the unhashable, hash everything
 Home-page: https://github.com/jeff-hykin/super_hash.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

