# Comparing `tmp/pyimclsts-0.1.1.7.tar.gz` & `tmp/pyimclsts-0.1.2.tar.gz`

## Comparing `pyimclsts-0.1.1.7.tar` & `pyimclsts-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/CHANGELOG.md
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/example/followRef.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/example/lsf2csv.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/example/selectedlsf2csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/src/pyimclsts/__init__.py
--rw-r--r--   0        0        0    17672 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/src/pyimclsts/_base_templates.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/src/pyimclsts/core.py
--rw-r--r--   0        0        0    17667 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/src/pyimclsts/extract.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/src/pyimclsts/extractutils.py
--rw-r--r--   0        0        0    32188 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/src/pyimclsts/network.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/LICENSE
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/pyproject.toml
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/example/followRef.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/example/lsf2csv.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/example/selectedlsf2csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/__init__.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/_base.py
+-rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/core.py
+-rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/extract.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/extractutils.py
+-rw-r--r--   0        0        0    35089 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/network.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/PKG-INFO
```

### Comparing `pyimclsts-0.1.1.7/example/followRef.py` & `pyimclsts-0.1.2/example/followRef.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/example/lsf2csv.py` & `pyimclsts-0.1.2/example/lsf2csv.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/example/selectedlsf2csv.py` & `pyimclsts-0.1.2/example/selectedlsf2csv.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/src/pyimclsts/_base_templates.py` & `pyimclsts-0.1.2/src/pyimclsts/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,66 +23,44 @@
 '''
 
 # "Global" definitions
 header_data = namedtuple('header_data', ['sync', 'mgid', 'size', 'timestamp', 'src', 'src_ent', 'dst', 'dst_ent'])
 MessageAttributes = namedtuple('MessageAttributes', %MESSAGE_ATTRIBUTES%)
 
 # "Global" variables
-_imc_options = ''
 _sync_number = %SYNCH_NUMBER%
 _default_src = 0x4000 | (core.get_initial_IP() & 0xFFFF)
 
-class IMC_message():
-    
-    __slots__ = []
-    
-    '''Empty message to break circular reference.
-
-    Initially, there was 'base_message' and the descriptor 'mutable_attr', which contained a reference
-    to a dictionary 'imc_types' that pointed back to base message. This is/was necessary to allow type 
-    checking a message whose field may contain other messages, that is, the message class must have a
-    descriptor object (as per protocol) and to check if it is of type 'message', it must have a reference 
-    to the 'message' class. However, this leads to the cyclic reference:
-            
-            'base_message' -> descriptor -> dictionary -> 'base_message'.
-    
-    Although python may be able to handle circular references, we choose not to.
-
-    Therefore, to circumvent this issue, an empty message is added to break this cycle.
-            'IMC_message' <- base_message -> descriptor
-            'IMC_message' <- dictionary   <- descriptor
-    
-    Because a parent class does not point to its child classes, there is no cycle.
-    '''
-    pass
+# "Re-exporting" from core
+IMC_message = core.IMC_message
 
 imc_types = %IMC_TYPES%
 
 class base_message(IMC_message):
     
-    __slots__ = ['_header', '_footer', '_Attributes']
+    __slots__ = ['_header', '_footer', 'Attributes']
 
     def __str__(self) -> str:
-        output = ['Message \'' + self._Attributes.name + '\':', 'Fields:']
-        for field in self._Attributes.fields:
+        output = ['Message \'' + self.Attributes.name + '\':', 'Fields:']
+        for field in self.Attributes.fields:
             value = getattr(self, field)
             if value is not None:
                 if type(value) == str:
                     value = '\'' + value + '\''
                 
                 #Check whether it is an Enumerated type
                 elif getattr(getattr(type(self), field), '_field_def').get('unit', None) in ['Enumerated', 'Bitfield']:
                     # check whether the Enum was "validated" by the descriptor
                     if isinstance(value, IntEnum) or isinstance(value, IntFlag):
                         enum_def = getattr(getattr(type(self), field), '_field_def').get('enum-def', None) if getattr(getattr(type(self), field), '_field_def').get('enum-def', None) \
                             else getattr(getattr(type(self), field), '_field_def').get('bitfield-def', None)
                         
                         # check whether it is local or global
                         if not enum_def:
-                            value = self._Attributes.abbrev + '.' + str(value)
+                            value = self.Attributes.abbrev + '.' + str(value)
                         else:
                             value = str(value)
                     else:
                         value = str(value)
 
                 elif isinstance(value, IMC_message):
                     value = ('\n' + str(value)).replace('\n', '\n    ')
@@ -97,69 +75,69 @@
         output = '\n'.join(output)
         if hasattr(self, '_header'):
             output = repr(self._header) + '\n' + output
         return output
 
     def __repr__(self) -> str:
         arguments = []
-        for field in self._Attributes.fields:
+        for field in self.Attributes.fields:
             value = getattr(self, field)            
             if value is not None:
                 #Check whether it is an Enumerated type
                 if getattr(getattr(type(self), field), '_field_def').get('unit', None) in ['Enumerated', 'Bitfield']:
                     # check whether the Enum was "validated" by the descriptor
                     if isinstance(value, IntEnum) or isinstance(value, IntFlag):
                         enum_def = getattr(getattr(type(self), field), '_field_def').get('enum-def', None) \
                             if getattr(getattr(type(self), field), '_field_def').get('enum-def', None) \
                             else getattr(getattr(type(self), field), '_field_def').get('bitfield-def', None)
 
                         # check whether it is local or global
                         if enum_def:
                             value = str(value)
                         else:
-                            value = self._Attributes.abbrev + '.' + str(value)
+                            value = self.Attributes.abbrev + '.' + str(value)
                     else:
                         value = repr(value)
                 else:
                     value = repr(value)
             else:
                 value = 'None'
 
             arguments.append(field + " = " + value)
         arguments = ', '.join(arguments)
-        output = self._Attributes.abbrev + '({})'.format(arguments)
+        output = self.Attributes.abbrev + '({})'.format(arguments)
         return output
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, base_message):
             # if both of them have already defined a '_header'
             if hasattr(self, '_header') and hasattr(__o, '_header'):
                 if self._header != __o._header:
                     return False
             # if any of them does not have '_header' -> happens when a message is 
             # inside another, I'll skip and check the contents
             
             if hasattr(self, '_header') and hasattr(__o, '_header'):
                 if self._header != __o._header:
                     return False
-            fields = self._Attributes.fields
+            fields = self.Attributes.fields
             if any([getattr(self, field) != getattr(__o, field) for field in fields]):
                 return False
             return True
         return False
 
     def _pack_fields(self, *, serial_functions : dict) -> bytes:
         # Check if any field is empty (None) and not type 'message' (checked through the descriptor)
-        if any([getattr(self, '_' + field) is None for field in self._Attributes.fields if getattr(getattr(type(self), field), '_field_def').get('type', None) != 'message']):
+        if any([getattr(self, '_' + field) is None for field in self.Attributes.fields if getattr(getattr(type(self), field), '_field_def').get('type', None) != 'message']):
             raise ValueError('Cannot serialize a message that contains an empty (NoneType) field that is not a message.')
         
         serial_functions = serial_functions
 
         serialized_fields = []
-        for field in self._Attributes.fields:
+        for field in self.Attributes.fields:
             # Access variable information through the descriptor
             datatype = getattr(getattr(type(self), field), '_field_def').get('type', None)
             
             # check if it is a "NULL" message
             if datatype == 'message' and getattr(self, '_' + field) is None:
                 serialized_fields.append(serial_functions['uint16_t'](65535))
             else:
@@ -172,15 +150,15 @@
         
         The tricky part is: Are the header fields fixed or not, that is, they should be hardcoded or not?
         There may be mutability on their: 1. existence; 2, name; 3. order; 4. type (and size).
         
         We will assume that only 4. can change.
             - As a result a namedTuple is globally defined.'''
 
-        mgid = self._Attributes.id
+        mgid = self.Attributes.id
 
         # If None or a "default" value, overwrite
         if not hasattr(self, '_header'):
             _timestamp = time.time()
             _src = src if src is not None else _default_src
             _src_ent = src_ent if src_ent is not None else 0xFF
             _dst = dst if dst is not None else 0xFFFF
@@ -213,15 +191,15 @@
             
             # footer:
             '''Calculates CRC-16 IBM of a bit string'''
             self._footer = core.CRC16IMB(s_message)
             s_message = s_message + serial_functions['uint16_t'](self._footer)
 
             return s_message
-        return serial_functions['uint16_t'](self._Attributes.id) + s_fields
+        return serial_functions['uint16_t'](self.Attributes.id) + s_fields
 
     def get_timestamp(self) -> float:
         '''Get the timestamp. Returns None if the message has no header yet.'''
         if hasattr(self, '_header'):
             return self._header.timestamp
         return None
```

### Comparing `pyimclsts-0.1.1.7/src/pyimclsts/core.py` & `pyimclsts-0.1.2/src/pyimclsts/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -142,14 +142,38 @@
         if ip != '127.0.0.1':
             return int(_ipaddress.IPv4Address(ip))
     return int(_ipaddress.IPv4Address('127.0.0.1'))
 
 async def _async_wrapper(func, *args):
     return func(*args)
 
+class IMC_message():
+    '''IMC message parent/root class.'''
+    __slots__ = []
+    
+    '''Empty message to break circular reference.
+
+    Initially, there was 'base_message' and the descriptor 'mutable_attr', which contained a reference
+    to a dictionary 'imc_types' that pointed back to base message. This is/was necessary to allow type 
+    checking a message whose field may contain other messages, that is, the message class must have a
+    descriptor object (as per protocol) and to check if it is of type 'message', it must have a reference 
+    to the 'message' class. However, this leads to the cyclic reference:
+            
+            'base_message' -> descriptor -> dictionary -> 'base_message'.
+    
+    Although python may be able to handle circular references, we choose not to.
+
+    Therefore, to circumvent this issue, an empty message is added to break this cycle.
+            'IMC_message' <- base_message -> descriptor
+            'IMC_message' <- dictionary   <- descriptor
+    
+    Because a parent class does not point to its child classes, there is no cycle.
+    '''
+    pass
+
 class base_IO_interface:
     '''
         An 'abstract'* class that describes the basic implementation of an I/O interface.
 
         * Not really abstract as in Java, but consider it so. 
         I will not use abc and its decorators.
     '''
```

### Comparing `pyimclsts-0.1.1.7/src/pyimclsts/extract.py` & `pyimclsts-0.1.2/src/pyimclsts/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,57 +13,56 @@
 
 import urllib.request
 import ssl
 
 _target_folder = 'pyimc_generated'
 
 unknown_message = '''
-class Unknown(_base_templates.base_message):
+class Unknown(_base.base_message):
     \'\'\'A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.
 
     Contains a byte string field named 'contents' and a boolean value that indicates if its big or little endian.
     On serialization, it forces the original endianess, regardless of what the user chose to use.
     \'\'\'
 
     __slots__ = ['_Attributes', '_header', '_footer', '_contents', '_endianess']
-    Attributes = _base_templates.immutable_attr('Message attributes. A namedtuple containing all attributes and their default values')
-    contents = _base_templates.mutable_attr({'name': 'Contents', 'type': 'rawdata'}, "contents")
-    endianess = _base_templates.mutable_attr({'name': 'endianess', 'type': 'rawdata'}, "endianess")
+    Attributes = _base.MessageAttributes(fields = ('contents','endianess', ), name = "Unknown", id = id, abbrev = "Unknown", description = "A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.", ##ATTRIBUTES##)
+    contents = _base.mutable_attr({'name': 'Contents', 'type': 'rawdata'}, "contents")
+    endianess = _base.mutable_attr({'name': 'endianess', 'type': 'rawdata'}, "endianess")
 
     def __init__(self, id, contents = None, endianess = None):
         \'\'\'Class constructor
         
         A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.
 
         This message class contains the following fields and their respective types:
         contents : rawdata, unit: NOT FOUND
         \'\'\'
-        self._Attributes = _base_templates.MessageAttributes(fields = ('contents','endianess', ), name = "Unknown", id = id, abbrev = "Unknown", description = "A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.", ##ATTRIBUTES##)
         self._contents = contents
         self._endianess = endianess
     
     def _pack_fields(self, *, serial_functions : dict) -> bytes:
         raise NotImplemented
 
     def pack(self, *, is_field_message : bool = False, is_big_endian : bool = True, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> bytes:
         \'\'\'Serialize function that optionally overwrites the header, if parameters are provided.\'\'\'
         
-        serial_functions = core.pack_functions_big if self._endianess else core.pack_functions_little
+        serial_functions = _core.pack_functions_big if self._endianess else _core.pack_functions_little
         
         s_fields = self._contents
         
         if not is_field_message:
         
             s_header = self._pack_header(serial_functions=serial_functions, size=(len(s_fields)), src=src, src_ent=src_ent, dst=dst, dst_ent=dst_ent)
             s_message = s_header + s_fields
             
             # footer:
             \'\'\'Calculates CRC-16 IBM of a bit string\'\'\'
-            self._footer = core.CRC16IMB(s_message)
+            self._footer = _core.CRC16IMB(s_message)
             s_message = s_message + serial_functions['uint16_t'](self._footer)
 
             return s_message
         return serial_functions['uint16_t'](self._Attributes.id) + s_fields
 
         '''
 
@@ -158,22 +157,21 @@
     # make nested classes (Enums) immutable too?
     class_def = \
 '''
 class {name}({namespace}base_message):
     \'\'\'{description}\'\'\'
 {local_enum}
     __slots__ = {priv_attrib}
-    Attributes = {namespace}immutable_attr(\'Message attributes. A namedtuple containing all attributes and their default values\')
+    Attributes = {namespace}MessageAttributes({attributes})
 
 {mutable_attrib}
     def __init__(self, {constructor_args}):
         \'\'\'Class constructor
         
         {description}\'\'\'
-        self._Attributes = {namespace}MessageAttributes({attributes})
 {constructor_values}
 '''.format(namespace = namespace,
 name = name,
 description = description,
 local_enum = local_enumeration,
 priv_attrib = priv_attrib,
 attributes = attributes,
@@ -337,48 +335,53 @@
     with open(_target_folder + '/' + file_name, mode = 'w', encoding='utf-8') as f:
         f.write('\'\'\'\nIMC global bitfields definitions.\n\'\'\'\n\n')
         f.write('import enum as _enum\n\n#Enumerations:\n')
         for k, v in metadata_encyclopedia['bitfields'].items():
             f.write(enum_extractor(v, k, True))
     
     lib_location = pathlib.Path(__file__).parent.resolve()
-    file_name = '_base_templates.py'
+    file_name = '_base.py'
     with open(str(lib_location) + '/' + file_name, mode = 'r', encoding='utf-8') as f_in:
         base_templates = f_in.read()
         base_templates = base_templates.replace('%SYNCH_NUMBER%', hex(metadata_encyclopedia['header']['fields']['sync']['value']))
         base_templates = base_templates.replace('%IMC_TYPES%', str(imc_types).replace('<class \'', '').replace("'>",'').replace('"',''))
         base_templates = base_templates.replace('%MESSAGE_ATTRIBUTES%', str([s.replace('-','') for s in message_attributes]))
 
         with open(_target_folder + '/' + file_name, mode = 'w', encoding='utf-8') as f_out:           
             f_out.write(base_templates)
 
     file_name = 'messages.py'
     with open(_target_folder + '/' + file_name, mode = 'w', encoding='utf-8') as f:
         f.write('\'\'\'\nIMC messages.\n\'\'\'\n\n')
         # write import statements
-        f.write('from . import _base_templates\nimport enum as _enum\nimport pyimclsts.core as core\nfrom . import categories\n')
+        f.write('from . import _base\nimport enum as _enum\nimport pyimclsts.core as _core\nfrom . import categories as _categories\n')
         f.write('\n_message_ids = {}\n'.format(str(dict((k, v['abbrev']) for k, v in message_encyclopedia.items()))))
+        f.write('\n# Re-export:\nIMC_message = _core.IMC_message\n')
         f.write(unknown_message.replace('##ATTRIBUTES##', ', '.join([i + '= None' for i in message_attributes if i not in {'fields', 'name', 'id', 'abbrev', 'description'}])))
 
         messages_w_cat = []
         for cat, l in metadata_encyclopedia['categories'].items():
             l_filtered = [x for x in l if x in message_encyclopedia.keys()]
             if l_filtered:
                 with open(_target_folder + '/categories/' + cat.replace(' ', '') + '.py', mode = 'w', encoding='utf-8') as f_cat:
                     f_cat.write(f'\'\'\'\nIMC {cat} messages.\n\'\'\'\n\n')
                     # write import statements
-                    f_cat.write('from .. import _base_templates\nimport enum as _enum\nimport pyimclsts.core as core\n')
+                    f_cat.write('from .. import _base\nimport enum as _enum\n')
                     
                     for id in l_filtered:
-                        f_cat.write(hardcode_message_extractor(message_encyclopedia[id], '_base_templates', message_attributes))    
+                        f_cat.write(hardcode_message_extractor(message_encyclopedia[id], '_base', message_attributes))    
                 messages_w_cat = messages_w_cat + l_filtered
         
         for k, v in message_encyclopedia.items():
             if k in messages_w_cat:
-                f.write('\n\n' + v['abbrev'] + ' = categories.' + v['category'].replace(' ', '') + '.' + v['abbrev'])
+                f.write('\n\n' + v['abbrev'] + ' = _categories.' + v['category'].replace(' ', '') + '.' + v['abbrev'])
             else:
-                f.write(hardcode_message_extractor(v, '_base_templates', message_attributes))
+                f.write(hardcode_message_extractor(v, '_base', message_attributes))
     
     create_init(_target_folder + '/categories')
     create_init(_target_folder)
 
+    # small ugly fix
+    with open(_target_folder + '/__init__.py', mode = 'a', encoding='utf-8') as f:
+        f.write('from . import categories')
+
     print('Finished extracting messages.')
```

### Comparing `pyimclsts-0.1.1.7/src/pyimclsts/extractutils.py` & `pyimclsts-0.1.2/src/pyimclsts/extractutils.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/src/pyimclsts/network.py` & `pyimclsts-0.1.2/src/pyimclsts/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     Contains classes that define the role this pyimc instance will perform and
     are intended to be used directly by the user or their abstraction layer
 
 '''
 import typing as _typing
 import functools as _functools
 import inspect as _inspect
+import types as _types
 
 import multiprocessing as _multiprocessing
 import asyncio as _asyncio
 import time as _time
 
 import importlib.util as _import
 import sys as _sys
@@ -22,30 +23,30 @@
 
 _spec = _import.spec_from_file_location(_module_name, _location)
 
 _pg = _import.module_from_spec(_spec)
 _sys.modules[_module_name] = _pg
 _spec.loader.exec_module(_pg)
 
-def unpack(message : bytes, *, is_big_endian : bool = None, is_field_message : bool = False, fast_mode : bool = False) -> _pg._base_templates.IMC_message:
+def unpack(message : bytes, *, is_big_endian : bool = None, is_field_message : bool = False, fast_mode : bool = False) -> _core.IMC_message:
     '''Expects a serializable (= exactly long (header + fields + CRC)) string of bits whose CRC has already been checked
     
     Fast mode skips all type checking performed by the descriptor by directly invoking the constructor.
     '''
     if is_big_endian is None:
-        is_big_endian = int.from_bytes(message[:2], byteorder='big') == _pg._base_templates._sync_number
+        is_big_endian = int.from_bytes(message[:2], byteorder='big') == _pg._base._sync_number
         # Note: is_big_endian is a function parameter to enable recursion
     
     unpack_functions = _core.unpack_functions_big if is_big_endian else _core.unpack_functions_little
     cursor = 0
     
     if not is_field_message:
         # deserialize header
         (m, size) = unpack_functions['header'](message[cursor:])
-        deserialized_header = _pg._base_templates.header_data(*m)
+        deserialized_header = _pg._base.header_data(*m)
         cursor += size
     
         msgid = deserialized_header.mgid
         if msgid not in _pg.messages._message_ids:
             unknown_msg = _pg.messages.Unknown(msgid, contents = message[cursor:-2], endianess = is_big_endian)
             unknown_msg._header = deserialized_header
             return unknown_msg
@@ -55,15 +56,15 @@
         if msgid not in _pg.messages._message_ids:
             raise KeyError(f'Cannot parse/unpack an unknown inlined message (no information about the size). Add message id {msgid} to extract list')
     
     if fast_mode:
         # get corresponding class
         message_class = getattr(_pg.messages, _pg.messages._message_ids.get(msgid, None))
 
-        fields = [(f, getattr(getattr(type(message_class()), f), '_field_def')['type']) for f in message_class()._Attributes.fields]
+        fields = [(f, getattr(getattr(type(message_class()), f), '_field_def')['type']) for f in message_class().Attributes.fields]
         arguments = dict()
         for field, t in fields:
             if t == 'message':
                 if unpack_functions['uint16_t'](message[cursor:cursor+2])[0] == 65535:
                     cursor += 2
                 else:
                     (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
@@ -86,15 +87,15 @@
         
     else:
         # instantiate empty class
         message_class = getattr(_pg.messages, _pg.messages._message_ids.get(msgid, None))()
 
         # deserialize fields
         # make a (field, type) tuple list, get information in the descriptor
-        fields = [(f, getattr(getattr(type(message_class), f), '_field_def')['type']) for f in message_class._Attributes.fields]
+        fields = [(f, getattr(getattr(type(message_class), f), '_field_def')['type']) for f in message_class.Attributes.fields]
         for field, t in fields:
             if t == 'message':
                 if unpack_functions['uint16_t'](message[cursor:cursor+2])[0] == 65535:
                     cursor += 2
                 else:
                     (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
                     cursor += size
@@ -117,15 +118,15 @@
         message_class._header = deserialized_header
         return message_class
     else:
         return (message_class, cursor)
 
 def _get_id_src_src_ent(message : bytes) -> int:
     src_ent = message[16]
-    if int.from_bytes(message[:2], byteorder='big') == _pg._base_templates._sync_number:
+    if int.from_bytes(message[:2], byteorder='big') == _pg._base._sync_number:
         id = int.from_bytes(message[2:4], byteorder='big')
         src = int.from_bytes(message[14:16], byteorder='big')
         
         return (id, src, src_ent)
     else:
         id = int.from_bytes(message[2:4], byteorder='little')
         src = int.from_bytes(message[14:16], byteorder='little')
@@ -157,21 +158,21 @@
     def block_outgoing(self):
         '''Blocks (and discards) outgoing messages'''
         self._block_outgoing = True
     def unblock_outgoing(self):
         '''Unblock outgoing messages'''
         self._block_outgoing = False
 
-    def send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+    def send(self, message : _pg._base.base_message, *, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> None:
         '''Wrapper around a queue (actually a pipe end).'''
         if not self._block_outgoing:
             self._send(message, src = src, src_ent = src_ent, dst = dst, dst_ent = dst_ent)
             
-    def _send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+    def _send(self, message : _pg._base.base_message, *, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> None:
         raise NotImplemented
 
 class message_bus(_message_bus):
     '''
         Send and receives messages as bytes, but exposes them as IMC messages
 
@@ -209,15 +210,15 @@
             buffer = bytearray()
             while keep_running.value:
                 try:
                     # magic number: 6 = sync number + (msgid + msgsize) size in bytes
                     if len(buffer) < 6:
                         buffer += await io_interface.read(6 - len(buffer))
 
-                    if int.from_bytes(buffer[:2], byteorder='little') == _pg._base_templates._sync_number:
+                    if int.from_bytes(buffer[:2], byteorder='little') == _pg._base._sync_number:
                         # get msg size
                         size = int.from_bytes(buffer[4:6], byteorder='little')
                         # magic number: 22 = 20(header size) + 2(CRC) sizes in bytes.
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         # Validate message, but do not unpack yet
@@ -227,15 +228,15 @@
                             # eliminate message from buffer
                             del buffer[:size + 22]
                         else:
                             # deserialization failed:
                             # sync number is not followed by a sound/valid message. Remove it from buffer
                             # to look for next message
                             del buffer[:2]
-                    elif int.from_bytes(buffer[:2], byteorder='big') == _pg._base_templates._sync_number:
+                    elif int.from_bytes(buffer[:2], byteorder='big') == _pg._base._sync_number:
                         size = int.from_bytes(buffer[4:6], byteorder='big')
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         unparsed_msg = bytes(buffer[:(size + 22)])
                         if _core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='big'):
                             child_end.send_bytes(unparsed_msg)
@@ -304,20 +305,20 @@
     def close(self, max_wait : float = 1) -> None:        
         with self._keep_running.get_lock():
             self._keep_running.value = False
         
         self._child_process.join()
         self._child_process.close()
 
-    def _send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+    def _send(self, message : _pg._base.base_message, *, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> None:
         self._parent_end.send_bytes(message.pack(is_big_endian=self._big_endian, src = src, src_ent = src_ent, 
                         dst = dst, dst_ent = dst_ent))
 
-    def recv(self) -> _pg._base_templates.base_message:
+    def recv(self) -> _pg._base.base_message:
         '''Wrapper around a queue (actually a pipe end). Blocks until a message is available.
         The _external_listener_loop is supposed to send complete messages (as per multiprocessing 
         documentation).'''       
         msg = self._parent_end.recv_bytes()
         
         if msg == b'':
             raise EOFError('Message Bus has been closed.')
@@ -382,15 +383,15 @@
             buffer = bytearray()
             while self._keep_running:
                 try:
                     # magic number: 6 = sync number + (msgid + msgsize) size in bytes
                     if len(buffer) < 6:
                         buffer += await io_interface.read(6 - len(buffer))
 
-                    if int.from_bytes(buffer[:2], byteorder='little') == _pg._base_templates._sync_number:
+                    if int.from_bytes(buffer[:2], byteorder='little') == _pg._base._sync_number:
                         # get msg size
                         size = int.from_bytes(buffer[4:6], byteorder='little')
                         # magic number: 22 = 20(header size) + 2(CRC) sizes in bytes.
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         # Validate message, but do not unpack yet
@@ -400,15 +401,15 @@
                             # eliminate message from buffer
                             del buffer[:size + 22]
                         else:
                             # deserialization failed:
                             # sync number is not followed by a sound/valid message. Remove it from buffer
                             # to look for next message
                             del buffer[:2]
-                    elif int.from_bytes(buffer[:2], byteorder='big') == _pg._base_templates._sync_number:
+                    elif int.from_bytes(buffer[:2], byteorder='big') == _pg._base._sync_number:
                         size = int.from_bytes(buffer[4:6], byteorder='big')
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         unparsed_msg = bytes(buffer[:(size + 22)])
                         if _core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='big'):
                             await self._reader_queue.put(unparsed_msg)
@@ -446,20 +447,20 @@
         self._task = _asyncio.create_task(main_loop())
     
     def close(self, max_wait : float = 1) -> None:
         self._keep_running = False
         self._task.cancel()
         print('Message Bus has been closed.')
 
-    def _send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+    def _send(self, message : _pg._base.base_message, *, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> None:
         self._writer_queue.put_nowait(message.pack(is_big_endian=self._big_endian, src = src, src_ent = src_ent, 
                         dst = dst, dst_ent = dst_ent))
 
-    async def recv(self) -> _pg._base_templates.base_message:
+    async def recv(self) -> _pg._base.base_message:
         '''Wrapper around a queue (actually a pipe end). Blocks until a message is available.
         The _external_listener_loop is supposed to send complete messages (as per multiprocessing 
         documentation).'''
 
         msg = await self._reader_queue.get()
         
         if msg == b'':
@@ -478,15 +479,15 @@
             print('Message bus event loop has been closed due to end of file.')
             return True
         print('Message bus event loop has been closed.')
         return None
 
 class subscriber:
 
-    __slots__ = ['_msg_manager', '_subscriptions', '_subscripted_all', '_periodic', '_call_once', '_use_mp', '_peers', '_src2name']
+    __slots__ = ['_msg_manager', '_subscriptions', '_subscripted_all', '_periodic', '_call_once', '_use_mp', '_peers', '_src2name', '_keep_running']
 
     def __init__(self, IO_interface : _core.base_IO_interface, *,big_endian=False, use_mp = False) -> None:
         self._use_mp = use_mp
         if self._use_mp:
             self._msg_manager = message_bus(IO_interface, big_endian)
         else:
             self._msg_manager = message_bus_st(IO_interface, big_endian)
@@ -500,26 +501,27 @@
         # a dictionary of {2: 'vehicle name'}
         self._src2name = dict()
         
         self.subscribe_async(self._abort, _pg.messages.Abort)
         
         self.call_once(self._queryEntityList, delay=1)
         self.periodic_async(self._queryEntityList, period=300)
+        self.subscribe_async(self._update_peers, _pg.messages.EntityInfo)
         self.subscribe_async(self._update_peers, _pg.messages.EntityList)
         self.subscribe_async(self._update_peers, _pg.messages.Announce)
 
-    async def _periodic_wrapper_coro(self, _period : float, f : _typing.Callable, send_callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+    async def _periodic_wrapper_coro(self, _period : float, f : _typing.Callable, send_callback : _typing.Callable[[_core.IMC_message], None]):
         loop = _asyncio.get_running_loop()
         while True:
             last_exec = loop.time()
             await f(send_callback)
             now = loop.time()
             await _asyncio.sleep(max(last_exec - now + _period, 0))
                 
-    async def _periodic_wrapper(self, _period : float, f : _typing.Callable, send_callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+    async def _periodic_wrapper(self, _period : float, f : _typing.Callable, send_callback : _typing.Callable[[_core.IMC_message], None]):
         loop = _asyncio.get_running_loop()
         f(send_callback)
         while True:
             await _asyncio.sleep(_period)
             loop.call_later(_period, f, send_callback)
 
     async def _event_loop(self):
@@ -543,15 +545,15 @@
                 if _inspect.iscoroutinefunction(f):
                     tasks.append(loop.create_task(self._periodic_wrapper_coro(period, f, msg_mgr.send)))
                 elif callable(f):
                     tasks.append(loop.create_task(self._periodic_wrapper(period, f, msg_mgr.send)))
                 else:
                     print(f'Warning: Given function {f} is neither _typing.Callable nor a coroutine.')
 
-            while True:
+            while self._keep_running:
                 msg = msg_mgr.recv() if self._use_mp else await msg_mgr.recv()
                 mgid, src, src_ent = _get_id_src_src_ent(msg)
                 if mgid in self._subscriptions:
                     desel_message = unpack(msg, fast_mode=True)
                     for f in self._subscriptions[mgid]:
                         if self._validate_call(src, src_ent, f[1], f[2]):
                             await f[0](desel_message, msg_mgr.send)
@@ -567,15 +569,15 @@
     async def _abort(self, msg, send_callback):
         if msg._header is not None:
             my_src = 0x4000 | (_core.get_initial_IP() & 0xFFFF)
             if msg._header.dst == my_src:
                 loop = _asyncio.get_running_loop()
                 loop.close()
 
-    def _update_peers(self, msg : _typing.Union[_pg.messages.EntityList, _pg.messages.Announce], send_callback):
+    def _update_peers(self, msg : _typing.Union[_pg.messages.EntityList, _pg.messages.Announce, _pg.messages.EntityInfo], send_callback):
         if msg._header is not None:
             src = msg._header.src
             
             if isinstance(msg, _pg.messages.EntityList):
                 if msg.op == msg.OP.REPORT:
                     entList =  [i.split(sep='=') for i in msg.list.split(sep=';')]
                     entList = {k : int(v) for [k, v] in entList}
@@ -583,14 +585,23 @@
                     name = self._src2name.get(src, None)
                     if name is not None:
                         # if it exists, update; else, create entry
                         if self._peers.get(name, None) is not None:
                             self._peers[name]['EntityList'] = entList
                         else:
                             self._peers[name] = {'EntityList' : entList}
+            
+            elif isinstance(msg, _pg.messages.EntityList):
+                name = self._src2name.get(src, None)
+                if name is not None:
+                    # if it exists, update; else, create entry
+                    if self._peers.get(name, None) is not None:
+                        self._peers[name]['EntityList'][msg.label] = msg.id
+                    else:
+                        self._peers[name] = {'EntityList' : {msg.label : msg.id}}
 
             elif isinstance(msg, _pg.messages.Announce):
                 name = msg.sys_name
 
                 self._src2name[src] = name
                 # if it exists, update; else, create entry
                 if self._peers.get(name, None) is not None:
@@ -623,46 +634,56 @@
             if (correct_src or correct_src_ent) and (desired_src is None or desired_src_ent is None):
                 return True
             elif correct_src and correct_src_ent:
                 return True
             
         return False
     
-    def subscribe_async(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None], msg_id : _typing.Union[int, _pg._base_templates.IMC_message] = None, *, src : str = None, src_ent : str = None):
-        '''Appends the callback to the list of subscripted functions.
-        msg_id can be provided as an int or the class of the message.
-        src and src_ent can be provided as strings. If None, then defaults to all.
+    def subscribe_async(self, callback : _typing.Callable[[_core.IMC_message, _typing.Callable[[_core.IMC_message], None]], None], msg_id : _typing.Union[int, _core.IMC_message, str, _types.ModuleType] = None, *, src : str = None, src_ent : str = None):
+        '''Appends the callback to the list of subscriptions to a message.
+        msg_id can be provided as an int, the class of the message, its instance or a category (string (camel case) or module).
+        src and src_ent should be provided as strings.
         
+        When a parameters is None, then it is interpreted as 'all'.
+
         The main loop calls the function and pass the message and a callback to send messages.
         The return value is discarded and the function must have exactly two parameters (the message and the callback)
         and must not have additional parameters, to avoid unintended behavior*.
         
         *Due to python's pass-by-assignment, the argument values are evaluated when a function is called.
         This means that even if we pass, say "x", to the .subscribe_async method and then try to
         pass "x" to the callback, we can only pass x's value at the moment .subscribe_async was called.
         This means that if we subscribe, for example, f(x) and somewhere a function g "updates" x, and then call
         f(x) again, f will be called with x's first value.
         This could be bypassed using mutable data structures, but let's not delve into that.
 
-        Tip: If the original function really needs arguments, wrap it with _functools.partial.
+        Tip: If the original function really needs arguments, wrap it with functools.partial.
         Tip2: Use a class instance to keep shared values across different calls. See followRef.py.
         '''
         key = None
-        if isinstance(msg_id, _pg._base_templates.IMC_message):
-            key = msg_id._Attributes.id
+        if isinstance(msg_id, _core.IMC_message):
+            key = msg_id.Attributes.id
         elif isinstance(msg_id, int):
             key = msg_id
         elif _inspect.isclass(msg_id):
-            if issubclass(msg_id, _pg._base_templates.IMC_message):
-                key = msg_id()._Attributes.id
+            if issubclass(msg_id, _core.IMC_message):
+                key = msg_id().Attributes.id
+        elif isinstance(msg_id, str):
+            module = getattr(_pg.categories, msg_id)
+            self.subscribe_async(callback, module, src=src, src_ent=src_ent)
+        elif isinstance(msg_id, _types.ModuleType):
+            msgs = [j for j in [getattr(msg_id, i) for i in dir(msg_id) if _inspect.isclass(getattr(msg_id, i))] if issubclass(j, _core.IMC_message)]
+            for m in msgs:
+                self.subscribe_async(callback, m, src=src, src_ent=src_ent)
         elif msg_id is None:
             pass
         else:
             print(f'Warning: Given message id {msg_id} is not a known message.')
-            
+        
+        
         # There is either an explicit subscription (the key is not None) or 'all'
         # (msg_id is None). There cannot be both nor neither.
         if (key is not None) ^ (msg_id is None):
             c = None
             if _inspect.iscoroutinefunction(callback):
                 c = callback
             elif callable(callback):
@@ -675,26 +696,78 @@
                     self._subscripted_all.append((c, src, src_ent))
                 else:
                     if self._subscriptions.get(key, None) is not None:
                         self._subscriptions[key].append((c, src, src_ent))
                     else:
                         self._subscriptions[key] = [(c, src, src_ent)]
 
-    def periodic_async(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None], period = float):
+    def periodic_async(self, callback : _typing.Callable[[_core.IMC_message], None], period = float):
         '''Add callback to a list to be called every period seconds. Function must take
         a send callback as parameter. This callback can be used to send messages.'''
         self._periodic.append((callback, period))
 
-    def subscribe_mp(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None], msg_id : _typing.Union[int, _pg._base_templates.IMC_message], *, src : str = None, scr_ent : str = None):
+    def subscribe_mp(self, callback : _typing.Callable[[_core.IMC_message, _typing.Callable[[_core.IMC_message], None]], None], msg_id : _typing.Union[int, _core.IMC_message, str, _types.ModuleType] = None, *, src : str = None, src_ent : str = None):
         '''Calls a function and pass the message and a callback to send messages to it.
         Runs the given callback in a different process and should be used only with heavy load
         functions.
         '''
         raise NotImplemented
 
-    def call_once(self, callback : _typing.Callable[[_typing.Callable[[_pg._base_templates.IMC_message], None]], None], delay : float = None):
+    def call_once(self, callback : _typing.Callable[[_typing.Callable[[_core.IMC_message], None]], None], delay : float = None):
         '''Calls the given callbacks as soon as the main loop starts or according to their delay in seconds.
         Callback parameters must be exactly one callback (that can be used to send messages).'''
         self._call_once.append((callback, delay))
 
+    def print_information(self):
+        '''Looks for (and asks for, when applicable) the first Announce and EntityList messages and print them.
+        
+        Executes no other subscription.
+        '''
+        
+        _subscriptions_temp = self._subscriptions
+        _subscripted_all_temp = self._subscripted_all
+        _periodic_temp = self._periodic
+        _call_once_temp = self._call_once
+
+        self._subscriptions = dict()
+        self._subscripted_all = []
+        self._periodic = []
+        self._call_once = []
+
+        self.call_once(self._queryEntityList, delay=1)
+        self.periodic_async(self._queryEntityList, period=10)
+        
+        msgs = dict()
+        def printmsg(msg, cb):
+            if isinstance(msg, _pg.messages.Announce):
+                msgs['Announce'] = msg
+            if isinstance(msg, _pg.messages.EntityList) and msg.op == _pg.messages.EntityList.OP.REPORT:
+                msgs['EntityList'] = msg
+            if len(msgs) >= 2:
+                self.stop()
+        
+        self.subscribe_async(printmsg, _pg.messages.Announce)
+        self.subscribe_async(printmsg, _pg.messages.EntityList)
+
+        self.run()
+
+        for i in msgs.values():
+            print(i)
+            print('\n')
+        
+        self._subscriptions = _subscriptions_temp
+        self._subscripted_all = _subscripted_all_temp
+        self._periodic = _periodic_temp
+        self._call_once = _call_once_temp
+
+    def stop(self):
+        '''Signals the subscriber to immediately stop.'''
+        self._keep_running = False
+    
     def run(self):
+        '''Starts the event loop of the subscriber. 
+        
+        That is: Open the IO_interface, wraps and runs the callbacks that have been subscribed to messages.
+        Since it uses asyncio, it blocks the whole interpreter.
+        '''
+        self._keep_running = True
         _asyncio.run(self._event_loop())
```

### Comparing `pyimclsts-0.1.1.7/.gitignore` & `pyimclsts-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/LICENSE` & `pyimclsts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/README.md` & `pyimclsts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.7/pyproject.toml` & `pyimclsts-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyimclsts"
-version = "0.1.1.7"
+version = "0.1.2"
 authors = [
   { name = "Choi Wang Dzak" },
 ]
 description = "Python bindings of the IMC message schema"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["IMC", "IMC message protocol", "LSTS"]
```

### Comparing `pyimclsts-0.1.1.7/PKG-INFO` & `pyimclsts-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimclsts
-Version: 0.1.1.7
+Version: 0.1.2
 Summary: Python bindings of the IMC message schema
 Project-URL: Homepage, https://github.com/choiwd/pyimctrans
 Project-URL: Bug Tracker, https://github.com/choiwd/pyimctrans/issues
 Author: Choi Wang Dzak
 License: Copyright (c) 2023 Laboratório de Sistemas e Tecnologia Subaquática
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

