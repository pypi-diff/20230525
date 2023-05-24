# Comparing `tmp/pyresidfp-0.6.6.tar.gz` & `tmp/pyresidfp-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.6.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyresidfp-0.6.7.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.6.6.tar` & `pyresidfp-0.6.7.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0     3914 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/COPYING
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/README.md
--rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/PythonSid.cpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/PythonSid.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/config.h.in
--rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/__init__.py
--rw-r--r--   0        0        0     8617 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/_pyresidfp/__init__.pyi
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/_version.py
--rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/musical_scale.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/py.typed
--rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/registers.py
--rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/AUTHORS
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/COPYING
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Dac.cpp
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Dac.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/ExternalFilter.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/ExternalFilter.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter.cpp
--rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter6581.cpp
--rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter6581.h
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter8580.cpp
--rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter8580.h
--rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig.h
--rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator6581.cpp
--rw-r--r--   0        0        0     9200 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator6581.h
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator8580.cpp
--rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator8580.h
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/OpAmp.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/OpAmp.h
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Potentiometer.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/README
--rw-r--r--   0        0        0    13759 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/SID.cpp
--rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/SID.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Spline.cpp
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Spline.h
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Voice.h
--rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformCalculator.h
--rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformGenerator.h
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/array.h
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/Resampler.h
--rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/SincResampler.h
--rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/siddefs-fp.h.in
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/version.cc
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/sidcxx11.h
--rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/sidcxx14.h
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     3943 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/README.md
+-rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/PythonSid.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/config.h.in
+-rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0     8720 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/_pyresidfp/__init__.pyi
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/py.typed
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     9187 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/COPYING
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9200 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/README
+-rw-r--r--   0        0        0    13759 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Voice.h
+-rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/version.cc
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/sidcxx11.h
+-rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/sidcxx14.h
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/tests/test_basic.py
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/tests/test_versions.py
+-rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/PKG-INFO
```

### Comparing `pyresidfp-0.6.6/CMakeLists.txt` & `pyresidfp-0.6.7/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 pybind11_add_module(_pyresidfp MODULE
         ${HEADER_FILES} ${SOURCE_FILES})
 target_include_directories(_pyresidfp
         PRIVATE ${CMAKE_CURRENT_BINARY_DIR} ${CMAKE_CURRENT_SOURCE_DIR}
         src/residfp src/residfp/resample)
 target_compile_definitions(_pyresidfp PRIVATE HAVE_CONFIG_H)
-target_compile_definitions(_pyresidfp PRIVATE PROJECT_VERSION)
+target_compile_definitions(_pyresidfp PRIVATE PROJECT_VERSION="${SKBUILD_PROJECT_VERSION}")
 set_property(TARGET _pyresidfp PROPERTY CXX_STANDARD 14)
 
 if (IPO_SUPPORTED)
   message(STATUS "IPO / LTO enabled")
   set_property(TARGET _pyresidfp PROPERTY INTERPROCEDURAL_OPTIMIZATION TRUE)
 else()
   message(STATUS "IPO / LTO not supported: <${IPO_ERROR}>")
```

### Comparing `pyresidfp-0.6.6/COPYING` & `pyresidfp-0.6.7/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/README.md` & `pyresidfp-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/pyproject.toml` & `pyresidfp-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/PythonSid.cpp` & `pyresidfp-0.6.7/src/PythonSid.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/PythonSid.h` & `pyresidfp-0.6.7/src/PythonSid.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/pyresidfp/__init__.py` & `pyresidfp-0.6.7/src/pyresidfp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/pyresidfp/_pyresidfp/__init__.pyi` & `pyresidfp-0.6.7/src/pyresidfp/_pyresidfp/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,19 @@
 
 class SID:
     """
     MOS6581/MOS8580 emulation.
     """
 
     def __init__(
-        self, arg0: ChipModel, arg1: SamplingMethod, arg2: float, arg3: float
+        self,
+        chip_model: ChipModel,
+        method: SamplingMethod,
+        clock_frequency: float,
+        sampling_frequency: float,
     ) -> None:
         """
         Creates a new instance of SID and sets sampling parameters.
 
         Use a clock freqency of 985248Hz for PAL C64, 1022730Hz for NTSC C64.
         The default end of passband frequency is pass_freq = 0.9*sample_freq/2
         for sample frequencies up to ~ 44.1kHz, and 20kHz for higher sample frequencies.
@@ -73,69 +77,69 @@
         For resampling, the ratio between the clock frequency and the sample frequency
         is limited as follows: 125*clock_freq/sample_freq < 16384
         E.g. provided a clock frequency of ~ 1MHz, the sample frequency can not be set
         lower than ~ 8kHz. A lower sample frequency would make the resampling code
         overfill its 16k sample ring buffer.
 
         Args:
-            chipModel (_pyresidfp.ChipModel):   Chip model to emulate
+            chip_model (_pyresidfp.ChipModel):  Chip model to emulate
             method (_pyresidfp.SamplingMethod): Sampling method to use
-            clockFrequency (float):             System clock frequency at Hz
-            samplingFrequency (float):          Desired output sampling rate
+            clock_frequency (float):            System clock frequency at Hz
+            sampling_frequency (float):         Desired output sampling rate
 
         Raises:
             RuntimeError
 
         Examples:
             Construct an emulated MOS 6581 chip with resampling sample method, PAL clock frequency,
             and a sampling frequency of 48kHz:
 
             >>> sid = SID(ChipModel.MOS6581, SamplingMethod.RESAMPLE, 985248.0, 48000.0)
         """
-    def clock(self, arg0: int) -> typing.List[int]:
+    def clock(self, cycles: int) -> typing.List[int]:
         """
         Clock SID forward using chosen output sampling algorithm and sample.
 
         Note:
             The number of samples is equal to
 
             samples = samplingFrequency * cycles / clockFrequency
 
         Args:
             cycles (int): Number of clock cycles to forward
 
         Returns:
              :obj:`list` of :obj:`int` samples in range -32768 to 32767
         """
-    def enable_filter(self, arg0: bool) -> None:
+    def enable_filter(self, enable: bool) -> None:
         """
         Enable filter emulation.
 
         Args:
             enable (bool): False to turn off filter emulation
         """
-    def input(self, arg0: int) -> None:
+    def input(self, value: int) -> None:
         """
         16-bit input (EXT IN). Write 16-bit sample to audio input. NB! The caller
         is responsible for keeping the value within 16 bits. Note that to mix in
         an external audio signal, the signal should be resampled to 1MHz first to\
         avoid sampling noise.
 
         Args:
             value (int): Input level to set
         """
-    def mute(self, arg0: int, arg1: bool) -> None:
+    def mute(self, channel: int, enable: bool) -> None:
         """
         SID voice muting.
 
         Args:
             channel (int): Channel to modify
             enable (bool): enable muting
         """
-    def read(self, arg0: int) -> int:
+    def read(self, offset: int) -> int:
         """
         Read registers.
 
         Reading a write only register returns the last char written to any SID register.
         The individual bits in this value start to fade down towards zero after a few cycles.
         All bits reach zero within approximately $2000 - $4000 cycles.
         It has been claimed that this fading happens in an orderly fashion,
@@ -161,29 +165,29 @@
     def reset(self) -> None:
         """
         Resets chip model, voice registers, filters and sampling method.
 
         Raises:
             RuntimeError
         """
-    def set_filter_6581_curve(self, arg0: float) -> None:
+    def set_filter_6581_curve(self, curve_position: float) -> None:
         """
         Set filter curve parameter for 6581 model.
 
         Args:
-            curvePosition (float): 0 .. 1, where 0 sets center frequency high ("light") and 1 sets it low ("dark"), default is 0.5
+            curve_position (float): 0 .. 1, where 0 sets center frequency high ("light") and 1 sets it low ("dark"), default is 0.5
         """
-    def set_filter_8580_curve(self, arg0: float) -> None:
+    def set_filter_8580_curve(self, curve_position: float) -> None:
         """
         Set filter curve parameter for 8580 model.
 
         Args:
-            curvePosition (float):
+            curve_position (float):
         """
-    def write(self, arg0: int, arg1: int) -> None:
+    def write(self, offset: int, value: int) -> None:
         """
         Write registers.
 
         Args:
             offset (int): Chip register to write to
             value  (char): Value to write
         """
```

### Comparing `pyresidfp-0.6.6/src/pyresidfp/musical_scale.py` & `pyresidfp-0.6.7/src/pyresidfp/musical_scale.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/pyresidfp/registers.py` & `pyresidfp-0.6.7/src/pyresidfp/registers.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.6.7/src/pyresidfp/sound_interface_device.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/pyresidfp.cpp` & `pyresidfp-0.6.7/src/pyresidfp.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -80,32 +80,34 @@
                Two-pass resampling
             )pbdoc");
 
     py::class_<::pysid::PythonSid>(m, "SID", R"pbdoc(
                MOS6581/MOS8580 emulation.
             )pbdoc")
 
-            .def(py::init<sid::ChipModel, sid::SamplingMethod, double, double>(), R"pbdoc(
+            .def(py::init<sid::ChipModel, sid::SamplingMethod, double, double>(),
+                    py::arg("chip_model"), py::arg("method"), py::arg("clock_frequency"), py::arg("sampling_frequency"),
+                    R"pbdoc(
                Creates a new instance of SID and sets sampling parameters.
 
                Use a clock freqency of 985248Hz for PAL C64, 1022730Hz for NTSC C64.
                The default end of passband frequency is pass_freq = 0.9*sample_freq/2
                for sample frequencies up to ~ 44.1kHz, and 20kHz for higher sample frequencies.
 
                For resampling, the ratio between the clock frequency and the sample frequency
                is limited as follows: 125*clock_freq/sample_freq < 16384
                E.g. provided a clock frequency of ~ 1MHz, the sample frequency can not be set
                lower than ~ 8kHz. A lower sample frequency would make the resampling code
                overfill its 16k sample ring buffer.
 
                Args:
-                   chipModel (_pyresidfp.ChipModel):   Chip model to emulate
+                   chip_model (_pyresidfp.ChipModel):  Chip model to emulate
                    method (_pyresidfp.SamplingMethod): Sampling method to use
-                   clockFrequency (float):             System clock frequency at Hz
-                   samplingFrequency (float):          Desired output sampling rate
+                   clock_frequency (float):            System clock frequency at Hz
+                   sampling_frequency (float):         Desired output sampling rate
 
                Raises:
                    RuntimeError
 
                Examples:
                    Construct an emulated MOS 6581 chip with resampling sample method, PAL clock frequency,
                    and a sampling frequency of 48kHz:
@@ -132,25 +134,25 @@
             .def("reset", &::pysid::PythonSid::reset, R"pbdoc(
                Resets chip model, voice registers, filters and sampling method.
 
                Raises:
                    RuntimeError
             )pbdoc")
 
-            .def("input", &::pysid::PythonSid::input, R"pbdoc(
+            .def("input", &::pysid::PythonSid::input, py::arg("value"), R"pbdoc(
                16-bit input (EXT IN). Write 16-bit sample to audio input. NB! The caller
                is responsible for keeping the value within 16 bits. Note that to mix in
                an external audio signal, the signal should be resampled to 1MHz first to\
                avoid sampling noise.
 
                Args:
                    value (int): Input level to set
             )pbdoc")
 
-            .def("read", &::pysid::PythonSid::read, R"pbdoc(
+            .def("read", &::pysid::PythonSid::read, py::arg("offset"), R"pbdoc(
                Read registers.
 
                Reading a write only register returns the last char written to any SID register.
                The individual bits in this value start to fade down towards zero after a few cycles.
                All bits reach zero within approximately $2000 - $4000 cycles.
                It has been claimed that this fading happens in an orderly fashion,
                however sampling of write only registers reveals that this is not the case.
@@ -169,59 +171,59 @@
                Args:
                    offset (int): SID register to read
 
                Returns:
                    char: Value read from chip
             )pbdoc")
 
-            .def("write", &::pysid::PythonSid::write, R"pbdoc(
+            .def("write", &::pysid::PythonSid::write, py::arg("offset"), py::arg("value"), R"pbdoc(
                Write registers.
 
                Args:
                    offset (int): Chip register to write to
                    value  (char): Value to write
             )pbdoc")
 
-            .def("mute", &::pysid::PythonSid::mute, R"pbdoc(
+            .def("mute", &::pysid::PythonSid::mute, py::arg("channel"), py::arg("enable"), R"pbdoc(
                SID voice muting.
 
                Args:
                    channel (int): Channel to modify
                    enable (bool): enable muting
             )pbdoc")
 
-            .def("clock", &::pysid::PythonSid::clock, R"pbdoc(
+            .def("clock", &::pysid::PythonSid::clock, py::arg("cycles"), R"pbdoc(
                Clock SID forward using chosen output sampling algorithm and sample.
 
                Note:
                    The number of samples is equal to
 
                    samples = samplingFrequency * cycles / clockFrequency
 
                Args:
                    cycles (int): Number of clock cycles to forward
 
                Returns:
                     :obj:`list` of :obj:`int` samples in range -32768 to 32767
             )pbdoc")
 
-            .def("set_filter_6581_curve", &::pysid::PythonSid::setFilter6581Curve, R"pbdoc(
+            .def("set_filter_6581_curve", &::pysid::PythonSid::setFilter6581Curve, py::arg("curve_position"), R"pbdoc(
                Set filter curve parameter for 6581 model.
 
                Args:
-                   curvePosition (float): 0 .. 1, where 0 sets center frequency high ("light") and 1 sets it low ("dark"), default is 0.5
+                   curve_position (float): 0 .. 1, where 0 sets center frequency high ("light") and 1 sets it low ("dark"), default is 0.5
             )pbdoc")
 
-            .def("set_filter_8580_curve", &::pysid::PythonSid::setFilter8580Curve, R"pbdoc(
+            .def("set_filter_8580_curve", &::pysid::PythonSid::setFilter8580Curve, py::arg("curve_position"), R"pbdoc(
                Set filter curve parameter for 8580 model.
 
                Args:
-                   curvePosition (float):
+                   curve_position (float):
             )pbdoc")
 
-            .def("enable_filter", &::pysid::PythonSid::enableFilter, R"pbdoc(
+            .def("enable_filter", &::pysid::PythonSid::enableFilter, py::arg("enable"), R"pbdoc(
                Enable filter emulation.
 
                Args:
                    enable (bool): False to turn off filter emulation
             )pbdoc");
 }
```

### Comparing `pyresidfp-0.6.6/src/residfp/COPYING` & `pyresidfp-0.6.7/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Dac.cpp` & `pyresidfp-0.6.7/src/residfp/Dac.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Dac.h` & `pyresidfp-0.6.7/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.6.7/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/ExternalFilter.h` & `pyresidfp-0.6.7/src/residfp/ExternalFilter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Filter.cpp` & `pyresidfp-0.6.7/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Filter.h` & `pyresidfp-0.6.7/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Filter6581.cpp` & `pyresidfp-0.6.7/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Filter6581.h` & `pyresidfp-0.6.7/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Filter8580.cpp` & `pyresidfp-0.6.7/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Filter8580.h` & `pyresidfp-0.6.7/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.6.7/src/residfp/FilterModelConfig.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/FilterModelConfig.h` & `pyresidfp-0.6.7/src/residfp/FilterModelConfig.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.cpp` & `pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.cpp` & `pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Integrator6581.cpp` & `pyresidfp-0.6.7/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Integrator6581.h` & `pyresidfp-0.6.7/src/residfp/Integrator6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Integrator8580.cpp` & `pyresidfp-0.6.7/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Integrator8580.h` & `pyresidfp-0.6.7/src/residfp/Integrator8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/OpAmp.cpp` & `pyresidfp-0.6.7/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/OpAmp.h` & `pyresidfp-0.6.7/src/residfp/OpAmp.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Potentiometer.h` & `pyresidfp-0.6.7/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/README` & `pyresidfp-0.6.7/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/SID.cpp` & `pyresidfp-0.6.7/src/residfp/SID.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/SID.h` & `pyresidfp-0.6.7/src/residfp/SID.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Spline.cpp` & `pyresidfp-0.6.7/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Spline.h` & `pyresidfp-0.6.7/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/Voice.h` & `pyresidfp-0.6.7/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/WaveformCalculator.cpp` & `pyresidfp-0.6.7/src/residfp/WaveformCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/WaveformCalculator.h` & `pyresidfp-0.6.7/src/residfp/WaveformCalculator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.6.7/src/residfp/WaveformGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/WaveformGenerator.h` & `pyresidfp-0.6.7/src/residfp/WaveformGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/array.h` & `pyresidfp-0.6.7/src/residfp/array.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/resample/Resampler.h` & `pyresidfp-0.6.7/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.6.7/src/residfp/resample/SincResampler.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/resample/SincResampler.h` & `pyresidfp-0.6.7/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.6.7/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.6.7/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.6.7/src/residfp/siddefs-fp.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/residfp/version.cc` & `pyresidfp-0.6.7/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/sidcxx11.h` & `pyresidfp-0.6.7/src/sidcxx11.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/src/sidcxx14.h` & `pyresidfp-0.6.7/src/sidcxx14.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.6/PKG-INFO` & `pyresidfp-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.6.6
+Version: 0.6.7
 Summary: Emulates the SID sound-chip
 Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

