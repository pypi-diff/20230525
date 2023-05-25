# Comparing `tmp/cupy-9.5.0.tar.gz` & `tmp/cupy-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cupy-9.5.0.tar", last modified: Wed Sep 29 18:02:42 2021, max compression
+gzip compressed data, was "dist/cupy-9.6.0.tar", last modified: Wed Nov 10 04:08:13 2021, max compression
```

## Comparing `cupy-9.5.0.tar` & `cupy-9.6.0.tar`

### file list

```diff
@@ -1,1001 +1,995 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/
--rw-r--r--   0 root         (0) root         (0)     1118 2021-09-29 17:55:54.000000 cupy-9.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      531 2021-09-29 17:55:54.000000 cupy-9.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2839 2021-09-29 18:02:42.000000 cupy-9.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4871 2021-09-29 17:55:54.000000 cupy-9.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/
--rw-r--r--   0 root         (0) root         (0)    31992 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_binary/
--rw-r--r--   0 root         (0) root         (0)      109 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_binary/__init__.py
--rw-r--r--   0 root         (0) root         (0)      242 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_binary/elementwise.py
--rw-r--r--   0 root         (0) root         (0)     2017 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_binary/packing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)     3795 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_accelerator.pxd
--rw-r--r--   0 root         (0) root         (0)     1148 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_accelerator.pyx
--rw-r--r--   0 root         (0) root         (0)     1092 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_carray.pxd
--rw-r--r--   0 root         (0) root         (0)     1654 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_carray.pyx
--rw-r--r--   0 root         (0) root         (0)      966 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_codeblock.py
--rw-r--r--   0 root         (0) root         (0)      431 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_cub_reduction.pxd
--rw-r--r--   0 root         (0) root         (0)    25442 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_cub_reduction.pyx
--rw-r--r--   0 root         (0) root         (0)      123 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_dtype.pxd
--rw-r--r--   0 root         (0) root         (0)     2185 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_dtype.pyx
--rw-r--r--   0 root         (0) root         (0)     8073 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_interface.py
--rw-r--r--   0 root         (0) root         (0)    13473 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_kernel.pyx
--rw-r--r--   0 root         (0) root         (0)    11191 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_op.py
--rw-r--r--   0 root         (0) root         (0)     2759 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_optimization.py
--rw-r--r--   0 root         (0) root         (0)     1163 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_thread_local.pyx
--rw-r--r--   0 root         (0) root         (0)    22671 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_trace.pyx
--rw-r--r--   0 root         (0) root         (0)       95 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_variable.pxd
--rw-r--r--   0 root         (0) root         (0)    10759 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_fusion_variable.pyx
--rw-r--r--   0 root         (0) root         (0)    21037 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_gufuncs.py
--rw-r--r--   0 root         (0) root         (0)     4243 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_kernel.pxd
--rw-r--r--   0 root         (0) root         (0)    47100 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_kernel.pyx
--rw-r--r--   0 root         (0) root         (0)      180 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_memory_range.pxd
--rw-r--r--   0 root         (0) root         (0)     1108 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_memory_range.pyx
--rw-r--r--   0 root         (0) root         (0)      511 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_optimize_config.pxd
--rw-r--r--   0 root         (0) root         (0)     2172 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_optimize_config.pyx
--rw-r--r--   0 root         (0) root         (0)     2146 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_reduction.pxd
--rw-r--r--   0 root         (0) root         (0)    30212 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_reduction.pyx
--rw-r--r--   0 root         (0) root         (0)      143 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_binary.pxd
--rw-r--r--   0 root         (0) root         (0)     2226 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_binary.pyx
--rw-r--r--   0 root         (0) root         (0)      774 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_indexing.pxd
--rw-r--r--   0 root         (0) root         (0)    34532 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_indexing.pyx
--rw-r--r--   0 root         (0) root         (0)      879 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_linalg.pxd
--rw-r--r--   0 root         (0) root         (0)    31721 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_linalg.pyx
--rw-r--r--   0 root         (0) root         (0)      473 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_logic.pxd
--rw-r--r--   0 root         (0) root         (0)     3334 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_logic.pyx
--rw-r--r--   0 root         (0) root         (0)     1434 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_manipulation.pxd
--rw-r--r--   0 root         (0) root         (0)    24579 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_manipulation.pyx
--rw-r--r--   0 root         (0) root         (0)     1191 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_math.pxd
--rw-r--r--   0 root         (0) root         (0)    37618 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_math.pyx
--rw-r--r--   0 root         (0) root         (0)      237 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_sorting.pxd
--rw-r--r--   0 root         (0) root         (0)    11478 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_sorting.pyx
--rw-r--r--   0 root         (0) root         (0)     1048 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_statistics.pxd
--rw-r--r--   0 root         (0) root         (0)    24808 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_routines_statistics.pyx
--rw-r--r--   0 root         (0) root         (0)      720 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_scalar.pxd
--rw-r--r--   0 root         (0) root         (0)     9948 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_scalar.pyx
--rw-r--r--   0 root         (0) root         (0)      283 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/_ufuncs.py
--rw-r--r--   0 root         (0) root         (0)     4888 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/core.pxd
--rw-r--r--   0 root         (0) root         (0)    87520 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/core.pyx
--rw-r--r--   0 root         (0) root         (0)      135 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/dlpack.pxd
--rw-r--r--   0 root         (0) root         (0)    10120 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/dlpack.pyx
--rw-r--r--   0 root         (0) root         (0)      950 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/flags.pyx
--rw-r--r--   0 root         (0) root         (0)    35369 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/fusion.pyx
--rw-r--r--   0 root         (0) root         (0)     4523 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/halffloat.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/
--rw-r--r--   0 root         (0) root         (0)      968 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/
--rw-r--r--   0 root         (0) root         (0)      187 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.0/
--rwxr-xr-x   0 root         (0) root         (0)    88634 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.h
--rwxr-xr-x   0 root         (0) root         (0)    72855 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.1/
--rwxr-xr-x   0 root         (0) root         (0)   109152 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.h
--rwxr-xr-x   0 root         (0) root         (0)    73059 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.2/
--rwxr-xr-x   0 root         (0) root         (0)   109689 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.h
--rwxr-xr-x   0 root         (0) root         (0)    73401 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.0/
--rwxr-xr-x   0 root         (0) root         (0)   125376 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.h
--rwxr-xr-x   0 root         (0) root         (0)    81098 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.1/
--rwxr-xr-x   0 root         (0) root         (0)   126227 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.h
--rwxr-xr-x   0 root         (0) root         (0)    86543 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.2/
--rw-r--r--   0 root         (0) root         (0)   126844 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.2/cuda_fp16.h
--rw-r--r--   0 root         (0) root         (0)    89130 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.2/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.3/
--rw-r--r--   0 root         (0) root         (0)   126844 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.3/cuda_fp16.h
--rw-r--r--   0 root         (0) root         (0)    89807 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.3/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.4/
--rw-r--r--   0 root         (0) root         (0)   127105 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.4/cuda_fp16.h
--rw-r--r--   0 root         (0) root         (0)    90464 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.4/cuda_fp16.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-9.2/
--rw-r--r--   0 root         (0) root         (0)    70901 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.h
--rw-r--r--   0 root         (0) root         (0)    72507 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.hpp
--rw-r--r--   0 root         (0) root         (0)     3539 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/atomics.cuh
--rw-r--r--   0 root         (0) root         (0)    17630 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/carray.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/
--rw-r--r--   0 root         (0) root         (0)       92 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/README.md
--rw-r--r--   0 root         (0) root         (0)     9577 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/arithmetic.h
--rw-r--r--   0 root         (0) root         (0)    24176 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/catrig.h
--rw-r--r--   0 root         (0) root         (0)    14169 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/catrigf.h
--rw-r--r--   0 root         (0) root         (0)     7149 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/ccosh.h
--rw-r--r--   0 root         (0) root         (0)     4554 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/ccoshf.h
--rw-r--r--   0 root         (0) root         (0)     5764 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/cexp.h
--rw-r--r--   0 root         (0) root         (0)     4954 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/cexpf.h
--rw-r--r--   0 root         (0) root         (0)     5921 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/clog.h
--rw-r--r--   0 root         (0) root         (0)     5455 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/clogf.h
--rw-r--r--   0 root         (0) root         (0)    20245 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/complex.h
--rw-r--r--   0 root         (0) root         (0)     4393 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/complex_inl.h
--rw-r--r--   0 root         (0) root         (0)     1550 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/cpow.h
--rw-r--r--   0 root         (0) root         (0)     1841 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/cproj.h
--rw-r--r--   0 root         (0) root         (0)     6689 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/csinh.h
--rw-r--r--   0 root         (0) root         (0)     4500 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/csinhf.h
--rw-r--r--   0 root         (0) root         (0)     4554 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/csqrt.h
--rw-r--r--   0 root         (0) root         (0)     4459 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/csqrtf.h
--rw-r--r--   0 root         (0) root         (0)     6089 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/ctanh.h
--rw-r--r--   0 root         (0) root         (0)     3739 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/ctanhf.h
--rw-r--r--   0 root         (0) root         (0)     4299 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex/math_private.h
--rw-r--r--   0 root         (0) root         (0)     2141 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/complex.cuh
--rw-r--r--   0 root         (0) root         (0)     1518 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/cuComplex_bridge.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/
--rw-r--r--   0 root         (0) root         (0)    22309 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/CHANGE_LOG.TXT
--rw-r--r--   0 root         (0) root         (0)     1600 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/LICENSE.TXT
--rw-r--r--   0 root         (0) root         (0)     6051 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/README.md
--rw-r--r--   0 root         (0) root         (0)     7688 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/common.mk
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/
--rw-r--r--   0 root         (0) root         (0)    33331 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    28525 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_downsweep.cuh
--rw-r--r--   0 root         (0) root         (0)    17917 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_upsweep.cuh
--rw-r--r--   0 root         (0) root         (0)    16916 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    24791 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce_by_key.cuh
--rw-r--r--   0 root         (0) root         (0)    35663 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_rle.cuh
--rw-r--r--   0 root         (0) root         (0)    18729 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    16655 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_segment_fixup.cuh
--rw-r--r--   0 root         (0) root         (0)    29594 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_select_if.cuh
--rw-r--r--   0 root         (0) root         (0)    27377 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_spmv_orig.cuh
--rw-r--r--   0 root         (0) root         (0)    27444 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/single_pass_scan_operators.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/
--rw-r--r--   0 root         (0) root         (0)    25011 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_adjacent_difference.cuh
--rw-r--r--   0 root         (0) root         (0)    54550 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_discontinuity.cuh
--rw-r--r--   0 root         (0) root         (0)    52305 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_exchange.cuh
--rw-r--r--   0 root         (0) root         (0)    16291 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    53671 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_load.cuh
--rw-r--r--   0 root         (0) root         (0)    25230 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_radix_rank.cuh
--rw-r--r--   0 root         (0) root         (0)    38342 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)     6181 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_raking_layout.cuh
--rw-r--r--   0 root         (0) root         (0)    25300 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)   102978 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    11964 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_shuffle.cuh
--rw-r--r--   0 root         (0) root         (0)    41449 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_store.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/
--rw-r--r--   0 root         (0) root         (0)     3285 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_atomic.cuh
--rw-r--r--   0 root         (0) root         (0)     8198 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_sort.cuh
--rw-r--r--   0 root         (0) root         (0)     9731 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking.cuh
--rw-r--r--   0 root         (0) root         (0)     8369 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking_commutative_only.cuh
--rw-r--r--   0 root         (0) root         (0)     9769 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_warp_reductions.cuh
--rw-r--r--   0 root         (0) root         (0)    28460 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_raking.cuh
--rw-r--r--   0 root         (0) root         (0)    19117 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans.cuh
--rw-r--r--   0 root         (0) root         (0)    20949 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans2.cuh
--rw-r--r--   0 root         (0) root         (0)    19463 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans3.cuh
--rw-r--r--   0 root         (0) root         (0)     3626 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/cub.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/
--rw-r--r--   0 root         (0) root         (0)    54347 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    13891 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_partition.cuh
--rw-r--r--   0 root         (0) root         (0)    42384 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)    38904 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    14817 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_run_length_encode.cuh
--rw-r--r--   0 root         (0) root         (0)    21786 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    54689 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)    36523 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    18838 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_select.cuh
--rw-r--r--   0 root         (0) root         (0)     8523 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_spmv.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/
--rw-r--r--   0 root         (0) root         (0)    57226 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    80406 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)    42707 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    25478 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce_by_key.cuh
--rw-r--r--   0 root         (0) root         (0)    23601 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_rle.cuh
--rw-r--r--   0 root         (0) root         (0)    22778 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    24454 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_select_if.cuh
--rw-r--r--   0 root         (0) root         (0)    33269 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_spmv_orig.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/
--rw-r--r--   0 root         (0) root         (0)     5861 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_barrier.cuh
--rw-r--r--   0 root         (0) root         (0)     8198 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_even_share.cuh
--rw-r--r--   0 root         (0) root         (0)     4827 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_mapping.cuh
--rw-r--r--   0 root         (0) root         (0)     7475 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_queue.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/host/
--rw-r--r--   0 root         (0) root         (0)     4581 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/host/mutex.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/
--rw-r--r--   0 root         (0) root         (0)     8781 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/arg_index_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     8104 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     8322 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_output_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     7650 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/constant_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     7369 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/counting_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     6817 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/discard_output_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)    10546 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/tex_obj_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)    12430 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/tex_ref_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     8611 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/transform_input_iterator.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/
--rw-r--r--   0 root         (0) root         (0)    18869 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_load.cuh
--rw-r--r--   0 root         (0) root         (0)     9228 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_operators.cuh
--rw-r--r--   0 root         (0) root         (0)     6037 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    10566 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_scan.cuh
--rw-r--r--   0 root         (0) root         (0)     4797 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_search.cuh
--rw-r--r--   0 root         (0) root         (0)    17932 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_store.cuh
--rw-r--r--   0 root         (0) root         (0)    28716 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_allocator.cuh
--rw-r--r--   0 root         (0) root         (0)     6955 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_arch.cuh
--rw-r--r--   0 root         (0) root         (0)     5061 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_debug.cuh
--rw-r--r--   0 root         (0) root         (0)    10658 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_device.cuh
--rw-r--r--   0 root         (0) root         (0)     3710 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_macro.cuh
--rw-r--r--   0 root         (0) root         (0)     2100 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_namespace.cuh
--rw-r--r--   0 root         (0) root         (0)    22318 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_ptx.cuh
--rw-r--r--   0 root         (0) root         (0)    40178 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_type.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/
--rw-r--r--   0 root         (0) root         (0)    21412 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_shfl.cuh
--rw-r--r--   0 root         (0) root         (0)    14280 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_smem.cuh
--rw-r--r--   0 root         (0) root         (0)    25284 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_shfl.cuh
--rw-r--r--   0 root         (0) root         (0)    16153 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_smem.cuh
--rw-r--r--   0 root         (0) root         (0)    25032 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/warp_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    38915 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/warp_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    16543 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/eclipse code style profile.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/
--rw-r--r--   0 root         (0) root         (0)     5255 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/Makefile
--rw-r--r--   0 root         (0) root         (0)    10724 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)     9644 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    11329 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
--rw-r--r--   0 root         (0) root         (0)     1554 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/
--rw-r--r--   0 root         (0) root         (0)     8830 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/Makefile
--rw-r--r--   0 root         (0) root         (0)     8173 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
--rw-r--r--   0 root         (0) root         (0)     8236 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
--rw-r--r--   0 root         (0) root         (0)     8303 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)     5825 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
--rw-r--r--   0 root         (0) root         (0)     6007 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
--rw-r--r--   0 root         (0) root         (0)     8156 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
--rw-r--r--   0 root         (0) root         (0)     8210 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
--rw-r--r--   0 root         (0) root         (0)     7493 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
--rw-r--r--   0 root         (0) root         (0)    13277 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/
--rw-r--r--   0 root         (0) root         (0)     4949 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/defunct/
--rw-r--r--   0 root         (0) root         (0)    37185 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
--rw-r--r--   0 root         (0) root         (0)    95317 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/
--rw-r--r--   0 root         (0) root         (0)     4374 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_cub.h
--rw-r--r--   0 root         (0) root         (0)     6368 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_gmem_atomics.h
--rw-r--r--   0 root         (0) root         (0)     6812 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_smem_atomics.h
--rw-r--r--   0 root         (0) root         (0)    21778 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
--rw-r--r--   0 root         (0) root         (0)    39231 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/sparse_matrix.h
--rw-r--r--   0 root         (0) root         (0)    30656 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
--rwxr-xr-x   0 root         (0) root         (0)      749 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/spmv_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/
--rw-r--r--   0 root         (0) root         (0)    18927 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/Makefile
--rw-r--r--   0 root         (0) root         (0)     8397 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/half.h
--rw-r--r--   0 root         (0) root         (0)      315 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/link_a.cu
--rw-r--r--   0 root         (0) root         (0)      315 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/link_b.cu
--rw-r--r--   0 root         (0) root         (0)     5148 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/mersenne.h
--rw-r--r--   0 root         (0) root         (0)    16564 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_allocator.cu
--rw-r--r--   0 root         (0) root         (0)     9623 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
--rw-r--r--   0 root         (0) root         (0)    19496 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
--rw-r--r--   0 root         (0) root         (0)    25392 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)    26628 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    34810 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_scan.cu
--rw-r--r--   0 root         (0) root         (0)    70313 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
--rw-r--r--   0 root         (0) root         (0)    46469 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)    49902 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    30363 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
--rw-r--r--   0 root         (0) root         (0)    31192 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
--rw-r--r--   0 root         (0) root         (0)    33600 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_scan.cu
--rw-r--r--   0 root         (0) root         (0)    37640 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
--rw-r--r--   0 root         (0) root         (0)    21518 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
--rw-r--r--   0 root         (0) root         (0)     5132 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
--rw-r--r--   0 root         (0) root         (0)    25549 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_iterator.cu
--rw-r--r--   0 root         (0) root         (0)    54847 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_util.h
--rw-r--r--   0 root         (0) root         (0)    27186 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    20350 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/tune/
--rw-r--r--   0 root         (0) root         (0)     6388 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/tune/Makefile
--rw-r--r--   0 root         (0) root         (0)    27663 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/dlpack/
--rw-r--r--   0 root         (0) root         (0)      232 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/dlpack/README.md
--rw-r--r--   0 root         (0) root         (0)     5308 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/dlpack/dlpack.h
--rw-r--r--   0 root         (0) root         (0)      623 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/hip_workaround.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/
--rw-r--r--   0 root         (0) root         (0)   106196 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/Doxyfile
--rw-r--r--   0 root         (0) root         (0)     1523 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2901 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/Makefile
--rw-r--r--   0 root         (0) root         (0)     3346 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/
--rw-r--r--   0 root         (0) root         (0)     2302 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/class_arg_kernel.cuh
--rw-r--r--   0 root         (0) root         (0)     1827 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/constant_header.cuh
--rw-r--r--   0 root         (0) root         (0)     1651 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/my_header1.cuh
--rw-r--r--   0 root         (0) root         (0)     1630 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/my_header2.cuh
--rw-r--r--   0 root         (0) root         (0)     1631 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/my_header3.cuh
--rw-r--r--   0 root         (0) root         (0)   160071 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/jitify.hpp
--rw-r--r--   0 root         (0) root         (0)    41241 2021-09-29 17:55:57.000000 cupy-9.5.0/cupy/_core/include/cupy/jitify/jitify_test.cu
--rw-r--r--   0 root         (0) root         (0)      655 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/math_constants.h
--rw-r--r--   0 root         (0) root         (0)      986 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/swap.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_core/include/cupy/tuple/
--rw-r--r--   0 root         (0) root         (0)    29357 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/tuple/tuple.h
--rw-r--r--   0 root         (0) root         (0)     1457 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/tuple/type_traits.h
--rw-r--r--   0 root         (0) root         (0)    20357 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/tuple.cuh
--rw-r--r--   0 root         (0) root         (0)     2919 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/include/cupy/type_dispatcher.cuh
--rw-r--r--   0 root         (0) root         (0)     1863 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/internal.pxd
--rw-r--r--   0 root         (0) root         (0)    13914 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/internal.pyx
--rw-r--r--   0 root         (0) root         (0)     6446 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/new_fusion.pyx
--rw-r--r--   0 root         (0) root         (0)      730 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/raw.pxd
--rw-r--r--   0 root         (0) root         (0)    22750 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/raw.pyx
--rw-r--r--   0 root         (0) root         (0)     1422 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_core/syncdetect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_creation/
--rw-r--r--   0 root         (0) root         (0)      116 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_creation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10475 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_creation/basic.py
--rw-r--r--   0 root         (0) root         (0)     5019 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_creation/from_data.py
--rw-r--r--   0 root         (0) root         (0)     3758 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_creation/matrix.py
--rw-r--r--   0 root         (0) root         (0)    14083 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_creation/ranges.py
--rw-r--r--   0 root         (0) root         (0)    11475 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_functional/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1997 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_functional/piecewise.py
--rw-r--r--   0 root         (0) root         (0)     3697 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_functional/vectorize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_indexing/
--rw-r--r--   0 root         (0) root         (0)      110 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_indexing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13669 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_indexing/generate.py
--rw-r--r--   0 root         (0) root         (0)     7132 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_indexing/indexing.py
--rw-r--r--   0 root         (0) root         (0)     7913 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_indexing/insert.py
--rw-r--r--   0 root         (0) root         (0)     4262 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_indexing/iterate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_io/
--rw-r--r--   0 root         (0) root         (0)      104 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1486 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_io/formatting.py
--rw-r--r--   0 root         (0) root         (0)     5136 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_io/npz.py
--rw-r--r--   0 root         (0) root         (0)      278 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_io/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_logic/
--rw-r--r--   0 root         (0) root         (0)      107 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_logic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4204 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_logic/comparison.py
--rw-r--r--   0 root         (0) root         (0)      880 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_logic/content.py
--rw-r--r--   0 root         (0) root         (0)     1057 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_logic/ops.py
--rw-r--r--   0 root         (0) root         (0)     4464 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_logic/truth.py
--rw-r--r--   0 root         (0) root         (0)     4562 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_logic/type_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_manipulation/
--rw-r--r--   0 root         (0) root         (0)      120 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6585 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/add_remove.py
--rw-r--r--   0 root         (0) root         (0)     2327 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/basic.py
--rw-r--r--   0 root         (0) root         (0)     4488 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/dims.py
--rw-r--r--   0 root         (0) root         (0)     3418 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/join.py
--rw-r--r--   0 root         (0) root         (0)     2639 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/kind.py
--rw-r--r--   0 root         (0) root         (0)     6226 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/rearrange.py
--rw-r--r--   0 root         (0) root         (0)     3404 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/shape.py
--rw-r--r--   0 root         (0) root         (0)     3017 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/split.py
--rw-r--r--   0 root         (0) root         (0)     2010 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/tiling.py
--rw-r--r--   0 root         (0) root         (0)     2323 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_manipulation/transpose.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_math/
--rw-r--r--   0 root         (0) root         (0)      106 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3149 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     1736 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/explog.py
--rw-r--r--   0 root         (0) root         (0)     1604 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/floating.py
--rw-r--r--   0 root         (0) root         (0)     1026 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/hyperbolic.py
--rw-r--r--   0 root         (0) root         (0)    13758 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/misc.py
--rw-r--r--   0 root         (0) root         (0)     1327 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/rational.py
--rw-r--r--   0 root         (0) root         (0)     1843 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/rounding.py
--rw-r--r--   0 root         (0) root         (0)      701 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/special.py
--rw-r--r--   0 root         (0) root         (0)    17478 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/sumprod.py
--rw-r--r--   0 root         (0) root         (0)     3231 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/trigonometric.py
--rw-r--r--   0 root         (0) root         (0)      577 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/ufunc.py
--rw-r--r--   0 root         (0) root         (0)     4814 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_math/window.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_misc/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1266 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_misc/memory_ranges.py
--rw-r--r--   0 root         (0) root         (0)     3358 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_misc/who.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_padding/
--rw-r--r--   0 root         (0) root         (0)      109 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_padding/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29422 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_padding/pad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_sorting/
--rw-r--r--   0 root         (0) root         (0)      106 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_sorting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1107 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_sorting/count.py
--rw-r--r--   0 root         (0) root         (0)    12917 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_sorting/search.py
--rw-r--r--   0 root         (0) root         (0)     6014 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_sorting/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/_statistics/
--rw-r--r--   0 root         (0) root         (0)      112 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_statistics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4601 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_statistics/correlation.py
--rw-r--r--   0 root         (0) root         (0)    21982 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_statistics/histogram.py
--rw-r--r--   0 root         (0) root         (0)    10202 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_statistics/meanvar.py
--rw-r--r--   0 root         (0) root         (0)    11821 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_statistics/order.py
--rw-r--r--   0 root         (0) root         (0)     5779 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_util.pyx
--rw-r--r--   0 root         (0) root         (0)       22 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/_version.py
--rw-r--r--   0 root         (0) root         (0)    26288 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cublas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/cuda/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)     6245 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      560 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/common.pxd
--rw-r--r--   0 root         (0) root         (0)     1587 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/common.pyx
--rw-r--r--   0 root         (0) root         (0)    31214 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/compiler.py
--rw-r--r--   0 root         (0) root         (0)      510 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cub.pxd
--rw-r--r--   0 root         (0) root         (0)    18465 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cub.pyx
--rw-r--r--   0 root         (0) root         (0)      297 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cudnn.py
--rw-r--r--   0 root         (0) root         (0)     2533 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cufft.pxd
--rw-r--r--   0 root         (0) root         (0)    44363 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cufft.pyx
--rw-r--r--   0 root         (0) root         (0)    31033 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_cub.cu
--rw-r--r--   0 root         (0) root         (0)     2559 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_cub.h
--rw-r--r--   0 root         (0) root         (0)     7941 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_cufft.h
--rw-r--r--   0 root         (0) root         (0)     2832 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_cufftXt.cu
--rw-r--r--   0 root         (0) root         (0)      190 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_cufftXt.h
--rw-r--r--   0 root         (0) root         (0)     1024 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_jitify.h
--rw-r--r--   0 root         (0) root         (0)    17156 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_thrust.cu
--rw-r--r--   0 root         (0) root         (0)      637 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cupy_thrust.h
--rw-r--r--   0 root         (0) root         (0)      309 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/cutensor.py
--rw-r--r--   0 root         (0) root         (0)      513 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/device.pxd
--rw-r--r--   0 root         (0) root         (0)     9678 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/device.pyx
--rw-r--r--   0 root         (0) root         (0)      857 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/function.pxd
--rw-r--r--   0 root         (0) root         (0)     8182 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/function.pyx
--rw-r--r--   0 root         (0) root         (0)     3633 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/jitify.pyx
--rw-r--r--   0 root         (0) root         (0)     2226 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory.pxd
--rw-r--r--   0 root         (0) root         (0)    62269 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory.pyx
--rw-r--r--   0 root         (0) root         (0)       56 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory_hook.pxd
--rw-r--r--   0 root         (0) root         (0)     6069 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory_hook.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/cuda/memory_hooks/
--rw-r--r--   0 root         (0) root         (0)      282 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory_hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2861 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory_hooks/debug_print.py
--rw-r--r--   0 root         (0) root         (0)     5992 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/memory_hooks/line_profile.py
--rw-r--r--   0 root         (0) root         (0)      293 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/nccl.py
--rw-r--r--   0 root         (0) root         (0)       51 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/nvtx.py
--rw-r--r--   0 root         (0) root         (0)      757 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/pinned_memory.pxd
--rw-r--r--   0 root         (0) root         (0)    10098 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/pinned_memory.pyx
--rw-r--r--   0 root         (0) root         (0)       55 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/profiler.py
--rw-r--r--   0 root         (0) root         (0)       53 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/runtime.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/stream.pxd
--rw-r--r--   0 root         (0) root         (0)    12064 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/stream.pyx
--rw-r--r--   0 root         (0) root         (0)     1271 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/texture.pxd
--rw-r--r--   0 root         (0) root         (0)    28856 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/texture.pyx
--rw-r--r--   0 root         (0) root         (0)     4576 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cuda/thrust.pyx
--rw-r--r--   0 root         (0) root         (0)   100532 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cudnn.pyx
--rw-r--r--   0 root         (0) root         (0)    29404 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cusolver.pyx
--rw-r--r--   0 root         (0) root         (0)    58069 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cusparse.py
--rw-r--r--   0 root         (0) root         (0)    29382 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/cutensor.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/fft/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/fft/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)      763 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/fft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22195 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/fft/_cache.pyx
--rw-r--r--   0 root         (0) root         (0)    23234 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/fft/_callback.pyx
--rw-r--r--   0 root         (0) root         (0)    41353 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/fft/_fft.py
--rw-r--r--   0 root         (0) root         (0)     1960 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/fft/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/lib/
--rw-r--r--   0 root         (0) root         (0)       43 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8511 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/lib/_polynomial.pyx
--rw-r--r--   0 root         (0) root         (0)    10867 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/lib/_routines_poly.py
--rw-r--r--   0 root         (0) root         (0)     2465 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/lib/_shape_base.py
--rw-r--r--   0 root         (0) root         (0)     1183 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/lib/stride_tricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/linalg/
--rw-r--r--   0 root         (0) root         (0)     1824 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19137 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_decomposition.py
--rw-r--r--   0 root         (0) root         (0)     5243 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_eigenvalue.py
--rw-r--r--   0 root         (0) root         (0)    22638 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_einsum.py
--rw-r--r--   0 root         (0) root         (0)    13566 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_einsum_opt.py
--rw-r--r--   0 root         (0) root         (0)    10472 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_norms.py
--rw-r--r--   0 root         (0) root         (0)    13242 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_product.py
--rw-r--r--   0 root         (0) root         (0)    16946 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_solve.py
--rw-r--r--   0 root         (0) root         (0)     5153 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/linalg/_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/polynomial/
--rw-r--r--   0 root         (0) root         (0)      243 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/polynomial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1299 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/polynomial/polynomial.py
--rw-r--r--   0 root         (0) root         (0)     3059 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/polynomial/polyutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/prof/
--rw-r--r--   0 root         (0) root         (0)      114 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/prof/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3565 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/prof/_time_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/random/
--rw-r--r--   0 root         (0) root         (0)     5112 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6658 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_bit_generator.pyx
--rw-r--r--   0 root         (0) root         (0)    32812 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_distributions.py
--rw-r--r--   0 root         (0) root         (0)    47615 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_generator.py
--rw-r--r--   0 root         (0) root         (0)    19509 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_generator_api.pyx
--rw-r--r--   0 root         (0) root         (0)    31073 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_kernels.py
--rw-r--r--   0 root         (0) root         (0)      716 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_permutations.py
--rw-r--r--   0 root         (0) root         (0)     7985 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/_sample.py
--rw-r--r--   0 root         (0) root         (0)    15005 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/cupy_distributions.cu
--rw-r--r--   0 root         (0) root         (0)     3139 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/random/cupy_distributions.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/sparse/
--rw-r--r--   0 root         (0) root         (0)      900 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/sparse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/sparse/linalg/
--rw-r--r--   0 root         (0) root         (0)      558 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/sparse/linalg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy/testing/
--rw-r--r--   0 root         (0) root         (0)     3010 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6258 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_array.py
--rw-r--r--   0 root         (0) root         (0)     1648 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_attr.py
--rw-r--r--   0 root         (0) root         (0)     1645 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_bundle.py
--rw-r--r--   0 root         (0) root         (0)     4270 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_condition.py
--rw-r--r--   0 root         (0) root         (0)    58118 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_helper.py
--rw-r--r--   0 root         (0) root         (0)     5954 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_hypothesis.py
--rw-r--r--   0 root         (0) root         (0)     3441 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_parameterized.py
--rw-r--r--   0 root         (0) root         (0)     1777 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_pytest_impl.py
--rw-r--r--   0 root         (0) root         (0)     4206 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy/testing/_random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2839 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34820 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      303 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy_backends/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/__init__.pxd
--rwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy_backends/cuda/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy_backends/cuda/api/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/api/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6232 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/api/driver.pxd
--rw-r--r--   0 root         (0) root         (0)    15313 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/api/driver.pyx
--rw-r--r--   0 root         (0) root         (0)    38292 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/api/runtime.pxd
--rw-r--r--   0 root         (0) root         (0)    40933 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/api/runtime.pyx
--rw-r--r--   0 root         (0) root         (0)      403 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cublas.h
--rw-r--r--   0 root         (0) root         (0)      173 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cuda.h
--rw-r--r--   0 root         (0) root         (0)      358 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cuda_runtime.h
--rw-r--r--   0 root         (0) root         (0)    11592 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cudnn.h
--rw-r--r--   0 root         (0) root         (0)     6053 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cusolver.h
--rw-r--r--   0 root         (0) root         (0)    17101 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cusparse.h
--rw-r--r--   0 root         (0) root         (0)      768 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_cusparselt.h
--rw-r--r--   0 root         (0) root         (0)      198 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_nccl.h
--rw-r--r--   0 root         (0) root         (0)      653 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/cupy_nvrtc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy_backends/cuda/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15979 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cublas.pxd
--rw-r--r--   0 root         (0) root         (0)    53109 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cublas.pyx
--rw-r--r--   0 root         (0) root         (0)    32131 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cudnn.pxd
--rw-r--r--   0 root         (0) root         (0)   106589 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cudnn.pyx
--rw-r--r--   0 root         (0) root         (0)     2154 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cugraph.pyx
--rw-r--r--   0 root         (0) root         (0)     1085 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/curand.pxd
--rw-r--r--   0 root         (0) root         (0)     7762 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/curand.pyx
--rw-r--r--   0 root         (0) root         (0)    40169 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cusolver.pxd
--rw-r--r--   0 root         (0) root         (0)   157185 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cusolver.pyx
--rw-r--r--   0 root         (0) root         (0)     5793 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cusparse.pxd
--rw-r--r--   0 root         (0) root         (0)   225346 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cusparse.pyx
--rw-r--r--   0 root         (0) root         (0)      866 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cusparselt.pxd
--rw-r--r--   0 root         (0) root         (0)    17991 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cusparselt.pyx
--rw-r--r--   0 root         (0) root         (0)     7045 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cutensor.pxd
--rw-r--r--   0 root         (0) root         (0)    34141 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/cutensor.pyx
--rw-r--r--   0 root         (0) root         (0)      477 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/nccl.pxd
--rw-r--r--   0 root         (0) root         (0)    17784 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/nccl.pyx
--rw-r--r--   0 root         (0) root         (0)      985 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/nvrtc.pxd
--rw-r--r--   0 root         (0) root         (0)     7326 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/nvrtc.pyx
--rw-r--r--   0 root         (0) root         (0)     6090 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/nvtx.pyx
--rw-r--r--   0 root         (0) root         (0)      218 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/profiler.pxd
--rw-r--r--   0 root         (0) root         (0)     1709 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/libs/profiler.pyx
--rwxr-xr-x   0 root         (0) root         (0)      184 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/stream.pxd
--rwxr-xr-x   0 root         (0) root         (0)     2351 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cuda/stream.pyx
--rw-r--r--   0 root         (0) root         (0)      308 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_backend.h
--rw-r--r--   0 root         (0) root         (0)      356 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_backend_runtime.h
--rw-r--r--   0 root         (0) root         (0)      322 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_blas.h
--rw-r--r--   0 root         (0) root         (0)      358 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_complex.h
--rw-r--r--   0 root         (0) root         (0)    11858 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_cudnn.h
--rw-r--r--   0 root         (0) root         (0)      685 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_cugraph.h
--rw-r--r--   0 root         (0) root         (0)      326 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_cusparselt.h
--rw-r--r--   0 root         (0) root         (0)      428 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_cutensor.h
--rw-r--r--   0 root         (0) root         (0)     2908 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_lapack.h
--rw-r--r--   0 root         (0) root         (0)     5128 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_nccl.h
--rw-r--r--   0 root         (0) root         (0)      332 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_profiler.h
--rw-r--r--   0 root         (0) root         (0)      312 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_rand.h
--rw-r--r--   0 root         (0) root         (0)      272 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_rtc.h
--rw-r--r--   0 root         (0) root         (0)      475 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_sparse.h
--rw-r--r--   0 root         (0) root         (0)      454 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/cupy_tx.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy_backends/hip/
--rw-r--r--   0 root         (0) root         (0)      424 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_cuComplex.h
--rw-r--r--   0 root         (0) root         (0)     3996 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_hip.h
--rw-r--r--   0 root         (0) root         (0)     4926 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_hip_common.h
--rw-r--r--   0 root         (0) root         (0)    10050 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_hip_runtime.h
--rw-r--r--   0 root         (0) root         (0)    42630 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_hipblas.h
--rw-r--r--   0 root         (0) root         (0)     3732 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_hiprand.h
--rw-r--r--   0 root         (0) root         (0)     2326 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_hiprtc.h
--rw-r--r--   0 root         (0) root         (0)      430 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_profiler.h
--rw-r--r--   0 root         (0) root         (0)      137 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_rccl.h
--rw-r--r--   0 root         (0) root         (0)    69921 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_rocsolver.h
--rw-r--r--   0 root         (0) root         (0)      740 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/hip/cupy_roctx.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupy_backends/stub/
--rw-r--r--   0 root         (0) root         (0)      490 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cuComplex.h
--rw-r--r--   0 root         (0) root         (0)     7195 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cublas.h
--rw-r--r--   0 root         (0) root         (0)     2549 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cuda.h
--rw-r--r--   0 root         (0) root         (0)     5605 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cuda_common.h
--rw-r--r--   0 root         (0) root         (0)     5773 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cuda_runtime.h
--rw-r--r--   0 root         (0) root         (0)    15056 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cudnn.h
--rw-r--r--   0 root         (0) root         (0)      960 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cugraph.h
--rw-r--r--   0 root         (0) root         (0)     1977 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_curand.h
--rw-r--r--   0 root         (0) root         (0)    22512 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cusolver.h
--rw-r--r--   0 root         (0) root         (0)    26413 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cusparse.h
--rw-r--r--   0 root         (0) root         (0)     2805 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cusparselt.h
--rw-r--r--   0 root         (0) root         (0)     2113 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_cutensor.h
--rw-r--r--   0 root         (0) root         (0)     1942 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_nccl.h
--rw-r--r--   0 root         (0) root         (0)     1309 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_nvrtc.h
--rw-r--r--   0 root         (0) root         (0)     1168 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_nvtx.h
--rw-r--r--   0 root         (0) root         (0)      484 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_backends/stub/cupy_profiler.h
--rw-r--r--   0 root         (0) root         (0)    43164 2021-09-29 17:55:54.000000 cupy-9.5.0/cupy_setup_build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/
--rw-r--r--   0 root         (0) root         (0)      923 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5100 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/_pinned_array.py
--rw-r--r--   0 root         (0) root         (0)      204 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/_rsqrt.py
--rw-r--r--   0 root         (0) root         (0)     9282 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/_runtime.py
--rw-r--r--   0 root         (0) root         (0)     5009 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/_scatter.py
--rw-r--r--   0 root         (0) root         (0)     3051 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/_ufunc_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/fallback_mode/
--rw-r--r--   0 root         (0) root         (0)      281 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/fallback_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20155 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/fallback_mode/fallback.py
--rw-r--r--   0 root         (0) root         (0)     2264 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/fallback_mode/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/jit/
--rw-r--r--   0 root         (0) root         (0)      500 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4058 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/_builtin_funcs.py
--rw-r--r--   0 root         (0) root         (0)    25657 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/_compile.py
--rw-r--r--   0 root         (0) root         (0)     4701 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/_cuda_typerules.py
--rw-r--r--   0 root         (0) root         (0)     3762 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/_cuda_types.py
--rw-r--r--   0 root         (0) root         (0)     5916 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/_interface.py
--rw-r--r--   0 root         (0) root         (0)     2056 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/jit/_internal_types.py
--rw-r--r--   0 root         (0) root         (0)    12219 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/lapack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/linalg/
--rw-r--r--   0 root         (0) root         (0)      121 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/linalg/__init__.py
--rw-r--r--   0 root         (0) root         (0)      883 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/linalg/_solve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/linalg/sparse/
--rw-r--r--   0 root         (0) root         (0)       91 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/linalg/sparse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1788 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/linalg/sparse/_solve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/optimizing/
--rw-r--r--   0 root         (0) root         (0)       56 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/optimizing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3545 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/optimizing/_optimize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/
--rw-r--r--   0 root         (0) root         (0)      867 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/fft/
--rw-r--r--   0 root         (0) root         (0)      248 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/fft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23827 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/fft/_fft.py
--rw-r--r--   0 root         (0) root         (0)     1407 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/fft/_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/fftpack/
--rw-r--r--   0 root         (0) root         (0)      460 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/fftpack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19420 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/fftpack/_fft.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/linalg/
--rw-r--r--   0 root         (0) root         (0)      204 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/linalg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11518 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/linalg/decomp_lu.py
--rw-r--r--   0 root         (0) root         (0)     3211 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/linalg/solve_triangular.py
--rw-r--r--   0 root         (0) root         (0)    18651 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/linalg/special_matrices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/ndimage/
--rw-r--r--   0 root         (0) root         (0)     4343 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/_filters_core.py
--rw-r--r--   0 root         (0) root         (0)    10302 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/_filters_generic.py
--rw-r--r--   0 root         (0) root         (0)    19643 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/_interp_kernels.py
--rw-r--r--   0 root         (0) root         (0)     2549 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/_spline_kernel_weights.py
--rw-r--r--   0 root         (0) root         (0)     8713 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/_spline_prefilter_core.py
--rw-r--r--   0 root         (0) root         (0)     5353 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/_util.py
--rw-r--r--   0 root         (0) root         (0)    55344 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/filters.py
--rw-r--r--   0 root         (0) root         (0)     9527 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/fourier.py
--rw-r--r--   0 root         (0) root         (0)    28769 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/interpolation.py
--rw-r--r--   0 root         (0) root         (0)    45338 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/measurements.py
--rw-r--r--   0 root         (0) root         (0)    43176 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/ndimage/morphology.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/signal/
--rw-r--r--   0 root         (0) root         (0)      741 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/signal/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10904 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/signal/_signaltools_core.py
--rw-r--r--   0 root         (0) root         (0)     1424 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/signal/bsplines.py
--rw-r--r--   0 root         (0) root         (0)    23641 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/signal/signaltools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/sparse/
--rw-r--r--   0 root         (0) root         (0)     1845 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23040 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/_index.py
--rw-r--r--   0 root         (0) root         (0)      440 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/_util.py
--rw-r--r--   0 root         (0) root         (0)    16329 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/base.py
--rw-r--r--   0 root         (0) root         (0)    30684 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/compressed.py
--rw-r--r--   0 root         (0) root         (0)    18942 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/construct.py
--rw-r--r--   0 root         (0) root         (0)    17879 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/coo.py
--rw-r--r--   0 root         (0) root         (0)    12055 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/csc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/sparse/csgraph/
--rw-r--r--   0 root         (0) root         (0)      191 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/csgraph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3822 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/csgraph/_traversal.py
--rw-r--r--   0 root         (0) root         (0)    41146 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/csr.py
--rw-r--r--   0 root         (0) root         (0)    13174 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/data.py
--rw-r--r--   0 root         (0) root         (0)     7254 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/dia.py
--rw-r--r--   0 root         (0) root         (0)     2472 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/extract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/
--rw-r--r--   0 root         (0) root         (0)     1084 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13295 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/_eigen.py
--rw-r--r--   0 root         (0) root         (0)    17234 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/_interface.py
--rw-r--r--   0 root         (0) root         (0)    11329 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/_iterative.py
--rw-r--r--   0 root         (0) root         (0)    24100 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/_lobpcg.py
--rw-r--r--   0 root         (0) root         (0)     4125 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/_norm.py
--rw-r--r--   0 root         (0) root         (0)    14695 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/linalg/_solve.py
--rw-r--r--   0 root         (0) root         (0)     3554 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/sparse/sputils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/special/
--rw-r--r--   0 root         (0) root         (0)     1227 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1271 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_bessel.py
--rw-r--r--   0 root         (0) root         (0)     2792 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_convex_analysis.py
--rw-r--r--   0 root         (0) root         (0)     4237 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_digamma.py
--rw-r--r--   0 root         (0) root         (0)     1277 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_erf.py
--rw-r--r--   0 root         (0) root         (0)      513 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_gamma.py
--rw-r--r--   0 root         (0) root         (0)      522 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_gammaln.py
--rw-r--r--   0 root         (0) root         (0)      598 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_polygamma.py
--rw-r--r--   0 root         (0) root         (0)      252 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_statistics.py
--rw-r--r--   0 root         (0) root         (0)     2921 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/special/_zeta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/scipy/stats/
--rw-r--r--   0 root         (0) root         (0)       60 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1950 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/scipy/stats/distributions.py
--rw-r--r--   0 root         (0) root         (0)     6547 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/cupyx/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/tools/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10974 2021-09-29 17:55:54.000000 cupy-9.5.0/cupyx/tools/install_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/docs/
--rw-r--r--   0 root         (0) root         (0)     3704 2021-09-29 17:55:54.000000 cupy-9.5.0/docs/LICENSE_THIRD_PARTY
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)     4457 2021-09-29 17:55:54.000000 cupy-9.5.0/docs/source/license.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/install/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/install/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27552 2021-09-29 17:55:54.000000 cupy-9.5.0/install/build.py
--rw-r--r--   0 root         (0) root         (0)      546 2021-09-29 17:55:54.000000 cupy-9.5.0/install/utils.py
--rw-r--r--   0 root         (0) root         (0)      748 2021-09-29 18:02:42.000000 cupy-9.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4845 2021-09-29 17:55:54.000000 cupy-9.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)      744 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/binary_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/binary_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1039 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/binary_tests/test_elementwise.py
--rw-r--r--   0 root         (0) root         (0)     1319 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/binary_tests/test_packing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/core_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5197 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/fusion_utils.py
--rw-r--r--   0 root         (0) root         (0)     9363 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_array.py
--rw-r--r--   0 root         (0) root         (0)     1541 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_example.py
--rw-r--r--   0 root         (0) root         (0)     4365 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_indexing.py
--rw-r--r--   0 root         (0) root         (0)     5578 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_kernel_cache.py
--rw-r--r--   0 root         (0) root         (0)    11350 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_misc.py
--rw-r--r--   0 root         (0) root         (0)     6429 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_optimization.py
--rw-r--r--   0 root         (0) root         (0)     6823 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_reduction.py
--rw-r--r--   0 root         (0) root         (0)    13249 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_routines.py
--rw-r--r--   0 root         (0) root         (0)    10119 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_ufunc.py
--rw-r--r--   0 root         (0) root         (0)     1970 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_array_function.py
--rw-r--r--   0 root         (0) root         (0)     2942 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_carray.py
--rw-r--r--   0 root         (0) root         (0)     2575 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_core.py
--rw-r--r--   0 root         (0) root         (0)     5987 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_cub_reduction.py
--rw-r--r--   0 root         (0) root         (0)     2807 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_dlpack.py
--rw-r--r--   0 root         (0) root         (0)     4150 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_elementwise.py
--rw-r--r--   0 root         (0) root         (0)     1596 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_flags.py
--rw-r--r--   0 root         (0) root         (0)     1305 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     7052 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_internal.py
--rw-r--r--   0 root         (0) root         (0)     1080 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_iter.py
--rw-r--r--   0 root         (0) root         (0)    19999 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray.py
--rw-r--r--   0 root         (0) root         (0)    25713 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_adv_indexing.py
--rw-r--r--   0 root         (0) root         (0)     5528 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_complex_ops.py
--rw-r--r--   0 root         (0) root         (0)      440 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_contiguity.py
--rw-r--r--   0 root         (0) root         (0)     1424 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_conversion.py
--rw-r--r--   0 root         (0) root         (0)    11293 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_copy_and_view.py
--rw-r--r--   0 root         (0) root         (0)    10782 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_cuda_array_interface.py
--rw-r--r--   0 root         (0) root         (0)    25050 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_elementwise_op.py
--rw-r--r--   0 root         (0) root         (0)     5172 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_get.py
--rw-r--r--   0 root         (0) root         (0)     8581 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_indexing.py
--rw-r--r--   0 root         (0) root         (0)     3527 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_math.py
--rw-r--r--   0 root         (0) root         (0)      465 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_owndata.py
--rw-r--r--   0 root         (0) root         (0)    19196 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_reduction.py
--rw-r--r--   0 root         (0) root         (0)    12170 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_scatter.py
--rw-r--r--   0 root         (0) root         (0)     3697 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_ufunc.py
--rw-r--r--   0 root         (0) root         (0)     3952 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_unary_op.py
--rw-r--r--   0 root         (0) root         (0)    46563 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_raw.py
--rw-r--r--   0 root         (0) root         (0)     5700 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_reduction.py
--rw-r--r--   0 root         (0) root         (0)     1427 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_scan.py
--rw-r--r--   0 root         (0) root         (0)      851 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_syncdetect.py
--rw-r--r--   0 root         (0) root         (0)    12653 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/core_tests/test_userkernel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/creation_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/creation_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16810 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/creation_tests/test_basic.py
--rw-r--r--   0 root         (0) root         (0)    24293 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/creation_tests/test_from_data.py
--rw-r--r--   0 root         (0) root         (0)     5162 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/creation_tests/test_matrix.py
--rw-r--r--   0 root         (0) root         (0)    13295 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/creation_tests/test_ranges.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1761 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_debug_print.py
--rw-r--r--   0 root         (0) root         (0)     1485 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_line_profile.py
--rw-r--r--   0 root         (0) root         (0)     4226 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_compiler.py
--rw-r--r--   0 root         (0) root         (0)      279 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cublas.py
--rw-r--r--   0 root         (0) root         (0)      374 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cudnn.py
--rw-r--r--   0 root         (0) root         (0)     8187 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cufft.py
--rw-r--r--   0 root         (0) root         (0)     1463 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_curand.py
--rw-r--r--   0 root         (0) root         (0)      281 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cusolver.py
--rw-r--r--   0 root         (0) root         (0)      285 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cusparse.py
--rw-r--r--   0 root         (0) root         (0)      353 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cutensor.py
--rw-r--r--   0 root         (0) root         (0)     6190 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_device.py
--rw-r--r--   0 root         (0) root         (0)     1310 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_driver.py
--rw-r--r--   0 root         (0) root         (0)    35944 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_memory.py
--rw-r--r--   0 root         (0) root         (0)     3348 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_memory_hook.py
--rw-r--r--   0 root         (0) root         (0)     3281 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_nccl.py
--rw-r--r--   0 root         (0) root         (0)      276 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_nvrtc.py
--rw-r--r--   0 root         (0) root         (0)      606 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_nvtx.py
--rw-r--r--   0 root         (0) root         (0)     3647 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_pinned_memory.py
--rw-r--r--   0 root         (0) root         (0)      910 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_profile.py
--rw-r--r--   0 root         (0) root         (0)      286 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_runtime.py
--rw-r--r--   0 root         (0) root         (0)     5749 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_stream.py
--rw-r--r--   0 root         (0) root         (0)    19118 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/cuda_tests/test_texture.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/fft_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/fft_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18440 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/fft_tests/test_cache.py
--rw-r--r--   0 root         (0) root         (0)    29413 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/fft_tests/test_callback.py
--rw-r--r--   0 root         (0) root         (0)    52212 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/fft_tests/test_fft.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/functional_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/functional_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4384 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/functional_tests/test_piecewise.py
--rw-r--r--   0 root         (0) root         (0)    18088 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/functional_tests/test_vectorize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/indexing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/indexing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9952 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/indexing_tests/test_generate.py
--rw-r--r--   0 root         (0) root         (0)    12861 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/indexing_tests/test_indexing.py
--rw-r--r--   0 root         (0) root         (0)    10296 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/indexing_tests/test_insert.py
--rw-r--r--   0 root         (0) root         (0)     4461 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/indexing_tests/test_iterate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/io_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/io_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1133 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/io_tests/test_base_n.py
--rw-r--r--   0 root         (0) root         (0)      505 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/io_tests/test_formatting.py
--rw-r--r--   0 root         (0) root         (0)     2479 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/io_tests/test_npz.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/io_tests/test_text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/lib_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/lib_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29213 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/lib_tests/test_polynomial.py
--rw-r--r--   0 root         (0) root         (0)     3076 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/lib_tests/test_shape_base.py
--rw-r--r--   0 root         (0) root         (0)     1535 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/lib_tests/test_strided_tricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12361 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/test_decomposition.py
--rw-r--r--   0 root         (0) root         (0)     5681 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/test_eigenvalue.py
--rw-r--r--   0 root         (0) root         (0)    19141 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/test_einsum.py
--rw-r--r--   0 root         (0) root         (0)     7092 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/test_norms.py
--rw-r--r--   0 root         (0) root         (0)    17288 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/test_product.py
--rw-r--r--   0 root         (0) root         (0)    11847 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/linalg_tests/test_solve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7774 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/test_comparison.py
--rw-r--r--   0 root         (0) root         (0)      835 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/test_content.py
--rw-r--r--   0 root         (0) root         (0)      895 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/test_ops.py
--rw-r--r--   0 root         (0) root         (0)     3487 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/test_truth.py
--rw-r--r--   0 root         (0) root         (0)     2493 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/logic_tests/test_type_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6870 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_add_remove.py
--rw-r--r--   0 root         (0) root         (0)     5111 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_basic.py
--rw-r--r--   0 root         (0) root         (0)    11670 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_dims.py
--rw-r--r--   0 root         (0) root         (0)    15026 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_join.py
--rw-r--r--   0 root         (0) root         (0)     3255 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_kind.py
--rw-r--r--   0 root         (0) root         (0)     8900 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_rearrange.py
--rw-r--r--   0 root         (0) root         (0)     6438 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_shape.py
--rw-r--r--   0 root         (0) root         (0)     3064 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)     3579 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_tiling.py
--rw-r--r--   0 root         (0) root         (0)     5684 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_transpose.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/math_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18103 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     1582 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_explog.py
--rw-r--r--   0 root         (0) root         (0)     2445 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_floating.py
--rw-r--r--   0 root         (0) root         (0)     1044 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_hyperbolic.py
--rw-r--r--   0 root         (0) root         (0)    11124 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_matmul.py
--rw-r--r--   0 root         (0) root         (0)    15622 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_misc.py
--rw-r--r--   0 root         (0) root         (0)     1279 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_rational.py
--rw-r--r--   0 root         (0) root         (0)     4943 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_rounding.py
--rw-r--r--   0 root         (0) root         (0)      728 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_special.py
--rw-r--r--   0 root         (0) root         (0)    37137 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_sumprod.py
--rw-r--r--   0 root         (0) root         (0)     2670 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_trigonometric.py
--rw-r--r--   0 root         (0) root         (0)      906 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/math_tests/test_window.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/misc_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/misc_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4730 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/misc_tests/test_memory_ranges.py
--rw-r--r--   0 root         (0) root         (0)     2271 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/misc_tests/test_who.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/padding_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/padding_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11536 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/padding_tests/test_pad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/polynomial_tests/
--rw-r--r--   0 root         (0) root         (0)     5036 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/polynomial_tests/test_polynomial.py
--rw-r--r--   0 root         (0) root         (0)     6169 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/polynomial_tests/test_polyutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/prof_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/prof_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3501 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/prof_tests/test_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/random_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7576 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/common_distributions.py
--rw-r--r--   0 root         (0) root         (0)     2202 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_bit_generator.py
--rw-r--r--   0 root         (0) root         (0)    32075 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_distributions.py
--rw-r--r--   0 root         (0) root         (0)    39103 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_generator.py
--rw-r--r--   0 root         (0) root         (0)     7818 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_generator_api.py
--rw-r--r--   0 root         (0) root         (0)       98 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_init.py
--rw-r--r--   0 root         (0) root         (0)     5681 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_permutations.py
--rw-r--r--   0 root         (0) root         (0)      444 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_random.py
--rw-r--r--   0 root         (0) root         (0)    10043 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/random_tests/test_sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/sorting_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/sorting_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2089 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/sorting_tests/test_count.py
--rw-r--r--   0 root         (0) root         (0)    26364 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/sorting_tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)    24284 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/sorting_tests/test_sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/statistics_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/statistics_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5831 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/statistics_tests/test_correlation.py
--rw-r--r--   0 root         (0) root         (0)    24002 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/statistics_tests/test_histogram.py
--rw-r--r--   0 root         (0) root         (0)    16002 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/statistics_tests/test_meanvar.py
--rw-r--r--   0 root         (0) root         (0)    16445 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/statistics_tests/test_order.py
--rw-r--r--   0 root         (0) root         (0)    18157 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_cublas.py
--rw-r--r--   0 root         (0) root         (0)    16446 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_cudnn.py
--rw-r--r--   0 root         (0) root         (0)    11471 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_cusolver.py
--rw-r--r--   0 root         (0) root         (0)    30425 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_cusparse.py
--rw-r--r--   0 root         (0) root         (0)    11389 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_cutensor.py
--rw-r--r--   0 root         (0) root         (0)     3854 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_init.py
--rw-r--r--   0 root         (0) root         (0)     1649 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_ndim.py
--rw-r--r--   0 root         (0) root         (0)     3763 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_numpy_interop.py
--rw-r--r--   0 root         (0) root         (0)     2929 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/test_type_routines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupy_tests/testing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/testing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3501 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/testing_tests/test_array.py
--rw-r--r--   0 root         (0) root         (0)     6116 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/testing_tests/test_condition.py
--rw-r--r--   0 root         (0) root         (0)    22164 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/testing_tests/test_helper.py
--rw-r--r--   0 root         (0) root         (0)     8035 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupy_tests/testing_tests/test_parameterized.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/fallback_mode_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/fallback_mode_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20564 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/fallback_mode_tests/test_fallback.py
--rw-r--r--   0 root         (0) root         (0)     5988 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/fallback_mode_tests/test_notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/jit_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/jit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5978 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/jit_tests/test_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/linalg_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/linalg_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/linalg_tests/sparse_tests/
--rw-r--r--   0 root         (0) root         (0)      154 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/linalg_tests/sparse_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2142 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/linalg_tests/sparse_tests/test_solve.py
--rw-r--r--   0 root         (0) root         (0)     2680 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/linalg_tests/test_solve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fft_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fft_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71797 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fft_tests/test_fft.py
--rw-r--r--   0 root         (0) root         (0)      548 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fft_tests/test_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fftpack_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fftpack_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31931 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/fftpack_tests/test_fftpack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4996 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_decomp_lu.py
--rw-r--r--   0 root         (0) root         (0)     3429 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_solve_triangular.py
--rw-r--r--   0 root         (0) root         (0)     4547 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_special_matrices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28755 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_filters.py
--rw-r--r--   0 root         (0) root         (0)    15105 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_fourier.py
--rw-r--r--   0 root         (0) root         (0)    35973 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_interpolation.py
--rw-r--r--   0 root         (0) root         (0)    17677 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_measurements.py
--rw-r--r--   0 root         (0) root         (0)    22561 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_morphology.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/signal_tests/
--rw-r--r--   0 root         (0) root         (0)      998 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/signal_tests/test_bsplines.py
--rw-r--r--   0 root         (0) root         (0)    12944 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/signal_tests/test_signaltools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/
--rw-r--r--   0 root         (0) root         (0)      154 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/csgraph_tests/
--rw-r--r--   0 root         (0) root         (0)     2144 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/csgraph_tests/test_traversal.py
--rw-r--r--   0 root         (0) root         (0)     2174 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_base.py
--rw-r--r--   0 root         (0) root         (0)    13149 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_construct.py
--rw-r--r--   0 root         (0) root         (0)    37864 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_coo.py
--rw-r--r--   0 root         (0) root         (0)    49302 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csc.py
--rw-r--r--   0 root         (0) root         (0)    72383 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csr.py
--rw-r--r--   0 root         (0) root         (0)    11331 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_dia.py
--rw-r--r--   0 root         (0) root         (0)     2748 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_extract.py
--rw-r--r--   0 root         (0) root         (0)    18940 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_index.py
--rw-r--r--   0 root         (0) root         (0)    50029 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_linalg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1568 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_bessel.py
--rw-r--r--   0 root         (0) root         (0)     2103 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_convex_analysis.py
--rw-r--r--   0 root         (0) root         (0)     1863 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_digamma.py
--rw-r--r--   0 root         (0) root         (0)     4572 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_erf.py
--rw-r--r--   0 root         (0) root         (0)     1370 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_gamma.py
--rw-r--r--   0 root         (0) root         (0)     1380 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_gammaln.py
--rw-r--r--   0 root         (0) root         (0)     2000 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_polygamma.py
--rw-r--r--   0 root         (0) root         (0)     1016 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1605 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_zeta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/stats_tests/
--rw-r--r--   0 root         (0) root         (0)     4908 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/stats_tests/test_distributions.py
--rw-r--r--   0 root         (0) root         (0)      891 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/scipy_tests/test_get_array_module.py
--rw-r--r--   0 root         (0) root         (0)      637 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_cupyx.py
--rw-r--r--   0 root         (0) root         (0)     5936 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_lapack.py
--rw-r--r--   0 root         (0) root         (0)     8299 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_optimize.py
--rw-r--r--   0 root         (0) root         (0)    14926 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_pinned_array.py
--rw-r--r--   0 root         (0) root         (0)      467 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_rsqrt.py
--rw-r--r--   0 root         (0) root         (0)     1485 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_runtime.py
--rw-r--r--   0 root         (0) root         (0)     1238 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_scatter.py
--rw-r--r--   0 root         (0) root         (0)     5318 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/test_time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/cupyx_tests/tools_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/tools_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1929 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/cupyx_tests/tools_tests/test_install_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/example_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/example_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      490 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/example_tests/example_test.py
--rw-r--r--   0 root         (0) root         (0)     2138 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/example_tests/test_finance.py
--rw-r--r--   0 root         (0) root         (0)      170 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/example_tests/test_gemm.py
--rw-r--r--   0 root         (0) root         (0)     1066 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/example_tests/test_gmm.py
--rw-r--r--   0 root         (0) root         (0)     1190 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/example_tests/test_kmeans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-29 18:02:42.000000 cupy-9.5.0/tests/install_tests/
--rw-r--r--   0 root         (0) root         (0)      359 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/install_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1708 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/install_tests/test_build.py
--rw-r--r--   0 root         (0) root         (0)      362 2021-09-29 17:55:54.000000 cupy-9.5.0/tests/install_tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1118 2021-11-10 04:01:46.000000 cupy-9.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      531 2021-11-10 04:01:46.000000 cupy-9.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2914 2021-11-10 04:08:13.000000 cupy-9.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4921 2021-11-10 04:01:46.000000 cupy-9.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/
+-rw-r--r--   0 root         (0) root         (0)    31992 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_binary/
+-rw-r--r--   0 root         (0) root         (0)      109 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_binary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      242 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_binary/elementwise.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_binary/packing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)     3795 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_accelerator.pxd
+-rw-r--r--   0 root         (0) root         (0)     1148 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_accelerator.pyx
+-rw-r--r--   0 root         (0) root         (0)     1092 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_carray.pxd
+-rw-r--r--   0 root         (0) root         (0)     1654 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_carray.pyx
+-rw-r--r--   0 root         (0) root         (0)      966 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_codeblock.py
+-rw-r--r--   0 root         (0) root         (0)      431 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_cub_reduction.pxd
+-rw-r--r--   0 root         (0) root         (0)    25442 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_cub_reduction.pyx
+-rw-r--r--   0 root         (0) root         (0)      123 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_dtype.pxd
+-rw-r--r--   0 root         (0) root         (0)     2185 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_dtype.pyx
+-rw-r--r--   0 root         (0) root         (0)     8073 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_interface.py
+-rw-r--r--   0 root         (0) root         (0)    13473 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_kernel.pyx
+-rw-r--r--   0 root         (0) root         (0)    11191 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_op.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     1163 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_thread_local.pyx
+-rw-r--r--   0 root         (0) root         (0)    22671 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_trace.pyx
+-rw-r--r--   0 root         (0) root         (0)       95 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_variable.pxd
+-rw-r--r--   0 root         (0) root         (0)    10759 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_fusion_variable.pyx
+-rw-r--r--   0 root         (0) root         (0)    21037 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_gufuncs.py
+-rw-r--r--   0 root         (0) root         (0)     4243 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_kernel.pxd
+-rw-r--r--   0 root         (0) root         (0)    47100 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_kernel.pyx
+-rw-r--r--   0 root         (0) root         (0)      180 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_memory_range.pxd
+-rw-r--r--   0 root         (0) root         (0)     1108 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_memory_range.pyx
+-rw-r--r--   0 root         (0) root         (0)      511 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_optimize_config.pxd
+-rw-r--r--   0 root         (0) root         (0)     2172 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_optimize_config.pyx
+-rw-r--r--   0 root         (0) root         (0)     2146 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_reduction.pxd
+-rw-r--r--   0 root         (0) root         (0)    30390 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_reduction.pyx
+-rw-r--r--   0 root         (0) root         (0)      143 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_binary.pxd
+-rw-r--r--   0 root         (0) root         (0)     2226 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_binary.pyx
+-rw-r--r--   0 root         (0) root         (0)      774 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_indexing.pxd
+-rw-r--r--   0 root         (0) root         (0)    34532 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_indexing.pyx
+-rw-r--r--   0 root         (0) root         (0)      879 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_linalg.pxd
+-rw-r--r--   0 root         (0) root         (0)    31721 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_linalg.pyx
+-rw-r--r--   0 root         (0) root         (0)      473 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_logic.pxd
+-rw-r--r--   0 root         (0) root         (0)     3334 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_logic.pyx
+-rw-r--r--   0 root         (0) root         (0)     1434 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_manipulation.pxd
+-rw-r--r--   0 root         (0) root         (0)    24624 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_manipulation.pyx
+-rw-r--r--   0 root         (0) root         (0)     1191 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_math.pxd
+-rw-r--r--   0 root         (0) root         (0)    37704 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_math.pyx
+-rw-r--r--   0 root         (0) root         (0)      237 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_sorting.pxd
+-rw-r--r--   0 root         (0) root         (0)    11478 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_sorting.pyx
+-rw-r--r--   0 root         (0) root         (0)     1048 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_statistics.pxd
+-rw-r--r--   0 root         (0) root         (0)    24980 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_routines_statistics.pyx
+-rw-r--r--   0 root         (0) root         (0)      720 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_scalar.pxd
+-rw-r--r--   0 root         (0) root         (0)     9948 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_scalar.pyx
+-rw-r--r--   0 root         (0) root         (0)      283 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/_ufuncs.py
+-rw-r--r--   0 root         (0) root         (0)     4884 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/core.pxd
+-rw-r--r--   0 root         (0) root         (0)    87404 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/core.pyx
+-rw-r--r--   0 root         (0) root         (0)      135 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/dlpack.pxd
+-rw-r--r--   0 root         (0) root         (0)    10120 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/dlpack.pyx
+-rw-r--r--   0 root         (0) root         (0)      950 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/flags.pyx
+-rw-r--r--   0 root         (0) root         (0)    35369 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/fusion.pyx
+-rw-r--r--   0 root         (0) root         (0)     4523 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/halffloat.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/
+-rw-r--r--   0 root         (0) root         (0)      968 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/
+-rw-r--r--   0 root         (0) root         (0)      406 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.0/
+-rwxr-xr-x   0 root         (0) root         (0)    88634 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.h
+-rwxr-xr-x   0 root         (0) root         (0)    72855 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.1/
+-rwxr-xr-x   0 root         (0) root         (0)   109152 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.h
+-rwxr-xr-x   0 root         (0) root         (0)    73059 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.2/
+-rwxr-xr-x   0 root         (0) root         (0)   109689 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.h
+-rwxr-xr-x   0 root         (0) root         (0)    73401 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11/
+-rw-r--r--   0 root         (0) root         (0)   129685 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11/cuda_fp16.h
+-rw-r--r--   0 root         (0) root         (0)    91190 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11/cuda_fp16.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.0/
+-rwxr-xr-x   0 root         (0) root         (0)   125376 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.h
+-rwxr-xr-x   0 root         (0) root         (0)    81098 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.1/
+-rwxr-xr-x   0 root         (0) root         (0)   126227 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.h
+-rwxr-xr-x   0 root         (0) root         (0)    86543 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-9.2/
+-rw-r--r--   0 root         (0) root         (0)    70901 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.h
+-rw-r--r--   0 root         (0) root         (0)    72507 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.hpp
+-rw-r--r--   0 root         (0) root         (0)     3539 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/atomics.cuh
+-rw-r--r--   0 root         (0) root         (0)    17630 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/carray.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/
+-rw-r--r--   0 root         (0) root         (0)       92 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/README.md
+-rw-r--r--   0 root         (0) root         (0)     9577 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/arithmetic.h
+-rw-r--r--   0 root         (0) root         (0)    24176 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/catrig.h
+-rw-r--r--   0 root         (0) root         (0)    14169 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/catrigf.h
+-rw-r--r--   0 root         (0) root         (0)     7149 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/ccosh.h
+-rw-r--r--   0 root         (0) root         (0)     4554 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/ccoshf.h
+-rw-r--r--   0 root         (0) root         (0)     5764 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/cexp.h
+-rw-r--r--   0 root         (0) root         (0)     4954 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/cexpf.h
+-rw-r--r--   0 root         (0) root         (0)     5921 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/clog.h
+-rw-r--r--   0 root         (0) root         (0)     5455 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/clogf.h
+-rw-r--r--   0 root         (0) root         (0)    20245 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/complex.h
+-rw-r--r--   0 root         (0) root         (0)     4393 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/complex_inl.h
+-rw-r--r--   0 root         (0) root         (0)     1550 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/cpow.h
+-rw-r--r--   0 root         (0) root         (0)     1841 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/cproj.h
+-rw-r--r--   0 root         (0) root         (0)     6689 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/csinh.h
+-rw-r--r--   0 root         (0) root         (0)     4500 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/csinhf.h
+-rw-r--r--   0 root         (0) root         (0)     4554 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/csqrt.h
+-rw-r--r--   0 root         (0) root         (0)     4459 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/csqrtf.h
+-rw-r--r--   0 root         (0) root         (0)     6089 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/ctanh.h
+-rw-r--r--   0 root         (0) root         (0)     3739 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/ctanhf.h
+-rw-r--r--   0 root         (0) root         (0)     4299 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex/math_private.h
+-rw-r--r--   0 root         (0) root         (0)     2141 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/complex.cuh
+-rw-r--r--   0 root         (0) root         (0)     1518 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/cuComplex_bridge.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/
+-rw-r--r--   0 root         (0) root         (0)    22309 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/CHANGE_LOG.TXT
+-rw-r--r--   0 root         (0) root         (0)     1600 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/LICENSE.TXT
+-rw-r--r--   0 root         (0) root         (0)     6051 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/README.md
+-rw-r--r--   0 root         (0) root         (0)     7688 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/common.mk
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/
+-rw-r--r--   0 root         (0) root         (0)    33331 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    28525 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_downsweep.cuh
+-rw-r--r--   0 root         (0) root         (0)    17917 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_upsweep.cuh
+-rw-r--r--   0 root         (0) root         (0)    16916 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    24791 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce_by_key.cuh
+-rw-r--r--   0 root         (0) root         (0)    35663 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_rle.cuh
+-rw-r--r--   0 root         (0) root         (0)    18729 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    16655 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_segment_fixup.cuh
+-rw-r--r--   0 root         (0) root         (0)    29594 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_select_if.cuh
+-rw-r--r--   0 root         (0) root         (0)    27377 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_spmv_orig.cuh
+-rw-r--r--   0 root         (0) root         (0)    27444 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/single_pass_scan_operators.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/
+-rw-r--r--   0 root         (0) root         (0)    25011 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_adjacent_difference.cuh
+-rw-r--r--   0 root         (0) root         (0)    54550 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_discontinuity.cuh
+-rw-r--r--   0 root         (0) root         (0)    52305 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_exchange.cuh
+-rw-r--r--   0 root         (0) root         (0)    16291 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    53671 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_load.cuh
+-rw-r--r--   0 root         (0) root         (0)    25230 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_radix_rank.cuh
+-rw-r--r--   0 root         (0) root         (0)    38342 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)     6181 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_raking_layout.cuh
+-rw-r--r--   0 root         (0) root         (0)    25300 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)   102978 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    11964 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_shuffle.cuh
+-rw-r--r--   0 root         (0) root         (0)    41449 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_store.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/
+-rw-r--r--   0 root         (0) root         (0)     3285 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_atomic.cuh
+-rw-r--r--   0 root         (0) root         (0)     8198 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)     9731 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking.cuh
+-rw-r--r--   0 root         (0) root         (0)     8369 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking_commutative_only.cuh
+-rw-r--r--   0 root         (0) root         (0)     9769 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_warp_reductions.cuh
+-rw-r--r--   0 root         (0) root         (0)    28460 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_raking.cuh
+-rw-r--r--   0 root         (0) root         (0)    19117 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans.cuh
+-rw-r--r--   0 root         (0) root         (0)    20949 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans2.cuh
+-rw-r--r--   0 root         (0) root         (0)    19463 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans3.cuh
+-rw-r--r--   0 root         (0) root         (0)     3626 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/cub.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/
+-rw-r--r--   0 root         (0) root         (0)    54347 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    13891 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_partition.cuh
+-rw-r--r--   0 root         (0) root         (0)    42384 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)    38904 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    14817 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_run_length_encode.cuh
+-rw-r--r--   0 root         (0) root         (0)    21786 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    54689 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)    36523 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    18838 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_select.cuh
+-rw-r--r--   0 root         (0) root         (0)     8523 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_spmv.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/
+-rw-r--r--   0 root         (0) root         (0)    57226 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    80406 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)    42707 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    25478 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce_by_key.cuh
+-rw-r--r--   0 root         (0) root         (0)    23601 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_rle.cuh
+-rw-r--r--   0 root         (0) root         (0)    22778 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    24454 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_select_if.cuh
+-rw-r--r--   0 root         (0) root         (0)    33269 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_spmv_orig.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/
+-rw-r--r--   0 root         (0) root         (0)     5861 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_barrier.cuh
+-rw-r--r--   0 root         (0) root         (0)     8198 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_even_share.cuh
+-rw-r--r--   0 root         (0) root         (0)     4827 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_mapping.cuh
+-rw-r--r--   0 root         (0) root         (0)     7475 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_queue.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/host/
+-rw-r--r--   0 root         (0) root         (0)     4581 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/host/mutex.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/
+-rw-r--r--   0 root         (0) root         (0)     8781 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/arg_index_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     8104 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     8322 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_output_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     7650 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/constant_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     7369 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/counting_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     6817 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/discard_output_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)    10546 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/tex_obj_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)    12430 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/tex_ref_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     8611 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/transform_input_iterator.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/
+-rw-r--r--   0 root         (0) root         (0)    18869 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_load.cuh
+-rw-r--r--   0 root         (0) root         (0)     9228 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_operators.cuh
+-rw-r--r--   0 root         (0) root         (0)     6037 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    10566 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)     4797 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_search.cuh
+-rw-r--r--   0 root         (0) root         (0)    17932 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_store.cuh
+-rw-r--r--   0 root         (0) root         (0)    28716 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_allocator.cuh
+-rw-r--r--   0 root         (0) root         (0)     6955 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_arch.cuh
+-rw-r--r--   0 root         (0) root         (0)     5061 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_debug.cuh
+-rw-r--r--   0 root         (0) root         (0)    10658 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_device.cuh
+-rw-r--r--   0 root         (0) root         (0)     3710 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_macro.cuh
+-rw-r--r--   0 root         (0) root         (0)     2100 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_namespace.cuh
+-rw-r--r--   0 root         (0) root         (0)    22318 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_ptx.cuh
+-rw-r--r--   0 root         (0) root         (0)    40178 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_type.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/
+-rw-r--r--   0 root         (0) root         (0)    21412 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_shfl.cuh
+-rw-r--r--   0 root         (0) root         (0)    14280 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_smem.cuh
+-rw-r--r--   0 root         (0) root         (0)    25284 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_shfl.cuh
+-rw-r--r--   0 root         (0) root         (0)    16153 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_smem.cuh
+-rw-r--r--   0 root         (0) root         (0)    25032 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/warp_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    38915 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/warp_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    16543 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/eclipse code style profile.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/
+-rw-r--r--   0 root         (0) root         (0)     5255 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/Makefile
+-rw-r--r--   0 root         (0) root         (0)    10724 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)     9644 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    11329 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-r--r--   0 root         (0) root         (0)     1554 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/
+-rw-r--r--   0 root         (0) root         (0)     8830 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/Makefile
+-rw-r--r--   0 root         (0) root         (0)     8173 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-r--r--   0 root         (0) root         (0)     8236 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-r--r--   0 root         (0) root         (0)     8303 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)     5825 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)     6007 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-r--r--   0 root         (0) root         (0)     8156 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-r--r--   0 root         (0) root         (0)     8210 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-r--r--   0 root         (0) root         (0)     7493 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-r--r--   0 root         (0) root         (0)    13277 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/
+-rw-r--r--   0 root         (0) root         (0)     4949 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-r--r--   0 root         (0) root         (0)    37185 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-r--r--   0 root         (0) root         (0)    95317 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/
+-rw-r--r--   0 root         (0) root         (0)     4374 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_cub.h
+-rw-r--r--   0 root         (0) root         (0)     6368 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_gmem_atomics.h
+-rw-r--r--   0 root         (0) root         (0)     6812 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_smem_atomics.h
+-rw-r--r--   0 root         (0) root         (0)    21778 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-r--r--   0 root         (0) root         (0)    39231 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/sparse_matrix.h
+-rw-r--r--   0 root         (0) root         (0)    30656 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+-rwxr-xr-x   0 root         (0) root         (0)      749 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/spmv_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/
+-rw-r--r--   0 root         (0) root         (0)    18927 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/Makefile
+-rw-r--r--   0 root         (0) root         (0)     8397 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/half.h
+-rw-r--r--   0 root         (0) root         (0)      315 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-r--r--   0 root         (0) root         (0)      315 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-r--r--   0 root         (0) root         (0)     5148 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/mersenne.h
+-rw-r--r--   0 root         (0) root         (0)    16564 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-r--r--   0 root         (0) root         (0)     9623 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-r--r--   0 root         (0) root         (0)    19496 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-r--r--   0 root         (0) root         (0)    25392 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)    26628 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    34810 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-r--r--   0 root         (0) root         (0)    70313 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-r--r--   0 root         (0) root         (0)    46469 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)    49902 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    30363 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-r--r--   0 root         (0) root         (0)    31192 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-r--r--   0 root         (0) root         (0)    33600 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-r--r--   0 root         (0) root         (0)    37640 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-r--r--   0 root         (0) root         (0)    21518 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-r--r--   0 root         (0) root         (0)     5132 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-r--r--   0 root         (0) root         (0)    25549 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-r--r--   0 root         (0) root         (0)    54847 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_util.h
+-rw-r--r--   0 root         (0) root         (0)    27186 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    20350 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/tune/
+-rw-r--r--   0 root         (0) root         (0)     6388 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/tune/Makefile
+-rw-r--r--   0 root         (0) root         (0)    27663 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/dlpack/
+-rw-r--r--   0 root         (0) root         (0)      232 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/dlpack/README.md
+-rw-r--r--   0 root         (0) root         (0)     5308 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/dlpack/dlpack.h
+-rw-r--r--   0 root         (0) root         (0)      623 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/hip_workaround.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/
+-rw-r--r--   0 root         (0) root         (0)   106196 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/Doxyfile
+-rw-r--r--   0 root         (0) root         (0)     1523 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2901 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3346 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/
+-rw-r--r--   0 root         (0) root         (0)     2302 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/class_arg_kernel.cuh
+-rw-r--r--   0 root         (0) root         (0)     1827 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/constant_header.cuh
+-rw-r--r--   0 root         (0) root         (0)     1651 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/my_header1.cuh
+-rw-r--r--   0 root         (0) root         (0)     1630 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/my_header2.cuh
+-rw-r--r--   0 root         (0) root         (0)     1631 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/my_header3.cuh
+-rw-r--r--   0 root         (0) root         (0)   160071 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/jitify.hpp
+-rw-r--r--   0 root         (0) root         (0)    41241 2021-11-10 04:01:49.000000 cupy-9.6.0/cupy/_core/include/cupy/jitify/jitify_test.cu
+-rw-r--r--   0 root         (0) root         (0)      655 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/math_constants.h
+-rw-r--r--   0 root         (0) root         (0)      986 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/swap.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_core/include/cupy/tuple/
+-rw-r--r--   0 root         (0) root         (0)    29357 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/tuple/tuple.h
+-rw-r--r--   0 root         (0) root         (0)     1457 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/tuple/type_traits.h
+-rw-r--r--   0 root         (0) root         (0)    20357 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/tuple.cuh
+-rw-r--r--   0 root         (0) root         (0)     2919 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/include/cupy/type_dispatcher.cuh
+-rw-r--r--   0 root         (0) root         (0)     1863 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/internal.pxd
+-rw-r--r--   0 root         (0) root         (0)    13990 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/internal.pyx
+-rw-r--r--   0 root         (0) root         (0)     6446 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/new_fusion.pyx
+-rw-r--r--   0 root         (0) root         (0)      730 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/raw.pxd
+-rw-r--r--   0 root         (0) root         (0)    22750 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/raw.pyx
+-rw-r--r--   0 root         (0) root         (0)     1422 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_core/syncdetect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_creation/
+-rw-r--r--   0 root         (0) root         (0)      116 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_creation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10475 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_creation/basic.py
+-rw-r--r--   0 root         (0) root         (0)     5019 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_creation/from_data.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_creation/matrix.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_creation/ranges.py
+-rw-r--r--   0 root         (0) root         (0)    11475 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_functional/piecewise.py
+-rw-r--r--   0 root         (0) root         (0)     3697 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_functional/vectorize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_indexing/
+-rw-r--r--   0 root         (0) root         (0)      110 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_indexing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13669 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_indexing/generate.py
+-rw-r--r--   0 root         (0) root         (0)     7132 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_indexing/indexing.py
+-rw-r--r--   0 root         (0) root         (0)     7913 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_indexing/insert.py
+-rw-r--r--   0 root         (0) root         (0)     4262 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_indexing/iterate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_io/
+-rw-r--r--   0 root         (0) root         (0)      104 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_io/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     5136 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_io/npz.py
+-rw-r--r--   0 root         (0) root         (0)      278 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_io/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_logic/
+-rw-r--r--   0 root         (0) root         (0)      107 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_logic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_logic/comparison.py
+-rw-r--r--   0 root         (0) root         (0)      880 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_logic/content.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_logic/ops.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_logic/truth.py
+-rw-r--r--   0 root         (0) root         (0)     4562 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_logic/type_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_manipulation/
+-rw-r--r--   0 root         (0) root         (0)      120 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6585 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/add_remove.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/basic.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/dims.py
+-rw-r--r--   0 root         (0) root         (0)     3418 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/join.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/kind.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/rearrange.py
+-rw-r--r--   0 root         (0) root         (0)     3404 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/shape.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/split.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/tiling.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_manipulation/transpose.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_math/
+-rw-r--r--   0 root         (0) root         (0)      106 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3149 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/explog.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/floating.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/hyperbolic.py
+-rw-r--r--   0 root         (0) root         (0)    13758 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/misc.py
+-rw-r--r--   0 root         (0) root         (0)     1327 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/rational.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/rounding.py
+-rw-r--r--   0 root         (0) root         (0)      701 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/special.py
+-rw-r--r--   0 root         (0) root         (0)    17478 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/sumprod.py
+-rw-r--r--   0 root         (0) root         (0)     3231 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/trigonometric.py
+-rw-r--r--   0 root         (0) root         (0)      577 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/ufunc.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_math/window.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_misc/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_misc/memory_ranges.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_misc/who.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_padding/
+-rw-r--r--   0 root         (0) root         (0)      109 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_padding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29422 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_padding/pad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_sorting/
+-rw-r--r--   0 root         (0) root         (0)      106 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_sorting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_sorting/count.py
+-rw-r--r--   0 root         (0) root         (0)    12917 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_sorting/search.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_sorting/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/_statistics/
+-rw-r--r--   0 root         (0) root         (0)      112 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_statistics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4601 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_statistics/correlation.py
+-rw-r--r--   0 root         (0) root         (0)    21982 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_statistics/histogram.py
+-rw-r--r--   0 root         (0) root         (0)    10202 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_statistics/meanvar.py
+-rw-r--r--   0 root         (0) root         (0)    11821 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_statistics/order.py
+-rw-r--r--   0 root         (0) root         (0)     5779 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_util.pyx
+-rw-r--r--   0 root         (0) root         (0)       22 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/_version.py
+-rw-r--r--   0 root         (0) root         (0)    26288 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cublas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/cuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)     6245 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      560 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/common.pxd
+-rw-r--r--   0 root         (0) root         (0)     1587 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/common.pyx
+-rw-r--r--   0 root         (0) root         (0)    31252 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/compiler.py
+-rw-r--r--   0 root         (0) root         (0)      510 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cub.pxd
+-rw-r--r--   0 root         (0) root         (0)    18465 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cub.pyx
+-rw-r--r--   0 root         (0) root         (0)      297 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cudnn.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cufft.pxd
+-rw-r--r--   0 root         (0) root         (0)    44363 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cufft.pyx
+-rw-r--r--   0 root         (0) root         (0)    31033 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_cub.cu
+-rw-r--r--   0 root         (0) root         (0)     2559 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_cub.h
+-rw-r--r--   0 root         (0) root         (0)     7941 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_cufft.h
+-rw-r--r--   0 root         (0) root         (0)     2832 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_cufftXt.cu
+-rw-r--r--   0 root         (0) root         (0)      190 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_cufftXt.h
+-rw-r--r--   0 root         (0) root         (0)     1024 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_jitify.h
+-rw-r--r--   0 root         (0) root         (0)    17156 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_thrust.cu
+-rw-r--r--   0 root         (0) root         (0)      637 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cupy_thrust.h
+-rw-r--r--   0 root         (0) root         (0)      309 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/cutensor.py
+-rw-r--r--   0 root         (0) root         (0)      513 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/device.pxd
+-rw-r--r--   0 root         (0) root         (0)     9678 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/device.pyx
+-rw-r--r--   0 root         (0) root         (0)      857 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/function.pxd
+-rw-r--r--   0 root         (0) root         (0)     8182 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/function.pyx
+-rw-r--r--   0 root         (0) root         (0)     3633 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/jitify.pyx
+-rw-r--r--   0 root         (0) root         (0)     2226 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory.pxd
+-rw-r--r--   0 root         (0) root         (0)    62269 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory.pyx
+-rw-r--r--   0 root         (0) root         (0)       56 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory_hook.pxd
+-rw-r--r--   0 root         (0) root         (0)     6069 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory_hook.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/cuda/memory_hooks/
+-rw-r--r--   0 root         (0) root         (0)      282 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory_hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory_hooks/debug_print.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/memory_hooks/line_profile.py
+-rw-r--r--   0 root         (0) root         (0)      293 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/nccl.py
+-rw-r--r--   0 root         (0) root         (0)       51 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/nvtx.py
+-rw-r--r--   0 root         (0) root         (0)      757 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/pinned_memory.pxd
+-rw-r--r--   0 root         (0) root         (0)    10098 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/pinned_memory.pyx
+-rw-r--r--   0 root         (0) root         (0)       55 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/profiler.py
+-rw-r--r--   0 root         (0) root         (0)       53 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/runtime.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/stream.pxd
+-rw-r--r--   0 root         (0) root         (0)    12064 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/stream.pyx
+-rw-r--r--   0 root         (0) root         (0)     1271 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/texture.pxd
+-rw-r--r--   0 root         (0) root         (0)    28856 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/texture.pyx
+-rw-r--r--   0 root         (0) root         (0)     4576 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cuda/thrust.pyx
+-rw-r--r--   0 root         (0) root         (0)   100532 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cudnn.pyx
+-rw-r--r--   0 root         (0) root         (0)    29404 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cusolver.pyx
+-rw-r--r--   0 root         (0) root         (0)    58069 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cusparse.py
+-rw-r--r--   0 root         (0) root         (0)    29470 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/cutensor.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/fft/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/fft/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)      763 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/fft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22195 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/fft/_cache.pyx
+-rw-r--r--   0 root         (0) root         (0)    23234 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/fft/_callback.pyx
+-rw-r--r--   0 root         (0) root         (0)    41353 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/fft/_fft.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/fft/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/lib/
+-rw-r--r--   0 root         (0) root         (0)       43 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8511 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/lib/_polynomial.pyx
+-rw-r--r--   0 root         (0) root         (0)    10867 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/lib/_routines_poly.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/lib/_shape_base.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/lib/stride_tricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/linalg/
+-rw-r--r--   0 root         (0) root         (0)     1824 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19167 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_decomposition.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_eigenvalue.py
+-rw-r--r--   0 root         (0) root         (0)    22681 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_einsum.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_einsum_opt.py
+-rw-r--r--   0 root         (0) root         (0)    10472 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_norms.py
+-rw-r--r--   0 root         (0) root         (0)    13242 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_product.py
+-rw-r--r--   0 root         (0) root         (0)    16946 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_solve.py
+-rw-r--r--   0 root         (0) root         (0)     5153 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/linalg/_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/polynomial/
+-rw-r--r--   0 root         (0) root         (0)      243 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/polynomial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/polynomial/polynomial.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/polynomial/polyutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/prof/
+-rw-r--r--   0 root         (0) root         (0)      114 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/prof/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/prof/_time_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/random/
+-rw-r--r--   0 root         (0) root         (0)     5112 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6658 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_bit_generator.pyx
+-rw-r--r--   0 root         (0) root         (0)    32812 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_distributions.py
+-rw-r--r--   0 root         (0) root         (0)    44197 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_generator.py
+-rw-r--r--   0 root         (0) root         (0)    19509 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_generator_api.pyx
+-rw-r--r--   0 root         (0) root         (0)    31073 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_kernels.py
+-rw-r--r--   0 root         (0) root         (0)      716 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_permutations.py
+-rw-r--r--   0 root         (0) root         (0)     7985 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15005 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/cupy_distributions.cu
+-rw-r--r--   0 root         (0) root         (0)     3139 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/random/cupy_distributions.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/sparse/
+-rw-r--r--   0 root         (0) root         (0)      900 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/sparse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/sparse/linalg/
+-rw-r--r--   0 root         (0) root         (0)      558 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/sparse/linalg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy/testing/
+-rw-r--r--   0 root         (0) root         (0)     3010 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6258 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_array.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_attr.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_bundle.py
+-rw-r--r--   0 root         (0) root         (0)     4270 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_condition.py
+-rw-r--r--   0 root         (0) root         (0)    58118 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_helper.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_hypothesis.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_parameterized.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_pytest_impl.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy/testing/_random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2914 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34604 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      303 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2021-11-10 04:08:12.000000 cupy-9.6.0/cupy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy_backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/__init__.pxd
+-rwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy_backends/cuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy_backends/cuda/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/api/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/api/driver.pxd
+-rw-r--r--   0 root         (0) root         (0)    15313 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/api/driver.pyx
+-rw-r--r--   0 root         (0) root         (0)    38292 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/api/runtime.pxd
+-rw-r--r--   0 root         (0) root         (0)    40933 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/api/runtime.pyx
+-rw-r--r--   0 root         (0) root         (0)      403 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cublas.h
+-rw-r--r--   0 root         (0) root         (0)      173 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cuda.h
+-rw-r--r--   0 root         (0) root         (0)      358 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cuda_runtime.h
+-rw-r--r--   0 root         (0) root         (0)    11592 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cudnn.h
+-rw-r--r--   0 root         (0) root         (0)     6053 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cusolver.h
+-rw-r--r--   0 root         (0) root         (0)    17101 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cusparse.h
+-rw-r--r--   0 root         (0) root         (0)      768 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_cusparselt.h
+-rw-r--r--   0 root         (0) root         (0)      198 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_nccl.h
+-rw-r--r--   0 root         (0) root         (0)      653 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/cupy_nvrtc.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy_backends/cuda/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15979 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cublas.pxd
+-rw-r--r--   0 root         (0) root         (0)    53109 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cublas.pyx
+-rw-r--r--   0 root         (0) root         (0)    32131 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cudnn.pxd
+-rw-r--r--   0 root         (0) root         (0)   106589 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cudnn.pyx
+-rw-r--r--   0 root         (0) root         (0)     2154 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cugraph.pyx
+-rw-r--r--   0 root         (0) root         (0)     1085 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/curand.pxd
+-rw-r--r--   0 root         (0) root         (0)     7762 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/curand.pyx
+-rw-r--r--   0 root         (0) root         (0)    40169 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cusolver.pxd
+-rw-r--r--   0 root         (0) root         (0)   157185 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cusolver.pyx
+-rw-r--r--   0 root         (0) root         (0)     5793 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cusparse.pxd
+-rw-r--r--   0 root         (0) root         (0)   225346 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cusparse.pyx
+-rw-r--r--   0 root         (0) root         (0)      866 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cusparselt.pxd
+-rw-r--r--   0 root         (0) root         (0)    17991 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cusparselt.pyx
+-rw-r--r--   0 root         (0) root         (0)     7045 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cutensor.pxd
+-rw-r--r--   0 root         (0) root         (0)    34141 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/cutensor.pyx
+-rw-r--r--   0 root         (0) root         (0)      477 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/nccl.pxd
+-rw-r--r--   0 root         (0) root         (0)    17784 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/nccl.pyx
+-rw-r--r--   0 root         (0) root         (0)      985 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/nvrtc.pxd
+-rw-r--r--   0 root         (0) root         (0)     7326 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/nvrtc.pyx
+-rw-r--r--   0 root         (0) root         (0)     6090 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/nvtx.pyx
+-rw-r--r--   0 root         (0) root         (0)      218 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/profiler.pxd
+-rw-r--r--   0 root         (0) root         (0)     1709 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/libs/profiler.pyx
+-rwxr-xr-x   0 root         (0) root         (0)      184 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/stream.pxd
+-rwxr-xr-x   0 root         (0) root         (0)     2351 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cuda/stream.pyx
+-rw-r--r--   0 root         (0) root         (0)      308 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_backend.h
+-rw-r--r--   0 root         (0) root         (0)      356 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_backend_runtime.h
+-rw-r--r--   0 root         (0) root         (0)      322 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_blas.h
+-rw-r--r--   0 root         (0) root         (0)      358 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_complex.h
+-rw-r--r--   0 root         (0) root         (0)    11858 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_cudnn.h
+-rw-r--r--   0 root         (0) root         (0)      685 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_cugraph.h
+-rw-r--r--   0 root         (0) root         (0)      326 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_cusparselt.h
+-rw-r--r--   0 root         (0) root         (0)      428 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_cutensor.h
+-rw-r--r--   0 root         (0) root         (0)     2908 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_lapack.h
+-rw-r--r--   0 root         (0) root         (0)     5128 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_nccl.h
+-rw-r--r--   0 root         (0) root         (0)      332 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_profiler.h
+-rw-r--r--   0 root         (0) root         (0)      312 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_rand.h
+-rw-r--r--   0 root         (0) root         (0)      272 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_rtc.h
+-rw-r--r--   0 root         (0) root         (0)      475 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_sparse.h
+-rw-r--r--   0 root         (0) root         (0)      454 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/cupy_tx.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy_backends/hip/
+-rw-r--r--   0 root         (0) root         (0)      424 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_cuComplex.h
+-rw-r--r--   0 root         (0) root         (0)     3996 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_hip.h
+-rw-r--r--   0 root         (0) root         (0)     4926 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_hip_common.h
+-rw-r--r--   0 root         (0) root         (0)    10050 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_hip_runtime.h
+-rw-r--r--   0 root         (0) root         (0)    42630 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_hipblas.h
+-rw-r--r--   0 root         (0) root         (0)     3732 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_hiprand.h
+-rw-r--r--   0 root         (0) root         (0)     2326 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_hiprtc.h
+-rw-r--r--   0 root         (0) root         (0)      430 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_profiler.h
+-rw-r--r--   0 root         (0) root         (0)      137 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_rccl.h
+-rw-r--r--   0 root         (0) root         (0)    69921 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_rocsolver.h
+-rw-r--r--   0 root         (0) root         (0)      740 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/hip/cupy_roctx.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupy_backends/stub/
+-rw-r--r--   0 root         (0) root         (0)      490 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cuComplex.h
+-rw-r--r--   0 root         (0) root         (0)     7195 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cublas.h
+-rw-r--r--   0 root         (0) root         (0)     2549 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cuda.h
+-rw-r--r--   0 root         (0) root         (0)     5605 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cuda_common.h
+-rw-r--r--   0 root         (0) root         (0)     5773 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cuda_runtime.h
+-rw-r--r--   0 root         (0) root         (0)    15056 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cudnn.h
+-rw-r--r--   0 root         (0) root         (0)      960 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cugraph.h
+-rw-r--r--   0 root         (0) root         (0)     1977 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_curand.h
+-rw-r--r--   0 root         (0) root         (0)    22512 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cusolver.h
+-rw-r--r--   0 root         (0) root         (0)    26413 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cusparse.h
+-rw-r--r--   0 root         (0) root         (0)     2805 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cusparselt.h
+-rw-r--r--   0 root         (0) root         (0)     2113 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_cutensor.h
+-rw-r--r--   0 root         (0) root         (0)     1942 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_nccl.h
+-rw-r--r--   0 root         (0) root         (0)     1309 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_nvrtc.h
+-rw-r--r--   0 root         (0) root         (0)     1168 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_nvtx.h
+-rw-r--r--   0 root         (0) root         (0)      484 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_backends/stub/cupy_profiler.h
+-rw-r--r--   0 root         (0) root         (0)    43164 2021-11-10 04:01:46.000000 cupy-9.6.0/cupy_setup_build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/
+-rw-r--r--   0 root         (0) root         (0)      923 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5100 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/_pinned_array.py
+-rw-r--r--   0 root         (0) root         (0)      204 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/_rsqrt.py
+-rw-r--r--   0 root         (0) root         (0)     9527 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/_runtime.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/_scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/_ufunc_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/fallback_mode/
+-rw-r--r--   0 root         (0) root         (0)      281 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/fallback_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20155 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/fallback_mode/fallback.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/fallback_mode/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/jit/
+-rw-r--r--   0 root         (0) root         (0)      500 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/_builtin_funcs.py
+-rw-r--r--   0 root         (0) root         (0)    25657 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/_compile.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/_cuda_typerules.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/_cuda_types.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/_interface.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/jit/_internal_types.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/lapack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/linalg/
+-rw-r--r--   0 root         (0) root         (0)      121 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/linalg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      883 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/linalg/_solve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/linalg/sparse/
+-rw-r--r--   0 root         (0) root         (0)       91 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/linalg/sparse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/linalg/sparse/_solve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/optimizing/
+-rw-r--r--   0 root         (0) root         (0)       56 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/optimizing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/optimizing/_optimize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/
+-rw-r--r--   0 root         (0) root         (0)      867 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/fft/
+-rw-r--r--   0 root         (0) root         (0)      248 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/fft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23827 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/fft/_fft.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/fft/_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/fftpack/
+-rw-r--r--   0 root         (0) root         (0)      460 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/fftpack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19420 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/fftpack/_fft.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/linalg/
+-rw-r--r--   0 root         (0) root         (0)      204 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/linalg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11518 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/linalg/decomp_lu.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/linalg/solve_triangular.py
+-rw-r--r--   0 root         (0) root         (0)    18651 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/linalg/special_matrices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/ndimage/
+-rw-r--r--   0 root         (0) root         (0)     4343 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/_filters_core.py
+-rw-r--r--   0 root         (0) root         (0)    10302 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/_filters_generic.py
+-rw-r--r--   0 root         (0) root         (0)    19643 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/_interp_kernels.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/_spline_kernel_weights.py
+-rw-r--r--   0 root         (0) root         (0)     8713 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/_spline_prefilter_core.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/_util.py
+-rw-r--r--   0 root         (0) root         (0)    55344 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/filters.py
+-rw-r--r--   0 root         (0) root         (0)     9527 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/fourier.py
+-rw-r--r--   0 root         (0) root         (0)    28769 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/interpolation.py
+-rw-r--r--   0 root         (0) root         (0)    45338 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/measurements.py
+-rw-r--r--   0 root         (0) root         (0)    43176 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/ndimage/morphology.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/signal/
+-rw-r--r--   0 root         (0) root         (0)      741 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/signal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10904 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/signal/_signaltools_core.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/signal/bsplines.py
+-rw-r--r--   0 root         (0) root         (0)    23641 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/signal/signaltools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/sparse/
+-rw-r--r--   0 root         (0) root         (0)     1845 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23040 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/_index.py
+-rw-r--r--   0 root         (0) root         (0)      440 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/_util.py
+-rw-r--r--   0 root         (0) root         (0)    16329 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/base.py
+-rw-r--r--   0 root         (0) root         (0)    30684 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/compressed.py
+-rw-r--r--   0 root         (0) root         (0)    18942 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/construct.py
+-rw-r--r--   0 root         (0) root         (0)    17879 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/coo.py
+-rw-r--r--   0 root         (0) root         (0)    12055 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/csc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/sparse/csgraph/
+-rw-r--r--   0 root         (0) root         (0)      191 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/csgraph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/csgraph/_traversal.py
+-rw-r--r--   0 root         (0) root         (0)    41146 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/csr.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/data.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/dia.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/extract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/
+-rw-r--r--   0 root         (0) root         (0)     1084 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13295 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/_eigen.py
+-rw-r--r--   0 root         (0) root         (0)    17234 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/_interface.py
+-rw-r--r--   0 root         (0) root         (0)    11329 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/_iterative.py
+-rw-r--r--   0 root         (0) root         (0)    24100 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/_lobpcg.py
+-rw-r--r--   0 root         (0) root         (0)     4125 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/_norm.py
+-rw-r--r--   0 root         (0) root         (0)    14695 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/linalg/_solve.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/sparse/sputils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/special/
+-rw-r--r--   0 root         (0) root         (0)     1227 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_bessel.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_convex_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     4237 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_digamma.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_erf.py
+-rw-r--r--   0 root         (0) root         (0)      513 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_gamma.py
+-rw-r--r--   0 root         (0) root         (0)      522 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_gammaln.py
+-rw-r--r--   0 root         (0) root         (0)      598 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_polygamma.py
+-rw-r--r--   0 root         (0) root         (0)      252 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/special/_zeta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/scipy/stats/
+-rw-r--r--   0 root         (0) root         (0)       60 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/scipy/stats/distributions.py
+-rw-r--r--   0 root         (0) root         (0)     6547 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/cupyx/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/tools/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13285 2021-11-10 04:01:46.000000 cupy-9.6.0/cupyx/tools/install_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     3704 2021-11-10 04:01:46.000000 cupy-9.6.0/docs/LICENSE_THIRD_PARTY
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)     4457 2021-11-10 04:01:46.000000 cupy-9.6.0/docs/source/license.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/install/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27552 2021-11-10 04:01:46.000000 cupy-9.6.0/install/build.py
+-rw-r--r--   0 root         (0) root         (0)      546 2021-11-10 04:01:46.000000 cupy-9.6.0/install/utils.py
+-rw-r--r--   0 root         (0) root         (0)      748 2021-11-10 04:08:13.000000 cupy-9.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4845 2021-11-10 04:01:46.000000 cupy-9.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      744 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/binary_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/binary_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/binary_tests/test_elementwise.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/binary_tests/test_packing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/core_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5197 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/fusion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9363 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_array.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_example.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_indexing.py
+-rw-r--r--   0 root         (0) root         (0)     5578 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_kernel_cache.py
+-rw-r--r--   0 root         (0) root         (0)    11350 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_misc.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_reduction.py
+-rw-r--r--   0 root         (0) root         (0)    13249 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_routines.py
+-rw-r--r--   0 root         (0) root         (0)    10119 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_ufunc.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_array_function.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_carray.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_core.py
+-rw-r--r--   0 root         (0) root         (0)     5987 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_cub_reduction.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_dlpack.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_elementwise.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_flags.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_internal.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_iter.py
+-rw-r--r--   0 root         (0) root         (0)    19999 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray.py
+-rw-r--r--   0 root         (0) root         (0)    25713 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_adv_indexing.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_complex_ops.py
+-rw-r--r--   0 root         (0) root         (0)      440 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_contiguity.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_conversion.py
+-rw-r--r--   0 root         (0) root         (0)    11293 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_copy_and_view.py
+-rw-r--r--   0 root         (0) root         (0)    10782 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_cuda_array_interface.py
+-rw-r--r--   0 root         (0) root         (0)    25050 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_elementwise_op.py
+-rw-r--r--   0 root         (0) root         (0)     5172 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_get.py
+-rw-r--r--   0 root         (0) root         (0)     8581 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_indexing.py
+-rw-r--r--   0 root         (0) root         (0)     3527 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_math.py
+-rw-r--r--   0 root         (0) root         (0)      465 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_owndata.py
+-rw-r--r--   0 root         (0) root         (0)    19196 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_reduction.py
+-rw-r--r--   0 root         (0) root         (0)    12170 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3697 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_ufunc.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_unary_op.py
+-rw-r--r--   0 root         (0) root         (0)    46563 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_raw.py
+-rw-r--r--   0 root         (0) root         (0)     5700 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_reduction.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_scan.py
+-rw-r--r--   0 root         (0) root         (0)      851 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_syncdetect.py
+-rw-r--r--   0 root         (0) root         (0)    12653 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/core_tests/test_userkernel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/creation_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/creation_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16810 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/creation_tests/test_basic.py
+-rw-r--r--   0 root         (0) root         (0)    24293 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/creation_tests/test_from_data.py
+-rw-r--r--   0 root         (0) root         (0)     5162 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/creation_tests/test_matrix.py
+-rw-r--r--   0 root         (0) root         (0)    13295 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/creation_tests/test_ranges.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_debug_print.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_line_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_compiler.py
+-rw-r--r--   0 root         (0) root         (0)      279 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cublas.py
+-rw-r--r--   0 root         (0) root         (0)      374 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cudnn.py
+-rw-r--r--   0 root         (0) root         (0)     8187 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cufft.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_curand.py
+-rw-r--r--   0 root         (0) root         (0)      281 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cusolver.py
+-rw-r--r--   0 root         (0) root         (0)      285 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cusparse.py
+-rw-r--r--   0 root         (0) root         (0)      353 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cutensor.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_device.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_driver.py
+-rw-r--r--   0 root         (0) root         (0)    35944 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_memory_hook.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_nccl.py
+-rw-r--r--   0 root         (0) root         (0)      276 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_nvrtc.py
+-rw-r--r--   0 root         (0) root         (0)      606 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_nvtx.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_pinned_memory.py
+-rw-r--r--   0 root         (0) root         (0)      910 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_profile.py
+-rw-r--r--   0 root         (0) root         (0)      286 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_runtime.py
+-rw-r--r--   0 root         (0) root         (0)     5749 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_stream.py
+-rw-r--r--   0 root         (0) root         (0)    19118 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/cuda_tests/test_texture.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/fft_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/fft_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18440 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/fft_tests/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)    29413 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/fft_tests/test_callback.py
+-rw-r--r--   0 root         (0) root         (0)    52289 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/fft_tests/test_fft.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/functional_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/functional_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4384 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/functional_tests/test_piecewise.py
+-rw-r--r--   0 root         (0) root         (0)    18088 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/functional_tests/test_vectorize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/indexing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/indexing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/indexing_tests/test_generate.py
+-rw-r--r--   0 root         (0) root         (0)    12861 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/indexing_tests/test_indexing.py
+-rw-r--r--   0 root         (0) root         (0)    10296 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/indexing_tests/test_insert.py
+-rw-r--r--   0 root         (0) root         (0)     4461 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/indexing_tests/test_iterate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/io_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/io_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/io_tests/test_base_n.py
+-rw-r--r--   0 root         (0) root         (0)      505 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/io_tests/test_formatting.py
+-rw-r--r--   0 root         (0) root         (0)     2479 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/io_tests/test_npz.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/io_tests/test_text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/lib_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/lib_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29213 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/lib_tests/test_polynomial.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/lib_tests/test_shape_base.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/lib_tests/test_strided_tricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12361 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/test_decomposition.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/test_eigenvalue.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/test_einsum.py
+-rw-r--r--   0 root         (0) root         (0)     7092 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/test_norms.py
+-rw-r--r--   0 root         (0) root         (0)    17288 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/test_product.py
+-rw-r--r--   0 root         (0) root         (0)    11847 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/linalg_tests/test_solve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7774 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/test_comparison.py
+-rw-r--r--   0 root         (0) root         (0)      835 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/test_content.py
+-rw-r--r--   0 root         (0) root         (0)      895 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/test_ops.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/test_truth.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/logic_tests/test_type_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6870 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_add_remove.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_basic.py
+-rw-r--r--   0 root         (0) root         (0)    11670 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_dims.py
+-rw-r--r--   0 root         (0) root         (0)    15026 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_join.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_kind.py
+-rw-r--r--   0 root         (0) root         (0)     8900 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_rearrange.py
+-rw-r--r--   0 root         (0) root         (0)     7072 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_shape.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_tiling.py
+-rw-r--r--   0 root         (0) root         (0)     5684 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_transpose.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/math_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18103 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_explog.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_floating.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_hyperbolic.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_matmul.py
+-rw-r--r--   0 root         (0) root         (0)    15622 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_misc.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_rational.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_rounding.py
+-rw-r--r--   0 root         (0) root         (0)      728 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_special.py
+-rw-r--r--   0 root         (0) root         (0)    37137 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_sumprod.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_trigonometric.py
+-rw-r--r--   0 root         (0) root         (0)      906 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/math_tests/test_window.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/misc_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/misc_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/misc_tests/test_memory_ranges.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/misc_tests/test_who.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/padding_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/padding_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11536 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/padding_tests/test_pad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/polynomial_tests/
+-rw-r--r--   0 root         (0) root         (0)     5036 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/polynomial_tests/test_polynomial.py
+-rw-r--r--   0 root         (0) root         (0)     6169 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/polynomial_tests/test_polyutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/prof_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/prof_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/prof_tests/test_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/random_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/common_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_bit_generator.py
+-rw-r--r--   0 root         (0) root         (0)    32075 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_distributions.py
+-rw-r--r--   0 root         (0) root         (0)    39103 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_generator.py
+-rw-r--r--   0 root         (0) root         (0)     7818 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_generator_api.py
+-rw-r--r--   0 root         (0) root         (0)       98 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_permutations.py
+-rw-r--r--   0 root         (0) root         (0)      444 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_random.py
+-rw-r--r--   0 root         (0) root         (0)    10043 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/random_tests/test_sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/sorting_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/sorting_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/sorting_tests/test_count.py
+-rw-r--r--   0 root         (0) root         (0)    26364 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/sorting_tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)    24284 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/sorting_tests/test_sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/statistics_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/statistics_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5831 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/statistics_tests/test_correlation.py
+-rw-r--r--   0 root         (0) root         (0)    24002 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/statistics_tests/test_histogram.py
+-rw-r--r--   0 root         (0) root         (0)    16002 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/statistics_tests/test_meanvar.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/statistics_tests/test_order.py
+-rw-r--r--   0 root         (0) root         (0)    18157 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_cublas.py
+-rw-r--r--   0 root         (0) root         (0)    16446 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_cudnn.py
+-rw-r--r--   0 root         (0) root         (0)    11471 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_cusolver.py
+-rw-r--r--   0 root         (0) root         (0)    30425 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_cusparse.py
+-rw-r--r--   0 root         (0) root         (0)    12008 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_cutensor.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_ndim.py
+-rw-r--r--   0 root         (0) root         (0)     3763 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_numpy_interop.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/test_type_routines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupy_tests/testing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/testing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/testing_tests/test_array.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/testing_tests/test_condition.py
+-rw-r--r--   0 root         (0) root         (0)    22164 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/testing_tests/test_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8035 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupy_tests/testing_tests/test_parameterized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/fallback_mode_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/fallback_mode_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20564 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/fallback_mode_tests/test_fallback.py
+-rw-r--r--   0 root         (0) root         (0)     5988 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/fallback_mode_tests/test_notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/jit_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/jit_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/jit_tests/test_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/linalg_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/linalg_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/linalg_tests/sparse_tests/
+-rw-r--r--   0 root         (0) root         (0)      154 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/linalg_tests/sparse_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/linalg_tests/sparse_tests/test_solve.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/linalg_tests/test_solve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fft_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fft_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71797 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fft_tests/test_fft.py
+-rw-r--r--   0 root         (0) root         (0)      548 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fft_tests/test_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fftpack_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fftpack_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31931 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/fftpack_tests/test_fftpack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_decomp_lu.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_solve_triangular.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_special_matrices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28755 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_filters.py
+-rw-r--r--   0 root         (0) root         (0)    15105 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_fourier.py
+-rw-r--r--   0 root         (0) root         (0)    35973 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_interpolation.py
+-rw-r--r--   0 root         (0) root         (0)    17677 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_measurements.py
+-rw-r--r--   0 root         (0) root         (0)    22561 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_morphology.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/signal_tests/
+-rw-r--r--   0 root         (0) root         (0)      998 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/signal_tests/test_bsplines.py
+-rw-r--r--   0 root         (0) root         (0)    12944 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/signal_tests/test_signaltools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/
+-rw-r--r--   0 root         (0) root         (0)      154 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/csgraph_tests/
+-rw-r--r--   0 root         (0) root         (0)     2144 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/csgraph_tests/test_traversal.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_base.py
+-rw-r--r--   0 root         (0) root         (0)    13149 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_construct.py
+-rw-r--r--   0 root         (0) root         (0)    37864 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_coo.py
+-rw-r--r--   0 root         (0) root         (0)    49302 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csc.py
+-rw-r--r--   0 root         (0) root         (0)    72383 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csr.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_dia.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_extract.py
+-rw-r--r--   0 root         (0) root         (0)    18940 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_index.py
+-rw-r--r--   0 root         (0) root         (0)    50029 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_linalg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_bessel.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_convex_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_digamma.py
+-rw-r--r--   0 root         (0) root         (0)     4572 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_erf.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_gammaln.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_polygamma.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_zeta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/stats_tests/
+-rw-r--r--   0 root         (0) root         (0)     4908 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/stats_tests/test_distributions.py
+-rw-r--r--   0 root         (0) root         (0)      891 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/scipy_tests/test_get_array_module.py
+-rw-r--r--   0 root         (0) root         (0)      637 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_cupyx.py
+-rw-r--r--   0 root         (0) root         (0)     5936 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_lapack.py
+-rw-r--r--   0 root         (0) root         (0)     8299 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_optimize.py
+-rw-r--r--   0 root         (0) root         (0)    14926 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_pinned_array.py
+-rw-r--r--   0 root         (0) root         (0)      467 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_rsqrt.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_runtime.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_scatter.py
+-rw-r--r--   0 root         (0) root         (0)     5318 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/cupyx_tests/tools_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/tools_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/cupyx_tests/tools_tests/test_install_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/example_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/example_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      490 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/example_tests/example_test.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/example_tests/test_finance.py
+-rw-r--r--   0 root         (0) root         (0)      170 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/example_tests/test_gemm.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/example_tests/test_gmm.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/example_tests/test_kmeans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-10 04:08:13.000000 cupy-9.6.0/tests/install_tests/
+-rw-r--r--   0 root         (0) root         (0)      359 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/install_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/install_tests/test_build.py
+-rw-r--r--   0 root         (0) root         (0)      362 2021-11-10 04:01:46.000000 cupy-9.6.0/tests/install_tests/test_utils.py
```

### Comparing `cupy-9.5.0/LICENSE` & `cupy-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/MANIFEST.in` & `cupy-9.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/PKG-INFO` & `cupy-9.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupy
-Version: 9.5.0
+Version: 9.6.0
 Summary: CuPy: NumPy & SciPy for GPU
 Home-page: https://cupy.dev/
 Author: Seiya Tokui
 Author-email: tokui@preferred.jp
 Maintainer: CuPy Developers
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/cupy/cupy/issues
@@ -42,14 +42,15 @@
 ============================
 
 `CuPy <https://cupy.dev/>`_ is a NumPy/SciPy-compatible array library for GPU-accelerated computing with Python.
 
 This package (``cupy``) is a source distribution.
 For most users, use of pre-build wheel distributions are recommended:
 
+- `cupy-cuda115 <https://pypi.org/project/cupy-cuda115/>`_ (for CUDA 11.5)
 - `cupy-cuda114 <https://pypi.org/project/cupy-cuda114/>`_ (for CUDA 11.4)
 - `cupy-cuda113 <https://pypi.org/project/cupy-cuda113/>`_ (for CUDA 11.3)
 - `cupy-cuda112 <https://pypi.org/project/cupy-cuda112/>`_ (for CUDA 11.2)
 - `cupy-cuda111 <https://pypi.org/project/cupy-cuda111/>`_ (for CUDA 11.1)
 - `cupy-cuda110 <https://pypi.org/project/cupy-cuda110/>`_ (for CUDA 11.0)
 - `cupy-cuda102 <https://pypi.org/project/cupy-cuda102/>`_ (for CUDA 10.2)
 - `cupy-cuda101 <https://pypi.org/project/cupy-cuda101/>`_ (for CUDA 10.1)
```

### Comparing `cupy-9.5.0/README.md` & `cupy-9.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 | CUDA 10.1     | `pip install cupy-cuda101`    |
 | CUDA 10.2     | `pip install cupy-cuda102`    |
 | CUDA 11.0     | `pip install cupy-cuda110`    |
 | CUDA 11.1     | `pip install cupy-cuda111`    |
 | CUDA 11.2     | `pip install cupy-cuda112`    |
 | CUDA 11.3     | `pip install cupy-cuda113`    |
 | CUDA 11.4     | `pip install cupy-cuda114`    |
+| CUDA 11.5     | `pip install cupy-cuda115`    |
 | ROCm 4.0 (*)  | `pip install cupy-rocm-4-0`   |
 | ROCm 4.2 (*)  | `pip install cupy-rocm-4-2`   |
 | ROCm 4.3 (*)  | `pip install cupy-rocm-4-3`   |
 
 (\*) ROCm support is an experimental feature. Refer to the [docs](https://docs.cupy.dev/en/latest/install.html#using-cupy-on-amd-gpu-experimental) for details.
 
 Use `-f https://pip.cupy.dev/pre` option to install pre-releases (e.g., `pip install cupy-cuda114 -f https://pip.cupy.dev/pre`).
```

### Comparing `cupy-9.5.0/cupy/__init__.py` & `cupy-9.6.0/cupy/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_binary/packing.py` & `cupy-9.6.0/cupy/_binary/packing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/__init__.py` & `cupy-9.6.0/cupy/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_accelerator.pyx` & `cupy-9.6.0/cupy/_core/_accelerator.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_carray.pxd` & `cupy-9.6.0/cupy/_core/_carray.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_carray.pyx` & `cupy-9.6.0/cupy/_core/_carray.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_codeblock.py` & `cupy-9.6.0/cupy/_core/_codeblock.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_cub_reduction.pyx` & `cupy-9.6.0/cupy/_core/_cub_reduction.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_dtype.pyx` & `cupy-9.6.0/cupy/_core/_dtype.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_interface.py` & `cupy-9.6.0/cupy/_core/_fusion_interface.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_kernel.pyx` & `cupy-9.6.0/cupy/_core/_fusion_kernel.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_op.py` & `cupy-9.6.0/cupy/_core/_fusion_op.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_optimization.py` & `cupy-9.6.0/cupy/_core/_fusion_optimization.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_thread_local.pyx` & `cupy-9.6.0/cupy/_core/_fusion_thread_local.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_trace.pyx` & `cupy-9.6.0/cupy/_core/_fusion_trace.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_fusion_variable.pyx` & `cupy-9.6.0/cupy/_core/_fusion_variable.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_gufuncs.py` & `cupy-9.6.0/cupy/_core/_gufuncs.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_kernel.pxd` & `cupy-9.6.0/cupy/_core/_kernel.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_kernel.pyx` & `cupy-9.6.0/cupy/_core/_kernel.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_memory_range.pyx` & `cupy-9.6.0/cupy/_core/_memory_range.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_optimize_config.pyx` & `cupy-9.6.0/cupy/_core/_optimize_config.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_reduction.pxd` & `cupy-9.6.0/cupy/_core/_reduction.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_reduction.pyx` & `cupy-9.6.0/cupy/_core/_reduction.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,17 @@
             tmp_contiguous_size *= a._shape[ndim-j-1]
         contiguous_size = max(contiguous_size, tmp_contiguous_size)
     return contiguous_size
 
 
 cdef Py_ssize_t _default_block_size = (
     256 if runtime._is_hip_environment else 512)
+cdef Py_ssize_t _min_block_size_log = 5
+cdef Py_ssize_t _max_block_size_log = (
+    8 if runtime._is_hip_environment else 9)
 
 
 cpdef (Py_ssize_t, Py_ssize_t, Py_ssize_t) _get_block_specs(  # NOQA
         Py_ssize_t in_size, Py_ssize_t out_size,
         Py_ssize_t contiguous_size,
         Py_ssize_t block_size) except*:
     cdef Py_ssize_t reduce_block_size, block_stride, out_block_num
@@ -414,15 +417,16 @@
         def target_func(block_size, block_stride, out_block_num):
             self._launch(
                 out_block_num, block_size, block_stride, in_args, out_args,
                 in_shape, out_shape, type_map, map_expr, reduce_expr,
                 post_map_expr, reduce_type, stream, self._params)
 
         def suggest_func(trial):
-            block_size_log = trial.suggest_int('block_size_log', 5, 9)
+            block_size_log = trial.suggest_int(
+                'block_size_log', _min_block_size_log, _max_block_size_log)
             block_size = 2 ** block_size_log
             block_stride_log = trial.suggest_int(
                 'block_stride_log', 0, block_size_log)
             block_stride = 2 ** block_stride_log
             max_out_block_num = (out_size + block_stride - 1) // block_stride
             out_block_num = trial.suggest_int(
                 'out_block_num', 1, max_out_block_num)
```

### Comparing `cupy-9.5.0/cupy/_core/_routines_binary.pyx` & `cupy-9.6.0/cupy/_core/_routines_binary.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_indexing.pxd` & `cupy-9.6.0/cupy/_core/_routines_indexing.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_indexing.pyx` & `cupy-9.6.0/cupy/_core/_routines_indexing.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_linalg.pxd` & `cupy-9.6.0/cupy/_core/_routines_linalg.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_linalg.pyx` & `cupy-9.6.0/cupy/_core/_routines_linalg.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_logic.pyx` & `cupy-9.6.0/cupy/_core/_routines_logic.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_manipulation.pxd` & `cupy-9.6.0/cupy/_core/_routines_manipulation.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_manipulation.pyx` & `cupy-9.6.0/cupy/_core/_routines_manipulation.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -327,25 +327,25 @@
 
     axes_size = axes.size()
     if axes_size == 0:
         return _T(self)
 
     ndim = self._shape.size()
     if axes_size != ndim:
-        raise ValueError('Invalid axes value: %s' % str(axes))
+        raise ValueError("axes don't match array")
 
     axis_flags.resize(ndim, 0)
     for i in range(axes_size):
         axis = axes[i]
         if axis < -ndim or axis >= ndim:
-            raise IndexError('Axes overrun')
+            raise numpy.AxisError(axis, ndim)
         axis %= ndim
         a_axes.push_back(axis)
         if axis_flags[axis]:
-            raise ValueError('Invalid axes value: %s' % str(axes))
+            raise ValueError('repeated axis in transpose')
         axis_flags[axis] = 1
         is_normal &= i == axis
         is_trans &= ndim - 1 - i == axis
 
     if is_normal:
         return self.view()
     if is_trans:
@@ -695,24 +695,25 @@
         if shape[dim] == 1:
             dim += 1
 
 
 cdef _normalize_axis_tuple(axis, Py_ssize_t ndim, shape_t &ret):
     """Normalizes an axis argument into a tuple of non-negative integer axes.
 
-    Arguments `allow_duplicate` and `axis_name` are not supported.
+    Arguments `argname` and `allow_duplicate` are not supported.
 
     """
     if numpy.isscalar(axis):
         axis = (axis,)
 
     for ax in axis:
         ax = internal._normalize_axis_index(ax, ndim)
         if _has_element(ret, ax):
-            raise numpy.AxisError('repeated axis')
+            # the message in `numpy.core.numeric.normalize_axis_tuple`
+            raise ValueError('repeated axis')
         ret.push_back(ax)
 
 
 cdef ndarray _concatenate_single_kernel(
         list arrays, Py_ssize_t axis, tuple shape, dtype,
         bint same_shape_and_contiguous, ndarray out):
     cdef ndarray a, x
```

### Comparing `cupy-9.5.0/cupy/_core/_routines_math.pxd` & `cupy-9.6.0/cupy/_core/_routines_math.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_math.pyx` & `cupy-9.6.0/cupy/_core/_routines_math.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 cdef ndarray _ndarray_prod(ndarray self, axis, dtype, out, keepdims):
     for accelerator in _accelerator._routine_accelerators:
         result = None
         if accelerator == _accelerator.ACCELERATOR_CUB:
             # result will be None if the reduction is not compatible with CUB
             result = cub.cub_reduction(
                 self, cub.CUPY_CUB_PROD, axis, dtype, out, keepdims)
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             result = cutensor._try_reduction_routine(
                 self, axis, dtype, out, keepdims, cuda_cutensor.OP_MUL, 1, 0)
         if result is not None:
             return result
     if dtype is None:
         return _prod_auto_dtype(self, axis, dtype, out, keepdims)
     else:
@@ -102,15 +103,16 @@
 cdef ndarray _ndarray_sum(ndarray self, axis, dtype, out, keepdims):
     for accelerator in _accelerator._routine_accelerators:
         result = None
         if accelerator == _accelerator.ACCELERATOR_CUB:
             # result will be None if the reduction is not compatible with CUB
             result = cub.cub_reduction(
                 self, cub.CUPY_CUB_SUM, axis, dtype, out, keepdims)
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             result = cutensor._try_reduction_routine(
                 self, axis, dtype, out, keepdims, cuda_cutensor.OP_ADD, 1, 0)
         if result is not None:
             return result
 
     if dtype is None:
         return _sum_auto_dtype(self, axis, dtype, out, keepdims)
```

### Comparing `cupy-9.5.0/cupy/_core/_routines_sorting.pyx` & `cupy-9.6.0/cupy/_core/_routines_sorting.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_statistics.pxd` & `cupy-9.6.0/cupy/_core/_routines_statistics.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_routines_statistics.pyx` & `cupy-9.6.0/cupy/_core/_routines_statistics.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 cdef ndarray _ndarray_max(ndarray self, axis, out, dtype, keepdims):
     for accelerator in _accelerator._routine_accelerators:
         result = None
         if accelerator == _accelerator.ACCELERATOR_CUB:
             # result will be None if the reduction is not compatible with CUB
             result = cub.cub_reduction(
                 self, cub.CUPY_CUB_MAX, axis, dtype, out, keepdims)
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             if self.dtype.kind == 'c' or dtype in ('F', 'D'):
                 # Complex dtype is not supported
                 continue
             result = cutensor._try_reduction_routine(
                 self, axis, dtype, out, keepdims, cuda_cutensor.OP_MAX, 1, 0)
         if result is not None:
             return result
@@ -44,15 +45,16 @@
 cdef ndarray _ndarray_min(ndarray self, axis, out, dtype, keepdims):
     for accelerator in _accelerator._routine_accelerators:
         result = None
         if accelerator == _accelerator.ACCELERATOR_CUB:
             # result will be None if the reduction is not compatible with CUB
             result = cub.cub_reduction(
                 self, cub.CUPY_CUB_MIN, axis, out, dtype, keepdims)
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             if self.dtype.kind == 'c' or dtype in ('F', 'D'):
                 # Complex dtype is not supported
                 continue
             result = cutensor._try_reduction_routine(
                 self, axis, dtype, out, keepdims, cuda_cutensor.OP_MIN, 1, 0)
         if result is not None:
             return result
@@ -65,15 +67,16 @@
             # result will be None if the reduction is not compatible with CUB
             result = cub.cub_reduction(
                 self, cub.CUPY_CUB_MAX, axis, out, None, keepdims)
             if result is not None:
                 result -= cub.cub_reduction(
                     self, cub.CUPY_CUB_MIN, axis, None, None, keepdims)
                 return result
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             if self.dtype.kind == 'c':
                 # Complex dtype is not supported
                 continue
             maxv = cutensor._try_reduction_routine(
                 self, axis, None, out, keepdims, cuda_cutensor.OP_MAX, 1, 0)
             if maxv is None:
                 continue
@@ -134,15 +137,16 @@
         if accelerator == _accelerator.ACCELERATOR_CUB and self.size != 0:
             result = cub.cub_reduction(
                 self, cub.CUPY_CUB_SUM, axis, dtype_sum, out, keepdims)
             if result is not None:
                 n = self.size // result.size
                 cupy.true_divide(result, n, out=result, casting='unsafe')
                 break
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             reduce_axis, _ = _reduction._get_axis(axis, self._shape.size())
             n = 1
             for i in reduce_axis:
                 n *= self._shape[i]
             n = max(n, 1)
             result = cutensor._try_reduction_routine(
                 self, axis, dtype_sum, out, keepdims,
```

### Comparing `cupy-9.5.0/cupy/_core/_scalar.pxd` & `cupy-9.6.0/cupy/_core/_scalar.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/_scalar.pyx` & `cupy-9.6.0/cupy/_core/_scalar.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/core.pxd` & `cupy-9.6.0/cupy/_core/core.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     cpdef ndarray max(self, axis=*, out=*, keepdims=*)
     cpdef ndarray argmax(self, axis=*, out=*, dtype=*,
                          keepdims=*)
     cpdef ndarray min(self, axis=*, out=*, keepdims=*)
     cpdef ndarray argmin(self, axis=*, out=*, dtype=*,
                          keepdims=*)
     cpdef ndarray ptp(self, axis=*, out=*, keepdims=*)
-    cpdef ndarray clip(self, a_min=*, a_max=*, out=*)
+    cpdef ndarray clip(self, min=*, max=*, out=*)
     cpdef ndarray round(self, decimals=*, out=*)
 
     cpdef ndarray trace(self, offset=*, axis1=*, axis2=*, dtype=*,
                         out=*)
     cpdef ndarray sum(self, axis=*, dtype=*, out=*, keepdims=*)
     cpdef ndarray cumsum(self, axis=*, dtype=*, out=*)
     cpdef ndarray mean(self, axis=*, dtype=*, out=*, keepdims=*)
```

### Comparing `cupy-9.5.0/cupy/_core/core.pyx` & `cupy-9.6.0/cupy/_core/core.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,16 @@
         """Returns an array flattened into one dimension.
 
         .. seealso::
            :func:`cupy.ravel` for full documentation,
            :meth:`numpy.ndarray.ravel`
 
         """
-        return _manipulation._ndarray_ravel(self, order)
+        return _internal_ascontiguousarray(
+            _manipulation._ndarray_ravel(self, order))
 
     cpdef ndarray squeeze(self, axis=None):
         """Returns a view with size-one axes removed.
 
         .. seealso::
            :func:`cupy.squeeze` for full documentation,
            :meth:`numpy.ndarray.squeeze`
@@ -913,23 +914,23 @@
         .. seealso::
            :func:`cupy.ptp` for full documentation,
            :meth:`numpy.ndarray.ptp`
 
         """
         return _statistics._ndarray_ptp(self, axis, out, keepdims)
 
-    cpdef ndarray clip(self, a_min=None, a_max=None, out=None):
-        """Returns an array with values limited to [a_min, a_max].
+    cpdef ndarray clip(self, min=None, max=None, out=None):
+        """Returns an array with values limited to [min, max].
 
         .. seealso::
            :func:`cupy.clip` for full documentation,
            :meth:`numpy.ndarray.clip`
 
         """
-        return _math._ndarray_clip(self, a_min, a_max, out)
+        return _math._ndarray_clip(self, min, max, out)
 
     cpdef ndarray round(self, decimals=0, out=None):
         """Returns an array with values rounded to the given number of decimals.
 
         .. seealso::
            :func:`cupy.around` for full documentation,
            :meth:`numpy.ndarray.round`
@@ -2007,20 +2008,17 @@
             bundled_include = 'cuda-10.1'
         elif 10020 <= _cuda_runtime_version < 10030:
             bundled_include = 'cuda-10.2'
         elif 11000 <= _cuda_runtime_version < 11010:
             bundled_include = 'cuda-11.0'
         elif 11010 <= _cuda_runtime_version < 11020:
             bundled_include = 'cuda-11.1'
-        elif 11020 <= _cuda_runtime_version < 11030:
-            bundled_include = 'cuda-11.2'
-        elif 11030 <= _cuda_runtime_version < 11040:
-            bundled_include = 'cuda-11.3'
-        elif 11040 <= _cuda_runtime_version < 11050:
-            bundled_include = 'cuda-11.4'
+        elif 11020 <= _cuda_runtime_version < 12000:
+            # for CUDA Enhanced Compatibility
+            bundled_include = 'cuda-11'
         else:
             # CUDA versions not yet supported.
             bundled_include = None
 
         if bundled_include is None and _cuda_path is None:
             raise RuntimeError(
                 'Failed to auto-detect CUDA root directory. '
```

### Comparing `cupy-9.5.0/cupy/_core/dlpack.pyx` & `cupy-9.6.0/cupy/_core/dlpack.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/flags.pyx` & `cupy-9.6.0/cupy/_core/flags.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/fusion.pyx` & `cupy-9.6.0/cupy/_core/fusion.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/halffloat.h` & `cupy-9.6.0/cupy/_core/halffloat.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/README.md` & `cupy-9.6.0/cupy/_core/include/cupy/README.md`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.hpp`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.hpp`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.hpp`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.hpp`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.hpp`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.2/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11/cuda_fp16.h`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 * \ingroup CUDA_MATH_INTRINSIC_HALF
 * To use these functions, include the header file \p cuda_fp16.h in your program.
 */
 
 #ifndef __CUDA_FP16_H__
 #define __CUDA_FP16_H__
 
+#define ___CUDA_FP16_STRINGIFY_INNERMOST(x) #x
+#define __CUDA_FP16_STRINGIFY(x) ___CUDA_FP16_STRINGIFY_INNERMOST(x)
+
 #if defined(__cplusplus)
 #if defined(__CUDACC__)
 #define __CUDA_FP16_DECL__ static __device__ __inline__
 #define __CUDA_HOSTDEVICE_FP16_DECL__ static __host__ __device__ __inline__
 #else
 #define __CUDA_HOSTDEVICE_FP16_DECL__ static
 #endif /* defined(__CUDACC__) */
@@ -360,15 +363,15 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ float2 __half22float2(const __half2 a);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed integer in round-to-nearest-even mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed integer in
-* round-to-nearest-even mode.
+* round-to-nearest-even mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns int
 * \retval h converted to a signed integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -376,15 +379,15 @@
 */
 __CUDA_FP16_DECL__ int __half2int_rn(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed integer in round-towards-zero mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed integer in
-* round-towards-zero mode.
+* round-towards-zero mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns int
 * \retval h converted to a signed integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -392,15 +395,15 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ int __half2int_rz(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed integer in round-down mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed integer in
-* round-down mode.
+* round-down mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns int
 * \retval h converted to a signed integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -408,15 +411,15 @@
 */
 __CUDA_FP16_DECL__ int __half2int_rd(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed integer in round-up mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed integer in
-* round-up mode.
+* round-up mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns int
 * \retval h converted to a signed integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -491,15 +494,15 @@
 
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed short integer in round-to-nearest-even
 * mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed short
-* integer in round-to-nearest-even mode.
+* integer in round-to-nearest-even mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns short int
 * \retval h converted to a signed short integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -507,15 +510,15 @@
 */
 __CUDA_FP16_DECL__ short int __half2short_rn(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed short integer in round-towards-zero mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed short
-* integer in round-towards-zero mode.
+* integer in round-towards-zero mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns short int
 * \retval h converted to a signed short integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -523,15 +526,15 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ short int __half2short_rz(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed short integer in round-down mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed short
-* integer in round-down mode.
+* integer in round-down mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns short int
 * \retval h converted to a signed short integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -539,15 +542,15 @@
 */
 __CUDA_FP16_DECL__ short int __half2short_rd(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed short integer in round-up mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed short
-* integer in round-up mode.
+* integer in round-up mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns short int
 * \retval h converted to a signed short integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -622,15 +625,15 @@
 __CUDA_FP16_DECL__ __half __short2half_ru(const short int i);
 
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned integer in round-to-nearest-even mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned integer
-* in round-to-nearest-even mode.
+* in round-to-nearest-even mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned int
 * \retval h converted to an unsigned integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -638,15 +641,15 @@
 */
 __CUDA_FP16_DECL__ unsigned int __half2uint_rn(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned integer in round-towards-zero mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned integer
-* in round-towards-zero mode.
+* in round-towards-zero mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned int
 * \retval h converted to an unsigned integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -654,15 +657,15 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ unsigned int __half2uint_rz(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned integer in round-down mode.
 *
 * \details Convert the half-precision floating-point value \p h to an unsigned integer
-* in round-down mode.
+* in round-down mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 *
 * \returns unsigned int
 * \retval h converted to an unsigned integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -670,15 +673,15 @@
 */
 __CUDA_FP16_DECL__ unsigned int __half2uint_rd(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned integer in round-up mode.
 *
 * \details Convert the half-precision floating-point value \p h to an unsigned integer
-* in round-up mode.
+* in round-up mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 *
 * \returns unsigned int
 * \retval h converted to an unsigned integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -753,15 +756,15 @@
 
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned short integer in round-to-nearest-even
 * mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned short
-* integer in round-to-nearest-even mode.
+* integer in round-to-nearest-even mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned short int
 * \retval h converted to an unsigned short integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -770,15 +773,15 @@
 __CUDA_FP16_DECL__ unsigned short int __half2ushort_rn(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned short integer in round-towards-zero
 * mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned short
-* integer in round-towards-zero mode.
+* integer in round-towards-zero mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned short int
 * \retval h converted to an unsigned short integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -786,27 +789,27 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ unsigned short int __half2ushort_rz(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned short integer in round-down mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned short
-* integer in round-down mode.
+* integer in round-down mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned short int
 * \retval h converted to an unsigned short integer. 
 */
 __CUDA_FP16_DECL__ unsigned short int __half2ushort_rd(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned short integer in round-up mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned short
-* integer in round-up mode.
+* integer in round-up mode. NaN inputs are converted to 0.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned short int
 * \retval h converted to an unsigned short integer. 
 */
 __CUDA_FP16_DECL__ unsigned short int __half2ushort_ru(const __half h);
 
@@ -879,15 +882,15 @@
 
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned 64-bit integer in round-to-nearest-even
 * mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned 64-bit
-* integer in round-to-nearest-even mode.
+* integer in round-to-nearest-even mode. NaN inputs return 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned long long int
 * \retval h converted to an unsigned 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -896,15 +899,15 @@
 __CUDA_FP16_DECL__ unsigned long long int __half2ull_rn(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned 64-bit integer in round-towards-zero
 * mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned 64-bit
-* integer in round-towards-zero mode.
+* integer in round-towards-zero mode. NaN inputs return 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned long long int
 * \retval h converted to an unsigned 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -912,15 +915,15 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ unsigned long long int __half2ull_rz(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned 64-bit integer in round-down mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned 64-bit
-* integer in round-down mode.
+* integer in round-down mode. NaN inputs return 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned long long int
 * \retval h converted to an unsigned 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -928,15 +931,15 @@
 */
 __CUDA_FP16_DECL__ unsigned long long int __half2ull_rd(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to an unsigned 64-bit integer in round-up mode.
 * 
 * \details Convert the half-precision floating-point value \p h to an unsigned 64-bit
-* integer in round-up mode.
+* integer in round-up mode. NaN inputs return 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns unsigned long long int
 * \retval h converted to an unsigned 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -1013,15 +1016,15 @@
 
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed 64-bit integer in round-to-nearest-even
 * mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed 64-bit
-* integer in round-to-nearest-even mode.
+* integer in round-to-nearest-even mode. NaN inputs return a long long int with hex value of 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns long long int
 * \retval h converted to a signed 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -1029,15 +1032,15 @@
 */
 __CUDA_FP16_DECL__ long long int __half2ll_rn(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed 64-bit integer in round-towards-zero mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed 64-bit
-* integer in round-towards-zero mode.
+* integer in round-towards-zero mode. NaN inputs return a long long int with hex value of 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns long long int
 * \retval h converted to a signed 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -1045,15 +1048,15 @@
 */
 __CUDA_HOSTDEVICE_FP16_DECL__ long long int __half2ll_rz(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed 64-bit integer in round-down mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed 64-bit
-* integer in round-down mode.
+* integer in round-down mode. NaN inputs return a long long int with hex value of 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns long long int
 * \retval h converted to a signed 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -1061,15 +1064,15 @@
 */
 __CUDA_FP16_DECL__ long long int __half2ll_rd(const __half h);
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Convert a half to a signed 64-bit integer in round-up mode.
 * 
 * \details Convert the half-precision floating-point value \p h to a signed 64-bit
-* integer in round-up mode.
+* integer in round-up mode. NaN inputs return a long long int with hex value of 0x8000000000000000.
 * \param[in] h - half. Is only being read. 
 * 
 * \returns long long int
 * \retval h converted to a signed 64-bit integer. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
@@ -1501,30 +1504,30 @@
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half __ushort_as_half(const unsigned short int i);
 
-#if __CUDA_ARCH__ >= 300 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 300)
 #if !defined warpSize && !defined __local_warpSize
 #define warpSize    32
 #define __local_warpSize
 #endif
 
 #if defined(_WIN32)
 # define __DEPRECATED__(msg) __declspec(deprecated(msg))
 #elif (defined(__GNUC__) && (__GNUC__ < 4 || (__GNUC__ == 4 && __GNUC_MINOR__ < 5 && !defined(__clang__))))
 # define __DEPRECATED__(msg) __attribute__((deprecated))
 #else
 # define __DEPRECATED__(msg) __attribute__((deprecated(msg)))
 #endif
 
 #if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ < 700
-#define __WSB_DEPRECATION_MESSAGE(x) #x"() is deprecated in favor of "#x"_sync() and may be removed in a future release (Use -Wno-deprecated-declarations to suppress this warning)."
+#define __WSB_DEPRECATION_MESSAGE(x) __CUDA_FP16_STRINGIFY(x) "() is deprecated in favor of " __CUDA_FP16_STRINGIFY(x) "_sync() and may be removed in a future release (Use -Wno-deprecated-declarations to suppress this warning)."
 
 __CUDA_FP16_DECL__ __DEPRECATED__(__WSB_DEPRECATION_MESSAGE(__shfl)) __half2 __shfl(const __half2 var, const int delta, const int width = warpSize);
 __CUDA_FP16_DECL__ __DEPRECATED__(__WSB_DEPRECATION_MESSAGE(__shfl_up)) __half2 __shfl_up(const __half2 var, const unsigned int delta, const int width = warpSize);
 __CUDA_FP16_DECL__ __DEPRECATED__(__WSB_DEPRECATION_MESSAGE(__shfl_down))__half2 __shfl_down(const __half2 var, const unsigned int delta, const int width = warpSize);
 __CUDA_FP16_DECL__ __DEPRECATED__(__WSB_DEPRECATION_MESSAGE(__shfl_xor)) __half2 __shfl_xor(const __half2 var, const int delta, const int width = warpSize);
 __CUDA_FP16_DECL__ __DEPRECATED__(__WSB_DEPRECATION_MESSAGE(__shfl)) __half __shfl(const __half var, const int delta, const int width = warpSize);
 __CUDA_FP16_DECL__ __DEPRECATED__(__WSB_DEPRECATION_MESSAGE(__shfl_up)) __half __shfl_up(const __half var, const unsigned int delta, const int width = warpSize);
@@ -1570,14 +1573,15 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half2. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 4-byte word referenced by var from the source thread ID as half2. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half2 __shfl_up_sync(const unsigned mask, const __half2 var, const unsigned int delta, const int width = warpSize);
 /**
@@ -1594,14 +1598,15 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half2. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 4-byte word referenced by var from the source thread ID as half2. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half2 __shfl_down_sync(const unsigned mask, const __half2 var, const unsigned int delta, const int width = warpSize);
 /**
@@ -1617,14 +1622,15 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half2. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 4-byte word referenced by var from the source thread ID as half2. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half2 __shfl_xor_sync(const unsigned mask, const __half2 var, const int delta, const int width = warpSize);
 /**
@@ -1641,14 +1647,15 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 2-byte word referenced by var from the source thread ID as half. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half __shfl_sync(const unsigned mask, const __half var, const int delta, const int width = warpSize);
 /**
@@ -1664,14 +1671,15 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 2-byte word referenced by var from the source thread ID as half. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half __shfl_up_sync(const unsigned mask, const __half var, const unsigned int delta, const int width = warpSize);
 /**
@@ -1688,14 +1696,15 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 2-byte word referenced by var from the source thread ID as half. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half __shfl_down_sync(const unsigned mask, const __half var, const unsigned int delta, const int width = warpSize);
 /**
@@ -1711,28 +1720,29 @@
 * \param[in] mask - unsigned int. Is only being read. 
 * \param[in] var - half. Is only being read. 
 * \param[in] delta - int. Is only being read. 
 * \param[in] width - int. Is only being read. 
 * 
 * \returns Returns the 2-byte word referenced by var from the source thread ID as half. 
 * If the source thread ID is out of range or the source thread has exited, the calling thread's own var is returned. 
+* \note_ref_guide_warp_shuffle
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior not reentrant, not thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half __shfl_xor_sync(const unsigned mask, const __half var, const int delta, const int width = warpSize);
 
 #if defined(__local_warpSize)
 #undef warpSize
 #undef __local_warpSize
 #endif
-#endif /*__CUDA_ARCH__ >= 300 || !defined(__CUDA_ARCH__) */
+#endif /*!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 300) */
 
-#if defined(__cplusplus) && ( __CUDA_ARCH__ >=320 || !defined(__CUDA_ARCH__) )
+#if defined(__cplusplus) && ( !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 320) )
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Generates a `ld.global.nc` load instruction.
 * \param[in] ptr - memory location
 * \returns The value pointed by `ptr`
 */
 __CUDA_FP16_DECL__ __half2 __ldg(const  __half2 *const ptr);
@@ -1865,17 +1875,17 @@
 /**
 * \ingroup CUDA_MATH__HALF_MISC
 * \brief Generates a `st.global.wt` store instruction.
 * \param[out] ptr - memory location
 * \param[in] value - the value to be stored
 */
 __CUDA_FP16_DECL__ void __stwt(__half *const ptr, const __half value);
-#endif /*defined(__cplusplus) && ( __CUDA_ARCH__ >=320 || !defined(__CUDA_ARCH__) )*/
+#endif /*defined(__cplusplus) && ( !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 320) )*/
 
-#if __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530)
 /**
 * \ingroup CUDA_MATH__HALF2_COMPARISON
 * \brief Performs half2 vector if-equal comparison.
 * 
 * \details Performs \p half2 vector if-equal comparison of inputs \p a and \p b.
 * The corresponding \p half results are set to 1.0 for true, or 0.0 for false.
 * NaN inputs generate false results.
@@ -3020,15 +3030,15 @@
 * \retval true iff argument is NaN. 
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ bool __hisnan(const __half a);
-#if __CUDA_ARCH__ >= 800 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 800)
 /**
 * \ingroup CUDA_MATH__HALF_COMPARISON
 * \brief Calculates \p half maximum of two input values.
 *
 * \details Calculates \p half max(\p a, \p b)
 * defined as (\p a > \p b) ? \p a : \p b.
 * - If either of inputs is NaN, the other input is returned.
@@ -3221,15 +3231,15 @@
 * \retval The result of elementwise fused multiply-add operation on vectors \p a, \p b, and \p c with relu saturation.
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half2 __hfma2_relu(const __half2 a, const __half2 b, const __half2 c);
-#endif /*__CUDA_ARCH__ >= 800 || !defined(__CUDA_ARCH__)*/
+#endif /* !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 800) */
 /**
 * \ingroup CUDA_MATH__HALF2_ARITHMETIC
 * \brief Performs fast complex multiply-accumulate
 *
 * \details Interprets vector \p half2 input pairs \p a, \p b, and \p c as
 * complex numbers in \p half precision and performs
 * complex multiply-accumulate operation: a*b + c
@@ -3600,32 +3610,68 @@
 * \internal
 * \exception-guarantee no-throw guarantee
 * \behavior reentrant, thread safe
 * \endinternal
 */
 __CUDA_FP16_DECL__ __half2 h2sin(const __half2 a);
 
-#endif /*if __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)*/
+#endif /*if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530)*/
+
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 600)
 
-#if __CUDA_ARCH__ >= 600 || !defined(__CUDA_ARCH__)
 
+/**
+* \ingroup CUDA_MATH__HALF2_FUNCTIONS
+* \brief Vector add \p val to the value stored at \p address in global or shared memory, and writes this
+* value back to \p address. The atomicity of the add operation is guaranteed separately for each of the
+* two __half elements; the entire __half2 is not guaranteed to be atomic as a single 32-bit access.
+* 
+* \details The location of \p address must be in global or shared memory. This operation has undefined
+* behavior otherwise. This operation is only supported by devices of compute capability 6.x and higher.
+* 
+* \param[in] address - half2*. An address in global or shared memory.
+* \param[in] val - half2. The value to be added.
+* 
+* \returns half2
+* \retval The old value read from \p address.
+*
+* \note_ref_guide_atomic
+*/
 __CUDA_FP16_DECL__ __half2 atomicAdd(__half2 *const address, const __half2 val);
 
-#endif /*if __CUDA_ARCH__ >= 600 || !defined(__CUDA_ARCH__)*/
+#endif /*if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 600)*/
 
-#if __CUDA_ARCH__ >= 700 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 700)
 
+/**
+* \ingroup CUDA_MATH__HALF_FUNCTIONS
+* \brief Adds \p val to the value stored at \p address in global or shared memory, and writes this value
+* back to \p address. This operation is performed in one atomic operation.
+* 
+* \details The location of \p address must be in global or shared memory. This operation has undefined
+* behavior otherwise. This operation is only supported by devices of compute capability 7.x and higher.
+* 
+* \param[in] address - half*. An address in global or shared memory.
+* \param[in] val - half. The value to be added.
+* 
+* \returns half
+* \retval The old value read from \p address.
+* 
+* \note_ref_guide_atomic
+*/
 __CUDA_FP16_DECL__ __half atomicAdd(__half *const address, const __half val);
 
-#endif /*if __CUDA_ARCH__ >= 700 || !defined(__CUDA_ARCH__)*/
+#endif /*if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 700)*/
 
 #endif /* defined(__CUDACC__) */
 
 #undef __CUDA_FP16_DECL__
 #undef __CUDA_HOSTDEVICE_FP16_DECL__
 
 #endif /* defined(__cplusplus) */
 
 /* Note the .hpp file is included even for host-side compilation, to capture the "half" & "half2" definitions */
 #include "cuda_fp16.hpp"
+#undef ___CUDA_FP16_STRINGIFY_INNERMOST
+#undef __CUDA_FP16_STRINGIFY
 
 #endif /* end of include guard: __CUDA_FP16_H__ */
```

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.2/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-11/cuda_fp16.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-* Copyright 1993-2020 NVIDIA Corporation.  All rights reserved.
+* Copyright 1993-2021 NVIDIA Corporation.  All rights reserved.
 *
 * NOTICE TO LICENSEE:
 *
 * This source code and/or documentation ("Licensed Deliverables") are
 * subject to NVIDIA intellectual property rights under U.S. and
 * international Copyright laws.
 *
@@ -114,33 +114,33 @@
 #define __HALF_TO_CUS(var) *(reinterpret_cast<const unsigned short *>(&(var)))
 #define __HALF2_TO_UI(var) *(reinterpret_cast<unsigned int *>(&(var)))
 #define __HALF2_TO_CUI(var) *(reinterpret_cast<const unsigned int *>(&(var)))
 
 /* Macros for half & half2 binary arithmetic */
 #define __BINARY_OP_HALF_MACRO(name) /* do */ {\
    __half val; \
-   asm( "{"#name".f16 %0,%1,%2;\n}" \
+   asm( "{" __CUDA_FP16_STRINGIFY(name) ".f16 %0,%1,%2;\n}" \
         :"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)),"h"(__HALF_TO_CUS(b))); \
    return val; \
 } /* while(0) */
 #define __BINARY_OP_HALF2_MACRO(name) /* do */ {\
    __half2 val; \
-   asm( "{"#name".f16x2 %0,%1,%2;\n}" \
+   asm( "{" __CUDA_FP16_STRINGIFY(name) ".f16x2 %0,%1,%2;\n}" \
         :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
    return val; \
 } /* while(0) */
 #define __TERNARY_OP_HALF_MACRO(name) /* do */ {\
    __half val; \
-   asm( "{"#name".f16 %0,%1,%2,%3;\n}" \
+   asm( "{" __CUDA_FP16_STRINGIFY(name) ".f16 %0,%1,%2,%3;\n}" \
         :"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)),"h"(__HALF_TO_CUS(b)),"h"(__HALF_TO_CUS(c))); \
    return val; \
 } /* while(0) */
 #define __TERNARY_OP_HALF2_MACRO(name) /* do */ {\
    __half2 val; \
-   asm( "{"#name".f16x2 %0,%1,%2,%3;\n}" \
+   asm( "{" __CUDA_FP16_STRINGIFY(name) ".f16x2 %0,%1,%2,%3;\n}" \
         :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b)),"r"(__HALF2_TO_CUI(c))); \
    return val; \
 } /* while(0) */
 
 /**
 * Types which allow static initialization of "half" and "half2" until
 * these become an actual builtin. Note this initialization is as a
@@ -243,15 +243,15 @@
 #endif /* !defined(__CUDA_NO_HALF_CONVERSIONS__) */
 };
 
 /* Global-space operator functions are only available to nvcc compilation */
 #if defined(__CUDACC__)
 
 /* Arithmetic FP16 operations only supported on arch >= 5.3 */
-#if __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530)
 #if !defined(__CUDA_NO_HALF_OPERATORS__)
 /* Some basic arithmetic operations expected of a builtin */
 __device__ __forceinline__ __half operator+(const __half &lh, const __half &rh) { return __hadd(lh, rh); }
 __device__ __forceinline__ __half operator-(const __half &lh, const __half &rh) { return __hsub(lh, rh); }
 __device__ __forceinline__ __half operator*(const __half &lh, const __half &rh) { return __hmul(lh, rh); }
 __device__ __forceinline__ __half operator/(const __half &lh, const __half &rh) { return __hdiv(lh, rh); }
 
@@ -259,30 +259,50 @@
 __device__ __forceinline__ __half &operator-=(__half &lh, const __half &rh) { lh = __hsub(lh, rh); return lh; }
 __device__ __forceinline__ __half &operator*=(__half &lh, const __half &rh) { lh = __hmul(lh, rh); return lh; }
 __device__ __forceinline__ __half &operator/=(__half &lh, const __half &rh) { lh = __hdiv(lh, rh); return lh; }
 
 /* Note for increment and decrement we use the raw value 0x3C00U equating to half(1.0F), to avoid the extra conversion */
 __device__ __forceinline__ __half &operator++(__half &h)      { __half_raw one; one.x = 0x3C00U; h += one; return h; }
 __device__ __forceinline__ __half &operator--(__half &h)      { __half_raw one; one.x = 0x3C00U; h -= one; return h; }
-__device__ __forceinline__ __half  operator++(__half &h, const int ignored) { const __half ret = h; __half_raw one; one.x = 0x3C00U; h += one; return ret; }
-__device__ __forceinline__ __half  operator--(__half &h, const int ignored) { const __half ret = h; __half_raw one; one.x = 0x3C00U; h -= one; return ret; }
+__device__ __forceinline__ __half  operator++(__half &h, const int ignored)
+{
+    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
+    static_cast<void>(ignored);
+
+    const __half ret = h;
+    __half_raw one;
+    one.x = 0x3C00U;
+    h += one;
+    return ret;
+}
+__device__ __forceinline__ __half  operator--(__half &h, const int ignored)
+{
+    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
+    static_cast<void>(ignored);
+
+    const __half ret = h;
+    __half_raw one;
+    one.x = 0x3C00U;
+    h -= one;
+    return ret;
+}
 
 /* Unary plus and inverse operators */
 __device__ __forceinline__ __half operator+(const __half &h) { return h; }
 __device__ __forceinline__ __half operator-(const __half &h) { return __hneg(h); }
 
 /* Some basic comparison operations to make it look like a builtin */
 __device__ __forceinline__ bool operator==(const __half &lh, const __half &rh) { return __heq(lh, rh); }
 __device__ __forceinline__ bool operator!=(const __half &lh, const __half &rh) { return __hneu(lh, rh); }
 __device__ __forceinline__ bool operator> (const __half &lh, const __half &rh) { return __hgt(lh, rh); }
 __device__ __forceinline__ bool operator< (const __half &lh, const __half &rh) { return __hlt(lh, rh); }
 __device__ __forceinline__ bool operator>=(const __half &lh, const __half &rh) { return __hge(lh, rh); }
 __device__ __forceinline__ bool operator<=(const __half &lh, const __half &rh) { return __hle(lh, rh); }
 #endif /* !defined(__CUDA_NO_HALF_OPERATORS__) */
-#endif /* __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__) */
+#endif /* !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530) */
 #endif /* defined(__CUDACC__) */
 
 /* __half2 is visible to non-nvcc host compilers */
 struct __CUDA_ALIGN__(4) __half2 {
     __half x;
     __half y;
 
@@ -305,42 +325,64 @@
     __CUDA_HOSTDEVICE__ operator __half2_raw() const { __half2_raw ret; ret.x = 0U; ret.y = 0U; __HALF2_TO_UI(ret) = __HALF2_TO_CUI(*this); return ret; }
 };
 
 /* Global-space operator functions are only available to nvcc compilation */
 #if defined(__CUDACC__)
 
 /* Arithmetic FP16x2 operations only supported on arch >= 5.3 */
-#if (__CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)) && !defined(__CUDA_NO_HALF2_OPERATORS__)
+#if (!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530)) && !defined(__CUDA_NO_HALF2_OPERATORS__)
 
 __device__ __forceinline__ __half2 operator+(const __half2 &lh, const __half2 &rh) { return __hadd2(lh, rh); }
 __device__ __forceinline__ __half2 operator-(const __half2 &lh, const __half2 &rh) { return __hsub2(lh, rh); }
 __device__ __forceinline__ __half2 operator*(const __half2 &lh, const __half2 &rh) { return __hmul2(lh, rh); }
 __device__ __forceinline__ __half2 operator/(const __half2 &lh, const __half2 &rh) { return __h2div(lh, rh); }
 
 __device__ __forceinline__ __half2& operator+=(__half2 &lh, const __half2 &rh) { lh = __hadd2(lh, rh); return lh; }
 __device__ __forceinline__ __half2& operator-=(__half2 &lh, const __half2 &rh) { lh = __hsub2(lh, rh); return lh; }
 __device__ __forceinline__ __half2& operator*=(__half2 &lh, const __half2 &rh) { lh = __hmul2(lh, rh); return lh; }
 __device__ __forceinline__ __half2& operator/=(__half2 &lh, const __half2 &rh) { lh = __h2div(lh, rh); return lh; }
 
 __device__ __forceinline__ __half2 &operator++(__half2 &h)      { __half2_raw one; one.x = 0x3C00U; one.y = 0x3C00U; h = __hadd2(h, one); return h; }
 __device__ __forceinline__ __half2 &operator--(__half2 &h)      { __half2_raw one; one.x = 0x3C00U; one.y = 0x3C00U; h = __hsub2(h, one); return h; }
-__device__ __forceinline__ __half2  operator++(__half2 &h, const int ignored) { const __half2 ret = h; __half2_raw one; one.x = 0x3C00U; one.y = 0x3C00U; h = __hadd2(h, one); return ret; }
-__device__ __forceinline__ __half2  operator--(__half2 &h, const int ignored) { const __half2 ret = h; __half2_raw one; one.x = 0x3C00U; one.y = 0x3C00U; h = __hsub2(h, one); return ret; }
+__device__ __forceinline__ __half2  operator++(__half2 &h, const int ignored)
+{
+    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
+    static_cast<void>(ignored);
+
+    const __half2 ret = h;
+    __half2_raw one;
+    one.x = 0x3C00U;
+    one.y = 0x3C00U;
+    h = __hadd2(h, one);
+    return ret;
+}
+__device__ __forceinline__ __half2  operator--(__half2 &h, const int ignored)
+{
+    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
+    static_cast<void>(ignored);
+
+    const __half2 ret = h;
+    __half2_raw one;
+    one.x = 0x3C00U;
+    one.y = 0x3C00U;
+    h = __hsub2(h, one);
+    return ret;
+}
 
 __device__ __forceinline__ __half2 operator+(const __half2 &h) { return h; }
 __device__ __forceinline__ __half2 operator-(const __half2 &h) { return __hneg2(h); }
 
 __device__ __forceinline__ bool operator==(const __half2 &lh, const __half2 &rh) { return __hbeq2(lh, rh); }
 __device__ __forceinline__ bool operator!=(const __half2 &lh, const __half2 &rh) { return __hbneu2(lh, rh); }
 __device__ __forceinline__ bool operator>(const __half2 &lh, const __half2 &rh) { return __hbgt2(lh, rh); }
 __device__ __forceinline__ bool operator<(const __half2 &lh, const __half2 &rh) { return __hblt2(lh, rh); }
 __device__ __forceinline__ bool operator>=(const __half2 &lh, const __half2 &rh) { return __hbge2(lh, rh); }
 __device__ __forceinline__ bool operator<=(const __half2 &lh, const __half2 &rh) { return __hble2(lh, rh); }
 
-#endif /* __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__) */
+#endif /* !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530) */
 #endif /* defined(__CUDACC__) */
 
 /* Restore warning for multiple assignment operators */
 #if defined(_MSC_VER) && _MSC_VER >= 1500
 #pragma warning( pop )
 #endif /* defined(_MSC_VER) && _MSC_VER >= 1500 */
 
@@ -384,14 +426,15 @@
     } else { // Denormal numbers
         const unsigned int exponent = u >> 23U;
         const unsigned int shift = 0x7eU - exponent;
         unsigned int mantissa = (u & 0x7fffffU);
         mantissa |= 0x800000U;
         remainder = mantissa << (32U - shift);
         result = (sign | (mantissa >> shift));
+        result &= 0x0000FFFFU;
     }
     return static_cast<unsigned short>(result);
 }
 #endif  /* #if !defined(__CUDACC_RTC__) */
 
 __CUDA_HOSTDEVICE_FP16_DECL__ __half __double2half(const double a)
 {
@@ -571,18 +614,23 @@
 #endif
     return val;
 }
 __CUDA_HOSTDEVICE_FP16_DECL__ __half2 __floats2half2_rn(const float a, const float b)
 {
     __half2 val;
 #if defined(__CUDA_ARCH__)
+#if (__CUDA_ARCH__ >= 800)
+    asm("{ cvt.rn.f16x2.f32 %0, %2, %1; }\n"
+        : "=r"(__HALF2_TO_UI(val)) : "f"(a), "f"(b));
+#else
     asm("{.reg .f16 low,high;\n"
         "  cvt.rn.f16.f32 low, %1;\n"
         "  cvt.rn.f16.f32 high, %2;\n"
         "  mov.b32 %0, {low,high};}\n" : "=r"(__HALF2_TO_UI(val)) : "f"(a), "f"(b));
+#endif
 #else
     val = __half2(__float2half_rn(a), __float2half_rn(b));
 #endif
     return val;
 }
 
 #ifndef __CUDACC_RTC__  /* no host functions in NVRTC mode */
@@ -607,15 +655,15 @@
                 --exponent;
             } while (msb == 0U);
             mantissa &= 0x7fffffU; /* 1.mantissa is implicit */
         }
     } else {
         exponent += 0x70U;
     }
-    unsigned int u = ((sign << 31U) | (exponent << 23U) | mantissa);
+    const unsigned int u = ((sign << 31U) | (exponent << 23U) | mantissa);
 #if defined(__CUDACC__)
     (void)memcpy(&f, &u, sizeof(u));
 #else
     (void)std::memcpy(&f, &u, sizeof(u));
 #endif
     return f;
 }
@@ -703,24 +751,27 @@
 #if defined __CUDA_ARCH__
     asm("cvt.rzi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
 #else
     const float f = __half2float(h);
                 i = static_cast<int>(f);
     const int max_val = (int)0x7fffffffU;
     const int min_val = (int)0x80000000U;
+    const unsigned short bits = static_cast<unsigned short>(static_cast<__half_raw>(h).x << 1U);
     // saturation fixup
-    if (f != f) {
+    if (bits > (unsigned short)0xF800U) {
         // NaN
         i = 0;
     } else if (f > static_cast<float>(max_val)) {
         // saturate maximum
         i = max_val;
     } else if (f < static_cast<float>(min_val)) {
         // saturate minimum
         i = min_val;
+    } else {
+        // normal value, do nothing
     }
 #endif
     return i;
 }
 __CUDA_FP16_DECL__ int __half2int_rd(const __half h)
 {
     int i;
@@ -779,24 +830,27 @@
 #if defined __CUDA_ARCH__
     asm("cvt.rzi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
 #else
     const float f = __half2float(h);
                 i = static_cast<short int>(f);
     const short int max_val = (short int)0x7fffU;
     const short int min_val = (short int)0x8000U;
+    const unsigned short bits = static_cast<unsigned short>(static_cast<__half_raw>(h).x << 1U);
     // saturation fixup
-    if (f != f) {
+    if (bits > (unsigned short)0xF800U) {
         // NaN
         i = 0;
     } else if (f > static_cast<float>(max_val)) {
         // saturate maximum
         i = max_val;
     } else if (f < static_cast<float>(min_val)) {
         // saturate minimum
         i = min_val;
+    } else {
+        // normal value, do nothing
     }
 #endif
     return i;
 }
 __CUDA_FP16_DECL__ short int __half2short_rd(const __half h)
 {
     short int i;
@@ -851,24 +905,27 @@
 #if defined __CUDA_ARCH__
     asm("cvt.rzi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
 #else
     const float f = __half2float(h);
                 i = static_cast<unsigned int>(f);
     const unsigned int max_val = 0xffffffffU;
     const unsigned int min_val = 0U;
+    const unsigned short bits = static_cast<unsigned short>(static_cast<__half_raw>(h).x << 1U);
     // saturation fixup
-    if (f != f) {
+    if (bits > (unsigned short)0xF800U) {
         // NaN
         i = 0U;
     } else if (f > static_cast<float>(max_val)) {
         // saturate maximum
         i = max_val;
     } else if (f < static_cast<float>(min_val)) {
         // saturate minimum
         i = min_val;
+    } else {
+        // normal value, do nothing
     }
 #endif
     return i;
 }
 __CUDA_FP16_DECL__ unsigned int __half2uint_rd(const __half h)
 {
     unsigned int i;
@@ -927,24 +984,27 @@
 #if defined __CUDA_ARCH__
     asm("cvt.rzi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
 #else
     const float f = __half2float(h);
                 i = static_cast<unsigned short int>(f);
     const unsigned short int max_val = 0xffffU;
     const unsigned short int min_val = 0U;
+    const unsigned short bits = static_cast<unsigned short>(static_cast<__half_raw>(h).x << 1U);
     // saturation fixup
-    if (f != f) {
+    if (bits > (unsigned short)0xF800U) {
         // NaN
         i = 0U;
     } else if (f > static_cast<float>(max_val)) {
         // saturate maximum
         i = max_val;
     } else if (f < static_cast<float>(min_val)) {
         // saturate minimum
         i = min_val;
+    } else {
+        // normal value, do nothing
     }
 #endif
     return i;
 }
 __CUDA_FP16_DECL__ unsigned short int __half2ushort_rd(const __half h)
 {
     unsigned short int i;
@@ -999,24 +1059,27 @@
 #if defined __CUDA_ARCH__
     asm("cvt.rzi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
 #else
     const float f = __half2float(h);
                 i = static_cast<unsigned long long int>(f);
     const unsigned long long int max_val = 0xffffffffffffffffULL;
     const unsigned long long int min_val = 0ULL;
+    const unsigned short bits = static_cast<unsigned short>(static_cast<__half_raw>(h).x << 1U);
     // saturation fixup
-    if (f != f) {
+    if (bits > (unsigned short)0xF800U) {
         // NaN
         i = 0x8000000000000000ULL;
     } else if (f > static_cast<float>(max_val)) {
         // saturate maximum
         i = max_val;
     } else if (f < static_cast<float>(min_val)) {
         // saturate minimum
         i = min_val;
+    } else {
+        // normal value, do nothing
     }
 #endif
     return i;
 }
 __CUDA_FP16_DECL__ unsigned long long int __half2ull_rd(const __half h)
 {
     unsigned long long int i;
@@ -1075,24 +1138,27 @@
 #if defined __CUDA_ARCH__
     asm("cvt.rzi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
 #else
     const float f = __half2float(h);
                 i = static_cast<long long int>(f);
     const long long int max_val = (long long int)0x7fffffffffffffffULL;
     const long long int min_val = (long long int)0x8000000000000000ULL;
+    const unsigned short bits = static_cast<unsigned short>(static_cast<__half_raw>(h).x << 1U);
     // saturation fixup
-    if (f != f) {
+    if (bits > (unsigned short)0xF800U) {
         // NaN
         i = min_val;
     } else if (f > static_cast<float>(max_val)) {
         // saturate maximum
         i = max_val;
     } else if (f < static_cast<float>(min_val)) {
         // saturate minimum
         i = min_val;
+    } else {
+        // normal value, do nothing
     }
 #endif
     return i;
 }
 __CUDA_FP16_DECL__ long long int __half2ll_rd(const __half h)
 {
     long long int i;
@@ -1305,28 +1371,28 @@
 __CUDA_FP16_DECL__ __half __ushort_as_half(const unsigned short int i)
 {
     __half h;
     __HALF_TO_US(h) = i;
     return h;
 }
 
-#if __CUDA_ARCH__ >= 300 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 300)
 /******************************************************************************
 *                           __half, __half2 warp shuffle                     *
 ******************************************************************************/
 #define __SHUFFLE_HALF2_MACRO(name) /* do */ {\
    __half2 r; \
-   asm volatile ("{"#name" %0,%1,%2,%3;\n}" \
+   asm volatile ("{" __CUDA_FP16_STRINGIFY(name) " %0,%1,%2,%3;\n}" \
        :"=r"(__HALF2_TO_UI(r)): "r"(__HALF2_TO_CUI(var)), "r"(delta), "r"(c)); \
    return r; \
 } /* while(0) */
 
 #define __SHUFFLE_SYNC_HALF2_MACRO(name) /* do */ {\
    __half2 r; \
-   asm volatile ("{"#name" %0,%1,%2,%3,%4;\n}" \
+   asm volatile ("{" __CUDA_FP16_STRINGIFY(name) " %0,%1,%2,%3,%4;\n}" \
        :"=r"(__HALF2_TO_UI(r)): "r"(__HALF2_TO_CUI(var)), "r"(delta), "r"(c), "r"(mask)); \
    return r; \
 } /* while(0) */
 
 #if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ < 700
 
 __CUDA_FP16_DECL__ __half2 __shfl(const __half2 var, const int delta, const int width)
@@ -1442,20 +1508,20 @@
 __CUDA_FP16_DECL__ __half __shfl_xor_sync(const unsigned mask, const __half var, const int delta, const int width)
 {
     const __half2 temp1 = __halves2half2(var, var);
     const __half2 temp2 = __shfl_xor_sync(mask, temp1, delta, width);
     return __low2half(temp2);
 }
 
-#endif /*__CUDA_ARCH__ >= 300 || !defined(__CUDA_ARCH__)*/
+#endif /*!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 300)*/
 /******************************************************************************
 *               __half and __half2 __ldg,__ldcg,__ldca,__ldcs                *
 ******************************************************************************/
 
-#if defined(__cplusplus) && (__CUDA_ARCH__ >= 320 || !defined(__CUDA_ARCH__))
+#if defined(__cplusplus) && (!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 320))
 #if (defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)
 #define __LDG_PTR   "l"
 #else
 #define __LDG_PTR   "r"
 #endif /*(defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)*/
 __CUDA_FP16_DECL__ __half2 __ldg(const  __half2 *const ptr)
 {
@@ -1558,22 +1624,22 @@
     asm ("st.global.wt.b32 [%0], %1;"  :: __LDG_PTR(ptr), "r"(__HALF2_TO_CUI(value)) : "memory");
 }
 __CUDA_FP16_DECL__ void __stwt(__half *const ptr, const __half value)
 {
     asm ("st.global.wt.b16 [%0], %1;"  :: __LDG_PTR(ptr),  "h"(__HALF_TO_CUS(value)) : "memory");
 }
 #undef __LDG_PTR
-#endif /*defined(__cplusplus) && (__CUDA_ARCH__ >= 320 || !defined(__CUDA_ARCH__))*/
-#if __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)
+#endif /*defined(__cplusplus) && (!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 320))*/
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530)
 /******************************************************************************
 *                             __half2 comparison                             *
 ******************************************************************************/
 #define __COMPARISON_OP_HALF2_MACRO(name) /* do */ {\
    __half2 val; \
-   asm( "{ "#name".f16x2.f16x2 %0,%1,%2;\n}" \
+   asm( "{ " __CUDA_FP16_STRINGIFY(name) ".f16x2.f16x2 %0,%1,%2;\n}" \
         :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
    return val; \
 } /* while(0) */
 __CUDA_FP16_DECL__ __half2 __heq2(const __half2 a, const __half2 b)
 {
     __COMPARISON_OP_HALF2_MACRO(set.eq)
 }
@@ -1621,15 +1687,15 @@
 {
     __COMPARISON_OP_HALF2_MACRO(set.gtu)
 }
 #undef __COMPARISON_OP_HALF2_MACRO
 #define __BOOL_COMPARISON_OP_HALF2_MACRO(name) /* do */ {\
    __half2 val; \
    bool retval; \
-   asm( "{ "#name".f16x2.f16x2 %0,%1,%2;\n}" \
+   asm( "{ " __CUDA_FP16_STRINGIFY(name) ".f16x2.f16x2 %0,%1,%2;\n}" \
         :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
    if (__HALF2_TO_CUI(val) == 0x3C003C00U) {\
       retval = true; \
    } else { \
       retval = false; \
    }\
    return retval;\
@@ -1685,15 +1751,15 @@
 #undef __BOOL_COMPARISON_OP_HALF2_MACRO
 /******************************************************************************
 *                             __half comparison                              *
 ******************************************************************************/
 #define __COMPARISON_OP_HALF_MACRO(name) /* do */ {\
    unsigned short val; \
    asm( "{ .reg .pred __$temp3;\n" \
-        "  setp."#name".f16  __$temp3, %1, %2;\n" \
+        "  setp." __CUDA_FP16_STRINGIFY(name) ".f16  __$temp3, %1, %2;\n" \
         "  selp.u16 %0, 1, 0, __$temp3;}" \
         : "=h"(val) : "h"(__HALF_TO_CUS(a)), "h"(__HALF_TO_CUS(b))); \
    return (val != 0U) ? true : false; \
 } /* while(0) */
 __CUDA_FP16_DECL__ bool __heq(const __half a, const __half b)
 {
     __COMPARISON_OP_HALF_MACRO(eq)
@@ -1814,15 +1880,14 @@
 {
     __BINARY_OP_HALF_MACRO(sub.sat)
 }
 __CUDA_FP16_DECL__ __half __hmul_sat(const __half a, const __half b)
 {
     __BINARY_OP_HALF_MACRO(mul.sat)
 }
-
 __CUDA_FP16_DECL__ __half __hfma(const __half a, const __half b, const __half c)
 {
     __TERNARY_OP_HALF_MACRO(fma.rn)
 }
 __CUDA_FP16_DECL__ __half __hfma_sat(const __half a, const __half b, const __half c)
 {
     __TERNARY_OP_HALF_MACRO(fma.rn.sat)
@@ -1852,190 +1917,179 @@
 }
 
 /******************************************************************************
 *                             __half2 functions                  *
 ******************************************************************************/
 #define __SPEC_CASE2(i,r, spc, ulp) \
    "{.reg.b32 spc, ulp, p;\n"\
-   "  mov.b32 spc,"#spc";\n"\
-   "  mov.b32 ulp,"#ulp";\n"\
-   "  set.eq.f16x2.f16x2 p,"#i", spc;\n"\
-   "  fma.rn.f16x2 "#r",p,ulp,"#r";\n}\n"
+   "  mov.b32 spc," __CUDA_FP16_STRINGIFY(spc) ";\n"\
+   "  mov.b32 ulp," __CUDA_FP16_STRINGIFY(ulp) ";\n"\
+   "  set.eq.f16x2.f16x2 p," __CUDA_FP16_STRINGIFY(i) ", spc;\n"\
+   "  fma.rn.f16x2 " __CUDA_FP16_STRINGIFY(r) ",p,ulp," __CUDA_FP16_STRINGIFY(r) ";\n}\n"
 #define __SPEC_CASE(i,r, spc, ulp) \
    "{.reg.b16 spc, ulp, p;\n"\
-   "  mov.b16 spc,"#spc";\n"\
-   "  mov.b16 ulp,"#ulp";\n"\
-   "  set.eq.f16.f16 p,"#i", spc;\n"\
-   "  fma.rn.f16 "#r",p,ulp,"#r";\n}\n"
+   "  mov.b16 spc," __CUDA_FP16_STRINGIFY(spc) ";\n"\
+   "  mov.b16 ulp," __CUDA_FP16_STRINGIFY(ulp) ";\n"\
+   "  set.eq.f16.f16 p," __CUDA_FP16_STRINGIFY(i) ", spc;\n"\
+   "  fma.rn.f16 " __CUDA_FP16_STRINGIFY(r) ",p,ulp," __CUDA_FP16_STRINGIFY(r) ";\n}\n"
 #define __APPROX_FCAST(fun) /* do */ {\
    __half val;\
    asm("{.reg.b32         f;        \n"\
                 " .reg.b16         r;        \n"\
                 "  mov.b16         r,%1;     \n"\
                 "  cvt.f32.f16     f,r;      \n"\
-                "  "#fun".approx.f32   f,f;  \n"\
+                "  " __CUDA_FP16_STRINGIFY(fun) ".approx.f32   f,f;  \n"\
                 "  cvt.rn.f16.f32      r,f;  \n"\
                 "  mov.b16         %0,r;     \n"\
                 "}": "=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));\
    return val;\
 } /* while(0) */
 #define __APPROX_FCAST2(fun) /* do */ {\
    __half2 val;\
    asm("{.reg.b16         hl, hu;         \n"\
                 " .reg.b32         fl, fu;         \n"\
                 "  mov.b32         {hl, hu}, %1;   \n"\
                 "  cvt.f32.f16     fl, hl;         \n"\
                 "  cvt.f32.f16     fu, hu;         \n"\
-                "  "#fun".approx.f32   fl, fl;     \n"\
-                "  "#fun".approx.f32   fu, fu;     \n"\
+                "  " __CUDA_FP16_STRINGIFY(fun) ".approx.f32   fl, fl;     \n"\
+                "  " __CUDA_FP16_STRINGIFY(fun) ".approx.f32   fu, fu;     \n"\
                 "  cvt.rn.f16.f32      hl, fl;     \n"\
                 "  cvt.rn.f16.f32      hu, fu;     \n"\
                 "  mov.b32         %0, {hl, hu};   \n"\
                 "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));       \
    return val;\
 } /* while(0) */
 static __device__ __forceinline__ float __float_simpl_sinf(float a);
 static __device__ __forceinline__ float __float_simpl_cosf(float a);
-__CUDA_FP16_DECL__ __half __hsin_internal(const __half a) {
-    float f = __half2float(a);
-    f = __float_simpl_sinf(f);
-    return __float2half_rn(f);
-}
 __CUDA_FP16_DECL__ __half hsin(const __half a) {
-    __half r = __hsin_internal(a);
+    const float sl = __float_simpl_sinf(__half2float(a));
+    __half r = __float2half_rn(sl);
     asm("{\n\t"
         "  .reg.b16 i,r,t;     \n\t"
         "  mov.b16 r, %0;      \n\t"
         "  mov.b16 i, %1;      \n\t"
-        "  mov.b16 t, 0x8000U;  \n\t"
-        "  and.b16 t,r,t;      \n\t"
+        "  and.b16 t, r, 0x8000U; \n\t"
+        "  abs.f16 r, r;   \n\t"
+        "  abs.f16 i, i;   \n\t"
         __SPEC_CASE(i, r, 0X32B3U, 0x0800U)
-        __SPEC_CASE(i, r, 0X5CB0U, 0x1000U)
-        __SPEC_CASE(i, r, 0XB2B3U, 0x8800U)
-        __SPEC_CASE(i, r, 0XDCB0U, 0x9000U)
+        __SPEC_CASE(i, r, 0X5CB0U, 0x9000U)
         "  or.b16  r,r,t;      \n\t"
         "  mov.b16 %0, r;      \n"
         "}\n" : "+h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)));
     return r;
 }
 __CUDA_FP16_DECL__ __half2 h2sin(const __half2 a) {
-    const __half l = __low2half(a);
-    const __half h = __high2half(a);
-    const __half sl = __hsin_internal(l);
-    const __half sh = __hsin_internal(h);
-    __half2 r = __halves2half2(sl, sh);
+    const float sl = __float_simpl_sinf(__half2float(a.x));
+    const float sh = __float_simpl_sinf(__half2float(a.y));
+    __half2 r = __floats2half2_rn(sl, sh);
     asm("{\n\t"
         "  .reg.b32 i,r,t;             \n\t"
         "  mov.b32 r, %0;              \n\t"
         "  mov.b32 i, %1;              \n\t"
         "  and.b32 t, r, 0x80008000U;   \n\t"
+        "  abs.f16x2 r, r;   \n\t"
+        "  abs.f16x2 i, i;   \n\t"
         __SPEC_CASE2(i, r, 0X32B332B3U, 0x08000800U)
-        __SPEC_CASE2(i, r, 0X5CB05CB0U, 0x10001000U)
-        __SPEC_CASE2(i, r, 0XB2B3B2B3U, 0x88008800U)
-        __SPEC_CASE2(i, r, 0XDCB0DCB0U, 0x90009000U)
+        __SPEC_CASE2(i, r, 0X5CB05CB0U, 0x90009000U)
         "  or.b32  r, r, t;            \n\t"
         "  mov.b32 %0, r;              \n"
         "}\n" : "+r"(__HALF2_TO_UI(r)) : "r"(__HALF2_TO_CUI(a)));
     return r;
 }
-__CUDA_FP16_DECL__ __half __hcos_internal(const __half a) {
-    float f = __half2float(a);
-    f = __float_simpl_cosf(f);
-    return __float2half_rn(f);
-}
 __CUDA_FP16_DECL__ __half hcos(const __half a) {
-    __half r = __hcos_internal(a);
+    const float cl = __float_simpl_cosf(__half2float(a));
+    __half r = __float2half_rn(cl);
     asm("{\n\t"
         "  .reg.b16 i,r;        \n\t"
         "  mov.b16 r, %0;       \n\t"
         "  mov.b16 i, %1;       \n\t"
+        "  abs.f16 i, i;        \n\t"
         __SPEC_CASE(i, r, 0X2B7CU, 0x1000U)
-        __SPEC_CASE(i, r, 0XAB7CU, 0x1000U)
         "  mov.b16 %0, r;       \n"
         "}\n" : "+h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)));
     return r;
 }
 __CUDA_FP16_DECL__ __half2 h2cos(const __half2 a) {
-    const __half l = __low2half(a);
-    const __half h = __high2half(a);
-    const __half cl = __hcos_internal(l);
-    const __half ch = __hcos_internal(h);
-    __half2 r = __halves2half2(cl, ch);
+    const float cl = __float_simpl_cosf(__half2float(a.x));
+    const float ch = __float_simpl_cosf(__half2float(a.y));
+    __half2 r = __floats2half2_rn(cl, ch);
     asm("{\n\t"
         "  .reg.b32 i,r;   \n\t"
         "  mov.b32 r, %0;  \n\t"
         "  mov.b32 i, %1;  \n\t"
+        "  abs.f16x2 i, i; \n\t"
         __SPEC_CASE2(i, r, 0X2B7C2B7CU, 0x10001000U)
-        __SPEC_CASE2(i, r, 0XAB7CAB7CU, 0x10001000U)
         "  mov.b32 %0, r;  \n"
         "}\n" : "+r"(__HALF2_TO_UI(r)) : "r"(__HALF2_TO_CUI(a)));
     return r;
 }
-static __device__ __forceinline__ float __internal_trig_reduction_kernel(const float a, int *quadrant)
+static __device__ __forceinline__ float __internal_trig_reduction_kernel(const float a, unsigned int *const quadrant)
 {
-    const int q = __float2int_rn(a * 0.636619772F);
-    const float j = static_cast<float>(q);
-    float t = __fmaf_rn(-j, 1.5707962512969971e+000F, a);
-    t = __fmaf_rn(-j, 7.5497894158615964e-008F, t);
+    const float ar = __fmaf_rn(a, 0.636619772F, 12582912.0F);
+    const unsigned q = __float_as_uint(ar);
+    const float j = __fsub_rn(ar, 12582912.0F);
+    float t = __fmaf_rn(j, -1.5707962512969971e+000F, a);
+    t = __fmaf_rn(j, -7.5497894158615964e-008F, t);
     *quadrant = q;
     return t;
 }
-static __device__ __forceinline__ float __internal_sin_cos_kernel(float x, const int i)
+static __device__ __forceinline__ float __internal_sin_cos_kernel(const float x, const unsigned int i)
 {
     float z;
     const float x2 = x*x;
-
-    if ((static_cast<unsigned>(i) & 1U) != 0U) {
-        z = 2.44331571e-5F;
-        z = __fmaf_rn(z, x2, -1.38873163e-3F);
-    }
-    else {
-        z = -1.95152959e-4F;
-        z = __fmaf_rn(z, x2, 8.33216087e-3F);
-    }
-    if ((static_cast<unsigned>(i) & 1U) != 0U) {
-        z = __fmaf_rn(z, x2, 4.16666457e-2F);
-        z = __fmaf_rn(z, x2, -5.00000000e-1F);
-    }
-    else {
-        z = __fmaf_rn(z, x2, -1.66666546e-1F);
-        z = __fmaf_rn(z, x2, 0.0F);
-    }
-    if ((static_cast<unsigned>(i) & 1U) != 0U) {
-        x = __fmaf_rn(z, x2, 1.0F);
+    float a8;
+    float a6;
+    float a4;
+    float a2;
+    float a1;
+    float a0;
+
+    if ((i & 1U) != 0U) {
+        // cos
+        a8 =  2.44331571e-5F;
+        a6 = -1.38873163e-3F;
+        a4 =  4.16666457e-2F;
+        a2 = -5.00000000e-1F;
+        a1 = x2;
+        a0 = 1.0F;
     }
     else {
-        x = __fmaf_rn(z, x, x);
-    }
-    if ((static_cast<unsigned>(i) & 2U) != 0U) {
-        x = __fmaf_rn(x, -1.0F, 0.0F);
+        // sin
+        a8 = -1.95152959e-4F;
+        a6 =  8.33216087e-3F;
+        a4 = -1.66666546e-1F;
+        a2 = 0.0F;
+        a1 = x;
+        a0 = x;
+    }
+
+    z = __fmaf_rn(a8, x2, a6);
+    z = __fmaf_rn(z, x2, a4);
+    z = __fmaf_rn(z, x2, a2);
+    z = __fmaf_rn(z, a1, a0);
+
+    if ((i & 2U) != 0U) {
+        z = -z;
     }
-    return x;
+    return z;
 }
 static __device__ __forceinline__ float __float_simpl_sinf(float a)
 {
     float z;
-    int i;
-    if (::isinf(a)) {
-        a = a * 0.0F;
-    }
+    unsigned i;
     a = __internal_trig_reduction_kernel(a, &i);
     z = __internal_sin_cos_kernel(a, i);
     return z;
 }
 static __device__ __forceinline__ float __float_simpl_cosf(float a)
 {
     float z;
-    int i;
-    if (::isinf(a)) {
-        a = a * 0.0F;
-    }
+    unsigned i;
     a = __internal_trig_reduction_kernel(a, &i);
-    i++;
-    z = __internal_sin_cos_kernel(a, i);
+    z = __internal_sin_cos_kernel(a, (i & 0x3U) + 1U);
     return z;
 }
 
 __CUDA_FP16_DECL__ __half hexp(const __half a) {
     __half val;
     asm("{.reg.b32         f, C;           \n"
         " .reg.b16         h,r;            \n"
@@ -2336,24 +2390,23 @@
 
 __CUDA_FP16_DECL__ __half2 __hcmadd(const __half2 a, const __half2 b, const __half2 c)
 {
     // fast version of complex multiply-accumulate
     // (a.re, a.im) * (b.re, b.im) + (c.re, c.im)
     // acc.re = (c.re + a.re*b.re) - a.im*b.im
     // acc.im = (c.im + a.re*b.im) + a.im*b.re
-    const __half2 a_re = __half2half2(a.x);
-          __half2 acc  = __hfma2(a_re, b, c);
-    const __half2 a_im = __half2half2(a.y);
-    const __half2 ib   = __halves2half2(__hneg(b.y), b.x);
-                  acc  = __hfma2(a_im, ib, acc);
-    return acc;
+    __half real_tmp =  __hfma(a.x, b.x, c.x);
+    __half img_tmp  =  __hfma(a.x, b.y, c.y);
+    real_tmp = __hfma(__hneg(a.y), b.y, real_tmp);
+    img_tmp  = __hfma(a.y,         b.x, img_tmp);
+    return make_half2(real_tmp, img_tmp);
 }
-#endif /*__CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)*/
+#endif /*!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 530)*/
 
-#if __CUDA_ARCH__ >= 800 || !defined(__CUDA_ARCH__)
+#if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 800)
 /******************************************************************************
 *                             __half arithmetic                             *
 ******************************************************************************/
 __CUDA_FP16_DECL__ __half __hmax(const __half a, const __half b)
 {
     __BINARY_OP_HALF_MACRO(max)
 }
@@ -2392,15 +2445,15 @@
 {
     __BINARY_OP_HALF2_MACRO(min.NaN)
 }
 __CUDA_FP16_DECL__ __half2 __hfma2_relu(const __half2 a, const __half2 b, const __half2 c)
 {
     __TERNARY_OP_HALF2_MACRO(fma.rn.relu)
 }
-#endif /*__CUDA_ARCH__ >= 800 || !defined(__CUDA_ARCH__)*/
+#endif /*!defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 800)*/
 
 /* Define __PTR for atomicAdd prototypes below, undef after done */
 #if (defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)
 #define __PTR   "l"
 #else
 #define __PTR   "r"
 #endif /*(defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)*/
@@ -2439,15 +2492,20 @@
 #undef __TERNARY_OP_HALF2_MACRO
 #undef __TERNARY_OP_HALF_MACRO
 #undef __BINARY_OP_HALF2_MACRO
 #undef __BINARY_OP_HALF_MACRO
 
 #undef __CUDA_HOSTDEVICE_FP16_DECL__
 #undef __CUDA_FP16_DECL__
- 
+
+#undef __HALF_TO_US
+#undef __HALF_TO_CUS
+#undef __HALF2_TO_UI
+#undef __HALF2_TO_CUI
+
 /* Define first-class types "half" and "half2", unless user specifies otherwise via "#define CUDA_NO_HALF" */
 /* C cannot ever have these types defined here, because __half and __half2 are C++ classes */
 #if defined(__cplusplus) && !defined(CUDA_NO_HALF)
 typedef __half half;
 typedef __half2 half2;
 // for consistency with __nv_bfloat16
 typedef __half      __nv_half;
```

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-11.3/cuda_fp16.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-* Copyright 1993-2020 NVIDIA Corporation.  All rights reserved.
+* Copyright 1993-2014 NVIDIA Corporation.  All rights reserved.
 *
 * NOTICE TO LICENSEE:
 *
 * This source code and/or documentation ("Licensed Deliverables") are
 * subject to NVIDIA intellectual property rights under U.S. and
 * international Copyright laws.
 *
@@ -46,119 +46,87 @@
 * comments to the code, the above Disclaimer and U.S. Government End
 * Users Notice.
 */
 
 #if !defined(__CUDA_FP16_HPP__)
 #define __CUDA_FP16_HPP__
 
-#if !defined(__CUDA_FP16_H__)
-#error "Do not include this file directly. Instead, include cuda_fp16.h."
-#endif
-
-#if !defined(_MSC_VER) && __cplusplus >= 201103L
-#   define __CPP_VERSION_AT_LEAST_11_FP16
-#elif _MSC_FULL_VER >= 190024210 && _MSVC_LANG >= 201103L
-#   define __CPP_VERSION_AT_LEAST_11_FP16
-#endif
-
 /* C++11 header for std::move. 
  * In RTC mode, std::move is provided implicitly; don't include the header
- */
-#if defined(__CPP_VERSION_AT_LEAST_11_FP16) && !defined(__CUDACC_RTC__)
+*/
+#if (__cplusplus >= 201103L) && !defined(__CUDACC_RTC__)
 #include <utility>
 #endif /* __cplusplus >= 201103L && !defined(__CUDACC_RTC__) */
 
-/* C++ header for std::memcpy (used for type punning in host-side implementations).
- * When compiling as a CUDA source file memcpy is provided implicitly.
- * !defined(__CUDACC__) implies !defined(__CUDACC_RTC__).
- */
-#if defined(__cplusplus) && !defined(__CUDACC__)
-#include <cstring>
-#endif /* defined(__cplusplus) && !defined(__CUDACC__) */
-
-
+/* Set up function decorations */
 /* Set up function decorations */
 #if defined(__CUDACC__)
 #define __CUDA_FP16_DECL__ static __device__ __inline__
 #define __CUDA_HOSTDEVICE_FP16_DECL__ static __host__ __device__ __inline__
 #define __VECTOR_FUNCTIONS_DECL__ static __inline__ __host__ __device__
 #define __CUDA_HOSTDEVICE__ __host__ __device__
 #else /* !defined(__CUDACC__) */
-#if defined(__GNUC__)
+#if defined(__GNUC__) /* || defined(__IBMC__) || defined(__clang__) || defined(__PGI) */
 #define __CUDA_HOSTDEVICE_FP16_DECL__ static __attribute__ ((unused))
 #else
 #define __CUDA_HOSTDEVICE_FP16_DECL__ static
 #endif /* defined(__GNUC__) */
 #define __CUDA_HOSTDEVICE__
 #endif /* defined(__CUDACC_) */
 
 /* Set up structure-alignment attribute */
 #if defined(__CUDACC__)
 #define __CUDA_ALIGN__(align) __align__(align)
 #else
 /* Define alignment macro based on compiler type (cannot assume C11 "_Alignas" is available) */
 #if __cplusplus >= 201103L
 #define __CUDA_ALIGN__(n) alignas(n)    /* C++11 kindly gives us a keyword for this */
-#else /* !defined(__CPP_VERSION_AT_LEAST_11_FP16)*/
-#if defined(__GNUC__)
+#else /* !(__cplusplus >= 201103L)*/
+#if defined(__GNUC__) /* || defined(__IBMC__) || defined(__clang__) || defined(__PGI) */
 #define __CUDA_ALIGN__(n) __attribute__ ((aligned(n)))
-#elif defined(_MSC_VER)
+#elif defined(_MSC_VER) /* || defined(__ICC) */
 #define __CUDA_ALIGN__(n) __declspec(align(n))
 #else
 #define __CUDA_ALIGN__(n)
 #endif /* defined(__GNUC__) */
-#endif /* defined(__CPP_VERSION_AT_LEAST_11_FP16) */
+#endif /* __cplusplus >= 201103L */
 #endif /* defined(__CUDACC__) */
 
+
 /* Macros to allow half & half2 to be used by inline assembly */
 #define __HALF_TO_US(var) *(reinterpret_cast<unsigned short *>(&(var)))
 #define __HALF_TO_CUS(var) *(reinterpret_cast<const unsigned short *>(&(var)))
+#define __HALF_TO_VUS(var) *(reinterpret_cast<volatile unsigned short *>(&(var)))
+#define __HALF_TO_CVUS(var) *(reinterpret_cast<const volatile unsigned short *>(&(var)))
 #define __HALF2_TO_UI(var) *(reinterpret_cast<unsigned int *>(&(var)))
 #define __HALF2_TO_CUI(var) *(reinterpret_cast<const unsigned int *>(&(var)))
 
-/* Macros for half & half2 binary arithmetic */
-#define __BINARY_OP_HALF_MACRO(name) /* do */ {\
-   __half val; \
-   asm( "{"#name".f16 %0,%1,%2;\n}" \
-        :"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)),"h"(__HALF_TO_CUS(b))); \
-   return val; \
-} /* while(0) */
-#define __BINARY_OP_HALF2_MACRO(name) /* do */ {\
-   __half2 val; \
-   asm( "{"#name".f16x2 %0,%1,%2;\n}" \
-        :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
-   return val; \
-} /* while(0) */
-#define __TERNARY_OP_HALF_MACRO(name) /* do */ {\
-   __half val; \
-   asm( "{"#name".f16 %0,%1,%2,%3;\n}" \
-        :"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)),"h"(__HALF_TO_CUS(b)),"h"(__HALF_TO_CUS(c))); \
-   return val; \
-} /* while(0) */
-#define __TERNARY_OP_HALF2_MACRO(name) /* do */ {\
-   __half2 val; \
-   asm( "{"#name".f16x2 %0,%1,%2,%3;\n}" \
-        :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b)),"r"(__HALF2_TO_CUI(c))); \
-   return val; \
-} /* while(0) */
+/* Type punning macros for host-side implementations */
+#if defined(__CUDACC__)
+#define __COPY_FLOAT_TO_UI(to, from) ((to) = *(reinterpret_cast<unsigned int *>(&(from))))
+#define __COPY_UI_TO_FLOAT(to, from) ((to) = *(reinterpret_cast<float *>(&(from))))
+#else
+#include <string.h>
+#define __COPY_FLOAT_TO_UI(to, from) memcpy(&(to), &(from), sizeof((to)))
+#define __COPY_UI_TO_FLOAT(to, from) memcpy(&(to), &(from), sizeof((to)))
+#endif
 
 /**
 * Types which allow static initialization of "half" and "half2" until
 * these become an actual builtin. Note this initialization is as a
 * bitfield representation of "half", and not a conversion from short->half.
 * Such a representation will be deprecated in a future version of CUDA. 
 * (Note these are visible to non-nvcc compilers, including C-only compilation)
 */
 typedef struct __CUDA_ALIGN__(2) {
     unsigned short x;
 } __half_raw;
 
 typedef struct __CUDA_ALIGN__(4) {
-    unsigned short x;
-    unsigned short y;
+    unsigned short x, y;
 } __half2_raw;
 
 /* All other definitions in this file are only visible to C++ compilers */
 #if defined(__cplusplus)
 
 /* Hide GCC member initialization list warnings because of host/device in-function init requirement */
 #if defined(__GNUC__)
@@ -177,72 +145,72 @@
 #endif /* defined(__GNUC__) */
 
 struct __CUDA_ALIGN__(2) __half {
 protected:
     unsigned short __x;
 
 public:
-#if defined(__CPP_VERSION_AT_LEAST_11_FP16)
+#if __cplusplus >= 201103L
     __half() = default;
 #else
     __CUDA_HOSTDEVICE__ __half() { }
-#endif /* defined(__CPP_VERSION_AT_LEAST_11_FP16) */
+#endif /* __cplusplus >= 201103L */
 
     /* Convert to/from __half_raw */
     __CUDA_HOSTDEVICE__ __half(const __half_raw &hr) : __x(hr.x) { }
     __CUDA_HOSTDEVICE__ __half &operator=(const __half_raw &hr) { __x = hr.x; return *this; }
     __CUDA_HOSTDEVICE__ volatile __half &operator=(const __half_raw &hr) volatile { __x = hr.x; return *this; }
     __CUDA_HOSTDEVICE__ volatile __half &operator=(const volatile __half_raw &hr) volatile { __x = hr.x; return *this; }
     __CUDA_HOSTDEVICE__ operator __half_raw() const { __half_raw ret; ret.x = __x; return ret; }
-    __CUDA_HOSTDEVICE__ operator __half_raw() const volatile { __half_raw ret; ret.x = __x; return ret; }
+    __CUDA_HOSTDEVICE__ operator volatile __half_raw() const volatile { __half_raw ret; ret.x = __x; return ret; }
 
 #if !defined(__CUDA_NO_HALF_CONVERSIONS__)
 
     /* Construct from float/double */
-    __CUDA_HOSTDEVICE__ __half(const float f) { __x = __float2half(f).__x;  }
-    __CUDA_HOSTDEVICE__ __half(const double f) { __x = __double2half(f).__x;  }
+    __CUDA_HOSTDEVICE__ __half(float f) { __x = __float2half(f).__x;  }
+    __CUDA_HOSTDEVICE__ __half(double f) { __x = __float2half(static_cast<float>(f)).__x;  }
 
     __CUDA_HOSTDEVICE__ operator float() const { return __half2float(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const float f) { __x = __float2half(f).__x; return *this; }
+    __CUDA_HOSTDEVICE__ __half &operator=(float f) { __x = __float2half(f).__x; return *this; }
 
     /* We omit "cast to double" operator, so as to not be ambiguous about up-cast */
-    __CUDA_HOSTDEVICE__ __half &operator=(const double f) { __x = __double2half(f).__x; return *this; }
+    __CUDA_HOSTDEVICE__ __half &operator=(double f) { __x = __float2half(static_cast<float>(f)).__x; return *this; }
 
 /* Member functions only available to nvcc compilation so far */
 #if defined(__CUDACC__)
     /* Allow automatic construction from types supported natively in hardware */
     /* Note we do avoid constructor init-list because of special host/device compilation rules */
-    __CUDA_HOSTDEVICE__ __half(const short val) { __x = __short2half_rn(val).__x;  }
-    __CUDA_HOSTDEVICE__ __half(const unsigned short val) { __x = __ushort2half_rn(val).__x;  }
-    __CUDA_HOSTDEVICE__ __half(const int val) { __x = __int2half_rn(val).__x;  }
-    __CUDA_HOSTDEVICE__ __half(const unsigned int val) { __x = __uint2half_rn(val).__x;  }
-    __CUDA_HOSTDEVICE__ __half(const long long val) { __x = __ll2half_rn(val).__x;  }
-    __CUDA_HOSTDEVICE__ __half(const unsigned long long val) { __x = __ull2half_rn(val).__x; }
+    __device__ __half(short val) { __x = __short2half_rn(val).__x;  }
+    __device__ __half(unsigned short val) { __x = __ushort2half_rn(val).__x;  }
+    __device__ __half(int val) { __x = __int2half_rn(val).__x;  }
+    __device__ __half(unsigned int val) { __x = __uint2half_rn(val).__x;  }
+    __device__ __half(long long val) { __x = __ll2half_rn(val).__x;  }
+    __device__ __half(unsigned long long val) { __x = __ull2half_rn(val).__x; }
 
     /* Allow automatic casts to supported builtin types, matching all that are permitted with float */
-    __CUDA_HOSTDEVICE__ operator short() const { return __half2short_rz(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const short val) { __x = __short2half_rn(val).__x; return *this; }
+    __device__ operator short() const { return __half2short_rn(*this); }
+    __device__ __half &operator=(short val) { __x = __short2half_rn(val).__x; return *this; }
 
-    __CUDA_HOSTDEVICE__ operator unsigned short() const { return __half2ushort_rz(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const unsigned short val) { __x = __ushort2half_rn(val).__x; return *this; }
+    __device__ operator unsigned short() const { return __half2ushort_rn(*this); }
+    __device__ __half &operator=(unsigned short val) { __x = __ushort2half_rn(val).__x; return *this; }
 
-    __CUDA_HOSTDEVICE__ operator int() const { return __half2int_rz(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const int val) { __x = __int2half_rn(val).__x; return *this; }
+    __device__ operator int() const { return __half2int_rn(*this); }
+    __device__ __half &operator=(int val) { __x = __int2half_rn(val).__x; return *this; }
 
-    __CUDA_HOSTDEVICE__ operator unsigned int() const { return __half2uint_rz(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const unsigned int val) { __x = __uint2half_rn(val).__x; return *this; }
+    __device__ operator unsigned int() const { return __half2uint_rn(*this); }
+    __device__ __half &operator=(unsigned int val) { __x = __uint2half_rn(val).__x; return *this; }
 
-    __CUDA_HOSTDEVICE__ operator long long() const { return __half2ll_rz(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const long long val) { __x = __ll2half_rn(val).__x; return *this; }
+    __device__ operator long long() const { return __half2ll_rn(*this); }
+    __device__ __half &operator=(long long val) { __x = __ll2half_rn(val).__x; return *this; }
 
-    __CUDA_HOSTDEVICE__ operator unsigned long long() const { return __half2ull_rz(*this); }
-    __CUDA_HOSTDEVICE__ __half &operator=(const unsigned long long val) { __x = __ull2half_rn(val).__x; return *this; }
+    __device__ operator unsigned long long() const { return __half2ull_rn(*this); }
+    __device__ __half &operator=(unsigned long long val) { __x = __ull2half_rn(val).__x; return *this; }
 
     /* Boolean conversion - note both 0 and -0 must return false */
-    __CUDA_HOSTDEVICE__ operator bool() const { return (__x & 0x7FFFU) != 0U; }
+    __device__ operator bool() const { return (__x & 0x7FFF) != 0; }
 #endif /* defined(__CUDACC__) */
 #endif /* !defined(__CUDA_NO_HALF_CONVERSIONS__) */
 };
 
 /* Global-space operator functions are only available to nvcc compilation */
 #if defined(__CUDACC__)
 
@@ -256,77 +224,56 @@
 __device__ __forceinline__ __half operator/(const __half &lh, const __half &rh) { return __hdiv(lh, rh); }
 
 __device__ __forceinline__ __half &operator+=(__half &lh, const __half &rh) { lh = __hadd(lh, rh); return lh; }
 __device__ __forceinline__ __half &operator-=(__half &lh, const __half &rh) { lh = __hsub(lh, rh); return lh; }
 __device__ __forceinline__ __half &operator*=(__half &lh, const __half &rh) { lh = __hmul(lh, rh); return lh; }
 __device__ __forceinline__ __half &operator/=(__half &lh, const __half &rh) { lh = __hdiv(lh, rh); return lh; }
 
-/* Note for increment and decrement we use the raw value 0x3C00U equating to half(1.0F), to avoid the extra conversion */
-__device__ __forceinline__ __half &operator++(__half &h)      { __half_raw one; one.x = 0x3C00U; h += one; return h; }
-__device__ __forceinline__ __half &operator--(__half &h)      { __half_raw one; one.x = 0x3C00U; h -= one; return h; }
-__device__ __forceinline__ __half  operator++(__half &h, const int ignored)
-{
-    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
-    static_cast<void>(ignored);
-
-    const __half ret = h;
-    __half_raw one;
-    one.x = 0x3C00U;
-    h += one;
-    return ret;
-}
-__device__ __forceinline__ __half  operator--(__half &h, const int ignored)
-{
-    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
-    static_cast<void>(ignored);
-
-    const __half ret = h;
-    __half_raw one;
-    one.x = 0x3C00U;
-    h -= one;
-    return ret;
-}
+/* Note for increment and decrement we use the raw value 0x3C00 equating to half(1.0f), to avoid the extra conversion */
+__device__ __forceinline__ __half &operator++(__half &h)      { __half_raw one; one.x = 0x3C00; h += one; return h; }
+__device__ __forceinline__ __half &operator--(__half &h)      { __half_raw one; one.x = 0x3C00; h -= one; return h; }
+__device__ __forceinline__ __half  operator++(__half &h, int) { __half ret = h; __half_raw one; one.x = 0x3C00; h += one; return ret; }
+__device__ __forceinline__ __half  operator--(__half &h, int) { __half ret = h; __half_raw one; one.x = 0x3C00; h -= one; return ret; }
 
 /* Unary plus and inverse operators */
 __device__ __forceinline__ __half operator+(const __half &h) { return h; }
 __device__ __forceinline__ __half operator-(const __half &h) { return __hneg(h); }
 
 /* Some basic comparison operations to make it look like a builtin */
 __device__ __forceinline__ bool operator==(const __half &lh, const __half &rh) { return __heq(lh, rh); }
-__device__ __forceinline__ bool operator!=(const __half &lh, const __half &rh) { return __hneu(lh, rh); }
+__device__ __forceinline__ bool operator!=(const __half &lh, const __half &rh) { return __hne(lh, rh); }
 __device__ __forceinline__ bool operator> (const __half &lh, const __half &rh) { return __hgt(lh, rh); }
 __device__ __forceinline__ bool operator< (const __half &lh, const __half &rh) { return __hlt(lh, rh); }
 __device__ __forceinline__ bool operator>=(const __half &lh, const __half &rh) { return __hge(lh, rh); }
 __device__ __forceinline__ bool operator<=(const __half &lh, const __half &rh) { return __hle(lh, rh); }
 #endif /* !defined(__CUDA_NO_HALF_OPERATORS__) */
 #endif /* __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__) */
 #endif /* defined(__CUDACC__) */
 
 /* __half2 is visible to non-nvcc host compilers */
 struct __CUDA_ALIGN__(4) __half2 {
-    __half x;
-    __half y;
+    __half x, y;
 
     // All construct/copy/assign/move
 public:
-#if defined(__CPP_VERSION_AT_LEAST_11_FP16)
+#if __cplusplus >= 201103L
     __half2() = default;
-    __CUDA_HOSTDEVICE__ __half2(const __half2 &&src) { __HALF2_TO_UI(*this) = std::move(__HALF2_TO_CUI(src)); }
-    __CUDA_HOSTDEVICE__ __half2 &operator=(const __half2 &&src) { __HALF2_TO_UI(*this) = std::move(__HALF2_TO_CUI(src)); return *this; }
+    __CUDA_HOSTDEVICE__ __half2(__half2 &&src) { __HALF2_TO_UI(*this) = std::move(__HALF2_TO_CUI(src)); }
+    __CUDA_HOSTDEVICE__ __half2 &operator=(__half2 &&src) { __HALF2_TO_UI(*this) = std::move(__HALF2_TO_CUI(src)); return *this; }
 #else
     __CUDA_HOSTDEVICE__ __half2() { }
-#endif /* defined(__CPP_VERSION_AT_LEAST_11_FP16) */
+#endif /* __cplusplus >= 201103L */
     __CUDA_HOSTDEVICE__ __half2(const __half &a, const __half &b) : x(a), y(b) { }
     __CUDA_HOSTDEVICE__ __half2(const __half2 &src) { __HALF2_TO_UI(*this) = __HALF2_TO_CUI(src); }
     __CUDA_HOSTDEVICE__ __half2 &operator=(const __half2 &src) { __HALF2_TO_UI(*this) = __HALF2_TO_CUI(src); return *this; }
 
     /* Convert to/from __half2_raw */
     __CUDA_HOSTDEVICE__ __half2(const __half2_raw &h2r ) { __HALF2_TO_UI(*this) = __HALF2_TO_CUI(h2r); }
     __CUDA_HOSTDEVICE__ __half2 &operator=(const __half2_raw &h2r) { __HALF2_TO_UI(*this) = __HALF2_TO_CUI(h2r); return *this; }
-    __CUDA_HOSTDEVICE__ operator __half2_raw() const { __half2_raw ret; ret.x = 0U; ret.y = 0U; __HALF2_TO_UI(ret) = __HALF2_TO_CUI(*this); return ret; }
+    __CUDA_HOSTDEVICE__ operator __half2_raw() const { __half2_raw ret; __HALF2_TO_UI(ret) = __HALF2_TO_CUI(*this); return ret; }
 };
 
 /* Global-space operator functions are only available to nvcc compilation */
 #if defined(__CUDACC__)
 
 /* Arithmetic FP16x2 operations only supported on arch >= 5.3 */
 #if (__CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)) && !defined(__CUDA_NO_HALF2_OPERATORS__)
@@ -337,848 +284,572 @@
 __device__ __forceinline__ __half2 operator/(const __half2 &lh, const __half2 &rh) { return __h2div(lh, rh); }
 
 __device__ __forceinline__ __half2& operator+=(__half2 &lh, const __half2 &rh) { lh = __hadd2(lh, rh); return lh; }
 __device__ __forceinline__ __half2& operator-=(__half2 &lh, const __half2 &rh) { lh = __hsub2(lh, rh); return lh; }
 __device__ __forceinline__ __half2& operator*=(__half2 &lh, const __half2 &rh) { lh = __hmul2(lh, rh); return lh; }
 __device__ __forceinline__ __half2& operator/=(__half2 &lh, const __half2 &rh) { lh = __h2div(lh, rh); return lh; }
 
-__device__ __forceinline__ __half2 &operator++(__half2 &h)      { __half2_raw one; one.x = 0x3C00U; one.y = 0x3C00U; h = __hadd2(h, one); return h; }
-__device__ __forceinline__ __half2 &operator--(__half2 &h)      { __half2_raw one; one.x = 0x3C00U; one.y = 0x3C00U; h = __hsub2(h, one); return h; }
-__device__ __forceinline__ __half2  operator++(__half2 &h, const int ignored)
-{
-    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
-    static_cast<void>(ignored);
-
-    const __half2 ret = h;
-    __half2_raw one;
-    one.x = 0x3C00U;
-    one.y = 0x3C00U;
-    h = __hadd2(h, one);
-    return ret;
-}
-__device__ __forceinline__ __half2  operator--(__half2 &h, const int ignored)
-{
-    // ignored on purpose. Parameter only needed to distinguish the function declaration from other types of operators.
-    static_cast<void>(ignored);
-
-    const __half2 ret = h;
-    __half2_raw one;
-    one.x = 0x3C00U;
-    one.y = 0x3C00U;
-    h = __hsub2(h, one);
-    return ret;
-}
+__device__ __forceinline__ __half2 &operator++(__half2 &h)      { __half2_raw one; one.x = 0x3C00; one.y = 0x3C00; h = __hadd2(h, one); return h; }
+__device__ __forceinline__ __half2 &operator--(__half2 &h)      { __half2_raw one; one.x = 0x3C00; one.y = 0x3C00; h = __hsub2(h, one); return h; }
+__device__ __forceinline__ __half2  operator++(__half2 &h, int) { __half2 ret = h; __half2_raw one; one.x = 0x3C00; one.y = 0x3C00; h = __hadd2(h, one); return ret; }
+__device__ __forceinline__ __half2  operator--(__half2 &h, int) { __half2 ret = h; __half2_raw one; one.x = 0x3C00; one.y = 0x3C00; h = __hsub2(h, one); return ret; }
 
 __device__ __forceinline__ __half2 operator+(const __half2 &h) { return h; }
 __device__ __forceinline__ __half2 operator-(const __half2 &h) { return __hneg2(h); }
 
-__device__ __forceinline__ bool operator==(const __half2 &lh, const __half2 &rh) { return __hbeq2(lh, rh); }
-__device__ __forceinline__ bool operator!=(const __half2 &lh, const __half2 &rh) { return __hbneu2(lh, rh); }
-__device__ __forceinline__ bool operator>(const __half2 &lh, const __half2 &rh) { return __hbgt2(lh, rh); }
-__device__ __forceinline__ bool operator<(const __half2 &lh, const __half2 &rh) { return __hblt2(lh, rh); }
-__device__ __forceinline__ bool operator>=(const __half2 &lh, const __half2 &rh) { return __hbge2(lh, rh); }
-__device__ __forceinline__ bool operator<=(const __half2 &lh, const __half2 &rh) { return __hble2(lh, rh); }
+__device__ __forceinline__ bool operator==(const __half2 &lh, const __half2 &rh) { __half2 res = __heq2(lh, rh); return (res.x && res.y); }
+__device__ __forceinline__ bool operator!=(const __half2 &lh, const __half2 &rh) { __half2 res = __hne2(lh, rh); return (res.x && res.y); }
+__device__ __forceinline__ bool operator>(const __half2 &lh, const __half2 &rh) { __half2 res = __hgt2(lh, rh); return (res.x && res.y); }
+__device__ __forceinline__ bool operator<(const __half2 &lh, const __half2 &rh) { __half2 res = __hlt2(lh, rh); return (res.x && res.y); }
+__device__ __forceinline__ bool operator>=(const __half2 &lh, const __half2 &rh) { __half2 res = __hge2(lh, rh); return (res.x && res.y); }
+__device__ __forceinline__ bool operator<=(const __half2 &lh, const __half2 &rh) { __half2 res = __hle2(lh, rh); return (res.x && res.y); }
 
 #endif /* __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__) */
 #endif /* defined(__CUDACC__) */
 
 /* Restore warning for multiple assignment operators */
 #if defined(_MSC_VER) && _MSC_VER >= 1500
 #pragma warning( pop )
-#endif /* defined(_MSC_VER) && _MSC_VER >= 1500 */
+#endif
 
 /* Restore -Weffc++ warnings from here on */
 #if defined(__GNUC__)
 #if __GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6)
 #pragma GCC diagnostic pop
 #endif /* __GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6) */
 #endif /* defined(__GNUC__) */
 
 #undef __CUDA_HOSTDEVICE__
 #undef __CUDA_ALIGN__
 
 #ifndef __CUDACC_RTC__  /* no host functions in NVRTC mode */
-static inline unsigned short __internal_float2half(const float f, unsigned int &sign, unsigned int &remainder)
+static unsigned short __internal_float2half(float f, unsigned int &sign, unsigned int &remainder)
 {
-    unsigned int x;
-    unsigned int u;
-    unsigned int result;
-#if defined(__CUDACC__)
-    (void)memcpy(&x, &f, sizeof(f));
-#else
-    (void)std::memcpy(&x, &f, sizeof(f));
-#endif
+    unsigned int x, u, shift, exponent, mantissa;
+    memcpy(&x, &f, sizeof(f));
     u = (x & 0x7fffffffU);
-    sign = ((x >> 16U) & 0x8000U);
+    sign = ((x >> 16) & 0x8000U);
     // NaN/+Inf/-Inf
     if (u >= 0x7f800000U) {
-        remainder = 0U;
-        result = ((u == 0x7f800000U) ? (sign | 0x7c00U) : 0x7fffU);
-    } else if (u > 0x477fefffU) { // Overflows
+        remainder = 0;
+        return static_cast<unsigned short>((u == 0x7f800000U) ? (sign | 0x7c00U) : 0x7fffU);
+    }
+    // Overflows
+    if (u > 0x477fefffU) {
         remainder = 0x80000000U;
-        result = (sign | 0x7bffU);
-    } else if (u >= 0x38800000U) { // Normal numbers
-        remainder = u << 19U;
+        return static_cast<unsigned short>(sign | 0x7bffU);
+    }
+    // Normal numbers
+    if (u >= 0x38800000U) {
+        remainder = u << 19;
         u -= 0x38000000U;
-        result = (sign | (u >> 13U));
-    } else if (u < 0x33000001U) { // +0/-0
+        return static_cast<unsigned short>(sign | (u >> 13));
+    }
+    // +0/-0
+    if (u < 0x33000001U) {
         remainder = u;
-        result = sign;
-    } else { // Denormal numbers
-        const unsigned int exponent = u >> 23U;
-        const unsigned int shift = 0x7eU - exponent;
-        unsigned int mantissa = (u & 0x7fffffU);
-        mantissa |= 0x800000U;
-        remainder = mantissa << (32U - shift);
-        result = (sign | (mantissa >> shift));
+        return static_cast<unsigned short>(sign);
     }
-    return static_cast<unsigned short>(result);
+    // Denormal numbers
+    exponent = u >> 23;
+    mantissa = (u & 0x7fffffU);
+    shift = 0x7eU - exponent;
+    mantissa |= 0x800000U;
+    remainder = mantissa << (32 - shift);
+    return static_cast<unsigned short>(sign | (mantissa >> shift));
 }
 #endif  /* #if !defined(__CUDACC_RTC__) */
 
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __double2half(const double a)
-{
-#if defined(__CUDA_ARCH__)
-    __half val;
-    asm("{  cvt.rn.f16.f64 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "d"(a));
-    return val;
-#else
-    __half result;
-    // Perform rounding to 11 bits of precision, convert value
-    // to float and call existing float to half conversion.
-    // By pre-rounding to 11 bits we avoid additional rounding
-    // in float to half conversion.
-    unsigned long long int absa;
-    unsigned long long int ua;
-    #if defined(__CUDACC__)
-        (void)memcpy(&ua, &a, sizeof(a));
-    #else
-        (void)std::memcpy(&ua, &a, sizeof(a));
-    #endif
-    absa = (ua & 0x7fffffffffffffffULL);
-    if ((absa >= 0x40f0000000000000ULL) || (absa <= 0x3e60000000000000ULL))
-    {
-        // |a| >= 2^16 or NaN or |a| <= 2^(-25)
-        // double-rounding is not a problem
-        result = __float2half(static_cast<float>(a));
-    }
-    else
-    {
-        // here 2^(-25) < |a| < 2^16
-        // prepare shifter value such that a + shifter
-        // done in double precision performs round-to-nearest-even
-        // and (a + shifter) - shifter results in a rounded to
-        // 11 bits of precision. Shifter needs to have exponent of
-        // a plus 53 - 11 = 42 and a leading bit in mantissa to guard
-        // against negative values.
-        // So need to have |a| capped to avoid overflow in exponent.
-        // For inputs that are smaller than half precision minnorm
-        // we prepare fixed shifter exponent.
-        unsigned long long shifterBits;
-        if (absa >= 0x3f10000000000000ULL)
-        {   // Here if |a| >= 2^(-14)
-            // add 42 to exponent bits
-            shifterBits  = (ua & 0x7ff0000000000000ULL) + 0x02A0000000000000ULL;
-        }
-        else
-        {   // 2^(-25) < |a| < 2^(-14), potentially results in denormal
-            // set exponent bits to 42 - 14 + bias
-            shifterBits = 0x41B0000000000000ULL;
-        }
-        // set leading mantissa bit to protect against negative inputs
-        shifterBits |= 0x0008000000000000ULL;
-        double shifter;
-        #if defined(__CUDACC__)
-            (void)memcpy(&shifter, &shifterBits, sizeof(shifterBits));
-        #else
-            (void)std::memcpy(&shifter, &shifterBits, sizeof(shifterBits));
-        #endif
-        double aShiftRound = a + shifter;
-
-        // Prevent the compiler from optimizing away a + shifter - shifter
-        // by doing intermediate memcopy and harmless bitwize operation
-        unsigned long long int aShiftRoundBits;
-        #if defined(__CUDACC__)
-            (void)memcpy(&aShiftRoundBits, &aShiftRound, sizeof(aShiftRound));
-        #else
-            (void)std::memcpy(&aShiftRoundBits, &aShiftRound, sizeof(aShiftRound));
-        #endif
-
-        // the value is positive, so this operation doesn't change anything
-        aShiftRoundBits &= 0x7fffffffffffffffULL;
-
-        #if defined(__CUDACC__)
-            (void)memcpy(&aShiftRound, &aShiftRoundBits, sizeof(aShiftRound));
-        #else
-            (void)std::memcpy(&aShiftRound, &aShiftRoundBits, sizeof(aShiftRound));
-        #endif
-
-        result = __float2half(static_cast<float>(aShiftRound - shifter));
-    }
-
-    return result;
-#endif
-}
-
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half(const float a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half(const float f)
 {
     __half val;
 #if defined(__CUDA_ARCH__)
-    asm("{  cvt.rn.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(a));
+    asm("{  cvt.rn.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(f));
 #else
     __half_raw r;
-    unsigned int sign = 0U;
-    unsigned int remainder = 0U;
-    r.x = __internal_float2half(a, sign, remainder);
-    if ((remainder > 0x80000000U) || ((remainder == 0x80000000U) && ((r.x & 0x1U) != 0U))) {
+    unsigned int sign, remainder;
+    r.x = __internal_float2half(f, sign, remainder);
+    if (remainder > 0x80000000U || (remainder == 0x80000000U && (r.x & 0x1)))
         r.x++;
-    }
     val = r;
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_rn(const float a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_rn(const float f)
 {
     __half val;
 #if defined(__CUDA_ARCH__)
-    asm("{  cvt.rn.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(a));
+    asm("{  cvt.rn.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(f));
 #else
     __half_raw r;
-    unsigned int sign = 0U;
-    unsigned int remainder = 0U;
-    r.x = __internal_float2half(a, sign, remainder);
-    if ((remainder > 0x80000000U) || ((remainder == 0x80000000U) && ((r.x & 0x1U) != 0U))) {
+    unsigned int sign, remainder;
+    r.x = __internal_float2half(f, sign, remainder);
+    if (remainder > 0x80000000U || (remainder == 0x80000000U && (r.x & 0x1)))
         r.x++;
-    }
     val = r;
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_rz(const float a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_rz(const float f)
 {
     __half val;
 #if defined(__CUDA_ARCH__)
-    asm("{  cvt.rz.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(a));
+    asm("{  cvt.rz.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(f));
 #else
     __half_raw r;
-    unsigned int sign = 0U;
-    unsigned int remainder = 0U;
-    r.x = __internal_float2half(a, sign, remainder);
+    unsigned int sign, remainder;
+    r.x = __internal_float2half(f, sign, remainder);
     val = r;
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_rd(const float a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_rd(const float f)
 {
     __half val;
 #if defined(__CUDA_ARCH__)
-    asm("{  cvt.rm.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(a));
+    asm("{  cvt.rm.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(f));
 #else
     __half_raw r;
-    unsigned int sign = 0U;
-    unsigned int remainder = 0U;
-    r.x = __internal_float2half(a, sign, remainder);
-    if ((remainder != 0U) && (sign != 0U)) {
+    unsigned int sign, remainder;
+    r.x = __internal_float2half(f, sign, remainder);
+    if (remainder && sign)
         r.x++;
-    }
     val = r;
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_ru(const float a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half __float2half_ru(const float f)
 {
     __half val;
 #if defined(__CUDA_ARCH__)
-    asm("{  cvt.rp.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(a));
+    asm("{  cvt.rp.f16.f32 %0, %1;}\n" : "=h"(__HALF_TO_US(val)) : "f"(f));
 #else
     __half_raw r;
-    unsigned int sign = 0U;
-    unsigned int remainder = 0U;
-    r.x = __internal_float2half(a, sign, remainder);
-    if ((remainder != 0U) && (sign == 0U)) {
+    unsigned int sign, remainder;
+    r.x = __internal_float2half(f, sign, remainder);
+    if (remainder && !sign)
         r.x++;
-    }
     val = r;
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half2 __float2half2_rn(const float a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half2 __float2half2_rn(const float f)
 {
     __half2 val;
 #if defined(__CUDA_ARCH__)
     asm("{.reg .f16 low;\n"
         "  cvt.rn.f16.f32 low, %1;\n"
-        "  mov.b32 %0, {low,low};}\n" : "=r"(__HALF2_TO_UI(val)) : "f"(a));
+        "  mov.b32 %0, {low,low};}\n" : "=r"(__HALF2_TO_UI(val)) : "f"(f));
 #else
-    val = __half2(__float2half_rn(a), __float2half_rn(a));
+    val = __half2(__float2half_rn(f), __float2half_rn(f));
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half2 __floats2half2_rn(const float a, const float b)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half2 __floats2half2_rn(const float f1, const float f2)
 {
     __half2 val;
 #if defined(__CUDA_ARCH__)
     asm("{.reg .f16 low,high;\n"
         "  cvt.rn.f16.f32 low, %1;\n"
         "  cvt.rn.f16.f32 high, %2;\n"
-        "  mov.b32 %0, {low,high};}\n" : "=r"(__HALF2_TO_UI(val)) : "f"(a), "f"(b));
+        "  mov.b32 %0, {low,high};}\n" : "=r"(__HALF2_TO_UI(val)) : "f"(f1), "f"(f2));
 #else
-    val = __half2(__float2half_rn(a), __float2half_rn(b));
+    val = __half2(__float2half_rn(f1), __float2half_rn(f2));
 #endif
     return val;
 }
 
 #ifndef __CUDACC_RTC__  /* no host functions in NVRTC mode */
-static inline float __internal_half2float(const unsigned short h)
+static float __internal_half2float(unsigned short h)
 {
-    unsigned int sign = ((static_cast<unsigned int>(h) >> 15U) & 1U);
-    unsigned int exponent = ((static_cast<unsigned int>(h) >> 10U) & 0x1fU);
-    unsigned int mantissa = ((static_cast<unsigned int>(h) & 0x3ffU) << 13U);
+    unsigned int sign = ((h >> 15) & 1);
+    unsigned int exponent = ((h >> 10) & 0x1f);
+    unsigned int mantissa = ((h & 0x3ff) << 13);
     float f;
     if (exponent == 0x1fU) { /* NaN or Inf */
-        /* discard sign of a NaN */
-        sign = ((mantissa != 0U) ? (sign >> 1U) : sign);
-        mantissa = ((mantissa != 0U) ? 0x7fffffU : 0U);
+        mantissa = (mantissa ? (sign = 0, 0x7fffffU) : 0);
         exponent = 0xffU;
-    } else if (exponent == 0U) { /* Denorm or Zero */
-        if (mantissa != 0U) {
+    } else if (!exponent) { /* Denorm or Zero */
+        if (mantissa) {
             unsigned int msb;
             exponent = 0x71U;
             do {
                 msb = (mantissa & 0x400000U);
-                mantissa <<= 1U; /* normalize */
+                mantissa <<= 1; /* normalize */
                 --exponent;
-            } while (msb == 0U);
+            } while (!msb);
             mantissa &= 0x7fffffU; /* 1.mantissa is implicit */
         }
     } else {
         exponent += 0x70U;
     }
-    unsigned int u = ((sign << 31U) | (exponent << 23U) | mantissa);
-#if defined(__CUDACC__)
-    (void)memcpy(&f, &u, sizeof(u));
-#else
-    (void)std::memcpy(&f, &u, sizeof(u));
-#endif
+    unsigned int u = ((sign << 31) | (exponent << 23) | mantissa);
+    memcpy(&f, &u, sizeof(u));
     return f;
 }
 #endif  /* !defined(__CUDACC_RTC__) */
 
-__CUDA_HOSTDEVICE_FP16_DECL__ float __half2float(const __half a)
+__CUDA_HOSTDEVICE_FP16_DECL__ float __half2float(const __half h)
 {
     float val;
 #if defined(__CUDA_ARCH__)
-    asm("{  cvt.f32.f16 %0, %1;}\n" : "=f"(val) : "h"(__HALF_TO_CUS(a)));
+    asm("{  cvt.f32.f16 %0, %1;}\n" : "=f"(val) : "h"(__HALF_TO_CUS(h)));
 #else
-    val = __internal_half2float(static_cast<__half_raw>(a).x);
+    val = __internal_half2float(static_cast<__half_raw>(h).x);
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ float __low2float(const __half2 a)
+__CUDA_HOSTDEVICE_FP16_DECL__ float __low2float(const __half2 l)
 {
     float val;
 #if defined(__CUDA_ARCH__)
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high},%1;\n"
-        "  cvt.f32.f16 %0, low;}\n" : "=f"(val) : "r"(__HALF2_TO_CUI(a)));
+        "  cvt.f32.f16 %0, low;}\n" : "=f"(val) : "r"(__HALF2_TO_CUI(l)));
 #else
-    val = __internal_half2float(static_cast<__half2_raw>(a).x);
+    val = __internal_half2float(static_cast<__half2_raw>(l).x);
 #endif
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ float __high2float(const __half2 a)
+__CUDA_HOSTDEVICE_FP16_DECL__ float __high2float(const __half2 l)
 {
     float val;
 #if defined(__CUDA_ARCH__)
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high},%1;\n"
-        "  cvt.f32.f16 %0, high;}\n" : "=f"(val) : "r"(__HALF2_TO_CUI(a)));
+        "  cvt.f32.f16 %0, high;}\n" : "=f"(val) : "r"(__HALF2_TO_CUI(l)));
 #else
-    val = __internal_half2float(static_cast<__half2_raw>(a).y);
+    val = __internal_half2float(static_cast<__half2_raw>(l).y);
 #endif
     return val;
 }
 
 /* Intrinsic functions only available to nvcc compilers */
 #if defined(__CUDACC__)
 
 /* CUDA vector-types compatible vector creation function (note returns __half2, not half2) */
-__VECTOR_FUNCTIONS_DECL__ __half2 make_half2(const __half x, const __half y)
+__VECTOR_FUNCTIONS_DECL__ __half2 make_half2(__half x, __half y)
 {
     __half2 t; t.x = x; t.y = y; return t;
 }
 #undef __VECTOR_FUNCTIONS_DECL__
 
 
 /* Definitions of intrinsics */
-__CUDA_HOSTDEVICE_FP16_DECL__ __half2 __float22half2_rn(const float2 a)
+__CUDA_HOSTDEVICE_FP16_DECL__ __half2 __float22half2_rn(const float2 f)
 {
-    const __half2 val = __floats2half2_rn(a.x, a.y);
+    __half2 val = __floats2half2_rn(f.x, f.y);
     return val;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ float2 __half22float2(const __half2 a)
+__CUDA_HOSTDEVICE_FP16_DECL__ float2 __half22float2(const __half2 l)
 {
     float hi_float;
     float lo_float;
 #if defined(__CUDA_ARCH__)
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high},%1;\n"
-        "  cvt.f32.f16 %0, low;}\n" : "=f"(lo_float) : "r"(__HALF2_TO_CUI(a)));
+        "  cvt.f32.f16 %0, low;}\n" : "=f"(lo_float) : "r"(__HALF2_TO_CUI(l)));
 
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high},%1;\n"
-        "  cvt.f32.f16 %0, high;}\n" : "=f"(hi_float) : "r"(__HALF2_TO_CUI(a)));
+        "  cvt.f32.f16 %0, high;}\n" : "=f"(hi_float) : "r"(__HALF2_TO_CUI(l)));
 #else
-    lo_float = __internal_half2float(((__half2_raw)a).x);
-    hi_float = __internal_half2float(((__half2_raw)a).y);
+    lo_float = __internal_half2float(((__half2_raw)l).x);
+    hi_float = __internal_half2float(((__half2_raw)l).y);
 #endif
     return make_float2(lo_float, hi_float);
 }
-__CUDA_FP16_DECL__ int __half2int_rn(const __half h)
+__CUDA_FP16_DECL__ int __half2int_rn(__half h)
 {
     int i;
-    asm("cvt.rni.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rni.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ int __half2int_rz(const __half h)
+__CUDA_FP16_DECL__ int __half2int_rz(__half h)
 {
     int i;
-#if defined __CUDA_ARCH__
-    asm("cvt.rzi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
-#else
-    const float f = __half2float(h);
-                i = static_cast<int>(f);
-    const int max_val = (int)0x7fffffffU;
-    const int min_val = (int)0x80000000U;
-    // saturation fixup
-    if (f != f) {
-        // NaN
-        i = 0;
-    } else if (f > static_cast<float>(max_val)) {
-        // saturate maximum
-        i = max_val;
-    } else if (f < static_cast<float>(min_val)) {
-        // saturate minimum
-        i = min_val;
-    }
-#endif
+    asm("cvt.rzi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ int __half2int_rd(const __half h)
+__CUDA_FP16_DECL__ int __half2int_rd(__half h)
 {
     int i;
-    asm("cvt.rmi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rmi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ int __half2int_ru(const __half h)
+__CUDA_FP16_DECL__ int __half2int_ru(__half h)
 {
     int i;
-    asm("cvt.rpi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rpi.s32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __int2half_rn(const int i)
+__CUDA_FP16_DECL__ __half __int2half_rn(int i)
 {
     __half h;
-#if defined(__CUDA_ARCH__)
     asm("cvt.rn.f16.s32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
-#else
-    // double-rounding is not a problem here: if integer
-    // has more than 24 bits, it is already too large to
-    // be represented in half precision, and result will
-    // be infinity.
-    const float  f = static_cast<float>(i);
-                 h = __float2half_rn(f);
-#endif
     return h;
 }
-__CUDA_FP16_DECL__ __half __int2half_rz(const int i)
+__CUDA_FP16_DECL__ __half __int2half_rz(int i)
 {
     __half h;
     asm("cvt.rz.f16.s32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __int2half_rd(const int i)
+__CUDA_FP16_DECL__ __half __int2half_rd(int i)
 {
     __half h;
     asm("cvt.rm.f16.s32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __int2half_ru(const int i)
+__CUDA_FP16_DECL__ __half __int2half_ru(int i)
 {
     __half h;
     asm("cvt.rp.f16.s32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
     return h;
 }
 
-__CUDA_FP16_DECL__ short int __half2short_rn(const __half h)
+__CUDA_FP16_DECL__ short int __half2short_rn(__half h)
 {
     short int i;
-    asm("cvt.rni.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rni.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ short int __half2short_rz(const __half h)
+__CUDA_FP16_DECL__ short int __half2short_rz(__half h)
 {
     short int i;
-#if defined __CUDA_ARCH__
-    asm("cvt.rzi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
-#else
-    const float f = __half2float(h);
-                i = static_cast<short int>(f);
-    const short int max_val = (short int)0x7fffU;
-    const short int min_val = (short int)0x8000U;
-    // saturation fixup
-    if (f != f) {
-        // NaN
-        i = 0;
-    } else if (f > static_cast<float>(max_val)) {
-        // saturate maximum
-        i = max_val;
-    } else if (f < static_cast<float>(min_val)) {
-        // saturate minimum
-        i = min_val;
-    }
-#endif
+    asm("cvt.rzi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ short int __half2short_rd(const __half h)
+__CUDA_FP16_DECL__ short int __half2short_rd(__half h)
 {
     short int i;
-    asm("cvt.rmi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rmi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ short int __half2short_ru(const __half h)
+__CUDA_FP16_DECL__ short int __half2short_ru(__half h)
 {
     short int i;
-    asm("cvt.rpi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rpi.s16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __short2half_rn(const short int i)
+__CUDA_FP16_DECL__ __half __short2half_rn(short int i)
 {
     __half h;
-#if defined __CUDA_ARCH__
     asm("cvt.rn.f16.s16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
-#else
-    const float  f = static_cast<float>(i);
-                 h = __float2half_rn(f);
-#endif
     return h;
 }
-__CUDA_FP16_DECL__ __half __short2half_rz(const short int i)
+__CUDA_FP16_DECL__ __half __short2half_rz(short int i)
 {
     __half h;
     asm("cvt.rz.f16.s16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __short2half_rd(const short int i)
+__CUDA_FP16_DECL__ __half __short2half_rd(short int i)
 {
     __half h;
     asm("cvt.rm.f16.s16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __short2half_ru(const short int i)
+__CUDA_FP16_DECL__ __half __short2half_ru(short int i)
 {
     __half h;
     asm("cvt.rp.f16.s16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
     return h;
 }
 
-__CUDA_FP16_DECL__ unsigned int __half2uint_rn(const __half h)
+__CUDA_FP16_DECL__ unsigned int __half2uint_rn(__half h)
 {
     unsigned int i;
-    asm("cvt.rni.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rni.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ unsigned int __half2uint_rz(const __half h)
+__CUDA_FP16_DECL__ unsigned int __half2uint_rz(__half h)
 {
     unsigned int i;
-#if defined __CUDA_ARCH__
-    asm("cvt.rzi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
-#else
-    const float f = __half2float(h);
-                i = static_cast<unsigned int>(f);
-    const unsigned int max_val = 0xffffffffU;
-    const unsigned int min_val = 0U;
-    // saturation fixup
-    if (f != f) {
-        // NaN
-        i = 0U;
-    } else if (f > static_cast<float>(max_val)) {
-        // saturate maximum
-        i = max_val;
-    } else if (f < static_cast<float>(min_val)) {
-        // saturate minimum
-        i = min_val;
-    }
-#endif
+    asm("cvt.rzi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ unsigned int __half2uint_rd(const __half h)
+__CUDA_FP16_DECL__ unsigned int __half2uint_rd(__half h)
 {
     unsigned int i;
-    asm("cvt.rmi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rmi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ unsigned int __half2uint_ru(const __half h)
+__CUDA_FP16_DECL__ unsigned int __half2uint_ru(__half h)
 {
     unsigned int i;
-    asm("cvt.rpi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rpi.u32.f16 %0, %1;" : "=r"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __uint2half_rn(const unsigned int i)
+__CUDA_FP16_DECL__ __half __uint2half_rn(unsigned int i)
 {
     __half h;
-#if defined __CUDA_ARCH__
     asm("cvt.rn.f16.u32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
-#else
-    // double-rounding is not a problem here: if integer
-    // has more than 24 bits, it is already too large to
-    // be represented in half precision, and result will
-    // be infinity.
-    const float  f = static_cast<float>(i);
-                 h = __float2half_rn(f);
-#endif
     return h;
 }
-__CUDA_FP16_DECL__ __half __uint2half_rz(const unsigned int i)
+__CUDA_FP16_DECL__ __half __uint2half_rz(unsigned int i)
 {
     __half h;
     asm("cvt.rz.f16.u32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __uint2half_rd(const unsigned int i)
+__CUDA_FP16_DECL__ __half __uint2half_rd(unsigned int i)
 {
     __half h;
     asm("cvt.rm.f16.u32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __uint2half_ru(const unsigned int i)
+__CUDA_FP16_DECL__ __half __uint2half_ru(unsigned int i)
 {
     __half h;
     asm("cvt.rp.f16.u32 %0, %1;" : "=h"(__HALF_TO_US(h)) : "r"(i));
     return h;
 }
 
-__CUDA_FP16_DECL__ unsigned short int __half2ushort_rn(const __half h)
+__CUDA_FP16_DECL__ unsigned short int __half2ushort_rn(__half h)
 {
     unsigned short int i;
-    asm("cvt.rni.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rni.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ unsigned short int __half2ushort_rz(const __half h)
+__CUDA_FP16_DECL__ unsigned short int __half2ushort_rz(__half h)
 {
     unsigned short int i;
-#if defined __CUDA_ARCH__
-    asm("cvt.rzi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
-#else
-    const float f = __half2float(h);
-                i = static_cast<unsigned short int>(f);
-    const unsigned short int max_val = 0xffffU;
-    const unsigned short int min_val = 0U;
-    // saturation fixup
-    if (f != f) {
-        // NaN
-        i = 0U;
-    } else if (f > static_cast<float>(max_val)) {
-        // saturate maximum
-        i = max_val;
-    } else if (f < static_cast<float>(min_val)) {
-        // saturate minimum
-        i = min_val;
-    }
-#endif
+    asm("cvt.rzi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ unsigned short int __half2ushort_rd(const __half h)
+__CUDA_FP16_DECL__ unsigned short int __half2ushort_rd(__half h)
 {
     unsigned short int i;
-    asm("cvt.rmi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rmi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ unsigned short int __half2ushort_ru(const __half h)
+__CUDA_FP16_DECL__ unsigned short int __half2ushort_ru(__half h)
 {
     unsigned short int i;
-    asm("cvt.rpi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rpi.u16.f16 %0, %1;" : "=h"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __ushort2half_rn(const unsigned short int i)
+__CUDA_FP16_DECL__ __half __ushort2half_rn(unsigned short int i)
 {
     __half h;
-#if defined __CUDA_ARCH__
     asm("cvt.rn.f16.u16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
-#else
-    const float  f = static_cast<float>(i);
-                 h = __float2half_rn(f);
-#endif
     return h;
 }
-__CUDA_FP16_DECL__ __half __ushort2half_rz(const unsigned short int i)
+__CUDA_FP16_DECL__ __half __ushort2half_rz(unsigned short int i)
 {
     __half h;
     asm("cvt.rz.f16.u16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __ushort2half_rd(const unsigned short int i)
+__CUDA_FP16_DECL__ __half __ushort2half_rd(unsigned short int i)
 {
     __half h;
     asm("cvt.rm.f16.u16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __ushort2half_ru(const unsigned short int i)
+__CUDA_FP16_DECL__ __half __ushort2half_ru(unsigned short int i)
 {
     __half h;
     asm("cvt.rp.f16.u16 %0, %1;" : "=h"(__HALF_TO_US(h)) : "h"(i));
     return h;
 }
 
-__CUDA_FP16_DECL__ unsigned long long int __half2ull_rn(const __half h)
+__CUDA_FP16_DECL__ unsigned long long int __half2ull_rn(__half h)
 {
     unsigned long long int i;
-    asm("cvt.rni.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rni.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ unsigned long long int __half2ull_rz(const __half h)
+__CUDA_FP16_DECL__ unsigned long long int __half2ull_rz(__half h)
 {
     unsigned long long int i;
-#if defined __CUDA_ARCH__
-    asm("cvt.rzi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
-#else
-    const float f = __half2float(h);
-                i = static_cast<unsigned long long int>(f);
-    const unsigned long long int max_val = 0xffffffffffffffffULL;
-    const unsigned long long int min_val = 0ULL;
-    // saturation fixup
-    if (f != f) {
-        // NaN
-        i = 0x8000000000000000ULL;
-    } else if (f > static_cast<float>(max_val)) {
-        // saturate maximum
-        i = max_val;
-    } else if (f < static_cast<float>(min_val)) {
-        // saturate minimum
-        i = min_val;
-    }
-#endif
+    asm("cvt.rzi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ unsigned long long int __half2ull_rd(const __half h)
+__CUDA_FP16_DECL__ unsigned long long int __half2ull_rd(__half h)
 {
     unsigned long long int i;
-    asm("cvt.rmi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rmi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ unsigned long long int __half2ull_ru(const __half h)
+__CUDA_FP16_DECL__ unsigned long long int __half2ull_ru(__half h)
 {
     unsigned long long int i;
-    asm("cvt.rpi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rpi.u64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __ull2half_rn(const unsigned long long int i)
+__CUDA_FP16_DECL__ __half __ull2half_rn(unsigned long long int i)
 {
     __half h;
-#if defined(__CUDA_ARCH__)
     asm("cvt.rn.f16.u64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
-#else
-    // double-rounding is not a problem here: if integer
-    // has more than 24 bits, it is already too large to
-    // be represented in half precision, and result will
-    // be infinity.
-    const float  f = static_cast<float>(i);
-                 h = __float2half_rn(f);
-#endif
     return h;
 }
-__CUDA_FP16_DECL__ __half __ull2half_rz(const unsigned long long int i)
+__CUDA_FP16_DECL__ __half __ull2half_rz(unsigned long long int i)
 {
     __half h;
     asm("cvt.rz.f16.u64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __ull2half_rd(const unsigned long long int i)
+__CUDA_FP16_DECL__ __half __ull2half_rd(unsigned long long int i)
 {
     __half h;
     asm("cvt.rm.f16.u64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __ull2half_ru(const unsigned long long int i)
+__CUDA_FP16_DECL__ __half __ull2half_ru(unsigned long long int i)
 {
     __half h;
     asm("cvt.rp.f16.u64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
     return h;
 }
 
-__CUDA_FP16_DECL__ long long int __half2ll_rn(const __half h)
+__CUDA_FP16_DECL__ long long int __half2ll_rn(__half h)
 {
     long long int i;
-    asm("cvt.rni.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rni.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ long long int __half2ll_rz(const __half h)
+__CUDA_FP16_DECL__ long long int __half2ll_rz(__half h)
 {
     long long int i;
-#if defined __CUDA_ARCH__
-    asm("cvt.rzi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
-#else
-    const float f = __half2float(h);
-                i = static_cast<long long int>(f);
-    const long long int max_val = (long long int)0x7fffffffffffffffULL;
-    const long long int min_val = (long long int)0x8000000000000000ULL;
-    // saturation fixup
-    if (f != f) {
-        // NaN
-        i = min_val;
-    } else if (f > static_cast<float>(max_val)) {
-        // saturate maximum
-        i = max_val;
-    } else if (f < static_cast<float>(min_val)) {
-        // saturate minimum
-        i = min_val;
-    }
-#endif
+    asm("cvt.rzi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ long long int __half2ll_rd(const __half h)
+__CUDA_FP16_DECL__ long long int __half2ll_rd(__half h)
 {
     long long int i;
-    asm("cvt.rmi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rmi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_FP16_DECL__ long long int __half2ll_ru(const __half h)
+__CUDA_FP16_DECL__ long long int __half2ll_ru(__half h)
 {
     long long int i;
-    asm("cvt.rpi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_CUS(h)));
+    asm("cvt.rpi.s64.f16 %0, %1;" : "=l"(i) : "h"(__HALF_TO_US(h)));
     return i;
 }
-__CUDA_HOSTDEVICE_FP16_DECL__ __half __ll2half_rn(const long long int i)
+__CUDA_FP16_DECL__ __half __ll2half_rn(long long int i)
 {
     __half h;
-#if defined(__CUDA_ARCH__)
     asm("cvt.rn.f16.s64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
-#else
-    // double-rounding is not a problem here: if integer
-    // has more than 24 bits, it is already too large to
-    // be represented in half precision, and result will
-    // be infinity.
-    const float  f = static_cast<float>(i);
-                 h = __float2half_rn(f);
-#endif
     return h;
 }
-__CUDA_FP16_DECL__ __half __ll2half_rz(const long long int i)
+__CUDA_FP16_DECL__ __half __ll2half_rz(long long int i)
 {
     __half h;
     asm("cvt.rz.f16.s64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __ll2half_rd(const long long int i)
+__CUDA_FP16_DECL__ __half __ll2half_rd(long long int i)
 {
     __half h;
     asm("cvt.rm.f16.s64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
     return h;
 }
-__CUDA_FP16_DECL__ __half __ll2half_ru(const long long int i)
+__CUDA_FP16_DECL__ __half __ll2half_ru(long long int i)
 {
     __half h;
     asm("cvt.rp.f16.s64 %0, %1;" : "=h"(__HALF_TO_US(h)) : "l"(i));
     return h;
 }
 
 __CUDA_FP16_DECL__ __half htrunc(const __half h)
@@ -1242,655 +913,612 @@
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high}, %1;\n"
         "  cvt.rni.f16.f16 low, low;\n"
         "  cvt.rni.f16.f16 high, high;\n"
         "  mov.b32 %0, {low,high};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(h)));
     return val;
 }
-__CUDA_FP16_DECL__ __half2 __lows2half2(const __half2 a, const __half2 b)
+__CUDA_FP16_DECL__ __half2 __lows2half2(const __half2 l, const __half2 h)
 {
     __half2 val;
     asm("{.reg .f16 alow,ahigh,blow,bhigh;\n"
         "  mov.b32 {alow,ahigh}, %1;\n"
         "  mov.b32 {blow,bhigh}, %2;\n"
-        "  mov.b32 %0, {alow,blow};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)), "r"(__HALF2_TO_CUI(b)));
+        "  mov.b32 %0, {alow,blow};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(l)), "r"(__HALF2_TO_CUI(h)));
     return val;
 }
-__CUDA_FP16_DECL__ __half2 __highs2half2(const __half2 a, const __half2 b)
+__CUDA_FP16_DECL__ __half2 __highs2half2(const __half2 l, const __half2 h)
 {
     __half2 val;
     asm("{.reg .f16 alow,ahigh,blow,bhigh;\n"
         "  mov.b32 {alow,ahigh}, %1;\n"
         "  mov.b32 {blow,bhigh}, %2;\n"
-        "  mov.b32 %0, {ahigh,bhigh};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)), "r"(__HALF2_TO_CUI(b)));
+        "  mov.b32 %0, {ahigh,bhigh};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(l)), "r"(__HALF2_TO_CUI(h)));
     return val;
 }
-__CUDA_FP16_DECL__ __half __low2half(const __half2 a)
+__CUDA_FP16_DECL__ __half __low2half(const __half2 h)
 {
     __half ret;
     asm("{.reg .f16 low,high;\n"
         " mov.b32 {low,high}, %1;\n"
-        " mov.b16 %0, low;}" : "=h"(__HALF_TO_US(ret)) : "r"(__HALF2_TO_CUI(a)));
+        " mov.b16 %0, low;}" : "=h"(__HALF_TO_US(ret)) : "r"(__HALF2_TO_CUI(h)));
     return ret;
 }
 __CUDA_FP16_DECL__ int __hisinf(const __half a)
 {
-    int retval;
-    if (__HALF_TO_CUS(a) == 0xFC00U) {
-        retval = -1;
-    } else if (__HALF_TO_CUS(a) == 0x7C00U) {
-        retval = 1;
-    } else {
-        retval = 0;
-    }
-    return retval;
+    if (__HALF_TO_CUS(a) == 0xFC00)
+        return -1;
+    if (__HALF_TO_CUS(a) == 0x7C00)
+        return 1;
+    return 0;
 }
-__CUDA_FP16_DECL__ __half2 __low2half2(const __half2 a)
+__CUDA_FP16_DECL__ __half2 __low2half2(const __half2 l)
 {
     __half2 val;
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high}, %1;\n"
-        "  mov.b32 %0, {low,low};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
+        "  mov.b32 %0, {low,low};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(l)));
     return val;
 }
-__CUDA_FP16_DECL__ __half2 __high2half2(const __half2 a)
+__CUDA_FP16_DECL__ __half2 __high2half2(const __half2 l)
 {
     __half2 val;
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high}, %1;\n"
-        "  mov.b32 %0, {high,high};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
+        "  mov.b32 %0, {high,high};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(l)));
     return val;
 }
-__CUDA_FP16_DECL__ __half __high2half(const __half2 a)
+__CUDA_FP16_DECL__ __half __high2half(const __half2 h)
 {
     __half ret;
     asm("{.reg .f16 low,high;\n"
         " mov.b32 {low,high}, %1;\n"
-        " mov.b16 %0, high;}" : "=h"(__HALF_TO_US(ret)) : "r"(__HALF2_TO_CUI(a)));
+        " mov.b16 %0, high;}" : "=h"(__HALF_TO_US(ret)) : "r"(__HALF2_TO_CUI(h)));
     return ret;
 }
-__CUDA_FP16_DECL__ __half2 __halves2half2(const __half a, const __half b)
+__CUDA_FP16_DECL__ __half2 __halves2half2(const __half l, const __half h)
 {
     __half2 val;
     asm("{  mov.b32 %0, {%1,%2};}\n"
-        : "=r"(__HALF2_TO_UI(val)) : "h"(__HALF_TO_CUS(a)), "h"(__HALF_TO_CUS(b)));
+        : "=r"(__HALF2_TO_UI(val)) : "h"(__HALF_TO_CUS(l)), "h"(__HALF_TO_CUS(h)));
     return val;
 }
-__CUDA_FP16_DECL__ __half2 __half2half2(const __half a)
+__CUDA_FP16_DECL__ __half2 __half2half2(const __half lh)
 {
     __half2 val;
     asm("{  mov.b32 %0, {%1,%1};}\n"
-        : "=r"(__HALF2_TO_UI(val)) : "h"(__HALF_TO_CUS(a)));
+        : "=r"(__HALF2_TO_UI(val)) : "h"(__HALF_TO_CUS(lh)));
     return val;
 }
-__CUDA_FP16_DECL__ __half2 __lowhigh2highlow(const __half2 a)
+__CUDA_FP16_DECL__ __half2 __lowhigh2highlow(const __half2 lh)
 {
     __half2 val;
     asm("{.reg .f16 low,high;\n"
         "  mov.b32 {low,high}, %1;\n"
-        "  mov.b32 %0, {high,low};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
+        "  mov.b32 %0, {high,low};}\n" : "=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(lh)));
     return val;
 }
 __CUDA_FP16_DECL__ short int __half_as_short(const __half h)
 {
-    return static_cast<short int>(__HALF_TO_CUS(h));
+    return (short int)__HALF_TO_CUS(h);
 }
 __CUDA_FP16_DECL__ unsigned short int __half_as_ushort(const __half h)
 {
     return __HALF_TO_CUS(h);
 }
 __CUDA_FP16_DECL__ __half __short_as_half(const short int i)
 {
     __half h;
-    __HALF_TO_US(h) = static_cast<unsigned short int>(i);
+    __HALF_TO_US(h) = (unsigned short int)i;
     return h;
 }
 __CUDA_FP16_DECL__ __half __ushort_as_half(const unsigned short int i)
 {
     __half h;
     __HALF_TO_US(h) = i;
     return h;
 }
 
 #if __CUDA_ARCH__ >= 300 || !defined(__CUDA_ARCH__)
 /******************************************************************************
 *                           __half, __half2 warp shuffle                     *
 ******************************************************************************/
-#define __SHUFFLE_HALF2_MACRO(name) /* do */ {\
+#define __SHUFFLE_HALF2_MACRO(name) do {\
    __half2 r; \
-   asm volatile ("{"#name" %0,%1,%2,%3;\n}" \
+   asm("{"#name" %0,%1,%2,%3;\n}" \
        :"=r"(__HALF2_TO_UI(r)): "r"(__HALF2_TO_CUI(var)), "r"(delta), "r"(c)); \
    return r; \
-} /* while(0) */
+} while(0)
 
-#define __SHUFFLE_SYNC_HALF2_MACRO(name) /* do */ {\
+#define __SHUFFLE_SYNC_HALF2_MACRO(name) do {\
    __half2 r; \
-   asm volatile ("{"#name" %0,%1,%2,%3,%4;\n}" \
+   asm("{"#name" %0,%1,%2,%3,%4;\n}" \
        :"=r"(__HALF2_TO_UI(r)): "r"(__HALF2_TO_CUI(var)), "r"(delta), "r"(c), "r"(mask)); \
    return r; \
-} /* while(0) */
-
-#if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ < 700
+} while(0)
 
-__CUDA_FP16_DECL__ __half2 __shfl(const __half2 var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl(__half2 var, int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = ((warp_size - static_cast<unsigned>(width)) << 8U) | 0x1fU;
-    __SHUFFLE_HALF2_MACRO(shfl.idx.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = ((warpSize - width) << 8) | 0x1f;
+    __SHUFFLE_HALF2_MACRO(shfl.idx.b32);
 }
-__CUDA_FP16_DECL__ __half2 __shfl_up(const __half2 var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_up(__half2 var, unsigned int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = (warp_size - static_cast<unsigned>(width)) << 8U;
-    __SHUFFLE_HALF2_MACRO(shfl.up.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = (warpSize - width) << 8;
+    __SHUFFLE_HALF2_MACRO(shfl.up.b32);
 }
-__CUDA_FP16_DECL__ __half2 __shfl_down(const __half2 var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_down(__half2 var, unsigned int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = ((warp_size - static_cast<unsigned>(width)) << 8U) | 0x1fU;
-    __SHUFFLE_HALF2_MACRO(shfl.down.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = ((warpSize - width) << 8) | 0x1f;
+    __SHUFFLE_HALF2_MACRO(shfl.down.b32);
 }
-__CUDA_FP16_DECL__ __half2 __shfl_xor(const __half2 var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_xor(__half2 var, int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = ((warp_size - static_cast<unsigned>(width)) << 8U) | 0x1fU;
-    __SHUFFLE_HALF2_MACRO(shfl.bfly.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = ((warpSize - width) << 8) | 0x1f;
+    __SHUFFLE_HALF2_MACRO(shfl.bfly.b32);
 }
 
-#endif /* !defined(__CUDA_ARCH__) || __CUDA_ARCH__ < 700 */
-
-__CUDA_FP16_DECL__ __half2 __shfl_sync(const unsigned mask, const __half2 var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_sync(unsigned mask, __half2 var, int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = ((warp_size - static_cast<unsigned>(width)) << 8U) | 0x1fU;
-    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.idx.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = ((warpSize - width) << 8) | 0x1f;
+    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.idx.b32);
 }
-__CUDA_FP16_DECL__ __half2 __shfl_up_sync(const unsigned mask, const __half2 var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_up_sync(unsigned mask, __half2 var, unsigned int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = (warp_size - static_cast<unsigned>(width)) << 8U;
-    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.up.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = (warpSize - width) << 8;
+    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.up.b32);
 }
-__CUDA_FP16_DECL__ __half2 __shfl_down_sync(const unsigned mask, const __half2 var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_down_sync(unsigned mask, __half2 var, unsigned int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = ((warp_size - static_cast<unsigned>(width)) << 8U) | 0x1fU;
-    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.down.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = ((warpSize - width) << 8) | 0x1f;
+    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.down.b32);
 }
-__CUDA_FP16_DECL__ __half2 __shfl_xor_sync(const unsigned mask, const __half2 var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half2 __shfl_xor_sync(unsigned mask, __half2 var, int delta, int width)
 {
-    unsigned int warp_size;
-    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warp_size));
-    const unsigned int c = ((warp_size - static_cast<unsigned>(width)) << 8U) | 0x1fU;
-    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.bfly.b32)
+    int warpSize;
+    asm("{mov.u32 %0, WARP_SZ;\n}" : "=r"(warpSize));
+    int c = ((warpSize - width) << 8) | 0x1f;
+    __SHUFFLE_SYNC_HALF2_MACRO(shfl.sync.bfly.b32);
 }
 
 #undef __SHUFFLE_HALF2_MACRO
 #undef __SHUFFLE_SYNC_HALF2_MACRO
 
-#if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ < 700
-
-__CUDA_FP16_DECL__ __half __shfl(const __half var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl(__half var, int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl(temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl(temp1, delta, width);
     return __low2half(temp2);
 }
-__CUDA_FP16_DECL__ __half __shfl_up(const __half var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_up(__half var, unsigned int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_up(temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_up(temp1, delta, width);
     return __low2half(temp2);
 }
-__CUDA_FP16_DECL__ __half __shfl_down(const __half var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_down(__half var, unsigned int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_down(temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_down(temp1, delta, width);
     return __low2half(temp2);
 }
-__CUDA_FP16_DECL__ __half __shfl_xor(const __half var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_xor(__half var, int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_xor(temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_xor(temp1, delta, width);
     return __low2half(temp2);
 }
 
-#endif /* !defined(__CUDA_ARCH__) || __CUDA_ARCH__ < 700 */
-
-__CUDA_FP16_DECL__ __half __shfl_sync(const unsigned mask, const __half var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_sync(unsigned mask, __half var, int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_sync(mask, temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_sync(mask, temp1, delta, width);
     return __low2half(temp2);
 }
-__CUDA_FP16_DECL__ __half __shfl_up_sync(const unsigned mask, const __half var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_up_sync(unsigned mask, __half var, unsigned int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_up_sync(mask, temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_up_sync(mask, temp1, delta, width);
     return __low2half(temp2);
 }
-__CUDA_FP16_DECL__ __half __shfl_down_sync(const unsigned mask, const __half var, const unsigned int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_down_sync(unsigned mask, __half var, unsigned int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_down_sync(mask, temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_down_sync(mask, temp1, delta, width);
     return __low2half(temp2);
 }
-__CUDA_FP16_DECL__ __half __shfl_xor_sync(const unsigned mask, const __half var, const int delta, const int width)
+__CUDA_FP16_DECL__ __half __shfl_xor_sync(unsigned mask, __half var, int delta, int width)
 {
-    const __half2 temp1 = __halves2half2(var, var);
-    const __half2 temp2 = __shfl_xor_sync(mask, temp1, delta, width);
+    __half2 temp1 = __halves2half2(var, var);
+    __half2 temp2 = __shfl_xor_sync(mask, temp1, delta, width);
     return __low2half(temp2);
 }
 
 #endif /*__CUDA_ARCH__ >= 300 || !defined(__CUDA_ARCH__)*/
 /******************************************************************************
 *               __half and __half2 __ldg,__ldcg,__ldca,__ldcs                *
 ******************************************************************************/
 
 #if defined(__cplusplus) && (__CUDA_ARCH__ >= 320 || !defined(__CUDA_ARCH__))
 #if (defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)
 #define __LDG_PTR   "l"
 #else
 #define __LDG_PTR   "r"
 #endif /*(defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)*/
-__CUDA_FP16_DECL__ __half2 __ldg(const  __half2 *const ptr)
+__CUDA_FP16_DECL__ __half2 __ldg(const  __half2 *ptr)
 {
     __half2 ret;
     asm ("ld.global.nc.b32 %0, [%1];"  : "=r"(__HALF2_TO_UI(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half __ldg(const __half *const ptr)
+__CUDA_FP16_DECL__ __half __ldg(const __half *ptr)
 {
     __half ret;
     asm ("ld.global.nc.b16 %0, [%1];"  : "=h"(__HALF_TO_US(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half2 __ldcg(const  __half2 *const ptr)
+__CUDA_FP16_DECL__ __half2 __ldcg(const  __half2 *ptr)
 {
     __half2 ret;
     asm ("ld.global.cg.b32 %0, [%1];"  : "=r"(__HALF2_TO_UI(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half __ldcg(const __half *const ptr)
+__CUDA_FP16_DECL__ __half __ldcg(const __half *ptr)
 {
     __half ret;
     asm ("ld.global.cg.b16 %0, [%1];"  : "=h"(__HALF_TO_US(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half2 __ldca(const  __half2 *const ptr)
+__CUDA_FP16_DECL__ __half2 __ldca(const  __half2 *ptr)
 {
     __half2 ret;
     asm ("ld.global.ca.b32 %0, [%1];"  : "=r"(__HALF2_TO_UI(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half __ldca(const __half *const ptr)
+__CUDA_FP16_DECL__ __half __ldca(const __half *ptr)
 {
     __half ret;
     asm ("ld.global.ca.b16 %0, [%1];"  : "=h"(__HALF_TO_US(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half2 __ldcs(const  __half2 *const ptr)
+__CUDA_FP16_DECL__ __half2 __ldcs(const  __half2 *ptr)
 {
     __half2 ret;
     asm ("ld.global.cs.b32 %0, [%1];"  : "=r"(__HALF2_TO_UI(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half __ldcs(const __half *const ptr)
+__CUDA_FP16_DECL__ __half __ldcs(const __half *ptr)
 {
     __half ret;
     asm ("ld.global.cs.b16 %0, [%1];"  : "=h"(__HALF_TO_US(ret)) : __LDG_PTR(ptr));
     return ret;
 }
-__CUDA_FP16_DECL__ __half2 __ldlu(const  __half2 *const ptr)
-{
-    __half2 ret;
-    asm ("ld.global.lu.b32 %0, [%1];"  : "=r"(__HALF2_TO_UI(ret)) : __LDG_PTR(ptr) : "memory");
-    return ret;
-}
-__CUDA_FP16_DECL__ __half __ldlu(const __half *const ptr)
-{
-    __half ret;
-    asm ("ld.global.lu.b16 %0, [%1];"  : "=h"(__HALF_TO_US(ret)) : __LDG_PTR(ptr) : "memory");
-    return ret;
-}
-__CUDA_FP16_DECL__ __half2 __ldcv(const  __half2 *const ptr)
-{
-    __half2 ret;
-    asm ("ld.global.cv.b32 %0, [%1];"  : "=r"(__HALF2_TO_UI(ret)) : __LDG_PTR(ptr) : "memory");
-    return ret;
-}
-__CUDA_FP16_DECL__ __half __ldcv(const __half *const ptr)
-{
-    __half ret;
-    asm ("ld.global.cv.b16 %0, [%1];"  : "=h"(__HALF_TO_US(ret)) : __LDG_PTR(ptr) : "memory");
-    return ret;
-}
-__CUDA_FP16_DECL__ void __stwb(__half2 *const ptr, const __half2 value)
-{
-    asm ("st.global.wb.b32 [%0], %1;"  :: __LDG_PTR(ptr), "r"(__HALF2_TO_CUI(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stwb(__half *const ptr, const __half value)
-{
-    asm ("st.global.wb.b16 [%0], %1;"  :: __LDG_PTR(ptr),  "h"(__HALF_TO_CUS(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stcg(__half2 *const ptr, const __half2 value)
-{
-    asm ("st.global.cg.b32 [%0], %1;"  :: __LDG_PTR(ptr), "r"(__HALF2_TO_CUI(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stcg(__half *const ptr, const __half value)
-{
-    asm ("st.global.cg.b16 [%0], %1;"  :: __LDG_PTR(ptr),  "h"(__HALF_TO_CUS(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stcs(__half2 *const ptr, const __half2 value)
-{
-    asm ("st.global.cs.b32 [%0], %1;"  :: __LDG_PTR(ptr), "r"(__HALF2_TO_CUI(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stcs(__half *const ptr, const __half value)
-{
-    asm ("st.global.cs.b16 [%0], %1;"  :: __LDG_PTR(ptr),  "h"(__HALF_TO_CUS(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stwt(__half2 *const ptr, const __half2 value)
-{
-    asm ("st.global.wt.b32 [%0], %1;"  :: __LDG_PTR(ptr), "r"(__HALF2_TO_CUI(value)) : "memory");
-}
-__CUDA_FP16_DECL__ void __stwt(__half *const ptr, const __half value)
-{
-    asm ("st.global.wt.b16 [%0], %1;"  :: __LDG_PTR(ptr),  "h"(__HALF_TO_CUS(value)) : "memory");
-}
 #undef __LDG_PTR
 #endif /*defined(__cplusplus) && (__CUDA_ARCH__ >= 320 || !defined(__CUDA_ARCH__))*/
 #if __CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)
 /******************************************************************************
 *                             __half2 comparison                             *
 ******************************************************************************/
-#define __COMPARISON_OP_HALF2_MACRO(name) /* do */ {\
+#define __COMPARISON_OP_HALF2_MACRO(name) do {\
    __half2 val; \
    asm( "{ "#name".f16x2.f16x2 %0,%1,%2;\n}" \
         :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
    return val; \
-} /* while(0) */
+} while(0)
 __CUDA_FP16_DECL__ __half2 __heq2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.eq)
+    __COMPARISON_OP_HALF2_MACRO(set.eq);
 }
 __CUDA_FP16_DECL__ __half2 __hne2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.ne)
+    __COMPARISON_OP_HALF2_MACRO(set.ne);
 }
 __CUDA_FP16_DECL__ __half2 __hle2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.le)
+    __COMPARISON_OP_HALF2_MACRO(set.le);
 }
 __CUDA_FP16_DECL__ __half2 __hge2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.ge)
+    __COMPARISON_OP_HALF2_MACRO(set.ge);
 }
 __CUDA_FP16_DECL__ __half2 __hlt2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.lt)
+    __COMPARISON_OP_HALF2_MACRO(set.lt);
 }
 __CUDA_FP16_DECL__ __half2 __hgt2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.gt)
+    __COMPARISON_OP_HALF2_MACRO(set.gt);
 }
 __CUDA_FP16_DECL__ __half2 __hequ2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.equ)
+    __COMPARISON_OP_HALF2_MACRO(set.equ);
 }
 __CUDA_FP16_DECL__ __half2 __hneu2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.neu)
+    __COMPARISON_OP_HALF2_MACRO(set.neu);
 }
 __CUDA_FP16_DECL__ __half2 __hleu2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.leu)
+    __COMPARISON_OP_HALF2_MACRO(set.leu);
 }
 __CUDA_FP16_DECL__ __half2 __hgeu2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.geu)
+    __COMPARISON_OP_HALF2_MACRO(set.geu);
 }
 __CUDA_FP16_DECL__ __half2 __hltu2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.ltu)
+    __COMPARISON_OP_HALF2_MACRO(set.ltu);
 }
 __CUDA_FP16_DECL__ __half2 __hgtu2(const __half2 a, const __half2 b)
 {
-    __COMPARISON_OP_HALF2_MACRO(set.gtu)
+    __COMPARISON_OP_HALF2_MACRO(set.gtu);
 }
 #undef __COMPARISON_OP_HALF2_MACRO
-#define __BOOL_COMPARISON_OP_HALF2_MACRO(name) /* do */ {\
+#define __BOOL_COMPARISON_OP_HALF2_MACRO(name) do {\
    __half2 val; \
-   bool retval; \
    asm( "{ "#name".f16x2.f16x2 %0,%1,%2;\n}" \
         :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
-   if (__HALF2_TO_CUI(val) == 0x3C003C00U) {\
-      retval = true; \
-   } else { \
-      retval = false; \
-   }\
-   return retval;\
-} /* while(0) */
+   if (__HALF2_TO_CUI(val) == 0x3C003C00) \
+      return true; \
+   else  \
+      return false; \
+} while(0)
 __CUDA_FP16_DECL__ bool __hbeq2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.eq)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.eq);
 }
 __CUDA_FP16_DECL__ bool __hbne2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.ne)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.ne);
 }
 __CUDA_FP16_DECL__ bool __hble2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.le)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.le);
 }
 __CUDA_FP16_DECL__ bool __hbge2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.ge)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.ge);
 }
 __CUDA_FP16_DECL__ bool __hblt2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.lt)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.lt);
 }
 __CUDA_FP16_DECL__ bool __hbgt2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.gt)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.gt);
 }
 __CUDA_FP16_DECL__ bool __hbequ2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.equ)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.equ);
 }
 __CUDA_FP16_DECL__ bool __hbneu2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.neu)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.neu);
 }
 __CUDA_FP16_DECL__ bool __hbleu2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.leu)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.leu);
 }
 __CUDA_FP16_DECL__ bool __hbgeu2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.geu)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.geu);
 }
 __CUDA_FP16_DECL__ bool __hbltu2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.ltu)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.ltu);
 }
 __CUDA_FP16_DECL__ bool __hbgtu2(const __half2 a, const __half2 b)
 {
-    __BOOL_COMPARISON_OP_HALF2_MACRO(set.gtu)
+    __BOOL_COMPARISON_OP_HALF2_MACRO(set.gtu);
 }
 #undef __BOOL_COMPARISON_OP_HALF2_MACRO
 /******************************************************************************
 *                             __half comparison                              *
 ******************************************************************************/
-#define __COMPARISON_OP_HALF_MACRO(name) /* do */ {\
+#define __COMPARISON_OP_HALF_MACRO(name) do {\
    unsigned short val; \
    asm( "{ .reg .pred __$temp3;\n" \
         "  setp."#name".f16  __$temp3, %1, %2;\n" \
         "  selp.u16 %0, 1, 0, __$temp3;}" \
         : "=h"(val) : "h"(__HALF_TO_CUS(a)), "h"(__HALF_TO_CUS(b))); \
-   return (val != 0U) ? true : false; \
-} /* while(0) */
+   return val ? true : false; \
+} while(0)
 __CUDA_FP16_DECL__ bool __heq(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(eq)
+    __COMPARISON_OP_HALF_MACRO(eq);
 }
 __CUDA_FP16_DECL__ bool __hne(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(ne)
+    __COMPARISON_OP_HALF_MACRO(ne);
 }
 __CUDA_FP16_DECL__ bool __hle(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(le)
+    __COMPARISON_OP_HALF_MACRO(le);
 }
 __CUDA_FP16_DECL__ bool __hge(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(ge)
+    __COMPARISON_OP_HALF_MACRO(ge);
 }
 __CUDA_FP16_DECL__ bool __hlt(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(lt)
+    __COMPARISON_OP_HALF_MACRO(lt);
 }
 __CUDA_FP16_DECL__ bool __hgt(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(gt)
+    __COMPARISON_OP_HALF_MACRO(gt);
 }
 __CUDA_FP16_DECL__ bool __hequ(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(equ)
+    __COMPARISON_OP_HALF_MACRO(equ);
 }
 __CUDA_FP16_DECL__ bool __hneu(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(neu)
+    __COMPARISON_OP_HALF_MACRO(neu);
 }
 __CUDA_FP16_DECL__ bool __hleu(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(leu)
+    __COMPARISON_OP_HALF_MACRO(leu);
 }
 __CUDA_FP16_DECL__ bool __hgeu(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(geu)
+    __COMPARISON_OP_HALF_MACRO(geu);
 }
 __CUDA_FP16_DECL__ bool __hltu(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(ltu)
+    __COMPARISON_OP_HALF_MACRO(ltu);
 }
 __CUDA_FP16_DECL__ bool __hgtu(const __half a, const __half b)
 {
-    __COMPARISON_OP_HALF_MACRO(gtu)
+    __COMPARISON_OP_HALF_MACRO(gtu);
 }
 #undef __COMPARISON_OP_HALF_MACRO
 /******************************************************************************
 *                            __half2 arithmetic                             *
 ******************************************************************************/
+#define __BINARY_OP_HALF2_MACRO(name) do {\
+   __half2 val; \
+   asm( "{"#name".f16x2 %0,%1,%2;\n}" \
+        :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b))); \
+   return val; \
+} while(0)
+
 __CUDA_FP16_DECL__ __half2 __hadd2(const __half2 a, const __half2 b)
 {
-    __BINARY_OP_HALF2_MACRO(add)
+    __BINARY_OP_HALF2_MACRO(add);
 }
 __CUDA_FP16_DECL__ __half2 __hsub2(const __half2 a, const __half2 b)
 {
-    __BINARY_OP_HALF2_MACRO(sub)
+    __BINARY_OP_HALF2_MACRO(sub);
 }
 __CUDA_FP16_DECL__ __half2 __hmul2(const __half2 a, const __half2 b)
 {
-    __BINARY_OP_HALF2_MACRO(mul)
+    __BINARY_OP_HALF2_MACRO(mul);
 }
 __CUDA_FP16_DECL__ __half2 __hadd2_sat(const __half2 a, const __half2 b)
 {
-    __BINARY_OP_HALF2_MACRO(add.sat)
+    __BINARY_OP_HALF2_MACRO(add.sat);
 }
 __CUDA_FP16_DECL__ __half2 __hsub2_sat(const __half2 a, const __half2 b)
 {
-    __BINARY_OP_HALF2_MACRO(sub.sat)
+    __BINARY_OP_HALF2_MACRO(sub.sat);
 }
 __CUDA_FP16_DECL__ __half2 __hmul2_sat(const __half2 a, const __half2 b)
 {
-    __BINARY_OP_HALF2_MACRO(mul.sat)
+    __BINARY_OP_HALF2_MACRO(mul.sat);
 }
+#undef __BINARY_OP_HALF2_MACRO
+#define __TERNARY_OP_HALF2_MACRO(name) do {\
+   __half2 val; \
+   asm( "{"#name".f16x2 %0,%1,%2,%3;\n}" \
+        :"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)),"r"(__HALF2_TO_CUI(b)),"r"(__HALF2_TO_CUI(c))); \
+   return val; \
+} while(0)
 __CUDA_FP16_DECL__ __half2 __hfma2(const __half2 a, const __half2 b, const __half2 c)
 {
-    __TERNARY_OP_HALF2_MACRO(fma.rn)
+    __TERNARY_OP_HALF2_MACRO(fma.rn);
 }
 __CUDA_FP16_DECL__ __half2 __hfma2_sat(const __half2 a, const __half2 b, const __half2 c)
 {
-    __TERNARY_OP_HALF2_MACRO(fma.rn.sat)
+    __TERNARY_OP_HALF2_MACRO(fma.rn.sat);
 }
-__CUDA_FP16_DECL__ __half2 __h2div(const __half2 a, const __half2 b) {
-    __half ha = __low2half(a);
-    __half hb = __low2half(b);
+#undef __TERNARY_OP_HALF2_MACRO
+__CUDA_FP16_DECL__ __half2 __h2div(__half2 a, __half2 b) {
+    __half ha, hb;
 
-    const __half v1 = __hdiv(ha, hb);
+    ha = __low2half(a);
+    hb = __low2half(b);
+
+    __half v1 = __hdiv(ha, hb);
 
     ha = __high2half(a);
     hb = __high2half(b);
 
-    const __half v2 = __hdiv(ha, hb);
+    __half v2 = __hdiv(ha, hb);
 
     return __halves2half2(v1, v2);
 }
 /******************************************************************************
 *                             __half arithmetic                             *
 ******************************************************************************/
+#define __BINARY_OP_HALF_MACRO(name) do {\
+   __half val; \
+   asm( "{"#name".f16 %0,%1,%2;\n}" \
+        :"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)),"h"(__HALF_TO_CUS(b))); \
+   return val; \
+} while(0)
 __CUDA_FP16_DECL__ __half __hadd(const __half a, const __half b)
 {
-    __BINARY_OP_HALF_MACRO(add)
+    __BINARY_OP_HALF_MACRO(add);
 }
 __CUDA_FP16_DECL__ __half __hsub(const __half a, const __half b)
 {
-    __BINARY_OP_HALF_MACRO(sub)
+    __BINARY_OP_HALF_MACRO(sub);
 }
 __CUDA_FP16_DECL__ __half __hmul(const __half a, const __half b)
 {
-    __BINARY_OP_HALF_MACRO(mul)
+    __BINARY_OP_HALF_MACRO(mul);
 }
 __CUDA_FP16_DECL__ __half __hadd_sat(const __half a, const __half b)
 {
-    __BINARY_OP_HALF_MACRO(add.sat)
+    __BINARY_OP_HALF_MACRO(add.sat);
 }
 __CUDA_FP16_DECL__ __half __hsub_sat(const __half a, const __half b)
 {
-    __BINARY_OP_HALF_MACRO(sub.sat)
+    __BINARY_OP_HALF_MACRO(sub.sat);
 }
 __CUDA_FP16_DECL__ __half __hmul_sat(const __half a, const __half b)
 {
-    __BINARY_OP_HALF_MACRO(mul.sat)
+    __BINARY_OP_HALF_MACRO(mul.sat);
 }
-
+#undef __BINARY_OP_HALF_MACRO
+#define __TERNARY_OP_HALF_MACRO(name) do {\
+   __half val; \
+   asm( "{"#name".f16 %0,%1,%2,%3;\n}" \
+        :"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)),"h"(__HALF_TO_CUS(b)),"h"(__HALF_TO_CUS(c))); \
+   return val; \
+} while(0)
 __CUDA_FP16_DECL__ __half __hfma(const __half a, const __half b, const __half c)
 {
-    __TERNARY_OP_HALF_MACRO(fma.rn)
+    __TERNARY_OP_HALF_MACRO(fma.rn);
 }
 __CUDA_FP16_DECL__ __half __hfma_sat(const __half a, const __half b, const __half c)
 {
-    __TERNARY_OP_HALF_MACRO(fma.rn.sat)
+    __TERNARY_OP_HALF_MACRO(fma.rn.sat);
 }
-__CUDA_FP16_DECL__ __half __hdiv(const __half a, const __half b) {
-    __half v;
-    __half abs;
-    __half den;
-    __HALF_TO_US(den) = 0x008FU;
+#undef __TERNARY_OP_HALF2_MACRO
+__CUDA_FP16_DECL__ __half __hdiv(__half a, __half b) {
+    __half v, abs, den;
+    __HALF_TO_US(den) = 0x008F;
+    float fa, fb, fv, rcp;
 
-    float rcp;
-    const float fa = __half2float(a);
-    const float fb = __half2float(b);
+    fa = __half2float(a);
+    fb = __half2float(b);
 
-    asm("{rcp.approx.ftz.f32 %0, %1;\n}" :"=f"(rcp) : "f"(fb));
+    asm("{rcp.approx.f32 %0, %1;\n}" :"=f"(rcp) : "f"(fb));
 
-    float fv = rcp * fa;
+    fv = rcp * fa;
 
     v = __float2half(fv);
-    __HALF_TO_US(abs) = static_cast<unsigned short>(static_cast<unsigned int>(__HALF_TO_CUS(v)) & 0x00007FFFU);
-    if (__hlt(abs, den) && (!(__HALF_TO_CUS(abs) == 0x0000U))) {
-        const float err = __fmaf_rn(-fb, fv, fa);
+    __HALF_TO_US(abs) = (unsigned short)(((unsigned int)__HALF_TO_CUS(v)) & 0x00007FFF);
+    if (__hlt(abs, den) && (!(__HALF_TO_CUS(abs) == 0x0000))) {
+        float err = __fmaf_rn(-fb, fv, fa);
         fv = __fmaf_rn(rcp, err, fv);
         v = __float2half(fv);
     }
     return v;
 }
 
 /******************************************************************************
@@ -1904,80 +1532,78 @@
    "  fma.rn.f16x2 "#r",p,ulp,"#r";\n}\n"
 #define __SPEC_CASE(i,r, spc, ulp) \
    "{.reg.b16 spc, ulp, p;\n"\
    "  mov.b16 spc,"#spc";\n"\
    "  mov.b16 ulp,"#ulp";\n"\
    "  set.eq.f16.f16 p,"#i", spc;\n"\
    "  fma.rn.f16 "#r",p,ulp,"#r";\n}\n"
-#define __APPROX_FCAST(fun) /* do */ {\
+#define __APPROX_FCAST(fun) do {\
    __half val;\
    asm("{.reg.b32         f;        \n"\
                 " .reg.b16         r;        \n"\
                 "  mov.b16         r,%1;     \n"\
                 "  cvt.f32.f16     f,r;      \n"\
                 "  "#fun".approx.f32   f,f;  \n"\
                 "  cvt.rn.f16.f32      r,f;  \n"\
                 "  mov.b16         %0,r;     \n"\
                 "}": "=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));\
    return val;\
-} /* while(0) */
-#define __APPROX_FCAST2(fun) /* do */ {\
+} while(0)
+#define __APPROX_FCAST2(fun) do {\
    __half2 val;\
    asm("{.reg.b16         hl, hu;         \n"\
                 " .reg.b32         fl, fu;         \n"\
                 "  mov.b32         {hl, hu}, %1;   \n"\
                 "  cvt.f32.f16     fl, hl;         \n"\
                 "  cvt.f32.f16     fu, hu;         \n"\
                 "  "#fun".approx.f32   fl, fl;     \n"\
                 "  "#fun".approx.f32   fu, fu;     \n"\
                 "  cvt.rn.f16.f32      hl, fl;     \n"\
                 "  cvt.rn.f16.f32      hu, fu;     \n"\
                 "  mov.b32         %0, {hl, hu};   \n"\
                 "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));       \
    return val;\
-} /* while(0) */
-static __device__ __forceinline__ float __float_simpl_sinf(float a);
-static __device__ __forceinline__ float __float_simpl_cosf(float a);
+} while(0)
+static __device__ __forceinline__ float __float_simpl_sinf(float);
+static __device__ __forceinline__ float __float_simpl_cosf(float);
 __CUDA_FP16_DECL__ __half __hsin_internal(const __half a) {
     float f = __half2float(a);
     f = __float_simpl_sinf(f);
     return __float2half_rn(f);
 }
 __CUDA_FP16_DECL__ __half hsin(const __half a) {
     __half r = __hsin_internal(a);
     asm("{\n\t"
         "  .reg.b16 i,r,t;     \n\t"
         "  mov.b16 r, %0;      \n\t"
         "  mov.b16 i, %1;      \n\t"
-        "  mov.b16 t, 0x8000U;  \n\t"
+        "  mov.b16 t, 0x8000;  \n\t"
         "  and.b16 t,r,t;      \n\t"
-        __SPEC_CASE(i, r, 0X32B3U, 0x0800U)
-        __SPEC_CASE(i, r, 0X5CB0U, 0x1000U)
-        __SPEC_CASE(i, r, 0XB2B3U, 0x8800U)
-        __SPEC_CASE(i, r, 0XDCB0U, 0x9000U)
+        __SPEC_CASE(i, r, 0X32B3, 0x0800)
+        __SPEC_CASE(i, r, 0X5CB0, 0x1000)
+        __SPEC_CASE(i, r, 0XB2B3, 0x8800)
+        __SPEC_CASE(i, r, 0XDCB0, 0x9000)
         "  or.b16  r,r,t;      \n\t"
         "  mov.b16 %0, r;      \n"
         "}\n" : "+h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)));
     return r;
 }
 __CUDA_FP16_DECL__ __half2 h2sin(const __half2 a) {
-    const __half l = __low2half(a);
-    const __half h = __high2half(a);
-    const __half sl = __hsin_internal(l);
-    const __half sh = __hsin_internal(h);
-    __half2 r = __halves2half2(sl, sh);
+    __half l = __low2half(a);
+    __half h = __high2half(a);
+    __half2 r = __halves2half2(__hsin_internal(l), __hsin_internal(h));
     asm("{\n\t"
         "  .reg.b32 i,r,t;             \n\t"
         "  mov.b32 r, %0;              \n\t"
         "  mov.b32 i, %1;              \n\t"
-        "  and.b32 t, r, 0x80008000U;   \n\t"
-        __SPEC_CASE2(i, r, 0X32B332B3U, 0x08000800U)
-        __SPEC_CASE2(i, r, 0X5CB05CB0U, 0x10001000U)
-        __SPEC_CASE2(i, r, 0XB2B3B2B3U, 0x88008800U)
-        __SPEC_CASE2(i, r, 0XDCB0DCB0U, 0x90009000U)
+        "  and.b32 t, r, 0x80008000;   \n\t"
+        __SPEC_CASE2(i, r, 0X32B332B3, 0x08000800)
+        __SPEC_CASE2(i, r, 0X5CB05CB0, 0x10001000)
+        __SPEC_CASE2(i, r, 0XB2B3B2B3, 0x88008800)
+        __SPEC_CASE2(i, r, 0XDCB0DCB0, 0x90009000)
         "  or.b32  r, r, t;            \n\t"
         "  mov.b32 %0, r;              \n"
         "}\n" : "+r"(__HALF2_TO_UI(r)) : "r"(__HALF2_TO_CUI(a)));
     return r;
 }
 __CUDA_FP16_DECL__ __half __hcos_internal(const __half a) {
     float f = __half2float(a);
@@ -1986,151 +1612,144 @@
 }
 __CUDA_FP16_DECL__ __half hcos(const __half a) {
     __half r = __hcos_internal(a);
     asm("{\n\t"
         "  .reg.b16 i,r;        \n\t"
         "  mov.b16 r, %0;       \n\t"
         "  mov.b16 i, %1;       \n\t"
-        __SPEC_CASE(i, r, 0X2B7CU, 0x1000U)
-        __SPEC_CASE(i, r, 0XAB7CU, 0x1000U)
+        __SPEC_CASE(i, r, 0X2B7C, 0x1000)
+        __SPEC_CASE(i, r, 0XAB7C, 0x1000)
         "  mov.b16 %0, r;       \n"
         "}\n" : "+h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)));
     return r;
 }
 __CUDA_FP16_DECL__ __half2 h2cos(const __half2 a) {
-    const __half l = __low2half(a);
-    const __half h = __high2half(a);
-    const __half cl = __hcos_internal(l);
-    const __half ch = __hcos_internal(h);
-    __half2 r = __halves2half2(cl, ch);
+    __half l = __low2half(a);
+    __half h = __high2half(a);
+    __half2 r = __halves2half2(__hcos_internal(l), __hcos_internal(h));
     asm("{\n\t"
         "  .reg.b32 i,r;   \n\t"
         "  mov.b32 r, %0;  \n\t"
         "  mov.b32 i, %1;  \n\t"
-        __SPEC_CASE2(i, r, 0X2B7C2B7CU, 0x10001000U)
-        __SPEC_CASE2(i, r, 0XAB7CAB7CU, 0x10001000U)
+        __SPEC_CASE2(i, r, 0X2B7C2B7C, 0x10001000)
+        __SPEC_CASE2(i, r, 0XAB7CAB7C, 0x10001000)
         "  mov.b32 %0, r;  \n"
         "}\n" : "+r"(__HALF2_TO_UI(r)) : "r"(__HALF2_TO_CUI(a)));
     return r;
 }
-static __device__ __forceinline__ float __internal_trig_reduction_kernel(const float a, int *quadrant)
+static __device__ __forceinline__ float __internal_trig_reduction_kernel(float a, int *quadrant)
 {
-    const int q = __float2int_rn(a * 0.636619772F);
-    const float j = static_cast<float>(q);
-    float t = __fmaf_rn(-j, 1.5707962512969971e+000F, a);
-    t = __fmaf_rn(-j, 7.5497894158615964e-008F, t);
+    float j, t;
+    int q;
+    q = __float2int_rn(a * 0.636619772f);
+    j = (float)q;
+    t = __fmaf_rn(-j, 1.5707962512969971e+000f, a);
+    t = __fmaf_rn(-j, 7.5497894158615964e-008f, t);
     *quadrant = q;
     return t;
 }
-static __device__ __forceinline__ float __internal_sin_cos_kernel(float x, const int i)
+static __device__ __forceinline__ float __internal_sin_cos_kernel(float x, int i)
 {
-    float z;
-    const float x2 = x*x;
+    float x2, z;
+    x2 = x*x;
 
-    if ((static_cast<unsigned>(i) & 1U) != 0U) {
-        z = 2.44331571e-5F;
-        z = __fmaf_rn(z, x2, -1.38873163e-3F);
-    }
-    else {
-        z = -1.95152959e-4F;
-        z = __fmaf_rn(z, x2, 8.33216087e-3F);
-    }
-    if ((static_cast<unsigned>(i) & 1U) != 0U) {
-        z = __fmaf_rn(z, x2, 4.16666457e-2F);
-        z = __fmaf_rn(z, x2, -5.00000000e-1F);
+    if (i & 1) {
+        z = 2.44331571e-5f;
+        z = __fmaf_rn(z, x2, -1.38873163e-3f);
     }
     else {
-        z = __fmaf_rn(z, x2, -1.66666546e-1F);
-        z = __fmaf_rn(z, x2, 0.0F);
+        z = -1.95152959e-4f;
+        z = __fmaf_rn(z, x2, 8.33216087e-3f);
     }
-    if ((static_cast<unsigned>(i) & 1U) != 0U) {
-        x = __fmaf_rn(z, x2, 1.0F);
+    if (i & 1) {
+        z = __fmaf_rn(z, x2, 4.16666457e-2f);
+        z = __fmaf_rn(z, x2, -5.00000000e-1f);
     }
     else {
-        x = __fmaf_rn(z, x, x);
-    }
-    if ((static_cast<unsigned>(i) & 2U) != 0U) {
-        x = __fmaf_rn(x, -1.0F, 0.0F);
+        z = __fmaf_rn(z, x2, -1.66666546e-1f);
+        z = __fmaf_rn(z, x2, 0.0f);
     }
+    x = __fmaf_rn(z, x, x);
+    if (i & 1) x = __fmaf_rn(z, x2, 1.0f);
+    if (i & 2) x = __fmaf_rn(x, -1.0f, 0.0f);
     return x;
 }
 static __device__ __forceinline__ float __float_simpl_sinf(float a)
 {
     float z;
     int i;
-    if (::isinf(a)) {
-        a = a * 0.0F;
+    if (isinf(a)) {
+        a = a * 0.0f;
     }
     a = __internal_trig_reduction_kernel(a, &i);
     z = __internal_sin_cos_kernel(a, i);
     return z;
 }
 static __device__ __forceinline__ float __float_simpl_cosf(float a)
 {
     float z;
     int i;
-    if (::isinf(a)) {
-        a = a * 0.0F;
+    if (isinf(a)) {
+        a = a * 0.0f;
     }
     a = __internal_trig_reduction_kernel(a, &i);
     i++;
     z = __internal_sin_cos_kernel(a, i);
     return z;
 }
-
 __CUDA_FP16_DECL__ __half hexp(const __half a) {
     __half val;
     asm("{.reg.b32         f, C;           \n"
         " .reg.b16         h,r;            \n"
         "  mov.b16         h,%1;           \n"
         "  cvt.f32.f16     f,h;            \n"
-        "  mov.b32         C, 0x3fb8aa3bU;  \n"
+        "  mov.b32         C, 0x3fb8aa3b;  \n"
         "  mul.f32         f,f,C;          \n"
         "  ex2.approx.f32      f,f;        \n"
         "  cvt.rn.f16.f32      r,f;        \n"
-        __SPEC_CASE(h, r, 0X1F79U, 0x9400U)
-        __SPEC_CASE(h, r, 0X25CFU, 0x9400U)
-        __SPEC_CASE(h, r, 0XC13BU, 0x0400U)
-        __SPEC_CASE(h, r, 0XC1EFU, 0x0200U)
+        __SPEC_CASE(h, r, 0X1F79, 0x9400)
+        __SPEC_CASE(h, r, 0X25CF, 0x9400)
+        __SPEC_CASE(h, r, 0XC13B, 0x0400)
+        __SPEC_CASE(h, r, 0XC1EF, 0x0200)
         "  mov.b16         %0,r;           \n"
         "}": "=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half2 h2exp(const __half2 a) {
     __half2 val;
     asm("{.reg.b16         hl, hu;         \n"
         " .reg.b32         h,r,fl,fu, C;   \n"
         "  mov.b32         {hl, hu}, %1;   \n"
         "  mov.b32         h, %1;          \n"
         "  cvt.f32.f16     fl, hl;         \n"
         "  cvt.f32.f16     fu, hu;         \n"
-        "  mov.b32         C, 0x3fb8aa3bU;  \n"
+        "  mov.b32         C, 0x3fb8aa3b;  \n"
         "  mul.f32         fl,fl,C;        \n"
         "  mul.f32         fu,fu,C;        \n"
         "  ex2.approx.f32      fl, fl;     \n"
         "  ex2.approx.f32      fu, fu;     \n"
         "  cvt.rn.f16.f32      hl, fl;     \n"
         "  cvt.rn.f16.f32      hu, fu;     \n"
         "  mov.b32         r, {hl, hu};    \n"
-        __SPEC_CASE2(h, r, 0X1F791F79U, 0x94009400U)
-        __SPEC_CASE2(h, r, 0X25CF25CFU, 0x94009400U)
-        __SPEC_CASE2(h, r, 0XC13BC13BU, 0x04000400U)
-        __SPEC_CASE2(h, r, 0XC1EFC1EFU, 0x02000200U)
+        __SPEC_CASE2(h, r, 0X1F791F79, 0x94009400)
+        __SPEC_CASE2(h, r, 0X25CF25CF, 0x94009400)
+        __SPEC_CASE2(h, r, 0XC13BC13B, 0x04000400)
+        __SPEC_CASE2(h, r, 0XC1EFC1EF, 0x02000200)
         "  mov.b32         %0, r;  \n"
         "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half hexp2(const __half a) {
     __half val;
     asm("{.reg.b32         f, ULP;         \n"
         " .reg.b16         r;              \n"
         "  mov.b16         r,%1;           \n"
         "  cvt.f32.f16     f,r;            \n"
         "  ex2.approx.f32      f,f;        \n"
-        "  mov.b32         ULP, 0x33800000U;\n"
+        "  mov.b32         ULP, 0x33800000;\n"
         "  fma.rn.f32      f,f,ULP,f;      \n"
         "  cvt.rn.f16.f32      r,f;        \n"
         "  mov.b16         %0,r;           \n"
         "}": "=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half2 h2exp2(const __half2 a) {
@@ -2138,77 +1757,77 @@
     asm("{.reg.b16         hl, hu;         \n"
         " .reg.b32         fl, fu, ULP;    \n"
         "  mov.b32         {hl, hu}, %1;   \n"
         "  cvt.f32.f16     fl, hl;         \n"
         "  cvt.f32.f16     fu, hu;         \n"
         "  ex2.approx.f32      fl, fl;     \n"
         "  ex2.approx.f32      fu, fu;     \n"
-        "  mov.b32         ULP, 0x33800000U;\n"
+        "  mov.b32         ULP, 0x33800000;\n"
         "  fma.rn.f32      fl,fl,ULP,fl;   \n"
         "  fma.rn.f32      fu,fu,ULP,fu;   \n"
         "  cvt.rn.f16.f32      hl, fl;     \n"
         "  cvt.rn.f16.f32      hu, fu;     \n"
         "  mov.b32         %0, {hl, hu};   \n"
         "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half hexp10(const __half a) {
     __half val;
     asm("{.reg.b16         h,r;            \n"
         " .reg.b32         f, C;           \n"
         "  mov.b16         h, %1;          \n"
         "  cvt.f32.f16     f, h;           \n"
-        "  mov.b32         C, 0x40549A78U;  \n"
+        "  mov.b32         C, 0x40549A78;  \n"
         "  mul.f32         f,f,C;          \n"
         "  ex2.approx.f32      f, f;       \n"
         "  cvt.rn.f16.f32      r, f;       \n"
-        __SPEC_CASE(h, r, 0x34DEU, 0x9800U)
-        __SPEC_CASE(h, r, 0x9766U, 0x9000U)
-        __SPEC_CASE(h, r, 0x9972U, 0x1000U)
-        __SPEC_CASE(h, r, 0xA5C4U, 0x1000U)
-        __SPEC_CASE(h, r, 0xBF0AU, 0x8100U)
+        __SPEC_CASE(h, r, 0x34DE, 0x9800)
+        __SPEC_CASE(h, r, 0x9766, 0x9000)
+        __SPEC_CASE(h, r, 0x9972, 0x1000)
+        __SPEC_CASE(h, r, 0xA5C4, 0x1000)
+        __SPEC_CASE(h, r, 0xBF0A, 0x8100)
         "  mov.b16         %0, r;          \n"
         "}":"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half2 h2exp10(const __half2 a) {
     __half2 val;
     asm("{.reg.b16         hl, hu;         \n"
         " .reg.b32         h,r,fl,fu, C;   \n"
         "  mov.b32         {hl, hu}, %1;   \n"
         "  mov.b32         h, %1;          \n"
         "  cvt.f32.f16     fl, hl;         \n"
         "  cvt.f32.f16     fu, hu;         \n"
-        "  mov.b32         C, 0x40549A78U;  \n"
+        "  mov.b32         C, 0x40549A78;  \n"
         "  mul.f32         fl,fl,C;        \n"
         "  mul.f32         fu,fu,C;        \n"
         "  ex2.approx.f32      fl, fl;     \n"
         "  ex2.approx.f32      fu, fu;     \n"
         "  cvt.rn.f16.f32      hl, fl;     \n"
         "  cvt.rn.f16.f32      hu, fu;     \n"
         "  mov.b32         r, {hl, hu};    \n"
-        __SPEC_CASE2(h, r, 0x34DE34DEU, 0x98009800U)
-        __SPEC_CASE2(h, r, 0x97669766U, 0x90009000U)
-        __SPEC_CASE2(h, r, 0x99729972U, 0x10001000U)
-        __SPEC_CASE2(h, r, 0xA5C4A5C4U, 0x10001000U)
-        __SPEC_CASE2(h, r, 0xBF0ABF0AU, 0x81008100U)
+        __SPEC_CASE2(h, r, 0x34DE34DE, 0x98009800)
+        __SPEC_CASE2(h, r, 0x97669766, 0x90009000)
+        __SPEC_CASE2(h, r, 0x99729972, 0x10001000)
+        __SPEC_CASE2(h, r, 0xA5C4A5C4, 0x10001000)
+        __SPEC_CASE2(h, r, 0xBF0ABF0A, 0x81008100)
         "  mov.b32         %0, r;  \n"
         "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half hlog2(const __half a) {
     __half val;
     asm("{.reg.b16         h, r;           \n"
         " .reg.b32         f;              \n"
         "  mov.b16         h, %1;          \n"
         "  cvt.f32.f16     f, h;           \n"
         "  lg2.approx.f32      f, f;       \n"
         "  cvt.rn.f16.f32      r, f;       \n"
-        __SPEC_CASE(r, r, 0xA2E2U, 0x8080U)
-        __SPEC_CASE(r, r, 0xBF46U, 0x9400U)
+        __SPEC_CASE(r, r, 0xA2E2, 0x8080)
+        __SPEC_CASE(r, r, 0xBF46, 0x9400)
         "  mov.b16         %0, r;          \n"
         "}":"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half2 h2log2(const __half2 a) {
     __half2 val;
     asm("{.reg.b16         hl, hu;         \n"
@@ -2217,123 +1836,123 @@
         "  cvt.f32.f16     fl, hl;         \n"
         "  cvt.f32.f16     fu, hu;         \n"
         "  lg2.approx.f32      fl, fl;     \n"
         "  lg2.approx.f32      fu, fu;     \n"
         "  cvt.rn.f16.f32      hl, fl;     \n"
         "  cvt.rn.f16.f32      hu, fu;     \n"
         "  mov.b32         r, {hl, hu};    \n"
-        __SPEC_CASE2(r, r, 0xA2E2A2E2U, 0x80808080U)
-        __SPEC_CASE2(r, r, 0xBF46BF46U, 0x94009400U)
+        __SPEC_CASE2(r, r, 0xA2E2A2E2, 0x80808080)
+        __SPEC_CASE2(r, r, 0xBF46BF46, 0x94009400)
         "  mov.b32         %0, r;          \n"
         "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half hlog(const __half a) {
     __half val;
     asm("{.reg.b32         f, C;           \n"
         " .reg.b16         r,h;            \n"
         "  mov.b16         h,%1;           \n"
         "  cvt.f32.f16     f,h;            \n"
         "  lg2.approx.f32      f,f;        \n"
-        "  mov.b32         C, 0x3f317218U;  \n"
+        "  mov.b32         C, 0x3f317218;  \n"
         "  mul.f32         f,f,C;          \n"
         "  cvt.rn.f16.f32      r,f;        \n"
-        __SPEC_CASE(h, r, 0X160DU, 0x9C00U)
-        __SPEC_CASE(h, r, 0X3BFEU, 0x8010U)
-        __SPEC_CASE(h, r, 0X3C0BU, 0x8080U)
-        __SPEC_CASE(h, r, 0X6051U, 0x1C00U)
+        __SPEC_CASE(h, r, 0X160D, 0x9C00)
+        __SPEC_CASE(h, r, 0X3BFE, 0x8010)
+        __SPEC_CASE(h, r, 0X3C0B, 0x8080)
+        __SPEC_CASE(h, r, 0X6051, 0x1C00)
         "  mov.b16         %0,r;           \n"
         "}": "=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half2 h2log(const __half2 a) {
     __half2 val;
     asm("{.reg.b16         hl, hu;             \n"
         " .reg.b32         r, fl, fu, C, h;    \n"
         "  mov.b32         {hl, hu}, %1;       \n"
         "  mov.b32         h, %1;              \n"
         "  cvt.f32.f16     fl, hl;             \n"
         "  cvt.f32.f16     fu, hu;             \n"
         "  lg2.approx.f32      fl, fl;         \n"
         "  lg2.approx.f32      fu, fu;         \n"
-        "  mov.b32         C, 0x3f317218U;     \n"
+        "  mov.b32         C, 0x3f317218;      \n"
         "  mul.f32         fl,fl,C;            \n"
         "  mul.f32         fu,fu,C;            \n"
         "  cvt.rn.f16.f32      hl, fl;         \n"
         "  cvt.rn.f16.f32      hu, fu;         \n"
         "  mov.b32         r, {hl, hu};        \n"
-        __SPEC_CASE2(h, r, 0X160D160DU, 0x9C009C00U)
-        __SPEC_CASE2(h, r, 0X3BFE3BFEU, 0x80108010U)
-        __SPEC_CASE2(h, r, 0X3C0B3C0BU, 0x80808080U)
-        __SPEC_CASE2(h, r, 0X60516051U, 0x1C001C00U)
+        __SPEC_CASE2(h, r, 0X160D160D, 0x9C009C00)
+        __SPEC_CASE2(h, r, 0X3BFE3BFE, 0x80108010)
+        __SPEC_CASE2(h, r, 0X3C0B3C0B, 0x80808080)
+        __SPEC_CASE2(h, r, 0X60516051, 0x1C001C00)
         "  mov.b32         %0, r;              \n"
         "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half hlog10(const __half a) {
     __half val;
     asm("{.reg.b16         h, r;           \n"
         " .reg.b32         f, C;           \n"
         "  mov.b16         h, %1;          \n"
         "  cvt.f32.f16     f, h;           \n"
         "  lg2.approx.f32      f, f;       \n"
-        "  mov.b32         C, 0x3E9A209BU; \n"
+        "  mov.b32         C, 0x3E9A209B;  \n"
         "  mul.f32         f,f,C;          \n"
         "  cvt.rn.f16.f32      r, f;       \n"
-        __SPEC_CASE(h, r, 0x338FU, 0x1000U)
-        __SPEC_CASE(h, r, 0x33F8U, 0x9000U)
-        __SPEC_CASE(h, r, 0x57E1U, 0x9800U)
-        __SPEC_CASE(h, r, 0x719DU, 0x9C00U)
+        __SPEC_CASE(h, r, 0x338F, 0x1000)
+        __SPEC_CASE(h, r, 0x33F8, 0x9000)
+        __SPEC_CASE(h, r, 0x57E1, 0x9800)
+        __SPEC_CASE(h, r, 0x719D, 0x9C00)
         "  mov.b16         %0, r;          \n"
         "}":"=h"(__HALF_TO_US(val)) : "h"(__HALF_TO_CUS(a)));
     return val;
 }
 __CUDA_FP16_DECL__ __half2 h2log10(const __half2 a) {
     __half2 val;
     asm("{.reg.b16         hl, hu;             \n"
         " .reg.b32         r, fl, fu, C, h;    \n"
         "  mov.b32         {hl, hu}, %1;       \n"
         "  mov.b32         h, %1;              \n"
         "  cvt.f32.f16     fl, hl;             \n"
         "  cvt.f32.f16     fu, hu;             \n"
         "  lg2.approx.f32      fl, fl;         \n"
         "  lg2.approx.f32      fu, fu;         \n"
-        "  mov.b32         C, 0x3E9A209BU;     \n"
+        "  mov.b32         C, 0x3E9A209B;      \n"
         "  mul.f32         fl,fl,C;            \n"
         "  mul.f32         fu,fu,C;            \n"
         "  cvt.rn.f16.f32      hl, fl;         \n"
         "  cvt.rn.f16.f32      hu, fu;         \n"
         "  mov.b32         r, {hl, hu};        \n"
-        __SPEC_CASE2(h, r, 0x338F338FU, 0x10001000U)
-        __SPEC_CASE2(h, r, 0x33F833F8U, 0x90009000U)
-        __SPEC_CASE2(h, r, 0x57E157E1U, 0x98009800U)
-        __SPEC_CASE2(h, r, 0x719D719DU, 0x9C009C00U)
+        __SPEC_CASE2(h, r, 0x338F338F, 0x10001000)
+        __SPEC_CASE2(h, r, 0x33F833F8, 0x90009000)
+        __SPEC_CASE2(h, r, 0x57E157E1, 0x98009800)
+        __SPEC_CASE2(h, r, 0x719D719D, 0x9C009C00)
         "  mov.b32         %0, r;              \n"
         "}":"=r"(__HALF2_TO_UI(val)) : "r"(__HALF2_TO_CUI(a)));
     return val;
 }
 #undef __SPEC_CASE2
 #undef __SPEC_CASE
 __CUDA_FP16_DECL__ __half2 h2rcp(const __half2 a) {
-    __APPROX_FCAST2(rcp)
+    __APPROX_FCAST2(rcp);
 }
 __CUDA_FP16_DECL__ __half hrcp(const __half a) {
-    __APPROX_FCAST(rcp)
+    __APPROX_FCAST(rcp);
 }
 __CUDA_FP16_DECL__ __half2 h2rsqrt(const __half2 a) {
-    __APPROX_FCAST2(rsqrt)
+    __APPROX_FCAST2(rsqrt);
 }
 __CUDA_FP16_DECL__ __half hrsqrt(const __half a) {
-    __APPROX_FCAST(rsqrt)
+    __APPROX_FCAST(rsqrt);
 }
 __CUDA_FP16_DECL__ __half2 h2sqrt(const __half2 a) {
-    __APPROX_FCAST2(sqrt)
+    __APPROX_FCAST2(sqrt);
 }
 __CUDA_FP16_DECL__ __half hsqrt(const __half a) {
-    __APPROX_FCAST(sqrt)
+    __APPROX_FCAST(sqrt);
 }
 #undef __APPROX_FCAST
 #undef __APPROX_FCAST2
 __CUDA_FP16_DECL__ __half2 __hisnan2(const __half2 a)
 {
     __half2 r;
     asm("{set.nan.f16x2.f16x2 %0,%1,%2;\n}"
@@ -2341,166 +1960,65 @@
     return r;
 }
 __CUDA_FP16_DECL__ bool __hisnan(const __half a)
 {
     __half r;
     asm("{set.nan.f16.f16 %0,%1,%2;\n}"
         :"=h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)), "h"(__HALF_TO_CUS(a)));
-    return __HALF_TO_CUS(r) != 0U;
+    if (__HALF_TO_CUS(r) == 0)
+        return false;
+    else return true;
 }
 __CUDA_FP16_DECL__ __half2 __hneg2(const __half2 a)
 {
-    __half2 r;
-    asm("{neg.f16x2 %0,%1;\n}"
-        :"=r"(__HALF2_TO_UI(r)) : "r"(__HALF2_TO_CUI(a)));
-    return r;
+    __half2 zero = __float2half2_rn(0.0);
+    return __hsub2(zero, a);
 }
 __CUDA_FP16_DECL__ __half __hneg(const __half a)
 {
-    __half r;
-    asm("{neg.f16 %0,%1;\n}"
-        :"=h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)));
-    return r;
-}
-__CUDA_FP16_DECL__ __half2 __habs2(const __half2 a)
-{
-    __half2 r;
-    asm("{abs.f16x2 %0,%1;\n}"
-        :"=r"(__HALF2_TO_UI(r)) : "r"(__HALF2_TO_CUI(a)));
-    return r;
-}
-__CUDA_FP16_DECL__ __half __habs(const __half a)
-{
-    __half r;
-    asm("{abs.f16 %0,%1;\n}"
-        :"=h"(__HALF_TO_US(r)) : "h"(__HALF_TO_CUS(a)));
-    return r;
-}
-
-__CUDA_FP16_DECL__ __half2 __hcmadd(const __half2 a, const __half2 b, const __half2 c)
-{
-    // fast version of complex multiply-accumulate
-    // (a.re, a.im) * (b.re, b.im) + (c.re, c.im)
-    // acc.re = (c.re + a.re*b.re) - a.im*b.im
-    // acc.im = (c.im + a.re*b.im) + a.im*b.re
-    __half real_tmp =  __hfma(a.x, b.x, c.x);
-    __half img_tmp  =  __hfma(a.x, b.y, c.y);
-    real_tmp = __hfma(__hneg(a.y), b.y, real_tmp);
-    img_tmp  = __hfma(a.y,         b.x, img_tmp);
-    return make_half2(real_tmp, img_tmp);
+    __half zero;
+    zero = __float2half(0.0);
+    return __hsub(zero, a);
 }
 #endif /*__CUDA_ARCH__ >= 530 || !defined(__CUDA_ARCH__)*/
 
-#if __CUDA_ARCH__ >= 800 || !defined(__CUDA_ARCH__)
-/******************************************************************************
-*                             __half arithmetic                             *
-******************************************************************************/
-__CUDA_FP16_DECL__ __half __hmax(const __half a, const __half b)
-{
-    __BINARY_OP_HALF_MACRO(max)
-}
-__CUDA_FP16_DECL__ __half __hmin(const __half a, const __half b)
-{
-    __BINARY_OP_HALF_MACRO(min)
-}
-__CUDA_FP16_DECL__ __half __hmax_nan(const __half a, const __half b)
-{
-    __BINARY_OP_HALF_MACRO(max.NaN)
-}
-__CUDA_FP16_DECL__ __half __hmin_nan(const __half a, const __half b)
-{
-    __BINARY_OP_HALF_MACRO(min.NaN)
-}
-__CUDA_FP16_DECL__ __half __hfma_relu(const __half a, const __half b, const __half c)
-{
-    __TERNARY_OP_HALF_MACRO(fma.rn.relu)
-}
-/******************************************************************************
-*                            __half2 arithmetic                             *
-******************************************************************************/
-__CUDA_FP16_DECL__ __half2 __hmax2(const __half2 a, const __half2 b)
-{
-    __BINARY_OP_HALF2_MACRO(max)
-}
-__CUDA_FP16_DECL__ __half2 __hmin2(const __half2 a, const __half2 b)
-{
-    __BINARY_OP_HALF2_MACRO(min)
-}
-__CUDA_FP16_DECL__ __half2 __hmax2_nan(const __half2 a, const __half2 b)
-{
-    __BINARY_OP_HALF2_MACRO(max.NaN)
-}
-__CUDA_FP16_DECL__ __half2 __hmin2_nan(const __half2 a, const __half2 b)
-{
-    __BINARY_OP_HALF2_MACRO(min.NaN)
-}
-__CUDA_FP16_DECL__ __half2 __hfma2_relu(const __half2 a, const __half2 b, const __half2 c)
-{
-    __TERNARY_OP_HALF2_MACRO(fma.rn.relu)
-}
-#endif /*__CUDA_ARCH__ >= 800 || !defined(__CUDA_ARCH__)*/
+#if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 600
 
-/* Define __PTR for atomicAdd prototypes below, undef after done */
 #if (defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)
 #define __PTR   "l"
 #else
 #define __PTR   "r"
 #endif /*(defined(_MSC_VER) && defined(_WIN64)) || defined(__LP64__) || defined(__CUDACC_RTC__)*/
 
-#if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 600
-
-__CUDA_FP16_DECL__  __half2 atomicAdd(__half2 *const address, const __half2 val) {
+__CUDA_FP16_DECL__  __half2 atomicAdd(__half2 *address, __half2 val) {
     __half2 r;
     asm volatile ("{ atom.add.noftz.f16x2 %0,[%1],%2; }\n"
                   : "=r"(__HALF2_TO_UI(r)) : __PTR(address), "r"(__HALF2_TO_CUI(val))
                   : "memory");
    return r;
 }
 
-#endif /*!defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 600*/
-
-#if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 700
-
-__CUDA_FP16_DECL__  __half atomicAdd(__half *const address, const __half val) {
-    __half r;
-    asm volatile ("{ atom.add.noftz.f16 %0,[%1],%2; }\n"
-                  : "=h"(__HALF_TO_US(r))
-                  : __PTR(address), "h"(__HALF_TO_CUS(val))
-                  : "memory");
-   return r;
-}
-
-#endif /*!defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 700*/
-
 #undef __PTR
 
+#endif /*!defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 600*/
+
 #undef __CUDA_FP16_DECL__
 #endif /* defined(__CUDACC__) */
 #endif /* defined(__cplusplus) */
 
-#undef __TERNARY_OP_HALF2_MACRO
-#undef __TERNARY_OP_HALF_MACRO
-#undef __BINARY_OP_HALF2_MACRO
-#undef __BINARY_OP_HALF_MACRO
-
 #undef __CUDA_HOSTDEVICE_FP16_DECL__
 #undef __CUDA_FP16_DECL__
- 
+#undef __HALF_TO_US
+#undef __HALF_TO_CUS
+#undef __HALF2_TO_UI
+#undef __HALF2_TO_CUI
+#undef __COPY_FLOAT_TO_UI
+#undef __COPY_UI_TO_FLOAT
+
 /* Define first-class types "half" and "half2", unless user specifies otherwise via "#define CUDA_NO_HALF" */
 /* C cannot ever have these types defined here, because __half and __half2 are C++ classes */
 #if defined(__cplusplus) && !defined(CUDA_NO_HALF)
 typedef __half half;
 typedef __half2 half2;
-// for consistency with __nv_bfloat16
-typedef __half      __nv_half;
-typedef __half2     __nv_half2;
-typedef __half_raw  __nv_half_raw;
-typedef __half2_raw __nv_half2_raw;
-typedef __half        nv_half;
-typedef __half2       nv_half2;
 #endif /* defined(__cplusplus) && !defined(CUDA_NO_HALF) */
 
-#if defined(__CPP_VERSION_AT_LEAST_11_FP16)
-#undef __CPP_VERSION_AT_LEAST_11_FP16
-#endif /* defined(__CPP_VERSION_AT_LEAST_11_FP16) */
-
 #endif /* end of include guard: __CUDA_FP16_HPP__ */
```

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.h` & `cupy-9.6.0/cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/atomics.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/atomics.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/carray.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/carray.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/arithmetic.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/arithmetic.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/catrig.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/catrig.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/catrigf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/catrigf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/ccosh.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/ccosh.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/ccoshf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/ccoshf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/cexp.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/cexp.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/cexpf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/cexpf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/clog.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/clog.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/clogf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/clogf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/complex.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/complex.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/complex_inl.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/complex_inl.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/cpow.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/cpow.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/cproj.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/cproj.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/csinh.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/csinh.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/csinhf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/csinhf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/csqrt.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/csqrt.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/csqrtf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/csqrtf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/ctanh.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/ctanh.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/ctanhf.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/ctanhf.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex/math_private.h` & `cupy-9.6.0/cupy/_core/include/cupy/complex/math_private.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/complex.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/complex.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cuComplex_bridge.h` & `cupy-9.6.0/cupy/_core/include/cupy/cuComplex_bridge.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/CHANGE_LOG.TXT` & `cupy-9.6.0/cupy/_core/include/cupy/cub/CHANGE_LOG.TXT`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/LICENSE.TXT` & `cupy-9.6.0/cupy/_core/include/cupy/cub/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/README.md` & `cupy-9.6.0/cupy/_core/include/cupy/cub/README.md`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/common.mk` & `cupy-9.6.0/cupy/_core/include/cupy/cub/common.mk`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_histogram.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_histogram.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_downsweep.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_downsweep.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_upsweep.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_radix_sort_upsweep.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce_by_key.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_reduce_by_key.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_rle.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_rle.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_scan.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_scan.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_segment_fixup.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_segment_fixup.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_select_if.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_select_if.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/agent_spmv_orig.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/agent_spmv_orig.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/agent/single_pass_scan_operators.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/agent/single_pass_scan_operators.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_adjacent_difference.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_adjacent_difference.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_discontinuity.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_discontinuity.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_exchange.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_exchange.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_histogram.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_histogram.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_load.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_load.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_radix_rank.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_radix_rank.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_radix_sort.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_raking_layout.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_raking_layout.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_scan.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_scan.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_shuffle.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_shuffle.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/block_store.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/block_store.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_atomic.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_atomic.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_sort.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_histogram_sort.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking_commutative_only.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_raking_commutative_only.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_warp_reductions.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_reduce_warp_reductions.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_raking.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_raking.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans2.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans2.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans3.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/block/specializations/block_scan_warp_scans3.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/cub.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/cub.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_histogram.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_histogram.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_partition.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_partition.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_radix_sort.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_run_length_encode.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_run_length_encode.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_scan.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_scan.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_radix_sort.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_segmented_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_select.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_select.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/device_spmv.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/device_spmv.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_histogram.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_histogram.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_radix_sort.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce_by_key.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_reduce_by_key.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_rle.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_rle.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_scan.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_scan.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_select_if.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_select_if.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_spmv_orig.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/device/dispatch/dispatch_spmv_orig.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_barrier.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_barrier.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_even_share.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_even_share.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_mapping.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_mapping.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/grid/grid_queue.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/grid/grid_queue.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/host/mutex.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/host/mutex.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/arg_index_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/arg_index_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_output_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/cache_modified_output_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/constant_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/constant_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/counting_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/counting_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/discard_output_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/discard_output_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/tex_obj_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/tex_obj_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/tex_ref_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/tex_ref_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/iterator/transform_input_iterator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/iterator/transform_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_load.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_load.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_operators.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_operators.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_scan.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_scan.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_search.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_search.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/thread/thread_store.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/thread/thread_store.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_allocator.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_allocator.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_arch.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_arch.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_debug.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_debug.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_device.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_device.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_macro.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_macro.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_namespace.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_namespace.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_ptx.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_ptx.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/util_type.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/util_type.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_shfl.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_shfl.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_smem.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_reduce_smem.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_shfl.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_shfl.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_smem.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/specializations/warp_scan_smem.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/warp_reduce.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/warp_reduce.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/cub/warp/warp_scan.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/cub/warp/warp_scan.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/eclipse code style profile.xml` & `cupy-9.6.0/cupy/_core/include/cupy/cub/eclipse code style profile.xml`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/Makefile` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/Makefile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/Makefile` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/Makefile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/Makefile` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/Makefile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_cub.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_cub.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_gmem_atomics.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_gmem_atomics.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_smem_atomics.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram/histogram_smem_atomics.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/sparse_matrix.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/sparse_matrix.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/experimental/spmv_script.sh` & `cupy-9.6.0/cupy/_core/include/cupy/cub/experimental/spmv_script.sh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/Makefile` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/Makefile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/half.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/half.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/mersenne.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/mersenne.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_allocator.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_allocator.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_histogram.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_histogram.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_load_store.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_load_store.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_block_scan.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_block_scan.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_histogram.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_histogram.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_scan.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_scan.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_select_if.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_iterator.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_iterator.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_util.h` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_util.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/test/test_warp_scan.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/test/test_warp_scan.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/tune/Makefile` & `cupy-9.6.0/cupy/_core/include/cupy/cub/tune/Makefile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu` & `cupy-9.6.0/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/dlpack/dlpack.h` & `cupy-9.6.0/cupy/_core/include/cupy/dlpack/dlpack.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/hip_workaround.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/hip_workaround.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/Doxyfile` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/Doxyfile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/LICENSE` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/LICENSE`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/Makefile` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/Makefile`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/README.md` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/README.md`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/class_arg_kernel.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/class_arg_kernel.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/constant_header.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/constant_header.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/my_header1.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/my_header1.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/my_header2.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/my_header2.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/example_headers/my_header3.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/example_headers/my_header3.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/jitify.hpp` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/jitify.hpp`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/jitify/jitify_test.cu` & `cupy-9.6.0/cupy/_core/include/cupy/jitify/jitify_test.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/math_constants.h` & `cupy-9.6.0/cupy/_core/include/cupy/math_constants.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/swap.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/swap.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/tuple/tuple.h` & `cupy-9.6.0/cupy/_core/include/cupy/tuple/tuple.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/tuple/type_traits.h` & `cupy-9.6.0/cupy/_core/include/cupy/tuple/type_traits.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/tuple.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/tuple.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/include/cupy/type_dispatcher.cuh` & `cupy-9.6.0/cupy/_core/include/cupy/type_dispatcher.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/internal.pxd` & `cupy-9.6.0/cupy/_core/internal.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/internal.pyx` & `cupy-9.6.0/cupy/_core/internal.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,16 @@
     elif not isinstance(axes, tuple):
         axes = axes,
 
     res = []
     for axis in axes:
         axis = _normalize_axis_index(axis, ndim)
         if axis in res:
-            raise ValueError('Duplicate value in \'axis\'')
+            # the message in `numpy/core/src/multiarray/conversion_utils.c`
+            raise ValueError('duplicate value in \'axis\'')
         res.append(axis)
 
     return tuple(sorted(res) if sort_axes else res)
 
 
 cpdef strides_t _get_strides_for_order_K(x, dtype, shape=None):
     # x here can be either numpy.ndarray or cupy.ndarray
```

### Comparing `cupy-9.5.0/cupy/_core/new_fusion.pyx` & `cupy-9.6.0/cupy/_core/new_fusion.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/raw.pxd` & `cupy-9.6.0/cupy/_core/raw.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/raw.pyx` & `cupy-9.6.0/cupy/_core/raw.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_core/syncdetect.py` & `cupy-9.6.0/cupy/_core/syncdetect.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_creation/basic.py` & `cupy-9.6.0/cupy/_creation/basic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_creation/from_data.py` & `cupy-9.6.0/cupy/_creation/from_data.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_creation/matrix.py` & `cupy-9.6.0/cupy/_creation/matrix.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_creation/ranges.py` & `cupy-9.6.0/cupy/_creation/ranges.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_environment.py` & `cupy-9.6.0/cupy/_environment.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_functional/piecewise.py` & `cupy-9.6.0/cupy/_functional/piecewise.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_functional/vectorize.py` & `cupy-9.6.0/cupy/_functional/vectorize.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_indexing/generate.py` & `cupy-9.6.0/cupy/_indexing/generate.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_indexing/indexing.py` & `cupy-9.6.0/cupy/_indexing/indexing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_indexing/insert.py` & `cupy-9.6.0/cupy/_indexing/insert.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_indexing/iterate.py` & `cupy-9.6.0/cupy/_indexing/iterate.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_io/formatting.py` & `cupy-9.6.0/cupy/_io/formatting.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_io/npz.py` & `cupy-9.6.0/cupy/_io/npz.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_logic/comparison.py` & `cupy-9.6.0/cupy/_logic/comparison.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_logic/content.py` & `cupy-9.6.0/cupy/_logic/content.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_logic/ops.py` & `cupy-9.6.0/cupy/_logic/ops.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_logic/truth.py` & `cupy-9.6.0/cupy/_logic/truth.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_logic/type_test.py` & `cupy-9.6.0/cupy/_logic/type_test.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/add_remove.py` & `cupy-9.6.0/cupy/_manipulation/add_remove.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/basic.py` & `cupy-9.6.0/cupy/_manipulation/basic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/dims.py` & `cupy-9.6.0/cupy/_manipulation/dims.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/join.py` & `cupy-9.6.0/cupy/_manipulation/join.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/kind.py` & `cupy-9.6.0/cupy/_manipulation/kind.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/rearrange.py` & `cupy-9.6.0/cupy/_manipulation/rearrange.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/shape.py` & `cupy-9.6.0/cupy/_manipulation/shape.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/split.py` & `cupy-9.6.0/cupy/_manipulation/split.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/tiling.py` & `cupy-9.6.0/cupy/_manipulation/tiling.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_manipulation/transpose.py` & `cupy-9.6.0/cupy/_manipulation/transpose.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/arithmetic.py` & `cupy-9.6.0/cupy/_math/arithmetic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/explog.py` & `cupy-9.6.0/cupy/_math/explog.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/floating.py` & `cupy-9.6.0/cupy/_math/floating.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/hyperbolic.py` & `cupy-9.6.0/cupy/_math/hyperbolic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/misc.py` & `cupy-9.6.0/cupy/_math/misc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/rational.py` & `cupy-9.6.0/cupy/_math/rational.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/rounding.py` & `cupy-9.6.0/cupy/_math/rounding.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/special.py` & `cupy-9.6.0/cupy/_math/special.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/sumprod.py` & `cupy-9.6.0/cupy/_math/sumprod.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/trigonometric.py` & `cupy-9.6.0/cupy/_math/trigonometric.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/ufunc.py` & `cupy-9.6.0/cupy/_math/ufunc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_math/window.py` & `cupy-9.6.0/cupy/_math/window.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_misc/memory_ranges.py` & `cupy-9.6.0/cupy/_misc/memory_ranges.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_misc/who.py` & `cupy-9.6.0/cupy/_misc/who.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_padding/pad.py` & `cupy-9.6.0/cupy/_padding/pad.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_sorting/count.py` & `cupy-9.6.0/cupy/_sorting/count.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_sorting/search.py` & `cupy-9.6.0/cupy/_sorting/search.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_sorting/sort.py` & `cupy-9.6.0/cupy/_sorting/sort.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_statistics/correlation.py` & `cupy-9.6.0/cupy/_statistics/correlation.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_statistics/histogram.py` & `cupy-9.6.0/cupy/_statistics/histogram.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_statistics/meanvar.py` & `cupy-9.6.0/cupy/_statistics/meanvar.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_statistics/order.py` & `cupy-9.6.0/cupy/_statistics/order.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/_util.pyx` & `cupy-9.6.0/cupy/_util.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cublas.py` & `cupy-9.6.0/cupy/cublas.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/__init__.py` & `cupy-9.6.0/cupy/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/common.pxd` & `cupy-9.6.0/cupy/cuda/common.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/common.pyx` & `cupy-9.6.0/cupy/cuda/common.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/compiler.py` & `cupy-9.6.0/cupy/cuda/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,26 +147,27 @@
     arch = device.Device().compute_capability
     if arch in _tegra_archs:
         return arch
     else:
         return min(arch, nvrtc_max_compute_capability)
 
 
+@_util.memoize(for_each_device=True)
 def _get_arch_for_options_for_nvrtc(arch=None):
     # NVRTC in CUDA 11.3+ generates PTX that cannot be run an earlier driver
     # version than the one included in the used CUDA version, as
     # documented in:
     # https://docs.nvidia.com/cuda/archive/11.3.0/nvrtc/index.html#versioning
     # Here we use `-arch=sm_*` instead of `-arch=compute_*` to directly
     # generate cubin (SASS) instead of PTX. See #5097 for details.
     if arch is None:
         arch = _get_arch()
     if (
         not _use_ptx and _cuda_hip_version >= 11010
-        and arch < _get_max_compute_capability()
+        and arch <= _get_max_compute_capability()
     ):
         return f'-arch=sm_{arch}', 'cubin'
     return f'-arch=compute_{arch}', 'ptx'
 
 
 def _is_cudadevrt_needed(options):
     return any(o for o in options if o in _rdc_flags)
```

### Comparing `cupy-9.5.0/cupy/cuda/cub.pyx` & `cupy-9.6.0/cupy/cuda/cub.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cufft.pxd` & `cupy-9.6.0/cupy/cuda/cufft.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cufft.pyx` & `cupy-9.6.0/cupy/cuda/cufft.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_cub.cu` & `cupy-9.6.0/cupy/cuda/cupy_cub.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_cub.h` & `cupy-9.6.0/cupy/cuda/cupy_cub.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_cufft.h` & `cupy-9.6.0/cupy/cuda/cupy_cufft.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_cufftXt.cu` & `cupy-9.6.0/cupy/cuda/cupy_cufftXt.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_jitify.h` & `cupy-9.6.0/cupy/cuda/cupy_jitify.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_thrust.cu` & `cupy-9.6.0/cupy/cuda/cupy_thrust.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/cupy_thrust.h` & `cupy-9.6.0/cupy/cuda/cupy_thrust.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/device.pxd` & `cupy-9.6.0/cupy/cuda/device.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/device.pyx` & `cupy-9.6.0/cupy/cuda/device.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/function.pxd` & `cupy-9.6.0/cupy/cuda/function.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/function.pyx` & `cupy-9.6.0/cupy/cuda/function.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/jitify.pyx` & `cupy-9.6.0/cupy/cuda/jitify.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/memory.pxd` & `cupy-9.6.0/cupy/cuda/memory.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/memory.pyx` & `cupy-9.6.0/cupy/cuda/memory.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/memory_hook.pyx` & `cupy-9.6.0/cupy/cuda/memory_hook.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/memory_hooks/debug_print.py` & `cupy-9.6.0/cupy/cuda/memory_hooks/debug_print.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/memory_hooks/line_profile.py` & `cupy-9.6.0/cupy/cuda/memory_hooks/line_profile.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/pinned_memory.pxd` & `cupy-9.6.0/cupy/cuda/pinned_memory.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/pinned_memory.pyx` & `cupy-9.6.0/cupy/cuda/pinned_memory.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/stream.pyx` & `cupy-9.6.0/cupy/cuda/stream.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/texture.pxd` & `cupy-9.6.0/cupy/cuda/texture.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/texture.pyx` & `cupy-9.6.0/cupy/cuda/texture.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cuda/thrust.pyx` & `cupy-9.6.0/cupy/cuda/thrust.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cudnn.pyx` & `cupy-9.6.0/cupy/cudnn.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cusolver.pyx` & `cupy-9.6.0/cupy/cusolver.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cusparse.py` & `cupy-9.6.0/cupy/cusparse.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/cutensor.pyx` & `cupy-9.6.0/cupy/cutensor.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -100,43 +100,45 @@
     if name in _available_compute_capability:
         compute_capability = int(_device.get_compute_capability())
         if compute_capability < _available_compute_capability[name]:
             return False
     return True
 
 
-cdef class Mode(object):
+cdef class Mode:
 
     cdef:
         object _array
         readonly int ndim
         readonly intptr_t data
 
     def __init__(self, mode):
         self._array = _numpy.array(mode, dtype=_numpy.int32)
         assert self._array.ndim == 1
         self.ndim = self._array.size
         self.data = self._array.ctypes.data
 
     def __repr__(self):
-        return 'mode([' + ', '.join(self._array) + '])'
+        return 'mode(' + ', '.join([str(x) for x in self._array]) + ')'
 
 
-cdef class _Scalar(object):
+cdef class _Scalar:
 
     cdef:
         object _array
         readonly intptr_t ptr
 
     def __init__(self, value, dtype):
         self._array = _numpy.asarray(value, dtype=dtype)
         self.ptr = self._array.ctypes.data
 
     def __repr__(self):
-        return self._array.item()
+        return (
+            'scalar(' + str(self._array.item()) +
+            ', dtype=' + str(self._array.dtype) + ')')
 
 
 cdef Handle _get_handle():
     cdef Handle handle
     cdef int dev = device.get_device_id()
     if dev not in _handles:
         handle = Handle()
```

### Comparing `cupy-9.5.0/cupy/fft/__init__.py` & `cupy-9.6.0/cupy/fft/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/fft/_cache.pyx` & `cupy-9.6.0/cupy/fft/_cache.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/fft/_callback.pyx` & `cupy-9.6.0/cupy/fft/_callback.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/fft/_fft.py` & `cupy-9.6.0/cupy/fft/_fft.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/fft/config.py` & `cupy-9.6.0/cupy/fft/config.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/lib/_polynomial.pyx` & `cupy-9.6.0/cupy/lib/_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/lib/_routines_poly.py` & `cupy-9.6.0/cupy/lib/_routines_poly.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/lib/_shape_base.py` & `cupy-9.6.0/cupy/lib/_shape_base.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/lib/stride_tricks.py` & `cupy-9.6.0/cupy/lib/stride_tricks.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/__init__.py` & `cupy-9.6.0/cupy/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/_decomposition.py` & `cupy-9.6.0/cupy/linalg/_decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,18 +153,18 @@
     """Cholesky decomposition.
 
     Decompose a given two-dimensional square matrix into ``L * L.T``,
     where ``L`` is a lower-triangular matrix and ``.T`` is a conjugate
     transpose operator.
 
     Args:
-        a (cupy.ndarray): The input matrix with dimension ``(N, N)``
+        a (cupy.ndarray): The input matrix with dimension ``(..., M, M)``
 
     Returns:
-        cupy.ndarray: The lower-triangular matrix.
+        cupy.ndarray: The lower-triangular matrix of shape ``(..., M, M)``.
 
     .. warning::
         This function calls one or more cuSOLVER routine(s) which may yield
         invalid results if input conditions are not met.
         To detect these invalid results, you can set the `linalg`
         configuration to a value that is not `ignore` in
         :func:`cupyx.errstate` or :func:`cupyx.seterr`.
```

### Comparing `cupy-9.5.0/cupy/linalg/_eigenvalue.py` & `cupy-9.6.0/cupy/linalg/_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/_einsum.py` & `cupy-9.6.0/cupy/linalg/_einsum.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,16 @@
             # to assure final output of einsum is C-contiguous
             sub_out = sub_others
         arr0 = _expand_dims_transpose(arr0, sub0, sub_out)
         arr1 = _expand_dims_transpose(arr1, sub1, sub_out)
         return arr0 * arr1, sub_out
 
     for accelerator in _accelerator.get_routine_accelerators():
-        if accelerator == _accelerator.ACCELERATOR_CUTENSOR:
+        if (accelerator == _accelerator.ACCELERATOR_CUTENSOR and
+                cutensor is not None):
             if _use_cutensor(arr0.dtype, sub0, arr1.dtype, sub1,
                              batch_dims, contract_dims):
                 if len(sub_out) == len(sub_others):
                     # to assure final output of einsum is C-contiguous
                     sub_out = sub_others
                 out_shape = _get_out_shape(
                     arr0.shape, sub0, arr1.shape, sub1, sub_out)
```

### Comparing `cupy-9.5.0/cupy/linalg/_einsum_opt.py` & `cupy-9.6.0/cupy/linalg/_einsum_opt.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/_norms.py` & `cupy-9.6.0/cupy/linalg/_norms.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/_product.py` & `cupy-9.6.0/cupy/linalg/_product.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/_solve.py` & `cupy-9.6.0/cupy/linalg/_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/linalg/_util.py` & `cupy-9.6.0/cupy/linalg/_util.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/polynomial/polynomial.py` & `cupy-9.6.0/cupy/polynomial/polynomial.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/polynomial/polyutils.py` & `cupy-9.6.0/cupy/polynomial/polyutils.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/prof/_time_range.py` & `cupy-9.6.0/cupy/prof/_time_range.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/__init__.py` & `cupy-9.6.0/cupy/random/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/_bit_generator.pyx` & `cupy-9.6.0/cupy/random/_bit_generator.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/_distributions.py` & `cupy-9.6.0/cupy/random/_distributions.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/_generator.py` & `cupy-9.6.0/cupy/random/_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1107,39 +1107,17 @@
         if isinstance(a, int):
             return self._permutation(a)
         else:
             return a[self._permutation(len(a))]
 
     def _permutation(self, num):
         """Returns a permuted range."""
-        sample = cupy.empty((num), dtype=numpy.int32)
+        sample = cupy.empty((num,), dtype=numpy.int32)
         curand.generate(self._generator, sample.data.ptr, num)
-        if 128 < num <= 32 * 1024 * 1024:
-            array = cupy.arange(num, dtype=numpy.int32)
-            # apply sort of cache blocking
-            block_size = 1 * 1024 * 1024
-            # The block size above is a value determined from the L2 cache size
-            # of GP100 (L2 cache size / size of int = 4MB / 4B = 1M). It may be
-            # better to change the value base on the L2 cache size of the GPU
-            # you use.
-            # When num > block_size, cupy kernel: _cupy_permutation is to be
-            # launched multiple times. However, it is observed that performance
-            # will be degraded if the launch count is too many. Therefore,
-            # the block size is adjusted so that launch count will not exceed
-            # twelve Note that this twelve is the value determined from
-            # measurement on GP100.
-            while num // block_size > 12:
-                block_size *= 2
-            for j_start in range(0, num, block_size):
-                j_end = j_start + block_size
-                _cupy_permutation(sample, j_start, j_end, array, size=num)
-        else:
-            # When num > 32M, argsort is used, because it is faster than
-            # custom kernel. See https://github.com/cupy/cupy/pull/603.
-            array = cupy.argsort(sample)
+        array = cupy.argsort(sample)
         return array
 
     _gumbel_kernel = _core.ElementwiseKernel(
         'T x, T loc, T scale', 'T y',
         'y = T(loc) - log(-log(x)) * T(scale)',
         'cupy_gumbel_kernel')
 
@@ -1185,70 +1163,14 @@
 
         diff = hi1 - lo
         x = self._interval(diff, size).astype(dtype, copy=False)
         cupy.add(x, lo, out=x)
         return x
 
 
-_cupy_permutation = _core.ElementwiseKernel(
-    'raw int32 sample, int32 j_start, int32 _j_end',
-    'raw int32 array',
-    '''
-        const int invalid = -1;
-        const int num = _ind.size();
-        int j = (sample[i] & 0x7fffffff) % num;
-        int j_end = _j_end;
-        if (j_end > num) j_end = num;
-        if (j == i || j < j_start || j >= j_end) continue;
-
-        // If a thread fails to do data swaping once, it changes j
-        // value using j_offset below and try data swaping again.
-        // This process is repeated until data swapping is succeeded.
-        // The j_offset is determined from the initial j
-        // (random number assigned to each thread) and the initial
-        // offset between j and i (ID of each thread).
-        // If a given number sequence in sample is really random,
-        // this j-update would not be necessary. This is work-around
-        // mainly to avoid potential eternal conflict when sample has
-        // rather synthetic number sequence.
-        int j_offset = ((2*j - i + num) % (num - 1)) + 1;
-
-        // A thread gives up to do data swapping if loop count exceed
-        // a threathod determined below. This is kind of safety
-        // mechanism to escape the eternal race condition, though I
-        // believe it never happens.
-        int loops = 256;
-
-        bool do_next = true;
-        while (do_next && loops > 0) {
-            // try to swap the contents of array[i] and array[j]
-            if (i != j) {
-                int val_j = atomicExch(&array[j], invalid);
-                if (val_j != invalid) {
-                    int val_i = atomicExch(&array[i], invalid);
-                    if (val_i != invalid) {
-                        array[i] = val_j;
-                        array[j] = val_i;
-                        do_next = false;
-                        // done
-                    }
-                    else {
-                        // restore array[j]
-                        array[j] = val_j;
-                    }
-                }
-            }
-            j = (j + j_offset) % num;
-            loops--;
-        }
-    ''',
-    'cupy_permutation',
-)
-
-
 def seed(seed=None):
     """Resets the state of the random number generator with a seed.
 
     This function resets the state of the global random number generator for
     the current device. Be careful that generators for other devices are not
     affected.
```

### Comparing `cupy-9.5.0/cupy/random/_generator_api.pyx` & `cupy-9.6.0/cupy/random/_generator_api.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/_kernels.py` & `cupy-9.6.0/cupy/random/_kernels.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/_permutations.py` & `cupy-9.6.0/cupy/random/_permutations.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/_sample.py` & `cupy-9.6.0/cupy/random/_sample.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/cupy_distributions.cu` & `cupy-9.6.0/cupy/random/cupy_distributions.cu`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/random/cupy_distributions.cuh` & `cupy-9.6.0/cupy/random/cupy_distributions.cuh`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/sparse/__init__.py` & `cupy-9.6.0/cupy/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/sparse/linalg/__init__.py` & `cupy-9.6.0/cupy/sparse/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/__init__.py` & `cupy-9.6.0/cupy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_array.py` & `cupy-9.6.0/cupy/testing/_array.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_attr.py` & `cupy-9.6.0/cupy/testing/_attr.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_bundle.py` & `cupy-9.6.0/cupy/testing/_bundle.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_condition.py` & `cupy-9.6.0/cupy/testing/_condition.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_helper.py` & `cupy-9.6.0/cupy/testing/_helper.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_hypothesis.py` & `cupy-9.6.0/cupy/testing/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_parameterized.py` & `cupy-9.6.0/cupy/testing/_parameterized.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_pytest_impl.py` & `cupy-9.6.0/cupy/testing/_pytest_impl.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy/testing/_random.py` & `cupy-9.6.0/cupy/testing/_random.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy.egg-info/PKG-INFO` & `cupy-9.6.0/cupy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupy
-Version: 9.5.0
+Version: 9.6.0
 Summary: CuPy: NumPy & SciPy for GPU
 Home-page: https://cupy.dev/
 Author: Seiya Tokui
 Author-email: tokui@preferred.jp
 Maintainer: CuPy Developers
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/cupy/cupy/issues
@@ -42,14 +42,15 @@
 ============================
 
 `CuPy <https://cupy.dev/>`_ is a NumPy/SciPy-compatible array library for GPU-accelerated computing with Python.
 
 This package (``cupy``) is a source distribution.
 For most users, use of pre-build wheel distributions are recommended:
 
+- `cupy-cuda115 <https://pypi.org/project/cupy-cuda115/>`_ (for CUDA 11.5)
 - `cupy-cuda114 <https://pypi.org/project/cupy-cuda114/>`_ (for CUDA 11.4)
 - `cupy-cuda113 <https://pypi.org/project/cupy-cuda113/>`_ (for CUDA 11.3)
 - `cupy-cuda112 <https://pypi.org/project/cupy-cuda112/>`_ (for CUDA 11.2)
 - `cupy-cuda111 <https://pypi.org/project/cupy-cuda111/>`_ (for CUDA 11.1)
 - `cupy-cuda110 <https://pypi.org/project/cupy-cuda110/>`_ (for CUDA 11.0)
 - `cupy-cuda102 <https://pypi.org/project/cupy-cuda102/>`_ (for CUDA 10.2)
 - `cupy-cuda101 <https://pypi.org/project/cupy-cuda101/>`_ (for CUDA 10.1)
```

### Comparing `cupy-9.5.0/cupy.egg-info/SOURCES.txt` & `cupy-9.6.0/cupy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,24 +95,20 @@
 cupy/_core/include/cupy/_cuda/README.md
 cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.h
 cupy/_core/include/cupy/_cuda/cuda-10.0/cuda_fp16.hpp
 cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.h
 cupy/_core/include/cupy/_cuda/cuda-10.1/cuda_fp16.hpp
 cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.h
 cupy/_core/include/cupy/_cuda/cuda-10.2/cuda_fp16.hpp
+cupy/_core/include/cupy/_cuda/cuda-11/cuda_fp16.h
+cupy/_core/include/cupy/_cuda/cuda-11/cuda_fp16.hpp
 cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.h
 cupy/_core/include/cupy/_cuda/cuda-11.0/cuda_fp16.hpp
 cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.h
 cupy/_core/include/cupy/_cuda/cuda-11.1/cuda_fp16.hpp
-cupy/_core/include/cupy/_cuda/cuda-11.2/cuda_fp16.h
-cupy/_core/include/cupy/_cuda/cuda-11.2/cuda_fp16.hpp
-cupy/_core/include/cupy/_cuda/cuda-11.3/cuda_fp16.h
-cupy/_core/include/cupy/_cuda/cuda-11.3/cuda_fp16.hpp
-cupy/_core/include/cupy/_cuda/cuda-11.4/cuda_fp16.h
-cupy/_core/include/cupy/_cuda/cuda-11.4/cuda_fp16.hpp
 cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.h
 cupy/_core/include/cupy/_cuda/cuda-9.2/cuda_fp16.hpp
 cupy/_core/include/cupy/complex/README.md
 cupy/_core/include/cupy/complex/arithmetic.h
 cupy/_core/include/cupy/complex/catrig.h
 cupy/_core/include/cupy/complex/catrigf.h
 cupy/_core/include/cupy/complex/ccosh.h
```

### Comparing `cupy-9.5.0/cupy_backends/cuda/api/driver.pxd` & `cupy-9.6.0/cupy_backends/cuda/api/driver.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/api/driver.pyx` & `cupy-9.6.0/cupy_backends/cuda/api/driver.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/api/runtime.pxd` & `cupy-9.6.0/cupy_backends/cuda/api/runtime.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/api/runtime.pyx` & `cupy-9.6.0/cupy_backends/cuda/api/runtime.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/cupy_cudnn.h` & `cupy-9.6.0/cupy_backends/cuda/cupy_cudnn.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/cupy_cusolver.h` & `cupy-9.6.0/cupy_backends/cuda/cupy_cusolver.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/cupy_cusparse.h` & `cupy-9.6.0/cupy_backends/cuda/cupy_cusparse.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/cupy_cusparselt.h` & `cupy-9.6.0/cupy_backends/cuda/cupy_cusparselt.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/cupy_nvrtc.h` & `cupy-9.6.0/cupy_backends/cuda/cupy_nvrtc.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cublas.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/cublas.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cublas.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cublas.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cudnn.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/cudnn.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cudnn.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cudnn.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cugraph.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cugraph.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/curand.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/curand.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/curand.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/curand.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cusolver.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/cusolver.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cusolver.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cusolver.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cusparse.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/cusparse.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cusparse.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cusparse.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cusparselt.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/cusparselt.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cusparselt.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cusparselt.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cutensor.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/cutensor.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/cutensor.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/cutensor.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/nccl.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/nccl.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/nvrtc.pxd` & `cupy-9.6.0/cupy_backends/cuda/libs/nvrtc.pxd`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/nvrtc.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/nvrtc.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/nvtx.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/nvtx.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/libs/profiler.pyx` & `cupy-9.6.0/cupy_backends/cuda/libs/profiler.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cuda/stream.pyx` & `cupy-9.6.0/cupy_backends/cuda/stream.pyx`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cupy_cudnn.h` & `cupy-9.6.0/cupy_backends/cupy_cudnn.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cupy_cugraph.h` & `cupy-9.6.0/cupy_backends/cupy_cugraph.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cupy_lapack.h` & `cupy-9.6.0/cupy_backends/cupy_lapack.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/cupy_nccl.h` & `cupy-9.6.0/cupy_backends/cupy_nccl.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_hip.h` & `cupy-9.6.0/cupy_backends/hip/cupy_hip.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_hip_common.h` & `cupy-9.6.0/cupy_backends/hip/cupy_hip_common.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_hip_runtime.h` & `cupy-9.6.0/cupy_backends/hip/cupy_hip_runtime.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_hipblas.h` & `cupy-9.6.0/cupy_backends/hip/cupy_hipblas.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_hiprand.h` & `cupy-9.6.0/cupy_backends/hip/cupy_hiprand.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_hiprtc.h` & `cupy-9.6.0/cupy_backends/hip/cupy_hiprtc.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_rocsolver.h` & `cupy-9.6.0/cupy_backends/hip/cupy_rocsolver.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/hip/cupy_roctx.h` & `cupy-9.6.0/cupy_backends/hip/cupy_roctx.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cublas.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cublas.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cuda.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cuda.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cuda_common.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cuda_common.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cuda_runtime.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cuda_runtime.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cudnn.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cudnn.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cugraph.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cugraph.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_curand.h` & `cupy-9.6.0/cupy_backends/stub/cupy_curand.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cusolver.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cusolver.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cusparse.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cusparse.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cusparselt.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cusparselt.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_cutensor.h` & `cupy-9.6.0/cupy_backends/stub/cupy_cutensor.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_nccl.h` & `cupy-9.6.0/cupy_backends/stub/cupy_nccl.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_nvrtc.h` & `cupy-9.6.0/cupy_backends/stub/cupy_nvrtc.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_backends/stub/cupy_nvtx.h` & `cupy-9.6.0/cupy_backends/stub/cupy_nvtx.h`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupy_setup_build.py` & `cupy-9.6.0/cupy_setup_build.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/__init__.py` & `cupy-9.6.0/cupyx/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/_pinned_array.py` & `cupy-9.6.0/cupyx/_pinned_array.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/_runtime.py` & `cupy-9.6.0/cupyx/_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,22 @@
             ('cuDNN Version', self.cudnn_version),
             ('NCCL Build Version', self.nccl_build_version),
             ('NCCL Runtime Version', self.nccl_runtime_version),
             ('cuTENSOR Version', self.cutensor_version),
             ('cuSPARSELt Build Version', self.cusparselt_version),
         ]
 
-        for device_id in range(cupy.cuda.runtime.getDeviceCount()):
+        device_count = 0
+        try:
+            device_count = cupy.cuda.runtime.getDeviceCount()
+        except cupy.cuda.runtime.CUDARuntimeError as e:
+            if 'ErrorNoDevice' not in e.args[0]:
+                raise
+            # No GPU devices available.
+        for device_id in range(device_count):
             with cupy.cuda.Device(device_id) as device:
                 props = cupy.cuda.runtime.getDeviceProperties(device_id)
                 name = ('Device {} Name'.format(device_id),
                         props['name'].decode())
                 pci_bus = ('Device {} PCI Bus ID'.format(device_id),
                            device.pci_bus_id)
                 if is_hip:
```

### Comparing `cupy-9.5.0/cupyx/_scatter.py` & `cupy-9.6.0/cupyx/_scatter.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/_ufunc_config.py` & `cupy-9.6.0/cupyx/_ufunc_config.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/fallback_mode/fallback.py` & `cupy-9.6.0/cupyx/fallback_mode/fallback.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/fallback_mode/notification.py` & `cupy-9.6.0/cupyx/fallback_mode/notification.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/jit/_builtin_funcs.py` & `cupy-9.6.0/cupyx/jit/_builtin_funcs.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/jit/_compile.py` & `cupy-9.6.0/cupyx/jit/_compile.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/jit/_cuda_typerules.py` & `cupy-9.6.0/cupyx/jit/_cuda_typerules.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/jit/_cuda_types.py` & `cupy-9.6.0/cupyx/jit/_cuda_types.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/jit/_interface.py` & `cupy-9.6.0/cupyx/jit/_interface.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/jit/_internal_types.py` & `cupy-9.6.0/cupyx/jit/_internal_types.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/lapack.py` & `cupy-9.6.0/cupyx/lapack.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/linalg/_solve.py` & `cupy-9.6.0/cupyx/linalg/_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/linalg/sparse/_solve.py` & `cupy-9.6.0/cupyx/linalg/sparse/_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/optimizing/_optimize.py` & `cupy-9.6.0/cupyx/optimizing/_optimize.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/__init__.py` & `cupy-9.6.0/cupyx/scipy/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/fft/_fft.py` & `cupy-9.6.0/cupyx/scipy/fft/_fft.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/fft/_helper.py` & `cupy-9.6.0/cupyx/scipy/fft/_helper.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/fftpack/_fft.py` & `cupy-9.6.0/cupyx/scipy/fftpack/_fft.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/linalg/decomp_lu.py` & `cupy-9.6.0/cupyx/scipy/linalg/decomp_lu.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/linalg/solve_triangular.py` & `cupy-9.6.0/cupyx/scipy/linalg/solve_triangular.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/linalg/special_matrices.py` & `cupy-9.6.0/cupyx/scipy/linalg/special_matrices.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/__init__.py` & `cupy-9.6.0/cupyx/scipy/ndimage/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/_filters_core.py` & `cupy-9.6.0/cupyx/scipy/ndimage/_filters_core.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/_filters_generic.py` & `cupy-9.6.0/cupyx/scipy/ndimage/_filters_generic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/_interp_kernels.py` & `cupy-9.6.0/cupyx/scipy/ndimage/_interp_kernels.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/_spline_kernel_weights.py` & `cupy-9.6.0/cupyx/scipy/ndimage/_spline_kernel_weights.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/_spline_prefilter_core.py` & `cupy-9.6.0/cupyx/scipy/ndimage/_spline_prefilter_core.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/_util.py` & `cupy-9.6.0/cupyx/scipy/ndimage/_util.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/filters.py` & `cupy-9.6.0/cupyx/scipy/ndimage/filters.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/fourier.py` & `cupy-9.6.0/cupyx/scipy/ndimage/fourier.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/interpolation.py` & `cupy-9.6.0/cupyx/scipy/ndimage/interpolation.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/measurements.py` & `cupy-9.6.0/cupyx/scipy/ndimage/measurements.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/ndimage/morphology.py` & `cupy-9.6.0/cupyx/scipy/ndimage/morphology.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/signal/__init__.py` & `cupy-9.6.0/cupyx/scipy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/signal/_signaltools_core.py` & `cupy-9.6.0/cupyx/scipy/signal/_signaltools_core.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/signal/bsplines.py` & `cupy-9.6.0/cupyx/scipy/signal/bsplines.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/signal/signaltools.py` & `cupy-9.6.0/cupyx/scipy/signal/signaltools.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/__init__.py` & `cupy-9.6.0/cupyx/scipy/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/_index.py` & `cupy-9.6.0/cupyx/scipy/sparse/_index.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/base.py` & `cupy-9.6.0/cupyx/scipy/sparse/base.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/compressed.py` & `cupy-9.6.0/cupyx/scipy/sparse/compressed.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/construct.py` & `cupy-9.6.0/cupyx/scipy/sparse/construct.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/coo.py` & `cupy-9.6.0/cupyx/scipy/sparse/coo.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/csc.py` & `cupy-9.6.0/cupyx/scipy/sparse/csc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/csgraph/_traversal.py` & `cupy-9.6.0/cupyx/scipy/sparse/csgraph/_traversal.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/csr.py` & `cupy-9.6.0/cupyx/scipy/sparse/csr.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/data.py` & `cupy-9.6.0/cupyx/scipy/sparse/data.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/dia.py` & `cupy-9.6.0/cupyx/scipy/sparse/dia.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/extract.py` & `cupy-9.6.0/cupyx/scipy/sparse/extract.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/__init__.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/_eigen.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/_eigen.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/_interface.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/_interface.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/_iterative.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/_iterative.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/_lobpcg.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/_lobpcg.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/_norm.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/_norm.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/linalg/_solve.py` & `cupy-9.6.0/cupyx/scipy/sparse/linalg/_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/sparse/sputils.py` & `cupy-9.6.0/cupyx/scipy/sparse/sputils.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/__init__.py` & `cupy-9.6.0/cupyx/scipy/special/__init__.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_bessel.py` & `cupy-9.6.0/cupyx/scipy/special/_bessel.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_convex_analysis.py` & `cupy-9.6.0/cupyx/scipy/special/_convex_analysis.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_digamma.py` & `cupy-9.6.0/cupyx/scipy/special/_digamma.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_erf.py` & `cupy-9.6.0/cupyx/scipy/special/_erf.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_gamma.py` & `cupy-9.6.0/cupyx/scipy/special/_gamma.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_gammaln.py` & `cupy-9.6.0/cupyx/scipy/special/_gammaln.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_polygamma.py` & `cupy-9.6.0/cupyx/scipy/special/_polygamma.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/special/_zeta.py` & `cupy-9.6.0/cupyx/scipy/special/_zeta.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/scipy/stats/distributions.py` & `cupy-9.6.0/cupyx/scipy/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/time.py` & `cupy-9.6.0/cupyx/time.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/cupyx/tools/install_library.py` & `cupy-9.6.0/cupyx/tools/install_library.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Keep the script runnable without CuPy dependency.
 
 import argparse
 import json
 import os
 import platform
 import shutil
+import subprocess
 import sys
 import tempfile
 import urllib.request
 
 
 _cudnn_records = []
 _cutensor_records = []
@@ -63,14 +64,18 @@
             },
         }
     }
 
 
 # Latest cuDNN versions: https://developer.nvidia.com/rdp/cudnn-download
 _cudnn_records.append(_make_cudnn_record(
+    '11.5', '8.2.4',
+    'cudnn-11.4-linux-x64-v8.2.4.15.tgz',
+    'cudnn-11.4-windows-x64-v8.2.4.15.zip'))
+_cudnn_records.append(_make_cudnn_record(
     '11.4', '8.2.4',
     'cudnn-11.4-linux-x64-v8.2.4.15.tgz',
     'cudnn-11.4-windows-x64-v8.2.4.15.zip'))
 _cudnn_records.append(_make_cudnn_record(
     '11.3', '8.2.4',
     'cudnn-11.4-linux-x64-v8.2.4.15.tgz',
     'cudnn-11.4-windows-x64-v8.2.4.15.zip'))
@@ -101,63 +106,74 @@
 _cudnn_records.append(_make_cudnn_record(
     '9.2', '7.6.5',
     'cudnn-9.2-linux-x64-v7.6.5.32.tgz',
     'cudnn-9.2-windows10-x64-v7.6.5.32.zip'))
 library_records['cudnn'] = _cudnn_records
 
 
-def _make_cutensor_url(public_version, filename):
-    # https://developer.download.nvidia.com/compute/cutensor/1.2.2/local_installers/libcutensor-linux-x86_64-1.2.2.5.tar.gz
+def _make_cutensor_url(platform, public_version, filename):
+    if public_version.startswith('1.2.'):
+        return (
+            'https://developer.download.nvidia.com/compute/cutensor/'
+            f'{public_version}/local_installers/{filename}')
+
+    # https://developer.download.nvidia.com/compute/cutensor/redist/libcutensor/linux-x86_64/libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz
     return (
         'https://developer.download.nvidia.com/compute/cutensor/' +
-        '{}/local_installers/{}'.format(public_version, filename))
+        f'redist/libcutensor/{platform}-x86_64/{filename}')
 
 
 def _make_cutensor_record(
         cuda_version, public_version, filename_linux, filename_windows):
     return {
         'cuda': cuda_version,
         'cutensor': public_version,
         'assets': {
             'Linux': {
-                'url': _make_cutensor_url(public_version, filename_linux),
+                'url': _make_cutensor_url(
+                    'linux', public_version, filename_linux),
                 'filenames': ['libcutensor.so.{}'.format(public_version)],
             },
             'Windows': {
-                'url': _make_cutensor_url(public_version, filename_windows),
+                'url': _make_cutensor_url(
+                    'windows', public_version, filename_windows),
                 'filenames': ['cutensor.dll'],
             },
         }
     }
 
 
 _cutensor_records.append(_make_cutensor_record(
-    '11.4', '1.3.1',
-    'libcutensor-linux-x86_64-1.3.1.3.tar.gz',
-    'libcutensor-windows-x86_64-1.3.1.3.zip'))
+    '11.5', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
 _cutensor_records.append(_make_cutensor_record(
-    '11.3', '1.3.1',
-    'libcutensor-linux-x86_64-1.3.1.3.tar.gz',
-    'libcutensor-windows-x86_64-1.3.1.3.zip'))
+    '11.4', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
 _cutensor_records.append(_make_cutensor_record(
-    '11.2', '1.3.1',
-    'libcutensor-linux-x86_64-1.3.1.3.tar.gz',
-    'libcutensor-windows-x86_64-1.3.1.3.zip'))
+    '11.3', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
 _cutensor_records.append(_make_cutensor_record(
-    '11.1', '1.3.1',
-    'libcutensor-linux-x86_64-1.3.1.3.tar.gz',
-    'libcutensor-windows-x86_64-1.3.1.3.zip'))
+    '11.2', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
 _cutensor_records.append(_make_cutensor_record(
-    '11.0', '1.3.1',
-    'libcutensor-linux-x86_64-1.3.1.3.tar.gz',
-    'libcutensor-windows-x86_64-1.3.1.3.zip'))
+    '11.1', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
 _cutensor_records.append(_make_cutensor_record(
-    '10.2', '1.3.1',
-    'libcutensor-linux-x86_64-1.3.1.3.tar.gz',
-    'libcutensor-windows-x86_64-1.3.1.3.zip'))
+    '11.0', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
+_cutensor_records.append(_make_cutensor_record(
+    '10.2', '1.3.3',
+    'libcutensor-linux-x86_64-1.3.3.2-archive.tar.xz',
+    'libcutensor-windows-x86_64-1.3.3.2-archive.zip'))
 _cutensor_records.append(_make_cutensor_record(
     '10.1', '1.2.2',
     'libcutensor-linux-x86_64-1.2.2.5.tar.gz',
     'libcutensor-windows-x86_64-1.2.2.5.zip'))
 library_records['cutensor'] = _cutensor_records
 
 
@@ -179,14 +195,17 @@
                 'filenames': ['libnccl.so.{}'.format(full_version)],
             },
         },
     }
 
 
 _nccl_records.append(_make_nccl_record(
+    '11.5', '2.11.4', '2.11',
+    'nccl_2.11.4-1+cuda11.4_x86_64.txz'))
+_nccl_records.append(_make_nccl_record(
     '11.4', '2.11.4', '2.11',
     'nccl_2.11.4-1+cuda11.4_x86_64.txz'))
 _nccl_records.append(_make_nccl_record(
     '11.3', '2.9.9', '2.9',
     'nccl_2.9.9-1+cuda11.3_x86_64.txz'))
 _nccl_records.append(_make_nccl_record(
     '11.2', '2.8.4', '2.8',
@@ -233,44 +252,79 @@
 
     target_platform = platform.system()
     asset = record['assets'].get(target_platform, None)
     if asset is None:
         raise RuntimeError('''
 The current platform ({}) is not supported.'''.format(target_platform))
 
+    if library == 'cudnn':
+        print('By downloading and using cuDNN, you accept the terms and'
+              ' conditions of the NVIDIA cuDNN Software License Agreement:')
+        print('  https://docs.nvidia.com/deeplearning/cudnn/sla/index.html')
+        print()
+    elif library == 'cutensor':
+        print('By downloading and using cuTENSOR, you accept the terms and'
+              ' conditions of the NVIDIA cuTENSOR Software License Agreement:')
+        print('  https://docs.nvidia.com/cuda/cutensor/license.html')
+        print()
+    elif library == 'nccl':
+        pass  # BSD
+    else:
+        assert False
+
     print('Installing {} {} for CUDA {} to: {}'.format(
         library, record[library], record['cuda'], destination))
 
     url = asset['url']
     print('Downloading {}...'.format(url))
     with tempfile.TemporaryDirectory() as tmpdir:
         with open(os.path.join(tmpdir, os.path.basename(url)), 'wb') as f:
             with urllib.request.urlopen(url) as response:
                 f.write(response.read())
         print('Extracting...')
         outdir = os.path.join(tmpdir, 'extract')
-        shutil.unpack_archive(f.name, outdir)
+        try:
+            shutil.unpack_archive(f.name, outdir)
+        except shutil.ReadError:
+            print('The archive format is not supported in your Python '
+                  'environment. Falling back to "tar" command...')
+            try:
+                os.makedirs(outdir, exist_ok=True)
+                subprocess.run(['tar', 'xf', f.name, '-C', outdir], check=True)
+            except subprocess.CalledProcessError:
+                msg = 'Failed to extract the archive using "tar" command.'
+                raise RuntimeError(msg)
         print('Installing...')
         if library == 'cudnn':
             shutil.move(os.path.join(outdir, 'cuda'), destination)
         elif library == 'cutensor':
             if cuda.startswith('11.') and cuda != '11.0':
                 cuda = '11'
+            if cuda == '10.1':
+                # cuTENSOR 1.2
+                dir_name = 'libcutensor'
+                license = 'license.pdf'
+            else:
+                if target_platform == 'Linux':
+                    ext = '.tar.xz'
+                elif target_platform == 'Windows':
+                    ext = '.zip'
+                else:
+                    assert False
+                assert url.endswith(ext)
+                dir_name = os.path.basename(url)[:-len(ext)]
+                license = 'LICENSE'
             shutil.move(
-                os.path.join(outdir, 'libcutensor', 'include'),
+                os.path.join(outdir, dir_name, 'include'),
                 os.path.join(destination, 'include'))
             shutil.move(
-                os.path.join(outdir, 'libcutensor', 'lib', cuda),
+                os.path.join(outdir, dir_name, 'lib', cuda),
                 os.path.join(destination, 'lib'))
-            if cuda == '10.1':
-                license = 'license.pdf'  # v1.2.2
-            else:
-                license = 'license.txt'  # v1.3.0
             shutil.move(
-                os.path.join(outdir, 'libcutensor', license), destination)
+                os.path.join(outdir, dir_name, license), destination)
         elif library == 'nccl':
             subdir = os.listdir(outdir)  # ['nccl_2.8.4-1+cuda11.2_x86_64']
             assert len(subdir) == 1
             shutil.move(os.path.join(outdir, subdir[0]), destination)
         else:
             assert False
         print('Cleaning up...')
```

### Comparing `cupy-9.5.0/docs/LICENSE_THIRD_PARTY` & `cupy-9.6.0/docs/LICENSE_THIRD_PARTY`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/docs/source/license.rst` & `cupy-9.6.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/install/build.py` & `cupy-9.6.0/install/build.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/install/utils.py` & `cupy-9.6.0/install/utils.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/setup.cfg` & `cupy-9.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/setup.py` & `cupy-9.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/conftest.py` & `cupy-9.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/binary_tests/test_elementwise.py` & `cupy-9.6.0/tests/cupy_tests/binary_tests/test_elementwise.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/binary_tests/test_packing.py` & `cupy-9.6.0/tests/cupy_tests/binary_tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/fusion_utils.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/fusion_utils.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_array.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_array.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_example.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_example.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_indexing.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_kernel_cache.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_kernel_cache.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_misc.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_optimization.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_reduction.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_reduction.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_routines.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/fusion_tests/test_ufunc.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/fusion_tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_array_function.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_array_function.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_carray.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_carray.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_core.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_core.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_cub_reduction.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_cub_reduction.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_dlpack.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_dlpack.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_elementwise.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_elementwise.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_flags.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_function.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_function.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_internal.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_iter.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_adv_indexing.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_adv_indexing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_complex_ops.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_complex_ops.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_conversion.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_conversion.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_copy_and_view.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_copy_and_view.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_cuda_array_interface.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_cuda_array_interface.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_elementwise_op.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_elementwise_op.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_get.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_get.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_indexing.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_indexing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_math.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_math.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_reduction.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_reduction.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_scatter.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_scatter.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_ufunc.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_ufunc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_ndarray_unary_op.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_ndarray_unary_op.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_raw.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_reduction.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_reduction.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_scan.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_syncdetect.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_syncdetect.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/core_tests/test_userkernel.py` & `cupy-9.6.0/tests/cupy_tests/core_tests/test_userkernel.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/creation_tests/test_basic.py` & `cupy-9.6.0/tests/cupy_tests/creation_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/creation_tests/test_from_data.py` & `cupy-9.6.0/tests/cupy_tests/creation_tests/test_from_data.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/creation_tests/test_matrix.py` & `cupy-9.6.0/tests/cupy_tests/creation_tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/creation_tests/test_ranges.py` & `cupy-9.6.0/tests/cupy_tests/creation_tests/test_ranges.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_debug_print.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_debug_print.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_line_profile.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/memory_hooks_tests/test_line_profile.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_compiler.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_cufft.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_cufft.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_curand.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_curand.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_device.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_device.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_driver.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_memory.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_memory_hook.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_memory_hook.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_nccl.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_nccl.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_nvtx.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_nvtx.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_pinned_memory.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_pinned_memory.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_profile.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_stream.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/cuda_tests/test_texture.py` & `cupy-9.6.0/tests/cupy_tests/cuda_tests/test_texture.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/fft_tests/test_cache.py` & `cupy-9.6.0/tests/cupy_tests/fft_tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/fft_tests/test_callback.py` & `cupy-9.6.0/tests/cupy_tests/fft_tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/fft_tests/test_fft.py` & `cupy-9.6.0/tests/cupy_tests/fft_tests/test_fft.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,16 @@
             a.append(cupy.empty(100000000))
         del a
         b = cupy.empty(100000007, dtype=cupy.float32)
         cupy.fft.fft(b)
         # Free huge memory for slow test
         del b
         cupy.get_default_memory_pool().free_all_blocks()
+        # Clean up FFT plan cache
+        cupy.fft.config.clear_plan_cache()
 
 
 @pytest.mark.usefixtures('skip_forward_backward')
 @testing.parameterize(*(
     testing.product_dict([
         {'shape': (3, 4), 's': None, 'axes': None},
         {'shape': (3, 4), 's': (1, None), 'axes': None},
```

### Comparing `cupy-9.5.0/tests/cupy_tests/functional_tests/test_piecewise.py` & `cupy-9.6.0/tests/cupy_tests/functional_tests/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/functional_tests/test_vectorize.py` & `cupy-9.6.0/tests/cupy_tests/functional_tests/test_vectorize.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/indexing_tests/test_generate.py` & `cupy-9.6.0/tests/cupy_tests/indexing_tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/indexing_tests/test_indexing.py` & `cupy-9.6.0/tests/cupy_tests/indexing_tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/indexing_tests/test_insert.py` & `cupy-9.6.0/tests/cupy_tests/indexing_tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/indexing_tests/test_iterate.py` & `cupy-9.6.0/tests/cupy_tests/indexing_tests/test_iterate.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/io_tests/test_base_n.py` & `cupy-9.6.0/tests/cupy_tests/io_tests/test_base_n.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/io_tests/test_npz.py` & `cupy-9.6.0/tests/cupy_tests/io_tests/test_npz.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/lib_tests/test_polynomial.py` & `cupy-9.6.0/tests/cupy_tests/lib_tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/lib_tests/test_shape_base.py` & `cupy-9.6.0/tests/cupy_tests/lib_tests/test_shape_base.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/lib_tests/test_strided_tricks.py` & `cupy-9.6.0/tests/cupy_tests/lib_tests/test_strided_tricks.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/linalg_tests/test_decomposition.py` & `cupy-9.6.0/tests/cupy_tests/linalg_tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/linalg_tests/test_eigenvalue.py` & `cupy-9.6.0/tests/cupy_tests/linalg_tests/test_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/linalg_tests/test_einsum.py` & `cupy-9.6.0/tests/cupy_tests/linalg_tests/test_einsum.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/linalg_tests/test_norms.py` & `cupy-9.6.0/tests/cupy_tests/linalg_tests/test_norms.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/linalg_tests/test_product.py` & `cupy-9.6.0/tests/cupy_tests/linalg_tests/test_product.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/linalg_tests/test_solve.py` & `cupy-9.6.0/tests/cupy_tests/linalg_tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/logic_tests/test_comparison.py` & `cupy-9.6.0/tests/cupy_tests/logic_tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/logic_tests/test_content.py` & `cupy-9.6.0/tests/cupy_tests/logic_tests/test_content.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/logic_tests/test_ops.py` & `cupy-9.6.0/tests/cupy_tests/logic_tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/logic_tests/test_truth.py` & `cupy-9.6.0/tests/cupy_tests/logic_tests/test_truth.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/logic_tests/test_type_test.py` & `cupy-9.6.0/tests/cupy_tests/logic_tests/test_type_test.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_add_remove.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_add_remove.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_basic.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_dims.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_dims.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_join.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_join.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_kind.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_rearrange.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_rearrange.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_shape.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_shape.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,14 +166,33 @@
     @testing.for_orders('CFA')
     @testing.numpy_cupy_array_equal()
     def test_ravel3(self, xp, order):
         a = testing.shaped_arange((2, 3, 4), xp)
         a = xp.asfortranarray(a)
         return a.ravel(order)
 
+    @testing.for_orders('CFA')
+    @testing.numpy_cupy_array_equal()
+    def test_ravel_non_contiguous(self, xp, order):
+        a = xp.arange(10)[::2]
+        assert not a.flags.c_contiguous and not a.flags.f_contiguous
+        b = a.ravel(order)
+        assert b.flags.c_contiguous
+        return b
+
+    @testing.for_orders('CFA')
+    @testing.numpy_cupy_array_equal()
+    def test_ravel_broadcasted(self, xp, order):
+        a = xp.array([1])
+        b = xp.broadcast_to(a, (10,))
+        assert not b.flags.c_contiguous and not b.flags.f_contiguous
+        b = b.ravel(order)
+        assert b.flags.c_contiguous
+        return b
+
     @testing.numpy_cupy_array_equal()
     def test_external_ravel(self, xp):
         a = testing.shaped_arange((2, 3, 4), xp)
         a = a.transpose(2, 0, 1)
         return xp.ravel(a)
```

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_split.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_split.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_tiling.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_tiling.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/manipulation_tests/test_transpose.py` & `cupy-9.6.0/tests/cupy_tests/manipulation_tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_arithmetic.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_explog.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_explog.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_floating.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_floating.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_hyperbolic.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_hyperbolic.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_matmul.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_matmul.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_misc.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_rational.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_rational.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_rounding.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_rounding.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_special.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_special.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_sumprod.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_sumprod.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_trigonometric.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_trigonometric.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/math_tests/test_window.py` & `cupy-9.6.0/tests/cupy_tests/math_tests/test_window.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/misc_tests/test_memory_ranges.py` & `cupy-9.6.0/tests/cupy_tests/misc_tests/test_memory_ranges.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/misc_tests/test_who.py` & `cupy-9.6.0/tests/cupy_tests/misc_tests/test_who.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/padding_tests/test_pad.py` & `cupy-9.6.0/tests/cupy_tests/padding_tests/test_pad.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/polynomial_tests/test_polynomial.py` & `cupy-9.6.0/tests/cupy_tests/polynomial_tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/polynomial_tests/test_polyutils.py` & `cupy-9.6.0/tests/cupy_tests/polynomial_tests/test_polyutils.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/prof_tests/test_range.py` & `cupy-9.6.0/tests/cupy_tests/prof_tests/test_range.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/common_distributions.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/common_distributions.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/test_bit_generator.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/test_bit_generator.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/test_distributions.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/test_generator.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/test_generator_api.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/test_generator_api.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/test_permutations.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/test_permutations.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/random_tests/test_sample.py` & `cupy-9.6.0/tests/cupy_tests/random_tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/sorting_tests/test_count.py` & `cupy-9.6.0/tests/cupy_tests/sorting_tests/test_count.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/sorting_tests/test_search.py` & `cupy-9.6.0/tests/cupy_tests/sorting_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/sorting_tests/test_sort.py` & `cupy-9.6.0/tests/cupy_tests/sorting_tests/test_sort.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/statistics_tests/test_correlation.py` & `cupy-9.6.0/tests/cupy_tests/statistics_tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/statistics_tests/test_histogram.py` & `cupy-9.6.0/tests/cupy_tests/statistics_tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/statistics_tests/test_meanvar.py` & `cupy-9.6.0/tests/cupy_tests/statistics_tests/test_meanvar.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/statistics_tests/test_order.py` & `cupy-9.6.0/tests/cupy_tests/statistics_tests/test_order.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_cublas.py` & `cupy-9.6.0/tests/cupy_tests/test_cublas.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_cudnn.py` & `cupy-9.6.0/tests/cupy_tests/test_cudnn.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_cusolver.py` & `cupy-9.6.0/tests/cupy_tests/test_cusolver.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_cusparse.py` & `cupy-9.6.0/tests/cupy_tests/test_cusparse.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_cutensor.py` & `cupy-9.6.0/tests/cupy_tests/test_cutensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -165,14 +165,36 @@
             self.beta * c_orig,
             d,
             rtol=self.tol, atol=self.tol
         )
 
 
 @pytest.mark.skipif(not ct.available, reason='cuTensor is unavailable')
+class TestMode:
+
+    def test_create_mode_int(self):
+        m = cutensor.create_mode(10, 11, 12)
+        assert m.ndim == 3
+        assert repr(m) == 'mode(10, 11, 12)'
+
+    def test_create_mode_ascii(self):
+        m = cutensor.create_mode('x', 'y')
+        assert m.ndim == 2
+        assert repr(m) == 'mode(120, 121)'
+
+
+@pytest.mark.skipif(not ct.available, reason='cuTensor is unavailable')
+class TestScalar:
+
+    def test_create(self):
+        s = cutensor._Scalar(10, cupy.float32)
+        assert repr(s) == 'scalar(10.0, dtype=float32)'
+
+
+@pytest.mark.skipif(not ct.available, reason='cuTensor is unavailable')
 class TestCuTensorDescriptor:
 
     @pytest.fixture(autouse=True)
     def setUp(self):
         self.a = testing.shaped_random(
             (20, 40, 30), cupy, numpy.float32, seed=0)
         self.b = testing.shaped_random(
```

### Comparing `cupy-9.5.0/tests/cupy_tests/test_init.py` & `cupy-9.6.0/tests/cupy_tests/test_init.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_ndim.py` & `cupy-9.6.0/tests/cupy_tests/test_ndim.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_numpy_interop.py` & `cupy-9.6.0/tests/cupy_tests/test_numpy_interop.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/test_type_routines.py` & `cupy-9.6.0/tests/cupy_tests/test_type_routines.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/testing_tests/test_array.py` & `cupy-9.6.0/tests/cupy_tests/testing_tests/test_array.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/testing_tests/test_condition.py` & `cupy-9.6.0/tests/cupy_tests/testing_tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/testing_tests/test_helper.py` & `cupy-9.6.0/tests/cupy_tests/testing_tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupy_tests/testing_tests/test_parameterized.py` & `cupy-9.6.0/tests/cupy_tests/testing_tests/test_parameterized.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/fallback_mode_tests/test_fallback.py` & `cupy-9.6.0/tests/cupyx_tests/fallback_mode_tests/test_fallback.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/fallback_mode_tests/test_notifications.py` & `cupy-9.6.0/tests/cupyx_tests/fallback_mode_tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/jit_tests/test_raw.py` & `cupy-9.6.0/tests/cupyx_tests/jit_tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/linalg_tests/sparse_tests/test_solve.py` & `cupy-9.6.0/tests/cupyx_tests/linalg_tests/sparse_tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/linalg_tests/test_solve.py` & `cupy-9.6.0/tests/cupyx_tests/linalg_tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/fft_tests/test_fft.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/fft_tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/fft_tests/test_helper.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/fft_tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/fftpack_tests/test_fftpack.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/fftpack_tests/test_fftpack.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_decomp_lu.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_decomp_lu.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_solve_triangular.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_solve_triangular.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_special_matrices.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/linalg_tests/test_special_matrices.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_filters.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_fourier.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_interpolation.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_measurements.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_measurements.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_morphology.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/ndimage_tests/test_morphology.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/signal_tests/test_bsplines.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/signal_tests/test_bsplines.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/signal_tests/test_signaltools.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/signal_tests/test_signaltools.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/csgraph_tests/test_traversal.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/csgraph_tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_base.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_base.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_construct.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_construct.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_coo.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_coo.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csc.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csc.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csr.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_csr.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_dia.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_dia.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_extract.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_index.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_index.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_linalg.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/sparse_tests/test_linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     'k': [3, 6, 12],
     'return_vectors': [True, False],
     'use_linear_operator': [True, False],
 }))
 @testing.with_requires('scipy')
 class TestSvds:
     density = 0.33
-    tol = {numpy.float32: 1e-4, numpy.complex64: 1e-4, 'default': 1e-12}
+    tol = {numpy.float32: 1e-4, numpy.complex64: 2e-4, 'default': 1e-12}
 
     def _make_matrix(self, dtype, xp):
         a = testing.shaped_random(self.shape, xp, dtype=dtype)
         mask = testing.shaped_random(self.shape, xp, dtype='f', scale=1)
         a[mask > self.density] = 0
         return a
```

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_bessel.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_bessel.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_convex_analysis.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_convex_analysis.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_digamma.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_digamma.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_erf.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_erf.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_gamma.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_gammaln.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_gammaln.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_polygamma.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_polygamma.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_statistics.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/special_tests/test_zeta.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/special_tests/test_zeta.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/stats_tests/test_distributions.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/stats_tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/scipy_tests/test_get_array_module.py` & `cupy-9.6.0/tests/cupyx_tests/scipy_tests/test_get_array_module.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_cupyx.py` & `cupy-9.6.0/tests/cupyx_tests/test_cupyx.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_lapack.py` & `cupy-9.6.0/tests/cupyx_tests/test_lapack.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_optimize.py` & `cupy-9.6.0/tests/cupyx_tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_pinned_array.py` & `cupy-9.6.0/tests/cupyx_tests/test_pinned_array.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_runtime.py` & `cupy-9.6.0/tests/cupyx_tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_scatter.py` & `cupy-9.6.0/tests/cupyx_tests/test_scatter.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/test_time.py` & `cupy-9.6.0/tests/cupyx_tests/test_time.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/cupyx_tests/tools_tests/test_install_library.py` & `cupy-9.6.0/tests/cupyx_tests/tools_tests/test_install_library.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/example_tests/test_finance.py` & `cupy-9.6.0/tests/example_tests/test_finance.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/example_tests/test_gmm.py` & `cupy-9.6.0/tests/example_tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/example_tests/test_kmeans.py` & `cupy-9.6.0/tests/example_tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `cupy-9.5.0/tests/install_tests/test_build.py` & `cupy-9.6.0/tests/install_tests/test_build.py`

 * *Files identical despite different names*

