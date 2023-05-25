# Comparing `tmp/pyeCam-0.0.8.tar.gz` & `tmp/pyeCam-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeCam-0.0.8.tar", last modified: Wed May 24 09:48:31 2023, max compression
+gzip compressed data, was "pyeCam-0.0.9.tar", last modified: Wed May 24 09:53:29 2023, max compression
```

## Comparing `pyeCam-0.0.8.tar` & `pyeCam-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:48:31.182210 pyeCam-0.0.8/
--rw-rw-rw-   0        0        0      151 2023-05-24 09:48:31.182210 pyeCam-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    16186 2023-05-24 09:47:39.000000 pyeCam-0.0.8/pyeCam.cpp
-drwxrwxrwx   0        0        0        0 2023-05-24 09:48:31.182210 pyeCam-0.0.8/pyeCam.egg-info/
--rw-rw-rw-   0        0        0      151 2023-05-24 09:48:31.000000 pyeCam-0.0.8/pyeCam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-24 09:48:31.000000 pyeCam-0.0.8/pyeCam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:48:31.000000 pyeCam-0.0.8/pyeCam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 09:48:31.000000 pyeCam-0.0.8/pyeCam.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-24 09:48:31.000000 pyeCam-0.0.8/pyeCam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 09:48:31.182210 pyeCam-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1973 2023-05-24 09:46:07.000000 pyeCam-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:53:29.916577 pyeCam-0.0.9/
+-rw-rw-rw-   0        0        0      151 2023-05-24 09:53:29.916577 pyeCam-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16366 2023-05-24 09:52:44.000000 pyeCam-0.0.9/pyeCam.cpp
+drwxrwxrwx   0        0        0        0 2023-05-24 09:53:29.916577 pyeCam-0.0.9/pyeCam.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-05-24 09:53:29.000000 pyeCam-0.0.9/pyeCam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-05-24 09:53:29.000000 pyeCam-0.0.9/pyeCam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:53:29.000000 pyeCam-0.0.9/pyeCam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 09:53:29.000000 pyeCam-0.0.9/pyeCam.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-24 09:53:29.000000 pyeCam-0.0.9/pyeCam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:53:29.916577 pyeCam-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-05-24 09:52:54.000000 pyeCam-0.0.9/setup.py
```

### Comparing `pyeCam-0.0.8/pyeCam.cpp` & `pyeCam-0.0.9/pyeCam.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,22 @@
 	bool getDeviceCount(pybind11::object& gDeviceCount) 
 	{
 		printf(" getDeviceCount called");
 	  initialize();
 	  printf(" getDeviceCount initialize()");
 	  int list = indexList;
 	  printf("Before list and gDeviceCount.attr(value) %d\n ",list);
+	  try
+	  {
 	  gDeviceCount.attr("value") = 0;
+	  }
+	 catch (const std::exception& ex) 
+		{
+			std::cout << "getDeviceCount(pybind11::object& gDeviceCount)  Exception caught: " << ex.what() << std::endl;
+		}
 	  if (!indexList) 
 	  {
 		printf(" getDeviceCount Device count failed");
 		 return false;
 	  }
 	  while (list)
 	  {
```

### Comparing `pyeCam-0.0.8/setup.py` & `pyeCam-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ext.extra_compile_args = extra_compile_args
             ext.extra_link_args = extra_link_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='pyeCam',
-    version='0.0.8',
+    version='0.0.9',
     description='Example project using pybind11',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

