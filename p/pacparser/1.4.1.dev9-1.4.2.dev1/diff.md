# Comparing `tmp/pacparser-1.4.1.dev9.tar.gz` & `tmp/pacparser-1.4.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacparser-1.4.1.dev9.tar", last modified: Wed May 24 05:41:36 2023, max compression
+gzip compressed data, was "pacparser-1.4.2.dev1.tar", last modified: Thu May 25 18:01:50 2023, max compression
```

## Comparing `pacparser-1.4.1.dev9.tar` & `pacparser-1.4.2.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:41:36.293882 pacparser-1.4.1.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 05:41:25.000000 pacparser-1.4.1.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 05:41:36.293882 pacparser-1.4.1.dev9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:41:36.293882 pacparser-1.4.1.dev9/pacparser/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-24 05:41:25.000000 pacparser-1.4.1.dev9/pacparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:41:36.293882 pacparser-1.4.1.dev9/pacparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 05:41:36.000000 pacparser-1.4.1.dev9/pacparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 05:41:36.000000 pacparser-1.4.1.dev9/pacparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 05:41:36.000000 pacparser-1.4.1.dev9/pacparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 05:41:36.000000 pacparser-1.4.1.dev9/pacparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-24 05:41:25.000000 pacparser-1.4.1.dev9/pacparser_py.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 05:41:36.293882 pacparser-1.4.1.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-24 05:41:25.000000 pacparser-1.4.1.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:01:50.121781 pacparser-1.4.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 18:01:50.117780 pacparser-1.4.2.dev1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:01:50.117780 pacparser-1.4.2.dev1/pacparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/pacparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:01:50.117780 pacparser-1.4.2.dev1/pacparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/pacparser_py.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:01:50.121781 pacparser-1.4.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/setup.py
```

### Comparing `pacparser-1.4.1.dev9/pacparser/__init__.py` & `pacparser-1.4.2.dev1/pacparser/__init__.py`

 * *Files identical despite different names*

### Comparing `pacparser-1.4.1.dev9/pacparser_py.c` & `pacparser-1.4.2.dev1/pacparser_py.c`

 * *Files identical despite different names*

### Comparing `pacparser-1.4.1.dev9/setup.py` & `pacparser-1.4.2.dev1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2007-2022 Manu Garg.
+# Copyright (C) 2007-2023 Manu Garg.
 # Author: Manu Garg <manugarg@gmail.com>
 #
 # pacparser is a library that provides methods to parse proxy auto-config
 # (PAC) files. Please read README file included with this package for more
 # information about this library.
 #
 # pacparser is free software; you can redistribute it and/or
@@ -35,127 +35,146 @@
 
 from unittest.mock import patch
 import distutils
 from setuptools import setup, Extension
 
 import distutils.cmd
 
+
 def setup_dir():
-  return os.path.dirname(os.path.join(os.getcwd(), sys.argv[0]))
+    return os.path.dirname(os.path.join(os.getcwd(), sys.argv[0]))
+
 
 def module_path():
-  py_ver = '*'.join([str(x) for x in sys.version_info[0:2]])
-  print('Python version: %s' % py_ver)
-  
-  builddir = os.path.join(setup_dir(), 'build')
-  print('Build dir: %s' % builddir)
-  print(os.listdir(builddir))
-  
-  return glob.glob(os.path.join(builddir, 'lib*%s*' % py_ver))[0]
+    py_ver = "*".join([str(x) for x in sys.version_info[0:2]])
+    print("Python version: %s" % py_ver)
 
-def sanitize_version(ver):
-  ver = ver.strip()
-  # Strip first 'v' and last part from git provided versions.
-  # For example, v1.3.8-12-g231 becomes v1.3.8-12.
-  ver = re.sub(r'^v?([\d]+\.[\d]+\.[\d]+(-[\d]+)).*$', '\\1', ver)
-  # 1.3.8-12 becomes 1.3.8.dev12
-  return ver.replace('-', '.dev')
+    builddir = os.path.join(setup_dir(), "build")
+    print("Build dir: %s" % builddir)
+    print(os.listdir(builddir))
 
-def git_version():
-  return sanitize_version(subprocess.check_output(
-    'git describe --always --tags --candidate=100'.split(' '),
-    text=True
-  ))
+    return glob.glob(os.path.join(builddir, "lib*%s*" % py_ver))[0]
 
-def pacparser_version():
-  if subprocess.call('git rev-parse --git-dir'.split(' '),
-                     stderr=subprocess.DEVNULL) == 0:
-    return git_version()
-
-  # Check if we have version.mk. It's added in the manual release tarball.
-  version_file = os.path.join(setup_dir(), '..', 'version.mk')
-  if os.path.exists(version_file):
-    with open(version_file) as f:
-      return sanitize_version(f.read().replace('VERSION=',''))
 
-  return sanitize_version(os.environ.get('PACPARSER_VERSION', '1.0.0'))
+def sanitize_version(ver):
+    ver = ver.strip()
+    # Strip first 'v' and last part from git provided versions.
+    # For example, v1.3.8-12-g231 becomes v1.3.8-12.
+    ver = re.sub(r"^v?([\d]{1,3}\.[\d]{1,3}\.[\d]{1,3}(-[\d]{1,3})).*$", "\\1", ver)
+    # 1.3.8-12 becomes 1.3.8.dev12
+    return ver.replace("-", ".dev")
+
 
+def git_version():
+    return sanitize_version(
+        subprocess.check_output(
+            "git describe --always --tags --candidate=100".split(" "), text=True
+        )
+    )
 
-class DistCmd(distutils.cmd.Command):
-  """Build pacparser python distribution."""
 
-  description = 'Build pacparser python distribution.'
-  user_options = []
+def pacparser_version():
+    if (
+        subprocess.call("git rev-parse --git-dir".split(" "), stderr=subprocess.DEVNULL)
+        == 0
+    ):
+        return git_version()
+
+    # Check if we have version.mk. It's added in the manual release tarball.
+    version_file = os.path.join(setup_dir(), "..", "version.mk")
+    if os.path.exists(version_file):
+        with open(version_file) as f:
+            return sanitize_version(f.read().replace("VERSION=", ""))
 
-  def initialize_options(self):
-    pass
+    return sanitize_version(os.environ.get("PACPARSER_VERSION", "1.0.0"))
 
-  def finalize_options(self):
-    pass
 
-  def run(self):
-    py_ver = '.'.join([str(x) for x in sys.version_info[0:2]])
-    pp_ver = pacparser_version()
+class DistCmd(distutils.cmd.Command):
+    """Build pacparser python distribution."""
 
-    mach = platform.machine().lower()
-    if mach == 'x86_64':
-      mach = 'amd64'
-    dist = 'pacparser-python%s-%s-%s-%s' % (
-      py_ver.replace('.',''), pp_ver, platform.system().lower(), mach)
+    description = "Build pacparser python distribution."
+    user_options = []
 
-    if os.path.exists(dist):
-      shutil.rmtree(dist)
-    os.mkdir(dist)
-    shutil.copytree(os.path.join(module_path(), 'pacparser'),
-                    dist+'/pacparser',
-                    ignore=shutil.ignore_patterns('*pycache*'))
+    def initialize_options(self):
+        # Override to do nothing.
+        pass
+
+    def finalize_options(self):
+        # Override to do nothing.
+        pass
+
+    def run(self):
+        py_ver = ".".join([str(x) for x in sys.version_info[0:2]])
+        pp_ver = pacparser_version()
+
+        mach = platform.machine().lower()
+        if mach == "x86_64":
+            mach = "amd64"
+        dist = "pacparser-python%s-%s-%s-%s" % (
+            py_ver.replace(".", ""),
+            pp_ver,
+            platform.system().lower(),
+            mach,
+        )
+
+        if os.path.exists(dist):
+            shutil.rmtree(dist)
+        os.mkdir(dist)
+        shutil.copytree(
+            os.path.join(module_path(), "pacparser"),
+            dist + "/pacparser",
+            ignore=shutil.ignore_patterns("*pycache*"),
+        )
 
 
-@patch('distutils.cygwinccompiler.get_msvcr')
+@patch("distutils.cygwinccompiler.get_msvcr")
 def main(patched_func):
-  python_home = os.path.dirname(sys.executable)
+    python_home = os.path.dirname(sys.executable)
 
-  extra_objects = []
-  obj_search_path = {
-    'pacparser.o': ['..', '.'],
-    'libjs.a': ['../spidermonkey', '.'],
-  }
-  for obj, paths in obj_search_path.items():
-    for path in paths:
-      if os.path.exists(os.path.join(path, obj)):
-        extra_objects.append(os.path.join(path, obj))
-        break
-
-  libraries = []
-  extra_link_args = []
-  if sys.platform == 'win32':
-    extra_objects = ['../pacparser.o', '../spidermonkey/js.lib']
-    libraries = ['ws2_32']
-    # python_home has vcruntime140.dll
-    patched_func.return_value =  ['vcruntime140']
-    extra_link_args = ['-static-libgcc', '-L'+python_home]
-
-  pacparser_module = Extension('_pacparser',
-                               include_dirs = ['..'],
-                               sources = ['pacparser_py.c'],
-                               libraries = libraries,
-                               extra_link_args = extra_link_args,
-                               extra_objects = extra_objects)
-  setup (
+    extra_objects = []
+    obj_search_path = {
+        "pacparser.o": ["..", "."],
+        "libjs.a": ["../spidermonkey", "."],
+    }
+    for obj, paths in obj_search_path.items():
+        for path in paths:
+            if os.path.exists(os.path.join(path, obj)):
+                extra_objects.append(os.path.join(path, obj))
+                break
+
+    libraries = []
+    extra_link_args = []
+    if sys.platform == "win32":
+        extra_objects = ["../pacparser.o", "../spidermonkey/js.lib"]
+        libraries = ["ws2_32"]
+        # python_home has vcruntime140.dll
+        patched_func.return_value = ["vcruntime140"]
+        extra_link_args = ["-static-libgcc", "-L" + python_home]
+
+    pacparser_module = Extension(
+        "_pacparser",
+        include_dirs=[".."],
+        sources=["pacparser_py.c"],
+        libraries=libraries,
+        extra_link_args=extra_link_args,
+        extra_objects=extra_objects,
+    )
+    setup(
         cmdclass={
-            'dist': DistCmd,
+            "dist": DistCmd,
         },
-        name = 'pacparser',
-        version = pacparser_version(),
-        description = 'Pacparser package',
-        author = 'Manu Garg',
-        author_email = 'manugarg@gmail.com',
-        url = 'http://github.com/manugarg/pacparser',
-        long_description = ('python library to parse proxy auto-config (PAC) '
-                            'files.'),
-        license = 'LGPL',
-        ext_package = 'pacparser',
-        ext_modules = [pacparser_module],
-        py_modules = ['pacparser.__init__'])
+        name="pacparser",
+        version=pacparser_version(),
+        description="Pacparser package",
+        author="Manu Garg",
+        author_email="manugarg@gmail.com",
+        url="https://github.com/manugarg/pacparser",
+        long_description=("python library to parse proxy auto-config (PAC) files."),
+        license="LGPL",
+        ext_package="pacparser",
+        ext_modules=[pacparser_module],
+        py_modules=["pacparser.__init__"],
+    )
+
 
-if __name__ == '__main__':
-  main()
+if __name__ == "__main__":
+    main()
```

