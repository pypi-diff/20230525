# Comparing `tmp/py_elf_structs-1.4.1.tar.gz` & `tmp/py_elf_structs-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py_elf_structs-1.4.1.tar", last modified: Sun Feb 26 21:04:30 2023, max compression
+gzip compressed data, was "dist/py_elf_structs-1.4.2.tar", last modified: Thu May 25 09:57:07 2023, max compression
```

## Comparing `py_elf_structs-1.4.1.tar` & `py_elf_structs-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonatan    (501) staff       (20)        0 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/
--rw-r--r--   0 jonatan    (501) staff       (20)     4101 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/PKG-INFO
-drwxr-xr-x   0 jonatan    (501) staff       (20)        0 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs.egg-info/
--rw-r--r--   0 jonatan    (501) staff       (20)     4101 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs.egg-info/PKG-INFO
--rw-r--r--   0 jonatan    (501) staff       (20)      447 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs.egg-info/SOURCES.txt
--rw-r--r--   0 jonatan    (501) staff       (20)       24 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs.egg-info/requires.txt
--rw-r--r--   0 jonatan    (501) staff       (20)       15 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs.egg-info/top_level.txt
--rw-r--r--   0 jonatan    (501) staff       (20)        1 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs.egg-info/dependency_links.txt
-drwxr-xr-x   0 jonatan    (501) staff       (20)        0 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs/
--rw-r--r--   0 jonatan    (501) staff       (20)      116 2022-04-22 15:54:32.000000 py_elf_structs-1.4.1/py_elf_structs/__init__.py
-drwxr-xr-x   0 jonatan    (501) staff       (20)        0 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/py_elf_structs/lib/
--rw-r--r--   0 jonatan    (501) staff       (20)      477 2022-04-22 15:53:50.000000 py_elf_structs-1.4.1/py_elf_structs/lib/generate_structs.py
--rw-r--r--   0 jonatan    (501) staff       (20)        0 2022-04-21 22:14:45.000000 py_elf_structs-1.4.1/py_elf_structs/lib/__init__.py
--rw-r--r--   0 jonatan    (501) staff       (20)     4381 2023-02-26 21:01:03.000000 py_elf_structs-1.4.1/py_elf_structs/lib/parser.py
--rw-r--r--   0 jonatan    (501) staff       (20)    10938 2023-02-26 21:02:44.000000 py_elf_structs-1.4.1/py_elf_structs/lib/structs.py
--rw-r--r--   0 jonatan    (501) staff       (20)      355 2022-04-22 16:06:49.000000 py_elf_structs-1.4.1/py_elf_structs/lib/utils.py
--rw-r--r--   0 jonatan    (501) staff       (20)      405 2023-02-24 19:10:10.000000 py_elf_structs-1.4.1/py_elf_structs/lib/loader.py
--rw-r--r--   0 jonatan    (501) staff       (20)      683 2022-04-23 14:27:58.000000 py_elf_structs-1.4.1/py_elf_structs/__main__.py
--rw-r--r--   0 jonatan    (501) staff       (20)     2486 2022-04-23 14:59:52.000000 py_elf_structs-1.4.1/README.md
--rw-r--r--   0 jonatan    (501) staff       (20)      740 2023-02-26 21:03:39.000000 py_elf_structs-1.4.1/setup.py
--rw-r--r--   0 jonatan    (501) staff       (20)       38 2023-02-26 21:04:30.000000 py_elf_structs-1.4.1/setup.cfg
+drwxr-xr-x   0 admin     (1000) root         (0)        0 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/
+-rw-r--r--   0 admin     (1000) root         (0)      335 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/PKG-INFO
+drwxr-xr-x   0 admin     (1000) root         (0)        0 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs.egg-info/
+-rw-r--r--   0 admin     (1000) root         (0)      335 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs.egg-info/PKG-INFO
+-rw-r--r--   0 admin     (1000) root         (0)      447 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs.egg-info/SOURCES.txt
+-rw-r--r--   0 admin     (1000) root         (0)       24 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs.egg-info/requires.txt
+-rw-r--r--   0 admin     (1000) root         (0)       15 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs.egg-info/top_level.txt
+-rw-r--r--   0 admin     (1000) root         (0)        1 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs.egg-info/dependency_links.txt
+drwxr-xr-x   0 admin     (1000) root         (0)        0 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs/
+-rw-r--r--   0 admin     (1000) root         (0)      116 2022-04-22 15:54:32.000000 py_elf_structs-1.4.2/py_elf_structs/__init__.py
+drwxr-xr-x   0 admin     (1000) root         (0)        0 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/py_elf_structs/lib/
+-rw-r--r--   0 admin     (1000) root         (0)      477 2022-04-22 15:53:50.000000 py_elf_structs-1.4.2/py_elf_structs/lib/generate_structs.py
+-rw-r--r--   0 admin     (1000) root         (0)        0 2022-04-21 22:14:45.000000 py_elf_structs-1.4.2/py_elf_structs/lib/__init__.py
+-rw-r--r--   0 admin     (1000) root         (0)     4484 2023-05-25 09:52:04.000000 py_elf_structs-1.4.2/py_elf_structs/lib/parser.py
+-rw-r--r--   0 admin     (1000) root         (0)    10887 2023-05-25 09:54:30.000000 py_elf_structs-1.4.2/py_elf_structs/lib/structs.py
+-rw-r--r--   0 admin     (1000) root         (0)      355 2022-04-22 16:06:49.000000 py_elf_structs-1.4.2/py_elf_structs/lib/utils.py
+-rw-r--r--   0 admin     (1000) root         (0)      405 2023-02-24 19:10:10.000000 py_elf_structs-1.4.2/py_elf_structs/lib/loader.py
+-rw-r--r--   0 admin     (1000) root         (0)      683 2022-04-23 14:27:58.000000 py_elf_structs-1.4.2/py_elf_structs/__main__.py
+-rw-r--r--   0 admin     (1000) root         (0)     2486 2022-04-23 14:59:52.000000 py_elf_structs-1.4.2/README.md
+-rw-r--r--   0 admin     (1000) root         (0)      740 2023-05-25 09:54:35.000000 py_elf_structs-1.4.2/setup.py
+-rw-r--r--   0 admin     (1000) root         (0)       38 2023-05-25 09:57:07.000000 py_elf_structs-1.4.2/setup.cfg
```

### Comparing `py_elf_structs-1.4.1/py_elf_structs/lib/parser.py` & `py_elf_structs-1.4.2/py_elf_structs/lib/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
                 if child.tag == "DW_TAG_structure_type":
                     logging.info("Parsing struct: {}".format(child.get_full_path()))
                     try:
                         struct_obj = build_struct_from_pyelf_child(dwarf,
                                                                    child,
                                                                    endian)
                         if isinstance(struct_obj, LazyResolveStruct):
+                            logging.info("Going to lazy resolving: {}".format(struct_obj.struct_name))
                             lazy_resolve.append(struct_obj)
                         structs.append(struct_obj)
                     except (TypeInformationNotFound, StructBuildException, Exception) as e:
                         logging.info("Parsing exception: {}, exception type: {}".format(e, type(e)))
 
     # Actually this function should be recursive !
     # Because one struct can define many structs !
```

### Comparing `py_elf_structs-1.4.1/py_elf_structs/lib/structs.py` & `py_elf_structs-1.4.2/py_elf_structs/lib/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,35 +74,32 @@
     struct c{
         struct b;
     }
 
     C can only be declared after b has been declared and the same is true for b.
     therefore we recursively try to resolve this structs until no change detect
     """
-    post_resolve_len = len(structs) + 1
-    pre_resolve_len = len(structs)
-    while pre_resolve_len != post_resolve_len:
-        pre_resolve_len = len(structs)
-        resolvers_to_remove = []
+    can_resolve = True
+    while can_resolve:
+        can_resolve = False
         for struct in lazy_resolvers:
+            logging.info("LazyResolver resolving: {}".format(struct.struct_name))
             resolved_struct = struct.resolve(structs)
             if resolved_struct:
+                can_resolve = True
                 lazy_resolvers.remove(struct)
                 for i in range(len(structs)):
                     if structs[i].__struct_name__ == struct.struct_name:
                         structs[i] = resolved_struct
 
-        for resolver in resolvers_to_remove:
-            resolver.remove(resolver)
-        post_resolve_len = len(structs)
-
     # Now removing all lazy resolve objects
     keys_to_delete = []
     for struct in structs:
         if isinstance(struct, LazyResolveStruct):
+            logging.info("Couldn't resolve: {}".format(struct.struct_name))
             keys_to_delete.append(struct)
 
     for key in keys_to_delete:
         structs.remove(key)
 
     return structs
```

### Comparing `py_elf_structs-1.4.1/py_elf_structs/__main__.py` & `py_elf_structs-1.4.2/py_elf_structs/__main__.py`

 * *Files identical despite different names*

### Comparing `py_elf_structs-1.4.1/README.md` & `py_elf_structs-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `py_elf_structs-1.4.1/setup.py` & `py_elf_structs-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     README = pypandoc.convert(os.path.join(os.path.dirname(__file__), 'README.md'), 'rst')
 except (ImportError, OSError) as e:
     print("Can't convert readme: {}".format(e))
     README = ""
 
 setup(
     name='py_elf_structs',
-    version='1.4.1',
+    version='1.4.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=['cstruct==1.8', 'pyelftools'],
     license='MIT License',
     description='Python package to extract struct and type information from dwarf and build python cstructs',
     long_description=README,
     url='https://github.com/jonatanSh/py-elf-structs',
```

