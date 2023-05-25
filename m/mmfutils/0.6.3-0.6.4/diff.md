# Comparing `tmp/mmfutils-0.6.3.tar.gz` & `tmp/mmfutils-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmfutils-0.6.3.tar", max compression
+gzip compressed data, was "mmfutils-0.6.4.tar", max compression
```

## Comparing `mmfutils-0.6.3.tar` & `mmfutils-0.6.4.tar`

### file list

```diff
@@ -1,343 +1,41 @@
--rw-r--r--   0        0        0     1504 2022-02-01 20:15:10.881772 mmfutils-0.6.3/LICENSE.txt
--rw-r--r--   0        0        0      448 2022-02-03 17:07:03.091621 mmfutils-0.6.3/description.md
--rw-r--r--   0        0        0     4002 2022-06-08 08:16:14.618098 mmfutils-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1051 2022-02-03 17:07:03.112917 mmfutils-0.6.3/src/mmfutils/__init__.py
--rw-r--r--   0        0        0    16838 2022-02-03 17:07:03.114265 mmfutils-0.6.3/src/mmfutils/containers.py
--rw-r--r--   0        0        0    20903 2022-02-03 17:07:03.115250 mmfutils-0.6.3/src/mmfutils/contexts.py
--rw-r--r--   0        0        0     3616 2022-02-03 17:07:03.116065 mmfutils-0.6.3/src/mmfutils/debugging.py
--rw-r--r--   0        0        0     7062 2022-02-03 17:07:03.116923 mmfutils-0.6.3/src/mmfutils/interface.py
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.117636 mmfutils-0.6.3/src/mmfutils/math/__init__.py
--rw-r--r--   0        0        0      147 2022-02-01 21:44:26.450599 mmfutils-0.6.3/src/mmfutils/math/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      151 2022-06-04 17:51:11.307605 mmfutils-0.6.3/src/mmfutils/math/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      155 2022-06-04 17:56:52.109124 mmfutils-0.6.3/src/mmfutils/math/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      155 2022-06-04 18:12:42.462231 mmfutils-0.6.3/src/mmfutils/math/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    12856 2022-02-01 21:44:26.458444 mmfutils-0.6.3/src/mmfutils/math/__pycache__/bessel.cpython-36.pyc
--rw-r--r--   0        0        0    12818 2022-06-04 17:51:11.316474 mmfutils-0.6.3/src/mmfutils/math/__pycache__/bessel.cpython-37.pyc
--rw-r--r--   0        0        0    12791 2022-06-04 17:56:52.118386 mmfutils-0.6.3/src/mmfutils/math/__pycache__/bessel.cpython-38.pyc
--rw-r--r--   0        0        0    12771 2022-06-04 18:12:43.333295 mmfutils-0.6.3/src/mmfutils/math/__pycache__/bessel.cpython-39.pyc
--rw-r--r--   0        0        0     8141 2022-02-01 21:44:26.554190 mmfutils-0.6.3/src/mmfutils/math/__pycache__/differentiate.cpython-36.pyc
--rw-r--r--   0        0        0     8145 2022-06-04 17:51:11.456180 mmfutils-0.6.3/src/mmfutils/math/__pycache__/differentiate.cpython-37.pyc
--rw-r--r--   0        0        0     8136 2022-06-04 17:56:52.293573 mmfutils-0.6.3/src/mmfutils/math/__pycache__/differentiate.cpython-38.pyc
--rw-r--r--   0        0        0     8144 2022-06-04 18:14:03.547691 mmfutils-0.6.3/src/mmfutils/math/__pycache__/differentiate.cpython-39.pyc
--rw-r--r--   0        0        0      987 2022-02-01 21:44:27.107143 mmfutils-0.6.3/src/mmfutils/math/__pycache__/linalg.cpython-36.pyc
--rw-r--r--   0        0        0      991 2022-06-04 17:51:11.947937 mmfutils-0.6.3/src/mmfutils/math/__pycache__/linalg.cpython-37.pyc
--rw-r--r--   0        0        0     1001 2022-06-04 17:56:53.144954 mmfutils-0.6.3/src/mmfutils/math/__pycache__/linalg.cpython-38.pyc
--rw-r--r--   0        0        0      997 2022-06-04 18:14:04.017561 mmfutils-0.6.3/src/mmfutils/math/__pycache__/linalg.cpython-39.pyc
--rw-r--r--   0        0        0     2167 2022-02-01 21:44:27.109658 mmfutils-0.6.3/src/mmfutils/math/__pycache__/special.cpython-36.pyc
--rw-r--r--   0        0        0     2171 2022-06-04 17:51:11.950113 mmfutils-0.6.3/src/mmfutils/math/__pycache__/special.cpython-37.pyc
--rw-r--r--   0        0        0     2164 2022-06-04 17:56:53.147374 mmfutils-0.6.3/src/mmfutils/math/__pycache__/special.cpython-38.pyc
--rw-r--r--   0        0        0     2164 2022-06-04 18:14:04.019957 mmfutils-0.6.3/src/mmfutils/math/__pycache__/special.cpython-39.pyc
--rw-r--r--   0        0        0     1692 2022-02-01 21:44:27.111655 mmfutils-0.6.3/src/mmfutils/math/__pycache__/wigner.cpython-36.pyc
--rw-r--r--   0        0        0     1691 2022-06-04 17:51:11.952678 mmfutils-0.6.3/src/mmfutils/math/__pycache__/wigner.cpython-37.pyc
--rw-r--r--   0        0        0     1699 2022-06-04 17:56:53.149433 mmfutils-0.6.3/src/mmfutils/math/__pycache__/wigner.cpython-38.pyc
--rw-r--r--   0        0        0     1699 2022-06-04 18:14:04.022533 mmfutils-0.6.3/src/mmfutils/math/__pycache__/wigner.cpython-39.pyc
--rw-r--r--   0        0        0      242 2022-02-03 17:07:03.118475 mmfutils-0.6.3/src/mmfutils/math/bases/__init__.py
--rw-r--r--   0        0        0      352 2022-02-01 21:44:27.140173 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      356 2022-06-04 17:51:13.043486 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      362 2022-06-04 17:56:53.563859 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      321 2022-06-04 18:12:42.464149 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    34509 2022-02-01 21:44:27.146377 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/bases.cpython-36.pyc
--rw-r--r--   0        0        0    36431 2022-06-08 08:34:52.399438 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/bases.cpython-37.pyc
--rw-r--r--   0        0        0    36404 2022-06-08 08:37:31.888623 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/bases.cpython-38.pyc
--rw-r--r--   0        0        0    36297 2022-06-08 08:40:29.279655 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/bases.cpython-39.pyc
--rw-r--r--   0        0        0     7725 2022-02-01 21:44:27.147738 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/interfaces.cpython-36.pyc
--rw-r--r--   0        0        0     7747 2022-06-04 17:51:13.066458 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/interfaces.cpython-37.pyc
--rw-r--r--   0        0        0     7833 2022-06-04 17:56:53.599694 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/interfaces.cpython-38.pyc
--rw-r--r--   0        0        0     7836 2022-06-04 18:12:42.770384 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/interfaces.cpython-39.pyc
--rw-r--r--   0        0        0     4144 2022-02-01 21:44:27.150285 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0        0        0     4133 2022-06-08 08:34:52.419272 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0        0        0     4058 2022-06-08 08:37:31.913046 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     4173 2022-06-04 18:13:57.231347 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/utils.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4058 2022-06-08 08:40:29.309288 mmfutils-0.6.3/src/mmfutils/math/bases/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    51178 2022-06-07 18:51:15.375589 mmfutils-0.6.3/src/mmfutils/math/bases/bases.py
--rw-r--r--   0        0        0     5861 2022-02-03 17:07:03.120761 mmfutils-0.6.3/src/mmfutils/math/bases/interfaces.py
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.121565 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__init__.py
--rw-r--r--   0        0        0      159 2022-02-01 21:44:27.165989 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      163 2022-06-04 17:51:13.083979 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      167 2022-06-04 17:56:53.617377 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      167 2022-06-04 18:14:04.394182 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    40434 2022-02-01 21:44:27.214026 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    42057 2022-06-07 16:58:42.929662 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    42057 2022-06-08 08:34:52.629463 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    38325 2022-06-07 17:01:42.449743 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    38325 2022-06-08 08:37:32.166331 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    37709 2022-06-04 23:48:18.133005 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    37709 2022-06-08 08:40:29.512954 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    41751 2022-06-07 16:58:43.045600 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases_.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    38019 2022-06-07 17:01:42.566916 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases_.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    37393 2022-06-07 17:32:38.261199 mmfutils-0.6.3/src/mmfutils/math/bases/tests/__pycache__/test_bases_.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    22192 2022-06-07 18:51:15.376633 mmfutils-0.6.3/src/mmfutils/math/bases/tests/test_bases.py
--rw-r--r--   0        0        0     3607 2022-06-07 18:51:15.377387 mmfutils-0.6.3/src/mmfutils/math/bases/utils.py
--rw-r--r--   0        0        0    14266 2022-02-03 17:07:03.124697 mmfutils-0.6.3/src/mmfutils/math/bessel.py
--rw-r--r--   0        0        0     7476 2022-02-03 17:07:03.125561 mmfutils-0.6.3/src/mmfutils/math/differentiate.py
--rw-r--r--   0        0        0    20573 2022-02-03 17:07:03.126644 mmfutils-0.6.3/src/mmfutils/math/integrate/__init__.py
--rw-r--r--   0        0        0    18533 2022-02-01 21:44:26.557583 mmfutils-0.6.3/src/mmfutils/math/integrate/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0    18533 2022-06-04 17:51:11.460922 mmfutils-0.6.3/src/mmfutils/math/integrate/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    18574 2022-06-04 17:56:52.297724 mmfutils-0.6.3/src/mmfutils/math/integrate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    18496 2022-06-04 18:14:03.552159 mmfutils-0.6.3/src/mmfutils/math/integrate/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0   918653 2022-02-03 17:07:03.135117 mmfutils-0.6.3/src/mmfutils/math/integrate/_ssum_cython.c
--rw-r--r--   0        0        0      918 2022-02-03 17:07:03.142062 mmfutils-0.6.3/src/mmfutils/math/integrate/_ssum_cython.pyx
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.143215 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__init__.py
--rw-r--r--   0        0        0      163 2022-02-01 21:44:27.246440 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      167 2022-06-04 17:51:13.188496 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      171 2022-06-04 17:56:53.722497 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      171 2022-06-04 18:14:04.579749 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9561 2022-02-01 21:44:27.260625 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     9440 2022-06-04 17:51:13.201725 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     9440 2022-06-08 08:34:52.688330 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     9509 2022-06-04 17:56:53.736783 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     9509 2022-06-08 08:37:32.221713 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     9348 2022-06-04 18:14:04.597050 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     9348 2022-06-08 08:40:29.572963 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/__pycache__/test_integrate.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3810 2022-02-03 17:07:03.144749 mmfutils-0.6.3/src/mmfutils/math/integrate/tests/test_integrate.py
--rw-r--r--   0        0        0      657 2022-02-03 17:07:03.145963 mmfutils-0.6.3/src/mmfutils/math/linalg.py
--rw-r--r--   0        0        0     1916 2022-02-03 17:07:03.147400 mmfutils-0.6.3/src/mmfutils/math/special.py
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.149087 mmfutils-0.6.3/src/mmfutils/math/tests/__init__.py
--rw-r--r--   0        0        0      153 2022-02-01 21:44:27.269338 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      157 2022-06-04 17:51:13.211689 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      161 2022-06-04 17:56:53.747130 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      161 2022-06-04 18:14:04.650914 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3680 2022-02-01 21:44:27.276399 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3660 2022-06-04 17:51:13.219160 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3660 2022-06-08 08:34:52.707631 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3658 2022-06-04 17:56:53.755561 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3658 2022-06-08 08:37:32.238470 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3608 2022-06-04 18:14:04.659725 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3608 2022-06-08 08:40:29.601317 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_bessel.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3081 2022-02-01 21:44:27.285091 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3054 2022-06-04 17:51:13.228662 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3054 2022-06-08 08:34:52.718548 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2870 2022-06-04 17:56:53.766357 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2870 2022-06-08 08:37:32.249206 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2818 2022-06-04 18:14:04.670939 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2818 2022-06-08 08:40:29.616224 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_differentiate.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3479 2022-02-01 21:44:27.294790 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3399 2022-06-04 17:51:13.238022 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3399 2022-06-08 08:34:52.730497 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3337 2022-06-04 17:56:53.776535 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3337 2022-06-08 08:37:32.262149 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3265 2022-06-04 18:14:04.682087 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3265 2022-06-08 08:40:29.631639 mmfutils-0.6.3/src/mmfutils/math/tests/__pycache__/test_special.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     1263 2022-02-03 17:07:03.150564 mmfutils-0.6.3/src/mmfutils/math/tests/test_bessel.py
--rw-r--r--   0        0        0     1091 2022-02-03 17:07:03.152176 mmfutils-0.6.3/src/mmfutils/math/tests/test_differentiate.py
--rw-r--r--   0        0        0      662 2022-02-03 17:07:03.153780 mmfutils-0.6.3/src/mmfutils/math/tests/test_special.py
--rw-r--r--   0        0        0     1624 2022-02-03 17:07:03.154865 mmfutils-0.6.3/src/mmfutils/math/wigner.py
--rw-r--r--   0        0        0     2159 2022-02-03 17:07:03.155797 mmfutils-0.6.3/src/mmfutils/optimize.py
--rw-r--r--   0        0        0     8944 2022-02-03 17:07:03.157131 mmfutils-0.6.3/src/mmfutils/parallel.py
--rw-r--r--   0        0        0      177 2022-02-03 17:07:03.158220 mmfutils-0.6.3/src/mmfutils/performance/__init__.py
--rw-r--r--   0        0        0      336 2022-02-01 21:44:27.112397 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      340 2022-06-04 17:51:11.953534 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      344 2022-06-04 17:56:53.150268 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      344 2022-06-04 18:12:42.787060 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4437 2022-02-01 21:44:27.300608 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/blas.cpython-36.pyc
--rw-r--r--   0        0        0     4441 2022-06-04 17:51:13.244251 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/blas.cpython-37.pyc
--rw-r--r--   0        0        0     3941 2022-06-04 17:56:53.783213 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/blas.cpython-38.pyc
--rw-r--r--   0        0        0     3915 2022-06-04 18:14:04.689224 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/blas.cpython-39.pyc
--rw-r--r--   0        0        0     6887 2022-02-01 21:44:27.114281 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/fft.cpython-36.pyc
--rw-r--r--   0        0        0     7795 2022-06-04 17:51:11.955641 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/fft.cpython-37.pyc
--rw-r--r--   0        0        0     7628 2022-06-04 17:56:53.152349 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/fft.cpython-38.pyc
--rw-r--r--   0        0        0     7641 2022-06-04 18:12:42.789592 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/fft.cpython-39.pyc
--rw-r--r--   0        0        0      845 2022-02-01 21:44:27.305030 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/numexpr.cpython-36.pyc
--rw-r--r--   0        0        0      849 2022-06-04 17:51:13.248612 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/numexpr.cpython-37.pyc
--rw-r--r--   0        0        0      857 2022-06-04 17:56:53.788364 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/numexpr.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-06-04 18:14:04.694924 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/numexpr.cpython-39.pyc
--rw-r--r--   0        0        0     1031 2022-02-01 21:44:27.114996 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/threads.cpython-36.pyc
--rw-r--r--   0        0        0     1035 2022-06-04 17:51:11.956518 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/threads.cpython-37.pyc
--rw-r--r--   0        0        0     1039 2022-06-04 17:56:53.153342 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/threads.cpython-38.pyc
--rw-r--r--   0        0        0     1035 2022-06-04 18:12:42.790881 mmfutils-0.6.3/src/mmfutils/performance/__pycache__/threads.cpython-39.pyc
--rw-r--r--   0        0        0     4282 2022-02-03 17:07:03.159288 mmfutils-0.6.3/src/mmfutils/performance/blas.py
--rw-r--r--   0        0        0     9777 2022-05-24 05:11:13.448353 mmfutils-0.6.3/src/mmfutils/performance/fft.py
--rw-r--r--   0        0        0      976 2022-02-03 17:07:03.161453 mmfutils-0.6.3/src/mmfutils/performance/numexpr.py
--rw-r--r--   0        0        0     1053 2022-02-03 17:07:03.162429 mmfutils-0.6.3/src/mmfutils/performance/threads.py
--rw-r--r--   0        0        0      421 2022-02-03 17:07:03.163438 mmfutils-0.6.3/src/mmfutils/plot/__init__.py
--rw-r--r--   0        0        0      573 2022-02-01 21:44:27.546819 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      577 2022-06-04 17:51:13.538980 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      583 2022-06-04 17:56:54.631167 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      553 2022-06-04 18:14:05.513244 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5081 2022-02-01 21:44:27.548492 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/animation.cpython-36.pyc
--rw-r--r--   0        0        0     5080 2022-06-04 17:51:13.540917 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/animation.cpython-37.pyc
--rw-r--r--   0        0        0     5099 2022-06-04 17:56:54.633674 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/animation.cpython-38.pyc
--rw-r--r--   0        0        0     5165 2022-06-04 18:14:05.515944 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/animation.cpython-39.pyc
--rw-r--r--   0        0        0    43939 2022-02-01 21:44:28.056618 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/cmaps.cpython-36.pyc
--rw-r--r--   0        0        0    43943 2022-06-04 17:51:13.995330 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/cmaps.cpython-37.pyc
--rw-r--r--   0        0        0    43983 2022-06-04 17:56:55.086997 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/cmaps.cpython-38.pyc
--rw-r--r--   0        0        0    39914 2022-06-04 18:14:05.913092 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/cmaps.cpython-39.pyc
--rw-r--r--   0        0        0     5908 2022-02-01 21:44:28.004462 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/colors.cpython-36.pyc
--rw-r--r--   0        0        0     5900 2022-06-04 17:51:13.986672 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/colors.cpython-37.pyc
--rw-r--r--   0        0        0     5935 2022-06-04 17:56:55.076257 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/colors.cpython-38.pyc
--rw-r--r--   0        0        0     6005 2022-06-04 18:14:05.901576 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0        0        0     4735 2022-02-01 21:44:28.065156 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/contour.cpython-36.pyc
--rw-r--r--   0        0        0     4719 2022-06-04 17:51:14.004925 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/contour.cpython-37.pyc
--rw-r--r--   0        0        0     4763 2022-06-04 17:56:55.097090 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/contour.cpython-38.pyc
--rw-r--r--   0        0        0     4754 2022-06-04 18:14:05.924868 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/contour.cpython-39.pyc
--rw-r--r--   0        0        0     2944 2022-02-01 21:44:28.078583 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/errors.cpython-36.pyc
--rw-r--r--   0        0        0     2948 2022-06-04 17:51:14.024957 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/errors.cpython-37.pyc
--rw-r--r--   0        0        0     2959 2022-06-04 17:56:55.129804 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/errors.cpython-38.pyc
--rw-r--r--   0        0        0     2990 2022-06-04 18:14:05.947535 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0    20293 2022-02-01 21:44:28.425581 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/publish.cpython-36.pyc
--rw-r--r--   0        0        0    20166 2022-06-04 17:51:14.217971 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/publish.cpython-37.pyc
--rw-r--r--   0        0        0    20214 2022-06-04 17:56:55.376999 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/publish.cpython-38.pyc
--rw-r--r--   0        0        0    20228 2022-06-04 18:14:06.244745 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/publish.cpython-39.pyc
--rw-r--r--   0        0        0     2143 2022-02-01 21:44:28.076969 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/rasterize.cpython-36.pyc
--rw-r--r--   0        0        0     2147 2022-06-04 17:51:14.023168 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/rasterize.cpython-37.pyc
--rw-r--r--   0        0        0     2173 2022-06-04 17:56:55.127856 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/rasterize.cpython-38.pyc
--rw-r--r--   0        0        0     2181 2022-06-04 18:14:05.945176 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/rasterize.cpython-39.pyc
--rw-r--r--   0        0        0      176 2022-06-04 17:51:14.224924 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/sparkline.cpython-37.pyc
--rw-r--r--   0        0        0      180 2022-06-04 17:56:55.384544 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/sparkline.cpython-38.pyc
--rw-r--r--   0        0        0      180 2022-06-04 18:14:06.252116 mmfutils-0.6.3/src/mmfutils/plot/__pycache__/sparkline.cpython-39.pyc
--rw-r--r--   0        0        0     7213 2022-02-03 17:07:03.164387 mmfutils-0.6.3/src/mmfutils/plot/animation.py
--rw-r--r--   0        0        0    37324 2022-02-03 17:07:03.166125 mmfutils-0.6.3/src/mmfutils/plot/cmaps.py
--rw-r--r--   0        0        0     6857 2022-02-03 17:07:03.167246 mmfutils-0.6.3/src/mmfutils/plot/colors.py
--rw-r--r--   0        0        0     4921 2022-02-03 17:07:03.168109 mmfutils-0.6.3/src/mmfutils/plot/contour.py
--rw-r--r--   0        0        0     4431 2022-02-03 17:07:03.169279 mmfutils-0.6.3/src/mmfutils/plot/errors.py
--rw-r--r--   0        0        0    26375 2022-02-03 17:07:03.171081 mmfutils-0.6.3/src/mmfutils/plot/publish.py
--rw-r--r--   0        0        0     1706 2022-02-03 17:07:03.172258 mmfutils-0.6.3/src/mmfutils/plot/rasterize.py
--rw-r--r--   0        0        0       19 2022-02-03 18:03:02.104323 mmfutils-0.6.3/src/mmfutils/plot/sparkline.py
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.173298 mmfutils-0.6.3/src/mmfutils/solve/__init__.py
--rw-r--r--   0        0        0      148 2022-02-01 21:44:28.579925 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      152 2022-06-04 17:51:14.226423 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      156 2022-06-04 17:56:55.386029 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      156 2022-06-04 18:14:06.253841 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    25770 2022-02-01 21:44:28.587387 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/broyden.cpython-36.pyc
--rw-r--r--   0        0        0    25717 2022-06-04 17:51:14.232746 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/broyden.cpython-37.pyc
--rw-r--r--   0        0        0    25751 2022-06-04 17:56:55.392836 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/broyden.cpython-38.pyc
--rw-r--r--   0        0        0    25726 2022-06-04 18:14:06.261531 mmfutils-0.6.3/src/mmfutils/solve/__pycache__/broyden.cpython-39.pyc
--rw-r--r--   0        0        0    28027 2022-02-03 17:33:07.363395 mmfutils-0.6.3/src/mmfutils/solve/broyden.py
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.176298 mmfutils-0.6.3/src/mmfutils/solve/tests/__init__.py
--rw-r--r--   0        0        0      154 2022-02-01 21:44:28.595229 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      158 2022-06-04 17:51:14.241221 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      162 2022-06-04 17:56:55.401280 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      162 2022-06-04 18:14:06.271031 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    17057 2022-02-01 21:44:28.622704 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16771 2022-06-04 17:51:14.333113 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16771 2022-06-08 08:34:53.660566 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    16334 2022-06-04 17:56:55.426458 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16334 2022-06-08 08:37:34.202900 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    16060 2022-06-04 18:14:06.301920 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16060 2022-06-08 08:40:32.044824 mmfutils-0.6.3/src/mmfutils/solve/tests/__pycache__/test_broyden.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     5781 2022-02-03 17:07:03.177518 mmfutils-0.6.3/src/mmfutils/solve/tests/test_broyden.py
--rw-r--r--   0        0        0     1302 2022-02-03 17:07:03.178351 mmfutils-0.6.3/src/mmfutils/testing.py
--rw-r--r--   0        0        0        0 2022-02-03 17:07:03.179275 mmfutils-0.6.3/src/mmfutils/tests/__init__.py
--rw-r--r--   0        0        0      148 2022-02-01 21:44:28.639141 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      152 2022-06-04 17:51:14.352118 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      156 2022-06-04 17:56:55.442174 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      156 2022-06-04 18:14:06.335742 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      979 2022-02-01 21:44:28.647492 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/parallel_module.cpython-36.pyc
--rw-r--r--   0        0        0      983 2022-06-04 17:51:14.360932 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/parallel_module.cpython-37.pyc
--rw-r--r--   0        0        0      991 2022-06-04 17:56:55.449977 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/parallel_module.cpython-38.pyc
--rw-r--r--   0        0        0      991 2022-06-04 18:14:06.345326 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/parallel_module.cpython-39.pyc
--rw-r--r--   0        0        0     2116 2022-02-01 21:44:28.650930 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2126 2022-06-04 17:51:14.365728 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2126 2022-06-08 08:34:53.686861 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2144 2022-06-04 17:56:55.453562 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2144 2022-06-08 08:37:34.228126 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2203 2022-06-04 18:14:06.349452 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2203 2022-06-08 08:40:32.072421 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_animation.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    16634 2022-02-01 21:44:28.681579 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16142 2022-06-04 17:51:14.393343 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16142 2022-06-08 08:34:53.722381 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    15028 2022-06-04 17:56:55.481986 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    15028 2022-06-08 08:37:34.267018 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    14605 2022-06-04 18:14:06.382297 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    14605 2022-06-08 08:40:32.141737 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_containers.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    13518 2022-02-01 21:44:28.730405 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    12952 2022-06-04 17:51:14.429482 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    12952 2022-06-08 08:34:53.829237 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    12669 2022-06-04 17:56:55.520510 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    12669 2022-06-08 08:37:34.308875 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    12941 2022-06-04 18:14:06.446783 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    12941 2022-06-08 08:40:32.253570 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_context.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2676 2022-02-01 21:44:28.744491 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2629 2022-06-04 17:51:14.440323 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2629 2022-06-08 08:34:53.839495 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2552 2022-06-04 17:56:55.532598 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2552 2022-06-08 08:37:34.318998 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2526 2022-06-04 18:14:06.460686 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2526 2022-06-08 08:40:32.266534 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_debugging.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     1718 2022-02-01 21:44:28.750392 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1721 2022-06-04 17:51:14.446370 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1721 2022-06-08 08:34:53.845384 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     1731 2022-06-04 17:56:55.538174 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1731 2022-06-08 08:37:34.326436 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     1713 2022-06-04 18:14:06.467334 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1713 2022-06-08 08:40:32.274104 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_differentiate.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3842 2022-02-01 21:44:28.754937 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3854 2022-06-04 17:51:14.450791 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3854 2022-06-08 08:34:53.849157 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3902 2022-06-04 17:56:55.542397 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3902 2022-06-08 08:37:34.330874 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3958 2022-06-04 18:14:06.472871 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3958 2022-06-08 08:40:32.279846 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_interface.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3304 2022-02-01 21:44:28.766244 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3205 2022-06-04 17:51:14.462071 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3205 2022-06-08 08:34:53.860628 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2957 2022-06-04 17:56:55.554193 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2957 2022-06-08 08:37:34.343490 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2886 2022-06-04 18:14:06.487446 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2886 2022-06-08 08:40:32.296236 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_mmfutils.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2307 2022-02-01 21:44:28.773144 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2300 2022-06-04 17:51:14.468948 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2300 2022-06-08 08:34:53.867356 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2276 2022-06-04 17:56:55.561064 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2276 2022-06-08 08:37:34.350241 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     2248 2022-06-04 18:14:06.495707 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2248 2022-06-08 08:40:32.304933 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_optimize.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     7652 2022-02-01 21:44:28.787604 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     7481 2022-06-04 17:51:14.481198 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     7481 2022-06-08 08:34:53.882373 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     7471 2022-06-04 17:56:55.575568 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     7471 2022-06-08 08:37:34.367315 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     7375 2022-06-04 18:14:06.511433 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     7375 2022-06-08 08:40:32.327141 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_parallel.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    15239 2022-02-01 21:44:28.815000 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    14942 2022-06-04 17:51:14.508317 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    14942 2022-06-08 08:34:53.915851 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    13582 2022-06-04 17:56:55.604802 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    13582 2022-06-08 08:37:34.406172 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    13310 2022-06-04 18:14:06.548995 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    13310 2022-06-08 08:40:32.375151 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_blas.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    13917 2022-02-01 21:44:28.845932 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    13869 2022-06-04 17:51:14.538372 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    13869 2022-06-08 08:34:53.952271 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    13300 2022-06-04 17:56:55.638603 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    13300 2022-06-08 08:37:34.450136 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0    13138 2022-06-04 18:14:06.593653 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    13138 2022-06-08 08:40:32.425982 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_fft.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     6900 2022-02-01 21:44:28.862814 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     6684 2022-06-04 17:51:14.554710 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     6684 2022-06-08 08:34:53.970061 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     6167 2022-06-04 17:56:55.655916 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     6167 2022-06-08 08:37:34.469345 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     6025 2022-06-04 18:14:06.618418 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     6025 2022-06-08 08:40:32.447972 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_performance_threads.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3919 2022-02-01 21:44:28.875216 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3893 2022-06-04 17:51:14.567219 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3893 2022-06-08 08:34:53.981651 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3921 2022-06-04 17:56:55.668488 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3921 2022-06-08 08:37:34.486079 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     3920 2022-06-04 18:14:06.634912 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3920 2022-06-08 08:40:32.462139 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_plot.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     5460 2022-02-01 21:44:28.893139 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5384 2022-06-04 17:51:14.584741 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-37-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5384 2022-06-08 08:34:54.002659 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     5282 2022-06-04 17:56:55.686815 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5282 2022-06-08 08:37:34.509391 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0        0        0     5128 2022-06-04 18:14:06.659280 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5128 2022-06-08 08:40:32.490333 mmfutils-0.6.3/src/mmfutils/tests/__pycache__/test_testing.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      755 2022-02-03 17:07:03.180466 mmfutils-0.6.3/src/mmfutils/tests/parallel_module.py
--rw-r--r--   0        0        0     1652 2022-02-03 17:07:03.181628 mmfutils-0.6.3/src/mmfutils/tests/test_animation.py
--rw-r--r--   0        0        0     6377 2022-02-03 17:07:03.183652 mmfutils-0.6.3/src/mmfutils/tests/test_containers.py
--rw-r--r--   0        0        0     9884 2022-02-03 17:07:03.185057 mmfutils-0.6.3/src/mmfutils/tests/test_context.py
--rw-r--r--   0        0        0      756 2022-02-03 17:07:03.186049 mmfutils-0.6.3/src/mmfutils/tests/test_debugging.py
--rw-r--r--   0        0        0      441 2022-02-03 17:07:03.187250 mmfutils-0.6.3/src/mmfutils/tests/test_differentiate.py
--rw-r--r--   0        0        0     2824 2022-02-03 17:07:03.188797 mmfutils-0.6.3/src/mmfutils/tests/test_interface.py
--rw-r--r--   0        0        0     1123 2022-02-03 17:07:03.190373 mmfutils-0.6.3/src/mmfutils/tests/test_mmfutils.py
--rw-r--r--   0        0        0      791 2022-02-03 17:07:03.191962 mmfutils-0.6.3/src/mmfutils/tests/test_optimize.py
--rw-r--r--   0        0        0     3065 2022-02-03 17:07:03.193349 mmfutils-0.6.3/src/mmfutils/tests/test_parallel.py
--rw-r--r--   0        0        0     4399 2022-02-03 17:07:03.194594 mmfutils-0.6.3/src/mmfutils/tests/test_performance_blas.py
--rw-r--r--   0        0        0     3572 2022-02-03 17:07:03.195723 mmfutils-0.6.3/src/mmfutils/tests/test_performance_fft.py
--rw-r--r--   0        0        0     2039 2022-02-03 17:07:03.196817 mmfutils-0.6.3/src/mmfutils/tests/test_performance_threads.py
--rw-r--r--   0        0        0     1324 2022-02-03 17:07:03.197889 mmfutils-0.6.3/src/mmfutils/tests/test_plot.py
--rw-r--r--   0        0        0     1574 2022-02-03 17:07:03.199233 mmfutils-0.6.3/src/mmfutils/tests/test_testing.py
--rw-r--r--   0        0        0     2763 2022-06-08 08:46:04.156695 mmfutils-0.6.3/setup.py
--rw-r--r--   0        0        0     3157 2022-06-08 08:46:04.157094 mmfutils-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-03-14 02:37:07.428202 mmfutils-0.6.4/LICENSE.txt
+-rw-r--r--   0        0        0      448 2023-03-14 02:37:07.430312 mmfutils-0.6.4/description.md
+-rw-r--r--   0        0        0     5146 2023-05-25 09:52:09.462298 mmfutils-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1071 2023-03-23 10:20:06.591896 mmfutils-0.6.4/src/mmfutils/__init__.py
+-rw-r--r--   0        0        0    16856 2023-03-23 10:20:06.592165 mmfutils-0.6.4/src/mmfutils/containers.py
+-rw-r--r--   0        0        0    25514 2023-03-23 10:20:06.592490 mmfutils-0.6.4/src/mmfutils/contexts.py
+-rw-r--r--   0        0        0     3616 2023-03-14 02:37:07.443437 mmfutils-0.6.4/src/mmfutils/debugging.py
+-rw-r--r--   0        0        0     7062 2023-03-14 02:37:07.443639 mmfutils-0.6.4/src/mmfutils/interface.py
+-rw-r--r--   0        0        0        0 2023-03-14 02:37:07.443792 mmfutils-0.6.4/src/mmfutils/math/__init__.py
+-rw-r--r--   0        0        0      242 2023-03-14 02:37:07.444002 mmfutils-0.6.4/src/mmfutils/math/bases/__init__.py
+-rw-r--r--   0        0        0    51198 2023-03-23 10:20:06.592908 mmfutils-0.6.4/src/mmfutils/math/bases/bases.py
+-rw-r--r--   0        0        0     5861 2023-03-14 02:37:07.444568 mmfutils-0.6.4/src/mmfutils/math/bases/interfaces.py
+-rw-r--r--   0        0        0     3646 2023-05-25 09:45:38.840475 mmfutils-0.6.4/src/mmfutils/math/bases/utils.py
+-rw-r--r--   0        0        0    14266 2023-03-14 02:37:07.445487 mmfutils-0.6.4/src/mmfutils/math/bessel.py
+-rw-r--r--   0        0        0     7476 2023-03-14 02:37:07.445736 mmfutils-0.6.4/src/mmfutils/math/differentiate.py
+-rw-r--r--   0        0        0    20573 2023-03-14 02:37:07.446021 mmfutils-0.6.4/src/mmfutils/math/integrate/__init__.py
+-rw-r--r--   0        0        0   918653 2023-03-14 02:37:07.449156 mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.c
+-rw-r--r--   0        0        0      918 2023-03-14 02:37:07.449431 mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.pyx
+-rw-r--r--   0        0        0      657 2023-03-14 02:37:07.450074 mmfutils-0.6.4/src/mmfutils/math/linalg.py
+-rw-r--r--   0        0        0     1916 2023-03-14 02:37:07.450271 mmfutils-0.6.4/src/mmfutils/math/special.py
+-rw-r--r--   0        0        0     1624 2023-03-14 02:37:07.451256 mmfutils-0.6.4/src/mmfutils/math/wigner.py
+-rw-r--r--   0        0        0     2159 2023-03-14 02:37:07.451445 mmfutils-0.6.4/src/mmfutils/optimize.py
+-rw-r--r--   0        0        0     8944 2023-03-14 02:37:07.451659 mmfutils-0.6.4/src/mmfutils/parallel.py
+-rw-r--r--   0        0        0      177 2023-03-14 02:37:07.451870 mmfutils-0.6.4/src/mmfutils/performance/__init__.py
+-rw-r--r--   0        0        0     4282 2023-03-14 02:37:07.452102 mmfutils-0.6.4/src/mmfutils/performance/blas.py
+-rw-r--r--   0        0        0     9777 2023-03-14 02:37:07.452369 mmfutils-0.6.4/src/mmfutils/performance/fft.py
+-rw-r--r--   0        0        0      976 2023-03-14 02:37:07.452583 mmfutils-0.6.4/src/mmfutils/performance/numexpr.py
+-rw-r--r--   0        0        0     1053 2023-03-14 02:37:07.452796 mmfutils-0.6.4/src/mmfutils/performance/threads.py
+-rw-r--r--   0        0        0      421 2023-03-14 02:37:07.453039 mmfutils-0.6.4/src/mmfutils/plot/__init__.py
+-rw-r--r--   0        0        0     6957 2023-05-25 09:45:38.840755 mmfutils-0.6.4/src/mmfutils/plot/animation.py
+-rw-r--r--   0        0        0    37324 2023-03-14 02:37:07.453620 mmfutils-0.6.4/src/mmfutils/plot/cmaps.py
+-rw-r--r--   0        0        0     6925 2023-03-23 10:20:06.593151 mmfutils-0.6.4/src/mmfutils/plot/colors.py
+-rw-r--r--   0        0        0     4921 2023-03-14 02:37:07.454080 mmfutils-0.6.4/src/mmfutils/plot/contour.py
+-rw-r--r--   0        0        0     4431 2023-03-14 02:37:07.454298 mmfutils-0.6.4/src/mmfutils/plot/errors.py
+-rw-r--r--   0        0        0     2474 2023-03-27 18:52:24.066912 mmfutils-0.6.4/src/mmfutils/plot/histogram.py
+-rw-r--r--   0        0        0    26375 2023-03-14 02:37:07.454584 mmfutils-0.6.4/src/mmfutils/plot/publish.py
+-rw-r--r--   0        0        0     1706 2023-03-14 02:37:07.454796 mmfutils-0.6.4/src/mmfutils/plot/rasterize.py
+-rw-r--r--   0        0        0        0 2023-03-14 02:37:07.455018 mmfutils-0.6.4/src/mmfutils/solve/__init__.py
+-rw-r--r--   0        0        0    28204 2023-03-23 10:20:06.593467 mmfutils-0.6.4/src/mmfutils/solve/broyden.py
+-rw-r--r--   0        0        0     1302 2023-03-14 02:37:07.456161 mmfutils-0.6.4/src/mmfutils/testing.py
+-rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 mmfutils-0.6.4/PKG-INFO
```

### Comparing `mmfutils-0.6.3/LICENSE.txt` & `mmfutils-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/__init__.py` & `mmfutils-0.6.4/src/mmfutils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     import importlib.metadata as _metadata
 except ImportError:
     import importlib_metadata as _metadata
 
 try:
     __version__ = _metadata.version(__name__)
-except _metadata.PackageNotFoundError:
+except _metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = "<unknown source distribution>"
 
 
 def unique_list(lst, preserve_order=True):
     """Make list contain only unique elements but preserve order.
 
     >>> lst = [1,2,4,3,2,3,1,0]
```

### Comparing `mmfutils-0.6.3/src/mmfutils/containers.py` & `mmfutils-0.6.4/src/mmfutils/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     ######################################################################
     # More comprehensive checks
     def _check_picklable(self, key, value):
         """Raise ValueError if obj is not picklable."""
         try:
             pickle.dumps(value)
-        except pickle.PicklingError:
+        except (AttributeError, pickle.PicklingError):
             raise ValueError(f"Attribute {key}={value} not picklable.")
 
     def _check_attribute(self, key, value=None):
         """Expended version that looks at exclusion lists and checks
         if value is picklable.  Raises AttributeError if _strict and
         attribute is not picklable.
         """
```

### Comparing `mmfutils-0.6.3/src/mmfutils/contexts.py` & `mmfutils-0.6.4/src/mmfutils/contexts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 """Various useful contexts.
 """
+import collections
+from contextlib import contextmanager
 import functools
+import math
 import os
 import signal
 import time
 
 import threading
 
 import warnings
 
+try:
+    # Try importing this here to prevent delays in contexts.
+    import IPython
+except ImportError:  # pragma: no cover
+    IPython = None
+
+__all__ = [
+    "is_main_thread",
+    "NoInterrupt",
+    "FPS",
+    "CoroutineWrapper",
+    "nointerrupt",
+    "coroutine",
+]
+
 
 def is_main_thread():
     """Return True if this is the main thread."""
     return threading.current_thread() is threading.main_thread()
 
 
-class NoInterrupt(object):
+class NoInterrupt:
     """Suspend the various signals during the execution block and a
     simple mechanism to allow threads to be interrupted.
 
     Arguments
     ---------
     ignore : bool
        If True, then do not raise a KeyboardInterrupt if a soft interrupt is
        caught unless forced by multiple interrupt requests in a
        limited time.
 
-
     There are two main entry points: globally by calling the :meth:`suspend()`
     method, and within a :class:`NoInterrupt()` context.
 
     **Main Thread**
 
     When executed in a context from the main thread, a signal handler
     is established which captures interrupt signals and represents
@@ -206,15 +223,14 @@
 
     Again: the exception can be ignored
     >>> n = [0, 0]
     >>> with NoInterrupt() as interrupted:
     ...     f(n, interrupted)
     >>> n
     [5, 5]
-
     """
 
     # Each time a signal is raised, it is inserted into the
     # _signals_raised dict and the corresponding entry of
     # _signal_count is incremented.  At the end of the final context
     # of the main thread (outermost context) the dict of
     # _signals_raised is cleared, but _signal_count is NOT reset.  The
@@ -235,18 +251,21 @@
     force_n = 3
     force_timeout = 1
 
     # Lock should be re-entrant (I think) since a signal might be sent during
     # operation of one of the functions.
     _lock = threading.RLock()
 
-    def __init__(self, ignore=True):
+    def __init__(self, ignore=True, timeout=None, unregister=False):
+        if unregister:
+            self.unregister()
         with self._lock:
             self.ignore = ignore
             self._active = True
+            self.timeout = timeout
             self.signal_count_at_start = dict(self._signal_count)
 
     @classmethod
     def is_registered(cls):
         """Return True if handlers are registered."""
         with cls._lock:
             registered = bool(cls._signals.intersection(cls._original_handlers))
@@ -389,15 +408,14 @@
             else:
                 os.kill(os.getpid(), signum)
 
     @classmethod
     def _forced_interrupt(cls, signum):
         """Return True if :attr:`force_n` interrupts have been recieved in the past
         :attr:`force_timeout` seconds
-
         """
         with cls._lock:
             signals_raised = cls._signals_raised.get(signum, [])
             return cls.force_n <= len(signals_raised) and cls.force_timeout > (
                 signals_raised[-1][-1] - signals_raised[-cls.force_n][-1]
             )
 
@@ -412,22 +430,19 @@
     @staticmethod
     def _post_handler_hook():
         pass
 
     def __enter__(self):
         """Enter context."""
         with self._lock:
-            try:
-                import IPython
-
+            self.tic = time.time()
+            if IPython and IPython.get_ipython():
                 kernel = IPython.get_ipython().kernel
                 kernel.pre_handler_hook = self._pre_handler_hook
                 kernel.post_handler_hook = self._post_handler_hook
-            except (ImportError, AttributeError):
-                pass
 
             self._active = True
             self.signal_count_at_start = dict(self._signal_count)
             if is_main_thread():
                 if not self.is_registered():
                     self.register()
                 self.suspend()
@@ -459,32 +474,33 @@
                 self.resume()
                 last_signal = self.reset()
 
                 if last_signal and not self.ignore:
                     # Call original handler.
                     signum, frame, _time = last_signal
                     self.handle_original_signal(signum=signum, frame=frame)
-            try:
-                import IPython
-
+            if IPython and IPython.get_ipython():
                 kernel = IPython.get_ipython().kernel
                 del kernel.pre_handler_hook
                 del kernel.post_handler_hook
-            except (ImportError, AttributeError):
-                pass
 
     def __bool__(self):
         """Return True if interrupted."""
         with self._lock:
-            return not self._active or any(
-                [
-                    self._signal_count.get(_signum, 0)
-                    > self.signal_count_at_start.get(_signum, 0)
-                    for _signum in self._signals
-                ]
+            timeout = self.timeout and time.time() - self.tic > self.timeout
+            return (
+                not self._active
+                or timeout
+                or any(
+                    [
+                        self._signal_count.get(_signum, 0)
+                        > self.signal_count_at_start.get(_signum, 0)
+                        for _signum in self._signals
+                    ]
+                )
             )
 
     __nonzero__ = __bool__  # For python 2.
 
     def map(self, function, sequence, *v, **kw):
         """Map function onto sequence until interrupted or done.
 
@@ -535,15 +551,14 @@
 
 
 class CoroutineWrapper(object):
     """Wrapper for coroutine contexts that allows them to function as a context but also as
     a function.  Similar to :func:`open()` which may be used both in a function or as a
     file object.  Note: be sure to call :meth:`close()` if you do not use this as a
     context.
-
     """
 
     def __init__(self, coroutine):
         self.coroutine = coroutine
         self.started = False
 
     def __enter__(self, *v, **kw):
@@ -565,15 +580,15 @@
         return self.send(*v)
 
     def close(self):
         self.coroutine.close()
 
 
 def coroutine(coroutine):
-    """Decorator for a context that yeilds an function from a coroutine.
+    """Decorator for a context that yeilds a function from a coroutine.
 
     This allows you to write functions that maintain state between calls.  The
     use as a context here ensures that the coroutine is closed.
 
     Examples
     --------
     Here is an example based on that suggested by Thomas Kluyver:
@@ -631,7 +646,145 @@
         return CoroutineWrapper(coroutine(*v, **kw))
         # primed_coroutine = coroutine(*v, **kw)
         # next(primed_coroutine)
         # yield primed_coroutine.send
         # primed_coroutine.close()
 
     return wrapper
+
+
+class FPS:
+    """Context manager to measure framerate and provide interrupt control.
+
+    This can be used in two ways:
+    1. As an iterator, which will run for the specified number of frames or until the
+       timeout is exceeded;
+    2. As flag that can be run while `bool(fps)`.  In this second usage, you must
+       manually update `fps.frame` to get a proper fps computation.
+
+    The `fps` instance can be used as to display the current frame-rate.
+
+    Arguments
+    ---------
+    frames : int | iterable
+        Yields iterator or range.
+    timeout : float
+        Timeout in seconds.
+    tics : int
+        How many of the last updates will be used to calculate the fps.
+    unregister : bool
+        If `True`, then call NoInterrupt.unregister() before the loop.
+
+    Examples
+    --------
+    >>> from time import sleep
+    >>> import numpy as np
+    >>> with FPS(frames=0.1*np.arange(10), timeout=10) as fps:
+    ...     for t in fps:
+    ...         print(f"t={t:.1f}: fps={fps:}")
+    ...         sleep(0.1)
+    ...     print(1/np.diff(fps.tics))
+    t=0.0: fps=nan
+    t=0.1: fps=9...
+    t=0.2: fps=9...
+    t=0.3: fps=9...
+    t=0.4: fps=9...
+    t=0.5: fps=9...
+    t=0.6: fps=9...
+    t=0.7: fps=9...
+    t=0.8: fps=9...
+    t=0.9: fps=9...
+
+    If you don't need to report the actual performance, you can just use the FPS class
+    as an iterator.  This will break only at the start of the loop if interrupted, or if
+    the timeout is exceeded.
+
+    >>> from time import sleep
+    >>> import numpy as np
+    >>> for t in FPS(frames=0.1*np.arange(10), timeout=10):
+    ...     print(f"t={t:.1f}")
+    ...     sleep(0.1)
+    t=0.0
+    t=0.1
+    t=0.2
+    t=0.3
+    t=0.4
+    t=0.5
+    t=0.6
+    t=0.7
+    t=0.8
+    t=0.9
+    """
+
+    def __init__(self, frames=200, timeout=5, tics=20, unregister=True):
+        self.frames = frames
+        self.timeout = timeout
+        self.tics = tics
+        self.unregister = unregister
+
+    def __enter__(self):
+        self._interrupted = NoInterrupt(
+            timeout=self.timeout, unregister=self.unregister
+        )
+        interrupted = self._interrupted.__enter__()
+        fps = self.Frame(interrupted=interrupted, frames=self.frames, tics=self.tics)
+        return fps
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        return self._interrupted.__exit__(exc_type, exc_value, traceback)
+
+    def __iter__(self):
+        with self as frames:
+            for frame in frames:
+                yield frame
+
+    class Frame:
+        def __init__(self, interrupted, frames, tics):
+            self.interrupted = interrupted
+            try:
+                self.the_frames = iter(frames)
+                try:
+                    self.frames = len(frames)
+                except TypeError:
+                    self.frames = None
+
+            except TypeError:
+                self.the_frames = range(frames)
+                self.frames = frames
+            self._frame = 0
+            self.tic = time.time()
+            self.tics = collections.deque([self.tic], maxlen=tics)
+
+        def __bool__(self):
+            """True while running"""
+            return not bool(self.interrupted) and (
+                self.frames is None or self.frame < self.frames
+            )
+
+        @property
+        def frame(self):
+            return self._frame
+
+        @frame.setter
+        def frame(self, frame):
+            if frame == self._frame + 1:
+                self.tics.append(time.time())
+            self._frame = frame
+
+        @property
+        def fps(self):
+            if len(self.tics) == 0:  # pragma: nocover
+                return 0  # Never happens if properly constructed.
+            elif len(self.tics) == 1:
+                return math.nan
+            else:
+                return (len(self.tics) - 1) / (self.tics[-1] - self.tics[0])
+
+        def __repr__(self):
+            return "{:.2f}".format(self.fps)
+
+        def __iter__(self):
+            for frame in self.the_frames:
+                if not self:
+                    break
+                yield frame
+                self.frame += 1
```

### Comparing `mmfutils-0.6.3/src/mmfutils/debugging.py` & `mmfutils-0.6.4/src/mmfutils/debugging.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/interface.py` & `mmfutils-0.6.4/src/mmfutils/interface.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/__pycache__/bessel.cpython-38.pyc` & `mmfutils-0.6.4/src/mmfutils/math/bessel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,800 +1,892 @@
-00000000: 550d 0d0a 0000 0000 b70b fc61 ba37 0000  U..........a.7..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 5a04 6401 6404 6c03 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 6d06 5a06 0100 6401 6403 6c07 5a08 6508  m.Z...d.d.l.Z.e.
-00000060: 5a09 6506 6504 6a0a 8301 6a0b 5a0c 6506  Z.e.e.j...j.Z.e.
-00000070: 6504 6a0a 8301 6a0d 5a0e 6405 6406 6407  e.j...j.Z.d.d.d.
-00000080: 6408 6704 5a0f 6412 6409 6405 8401 5a10  d.g.Z.d.d.d...Z.
-00000090: 6413 640a 6406 8401 5a11 640b 650c 1400  d.d.d...Z.d.e...
-000000a0: 6601 640c 640d 8401 5a12 640b 650c 1400  f.d.d...Z.d.e...
-000000b0: 6601 640e 6407 8401 5a13 6414 640f 6408  f.d.d...Z.d.d.d.
-000000c0: 8401 5a14 6410 6411 8400 5a15 6403 5300  ..Z.d.d...Z.d.S.
-000000d0: 2915 7a52 536f 6d65 2075 7469 6c69 7469  ).zRSome utiliti
-000000e0: 6573 2066 6f72 2063 6f6d 7075 7469 6e67  es for computing
-000000f0: 2070 726f 7065 7274 6965 7320 6f66 2074   properties of t
-00000100: 6865 2042 6573 7365 6c20 6675 6e63 7469  he Bessel functi
-00000110: 6f6e 7320 666f 7220 7468 6520 4456 520a  ons for the DVR.
-00000120: 6261 7369 732e e900 0000 0029 01da 0477  basis......)...w
-00000130: 6172 6e4e 2902 da02 7069 da05 6669 6e66  arnN)...pi..finf
-00000140: 6fda 0473 696e 63da 014a da06 6a5f 726f  o..sinc..J..j_ro
-00000150: 6f74 da0b 4a5f 7371 7274 5f70 6f6c 6563  ot..J_sqrt_polec
-00000160: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000170: 0a00 0000 4300 0000 73a8 0000 0064 017c  ....C...s....d.|
-00000180: 016b 0272 1874 00a0 017c 0074 006a 021b  .k.r.t...|.t.j..
-00000190: 00a1 0153 0064 027c 016b 0272 967c 007c  ...S.d.|.k.r.|.|
-000001a0: 0014 007d 0274 006a 0364 0364 0364 048d  ...}.t.j.d.d.d..
-000001b0: 028f 5801 0074 00a0 0474 057c 0083 0164  ..X..t...t.|...d
-000001c0: 056b 007c 007c 027c 020b 0064 061b 0064  .k.|.|.|...d...d
-000001d0: 0717 0014 0064 0818 0014 0064 091b 0074  .....d.....d...t
-000001e0: 00a0 067c 00a1 0174 00a0 017c 0074 006a  ...|...t...|.t.j
-000001f0: 021b 00a1 0118 007c 001b 00a1 0357 0002  .......|.....W..
-00000200: 0035 0051 0052 00a3 0053 0051 0052 0058  .5.Q.R...S.Q.R.X
-00000210: 006e 0e74 0764 0aa0 087c 01a1 0183 0182  .n.t.d...|......
-00000220: 0164 0b53 0029 0c61 f701 0000 5265 7475  .d.S.).a....Retu
-00000230: 726e 2074 6865 2060 6460 2774 6820 6465  rn the `d`'th de
-00000240: 7269 7661 7469 7665 206f 6620 6073 696e  rivative of `sin
-00000250: 6328 7829 203d 2073 696e 2878 292f 7860  c(x) = sin(x)/x`
-00000260: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00000270: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00000280: 0a20 2020 2078 203a 207b 666c 6f61 742c  .    x : {float,
-00000290: 2061 7272 6179 7d0a 2020 2020 2020 2041   array}.       A
-000002a0: 7267 756d 656e 740a 2020 2020 6420 3a20  rgument.    d : 
-000002b0: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-000002c0: 2020 2020 204f 7264 6572 206f 6620 6465       Order of de
-000002d0: 7269 7661 7469 7665 2e0a 0a20 2020 2045  rivative...    E
-000002e0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-000002f0: 2d2d 2d2d 0a20 2020 203e 3e3e 204e 203d  ----.    >>> N =
-00000300: 2033 0a20 2020 203e 3e3e 206e 702e 616c   3.    >>> np.al
-00000310: 6c63 6c6f 7365 2873 696e 6328 322e 3029  lclose(sinc(2.0)
-00000320: 2c20 6e70 2e73 696e 2832 2e30 292f 322e  , np.sin(2.0)/2.
-00000330: 3029 0a20 2020 2054 7275 650a 2020 2020  0).    True.    
-00000340: 3e3e 3e20 7072 696e 7428 2273 6b69 7020  >>> print("skip 
-00000350: 2e2e 2e22 293b 6672 6f6d 206d 6d66 7574  ...");from mmfut
-00000360: 696c 732e 6d61 7468 2e64 6966 6665 7265  ils.math.differe
-00000370: 6e74 6961 7465 2069 6d70 6f72 7420 6469  ntiate import di
-00000380: 6666 6572 656e 7469 6174 650a 2020 2020  fferentiate.    
-00000390: 736b 6970 202e 2e2e 0a20 2020 203e 3e3e  skip ....    >>>
-000003a0: 2078 203d 206e 702e 6172 7261 7928 5b2d   x = np.array([-
-000003b0: 312c 302c 302e 352c 315d 290a 2020 2020  1,0,0.5,1]).    
-000003c0: 3e3e 3e20 6e70 2e61 6c6c 636c 6f73 6528  >>> np.allclose(
-000003d0: 6469 6666 6572 656e 7469 6174 6528 6c61  differentiate(la
-000003e0: 6d62 6461 2078 3a73 696e 6328 7829 2c20  mbda x:sinc(x), 
-000003f0: 7829 2c0a 2020 2020 2e2e 2e20 2020 2020  x),.    ...     
-00000400: 2020 2020 2020 2020 7369 6e63 2878 2c20          sinc(x, 
-00000410: 643d 3129 290a 2020 2020 5472 7565 0a20  d=1)).    True. 
-00000420: 2020 2072 0100 0000 e901 0000 00da 0669     r...........i
-00000430: 676e 6f72 6529 02da 0664 6976 6964 65da  gnore)...divide.
-00000440: 0769 6e76 616c 6964 677b 14ae 47e1 7a84  .invalidg{..G.z.
-00000450: 3f69 1801 0000 679a 9999 9999 99b9 3fe7  ?i....g.......?.
-00000460: 0000 0000 0000 f03f e700 0000 0000 0008  .......?........
-00000470: 40fa 234f 6e6c 7920 643d 3020 6f72 2031  @.#Only d=0 or 1
-00000480: 2073 7570 706f 7274 6564 2028 676f 7420   supported (got 
-00000490: 643d 7b7d 292e 4e29 09da 026e 7072 0500  d={}).N)...npr..
-000004a0: 0000 7203 0000 00da 0865 7272 7374 6174  ..r......errstat
-000004b0: 65da 0577 6865 7265 da03 6162 73da 0363  e..where..abs..c
-000004c0: 6f73 da13 4e6f 7449 6d70 6c65 6d65 6e74  os..NotImplement
-000004d0: 6564 4572 726f 72da 0666 6f72 6d61 7429  edError..format)
-000004e0: 03da 0178 da01 64da 0278 32a9 0072 1a00  ...x..d..x2..r..
-000004f0: 0000 fa3e 2f55 7365 7273 2f6d 666f 7262  ...>/Users/mforb
-00000500: 6573 2f77 6f72 6b2f 6d6d 6662 622f 6d6d  es/work/mmfbb/mm
-00000510: 6675 7469 6c73 2f73 7263 2f6d 6d66 7574  futils/src/mmfut
-00000520: 696c 732f 6d61 7468 2f62 6573 7365 6c2e  ils/math/bessel.
-00000530: 7079 7205 0000 0013 0000 0073 1600 0000  pyr........s....
-00000540: 0016 0801 1001 0801 0801 1001 0401 0a01  ................
-00000550: 1c01 1cfd 1806 6302 0000 0000 0000 0000  ......c.........
-00000560: 0000 0004 0000 0003 0000 0003 0000 0073  ...............s
-00000570: 6600 0000 6401 8801 1400 7d02 6402 8800  f...d.....}.d...
-00000580: 6b02 7254 6403 7c02 6b02 7222 6404 6405  k.rTd.|.k.r"d.d.
-00000590: 8400 7d03 7162 6406 7c02 6b02 7234 6407  ..}.qbd.|.k.r4d.
-000005a0: 6405 8400 7d03 7162 6408 7c02 6b02 7246  d...}.qbd.|.k.rF
-000005b0: 6409 6405 8400 7d03 7162 8701 6601 640a  d.d...}.qb..f.d.
-000005c0: 6405 8408 7d03 6e0e 8700 8701 6602 640b  d...}.n.....f.d.
-000005d0: 6405 8408 7d03 7c03 5300 290c 61ad 0100  d...}.|.S.).a...
-000005e0: 0052 6574 7572 6e20 7468 6520 6064 6027  .Return the `d`'
-000005f0: 7468 2064 6572 6976 6174 6976 6520 6f66  th derivative of
-00000600: 2074 6865 2062 6573 7365 6c20 6675 6e63   the bessel func
-00000610: 7469 6f6e 730a 2020 2020 3a6d 6174 683a  tions.    :math:
-00000620: 604a 5f7b 5c6e 757d 287a 2960 2e0a 0a0a  `J_{\nu}(z)`....
-00000630: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000640: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000650: 2020 6e75 203a 2066 6c6f 6174 0a20 2020    nu : float.   
-00000660: 2020 2020 4f72 6465 722e 0a20 2020 2064      Order..    d
-00000670: 203a 2069 6e74 0a20 2020 2020 2020 436f   : int.       Co
-00000680: 6d70 7574 6520 7468 6520 6064 6027 7468  mpute the `d`'th
-00000690: 2064 6572 6976 6174 6976 652e 0a0a 2020   derivative...  
-000006a0: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-000006b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
-000006c0: 4a30 203d 204a 2830 2e35 293b 204a 3120  J0 = J(0.5); J1 
-000006d0: 3d20 4a28 312e 3529 3b20 4a32 203d 204a  = J(1.5); J2 = J
-000006e0: 2832 2e35 293b 0a20 2020 203e 3e3e 207a  (2.5);.    >>> z
-000006f0: 203d 2032 2e35 3b20 6e75 203d 2031 2e35   = 2.5; nu = 1.5
-00000700: 0a20 2020 203e 3e3e 2061 6273 284a 3028  .    >>> abs(J0(
-00000710: 7a29 202b 204a 3228 7a29 202d 2032 2a6e  z) + J2(z) - 2*n
-00000720: 752f 7a2a 4a31 287a 2929 203c 205f 4550  u/z*J1(z)) < _EP
-00000730: 530a 2020 2020 5472 7565 0a0a 2020 2020  S.    True..    
-00000740: 2e2e 2074 6f64 6f3a 3a20 4669 7820 746f  .. todo:: Fix to
-00000750: 6c65 7261 6e63 6573 2073 6f20 7468 6174  lerances so that
-00000760: 2074 6865 7365 2061 7265 2063 6f6d 7075   these are compu
-00000770: 7465 6420 746f 206d 6163 6869 6e65 2070  ted to machine p
-00000780: 7265 6369 7369 6f6e 2e0a 2020 2020 e902  recision..    ..
-00000790: 0000 0072 0100 0000 7209 0000 0063 0100  ...r....r....c..
-000007a0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-000007b0: 0000 5300 0000 731a 0000 0074 00a0 0164  ..S...s....t...d
-000007c0: 017c 0014 0074 021b 00a1 0174 037c 0083  .|...t.....t.|..
-000007d0: 0114 0053 00a9 024e 721c 0000 0029 0472  ...S...Nr....).r
-000007e0: 1000 0000 da04 7371 7274 7203 0000 0072  ......sqrtr....r
-000007f0: 0500 0000 a901 da01 7a72 1a00 0000 721a  ........zr....r.
-00000800: 0000 0072 1b00 0000 da01 6a50 0000 0073  ...r......jP...s
-00000810: 0200 0000 0001 7a0c 4a2e 3c6c 6f63 616c  ......z.J.<local
-00000820: 733e 2e6a e903 0000 0063 0100 0000 0000  s>.j.....c......
-00000830: 0000 0000 0000 0100 0000 0500 0000 5300  ..............S.
-00000840: 0000 7324 0000 0074 00a0 0164 017c 001b  ..s$...t...d.|..
-00000850: 0074 021b 00a1 0174 037c 0083 0174 00a0  .t.....t.|...t..
-00000860: 047c 00a1 0118 0014 0053 0072 1d00 0000  .|.......S.r....
-00000870: a905 7210 0000 0072 1e00 0000 7203 0000  ..r....r....r...
-00000880: 0072 0500 0000 7214 0000 0072 1f00 0000  .r....r....r....
-00000890: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000008a0: 2100 0000 5500 0000 7302 0000 0000 01e9  !...U...s.......
-000008b0: 0500 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000008c0: 0001 0000 0006 0000 0053 0000 0073 3800  .........S...s8.
-000008d0: 0000 7400 a001 6401 7c00 1b00 7402 1b00  ..t...d.|...t...
-000008e0: a101 7c00 1b00 6402 7c00 7c00 1400 1800  ..|...d.|.|.....
-000008f0: 7403 7c00 8301 1400 6403 7400 a004 7c00  t.|.....d.t...|.
-00000900: a101 1400 1800 1400 5300 2904 4e72 1c00  ........S.).Nr..
-00000910: 0000 720e 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
-00000920: 0072 1f00 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00000930: 721b 0000 0072 2100 0000 5a00 0000 7304  r....r!...Z...s.
-00000940: 0000 0000 0236 ff63 0100 0000 0000 0000  .....6.c........
-00000950: 0000 0000 0100 0000 0400 0000 1300 0000  ................
-00000960: 730e 0000 0074 006a 01a0 0288 007c 00a1  s....t.j.....|..
-00000970: 0253 00a9 014e 2903 da02 7370 da07 7370  .S...N)...sp..sp
-00000980: 6563 6961 6c5a 026a 6e72 1f00 0000 a901  ecialZ.jnr......
-00000990: da02 6e75 721a 0000 0072 1b00 0000 7221  ..nur....r....r!
-000009a0: 0000 0066 0000 0073 0200 0000 0001 6301  ...f...s......c.
-000009b0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-000009c0: 0000 0013 0000 0073 3000 0000 7400 8801  .......s0...t...
-000009d0: 6401 1800 8800 6401 1800 8302 7c00 8301  d.....d.....|...
-000009e0: 7400 8801 6401 1700 8800 6401 1800 8302  t...d.....d.....
-000009f0: 7c00 8301 1800 6402 1b00 5300 2903 4e72  |.....d...S.).Nr
-00000a00: 0900 0000 6700 0000 0000 0000 4029 0172  ....g.......@).r
-00000a10: 0600 0000 721f 0000 00a9 0272 1800 0000  ....r......r....
-00000a20: 7229 0000 0072 1a00 0000 721b 0000 0072  r)...r....r....r
-00000a30: 2100 0000 6c00 0000 7302 0000 0000 0172  !...l...s......r
-00000a40: 1a00 0000 2904 7229 0000 0072 1800 0000  ....).r)...r....
-00000a50: da03 6e75 3272 2100 0000 721a 0000 0072  ..nu2r!...r....r
-00000a60: 2a00 0000 721b 0000 0072 0600 0000 3700  *...r....r....7.
-00000a70: 0000 7316 0000 0000 1508 0108 0108 020a  ..s.............
-00000a80: 0308 020a 0308 020a 0c0e 060e 0372 1c00  .............r..
-00000a90: 0000 6303 0000 0000 0000 0000 0000 0008  ..c.............
-00000aa0: 0000 0006 0000 0043 0000 0073 ec00 0000  .......C...s....
-00000ab0: 6401 7d03 6402 7d04 6403 7d05 7400 a001  d.}.d.}.d.}.t...
-00000ac0: 7c01 7c00 6b04 a101 72d6 7c04 7c02 6b04  |.|.k...r.|.|.k.
-00000ad0: 72d6 7c05 6402 3700 7d05 7402 7c00 6404  r.|.d.7.}.t.|.d.
-00000ae0: 8d01 7c01 8301 7402 7c00 6402 1800 6404  ..|...t.|.d...d.
-00000af0: 8d01 7c01 8301 1b00 7d06 7400 a003 7400  ..|.....}.t...t.
-00000b00: a004 7c06 a101 6402 6b04 7400 a005 7c06  ..|...d.k.t...|.
-00000b10: a101 7c06 a103 7d06 7c01 7d07 7c01 7c06  ..|...}.|.}.|.|.
-00000b20: 6402 7c06 7c06 1400 1700 1b00 1800 7d01  d.|.|.........}.
-00000b30: 7400 a003 7c01 6403 6b00 7c07 6405 1b00  t...|.d.k.|.d...
-00000b40: 7c01 a103 7d01 7c04 7d03 7400 a006 7400  |...}.|.}.t...t.
-00000b50: a004 7c06 7c01 1b00 a101 a101 7d04 7c04  ..|.|.......}.|.
-00000b60: 7c03 6b05 720c 7c05 6406 6b04 720c 7407  |.k.r.|.d.k.r.t.
-00000b70: 6407 6408 7c04 7c02 6602 1600 1700 8301  d.d.|.|.f.......
-00000b80: 0100 71d6 710c 7400 a003 7c01 7c00 6b00  ..q.q.t...|.|.k.
-00000b90: 6403 7c01 a103 7d01 7c01 5300 2909 612c  d.|...}.|.S.).a,
-00000ba0: 0100 0052 6574 7572 6e20 7468 6520 726f  ...Return the ro
-00000bb0: 6f74 7320 6f66 2074 6865 2062 6573 7365  ots of the besse
-00000bc0: 6c20 6675 6e63 7469 6f6e 2063 6c6f 7365  l function close
-00000bd0: 7374 2074 6f20 6078 6020 666f 756e 640a  st to `x` found.
-00000be0: 2020 2020 6279 2069 7465 7261 7469 6e67      by iterating
-00000bf0: 2061 2076 6572 7369 6f6e 206f 6620 4e65   a version of Ne
-00000c00: 7774 6f6e 2773 206d 6574 686f 642e 0a0a  wton's method...
-00000c10: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000c20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000c30: 2020 6e75 203a 2066 6c6f 6174 0a20 2020    nu : float.   
-00000c40: 2020 2020 4f72 6465 7220 6f66 2062 6573      Order of bes
-00000c50: 7365 6c20 6675 6e63 7469 6f6e 0a20 2020  sel function.   
-00000c60: 204e 203a 2069 6e74 0a20 2020 2020 2020   N : int.       
-00000c70: 4e75 6d62 6572 206f 6620 726f 6f74 730a  Number of roots.
-00000c80: 2020 2020 7265 6c5f 746f 6c20 3a20 666c      rel_tol : fl
-00000c90: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-00000ca0: 2020 2020 2044 6573 6972 6564 2072 656c       Desired rel
-00000cb0: 6174 6976 6520 746f 6c65 7261 6e63 6520  ative tolerance 
-00000cc0: 666f 7220 726f 6f74 732e 0a20 2020 20e9  for roots..    .
-00000cd0: 0a00 0000 7209 0000 0072 0100 0000 7228  ....r....r....r(
-00000ce0: 0000 0072 1c00 0000 e914 0000 007a 296a  ...r.........z)j
-00000cf0: 5f72 6f6f 743a 2074 6572 6d69 6e61 7469  _root: terminati
-00000d00: 6e67 2069 7465 7261 7469 6f6e 2077 6974  ng iteration wit
-00000d10: 6820 6572 726f 7220 7a23 2567 203c 2025  h error z#%g < %
-00000d20: 6720 6c65 7373 2074 6861 7420 7370 6563  g less that spec
-00000d30: 6966 6965 6420 7265 6c5f 746f 6c29 0872  ified rel_tol).r
-00000d40: 1000 0000 da03 616e 7972 0600 0000 7212  ......anyr....r.
-00000d50: 0000 0072 1300 0000 da04 7369 676e da03  ...r......sign..
-00000d60: 6d61 7872 0200 0000 2908 7229 0000 0072  maxr....).r)...r
-00000d70: 1700 0000 da07 7265 6c5f 746f 6c5a 076f  ......rel_tolZ.o
-00000d80: 6c64 5f65 7272 da03 6572 725a 066e 5f69  ld_err..errZ.n_i
-00000d90: 7465 72da 0168 5a03 785f 6172 1a00 0000  ter..hZ.x_ar....
-00000da0: 721a 0000 0072 1b00 0000 da08 6a5f 726f  r....r......j_ro
-00000db0: 6f74 5f78 7200 0000 732a 0000 0000 1004  ot_xr...s*......
-00000dc0: 0104 0104 0116 0108 0120 011e 0104 0114  ......... ......
-00000dd0: 0116 0104 0114 0110 0102 0102 010a ff02  ................
-00000de0: ff04 0404 0112 0c72 3400 0000 6303 0000  .......r4...c...
-00000df0: 0000 0000 0000 0000 0012 0000 000c 0000  ................
-00000e00: 0043 0000 0073 7c02 0000 7400 7c00 8301  .C...s|...t.|...
-00000e10: 7d03 6401 7c00 1400 7d04 7c04 6402 6b00  }.d.|...}.|.d.k.
-00000e20: 7224 7401 6403 8301 8201 9002 6e54 6404  r$t.d.......nTd.
-00000e30: 7c04 6b02 7240 7402 7403 a004 6404 7c01  |.k.r@t.t...d.|.
-00000e40: 6404 1700 a102 1400 5300 6405 7c04 6b02  d.......S.d.|.k.
-00000e50: 72d2 7403 a005 6406 6407 6408 6409 640a  r.t...d.d.d.d.d.
-00000e60: 640b 640c 640d 640e 640f 670a a101 7d05  d.d.d.d.d.g...}.
-00000e70: 7c01 6410 6b04 72c2 7403 a004 6411 7c01  |.d.k.r.t...d.|.
-00000e80: 6404 1700 a102 7d06 7c06 7402 1400 7d07  d.....}.|.t...}.
-00000e90: 7c06 6412 1700 7402 1400 7d08 7406 6413  |.d...t...}.t.d.
-00000ea0: 8301 4400 5d18 7d09 7403 a007 7c08 7c08  ..D.].}.t...|.|.
-00000eb0: a102 0100 7c08 7c07 3700 7d08 719a 7403  ....|.|.7.}.q.t.
-00000ec0: a008 7c05 7c08 6602 a101 5300 7c05 6414  ..|.|.f...S.|.d.
-00000ed0: 7c01 8502 1900 5300 9001 6ea6 7403 6a09  |.....S...n.t.j.
-00000ee0: 7c01 6404 1700 740a 6415 8d02 7d05 7403  |.d...t.d...}.t.
-00000ef0: 6a09 7c01 6404 1700 740a 6415 8d02 7d0a  j.|.d...t.d...}.
-00000f00: 7c00 7c00 6416 1300 1700 7c05 6402 3c00  |.|.d.....|.d.<.
-00000f10: 7c03 7c05 6402 1900 8301 7c0a 6402 3c00  |.|.d.....|.d.<.
-00000f20: 7406 6404 7c01 6404 1700 8302 4400 5d68  t.d.|.d.....D.]h
-00000f30: 7d06 7c05 7c06 6404 1800 1900 7402 1700  }.|.|.d.....t...
-00000f40: 7c05 7c06 3c00 7c03 7c05 7c06 1900 8301  |.|.<.|.|.|.....
-00000f50: 7c0a 7c06 3c00 7c0a 7c06 1900 7c0a 7c06  |.|.<.|.|...|.|.
-00000f60: 6404 1800 1900 1400 6402 6b04 9001 7224  d.......d.k...r$
-00000f70: 7c05 7c06 0500 1900 7402 3700 0300 3c00  |.|.....t.7...<.
-00000f80: 7c03 7c05 7c06 1900 8301 7c0a 7c06 3c00  |.|.|.....|.|.<.
-00000f90: 9001 714c 9001 7124 7c05 6414 6417 8502  ..qL..q$|.d.d...
-00000fa0: 1900 7d08 7c05 6404 6414 8502 1900 7d0b  ..}.|.d.d.....}.
-00000fb0: 7c0a 6414 6417 8502 1900 7d0c 7c0a 6404  |.d.d.....}.|.d.
-00000fc0: 6414 8502 1900 7d0d 7406 6401 8301 4400  d.....}.t.d...D.
-00000fd0: 5d8a 7d06 7c08 7c0b 1700 6401 1b00 7d0e  ].}.|.|...d...}.
-00000fe0: 7c03 7c0e 8301 7d0f 7c0f 7c0c 1400 7d10  |.|...}.|.|...}.
-00000ff0: 7c0f 7c0d 1400 7d11 7403 a00b 7c10 7c11  |.|...}.t...|.|.
-00001000: 1400 6402 6b01 a101 9002 7306 740c 8201  ..d.k.....s.t...
-00001010: 7403 a00d 7c10 6402 6b05 7c0e 7c08 a103  t...|.d.k.|.|...
-00001020: 7d08 7403 a00d 7c11 6402 6b05 7c0e 7c0b  }.t...|.d.k.|.|.
-00001030: a103 7d0b 7403 a00d 7c10 6402 6b05 7c0f  ..}.t...|.d.k.|.
-00001040: 7c0c a103 7d0c 7403 a00d 7c11 6402 6b05  |...}.t...|.d.k.
-00001050: 7c0f 7c0d a103 7d0d 9001 71c6 7c0d 7c08  |.|...}...q.|.|.
-00001060: 1400 7c0c 7c0b 1400 1800 7c0d 7c0c 1800  ..|.|.....|.|...
-00001070: 1b00 7d05 740e 7c00 7c05 7c02 6418 8d03  ..}.t.|.|.|.d...
-00001080: 5300 6414 5300 2919 619c 0500 0052 6574  S.d.S.).a....Ret
-00001090: 7572 6e20 7468 6520 6669 7273 7420 4e20  urn the first N 
-000010a0: 706f 7369 7469 7665 2072 6f6f 7473 206f  positive roots o
-000010b0: 6620 7468 6520 6265 7373 656c 2066 756e  f the bessel fun
-000010c0: 6374 696f 6e0a 2020 2020 604a 5f6e 7528  ction.    `J_nu(
-000010d0: 7829 602e 0a0a 2020 2020 5061 7261 6d65  x)`...    Parame
-000010e0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-000010f0: 2d2d 2d0a 2020 2020 6e75 203a 2066 6c6f  ---.    nu : flo
-00001100: 6174 0a20 2020 2020 2020 4f72 6465 7220  at.       Order 
-00001110: 6f66 2062 6573 7365 6c20 6675 6e63 7469  of bessel functi
-00001120: 6f6e 0a20 2020 204e 203a 2069 6e74 0a20  on.    N : int. 
-00001130: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
-00001140: 726f 6f74 730a 2020 2020 7265 6c5f 746f  roots.    rel_to
-00001150: 6c20 3a20 666c 6f61 742c 206f 7074 696f  l : float, optio
-00001160: 6e61 6c0a 2020 2020 2020 2044 6573 6972  nal.       Desir
-00001170: 6564 2072 656c 6174 6976 6520 746f 6c65  ed relative tole
-00001180: 7261 6e63 6520 666f 7220 726f 6f74 732e  rance for roots.
-00001190: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
-000011a0: 2d2d 2d2d 2d0a 2020 2020 5468 6520 6765  -----.    The ge
-000011b0: 6e65 7261 6c20 6d65 7468 6f64 2069 7320  neral method is 
-000011c0: 746f 2066 6972 7374 2065 7374 696d 6174  to first estimat
-000011d0: 6520 7468 6520 726f 6f74 7320 7769 7468  e the roots with
-000011e0: 2061 0a20 2020 2062 6973 6563 7469 6f6e   a.    bisection
-000011f0: 2f73 6563 616e 7420 6d65 7468 6f64 2c20  /secant method, 
-00001200: 616e 6420 7468 656e 2070 6f6c 6973 6820  and then polish 
-00001210: 7468 656d 2075 7369 6e67 204e 6577 746f  them using Newto
-00001220: 6e27 730a 2020 2020 6d65 7468 6f64 2e0a  n's.    method..
-00001230: 0a20 2020 2057 6520 7374 6172 7420 6279  .    We start by
-00001240: 2065 7374 696d 6174 696e 6720 7468 6520   estimating the 
-00001250: 6c6f 7765 7220 626f 756e 6420 666f 7220  lower bound for 
-00001260: 7468 6520 6669 7273 7420 666f 720a 2020  the first for.  
-00001270: 2020 6e6f 6e2d 6e65 6761 7469 7665 203a    non-negative :
-00001280: 6d61 7468 3a60 5c6e 7560 0a0a 2020 2020  math:`\nu`..    
-00001290: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
-000012a0: 205c 6e75 202b 205c 6e75 5e7b 312f 337d   \nu + \nu^{1/3}
-000012b0: 203c 206a 5f7b 5c6e 752c 317d 203c 205c   < j_{\nu,1} < \
-000012c0: 6e75 202b 2031 2e38 3535 3735 205c 6e75  nu + 1.85575 \nu
-000012d0: 5e7b 312f 337d 202b 205c 7069 0a0a 2020  ^{1/3} + \pi..  
-000012e0: 2020 5468 656e 2c20 7573 696e 6720 7468    Then, using th
-000012f0: 6520 6661 6374 2074 6861 7420 7468 6520  e fact that the 
-00001300: 726f 6f74 7320 6172 6520 7370 6163 6564  roots are spaced
-00001310: 2062 7920 6174 206c 6561 7374 0a20 2020   by at least.   
-00001320: 203a 6d61 7468 3a60 5c70 6960 2c20 7765   :math:`\pi`, we
-00001330: 2073 7465 7020 7468 726f 7567 6820 7468   step through th
-00001340: 6520 7369 676e 2063 6861 6e67 6573 2074  e sign changes t
-00001350: 6f20 6272 6163 6b65 7420 616c 6c20 6f66  o bracket all of
-00001360: 0a20 2020 2074 6865 2064 6573 6972 6564  .    the desired
-00001370: 2072 6f6f 7473 2e0a 0a20 2020 206c 6f77   roots...    low
-00001380: 6573 7420 726f 6f74 2075 7369 6e67 2074  est root using t
-00001390: 6865 2066 6f6c 6c6f 7769 6e67 0a20 2020  he following.   
-000013a0: 2068 6575 7269 7374 6963 730a 0a20 2020   heuristics..   
-000013b0: 202e 2e20 6d61 7468 3a3a 0a20 2020 2020   .. math::.     
-000013c0: 2020 6a5f 7b5c 6e75 2c73 7d20 5c61 7070    j_{\nu,s} \app
-000013d0: 726f 7820 5c62 6567 696e 7b63 6173 6573  rox \begin{cases
-000013e0: 7d0a 2020 2020 2020 2020 2020 325c 7371  }.          2\sq
-000013f0: 7274 7b5c 6e75 202b 2031 7d0a 2020 2020  rt{\nu + 1}.    
-00001400: 2020 2020 2020 2020 2026 202d 3120 3c20           & -1 < 
-00001410: 5c6e 7520 3c20 2d30 2e38 5c5c 0a20 2020  \nu < -0.8\\.   
-00001420: 2020 2020 2020 205c 6c65 6674 285c 6672         \left(\fr
-00001430: 6163 7b5c 6e75 7d7b 327d 202b 205c 6672  ac{\nu}{2} + \fr
-00001440: 6163 7b33 7d7b 347d 5c72 6967 6874 295c  ac{3}{4}\right)\
-00001450: 7069 0a20 2020 2020 2020 2020 2020 2020  pi.             
-00001460: 2620 2d30 2e38 203c 205c 6e75 203c 2032  & -0.8 < \nu < 2
-00001470: 2e35 5c5c 0a20 2020 2020 2020 2020 205c  .5\\.          \
-00001480: 6e75 202b 2031 2e38 3535 3735 205c 6e75  nu + 1.85575 \nu
-00001490: 5e7b 312f 337d 0a20 2020 2020 2020 2020  ^{1/3}.         
-000014a0: 2020 2020 2620 322e 3520 5c6c 6571 205c      & 2.5 \leq \
-000014b0: 6e75 0a20 2020 2020 2020 5c65 6e64 7b63  nu.       \end{c
-000014c0: 6173 6573 7d0a 0a20 2020 2045 7861 6d70  ases}..    Examp
-000014d0: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-000014e0: 0a20 2020 203e 3e3e 206e 7520 3d20 322e  .    >>> nu = 2.
-000014f0: 350a 2020 2020 3e3e 3e20 6a5f 203d 206a  5.    >>> j_ = j
-00001500: 5f72 6f6f 7428 6e75 2c20 3230 3030 290a  _root(nu, 2000).
-00001510: 2020 2020 3e3e 3e20 4a5f 203d 204a 286e      >>> J_ = J(n
-00001520: 7529 286a 5f29 0a0a 2020 2020 5468 6573  u)(j_)..    Thes
-00001530: 6520 6172 6520 726f 6f74 7321 0a0a 2020  e are roots!..  
-00001540: 2020 3e3e 3e20 6e70 2e6d 6178 2861 6273    >>> np.max(abs
-00001550: 284a 5f2f 6a5f 2929 203c 205f 4550 530a  (J_/j_)) < _EPS.
-00001560: 2020 2020 5472 7565 0a0a 2020 2020 5468      True..    Th
-00001570: 6579 2061 7265 2061 6c73 6f20 6469 7374  ey are also dist
-00001580: 696e 6374 0a0a 2020 2020 3e3e 3e20 7069  inct..    >>> pi
-00001590: 203c 206d 696e 286e 702e 6469 6666 286a   < min(np.diff(j
-000015a0: 5f29 290a 2020 2020 5472 7565 0a0a 2020  _)).    True..  
-000015b0: 2020 416e 6420 7468 6520 7370 6163 696e    And the spacin
-000015c0: 6720 6973 2064 6563 7265 6173 696e 672c  g is decreasing,
-000015d0: 206d 6561 6e69 6e67 2077 6520 6861 7665   meaning we have
-000015e0: 206e 6f74 2073 6b69 7070 6564 2061 6e79   not skipped any
-000015f0: 2e0a 0a20 2020 203e 3e3e 206e 702e 6d61  ...    >>> np.ma
-00001600: 7828 6e70 2e64 6966 6628 6e70 2e64 6966  x(np.diff(np.dif
-00001610: 6628 6a5f 2929 2920 3c20 300a 2020 2020  f(j_))) < 0.    
-00001620: 5472 7565 0a20 2020 2072 1c00 0000 7201  True.    r....r.
-00001630: 0000 007a 176e 7520 6d75 7374 2062 6520  ...z.nu must be 
-00001640: 6e6f 6e2d 6e65 6761 7469 7665 7209 0000  non-negativer...
-00001650: 0072 2200 0000 67ad 0635 5440 f911 4067  .r"...g..5T@..@g
-00001660: a60b e46a a8e6 1e40 676a b4bd 08e9 ce25  ...j...@gj.....%
-00001670: 4067 649c 252b e421 2c40 67bc 5ce1 6a83  @gd.%+.!,@g.\.j.
-00001680: 3831 4067 500c f3b5 0d5f 3440 67dc b1c5  81@gP...._4@g...
-00001690: d6fa 8437 4067 42f6 2a88 82aa 3a40 67c0  ...7@gB.*...:@g.
-000016a0: 5b38 f0c4 cf3d 4067 2b25 c0f4 6a7a 4040  [8...=@g+%..jz@@
-000016b0: 722c 0000 00e9 0b00 0000 6700 0000 0000  r,........g.....
-000016c0: 00e0 3f72 2400 0000 4ea9 01da 0564 7479  ..?r$...N....dty
-000016d0: 7065 6755 5555 5555 55d5 3fe9 ffff ffff  pegUUUUUU.?.....
-000016e0: 2903 7229 0000 0072 1700 0000 7231 0000  ).r)...r....r1..
-000016f0: 0029 0f72 0600 0000 da0a 5661 6c75 6545  .).r......ValueE
-00001700: 7272 6f72 7203 0000 0072 1000 0000 da06  rrorr....r......
-00001710: 6172 616e 6765 da05 6172 7261 79da 0572  arange..array..r
-00001720: 616e 6765 da06 6172 6374 616e da06 6873  ange..arctan..hs
-00001730: 7461 636b da05 656d 7074 79da 0566 6c6f  tack..empty..flo
-00001740: 6174 da03 616c 6cda 0e41 7373 6572 7469  at..all..Asserti
-00001750: 6f6e 4572 726f 7272 1200 0000 7234 0000  onErrorr....r4..
-00001760: 0029 1272 2900 0000 da01 4e72 3100 0000  .).r).....Nr1...
-00001770: da02 4a5f 722b 0000 0072 1700 0000 da01  ..J_r+...r......
-00001780: 6e5a 036e 7069 da02 7830 da01 635a 024a  nZ.npi..x0..cZ.J
-00001790: 78da 0278 315a 024a 305a 024a 315a 0578  x..x1Z.J0Z.J1Z.x
-000017a0: 5f6d 6964 5a05 4a5f 6d69 64da 0273 30da  _midZ.J_mid..s0.
-000017b0: 0273 3172 1a00 0000 721a 0000 0072 1b00  .s1r....r....r..
-000017c0: 0000 7207 0000 00a3 0000 0073 6e00 0000  ..r........sn...
-000017d0: 003f 0802 0802 0801 0c01 0803 1401 0805  .?..............
-000017e0: 0402 0201 0201 0201 0201 0201 0201 0201  ................
-000017f0: 0201 0201 02f6 02ff 040e 0801 1001 0801  ................
-00001800: 0c01 0c01 0c01 0a01 0e02 1003 1201 1202  ................
-00001810: 1001 1001 1201 1401 1001 1a01 1001 1803  ................
-00001820: 0c01 0c01 0c01 0c01 0c03 0c01 0801 0801  ................
-00001830: 0801 1801 1201 1201 1201 1607 1801 6303  ..............c.
-00001840: 0000 0000 0000 0000 0000 000b 0000 0006  ................
-00001850: 0000 0003 0000 0073 ca01 0000 7400 7c00  .......s....t.|.
-00001860: 8301 7d03 7400 7c00 6401 8302 7d04 7c00  ..}.t.|.d...}.|.
-00001870: 7c00 1400 6402 1800 8806 1b00 8806 1b00  |...d...........
-00001880: 7d05 7401 6a02 6403 7403 6404 8d02 7d06  }.t.j.d.t.d...}.
-00001890: 7401 a004 8806 a101 7c04 8806 8301 1400  t.......|.......
-000018a0: 7c06 6401 3c00 7c05 6401 1800 7c06 6401  |.d.<.|.d...|.d.
-000018b0: 1900 1400 7c06 6405 3c00 6406 7c05 1400  ....|.d.<.d.|...
-000018c0: 8806 1b00 7c06 6401 1900 1400 7c06 6407  ....|.d.....|.d.
-000018d0: 3c00 6408 7c05 1400 8806 1b00 8806 1b00  <.d.|...........
-000018e0: 7c05 6401 1800 6409 1300 1700 7c06 6401  |.d...d.....|.d.
-000018f0: 1900 1400 7c06 640a 3c00 640b 640c 8806  ....|.d.<.d.d...
-00001900: 1b00 8806 1b00 7c05 6401 1800 1700 1400  ......|.d.......
-00001910: 7c05 1400 8806 1b00 7c06 6401 1900 1400  |.......|.d.....
-00001920: 7c06 640d 3c00 7401 a005 640e 7406 7c06  |.d.<.t...d.t.|.
-00001930: 8301 6401 1800 a102 7d07 7c06 7c07 6401  ..d.....}.|.|.d.
-00001940: 1700 1900 7c07 6401 1700 1b00 8900 7401  ....|.d.......t.
-00001950: a005 640e 7406 7c06 8301 6409 1800 a102  ..d.t.|...d.....
-00001960: 7d07 7c06 7c07 6409 1700 1900 7c07 6409  }.|.|.d.....|.d.
-00001970: 1700 1b00 8901 640f 7d08 7401 a007 6410  ......d.}.t...d.
-00001980: 7401 a004 6409 a101 1400 7408 1400 8806  t...d.....t.....
-00001990: 1400 7c08 1400 a101 6411 1300 8903 7401  ..|.....d.....t.
-000019a0: a007 6412 7408 1400 8806 1400 7c08 1400  ..d.t.......|...
-000019b0: a101 6411 1300 8902 7c03 6601 6413 6414  ..d.....|.f.d.d.
-000019c0: 8401 8905 7c03 7c04 6602 6415 6416 8401  ....|.|.f.d.d...
-000019d0: 8904 640e 7c02 6b02 9001 7296 8700 8703  ..d.|.k...r.....
-000019e0: 8705 8706 6604 6417 6418 8408 7d09 7c09  ....f.d.d...}.|.
-000019f0: 5300 6401 7c02 6b02 9001 72b8 8701 8702  S.d.|.k...r.....
-00001a00: 8704 8705 8706 6605 6419 641a 8408 7d0a  ......f.d.d...}.
-00001a10: 7c0a 5300 7409 641b a00a 7c02 a101 8301  |.S.t.d...|.....
-00001a20: 8201 641c 5300 291d 6134 1100 0052 6574  ..d.S.).a4...Ret
-00001a30: 7572 6e20 6120 6675 6e63 7469 6f6e 2074  urn a function t
-00001a40: 6861 7420 636f 6d70 7574 6573 2074 6865  hat computes the
-00001a50: 2060 6460 2774 6820 6465 7269 7661 7469   `d`'th derivati
-00001a60: 7665 206f 660a 2020 2020 6073 7172 7428  ve of.    `sqrt(
-00001a70: 7a29 2a4a 286e 752c 7a29 2f28 7a20 2d20  z)*J(nu,z)/(z - 
-00001a80: 7a6e 2960 2077 6865 7265 2060 7a6e 6020  zn)` where `zn` 
-00001a90: 6973 2061 2072 6f6f 743a 2060 4a28 6e75  is a root: `J(nu
-00001aa0: 2c20 7a6e 2920 3d20 3060 2e0a 2020 2020  , zn) = 0`..    
-00001ab0: 5468 6973 2063 6f6d 6269 6e61 7469 6f6e  This combination
-00001ac0: 2061 7070 6561 7273 2069 6e20 7468 6520   appears in the 
-00001ad0: 4265 7373 656c 2066 756e 6374 696f 6e20  Bessel function 
-00001ae0: 4456 5220 6261 7369 732e 0a0a 2020 2020  DVR basis...    
-00001af0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00001b00: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6e75  ---------.    nu
-00001b10: 203a 2066 6c6f 6174 0a20 2020 2020 2020   : float.       
-00001b20: 4f72 6465 720a 2020 2020 7a6e 203a 2066  Order.    zn : f
-00001b30: 6c6f 6174 0a20 2020 2020 2020 526f 6f74  loat.       Root
-00001b40: 206f 6620 604a 286e 752c 207a 2960 0a20   of `J(nu, z)`. 
-00001b50: 2020 2064 203a 2069 6e74 0a20 2020 2020     d : int.     
-00001b60: 2020 4f72 6465 7220 6f66 2064 6572 6976    Order of deriv
-00001b70: 6174 6976 6520 746f 2074 616b 652e 0a0a  ative to take...
-00001b80: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
-00001b90: 2d2d 2d0a 2020 2020 2e2e 206d 6174 683a  ---.    .. math:
-00001ba0: 3a0a 2020 2020 2020 205c 6672 6163 7b5c  :.       \frac{\
-00001bb0: 7371 7274 7b7a 7d4a 5f7b 5c6e 757d 287a  sqrt{z}J_{\nu}(z
-00001bc0: 297d 7b7a 202d 207a 5f7b 6e7d 7d0a 0a20  )}{z - z_{n}}.. 
-00001bd0: 2020 2041 7320 3a6d 6174 683a 607a 6020     As :math:`z` 
-00001be0: 6170 7072 6f61 6368 6573 203a 6d61 7468  approaches :math
-00001bf0: 3a60 7a5f 6e60 2c20 7468 6973 2068 6173  :`z_n`, this has
-00001c00: 2074 6865 2066 6f72 6d20 6f66 2060 302f   the form of `0/
-00001c10: 3060 2c0a 2020 2020 736f 206f 6e65 2063  0`,.    so one c
-00001c20: 616e 2061 7070 6c79 2061 2066 6f72 6d20  an apply a form 
-00001c30: 6f66 206c 2748 6f70 6974 616c 2773 2072  of l'Hopital's r
-00001c40: 756c 6520 746f 2072 6564 7563 6520 7468  ule to reduce th
-00001c50: 650a 2020 2020 726f 756e 642d 6f66 6620  e.    round-off 
-00001c60: 6572 726f 722e 2020 5468 6520 7370 6563  error.  The spec
-00001c70: 6966 6965 6420 666f 726d 206f 6620 7468  ified form of th
-00001c80: 6520 6675 6e63 7469 6f6e 2068 6173 2062  e function has b
-00001c90: 6565 6e0a 2020 2020 6368 6f73 656e 2066  een.    chosen f
-00001ca0: 6f72 2073 7065 6369 616c 2070 726f 7065  or special prope
-00001cb0: 7274 6965 7320 6f66 2074 6865 2042 6573  rties of the Bes
-00001cc0: 7365 6c20 6675 6e63 7469 6f6e 732e 2020  sel functions.  
-00001cd0: 4578 7072 6573 730a 2020 2020 7468 6520  Express.    the 
-00001ce0: 6675 6e63 7469 6f6e 2061 730a 0a20 2020  function as..   
-00001cf0: 202e 2e20 6d61 7468 3a3a 0a20 2020 2020   .. math::.     
-00001d00: 2020 4628 7a29 2026 3d20 5c66 7261 637b    F(z) &= \frac{
-00001d10: 6628 7a29 7d7b 7a20 2d20 7a5f 6e7d 2020  f(z)}{z - z_n}  
-00001d20: 3d20 5c66 7261 637b 5c73 7172 747b 7a7d  = \frac{\sqrt{z}
-00001d30: 4a5f 7b5c 6e75 7d28 7a29 7d7b 7a20 2d20  J_{\nu}(z)}{z - 
-00001d40: 7a5f 6e7d 5c5c 0a20 2020 2020 2020 4627  z_n}\\.       F'
-00001d50: 287a 2920 263d 205c 6672 6163 7b66 2728  (z) &= \frac{f'(
-00001d60: 7a29 7d7b 7a20 2d20 7a5f 6e7d 202d 205c  z)}{z - z_n} - \
-00001d70: 6672 6163 7b66 287a 297d 7b28 7a20 2d20  frac{f(z)}{(z - 
-00001d80: 7a5f 6e29 5e32 7d0a 0a0a 2020 2020 4c65  z_n)^2}...    Le
-00001d90: 7420 3a6d 6174 683a 605c 6465 6c74 6120  t :math:`\delta 
-00001da0: 3d20 7a20 2d20 7a5f 6e60 2e20 2043 6c6f  = z - z_n`.  Clo
-00001db0: 7365 2074 6f20 7468 6520 7369 6e67 756c  se to the singul
-00001dc0: 6172 2070 6f69 6e74 2077 6520 7573 650a  ar point we use.
-00001dd0: 2020 2020 7468 6520 5461 796c 6f72 2073      the Taylor s
-00001de0: 6572 6965 733a 0a0a 2020 2020 2e2e 206d  eries:..    .. m
-00001df0: 6174 683a 3a0a 2020 2020 2020 205c 7375  ath::.       \su
-00001e00: 6d5f 7b6d 3d30 7d5e 7b5c 696e 6674 797d  m_{m=0}^{\infty}
-00001e10: 5c66 7261 637b 615f 6d5c 6465 6c74 615e  \frac{a_m\delta^
-00001e20: 7b6d 7d7d 7b6d 217d 0a0a 2020 2020 2e2e  {m}}{m!}..    ..
-00001e30: 206d 6174 683a 3a0a 2020 2020 2020 2046   math::.       F
-00001e40: 287a 2920 263d 2066 2728 7a5f 6e29 0a20  (z) &= f'(z_n). 
-00001e50: 2020 2020 2020 2020 2020 202b 205c 7375             + \su
-00001e60: 6d5f 7b6d 3d33 7d5e 7b5c 696e 6674 797d  m_{m=3}^{\infty}
-00001e70: 5c66 7261 637b 665e 7b28 6d29 7d28 7a5f  \frac{f^{(m)}(z_
-00001e80: 6e29 5c64 656c 7461 5e7b 6d2d 317d 7d7b  n)\delta^{m-1}}{
-00001e90: 6d21 7d0a 2020 2020 2020 2020 2020 2020  m!}.            
-00001ea0: 3d20 5c73 756d 5f7b 6d3d 307d 5e7b 5c69  = \sum_{m=0}^{\i
-00001eb0: 6e66 7479 7d5c 6672 6163 7b66 5e7b 286d  nfty}\frac{f^{(m
-00001ec0: 2b31 297d 287a 5f6e 295c 6465 6c74 615e  +1)}(z_n)\delta^
-00001ed0: 7b6d 7d7d 7b28 6d2b 3129 6d21 7d5c 5c0a  {m}}{(m+1)m!}\\.
-00001ee0: 2020 2020 2020 2020 615f 6d20 263d 205c          a_m &= \
-00001ef0: 6672 6163 7b66 5e7b 286d 2b31 297d 7d7b  frac{f^{(m+1)}}{
-00001f00: 6d2b 317d 5c5c 0a20 2020 2020 2020 4627  m+1}\\.       F'
-00001f10: 287a 2920 263d 205c 7375 6d5f 7b6d 3d33  (z) &= \sum_{m=3
-00001f20: 7d5e 7b5c 696e 6674 797d 5c66 7261 637b  }^{\infty}\frac{
-00001f30: 286d 2d31 2966 5e7b 286d 297d 287a 5f6e  (m-1)f^{(m)}(z_n
-00001f40: 295c 6465 6c74 615e 7b6d 2d32 7d7d 7b6d  )\delta^{m-2}}{m
-00001f50: 217d 0a20 2020 2020 2020 2020 2020 2020  !}.             
-00001f60: 3d20 5c73 756d 5f7b 6d3d 317d 5e7b 5c69  = \sum_{m=1}^{\i
-00001f70: 6e66 7479 7d5c 6672 6163 7b66 5e7b 286d  nfty}\frac{f^{(m
-00001f80: 2b32 297d 287a 5f6e 295c 6465 6c74 615e  +2)}(z_n)\delta^
-00001f90: 7b6d 7d7d 7b28 6d2b 3229 6d21 7d5c 5c0a  {m}}{(m+2)m!}\\.
-00001fa0: 2020 2020 2020 2020 2061 5f6d 2026 3d20           a_m &= 
-00001fb0: 5c66 7261 637b 665e 7b28 6d2b 3229 7d7d  \frac{f^{(m+2)}}
-00001fc0: 7b6d 2b32 7d5c 5c0a 0a20 2020 2054 6865  {m+2}\\..    The
-00001fd0: 2066 6972 7374 2066 6577 2064 6572 6976   first few deriv
-00001fe0: 6174 6976 6573 2061 7265 2070 7265 7365  atives are prese
-00001ff0: 6e74 6564 2068 6572 653a 0a0a 2020 2020  nted here:..    
-00002000: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
-00002010: 2066 287a 2920 263d 205c 7371 7274 7b7a   f(z) &= \sqrt{z
-00002020: 7d4a 5f7b 5c6e 757d 287a 295c 5c0a 2020  }J_{\nu}(z)\\.  
-00002030: 2020 2020 2066 2728 7a29 2026 3d20 5c66       f'(z) &= \f
-00002040: 7261 637b 4a5f 7b5c 6e75 7d28 7a29 7d7b  rac{J_{\nu}(z)}{
-00002050: 325c 7371 7274 7b7a 7d7d 202b 205c 7371  2\sqrt{z}} + \sq
-00002060: 7274 7b7a 7d4a 275f 7b5c 6e75 7d28 7a29  rt{z}J'_{\nu}(z)
-00002070: 0a20 2020 2020 2020 2020 2020 2020 203d  .              =
-00002080: 205c 6672 6163 7b66 287a 297d 7b32 7a7d   \frac{f(z)}{2z}
-00002090: 202b 205c 7371 7274 7b7a 7d4a 275f 7b5c   + \sqrt{z}J'_{\
-000020a0: 6e75 7d28 7a29 5c5c 0a20 2020 2020 2020  nu}(z)\\.       
-000020b0: 6627 2728 7a29 2026 3d20 5c73 7172 747b  f''(z) &= \sqrt{
-000020c0: 7a7d 4a5f 7b5c 6e75 7d28 7a29 5c6c 6566  z}J_{\nu}(z)\lef
-000020d0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000020e0: 2020 2020 2020 2020 5c66 7261 637b 5c6e          \frac{\n
-000020f0: 755e 3220 2d20 5c74 6672 6163 7b31 7d7b  u^2 - \tfrac{1}{
-00002100: 347d 7d7b 7a5e 327d 202d 2031 5c72 6967  4}}{z^2} - 1\rig
-00002110: 6874 290a 2020 2020 2020 2020 2020 2020  ht).            
-00002120: 2020 203d 2066 287a 295c 6c65 6674 285c     = f(z)\left(\
-00002130: 6672 6163 7b5c 6e75 5e32 202d 205c 7466  frac{\nu^2 - \tf
-00002140: 7261 637b 317d 7b34 7d7d 7b7a 5e32 7d20  rac{1}{4}}{z^2} 
-00002150: 2d20 315c 7269 6768 7429 5c5c 0a20 2020  - 1\right)\\.   
-00002160: 2020 2020 6627 2727 287a 2920 263d 2066      f'''(z) &= f
-00002170: 2728 7a29 5c6c 6566 7428 5c66 7261 637b  '(z)\left(\frac{
-00002180: 5c6e 755e 3220 2d20 5c74 6672 6163 7b31  \nu^2 - \tfrac{1
-00002190: 7d7b 347d 7d7b 7a5e 327d 202d 2031 5c72  }{4}}{z^2} - 1\r
-000021a0: 6967 6874 290a 2020 2020 2020 2020 2020  ight).          
-000021b0: 2020 2020 202d 2032 6628 7a29 5c66 7261       - 2f(z)\fra
-000021c0: 637b 5c6e 755e 3220 2d20 5c74 6672 6163  c{\nu^2 - \tfrac
-000021d0: 7b31 7d7b 347d 7d7b 7a5e 337d 5c5c 0a20  {1}{4}}{z^3}\\. 
-000021e0: 2020 2020 2020 665e 7b28 3429 7d28 7a29        f^{(4)}(z)
-000021f0: 2026 3d0a 2020 2020 2020 2066 287a 295c   &=.       f(z)\
-00002200: 6c65 6674 5b0a 2020 2020 2020 2020 2020  left[.          
-00002210: 5c6c 6566 7428 5c66 7261 637b 5c6e 755e  \left(\frac{\nu^
-00002220: 3220 2d20 5c74 6672 6163 7b31 7d7b 347d  2 - \tfrac{1}{4}
-00002230: 7d7b 7a5e 327d 202d 2031 5c72 6967 6874  }{z^2} - 1\right
-00002240: 295e 320a 2020 2020 2020 2020 2020 2b20  )^2.          + 
-00002250: 365c 6672 6163 7b5c 6e75 5e32 202d 205c  6\frac{\nu^2 - \
-00002260: 7466 7261 637b 317d 7b34 7d7d 7b7a 5e34  tfrac{1}{4}}{z^4
-00002270: 7d5c 7269 6768 745d 0a20 2020 2020 2020  }\right].       
-00002280: 2d20 3466 2728 7a29 5c66 7261 637b 5c6e  - 4f'(z)\frac{\n
-00002290: 755e 3220 2d20 5c74 6672 6163 7b31 7d7b  u^2 - \tfrac{1}{
-000022a0: 347d 7d7b 7a5e 337d 0a20 2020 202e 2e20  4}}{z^3}.    .. 
-000022b0: 4368 6563 6b65 6420 7769 7468 204d 6170  Checked with Map
-000022c0: 6c65 2e0a 0a20 2020 2045 7661 6c75 6174  le...    Evaluat
-000022d0: 6564 2061 7420 7468 6520 726f 6f74 203a  ed at the root :
-000022e0: 6d61 7468 3a60 7a3d 7a5f 6e60 2074 6865  math:`z=z_n` the
-000022f0: 7365 2062 6563 6f6d 653a 0a0a 2020 2020  se become:..    
-00002300: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
-00002310: 2066 287a 5f7b 6e7d 2920 263d 2030 5c5c   f(z_{n}) &= 0\\
-00002320: 0a20 2020 2020 2020 6627 287a 5f7b 6e7d  .       f'(z_{n}
-00002330: 2920 263d 205c 7371 7274 7b7a 5f7b 6e7d  ) &= \sqrt{z_{n}
-00002340: 7d4a 275f 7b5c 6e75 7d28 7a5f 7b6e 7d29  }J'_{\nu}(z_{n})
-00002350: 5c5c 0a20 2020 2020 2020 6627 2728 7a5f  \\.       f''(z_
-00002360: 7b6e 7d29 2026 3d20 305c 5c0a 2020 2020  {n}) &= 0\\.    
-00002370: 2020 2066 2727 2728 7a5f 7b6e 7d29 2026     f'''(z_{n}) &
-00002380: 3d20 6627 287a 5f7b 6e7d 295c 6c65 6674  = f'(z_{n})\left
-00002390: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000023a0: 2020 2020 2020 2020 2020 5c66 7261 637b            \frac{
-000023b0: 5c6e 755e 3220 2d20 5c74 6672 6163 7b31  \nu^2 - \tfrac{1
-000023c0: 7d7b 347d 7d7b 7a5f 7b6e 7d5e 327d 202d  }{4}}{z_{n}^2} -
-000023d0: 2031 5c72 6967 6874 295c 5c0a 2020 2020   1\right)\\.    
-000023e0: 2020 2066 5e7b 2834 297d 287a 5f7b 6e7d     f^{(4)}(z_{n}
-000023f0: 2920 263d 202d 2034 6627 287a 5f7b 6e7d  ) &= - 4f'(z_{n}
-00002400: 295c 6672 6163 7b5c 6e75 5e32 202d 205c  )\frac{\nu^2 - \
-00002410: 7466 7261 637b 317d 7b34 7d7d 7b7a 5f7b  tfrac{1}{4}}{z_{
-00002420: 6e7d 5e33 7d0a 0a20 2020 2077 6974 6820  n}^3}..    with 
-00002430: 626f 7468 2074 6865 2066 756e 6374 696f  both the functio
-00002440: 6e20 616e 6420 7468 6520 7365 636f 6e64  n and the second
-00002450: 2064 6572 6976 6174 6976 6520 7661 6e69   derivative vani
-00002460: 7368 696e 672e 0a0a 2020 2020 546f 2064  shing...    To d
-00002470: 6574 6572 6d69 6e65 2077 6865 7265 2074  etermine where t
-00002480: 6f20 7573 6520 7468 6973 2066 6f72 6d75  o use this formu
-00002490: 6c61 2c20 7765 206d 6174 6368 2074 6865  la, we match the
-000024a0: 2065 7374 696d 6174 650a 2020 2020 726f   estimate.    ro
-000024b0: 756e 646f 6666 2065 7272 6f72 2077 6974  undoff error wit
-000024c0: 6820 7468 6520 7472 756e 6361 7469 6f6e  h the truncation
-000024d0: 2065 7272 6f72 2e20 2054 6865 2042 6573   error.  The Bes
-000024e0: 7365 6c20 6675 6e63 7469 6f6e 730a 2020  sel functions.  
-000024f0: 2020 6172 6520 6f66 206f 7264 6572 2075    are of order u
-00002500: 6e69 7479 2061 6e64 2061 7265 2074 7970  nity and are typ
-00002510: 6963 616c 6c79 2063 616c 6375 6c61 7465  ically calculate
-00002520: 6420 746f 2061 6e20 6162 736f 6c75 7465  d to an absolute
-00002530: 0a20 2020 2061 6363 7572 6163 7920 6f66  .    accuracy of
-00002540: 203a 6d61 7468 3a60 5c65 7073 696c 6f6e   :math:`\epsilon
-00002550: 602e 2020 5468 6520 726f 756e 642d 6f66  `.  The round-of
-00002560: 6620 6572 726f 7220 696e 2074 6865 0a20  f error in the. 
-00002570: 2020 206e 756d 6572 6174 6f72 2069 7320     numerator is 
-00002580: 3a6d 6174 683a 605c 6570 7369 6c6f 6e20  :math:`\epsilon 
-00002590: 6628 7a29 6020 616e 6420 3a6d 6174 683a  f(z)` and :math:
-000025a0: 605c 6570 7369 6c6f 6e20 5c73 7172 747b  `\epsilon \sqrt{
-000025b0: 327d 0a20 2020 207a 5f6e 6020 696e 2074  2}.    z_n` in t
-000025c0: 6865 2064 656e 6f6d 696e 6174 6f72 2e20  he denominator. 
-000025d0: 2054 6865 2072 6f75 6e64 6f66 6620 6572   The roundoff er
-000025e0: 726f 7273 2069 6e20 7468 6520 6465 6e6f  rors in the deno
-000025f0: 6d69 6e61 746f 720a 2020 2020 646f 6d69  minator.    domi
-00002600: 6e61 7465 2062 6f74 6820 6361 7365 733a  nate both cases:
-00002610: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
-00002620: 2020 2020 2020 205c 6465 6c74 6120 4628         \delta F(
-00002630: 7a29 2026 5c73 696d 205c 6570 7369 6c6f  z) &\sim \epsilo
-00002640: 6e20 5c66 7261 637b 5c73 7172 747b 327d  n \frac{\sqrt{2}
-00002650: 7a5f 6e20 4628 7a29 7d7b 5c64 656c 7461  z_n F(z)}{\delta
-00002660: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00002670: 2020 2020 2020 5c73 696d 205c 6672 6163        \sim \frac
-00002680: 7b5c 7371 7274 7b32 7d5c 6570 7369 6c6f  {\sqrt{2}\epsilo
-00002690: 6e20 7a5f 6e20 6628 7a29 7d7b 5c64 656c  n z_n f(z)}{\del
-000026a0: 7461 5e32 7d0a 2020 2020 2020 2020 2020  ta^2}.          
-000026b0: 2020 2020 2020 2020 2020 5c73 696d 205c            \sim \
-000026c0: 6672 6163 7b5c 7371 7274 7b32 7d5c 6570  frac{\sqrt{2}\ep
-000026d0: 7369 6c6f 6e20 7a5f 6e20 6627 287a 5f6e  silon z_n f'(z_n
-000026e0: 297d 7b5c 6465 6c74 617d 5c5c 0a20 2020  )}{\delta}\\.   
-000026f0: 2020 2020 5c64 656c 7461 2046 2728 7a29      \delta F'(z)
-00002700: 2026 5c73 696d 205c 6672 6163 7b32 5c65   &\sim \frac{2\e
-00002710: 7073 696c 6f6e 207a 5f6e 2066 287a 297d  psilon z_n f(z)}
-00002720: 7b5c 6465 6c74 615e 337d 0a20 2020 2020  {\delta^3}.     
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 5c73 696d 205c 6672 6163 7b32 5c65 7073  \sim \frac{2\eps
-00002750: 696c 6f6e 207a 5f6e 2066 2728 7a5f 6e29  ilon z_n f'(z_n)
-00002760: 7d7b 5c64 656c 7461 5e32 7d0a 0a20 2020  }{\delta^2}..   
-00002770: 2054 6f20 6368 6f6f 7365 2074 6865 2061   To choose the a
-00002780: 7070 726f 7072 6961 7465 2074 7261 6e73  ppropriate trans
-00002790: 6974 696f 6e20 706f 696e 742c 2077 6520  ition point, we 
-000027a0: 6571 7561 7465 2068 616c 6620 6f66 2074  equate half of t
-000027b0: 6869 730a 2020 2020 7769 7468 2074 6865  his.    with the
-000027c0: 2074 7275 6e63 6174 696f 6e20 6572 726f   truncation erro
-000027d0: 7220 746f 2074 7261 6e73 6974 696f 6e20  r to transition 
-000027e0: 706f 696e 7473 3a0a 0a20 2020 202e 2e20  points:..    .. 
-000027f0: 6d61 7468 3a3a 0a20 2020 2020 2020 5c64  math::.       \d
-00002800: 656c 7461 5f63 2026 5c73 696d 205c 6c65  elta_c &\sim \le
-00002810: 6674 280a 2020 2020 2020 2020 2020 5c66  ft(.          \f
-00002820: 7261 637b 3732 5c65 7073 696c 6f6e 207a  rac{72\epsilon z
-00002830: 5f6e 2066 2728 7a5f 6e29 7d7b 5c73 7172  _n f'(z_n)}{\sqr
-00002840: 747b 327d 665e 7b28 3429 7d28 7a5f 6e29  t{2}f^{(4)}(z_n)
-00002850: 7d0a 2020 2020 2020 2020 2020 5c72 6967  }.          \rig
-00002860: 6874 295e 7b31 2f34 7d0a 2020 2020 2020  ht)^{1/4}.      
-00002870: 205c 7369 6d20 5c6c 6566 7428 5c66 7261   \sim \left(\fra
-00002880: 637b 3732 5c65 7073 696c 6f6e 207a 5f6e  c{72\epsilon z_n
-00002890: 7d7b 5c73 7172 747b 327d 7d20 5c72 6967  }{\sqrt{2}} \rig
-000028a0: 6874 295e 7b31 2f34 7d5c 5c0a 2020 2020  ht)^{1/4}\\.    
-000028b0: 2020 205c 6465 6c74 615f 6327 2026 5c73     \delta_c' &\s
-000028c0: 696d 205c 6c65 6674 2831 3230 5c65 7073  im \left(120\eps
-000028d0: 696c 6f6e 207a 5f6e 5c72 6967 6874 295e  ilon z_n\right)^
-000028e0: 7b31 2f35 7d0a 0a20 2020 2074 6865 2066  {1/5}..    the f
-000028f0: 6163 7420 7468 6174 203a 5c6d 6174 683a  act that :\math:
-00002900: 6066 287a 2960 2062 6568 6176 6573 0a20  `f(z)` behaves. 
-00002910: 2020 2061 7379 6d70 746f 7469 6361 6c6c     asymptoticall
-00002920: 7920 6173 2061 203a 6d61 7468 3a60 5c73  y as a :math:`\s
-00002930: 7172 747b 322f 5c70 697d 5c63 6f73 287a  qrt{2/\pi}\cos(z
-00002940: 202b 205c 7068 6929 6020 616e 6420 736f   + \phi)` and so
-00002950: 2061 6c6c 0a20 2020 2064 6572 6976 6174   all.    derivat
-00002960: 6976 6573 2068 6176 6520 6573 7365 6e74  ives have essent
-00002970: 6961 6c6c 7920 7468 6520 7361 6d65 206d  ially the same m
-00002980: 6167 6e69 7475 6465 2e0a 0a20 2020 2045  agnitude...    E
-00002990: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-000029a0: 2d2d 2d2d 0a20 2020 203e 3e3e 206e 7520  ----.    >>> nu 
-000029b0: 3d20 352e 350a 2020 2020 3e3e 3e20 7a6e  = 5.5.    >>> zn
-000029c0: 203d 206a 5f72 6f6f 7428 6e75 2c32 3129   = j_root(nu,21)
-000029d0: 5b2d 315d 0a20 2020 203e 3e3e 2061 6273  [-1].    >>> abs
-000029e0: 287a 6e20 2d20 3733 2e36 3233 3631 3331  (zn - 73.6236131
-000029f0: 3832 3531 3735 3333 3931 3634 3629 203c  8251753391646) <
-00002a00: 2031 652d 3136 0a20 2020 2054 7275 650a   1e-16.    True.
-00002a10: 2020 2020 3e3e 3e20 666c 6f61 7428 4a5f      >>> float(J_
-00002a20: 7371 7274 5f70 6f6c 6528 6e75 2c7a 6e29  sqrt_pole(nu,zn)
-00002a30: 287a 6e29 2920 2020 2320 646f 6374 6573  (zn))   # doctes
-00002a40: 743a 202b 454c 4c49 5053 4953 0a20 2020  t: +ELLIPSIS.   
-00002a50: 202d 302e 3739 3637 3738 3537 3637 3830   -0.796778576780
-00002a60: 3031 332e 2e2e 0a0a 2020 2020 2d30 2e37  013.....    -0.7
-00002a70: 3936 3737 3835 3736 3738 3030 3133 3132  9677857678001312
-00002a80: 3937 3630 0a0a 2020 2020 596f 7520 6361  9760..    You ca
-00002a90: 6e20 616c 736f 2075 7365 2061 2076 6563  n also use a vec
-00002aa0: 746f 7220 6f66 2060 7a6e 602c 2062 7574  tor of `zn`, but
-00002ab0: 206f 6e6c 7920 6966 2069 7420 6973 2063   only if it is c
-00002ac0: 6f6d 6d65 6e73 7572 6174 650a 2020 2020  ommensurate.    
-00002ad0: 7769 7468 2074 6865 2061 7267 756d 656e  with the argumen
-00002ae0: 743a 0a0a 2020 2020 3e3e 3e20 7a6e 203d  t:..    >>> zn =
-00002af0: 206a 5f72 6f6f 7428 6e75 2c32 3129 0a20   j_root(nu,21). 
-00002b00: 2020 203e 3e3e 2066 6c6f 6174 284a 5f73     >>> float(J_s
-00002b10: 7172 745f 706f 6c65 286e 752c 207a 6e29  qrt_pole(nu, zn)
-00002b20: 287a 6e5b 2d31 5d29 5b32 305d 2920 2320  (zn[-1])[20]) # 
-00002b30: 646f 6374 6573 743a 202b 454c 4c49 5053  doctest: +ELLIPS
-00002b40: 4953 0a20 2020 202d 302e 3739 3637 3738  IS.    -0.796778
-00002b50: 3537 3637 3830 3031 332e 2e2e 0a20 2020  576780013....   
-00002b60: 2072 0900 0000 6700 0000 0000 00d0 3fe9   r....g.......?.
-00002b70: 0700 0000 7236 0000 0072 2200 0000 e9fc  ....r6...r".....
-00002b80: ffff ffe9 0400 0000 e912 0000 0072 1c00  .............r..
-00002b90: 0000 7224 0000 0069 f4ff ffff e908 0000  ..r$...i........
-00002ba0: 00e9 0600 0000 7201 0000 0072 0d00 0000  ......r....r....
-00002bb0: 69d0 0200 0067 5555 5555 5555 c53f 6920  i....gUUUUUU.?i 
-00002bc0: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
-00002bd0: 0200 0000 0300 0000 5300 0000 7312 0000  ........S...s...
-00002be0: 0074 00a0 017c 00a1 017c 017c 0083 0114  .t...|...|.|....
-00002bf0: 0053 0072 2500 0000 a902 7210 0000 0072  .S.r%.....r....r
-00002c00: 1e00 0000 2902 7220 0000 0072 0600 0000  ....).r ...r....
-00002c10: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00002c20: 0166 c601 0000 7302 0000 0000 017a 164a  .f....s......z.J
-00002c30: 5f73 7172 745f 706f 6c65 2e3c 6c6f 6361  _sqrt_pole.<loca
-00002c40: 6c73 3e2e 6663 0300 0000 0000 0000 0000  ls>.fc..........
-00002c50: 0000 0300 0000 0400 0000 5300 0000 7328  ..........S...s(
-00002c60: 0000 007c 017c 0083 0164 011b 0074 00a0  ...|.|...d...t..
-00002c70: 017c 00a1 011b 0074 00a0 017c 00a1 017c  .|.....t...|...|
-00002c80: 027c 0083 0114 0017 0053 0072 1d00 0000  .|.......S.r....
-00002c90: 7251 0000 0029 0372 2000 0000 7206 0000  rQ...).r ...r...
-00002ca0: 00da 0264 4a72 1a00 0000 721a 0000 0072  ...dJr....r....r
-00002cb0: 1b00 0000 da02 6466 c901 0000 7302 0000  ......df....s...
-00002cc0: 0000 017a 174a 5f73 7172 745f 706f 6c65  ...z.J_sqrt_pole
-00002cd0: 2e3c 6c6f 6361 6c73 3e2e 6466 6301 0000  .<locals>.dfc...
-00002ce0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-00002cf0: 0013 0000 0073 3400 0000 7c00 8803 1800  .....s4...|.....
-00002d00: 7d01 7400 a001 7402 7c01 8301 8801 6b04  }.t...t.|.....k.
-00002d10: 7400 a003 8802 7c00 8301 7c01 7404 1700  t.....|...|.t...
-00002d20: a102 7405 8800 7c01 8302 a103 5300 7225  ..t...|.....S.r%
-00002d30: 0000 0029 0672 1000 0000 7212 0000 0072  ...).r....r....r
-00002d40: 1300 0000 720b 0000 00da 055f 5449 4e59  ....r......_TINY
-00002d50: da07 5f48 6f72 6e65 72a9 0272 2000 0000  .._Horner..r ...
-00002d60: da05 6465 6e6f 6d29 04da 0361 5f46 da07  ..denom)...a_F..
-00002d70: 6465 6c74 615f 6372 5200 0000 da02 7a6e  delta_crR.....zn
-00002d80: 721a 0000 0072 1b00 0000 da01 46ce 0100  r....r......F...
-00002d90: 0073 0c00 0000 0001 0801 0401 0a01 1201  .s..............
-00002da0: 08fd 7a16 4a5f 7371 7274 5f70 6f6c 652e  ..z.J_sqrt_pole.
-00002db0: 3c6c 6f63 616c 733e 2e46 6301 0000 0000  <locals>.Fc.....
-00002dc0: 0000 0000 0000 0002 0000 000a 0000 0013  ................
-00002dd0: 0000 0073 4000 0000 7c00 8804 1800 7d01  ...s@...|.....}.
-00002de0: 7400 a001 7402 7c01 8301 8801 6b04 7400  t...t.|.....k.t.
-00002df0: a003 8802 7c00 8301 7400 a003 8803 7c00  ....|...t.....|.
-00002e00: 8301 7c01 a102 1800 7c01 a102 7404 8800  ..|.....|...t...
-00002e10: 7c01 8302 a103 5300 7225 0000 0029 0572  |.....S.r%...).r
-00002e20: 1000 0000 7212 0000 0072 1300 0000 720b  ....r....r....r.
-00002e30: 0000 0072 5600 0000 7257 0000 0029 05da  ...rV...rW...)..
-00002e40: 0461 5f64 46da 0864 6465 6c74 615f 6372  .a_dF..ddelta_cr
-00002e50: 5400 0000 7252 0000 0072 5b00 0000 721a  T...rR...r[...r.
-00002e60: 0000 0072 1b00 0000 da02 6446 d901 0000  ...r......dF....
-00002e70: 730c 0000 0000 0108 0104 010a 011e 0108  s...............
-00002e80: fd7a 174a 5f73 7172 745f 706f 6c65 2e3c  .z.J_sqrt_pole.<
-00002e90: 6c6f 6361 6c73 3e2e 6446 720f 0000 004e  locals>.dFr....N
-00002ea0: 290b 7206 0000 0072 1000 0000 da05 7a65  ).r....r......ze
-00002eb0: 726f 73da 066f 626a 6563 7472 1e00 0000  ros..objectr....
-00002ec0: 723a 0000 00da 036c 656e 7213 0000 00da  r:.....lenr.....
-00002ed0: 045f 4550 5372 1500 0000 7216 0000 0029  ._EPSr....r....)
-00002ee0: 0b72 2900 0000 725b 0000 0072 1800 0000  .r)...r[...r....
-00002ef0: 7244 0000 0072 5300 0000 7247 0000 005a  rD...rS...rG...Z
-00002f00: 0366 7a6e da01 6d5a 0566 315f 6636 725c  .fzn..mZ.f1_f6r\
-00002f10: 0000 0072 5f00 0000 721a 0000 0029 0772  ...r_...r....).r
-00002f20: 5900 0000 725d 0000 0072 5e00 0000 725a  Y...r]...r^...rZ
-00002f30: 0000 0072 5400 0000 7252 0000 0072 5b00  ...rT...rR...r[.
-00002f40: 0000 721b 0000 0072 0800 0000 3201 0000  ..r....r....2...
-00002f50: 7332 0000 0000 7a08 010a 0314 020e 0116  s2....z.........
-00002f60: 0114 0118 0128 012c 0214 0114 0214 0114  .....(.,........
-00002f70: 0404 0224 011a 020c 030e 030a 0212 0804  ...$............
-00002f80: 010a 0214 0804 0263 0200 0000 0000 0000  .......c........
-00002f90: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00002fa0: 734c 0000 0074 00a0 017c 01a1 017d 0164  sL...t...|...}.d
-00002fb0: 017c 0114 007d 0274 0274 0374 047c 0083  .|...}.t.t.t.|..
-00002fc0: 0183 0183 0144 005d 247d 037c 027c 007c  .....D.]$}.|.|.|
-00002fd0: 0319 0037 007d 027c 0364 016b 0472 227c  ...7.}.|.d.k.r"|
-00002fe0: 027c 017c 031b 0039 007d 0271 227c 0253  .|.|...9.}.q"|.S
-00002ff0: 0029 027a aa52 6574 7572 6e20 7375 6d28  .).z.Return sum(
-00003000: 615b 6e5d 2f6e 212a 645e 6e29 2065 7661  a[n]/n!*d^n) eva
-00003010: 6c75 6174 6564 2075 7369 6e67 2048 6f72  luated using Hor
-00003020: 6e65 7227 730a 2020 2020 6d65 7468 6f64  ner's.    method
-00003030: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
-00003040: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00003050: 203e 3e3e 2061 203d 205b 312c 2031 2c20   >>> a = [1, 1, 
-00003060: 322c 2033 2a32 2c20 342a 332a 325d 0a20  2, 3*2, 4*3*2]. 
-00003070: 2020 203e 3e3e 2064 203d 2032 0a20 2020     >>> d = 2.   
-00003080: 203e 3e3e 205f 486f 726e 6572 2861 2c64   >>> _Horner(a,d
-00003090: 290a 2020 2020 3331 2e30 0a20 2020 2072  ).    31.0.    r
-000030a0: 0100 0000 2905 7210 0000 00da 0761 7361  ....).r......asa
-000030b0: 7272 6179 da08 7265 7665 7273 6564 723c  rray..reversedr<
-000030c0: 0000 0072 6200 0000 2904 da01 6172 1800  ...rb...)...ar..
-000030d0: 0000 da03 616e 7372 4500 0000 721a 0000  ....ansrE...r...
-000030e0: 0072 1a00 0000 721b 0000 0072 5600 0000  .r....r....rV...
-000030f0: e601 0000 730e 0000 0000 0b0a 0108 0114  ....s...........
-00003100: 010c 0108 010e 0172 5600 0000 2901 7201  .......rV...).r.
-00003110: 0000 0029 0172 0100 0000 2901 7201 0000  ...).r....).r...
-00003120: 0029 16da 075f 5f64 6f63 5f5f da08 7761  .)...__doc__..wa
-00003130: 726e 696e 6773 7202 0000 00da 056e 756d  rningsr......num
-00003140: 7079 7210 0000 0072 0300 0000 7204 0000  pyr....r....r...
-00003150: 005a 0d73 6369 7079 2e73 7065 6369 616c  .Z.scipy.special
-00003160: da05 7363 6970 7972 2600 0000 da06 646f  ..scipyr&.....do
-00003170: 7562 6c65 da03 6570 7372 6300 0000 da04  uble..epsrc.....
-00003180: 7469 6e79 7255 0000 00da 075f 5f61 6c6c  tinyrU.....__all
-00003190: 5f5f 7205 0000 0072 0600 0000 7234 0000  __r....r....r4..
-000031a0: 0072 0700 0000 7208 0000 0072 5600 0000  .r....r....rV...
-000031b0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-000031c0: 1b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000031d0: 0000 7320 0000 0004 020c 0208 0110 0208  ..s ............
-000031e0: 0204 020c 010c 030c 030a 240a 3b10 3110  ..........$.;.1.
-000031f0: 7f00 100a 7f00 35                        ......5
+00000000: 7222 2222 536f 6d65 2075 7469 6c69 7469  r"""Some utiliti
+00000010: 6573 2066 6f72 2063 6f6d 7075 7469 6e67  es for computing
+00000020: 2070 726f 7065 7274 6965 7320 6f66 2074   properties of t
+00000030: 6865 2042 6573 7365 6c20 6675 6e63 7469  he Bessel functi
+00000040: 6f6e 7320 666f 7220 7468 6520 4456 520a  ons for the DVR.
+00000050: 6261 7369 732e 2222 220a 6672 6f6d 2077  basis.""".from w
+00000060: 6172 6e69 6e67 7320 696d 706f 7274 2077  arnings import w
+00000070: 6172 6e0a 0a69 6d70 6f72 7420 6e75 6d70  arn..import nump
+00000080: 7920 6173 206e 700a 6672 6f6d 206e 756d  y as np.from num
+00000090: 7079 2069 6d70 6f72 7420 7069 2c20 6669  py import pi, fi
+000000a0: 6e66 6f0a 0a69 6d70 6f72 7420 7363 6970  nfo..import scip
+000000b0: 792e 7370 6563 6961 6c0a 0a73 7020 3d20  y.special..sp = 
+000000c0: 7363 6970 790a 0a5f 4550 5320 3d20 6669  scipy.._EPS = fi
+000000d0: 6e66 6f28 6e70 2e64 6f75 626c 6529 2e65  nfo(np.double).e
+000000e0: 7073 0a5f 5449 4e59 203d 2066 696e 666f  ps._TINY = finfo
+000000f0: 286e 702e 646f 7562 6c65 292e 7469 6e79  (np.double).tiny
+00000100: 0a0a 0a5f 5f61 6c6c 5f5f 203d 205b 2273  ...__all__ = ["s
+00000110: 696e 6322 2c20 224a 222c 2022 6a5f 726f  inc", "J", "j_ro
+00000120: 6f74 222c 2022 4a5f 7371 7274 5f70 6f6c  ot", "J_sqrt_pol
+00000130: 6522 5d0a 0a0a 6465 6620 7369 6e63 2878  e"]...def sinc(x
+00000140: 2c20 643d 3029 3a0a 2020 2020 7222 2222  , d=0):.    r"""
+00000150: 5265 7475 726e 2074 6865 2060 6460 2774  Return the `d`'t
+00000160: 6820 6465 7269 7661 7469 7665 206f 6620  h derivative of 
+00000170: 6073 696e 6328 7829 203d 2073 696e 2878  `sinc(x) = sin(x
+00000180: 292f 7860 2e0a 0a20 2020 2050 6172 616d  )/x`...    Param
+00000190: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000001a0: 2d2d 2d2d 0a20 2020 2078 203a 207b 666c  ----.    x : {fl
+000001b0: 6f61 742c 2061 7272 6179 7d0a 2020 2020  oat, array}.    
+000001c0: 2020 2041 7267 756d 656e 740a 2020 2020     Argument.    
+000001d0: 6420 3a20 696e 742c 206f 7074 696f 6e61  d : int, optiona
+000001e0: 6c0a 2020 2020 2020 204f 7264 6572 206f  l.       Order o
+000001f0: 6620 6465 7269 7661 7469 7665 2e0a 0a20  f derivative... 
+00000200: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00000210: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
+00000220: 204e 203d 2033 0a20 2020 203e 3e3e 206e   N = 3.    >>> n
+00000230: 702e 616c 6c63 6c6f 7365 2873 696e 6328  p.allclose(sinc(
+00000240: 322e 3029 2c20 6e70 2e73 696e 2832 2e30  2.0), np.sin(2.0
+00000250: 292f 322e 3029 0a20 2020 2054 7275 650a  )/2.0).    True.
+00000260: 2020 2020 3e3e 3e20 7072 696e 7428 2273      >>> print("s
+00000270: 6b69 7020 2e2e 2e22 293b 6672 6f6d 206d  kip ...");from m
+00000280: 6d66 7574 696c 732e 6d61 7468 2e64 6966  mfutils.math.dif
+00000290: 6665 7265 6e74 6961 7465 2069 6d70 6f72  ferentiate impor
+000002a0: 7420 6469 6666 6572 656e 7469 6174 650a  t differentiate.
+000002b0: 2020 2020 736b 6970 202e 2e2e 0a20 2020      skip ....   
+000002c0: 203e 3e3e 2078 203d 206e 702e 6172 7261   >>> x = np.arra
+000002d0: 7928 5b2d 312c 302c 302e 352c 315d 290a  y([-1,0,0.5,1]).
+000002e0: 2020 2020 3e3e 3e20 6e70 2e61 6c6c 636c      >>> np.allcl
+000002f0: 6f73 6528 6469 6666 6572 656e 7469 6174  ose(differentiat
+00000300: 6528 6c61 6d62 6461 2078 3a73 696e 6328  e(lambda x:sinc(
+00000310: 7829 2c20 7829 2c0a 2020 2020 2e2e 2e20  x), x),.    ... 
+00000320: 2020 2020 2020 2020 2020 2020 7369 6e63              sinc
+00000330: 2878 2c20 643d 3129 290a 2020 2020 5472  (x, d=1)).    Tr
+00000340: 7565 0a20 2020 2022 2222 0a20 2020 2069  ue.    """.    i
+00000350: 6620 3020 3d3d 2064 3a0a 2020 2020 2020  f 0 == d:.      
+00000360: 2020 7265 7475 726e 206e 702e 7369 6e63    return np.sinc
+00000370: 2878 202f 206e 702e 7069 290a 2020 2020  (x / np.pi).    
+00000380: 656c 6966 2031 203d 3d20 643a 0a20 2020  elif 1 == d:.   
+00000390: 2020 2020 2078 3220 3d20 7820 2a20 780a       x2 = x * x.
+000003a0: 2020 2020 2020 2020 7769 7468 206e 702e          with np.
+000003b0: 6572 7273 7461 7465 2864 6976 6964 653d  errstate(divide=
+000003c0: 2269 676e 6f72 6522 2c20 696e 7661 6c69  "ignore", invali
+000003d0: 643d 2269 676e 6f72 6522 293a 0a20 2020  d="ignore"):.   
+000003e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000003f0: 6e70 2e77 6865 7265 280a 2020 2020 2020  np.where(.      
+00000400: 2020 2020 2020 2020 2020 6162 7328 7829            abs(x)
+00000410: 203c 2030 2e30 312c 0a20 2020 2020 2020   < 0.01,.       
+00000420: 2020 2020 2020 2020 2078 202a 2028 7832           x * (x2
+00000430: 202a 2028 2d78 3220 2f20 3238 3020 2b20   * (-x2 / 280 + 
+00000440: 302e 3129 202d 2031 2e30 2920 2f20 332e  0.1) - 1.0) / 3.
+00000450: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00000460: 2020 2028 6e70 2e63 6f73 2878 2920 2d20     (np.cos(x) - 
+00000470: 6e70 2e73 696e 6328 7820 2f20 6e70 2e70  np.sinc(x / np.p
+00000480: 6929 2920 2f20 782c 0a20 2020 2020 2020  i)) / x,.       
+00000490: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+000004a0: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
+000004b0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+000004c0: 6f72 2822 4f6e 6c79 2064 3d30 206f 7220  or("Only d=0 or 
+000004d0: 3120 7375 7070 6f72 7465 6420 2867 6f74  1 supported (got
+000004e0: 2064 3d7b 7d29 2e22 2e66 6f72 6d61 7428   d={}).".format(
+000004f0: 6429 290a 0a0a 6465 6620 4a28 6e75 2c20  d))...def J(nu, 
+00000500: 643d 3029 3a0a 2020 2020 7222 2222 5265  d=0):.    r"""Re
+00000510: 7475 726e 2074 6865 2060 6460 2774 6820  turn the `d`'th 
+00000520: 6465 7269 7661 7469 7665 206f 6620 7468  derivative of th
+00000530: 6520 6265 7373 656c 2066 756e 6374 696f  e bessel functio
+00000540: 6e73 0a20 2020 203a 6d61 7468 3a60 4a5f  ns.    :math:`J_
+00000550: 7b5c 6e75 7d28 7a29 602e 0a0a 0a20 2020  {\nu}(z)`....   
+00000560: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
+00000580: 7520 3a20 666c 6f61 740a 2020 2020 2020  u : float.      
+00000590: 204f 7264 6572 2e0a 2020 2020 6420 3a20   Order..    d : 
+000005a0: 696e 740a 2020 2020 2020 2043 6f6d 7075  int.       Compu
+000005b0: 7465 2074 6865 2060 6460 2774 6820 6465  te the `d`'th de
+000005c0: 7269 7661 7469 7665 2e0a 0a20 2020 2045  rivative...    E
+000005d0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+000005e0: 2d2d 2d2d 0a20 2020 203e 3e3e 204a 3020  ----.    >>> J0 
+000005f0: 3d20 4a28 302e 3529 3b20 4a31 203d 204a  = J(0.5); J1 = J
+00000600: 2831 2e35 293b 204a 3220 3d20 4a28 322e  (1.5); J2 = J(2.
+00000610: 3529 3b0a 2020 2020 3e3e 3e20 7a20 3d20  5);.    >>> z = 
+00000620: 322e 353b 206e 7520 3d20 312e 350a 2020  2.5; nu = 1.5.  
+00000630: 2020 3e3e 3e20 6162 7328 4a30 287a 2920    >>> abs(J0(z) 
+00000640: 2b20 4a32 287a 2920 2d20 322a 6e75 2f7a  + J2(z) - 2*nu/z
+00000650: 2a4a 3128 7a29 2920 3c20 5f45 5053 0a20  *J1(z)) < _EPS. 
+00000660: 2020 2054 7275 650a 0a20 2020 202e 2e20     True..    .. 
+00000670: 746f 646f 3a3a 2046 6978 2074 6f6c 6572  todo:: Fix toler
+00000680: 616e 6365 7320 736f 2074 6861 7420 7468  ances so that th
+00000690: 6573 6520 6172 6520 636f 6d70 7574 6564  ese are computed
+000006a0: 2074 6f20 6d61 6368 696e 6520 7072 6563   to machine prec
+000006b0: 6973 696f 6e2e 0a20 2020 2022 2222 0a20  ision..    """. 
+000006c0: 2020 206e 7532 203d 2032 202a 206e 750a     nu2 = 2 * nu.
+000006d0: 2020 2020 6966 2030 203d 3d20 643a 0a20      if 0 == d:. 
+000006e0: 2020 2020 2020 2069 6620 3120 3d3d 206e         if 1 == n
+000006f0: 7532 3a0a 0a20 2020 2020 2020 2020 2020  u2:..           
+00000700: 2064 6566 206a 287a 293a 0a20 2020 2020   def j(z):.     
+00000710: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000720: 6e20 6e70 2e73 7172 7428 3220 2a20 7a20  n np.sqrt(2 * z 
+00000730: 2f20 7069 2920 2a20 7369 6e63 287a 290a  / pi) * sinc(z).
+00000740: 0a20 2020 2020 2020 2065 6c69 6620 3320  .        elif 3 
+00000750: 3d3d 206e 7532 3a0a 0a20 2020 2020 2020  == nu2:..       
+00000760: 2020 2020 2064 6566 206a 287a 293a 0a20       def j(z):. 
+00000770: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00000780: 6574 7572 6e20 6e70 2e73 7172 7428 3220  eturn np.sqrt(2 
+00000790: 2f20 7a20 2f20 7069 2920 2a20 2873 696e  / z / pi) * (sin
+000007a0: 6328 7a29 202d 206e 702e 636f 7328 7a29  c(z) - np.cos(z)
+000007b0: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+000007c0: 3520 3d3d 206e 7532 3a0a 0a20 2020 2020  5 == nu2:..     
+000007d0: 2020 2020 2020 2064 6566 206a 287a 293a         def j(z):
+000007e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007f0: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
+00000800: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+00000810: 2e73 7172 7428 3220 2f20 7a20 2f20 7069  .sqrt(2 / z / pi
+00000820: 2920 2f20 7a20 2a20 2828 332e 3020 2d20  ) / z * ((3.0 - 
+00000830: 7a20 2a20 7a29 202a 2073 696e 6328 7a29  z * z) * sinc(z)
+00000840: 202d 2033 202a 206e 702e 636f 7328 7a29   - 3 * np.cos(z)
+00000850: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00000860: 2020 290a 0a20 2020 2020 2020 2065 6c69    )..        eli
+00000870: 6620 4661 6c73 653a 2020 2320 7072 6167  f False:  # prag
+00000880: 6d61 3a20 6e6f 2063 6f76 6572 0a0a 2020  ma: no cover..  
+00000890: 2020 2020 2020 2020 2020 6465 6620 6a28            def j(
+000008a0: 7a29 3a0a 2020 2020 2020 2020 2020 2020  z):.            
+000008b0: 2020 2020 7265 7475 726e 2032 202a 2028      return 2 * (
+000008c0: 6e75 202d 2031 2920 2f20 7a20 2a20 4a28  nu - 1) / z * J(
+000008d0: 6e75 202d 2031 2928 7a29 202d 204a 286e  nu - 1)(z) - J(n
+000008e0: 7520 2d20 3229 287a 290a 0a20 2020 2020  u - 2)(z)..     
+000008f0: 2020 2065 6c73 653a 0a0a 2020 2020 2020     else:..      
+00000900: 2020 2020 2020 6465 6620 6a28 7a29 3a0a        def j(z):.
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 7265 7475 726e 2073 702e 7370 6563 6961  return sp.specia
+00000930: 6c2e 6a6e 286e 752c 207a 290a 0a20 2020  l.jn(nu, z)..   
+00000940: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+00000950: 2043 6f6d 7075 7465 2064 6572 6976 6174   Compute derivat
+00000960: 6976 6573 2075 7369 6e67 2072 6563 7572  ives using recur
+00000970: 7265 6e63 6520 7265 6c61 7469 6f6e 732e  rence relations.
+00000980: 2020 4e6f 740a 2020 2020 2020 2020 2320    Not.        # 
+00000990: 6566 6669 6369 656e 7420 666f 7220 6869  efficient for hi
+000009a0: 6768 206f 7264 6572 7321 0a20 2020 2020  gh orders!.     
+000009b0: 2020 2064 6566 206a 287a 293a 0a20 2020     def j(z):.   
+000009c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000009d0: 284a 286e 7520 2d20 312c 2064 202d 2031  (J(nu - 1, d - 1
+000009e0: 2928 7a29 202d 204a 286e 7520 2b20 312c  )(z) - J(nu + 1,
+000009f0: 2064 202d 2031 2928 7a29 2920 2f20 322e   d - 1)(z)) / 2.
+00000a00: 300a 0a20 2020 2072 6574 7572 6e20 6a0a  0..    return j.
+00000a10: 0a0a 6465 6620 6a5f 726f 6f74 5f78 286e  ..def j_root_x(n
+00000a20: 752c 2078 2c20 7265 6c5f 746f 6c3d 3220  u, x, rel_tol=2 
+00000a30: 2a20 5f45 5053 293a 0a20 2020 2072 2222  * _EPS):.    r""
+00000a40: 2252 6574 7572 6e20 7468 6520 726f 6f74  "Return the root
+00000a50: 7320 6f66 2074 6865 2062 6573 7365 6c20  s of the bessel 
+00000a60: 6675 6e63 7469 6f6e 2063 6c6f 7365 7374  function closest
+00000a70: 2074 6f20 6078 6020 666f 756e 640a 2020   to `x` found.  
+00000a80: 2020 6279 2069 7465 7261 7469 6e67 2061    by iterating a
+00000a90: 2076 6572 7369 6f6e 206f 6620 4e65 7774   version of Newt
+00000aa0: 6f6e 2773 206d 6574 686f 642e 0a0a 2020  on's method...  
+00000ab0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000ac0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000ad0: 6e75 203a 2066 6c6f 6174 0a20 2020 2020  nu : float.     
+00000ae0: 2020 4f72 6465 7220 6f66 2062 6573 7365    Order of besse
+00000af0: 6c20 6675 6e63 7469 6f6e 0a20 2020 204e  l function.    N
+00000b00: 203a 2069 6e74 0a20 2020 2020 2020 4e75   : int.       Nu
+00000b10: 6d62 6572 206f 6620 726f 6f74 730a 2020  mber of roots.  
+00000b20: 2020 7265 6c5f 746f 6c20 3a20 666c 6f61    rel_tol : floa
+00000b30: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+00000b40: 2020 2044 6573 6972 6564 2072 656c 6174     Desired relat
+00000b50: 6976 6520 746f 6c65 7261 6e63 6520 666f  ive tolerance fo
+00000b60: 7220 726f 6f74 732e 0a20 2020 2022 2222  r roots..    """
+00000b70: 0a20 2020 2069 6620 5472 7565 3a0a 2020  .    if True:.  
+00000b80: 2020 2020 2020 2320 416c 676f 7269 7468        # Algorith
+00000b90: 6d20 6672 6f6d 0a20 2020 2020 2020 2023  m from.        #
+00000ba0: 204e 756d 6572 6963 616c 2041 6c67 6f72   Numerical Algor
+00000bb0: 6974 686d 7320 3138 2028 3139 3938 2920  ithms 18 (1998) 
+00000bc0: 3235 392d 3237 360a 2020 2020 2020 2020  259-276.        
+00000bd0: 6f6c 645f 6572 7220 3d20 3130 0a20 2020  old_err = 10.   
+00000be0: 2020 2020 2065 7272 203d 2031 0a20 2020       err = 1.   
+00000bf0: 2020 2020 206e 5f69 7465 7220 3d20 300a       n_iter = 0.
+00000c00: 2020 2020 2020 2020 7768 696c 6520 6e70          while np
+00000c10: 2e61 6e79 2878 203e 206e 7529 2061 6e64  .any(x > nu) and
+00000c20: 2065 7272 203e 2072 656c 5f74 6f6c 3a0a   err > rel_tol:.
+00000c30: 2020 2020 2020 2020 2020 2020 6e5f 6974              n_it
+00000c40: 6572 202b 3d20 310a 2020 2020 2020 2020  er += 1.        
+00000c50: 2020 2020 6820 3d20 4a28 6e75 3d6e 7529      h = J(nu=nu)
+00000c60: 2878 2920 2f20 4a28 6e75 3d6e 7520 2d20  (x) / J(nu=nu - 
+00000c70: 3129 2878 290a 2020 2020 2020 2020 2020  1)(x).          
+00000c80: 2020 6820 3d20 6e70 2e77 6865 7265 286e    h = np.where(n
+00000c90: 702e 6162 7328 6829 203e 2031 2c20 6e70  p.abs(h) > 1, np
+00000ca0: 2e73 6967 6e28 6829 2c20 6829 0a20 2020  .sign(h), h).   
+00000cb0: 2020 2020 2020 2020 2078 5f61 203d 2078           x_a = x
+00000cc0: 0a20 2020 2020 2020 2020 2020 2078 203d  .            x =
+00000cd0: 2078 202d 2068 202f 2028 3120 2b20 6820   x - h / (1 + h 
+00000ce0: 2a20 6829 0a20 2020 2020 2020 2020 2020  * h).           
+00000cf0: 2078 203d 206e 702e 7768 6572 6528 7820   x = np.where(x 
+00000d00: 3c20 302c 2078 5f61 202f 2032 2c20 7829  < 0, x_a / 2, x)
+00000d10: 0a20 2020 2020 2020 2020 2020 206f 6c64  .            old
+00000d20: 5f65 7272 203d 2065 7272 0a20 2020 2020  _err = err.     
+00000d30: 2020 2020 2020 2065 7272 203d 206e 702e         err = np.
+00000d40: 6d61 7828 6e70 2e61 6273 2868 202f 2078  max(np.abs(h / x
+00000d50: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+00000d60: 6620 6572 7220 3e3d 206f 6c64 5f65 7272  f err >= old_err
+00000d70: 2061 6e64 206e 5f69 7465 7220 3e20 3230   and n_iter > 20
+00000d80: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00000d90: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00000da0: 2020 2020 2020 7761 726e 280a 2020 2020        warn(.    
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 226a 5f72 6f6f 743a 2074 6572 6d69 6e61  "j_root: termina
+00000dd0: 7469 6e67 2069 7465 7261 7469 6f6e 2077  ting iteration w
+00000de0: 6974 6820 6572 726f 7220 220a 2020 2020  ith error ".    
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 2b20 2225 6720 3c20 2567 206c 6573 7320  + "%g < %g less 
+00000e10: 7468 6174 2073 7065 6369 6669 6564 2072  that specified r
+00000e20: 656c 5f74 6f6c 2220 2520 2865 7272 2c20  el_tol" % (err, 
+00000e30: 7265 6c5f 746f 6c29 0a20 2020 2020 2020  rel_tol).       
+00000e40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00000e50: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00000e60: 0a20 2020 2020 2020 2078 203d 206e 702e  .        x = np.
+00000e70: 7768 6572 6528 7820 3c20 6e75 2c20 302c  where(x < nu, 0,
+00000e80: 2078 290a 2020 2020 656c 7365 3a20 2023   x).    else:  #
+00000e90: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+00000ea0: 720a 2020 2020 2020 2020 2320 5374 616e  r.        # Stan
+00000eb0: 6461 7264 204e 6577 746f 6e27 7320 6d65  dard Newton's me
+00000ec0: 7468 6f64 0a20 2020 2020 2020 2064 6566  thod.        def
+00000ed0: 206e 6577 746f 6e28 7829 3a0a 2020 2020   newton(x):.    
+00000ee0: 2020 2020 2020 2020 7265 7475 726e 2078          return x
+00000ef0: 202d 204a 2878 2920 2f20 4a28 782c 206e   - J(x) / J(x, n
+00000f00: 753d 3129 0a0a 2020 2020 2020 2020 7830  u=1)..        x0
+00000f10: 203d 2078 0a20 2020 2020 2020 2078 203d   = x.        x =
+00000f20: 206e 6577 746f 6e28 7830 290a 2020 2020   newton(x0).    
+00000f30: 2020 2020 7768 696c 6520 6e70 2e6d 6178      while np.max
+00000f40: 2861 6273 2828 7820 2d20 7830 2920 2f20  (abs((x - x0) / 
+00000f50: 7829 2920 3e20 7265 6c5f 746f 6c3a 0a20  x)) > rel_tol:. 
+00000f60: 2020 2020 2020 2020 2020 2078 3020 3d20             x0 = 
+00000f70: 780a 2020 2020 2020 2020 2020 2020 7820  x.            x 
+00000f80: 3d20 6e65 7774 6f6e 2878 3029 0a0a 2020  = newton(x0)..  
+00000f90: 2020 7265 7475 726e 2078 0a0a 0a64 6566    return x...def
+00000fa0: 206a 5f72 6f6f 7428 6e75 2c20 4e2c 2072   j_root(nu, N, r
+00000fb0: 656c 5f74 6f6c 3d32 202a 205f 4550 5329  el_tol=2 * _EPS)
+00000fc0: 3a0a 2020 2020 7222 2222 5265 7475 726e  :.    r"""Return
+00000fd0: 2074 6865 2066 6972 7374 204e 2070 6f73   the first N pos
+00000fe0: 6974 6976 6520 726f 6f74 7320 6f66 2074  itive roots of t
+00000ff0: 6865 2062 6573 7365 6c20 6675 6e63 7469  he bessel functi
+00001000: 6f6e 0a20 2020 2060 4a5f 6e75 2878 2960  on.    `J_nu(x)`
+00001010: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+00001020: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00001030: 0a20 2020 206e 7520 3a20 666c 6f61 740a  .    nu : float.
+00001040: 2020 2020 2020 204f 7264 6572 206f 6620         Order of 
+00001050: 6265 7373 656c 2066 756e 6374 696f 6e0a  bessel function.
+00001060: 2020 2020 4e20 3a20 696e 740a 2020 2020      N : int.    
+00001070: 2020 204e 756d 6265 7220 6f66 2072 6f6f     Number of roo
+00001080: 7473 0a20 2020 2072 656c 5f74 6f6c 203a  ts.    rel_tol :
+00001090: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+000010a0: 0a20 2020 2020 2020 4465 7369 7265 6420  .       Desired 
+000010b0: 7265 6c61 7469 7665 2074 6f6c 6572 616e  relative toleran
+000010c0: 6365 2066 6f72 2072 6f6f 7473 2e0a 0a20  ce for roots... 
+000010d0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+000010e0: 2d2d 0a20 2020 2054 6865 2067 656e 6572  --.    The gener
+000010f0: 616c 206d 6574 686f 6420 6973 2074 6f20  al method is to 
+00001100: 6669 7273 7420 6573 7469 6d61 7465 2074  first estimate t
+00001110: 6865 2072 6f6f 7473 2077 6974 6820 610a  he roots with a.
+00001120: 2020 2020 6269 7365 6374 696f 6e2f 7365      bisection/se
+00001130: 6361 6e74 206d 6574 686f 642c 2061 6e64  cant method, and
+00001140: 2074 6865 6e20 706f 6c69 7368 2074 6865   then polish the
+00001150: 6d20 7573 696e 6720 4e65 7774 6f6e 2773  m using Newton's
+00001160: 0a20 2020 206d 6574 686f 642e 0a0a 2020  .    method...  
+00001170: 2020 5765 2073 7461 7274 2062 7920 6573    We start by es
+00001180: 7469 6d61 7469 6e67 2074 6865 206c 6f77  timating the low
+00001190: 6572 2062 6f75 6e64 2066 6f72 2074 6865  er bound for the
+000011a0: 2066 6972 7374 2066 6f72 0a20 2020 206e   first for.    n
+000011b0: 6f6e 2d6e 6567 6174 6976 6520 3a6d 6174  on-negative :mat
+000011c0: 683a 605c 6e75 600a 0a20 2020 202e 2e20  h:`\nu`..    .. 
+000011d0: 6d61 7468 3a3a 0a20 2020 2020 2020 5c6e  math::.       \n
+000011e0: 7520 2b20 5c6e 755e 7b31 2f33 7d20 3c20  u + \nu^{1/3} < 
+000011f0: 6a5f 7b5c 6e75 2c31 7d20 3c20 5c6e 7520  j_{\nu,1} < \nu 
+00001200: 2b20 312e 3835 3537 3520 5c6e 755e 7b31  + 1.85575 \nu^{1
+00001210: 2f33 7d20 2b20 5c70 690a 0a20 2020 2054  /3} + \pi..    T
+00001220: 6865 6e2c 2075 7369 6e67 2074 6865 2066  hen, using the f
+00001230: 6163 7420 7468 6174 2074 6865 2072 6f6f  act that the roo
+00001240: 7473 2061 7265 2073 7061 6365 6420 6279  ts are spaced by
+00001250: 2061 7420 6c65 6173 740a 2020 2020 3a6d   at least.    :m
+00001260: 6174 683a 605c 7069 602c 2077 6520 7374  ath:`\pi`, we st
+00001270: 6570 2074 6872 6f75 6768 2074 6865 2073  ep through the s
+00001280: 6967 6e20 6368 616e 6765 7320 746f 2062  ign changes to b
+00001290: 7261 636b 6574 2061 6c6c 206f 660a 2020  racket all of.  
+000012a0: 2020 7468 6520 6465 7369 7265 6420 726f    the desired ro
+000012b0: 6f74 732e 0a0a 2020 2020 6c6f 7765 7374  ots...    lowest
+000012c0: 2072 6f6f 7420 7573 696e 6720 7468 6520   root using the 
+000012d0: 666f 6c6c 6f77 696e 670a 2020 2020 6865  following.    he
+000012e0: 7572 6973 7469 6373 0a0a 2020 2020 2e2e  uristics..    ..
+000012f0: 206d 6174 683a 3a0a 2020 2020 2020 206a   math::.       j
+00001300: 5f7b 5c6e 752c 737d 205c 6170 7072 6f78  _{\nu,s} \approx
+00001310: 205c 6265 6769 6e7b 6361 7365 737d 0a20   \begin{cases}. 
+00001320: 2020 2020 2020 2020 2032 5c73 7172 747b           2\sqrt{
+00001330: 5c6e 7520 2b20 317d 0a20 2020 2020 2020  \nu + 1}.       
+00001340: 2020 2020 2020 2620 2d31 203c 205c 6e75        & -1 < \nu
+00001350: 203c 202d 302e 385c 5c0a 2020 2020 2020   < -0.8\\.      
+00001360: 2020 2020 5c6c 6566 7428 5c66 7261 637b      \left(\frac{
+00001370: 5c6e 757d 7b32 7d20 2b20 5c66 7261 637b  \nu}{2} + \frac{
+00001380: 337d 7b34 7d5c 7269 6768 7429 5c70 690a  3}{4}\right)\pi.
+00001390: 2020 2020 2020 2020 2020 2020 2026 202d               & -
+000013a0: 302e 3820 3c20 5c6e 7520 3c20 322e 355c  0.8 < \nu < 2.5\
+000013b0: 5c0a 2020 2020 2020 2020 2020 5c6e 7520  \.          \nu 
+000013c0: 2b20 312e 3835 3537 3520 5c6e 755e 7b31  + 1.85575 \nu^{1
+000013d0: 2f33 7d0a 2020 2020 2020 2020 2020 2020  /3}.            
+000013e0: 2026 2032 2e35 205c 6c65 7120 5c6e 750a   & 2.5 \leq \nu.
+000013f0: 2020 2020 2020 205c 656e 647b 6361 7365         \end{case
+00001400: 737d 0a0a 2020 2020 4578 616d 706c 6573  s}..    Examples
+00001410: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
+00001420: 2020 3e3e 3e20 6e75 203d 2032 2e35 0a20    >>> nu = 2.5. 
+00001430: 2020 203e 3e3e 206a 5f20 3d20 6a5f 726f     >>> j_ = j_ro
+00001440: 6f74 286e 752c 2032 3030 3029 0a20 2020  ot(nu, 2000).   
+00001450: 203e 3e3e 204a 5f20 3d20 4a28 6e75 2928   >>> J_ = J(nu)(
+00001460: 6a5f 290a 0a20 2020 2054 6865 7365 2061  j_)..    These a
+00001470: 7265 2072 6f6f 7473 210a 0a20 2020 203e  re roots!..    >
+00001480: 3e3e 206e 702e 6d61 7828 6162 7328 4a5f  >> np.max(abs(J_
+00001490: 2f6a 5f29 2920 3c20 5f45 5053 0a20 2020  /j_)) < _EPS.   
+000014a0: 2054 7275 650a 0a20 2020 2054 6865 7920   True..    They 
+000014b0: 6172 6520 616c 736f 2064 6973 7469 6e63  are also distinc
+000014c0: 740a 0a20 2020 203e 3e3e 2070 6920 3c20  t..    >>> pi < 
+000014d0: 6d69 6e28 6e70 2e64 6966 6628 6a5f 2929  min(np.diff(j_))
+000014e0: 0a20 2020 2054 7275 650a 0a20 2020 2041  .    True..    A
+000014f0: 6e64 2074 6865 2073 7061 6369 6e67 2069  nd the spacing i
+00001500: 7320 6465 6372 6561 7369 6e67 2c20 6d65  s decreasing, me
+00001510: 616e 696e 6720 7765 2068 6176 6520 6e6f  aning we have no
+00001520: 7420 736b 6970 7065 6420 616e 792e 0a0a  t skipped any...
+00001530: 2020 2020 3e3e 3e20 6e70 2e6d 6178 286e      >>> np.max(n
+00001540: 702e 6469 6666 286e 702e 6469 6666 286a  p.diff(np.diff(j
+00001550: 5f29 2929 203c 2030 0a20 2020 2054 7275  _))) < 0.    Tru
+00001560: 650a 2020 2020 2222 220a 2020 2020 4a5f  e.    """.    J_
+00001570: 203d 204a 286e 7529 0a0a 2020 2020 6e75   = J(nu)..    nu
+00001580: 3220 3d20 3220 2a20 6e75 0a0a 2020 2020  2 = 2 * nu..    
+00001590: 6966 206e 7532 203c 2030 3a0a 2020 2020  if nu2 < 0:.    
+000015a0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000015b0: 7272 6f72 2822 6e75 206d 7573 7420 6265  rror("nu must be
+000015c0: 206e 6f6e 2d6e 6567 6174 6976 6522 290a   non-negative").
+000015d0: 2020 2020 656c 6966 2031 203d 3d20 6e75      elif 1 == nu
+000015e0: 323a 0a20 2020 2020 2020 2023 2052 6f6f  2:.        # Roo
+000015f0: 7473 206f 6620 7369 6e28 7829 2f78 203d  ts of sin(x)/x =
+00001600: 2030 3a0a 2020 2020 2020 2020 2320 7820   0:.        # x 
+00001610: 3d20 7069 2a6e 2065 7863 6c75 6469 6e67  = pi*n excluding
+00001620: 206e 3d30 0a20 2020 2020 2020 2072 6574   n=0.        ret
+00001630: 7572 6e20 7069 202a 206e 702e 6172 616e  urn pi * np.aran
+00001640: 6765 2831 2c20 4e20 2b20 3129 0a20 2020  ge(1, N + 1).   
+00001650: 2065 6c69 6620 3320 3d3d 206e 7532 3a0a   elif 3 == nu2:.
+00001660: 2020 2020 2020 2020 2320 526f 6f74 7320          # Roots 
+00001670: 6f66 2073 696e 2878 292f 782a 2a32 202d  of sin(x)/x**2 -
+00001680: 2063 6f73 2878 292f 783a 0a20 2020 2020   cos(x)/x:.     
+00001690: 2020 2023 2078 203d 2074 616e 2878 2920     # x = tan(x) 
+000016a0: 6578 636c 7564 696e 6720 7820 3d20 300a  excluding x = 0.
+000016b0: 2020 2020 2020 2020 2320 4966 206e 203e          # If n >
+000016c0: 2031 3020 6974 6572 6174 6520 7820 3a2d   10 iterate x :-
+000016d0: 3e20 6e2a 7069 202b 2061 7263 7461 6e28  > n*pi + arctan(
+000016e0: 7829 0a20 2020 2020 2020 2023 2035 2074  x).        # 5 t
+000016f0: 696d 6573 2073 7461 7274 696e 6720 7769  imes starting wi
+00001700: 7468 2078 203d 2070 692a 286e 2b30 2e35  th x = pi*(n+0.5
+00001710: 290a 2020 2020 2020 2020 7820 3d20 6e70  ).        x = np
+00001720: 2e61 7272 6179 280a 2020 2020 2020 2020  .array(.        
+00001730: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00001740: 2020 2020 2020 342e 3439 3334 3039 3435        4.49340945
+00001750: 3739 3039 3036 3432 2c0a 2020 2020 2020  79090642,.      
+00001760: 2020 2020 2020 2020 2020 372e 3732 3532            7.7252
+00001770: 3531 3833 3639 3337 3730 3638 2c0a 2020  518369377068,.  
+00001780: 2020 2020 2020 2020 2020 2020 2020 3130                10
+00001790: 2e39 3034 3132 3136 3539 3432 3838 3939  .904121659428899
+000017a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000017b0: 2020 3134 2e30 3636 3139 3339 3132 3833    14.06619391283
+000017c0: 3134 3733 2c0a 2020 2020 2020 2020 2020  1473,.          
+000017d0: 2020 2020 2020 3137 2e32 3230 3735 3532        17.2207552
+000017e0: 3731 3933 3037 3730 2c0a 2020 2020 2020  71930770,.      
+000017f0: 2020 2020 2020 2020 2020 3230 2e33 3731            20.371
+00001800: 3330 3239 3539 3238 3735 3631 2c0a 2020  302959287561,.  
+00001810: 2020 2020 2020 2020 2020 2020 2020 3233                23
+00001820: 2e35 3139 3435 3234 3938 3638 3930 3036  .519452498689006
+00001830: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001840: 2020 3236 2e36 3636 3035 3432 3538 3831    26.66605425881
+00001850: 3236 3732 2c0a 2020 2020 2020 2020 2020  2672,.          
+00001860: 2020 2020 2020 3239 2e38 3131 3539 3837        29.8115987
+00001870: 3930 3839 3239 3538 2c0a 2020 2020 2020  90892958,.      
+00001880: 2020 2020 2020 2020 2020 3332 2e39 3536            32.956
+00001890: 3338 3930 3339 3832 3234 3736 2c0a 2020  389039822476,.  
+000018a0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+000018b0: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+000018c0: 204e 203e 2031 303a 0a20 2020 2020 2020   N > 10:.       
+000018d0: 2020 2020 206e 203d 206e 702e 6172 616e       n = np.aran
+000018e0: 6765 2831 312c 204e 202b 2031 290a 2020  ge(11, N + 1).  
+000018f0: 2020 2020 2020 2020 2020 6e70 6920 3d20            npi = 
+00001900: 6e20 2a20 7069 0a20 2020 2020 2020 2020  n * pi.         
+00001910: 2020 2078 3020 3d20 286e 202b 2030 2e35     x0 = (n + 0.5
+00001920: 2920 2a20 7069 0a20 2020 2020 2020 2020  ) * pi.         
+00001930: 2020 2066 6f72 2063 2069 6e20 7261 6e67     for c in rang
+00001940: 6528 3529 3a0a 2020 2020 2020 2020 2020  e(5):.          
+00001950: 2020 2020 2020 6e70 2e61 7263 7461 6e28        np.arctan(
+00001960: 7830 2c20 7830 290a 2020 2020 2020 2020  x0, x0).        
+00001970: 2020 2020 2020 2020 7830 202b 3d20 6e70          x0 += np
+00001980: 690a 2020 2020 2020 2020 2020 2020 7265  i.            re
+00001990: 7475 726e 206e 702e 6873 7461 636b 2828  turn np.hstack((
+000019a0: 782c 2078 3029 290a 2020 2020 2020 2020  x, x0)).        
+000019b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000019c0: 2020 7265 7475 726e 2078 5b3a 4e5d 0a20    return x[:N]. 
+000019d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000019e0: 2023 2046 696e 6420 6272 6163 6b65 7473   # Find brackets
+000019f0: 2e0a 2020 2020 2020 2020 7820 3d20 6e70  ..        x = np
+00001a00: 2e65 6d70 7479 284e 202b 2031 2c20 6474  .empty(N + 1, dt
+00001a10: 7970 653d 666c 6f61 7429 0a20 2020 2020  ype=float).     
+00001a20: 2020 204a 7820 3d20 6e70 2e65 6d70 7479     Jx = np.empty
+00001a30: 284e 202b 2031 2c20 6474 7970 653d 666c  (N + 1, dtype=fl
+00001a40: 6f61 7429 0a0a 2020 2020 2020 2020 785b  oat)..        x[
+00001a50: 305d 203d 206e 7520 2b20 6e75 202a 2a20  0] = nu + nu ** 
+00001a60: 2831 2e30 202f 2033 2e30 290a 2020 2020  (1.0 / 3.0).    
+00001a70: 2020 2020 4a78 5b30 5d20 3d20 4a5f 2878      Jx[0] = J_(x
+00001a80: 5b30 5d29 0a20 2020 2020 2020 2066 6f72  [0]).        for
+00001a90: 206e 2069 6e20 7261 6e67 6528 312c 204e   n in range(1, N
+00001aa0: 202b 2031 293a 0a20 2020 2020 2020 2020   + 1):.         
+00001ab0: 2020 2078 5b6e 5d20 3d20 785b 6e20 2d20     x[n] = x[n - 
+00001ac0: 315d 202b 2070 690a 2020 2020 2020 2020  1] + pi.        
+00001ad0: 2020 2020 4a78 5b6e 5d20 3d20 4a5f 2878      Jx[n] = J_(x
+00001ae0: 5b6e 5d29 0a20 2020 2020 2020 2020 2020  [n]).           
+00001af0: 2077 6869 6c65 204a 785b 6e5d 202a 204a   while Jx[n] * J
+00001b00: 785b 6e20 2d20 315d 203e 2030 3a0a 2020  x[n - 1] > 0:.  
+00001b10: 2020 2020 2020 2020 2020 2020 2020 785b                x[
+00001b20: 6e5d 202b 3d20 7069 0a20 2020 2020 2020  n] += pi.       
+00001b30: 2020 2020 2020 2020 204a 785b 6e5d 203d           Jx[n] =
+00001b40: 204a 5f28 785b 6e5d 290a 0a20 2020 2020   J_(x[n])..     
+00001b50: 2020 2023 2054 776f 2073 7465 7073 206f     # Two steps o
+00001b60: 6620 6269 7365 6374 696f 6e20 6d65 7468  f bisection meth
+00001b70: 6f64 0a20 2020 2020 2020 2078 3020 3d20  od.        x0 = 
+00001b80: 785b 3a2d 315d 0a20 2020 2020 2020 2078  x[:-1].        x
+00001b90: 3120 3d20 785b 313a 5d0a 2020 2020 2020  1 = x[1:].      
+00001ba0: 2020 4a30 203d 204a 785b 3a2d 315d 0a20    J0 = Jx[:-1]. 
+00001bb0: 2020 2020 2020 204a 3120 3d20 4a78 5b31         J1 = Jx[1
+00001bc0: 3a5d 0a20 2020 2020 2020 2066 6f72 206e  :].        for n
+00001bd0: 2069 6e20 7261 6e67 6528 3229 3a0a 2020   in range(2):.  
+00001be0: 2020 2020 2020 2020 2020 2320 496e 7661            # Inva
+00001bf0: 7269 616e 743a 0a20 2020 2020 2020 2020  riant:.         
+00001c00: 2020 2023 204a 302a 4a31 203c 2030 206f     # J0*J1 < 0 o
+00001c10: 7220 4a30 203d 204a 3120 3d20 3020 616e  r J0 = J1 = 0 an
+00001c20: 6420 7830 203d 2078 310a 2020 2020 2020  d x0 = x1.      
+00001c30: 2020 2020 2020 785f 6d69 6420 3d20 2878        x_mid = (x
+00001c40: 3020 2b20 7831 2920 2f20 320a 2020 2020  0 + x1) / 2.    
+00001c50: 2020 2020 2020 2020 4a5f 6d69 6420 3d20          J_mid = 
+00001c60: 4a5f 2878 5f6d 6964 290a 2020 2020 2020  J_(x_mid).      
+00001c70: 2020 2020 2020 7330 203d 204a 5f6d 6964        s0 = J_mid
+00001c80: 202a 204a 300a 2020 2020 2020 2020 2020   * J0.          
+00001c90: 2020 7331 203d 204a 5f6d 6964 202a 204a    s1 = J_mid * J
+00001ca0: 310a 2020 2020 2020 2020 2020 2020 6173  1.            as
+00001cb0: 7365 7274 206e 702e 616c 6c28 7330 202a  sert np.all(s0 *
+00001cc0: 2073 3120 3c3d 2030 290a 2020 2020 2020   s1 <= 0).      
+00001cd0: 2020 2020 2020 7830 203d 206e 702e 7768        x0 = np.wh
+00001ce0: 6572 6528 7330 203e 3d20 302c 2078 5f6d  ere(s0 >= 0, x_m
+00001cf0: 6964 2c20 7830 290a 2020 2020 2020 2020  id, x0).        
+00001d00: 2020 2020 7831 203d 206e 702e 7768 6572      x1 = np.wher
+00001d10: 6528 7331 203e 3d20 302c 2078 5f6d 6964  e(s1 >= 0, x_mid
+00001d20: 2c20 7831 290a 2020 2020 2020 2020 2020  , x1).          
+00001d30: 2020 4a30 203d 206e 702e 7768 6572 6528    J0 = np.where(
+00001d40: 7330 203e 3d20 302c 204a 5f6d 6964 2c20  s0 >= 0, J_mid, 
+00001d50: 4a30 290a 2020 2020 2020 2020 2020 2020  J0).            
+00001d60: 4a31 203d 206e 702e 7768 6572 6528 7331  J1 = np.where(s1
+00001d70: 203e 3d20 302c 204a 5f6d 6964 2c20 4a31   >= 0, J_mid, J1
+00001d80: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00001d90: 7330 2c20 7331 203e 2030 206f 7220 7330  s0, s1 > 0 or s0
+00001da0: 202c 2073 3120 3c20 303a 2043 616e 2774   , s1 < 0: Can't
+00001db0: 2068 6170 7065 6e0a 2020 2020 2020 2020   happen.        
+00001dc0: 2020 2020 2320 7330 203c 2030 2c20 7331      # s0 < 0, s1
+00001dd0: 203e 3d20 303a 204a 302a 4a31 203d 204a   >= 0: J0*J1 = J
+00001de0: 302a 4a5f 6d69 6420 3d20 7330 203c 2030  0*J_mid = s0 < 0
+00001df0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00001e00: 3020 3e3d 2030 2c20 7331 203c 2030 3a20  0 >= 0, s1 < 0: 
+00001e10: 4a30 2a4a 3120 3d20 4a5f 6d69 642a 4a31  J0*J1 = J_mid*J1
+00001e20: 203d 2073 3120 3c3d 2030 0a20 2020 2020   = s1 <= 0.     
+00001e30: 2020 2020 2020 2023 2073 3020 3d20 7331         # s0 = s1
+00001e40: 203d 2030 3a20 7830 203d 2078 3120 3d20   = 0: x0 = x1 = 
+00001e50: 785f 6d69 6420 616e 6420 4a5f 6d69 6420  x_mid and J_mid 
+00001e60: 3d20 300a 0a20 2020 2020 2020 2023 204e  = 0..        # N
+00001e70: 6f77 2066 6f72 6d20 6775 6573 7320 7573  ow form guess us
+00001e80: 696e 6720 7365 6361 6e74 206d 6574 686f  ing secant metho
+00001e90: 642e 0a20 2020 2020 2020 2078 203d 2028  d..        x = (
+00001ea0: 4a31 202a 2078 3020 2d20 4a30 202a 2078  J1 * x0 - J0 * x
+00001eb0: 3129 202f 2028 4a31 202d 204a 3029 0a20  1) / (J1 - J0). 
+00001ec0: 2020 2020 2020 2072 6574 7572 6e20 6a5f         return j_
+00001ed0: 726f 6f74 5f78 286e 753d 6e75 2c20 783d  root_x(nu=nu, x=
+00001ee0: 782c 2072 656c 5f74 6f6c 3d72 656c 5f74  x, rel_tol=rel_t
+00001ef0: 6f6c 290a 0a0a 6465 6620 4a5f 7371 7274  ol)...def J_sqrt
+00001f00: 5f70 6f6c 6528 6e75 2c20 7a6e 2c20 643d  _pole(nu, zn, d=
+00001f10: 3029 3a0a 2020 2020 7222 2222 5265 7475  0):.    r"""Retu
+00001f20: 726e 2061 2066 756e 6374 696f 6e20 7468  rn a function th
+00001f30: 6174 2063 6f6d 7075 7465 7320 7468 6520  at computes the 
+00001f40: 6064 6027 7468 2064 6572 6976 6174 6976  `d`'th derivativ
+00001f50: 6520 6f66 0a20 2020 2060 7371 7274 287a  e of.    `sqrt(z
+00001f60: 292a 4a28 6e75 2c7a 292f 287a 202d 207a  )*J(nu,z)/(z - z
+00001f70: 6e29 6020 7768 6572 6520 607a 6e60 2069  n)` where `zn` i
+00001f80: 7320 6120 726f 6f74 3a20 604a 286e 752c  s a root: `J(nu,
+00001f90: 207a 6e29 203d 2030 602e 0a20 2020 2054   zn) = 0`..    T
+00001fa0: 6869 7320 636f 6d62 696e 6174 696f 6e20  his combination 
+00001fb0: 6170 7065 6172 7320 696e 2074 6865 2042  appears in the B
+00001fc0: 6573 7365 6c20 6675 6e63 7469 6f6e 2044  essel function D
+00001fd0: 5652 2062 6173 6973 2e0a 0a20 2020 2050  VR basis...    P
+00001fe0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00001ff0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 7520  --------.    nu 
+00002000: 3a20 666c 6f61 740a 2020 2020 2020 204f  : float.       O
+00002010: 7264 6572 0a20 2020 207a 6e20 3a20 666c  rder.    zn : fl
+00002020: 6f61 740a 2020 2020 2020 2052 6f6f 7420  oat.       Root 
+00002030: 6f66 2060 4a28 6e75 2c20 7a29 600a 2020  of `J(nu, z)`.  
+00002040: 2020 6420 3a20 696e 740a 2020 2020 2020    d : int.      
+00002050: 204f 7264 6572 206f 6620 6465 7269 7661   Order of deriva
+00002060: 7469 7665 2074 6f20 7461 6b65 2e0a 0a20  tive to take... 
+00002070: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+00002080: 2d2d 0a20 2020 202e 2e20 6d61 7468 3a3a  --.    .. math::
+00002090: 0a20 2020 2020 2020 5c66 7261 637b 5c73  .       \frac{\s
+000020a0: 7172 747b 7a7d 4a5f 7b5c 6e75 7d28 7a29  qrt{z}J_{\nu}(z)
+000020b0: 7d7b 7a20 2d20 7a5f 7b6e 7d7d 0a0a 2020  }{z - z_{n}}..  
+000020c0: 2020 4173 203a 6d61 7468 3a60 7a60 2061    As :math:`z` a
+000020d0: 7070 726f 6163 6865 7320 3a6d 6174 683a  pproaches :math:
+000020e0: 607a 5f6e 602c 2074 6869 7320 6861 7320  `z_n`, this has 
+000020f0: 7468 6520 666f 726d 206f 6620 6030 2f30  the form of `0/0
+00002100: 602c 0a20 2020 2073 6f20 6f6e 6520 6361  `,.    so one ca
+00002110: 6e20 6170 706c 7920 6120 666f 726d 206f  n apply a form o
+00002120: 6620 6c27 486f 7069 7461 6c27 7320 7275  f l'Hopital's ru
+00002130: 6c65 2074 6f20 7265 6475 6365 2074 6865  le to reduce the
+00002140: 0a20 2020 2072 6f75 6e64 2d6f 6666 2065  .    round-off e
+00002150: 7272 6f72 2e20 2054 6865 2073 7065 6369  rror.  The speci
+00002160: 6669 6564 2066 6f72 6d20 6f66 2074 6865  fied form of the
+00002170: 2066 756e 6374 696f 6e20 6861 7320 6265   function has be
+00002180: 656e 0a20 2020 2063 686f 7365 6e20 666f  en.    chosen fo
+00002190: 7220 7370 6563 6961 6c20 7072 6f70 6572  r special proper
+000021a0: 7469 6573 206f 6620 7468 6520 4265 7373  ties of the Bess
+000021b0: 656c 2066 756e 6374 696f 6e73 2e20 2045  el functions.  E
+000021c0: 7870 7265 7373 0a20 2020 2074 6865 2066  xpress.    the f
+000021d0: 756e 6374 696f 6e20 6173 0a0a 2020 2020  unction as..    
+000021e0: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
+000021f0: 2046 287a 2920 263d 205c 6672 6163 7b66   F(z) &= \frac{f
+00002200: 287a 297d 7b7a 202d 207a 5f6e 7d20 203d  (z)}{z - z_n}  =
+00002210: 205c 6672 6163 7b5c 7371 7274 7b7a 7d4a   \frac{\sqrt{z}J
+00002220: 5f7b 5c6e 757d 287a 297d 7b7a 202d 207a  _{\nu}(z)}{z - z
+00002230: 5f6e 7d5c 5c0a 2020 2020 2020 2046 2728  _n}\\.       F'(
+00002240: 7a29 2026 3d20 5c66 7261 637b 6627 287a  z) &= \frac{f'(z
+00002250: 297d 7b7a 202d 207a 5f6e 7d20 2d20 5c66  )}{z - z_n} - \f
+00002260: 7261 637b 6628 7a29 7d7b 287a 202d 207a  rac{f(z)}{(z - z
+00002270: 5f6e 295e 327d 0a0a 0a20 2020 204c 6574  _n)^2}...    Let
+00002280: 203a 6d61 7468 3a60 5c64 656c 7461 203d   :math:`\delta =
+00002290: 207a 202d 207a 5f6e 602e 2020 436c 6f73   z - z_n`.  Clos
+000022a0: 6520 746f 2074 6865 2073 696e 6775 6c61  e to the singula
+000022b0: 7220 706f 696e 7420 7765 2075 7365 0a20  r point we use. 
+000022c0: 2020 2074 6865 2054 6179 6c6f 7220 7365     the Taylor se
+000022d0: 7269 6573 3a0a 0a20 2020 202e 2e20 6d61  ries:..    .. ma
+000022e0: 7468 3a3a 0a20 2020 2020 2020 5c73 756d  th::.       \sum
+000022f0: 5f7b 6d3d 307d 5e7b 5c69 6e66 7479 7d5c  _{m=0}^{\infty}\
+00002300: 6672 6163 7b61 5f6d 5c64 656c 7461 5e7b  frac{a_m\delta^{
+00002310: 6d7d 7d7b 6d21 7d0a 0a20 2020 202e 2e20  m}}{m!}..    .. 
+00002320: 6d61 7468 3a3a 0a20 2020 2020 2020 4628  math::.       F(
+00002330: 7a29 2026 3d20 6627 287a 5f6e 290a 2020  z) &= f'(z_n).  
+00002340: 2020 2020 2020 2020 2020 2b20 5c73 756d            + \sum
+00002350: 5f7b 6d3d 337d 5e7b 5c69 6e66 7479 7d5c  _{m=3}^{\infty}\
+00002360: 6672 6163 7b66 5e7b 286d 297d 287a 5f6e  frac{f^{(m)}(z_n
+00002370: 295c 6465 6c74 615e 7b6d 2d31 7d7d 7b6d  )\delta^{m-1}}{m
+00002380: 217d 0a20 2020 2020 2020 2020 2020 203d  !}.            =
+00002390: 205c 7375 6d5f 7b6d 3d30 7d5e 7b5c 696e   \sum_{m=0}^{\in
+000023a0: 6674 797d 5c66 7261 637b 665e 7b28 6d2b  fty}\frac{f^{(m+
+000023b0: 3129 7d28 7a5f 6e29 5c64 656c 7461 5e7b  1)}(z_n)\delta^{
+000023c0: 6d7d 7d7b 286d 2b31 296d 217d 5c5c 0a20  m}}{(m+1)m!}\\. 
+000023d0: 2020 2020 2020 2061 5f6d 2026 3d20 5c66         a_m &= \f
+000023e0: 7261 637b 665e 7b28 6d2b 3129 7d7d 7b6d  rac{f^{(m+1)}}{m
+000023f0: 2b31 7d5c 5c0a 2020 2020 2020 2046 2728  +1}\\.       F'(
+00002400: 7a29 2026 3d20 5c73 756d 5f7b 6d3d 337d  z) &= \sum_{m=3}
+00002410: 5e7b 5c69 6e66 7479 7d5c 6672 6163 7b28  ^{\infty}\frac{(
+00002420: 6d2d 3129 665e 7b28 6d29 7d28 7a5f 6e29  m-1)f^{(m)}(z_n)
+00002430: 5c64 656c 7461 5e7b 6d2d 327d 7d7b 6d21  \delta^{m-2}}{m!
+00002440: 7d0a 2020 2020 2020 2020 2020 2020 203d  }.             =
+00002450: 205c 7375 6d5f 7b6d 3d31 7d5e 7b5c 696e   \sum_{m=1}^{\in
+00002460: 6674 797d 5c66 7261 637b 665e 7b28 6d2b  fty}\frac{f^{(m+
+00002470: 3229 7d28 7a5f 6e29 5c64 656c 7461 5e7b  2)}(z_n)\delta^{
+00002480: 6d7d 7d7b 286d 2b32 296d 217d 5c5c 0a20  m}}{(m+2)m!}\\. 
+00002490: 2020 2020 2020 2020 615f 6d20 263d 205c          a_m &= \
+000024a0: 6672 6163 7b66 5e7b 286d 2b32 297d 7d7b  frac{f^{(m+2)}}{
+000024b0: 6d2b 327d 5c5c 0a0a 2020 2020 5468 6520  m+2}\\..    The 
+000024c0: 6669 7273 7420 6665 7720 6465 7269 7661  first few deriva
+000024d0: 7469 7665 7320 6172 6520 7072 6573 656e  tives are presen
+000024e0: 7465 6420 6865 7265 3a0a 0a20 2020 202e  ted here:..    .
+000024f0: 2e20 6d61 7468 3a3a 0a20 2020 2020 2020  . math::.       
+00002500: 6628 7a29 2026 3d20 5c73 7172 747b 7a7d  f(z) &= \sqrt{z}
+00002510: 4a5f 7b5c 6e75 7d28 7a29 5c5c 0a20 2020  J_{\nu}(z)\\.   
+00002520: 2020 2020 6627 287a 2920 263d 205c 6672      f'(z) &= \fr
+00002530: 6163 7b4a 5f7b 5c6e 757d 287a 297d 7b32  ac{J_{\nu}(z)}{2
+00002540: 5c73 7172 747b 7a7d 7d20 2b20 5c73 7172  \sqrt{z}} + \sqr
+00002550: 747b 7a7d 4a27 5f7b 5c6e 757d 287a 290a  t{z}J'_{\nu}(z).
+00002560: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+00002570: 5c66 7261 637b 6628 7a29 7d7b 327a 7d20  \frac{f(z)}{2z} 
+00002580: 2b20 5c73 7172 747b 7a7d 4a27 5f7b 5c6e  + \sqrt{z}J'_{\n
+00002590: 757d 287a 295c 5c0a 2020 2020 2020 2066  u}(z)\\.       f
+000025a0: 2727 287a 2920 263d 205c 7371 7274 7b7a  ''(z) &= \sqrt{z
+000025b0: 7d4a 5f7b 5c6e 757d 287a 295c 6c65 6674  }J_{\nu}(z)\left
+000025c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000025d0: 2020 2020 2020 205c 6672 6163 7b5c 6e75         \frac{\nu
+000025e0: 5e32 202d 205c 7466 7261 637b 317d 7b34  ^2 - \tfrac{1}{4
+000025f0: 7d7d 7b7a 5e32 7d20 2d20 315c 7269 6768  }}{z^2} - 1\righ
+00002600: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00002610: 2020 3d20 6628 7a29 5c6c 6566 7428 5c66    = f(z)\left(\f
+00002620: 7261 637b 5c6e 755e 3220 2d20 5c74 6672  rac{\nu^2 - \tfr
+00002630: 6163 7b31 7d7b 347d 7d7b 7a5e 327d 202d  ac{1}{4}}{z^2} -
+00002640: 2031 5c72 6967 6874 295c 5c0a 2020 2020   1\right)\\.    
+00002650: 2020 2066 2727 2728 7a29 2026 3d20 6627     f'''(z) &= f'
+00002660: 287a 295c 6c65 6674 285c 6672 6163 7b5c  (z)\left(\frac{\
+00002670: 6e75 5e32 202d 205c 7466 7261 637b 317d  nu^2 - \tfrac{1}
+00002680: 7b34 7d7d 7b7a 5e32 7d20 2d20 315c 7269  {4}}{z^2} - 1\ri
+00002690: 6768 7429 0a20 2020 2020 2020 2020 2020  ght).           
+000026a0: 2020 2020 2d20 3266 287a 295c 6672 6163      - 2f(z)\frac
+000026b0: 7b5c 6e75 5e32 202d 205c 7466 7261 637b  {\nu^2 - \tfrac{
+000026c0: 317d 7b34 7d7d 7b7a 5e33 7d5c 5c0a 2020  1}{4}}{z^3}\\.  
+000026d0: 2020 2020 2066 5e7b 2834 297d 287a 2920       f^{(4)}(z) 
+000026e0: 263d 0a20 2020 2020 2020 6628 7a29 5c6c  &=.       f(z)\l
+000026f0: 6566 745b 0a20 2020 2020 2020 2020 205c  eft[.          \
+00002700: 6c65 6674 285c 6672 6163 7b5c 6e75 5e32  left(\frac{\nu^2
+00002710: 202d 205c 7466 7261 637b 317d 7b34 7d7d   - \tfrac{1}{4}}
+00002720: 7b7a 5e32 7d20 2d20 315c 7269 6768 7429  {z^2} - 1\right)
+00002730: 5e32 0a20 2020 2020 2020 2020 202b 2036  ^2.          + 6
+00002740: 5c66 7261 637b 5c6e 755e 3220 2d20 5c74  \frac{\nu^2 - \t
+00002750: 6672 6163 7b31 7d7b 347d 7d7b 7a5e 347d  frac{1}{4}}{z^4}
+00002760: 5c72 6967 6874 5d0a 2020 2020 2020 202d  \right].       -
+00002770: 2034 6627 287a 295c 6672 6163 7b5c 6e75   4f'(z)\frac{\nu
+00002780: 5e32 202d 205c 7466 7261 637b 317d 7b34  ^2 - \tfrac{1}{4
+00002790: 7d7d 7b7a 5e33 7d0a 2020 2020 2e2e 2043  }}{z^3}.    .. C
+000027a0: 6865 636b 6564 2077 6974 6820 4d61 706c  hecked with Mapl
+000027b0: 652e 0a0a 2020 2020 4576 616c 7561 7465  e...    Evaluate
+000027c0: 6420 6174 2074 6865 2072 6f6f 7420 3a6d  d at the root :m
+000027d0: 6174 683a 607a 3d7a 5f6e 6020 7468 6573  ath:`z=z_n` thes
+000027e0: 6520 6265 636f 6d65 3a0a 0a20 2020 202e  e become:..    .
+000027f0: 2e20 6d61 7468 3a3a 0a20 2020 2020 2020  . math::.       
+00002800: 6628 7a5f 7b6e 7d29 2026 3d20 305c 5c0a  f(z_{n}) &= 0\\.
+00002810: 2020 2020 2020 2066 2728 7a5f 7b6e 7d29         f'(z_{n})
+00002820: 2026 3d20 5c73 7172 747b 7a5f 7b6e 7d7d   &= \sqrt{z_{n}}
+00002830: 4a27 5f7b 5c6e 757d 287a 5f7b 6e7d 295c  J'_{\nu}(z_{n})\
+00002840: 5c0a 2020 2020 2020 2066 2727 287a 5f7b  \.       f''(z_{
+00002850: 6e7d 2920 263d 2030 5c5c 0a20 2020 2020  n}) &= 0\\.     
+00002860: 2020 6627 2727 287a 5f7b 6e7d 2920 263d    f'''(z_{n}) &=
+00002870: 2066 2728 7a5f 7b6e 7d29 5c6c 6566 7428   f'(z_{n})\left(
+00002880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002890: 2020 2020 2020 2020 205c 6672 6163 7b5c           \frac{\
+000028a0: 6e75 5e32 202d 205c 7466 7261 637b 317d  nu^2 - \tfrac{1}
+000028b0: 7b34 7d7d 7b7a 5f7b 6e7d 5e32 7d20 2d20  {4}}{z_{n}^2} - 
+000028c0: 315c 7269 6768 7429 5c5c 0a20 2020 2020  1\right)\\.     
+000028d0: 2020 665e 7b28 3429 7d28 7a5f 7b6e 7d29    f^{(4)}(z_{n})
+000028e0: 2026 3d20 2d20 3466 2728 7a5f 7b6e 7d29   &= - 4f'(z_{n})
+000028f0: 5c66 7261 637b 5c6e 755e 3220 2d20 5c74  \frac{\nu^2 - \t
+00002900: 6672 6163 7b31 7d7b 347d 7d7b 7a5f 7b6e  frac{1}{4}}{z_{n
+00002910: 7d5e 337d 0a0a 2020 2020 7769 7468 2062  }^3}..    with b
+00002920: 6f74 6820 7468 6520 6675 6e63 7469 6f6e  oth the function
+00002930: 2061 6e64 2074 6865 2073 6563 6f6e 6420   and the second 
+00002940: 6465 7269 7661 7469 7665 2076 616e 6973  derivative vanis
+00002950: 6869 6e67 2e0a 0a20 2020 2054 6f20 6465  hing...    To de
+00002960: 7465 726d 696e 6520 7768 6572 6520 746f  termine where to
+00002970: 2075 7365 2074 6869 7320 666f 726d 756c   use this formul
+00002980: 612c 2077 6520 6d61 7463 6820 7468 6520  a, we match the 
+00002990: 6573 7469 6d61 7465 0a20 2020 2072 6f75  estimate.    rou
+000029a0: 6e64 6f66 6620 6572 726f 7220 7769 7468  ndoff error with
+000029b0: 2074 6865 2074 7275 6e63 6174 696f 6e20   the truncation 
+000029c0: 6572 726f 722e 2020 5468 6520 4265 7373  error.  The Bess
+000029d0: 656c 2066 756e 6374 696f 6e73 0a20 2020  el functions.   
+000029e0: 2061 7265 206f 6620 6f72 6465 7220 756e   are of order un
+000029f0: 6974 7920 616e 6420 6172 6520 7479 7069  ity and are typi
+00002a00: 6361 6c6c 7920 6361 6c63 756c 6174 6564  cally calculated
+00002a10: 2074 6f20 616e 2061 6273 6f6c 7574 650a   to an absolute.
+00002a20: 2020 2020 6163 6375 7261 6379 206f 6620      accuracy of 
+00002a30: 3a6d 6174 683a 605c 6570 7369 6c6f 6e60  :math:`\epsilon`
+00002a40: 2e20 2054 6865 2072 6f75 6e64 2d6f 6666  .  The round-off
+00002a50: 2065 7272 6f72 2069 6e20 7468 650a 2020   error in the.  
+00002a60: 2020 6e75 6d65 7261 746f 7220 6973 203a    numerator is :
+00002a70: 6d61 7468 3a60 5c65 7073 696c 6f6e 2066  math:`\epsilon f
+00002a80: 287a 2960 2061 6e64 203a 6d61 7468 3a60  (z)` and :math:`
+00002a90: 5c65 7073 696c 6f6e 205c 7371 7274 7b32  \epsilon \sqrt{2
+00002aa0: 7d0a 2020 2020 7a5f 6e60 2069 6e20 7468  }.    z_n` in th
+00002ab0: 6520 6465 6e6f 6d69 6e61 746f 722e 2020  e denominator.  
+00002ac0: 5468 6520 726f 756e 646f 6666 2065 7272  The roundoff err
+00002ad0: 6f72 7320 696e 2074 6865 2064 656e 6f6d  ors in the denom
+00002ae0: 696e 6174 6f72 0a20 2020 2064 6f6d 696e  inator.    domin
+00002af0: 6174 6520 626f 7468 2063 6173 6573 3a0a  ate both cases:.
+00002b00: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a20  .    .. math::. 
+00002b10: 2020 2020 2020 5c64 656c 7461 2046 287a        \delta F(z
+00002b20: 2920 265c 7369 6d20 5c65 7073 696c 6f6e  ) &\sim \epsilon
+00002b30: 205c 6672 6163 7b5c 7371 7274 7b32 7d7a   \frac{\sqrt{2}z
+00002b40: 5f6e 2046 287a 297d 7b5c 6465 6c74 617d  _n F(z)}{\delta}
+00002b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b60: 2020 2020 205c 7369 6d20 5c66 7261 637b       \sim \frac{
+00002b70: 5c73 7172 747b 327d 5c65 7073 696c 6f6e  \sqrt{2}\epsilon
+00002b80: 207a 5f6e 2066 287a 297d 7b5c 6465 6c74   z_n f(z)}{\delt
+00002b90: 615e 327d 0a20 2020 2020 2020 2020 2020  a^2}.           
+00002ba0: 2020 2020 2020 2020 205c 7369 6d20 5c66           \sim \f
+00002bb0: 7261 637b 5c73 7172 747b 327d 5c65 7073  rac{\sqrt{2}\eps
+00002bc0: 696c 6f6e 207a 5f6e 2066 2728 7a5f 6e29  ilon z_n f'(z_n)
+00002bd0: 7d7b 5c64 656c 7461 7d5c 5c0a 2020 2020  }{\delta}\\.    
+00002be0: 2020 205c 6465 6c74 6120 4627 287a 2920     \delta F'(z) 
+00002bf0: 265c 7369 6d20 5c66 7261 637b 325c 6570  &\sim \frac{2\ep
+00002c00: 7369 6c6f 6e20 7a5f 6e20 6628 7a29 7d7b  silon z_n f(z)}{
+00002c10: 5c64 656c 7461 5e33 7d0a 2020 2020 2020  \delta^3}.      
+00002c20: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00002c30: 7369 6d20 5c66 7261 637b 325c 6570 7369  sim \frac{2\epsi
+00002c40: 6c6f 6e20 7a5f 6e20 6627 287a 5f6e 297d  lon z_n f'(z_n)}
+00002c50: 7b5c 6465 6c74 615e 327d 0a0a 2020 2020  {\delta^2}..    
+00002c60: 546f 2063 686f 6f73 6520 7468 6520 6170  To choose the ap
+00002c70: 7072 6f70 7269 6174 6520 7472 616e 7369  propriate transi
+00002c80: 7469 6f6e 2070 6f69 6e74 2c20 7765 2065  tion point, we e
+00002c90: 7175 6174 6520 6861 6c66 206f 6620 7468  quate half of th
+00002ca0: 6973 0a20 2020 2077 6974 6820 7468 6520  is.    with the 
+00002cb0: 7472 756e 6361 7469 6f6e 2065 7272 6f72  truncation error
+00002cc0: 2074 6f20 7472 616e 7369 7469 6f6e 2070   to transition p
+00002cd0: 6f69 6e74 733a 0a0a 2020 2020 2e2e 206d  oints:..    .. m
+00002ce0: 6174 683a 3a0a 2020 2020 2020 205c 6465  ath::.       \de
+00002cf0: 6c74 615f 6320 265c 7369 6d20 5c6c 6566  lta_c &\sim \lef
+00002d00: 7428 0a20 2020 2020 2020 2020 205c 6672  t(.          \fr
+00002d10: 6163 7b37 325c 6570 7369 6c6f 6e20 7a5f  ac{72\epsilon z_
+00002d20: 6e20 6627 287a 5f6e 297d 7b5c 7371 7274  n f'(z_n)}{\sqrt
+00002d30: 7b32 7d66 5e7b 2834 297d 287a 5f6e 297d  {2}f^{(4)}(z_n)}
+00002d40: 0a20 2020 2020 2020 2020 205c 7269 6768  .          \righ
+00002d50: 7429 5e7b 312f 347d 0a20 2020 2020 2020  t)^{1/4}.       
+00002d60: 5c73 696d 205c 6c65 6674 285c 6672 6163  \sim \left(\frac
+00002d70: 7b37 325c 6570 7369 6c6f 6e20 7a5f 6e7d  {72\epsilon z_n}
+00002d80: 7b5c 7371 7274 7b32 7d7d 205c 7269 6768  {\sqrt{2}} \righ
+00002d90: 7429 5e7b 312f 347d 5c5c 0a20 2020 2020  t)^{1/4}\\.     
+00002da0: 2020 5c64 656c 7461 5f63 2720 265c 7369    \delta_c' &\si
+00002db0: 6d20 5c6c 6566 7428 3132 305c 6570 7369  m \left(120\epsi
+00002dc0: 6c6f 6e20 7a5f 6e5c 7269 6768 7429 5e7b  lon z_n\right)^{
+00002dd0: 312f 357d 0a0a 2020 2020 7468 6520 6661  1/5}..    the fa
+00002de0: 6374 2074 6861 7420 3a5c 6d61 7468 3a60  ct that :\math:`
+00002df0: 6628 7a29 6020 6265 6861 7665 730a 2020  f(z)` behaves.  
+00002e00: 2020 6173 796d 7074 6f74 6963 616c 6c79    asymptotically
+00002e10: 2061 7320 6120 3a6d 6174 683a 605c 7371   as a :math:`\sq
+00002e20: 7274 7b32 2f5c 7069 7d5c 636f 7328 7a20  rt{2/\pi}\cos(z 
+00002e30: 2b20 5c70 6869 2960 2061 6e64 2073 6f20  + \phi)` and so 
+00002e40: 616c 6c0a 2020 2020 6465 7269 7661 7469  all.    derivati
+00002e50: 7665 7320 6861 7665 2065 7373 656e 7469  ves have essenti
+00002e60: 616c 6c79 2074 6865 2073 616d 6520 6d61  ally the same ma
+00002e70: 676e 6974 7564 652e 0a0a 2020 2020 4578  gnitude...    Ex
+00002e80: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00002e90: 2d2d 2d0a 2020 2020 3e3e 3e20 6e75 203d  ---.    >>> nu =
+00002ea0: 2035 2e35 0a20 2020 203e 3e3e 207a 6e20   5.5.    >>> zn 
+00002eb0: 3d20 6a5f 726f 6f74 286e 752c 3231 295b  = j_root(nu,21)[
+00002ec0: 2d31 5d0a 2020 2020 3e3e 3e20 6162 7328  -1].    >>> abs(
+00002ed0: 7a6e 202d 2037 332e 3632 3336 3133 3138  zn - 73.62361318
+00002ee0: 3235 3137 3533 3339 3136 3436 2920 3c20  251753391646) < 
+00002ef0: 3165 2d31 360a 2020 2020 5472 7565 0a20  1e-16.    True. 
+00002f00: 2020 203e 3e3e 2066 6c6f 6174 284a 5f73     >>> float(J_s
+00002f10: 7172 745f 706f 6c65 286e 752c 7a6e 2928  qrt_pole(nu,zn)(
+00002f20: 7a6e 2929 2020 2023 2064 6f63 7465 7374  zn))   # doctest
+00002f30: 3a20 2b45 4c4c 4950 5349 530a 2020 2020  : +ELLIPSIS.    
+00002f40: 2d30 2e37 3936 3737 3835 3736 3738 3030  -0.7967785767800
+00002f50: 3133 2e2e 2e0a 0a20 2020 202d 302e 3739  13.....    -0.79
+00002f60: 3637 3738 3537 3637 3830 3031 3331 3239  6778576780013129
+00002f70: 3736 300a 0a20 2020 2059 6f75 2063 616e  760..    You can
+00002f80: 2061 6c73 6f20 7573 6520 6120 7665 6374   also use a vect
+00002f90: 6f72 206f 6620 607a 6e60 2c20 6275 7420  or of `zn`, but 
+00002fa0: 6f6e 6c79 2069 6620 6974 2069 7320 636f  only if it is co
+00002fb0: 6d6d 656e 7375 7261 7465 0a20 2020 2077  mmensurate.    w
+00002fc0: 6974 6820 7468 6520 6172 6775 6d65 6e74  ith the argument
+00002fd0: 3a0a 0a20 2020 203e 3e3e 207a 6e20 3d20  :..    >>> zn = 
+00002fe0: 6a5f 726f 6f74 286e 752c 3231 290a 2020  j_root(nu,21).  
+00002ff0: 2020 3e3e 3e20 666c 6f61 7428 4a5f 7371    >>> float(J_sq
+00003000: 7274 5f70 6f6c 6528 6e75 2c20 7a6e 2928  rt_pole(nu, zn)(
+00003010: 7a6e 5b2d 315d 295b 3230 5d29 2023 2064  zn[-1])[20]) # d
+00003020: 6f63 7465 7374 3a20 2b45 4c4c 4950 5349  octest: +ELLIPSI
+00003030: 530a 2020 2020 2d30 2e37 3936 3737 3835  S.    -0.7967785
+00003040: 3736 3738 3030 3133 2e2e 2e0a 2020 2020  76780013....    
+00003050: 2222 220a 2020 2020 4a5f 203d 204a 286e  """.    J_ = J(n
+00003060: 7529 0a20 2020 2064 4a20 3d20 4a28 6e75  u).    dJ = J(nu
+00003070: 2c20 3129 0a0a 2020 2020 2320 5461 796c  , 1)..    # Tayl
+00003080: 6f72 2063 6f65 6666 6963 6965 6e74 730a  or coefficients.
+00003090: 2020 2020 6320 3d20 286e 7520 2a20 6e75      c = (nu * nu
+000030a0: 202d 2030 2e32 3529 202f 207a 6e20 2f20   - 0.25) / zn / 
+000030b0: 7a6e 0a0a 2020 2020 667a 6e20 3d20 6e70  zn..    fzn = np
+000030c0: 2e7a 6572 6f73 2837 2c20 6474 7970 653d  .zeros(7, dtype=
+000030d0: 6f62 6a65 6374 290a 2020 2020 667a 6e5b  object).    fzn[
+000030e0: 315d 203d 206e 702e 7371 7274 287a 6e29  1] = np.sqrt(zn)
+000030f0: 202a 2064 4a28 7a6e 290a 2020 2020 667a   * dJ(zn).    fz
+00003100: 6e5b 335d 203d 2028 6320 2d20 3129 202a  n[3] = (c - 1) *
+00003110: 2066 7a6e 5b31 5d0a 2020 2020 667a 6e5b   fzn[1].    fzn[
+00003120: 345d 203d 202d 3420 2a20 6320 2f20 7a6e  4] = -4 * c / zn
+00003130: 202a 2066 7a6e 5b31 5d0a 2020 2020 667a   * fzn[1].    fz
+00003140: 6e5b 355d 203d 2028 3138 202a 2063 202f  n[5] = (18 * c /
+00003150: 207a 6e20 2f20 7a6e 202b 2028 6320 2d20   zn / zn + (c - 
+00003160: 3129 202a 2a20 3229 202a 2066 7a6e 5b31  1) ** 2) * fzn[1
+00003170: 5d0a 2020 2020 667a 6e5b 365d 203d 202d  ].    fzn[6] = -
+00003180: 3132 202a 2028 3820 2f20 7a6e 202f 207a  12 * (8 / zn / z
+00003190: 6e20 2b20 2863 202d 2031 2929 202a 2063  n + (c - 1)) * c
+000031a0: 202f 207a 6e20 2a20 667a 6e5b 315d 0a0a   / zn * fzn[1]..
+000031b0: 2020 2020 6d20 3d20 6e70 2e61 7261 6e67      m = np.arang
+000031c0: 6528 302c 206c 656e 2866 7a6e 2920 2d20  e(0, len(fzn) - 
+000031d0: 3129 0a20 2020 2061 5f46 203d 2066 7a6e  1).    a_F = fzn
+000031e0: 5b6d 202b 2031 5d20 2f20 286d 202b 2031  [m + 1] / (m + 1
+000031f0: 290a 0a20 2020 206d 203d 206e 702e 6172  )..    m = np.ar
+00003200: 616e 6765 2830 2c20 6c65 6e28 667a 6e29  ange(0, len(fzn)
+00003210: 202d 2032 290a 2020 2020 615f 6446 203d   - 2).    a_dF =
+00003220: 2066 7a6e 5b6d 202b 2032 5d20 2f20 286d   fzn[m + 2] / (m
+00003230: 202b 2032 290a 0a20 2020 2023 2041 206d   + 2)..    # A m
+00003240: 6f72 6520 636f 6d70 6c69 6361 7465 6420  ore complicated 
+00003250: 6573 7469 6d61 7465 2063 6f75 6c64 2062  estimate could b
+00003260: 6520 6d61 6465 2068 6572 652c 2062 7574  e made here, but
+00003270: 206f 6e65 206d 7573 7420 6265 0a20 2020   one must be.   
+00003280: 2023 2063 6172 6566 756c 2061 626f 7574   # careful about
+00003290: 2063 6173 6573 2073 7563 6820 6173 206e   cases such as n
+000032a0: 7520 3d20 302e 3520 7768 6572 6520 636f  u = 0.5 where co
+000032b0: 6566 6669 6369 656e 7473 2076 616e 6973  efficients vanis
+000032c0: 682e 0a20 2020 2066 315f 6636 203d 2031  h..    f1_f6 = 1
+000032d0: 2e30 2020 2320 667a 6e5b 315d 2f66 7a6e  .0  # fzn[1]/fzn
+000032e0: 5b36 5d0a 0a20 2020 2064 656c 7461 5f63  [6]..    delta_c
+000032f0: 203d 206e 702e 6162 7328 3732 3020 2a20   = np.abs(720 * 
+00003300: 6e70 2e73 7172 7428 3229 202a 205f 4550  np.sqrt(2) * _EP
+00003310: 5320 2a20 7a6e 202a 2066 315f 6636 2920  S * zn * f1_f6) 
+00003320: 2a2a 2028 3120 2f20 3629 0a20 2020 2064  ** (1 / 6).    d
+00003330: 6465 6c74 615f 6320 3d20 6e70 2e61 6273  delta_c = np.abs
+00003340: 2831 3434 202a 2032 202a 205f 4550 5320  (144 * 2 * _EPS 
+00003350: 2a20 7a6e 202a 2066 315f 6636 2920 2a2a  * zn * f1_f6) **
+00003360: 2028 3120 2f20 3629 0a0a 2020 2020 6465   (1 / 6)..    de
+00003370: 6620 6628 7a2c 204a 3d4a 5f29 3a0a 2020  f f(z, J=J_):.  
+00003380: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
+00003390: 7371 7274 287a 2920 2a20 4a28 7a29 0a0a  sqrt(z) * J(z)..
+000033a0: 2020 2020 6465 6620 6466 287a 2c20 4a3d      def df(z, J=
+000033b0: 4a5f 2c20 644a 3d64 4a29 3a0a 2020 2020  J_, dJ=dJ):.    
+000033c0: 2020 2020 7265 7475 726e 204a 287a 2920      return J(z) 
+000033d0: 2f20 3220 2f20 6e70 2e73 7172 7428 7a29  / 2 / np.sqrt(z)
+000033e0: 202b 206e 702e 7371 7274 287a 2920 2a20   + np.sqrt(z) * 
+000033f0: 644a 287a 290a 0a20 2020 2069 6620 3020  dJ(z)..    if 0 
+00003400: 3d3d 2064 3a0a 0a20 2020 2020 2020 2064  == d:..        d
+00003410: 6566 2046 287a 293a 0a20 2020 2020 2020  ef F(z):.       
+00003420: 2020 2020 2064 656e 6f6d 203d 207a 202d       denom = z -
+00003430: 207a 6e0a 2020 2020 2020 2020 2020 2020   zn.            
+00003440: 7265 7475 726e 206e 702e 7768 6572 6528  return np.where(
+00003450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003460: 2061 6273 2864 656e 6f6d 2920 3e20 6465   abs(denom) > de
+00003470: 6c74 615f 632c 0a20 2020 2020 2020 2020  lta_c,.         
+00003480: 2020 2020 2020 206e 702e 6469 7669 6465         np.divide
+00003490: 2866 287a 292c 2064 656e 6f6d 202b 205f  (f(z), denom + _
+000034a0: 5449 4e59 292c 0a20 2020 2020 2020 2020  TINY),.         
+000034b0: 2020 2020 2020 205f 486f 726e 6572 2861         _Horner(a
+000034c0: 5f46 2c20 6465 6e6f 6d29 2c0a 2020 2020  _F, denom),.    
+000034d0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000034e0: 2020 2072 6574 7572 6e20 460a 2020 2020     return F.    
+000034f0: 656c 6966 2031 203d 3d20 643a 0a0a 2020  elif 1 == d:..  
+00003500: 2020 2020 2020 6465 6620 6446 287a 293a        def dF(z):
+00003510: 0a20 2020 2020 2020 2020 2020 2064 656e  .            den
+00003520: 6f6d 203d 207a 202d 207a 6e0a 2020 2020  om = z - zn.    
+00003530: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00003540: 702e 7768 6572 6528 0a20 2020 2020 2020  p.where(.       
+00003550: 2020 2020 2020 2020 2061 6273 2864 656e           abs(den
+00003560: 6f6d 2920 3e20 6464 656c 7461 5f63 2c0a  om) > ddelta_c,.
+00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003580: 6e70 2e64 6976 6964 6528 6466 287a 2920  np.divide(df(z) 
+00003590: 2d20 6e70 2e64 6976 6964 6528 6628 7a29  - np.divide(f(z)
+000035a0: 2c20 6465 6e6f 6d29 2c20 6465 6e6f 6d29  , denom), denom)
+000035b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000035c0: 2020 5f48 6f72 6e65 7228 615f 6446 2c20    _Horner(a_dF, 
+000035d0: 6465 6e6f 6d29 2c0a 2020 2020 2020 2020  denom),.        
+000035e0: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
+000035f0: 6574 7572 6e20 6446 0a20 2020 2065 6c73  eturn dF.    els
+00003600: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+00003610: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00003620: 7272 6f72 2822 4f6e 6c79 2064 3d30 206f  rror("Only d=0 o
+00003630: 7220 3120 7375 7070 6f72 7465 6420 2867  r 1 supported (g
+00003640: 6f74 2064 3d7b 7d29 2e22 2e66 6f72 6d61  ot d={}).".forma
+00003650: 7428 6429 290a 0a0a 6465 6620 5f48 6f72  t(d))...def _Hor
+00003660: 6e65 7228 612c 2064 293a 0a20 2020 2022  ner(a, d):.    "
+00003670: 2222 5265 7475 726e 2073 756d 2861 5b6e  ""Return sum(a[n
+00003680: 5d2f 6e21 2a64 5e6e 2920 6576 616c 7561  ]/n!*d^n) evalua
+00003690: 7465 6420 7573 696e 6720 486f 726e 6572  ted using Horner
+000036a0: 2773 0a20 2020 206d 6574 686f 642e 0a0a  's.    method...
+000036b0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+000036c0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
+000036d0: 3e20 6120 3d20 5b31 2c20 312c 2032 2c20  > a = [1, 1, 2, 
+000036e0: 332a 322c 2034 2a33 2a32 5d0a 2020 2020  3*2, 4*3*2].    
+000036f0: 3e3e 3e20 6420 3d20 320a 2020 2020 3e3e  >>> d = 2.    >>
+00003700: 3e20 5f48 6f72 6e65 7228 612c 6429 0a20  > _Horner(a,d). 
+00003710: 2020 2033 312e 300a 2020 2020 2222 220a     31.0.    """.
+00003720: 2020 2020 6420 3d20 6e70 2e61 7361 7272      d = np.asarr
+00003730: 6179 2864 290a 2020 2020 616e 7320 3d20  ay(d).    ans = 
+00003740: 3020 2a20 640a 2020 2020 666f 7220 6e20  0 * d.    for n 
+00003750: 696e 2072 6576 6572 7365 6428 7261 6e67  in reversed(rang
+00003760: 6528 6c65 6e28 6129 2929 3a0a 2020 2020  e(len(a))):.    
+00003770: 2020 2020 616e 7320 2b3d 2061 5b6e 5d0a      ans += a[n].
+00003780: 2020 2020 2020 2020 6966 206e 203e 2030          if n > 0
+00003790: 3a0a 2020 2020 2020 2020 2020 2020 616e  :.            an
+000037a0: 7320 2a3d 2064 202f 206e 0a20 2020 2072  s *= d / n.    r
+000037b0: 6574 7572 6e20 616e 730a                 eturn ans.
```

### Comparing `mmfutils-0.6.3/src/mmfutils/math/__pycache__/wigner.cpython-39.pyc` & `mmfutils-0.6.4/src/mmfutils/math/wigner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,102 @@
-00000000: 610d 0d0a 0000 0000 b70b fc61 5806 0000  a..........aX...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
-00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
-00000040: 6d04 5a04 6d05 5a05 0100 6409 6407 6408  m.Z.m.Z...d.d.d.
-00000050: 8401 5a06 6402 5300 290a 7a76 5769 676e  ..Z.d.S.).zvWign
-00000060: 6572 2056 696c 6c65 2064 6973 7472 6962  er Ville distrib
-00000070: 7574 696f 6e2e 0a0a 5468 6973 206d 6f64  ution...This mod
-00000080: 756c 6520 636f 6e74 6169 6e73 2073 6f6d  ule contains som
-00000090: 6520 4646 542d 6261 7365 6420 726f 7574  e FFT-based rout
-000000a0: 696e 6573 2066 6f72 2063 6f6d 7075 7469  ines for computi
-000000b0: 6e67 2074 6865 0a57 6967 6e65 722d 5669  ng the.Wigner-Vi
-000000c0: 6c6c 6520 6469 7374 7269 6275 7469 6f6e  lle distribution
-000000d0: 2e0a e900 0000 004e 2902 da03 6666 74da  .......N)...fft.
-000000e0: 0469 6666 74e9 0100 0000 4654 6305 0000  .ifft.....FTc...
-000000f0: 0000 0000 0000 0000 000e 0000 0006 0000  ................
-00000100: 0043 0000 0073 0a01 0000 7400 7c00 8301  .C...s....t.|...
-00000110: 7d05 7401 6a02 7401 6a03 a004 7c05 7c01  }.t.j.t.j...|.|.
-00000120: a102 1400 7d06 7c02 723a 7405 7401 a006  ....}.|.r:t.t...
-00000130: 7c06 a101 6401 1700 7403 7c00 8301 1400  |...d...t.|.....
-00000140: 8301 7d00 7c04 725c 7401 a007 7c00 7401  ..}.|.r\t...|.t.
-00000150: a008 7c00 a101 6702 a101 7d00 7c05 6402  ..|...g...}.|.d.
-00000160: 1400 7d07 6e04 7c05 7d07 7401 a009 6403  ..}.n.|.}.t...d.
-00000170: 7c05 7c03 a103 6404 6404 8502 6404 6602  |.|...d.d...d.f.
-00000180: 1900 7d08 7401 a009 7c05 a101 6404 6404  ..}.t...|...d.d.
-00000190: 6404 8502 6602 1900 7d09 7c08 7c09 1700  d...f...}.|.|...
-000001a0: 7c07 1600 7d0a 7c08 7c09 1800 7c07 1600  |...}.|.|...|...
-000001b0: 7d0b 7c00 7c0a 1900 7c00 7c0b 1900 a00a  }.|.|...|.|.....
-000001c0: a100 1400 7d0c 6402 7403 7c0c 6405 6406  ....}.d.t.|.d.d.
-000001d0: 8d02 6a0b 6404 7c05 8502 6404 6404 8502  ..j.d.|...d.d...
-000001e0: 6602 1900 1400 7c01 1400 7d0d 7401 6a03  f.....|...}.t.j.
-000001f0: 6a0c 7c0d 6405 6407 8d02 7d0d 7401 6a03  j.|.d.d...}.t.j.
-00000200: a00c 7c06 a101 7d06 7c06 7c0d 7c01 1400  ..|...}.|.|.|...
-00000210: 6602 5300 2908 61c1 0200 0052 6574 7572  f.S.).a....Retur
-00000220: 6e20 6028 7773 2c20 5029 6020 7768 6572  n `(ws, P)` wher
-00000230: 6520 6050 6020 6973 2074 6865 2057 6967  e `P` is the Wig
-00000240: 6e65 7220 5669 6c6c 6520 7175 6173 692d  ner Ville quasi-
-00000250: 6469 7374 7269 6275 7469 6f6e 2066 6f72  distribution for
-00000260: 2070 7369 2e0a 0a20 2020 2041 7373 756d   psi...    Assum
-00000270: 6573 2074 6861 7420 7073 6920 6973 2070  es that psi is p
-00000280: 6572 696f 6469 632e 2020 4e6f 7465 3a20  eriodic.  Note: 
-00000290: 7468 6520 6672 6571 7565 6e63 6965 7320  the frequencies 
-000002a0: 6174 2077 6869 6368 2060 5060 0a20 2020  at which `P`.   
-000002b0: 2069 7320 7661 6c69 6420 6172 6520 6861   is valid are ha
-000002c0: 6c66 2074 6865 2066 7265 7175 656e 6369  lf the frequenci
-000002d0: 6573 206e 6f72 6d61 6c6c 7920 6173 736f  es normally asso
-000002e0: 6369 6174 6564 2077 6974 6820 7468 650a  ciated with the.
-000002f0: 2020 2020 7761 7665 6675 6e63 7469 6f6e      wavefunction
-00000300: 2e20 2054 6875 7320 7765 2061 6c73 6f20  .  Thus we also 
-00000310: 7265 7475 726e 2074 6865 2061 7373 6f63  return the assoc
-00000320: 6961 7465 6420 6672 6571 7565 6e63 6965  iated frequencie
-00000330: 7320 746f 0a20 2020 2061 766f 6964 2070  s to.    avoid p
-00000340: 6f73 7369 626c 6520 636f 6e66 7573 696f  ossible confusio
-00000350: 6e2e 0a0a 2020 2020 4172 6775 6d65 6e74  n...    Argument
-00000360: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d0a  s.    ---------.
-00000370: 2020 2020 7073 6920 3a20 6172 7261 792d      psi : array-
-00000380: 6c69 6b65 0a20 2020 2020 2020 5468 6520  like.       The 
-00000390: 696e 7075 7420 7369 676e 616c 2e0a 2020  input signal..  
-000003a0: 2020 6474 203a 2066 6c6f 6174 0a20 2020    dt : float.   
-000003b0: 2020 2020 5374 6570 2073 697a 6520 666f      Step size fo
-000003c0: 7220 7468 6520 696e 7075 7420 6162 7363  r the input absc
-000003d0: 6973 7361 2e0a 2020 2020 6d61 6b65 5f61  issa..    make_a
-000003e0: 6e61 6c79 7469 6320 3a20 626f 6f6c 0a20  nalytic : bool. 
-000003f0: 2020 2020 2020 4966 2054 7275 652c 2074        If True, t
-00000400: 6865 6e20 6e65 6761 7469 7665 2066 7265  hen negative fre
-00000410: 7175 656e 6379 2063 6f6d 706f 6e65 6e74  quency component
-00000420: 7320 6172 6520 7365 7420 746f 207a 6572  s are set to zer
-00000430: 6f2e 0a20 2020 2073 6b69 7020 3a20 696e  o..    skip : in
-00000440: 740a 2020 2020 2020 2044 6f77 6e73 616d  t.       Downsam
-00000450: 706c 6520 7468 6520 7469 6d65 2d64 6f6d  ple the time-dom
-00000460: 6169 6e20 6279 2073 6b69 7070 696e 6720  ain by skipping 
-00000470: 7468 6973 206d 616e 7920 706f 696e 7473  this many points
-00000480: 2e0a 2020 2020 7061 6420 3a20 626f 6f6c  ..    pad : bool
-00000490: 0a20 2020 2020 2020 4966 2054 7275 652c  .       If True,
-000004a0: 2074 6865 6e20 7061 6420 7468 6520 696e   then pad the in
-000004b0: 7075 7420 6172 7261 7920 746f 2072 656d  put array to rem
-000004c0: 6f76 6520 616c 6961 7369 6e67 2061 7274  ove aliasing art
-000004d0: 6966 6163 7473 2e0a 2020 2020 7204 0000  ifacts..    r...
-000004e0: 00e9 0200 0000 7201 0000 004e e9ff ffff  ......r....N....
-000004f0: ff29 01da 0461 7869 7329 01da 0461 7865  .)...axis)...axe
-00000500: 7329 0dda 036c 656e da02 6e70 da02 7069  s)...len..np..pi
-00000510: 7202 0000 00da 0766 6674 6672 6571 7203  r......fftfreqr.
-00000520: 0000 00da 0473 6967 6eda 0668 7374 6163  .....sign..hstac
-00000530: 6bda 0a7a 6572 6f73 5f6c 696b 65da 0661  k..zeros_like..a
-00000540: 7261 6e67 65da 0463 6f6e 6ada 0472 6561  range..conj..rea
-00000550: 6cda 0866 6674 7368 6966 7429 0eda 0370  l..fftshift)...p
-00000560: 7369 da02 6474 5a0d 6d61 6b65 5f61 6e61  si..dtZ.make_ana
-00000570: 6c79 7469 63da 0473 6b69 70da 0370 6164  lytic..skip..pad
-00000580: da01 4eda 0277 735a 044e 7061 64da 0169  ..N..wsZ.Npad..i
-00000590: da01 6a5a 0269 5f5a 026a 5fda 0350 7369  ..jZ.i_Z.j_..Psi
-000005a0: da01 50a9 0072 1e00 0000 fa3e 2f55 7365  ..P..r.....>/Use
-000005b0: 7273 2f6d 666f 7262 6573 2f77 6f72 6b2f  rs/mforbes/work/
-000005c0: 6d6d 6662 622f 6d6d 6675 7469 6c73 2f73  mmfbb/mmfutils/s
-000005d0: 7263 2f6d 6d66 7574 696c 732f 6d61 7468  rc/mmfutils/math
-000005e0: 2f77 6967 6e65 722e 7079 da0c 7769 676e  /wigner.py..wign
-000005f0: 6572 5f76 696c 6c65 0b00 0000 7322 0000  er_ville....s"..
-00000600: 0000 1608 0114 0104 031a 0204 0114 010a  ................
-00000610: 0204 021a 0116 010c 010c 0114 0126 0110  .............&..
-00000620: 010c 0172 2000 0000 2904 7204 0000 0046  ...r ...).r....F
-00000630: 7204 0000 0054 2907 da07 5f5f 646f 635f  r....T)...__doc_
-00000640: 5fda 056e 756d 7079 720a 0000 005a 186d  _..numpyr....Z.m
-00000650: 6d66 7574 696c 732e 7065 7266 6f72 6d61  mfutils.performa
-00000660: 6e63 652e 6666 7472 0200 0000 7203 0000  nce.fftr....r...
-00000670: 0072 2000 0000 721e 0000 0072 1e00 0000  .r ...r....r....
-00000680: 721e 0000 0072 1f00 0000 da08 3c6d 6f64  r....r......<mod
-00000690: 756c 653e 0100 0000 7306 0000 0004 0508  ule>....s.......
-000006a0: 0210 03                                  ...
+00000000: 2222 2257 6967 6e65 7220 5669 6c6c 6520  """Wigner Ville 
+00000010: 6469 7374 7269 6275 7469 6f6e 2e0a 0a54  distribution...T
+00000020: 6869 7320 6d6f 6475 6c65 2063 6f6e 7461  his module conta
+00000030: 696e 7320 736f 6d65 2046 4654 2d62 6173  ins some FFT-bas
+00000040: 6564 2072 6f75 7469 6e65 7320 666f 7220  ed routines for 
+00000050: 636f 6d70 7574 696e 6720 7468 650a 5769  computing the.Wi
+00000060: 676e 6572 2d56 696c 6c65 2064 6973 7472  gner-Ville distr
+00000070: 6962 7574 696f 6e2e 0a22 2222 0a69 6d70  ibution..""".imp
+00000080: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00000090: 0a66 726f 6d20 6d6d 6675 7469 6c73 2e70  .from mmfutils.p
+000000a0: 6572 666f 726d 616e 6365 2e66 6674 2069  erformance.fft i
+000000b0: 6d70 6f72 7420 6666 742c 2069 6666 740a  mport fft, ifft.
+000000c0: 0a0a 6465 6620 7769 676e 6572 5f76 696c  ..def wigner_vil
+000000d0: 6c65 2870 7369 2c20 6474 3d31 2c20 6d61  le(psi, dt=1, ma
+000000e0: 6b65 5f61 6e61 6c79 7469 633d 4661 6c73  ke_analytic=Fals
+000000f0: 652c 2073 6b69 703d 312c 2070 6164 3d54  e, skip=1, pad=T
+00000100: 7275 6529 3a0a 2020 2020 2222 2252 6574  rue):.    """Ret
+00000110: 7572 6e20 6028 7773 2c20 5029 6020 7768  urn `(ws, P)` wh
+00000120: 6572 6520 6050 6020 6973 2074 6865 2057  ere `P` is the W
+00000130: 6967 6e65 7220 5669 6c6c 6520 7175 6173  igner Ville quas
+00000140: 692d 6469 7374 7269 6275 7469 6f6e 2066  i-distribution f
+00000150: 6f72 2070 7369 2e0a 0a20 2020 2041 7373  or psi...    Ass
+00000160: 756d 6573 2074 6861 7420 7073 6920 6973  umes that psi is
+00000170: 2070 6572 696f 6469 632e 2020 4e6f 7465   periodic.  Note
+00000180: 3a20 7468 6520 6672 6571 7565 6e63 6965  : the frequencie
+00000190: 7320 6174 2077 6869 6368 2060 5060 0a20  s at which `P`. 
+000001a0: 2020 2069 7320 7661 6c69 6420 6172 6520     is valid are 
+000001b0: 6861 6c66 2074 6865 2066 7265 7175 656e  half the frequen
+000001c0: 6369 6573 206e 6f72 6d61 6c6c 7920 6173  cies normally as
+000001d0: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
+000001e0: 650a 2020 2020 7761 7665 6675 6e63 7469  e.    wavefuncti
+000001f0: 6f6e 2e20 2054 6875 7320 7765 2061 6c73  on.  Thus we als
+00000200: 6f20 7265 7475 726e 2074 6865 2061 7373  o return the ass
+00000210: 6f63 6961 7465 6420 6672 6571 7565 6e63  ociated frequenc
+00000220: 6965 7320 746f 0a20 2020 2061 766f 6964  ies to.    avoid
+00000230: 2070 6f73 7369 626c 6520 636f 6e66 7573   possible confus
+00000240: 696f 6e2e 0a0a 2020 2020 4172 6775 6d65  ion...    Argume
+00000250: 6e74 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  nts.    --------
+00000260: 2d0a 2020 2020 7073 6920 3a20 6172 7261  -.    psi : arra
+00000270: 792d 6c69 6b65 0a20 2020 2020 2020 5468  y-like.       Th
+00000280: 6520 696e 7075 7420 7369 676e 616c 2e0a  e input signal..
+00000290: 2020 2020 6474 203a 2066 6c6f 6174 0a20      dt : float. 
+000002a0: 2020 2020 2020 5374 6570 2073 697a 6520        Step size 
+000002b0: 666f 7220 7468 6520 696e 7075 7420 6162  for the input ab
+000002c0: 7363 6973 7361 2e0a 2020 2020 6d61 6b65  scissa..    make
+000002d0: 5f61 6e61 6c79 7469 6320 3a20 626f 6f6c  _analytic : bool
+000002e0: 0a20 2020 2020 2020 4966 2054 7275 652c  .       If True,
+000002f0: 2074 6865 6e20 6e65 6761 7469 7665 2066   then negative f
+00000300: 7265 7175 656e 6379 2063 6f6d 706f 6e65  requency compone
+00000310: 6e74 7320 6172 6520 7365 7420 746f 207a  nts are set to z
+00000320: 6572 6f2e 0a20 2020 2073 6b69 7020 3a20  ero..    skip : 
+00000330: 696e 740a 2020 2020 2020 2044 6f77 6e73  int.       Downs
+00000340: 616d 706c 6520 7468 6520 7469 6d65 2d64  ample the time-d
+00000350: 6f6d 6169 6e20 6279 2073 6b69 7070 696e  omain by skippin
+00000360: 6720 7468 6973 206d 616e 7920 706f 696e  g this many poin
+00000370: 7473 2e0a 2020 2020 7061 6420 3a20 626f  ts..    pad : bo
+00000380: 6f6c 0a20 2020 2020 2020 4966 2054 7275  ol.       If Tru
+00000390: 652c 2074 6865 6e20 7061 6420 7468 6520  e, then pad the 
+000003a0: 696e 7075 7420 6172 7261 7920 746f 2072  input array to r
+000003b0: 656d 6f76 6520 616c 6961 7369 6e67 2061  emove aliasing a
+000003c0: 7274 6966 6163 7473 2e0a 2020 2020 2222  rtifacts..    ""
+000003d0: 220a 0a20 2020 204e 203d 206c 656e 2870  "..    N = len(p
+000003e0: 7369 290a 2020 2020 7773 203d 206e 702e  si).    ws = np.
+000003f0: 7069 202a 206e 702e 6666 742e 6666 7466  pi * np.fft.fftf
+00000400: 7265 7128 4e2c 2064 7429 2020 2320 4e6f  req(N, dt)  # No
+00000410: 7465 206d 6973 7369 6e67 2066 6163 746f  te missing facto
+00000420: 7220 6f66 2032 0a20 2020 2069 6620 6d61  r of 2.    if ma
+00000430: 6b65 5f61 6e61 6c79 7469 633a 0a20 2020  ke_analytic:.   
+00000440: 2020 2020 2023 204d 616b 6520 7369 676e       # Make sign
+00000450: 616c 2061 6e61 6c79 7469 630a 2020 2020  al analytic.    
+00000460: 2020 2020 2320 5365 6520 6874 7470 733a      # See https:
+00000470: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00000480: 7267 2f77 696b 692f 416e 616c 7974 6963  rg/wiki/Analytic
+00000490: 5f73 6967 6e61 6c0a 2020 2020 2020 2020  _signal.        
+000004a0: 7073 6920 3d20 6966 6674 2828 6e70 2e73  psi = ifft((np.s
+000004b0: 6967 6e28 7773 2920 2b20 3129 202a 2066  ign(ws) + 1) * f
+000004c0: 6674 2870 7369 2929 0a0a 2020 2020 6966  ft(psi))..    if
+000004d0: 2070 6164 3a0a 2020 2020 2020 2020 7073   pad:.        ps
+000004e0: 6920 3d20 6e70 2e68 7374 6163 6b28 5b70  i = np.hstack([p
+000004f0: 7369 2c20 6e70 2e7a 6572 6f73 5f6c 696b  si, np.zeros_lik
+00000500: 6528 7073 6929 5d29 0a20 2020 2020 2020  e(psi)]).       
+00000510: 204e 7061 6420 3d20 4e20 2a20 320a 2020   Npad = N * 2.  
+00000520: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00000530: 4e70 6164 203d 204e 0a0a 2020 2020 6920  Npad = N..    i 
+00000540: 3d20 6e70 2e61 7261 6e67 6528 302c 204e  = np.arange(0, N
+00000550: 2c20 736b 6970 295b 3a2c 204e 6f6e 655d  , skip)[:, None]
+00000560: 0a20 2020 206a 203d 206e 702e 6172 616e  .    j = np.aran
+00000570: 6765 284e 295b 4e6f 6e65 2c20 3a5d 0a20  ge(N)[None, :]. 
+00000580: 2020 2069 5f20 3d20 2869 202b 206a 2920     i_ = (i + j) 
+00000590: 2520 4e70 6164 0a20 2020 206a 5f20 3d20  % Npad.    j_ = 
+000005a0: 2869 202d 206a 2920 2520 4e70 6164 0a20  (i - j) % Npad. 
+000005b0: 2020 2050 7369 203d 2070 7369 5b69 5f5d     Psi = psi[i_]
+000005c0: 202a 2070 7369 5b6a 5f5d 2e63 6f6e 6a28   * psi[j_].conj(
+000005d0: 290a 2020 2020 5020 3d20 3220 2a20 6666  ).    P = 2 * ff
+000005e0: 7428 5073 692c 2061 7869 733d 2d31 292e  t(Psi, axis=-1).
+000005f0: 7265 616c 5b3a 4e2c 203a 5d20 2a20 6474  real[:N, :] * dt
+00000600: 0a20 2020 2050 203d 206e 702e 6666 742e  .    P = np.fft.
+00000610: 6666 7473 6869 6674 2850 2c20 6178 6573  fftshift(P, axes
+00000620: 3d2d 3129 0a20 2020 2077 7320 3d20 6e70  =-1).    ws = np
+00000630: 2e66 6674 2e66 6674 7368 6966 7428 7773  .fft.fftshift(ws
+00000640: 290a 2020 2020 7265 7475 726e 2077 732c  ).    return ws,
+00000650: 2050 202a 2064 740a                       P * dt.
```

### Comparing `mmfutils-0.6.3/src/mmfutils/math/bases/bases.py` & `mmfutils-0.6.4/src/mmfutils/math/bases/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def init(self):
         dx = self.R / self.N
         r = np.arange(1, self.N + 1) * dx
         k = np.pi * (0.5 + np.arange(self.N)) / self.R
         self.xyz = [r]
         self._pxyz = [k]
-        self.metric = 4 * np.pi * r ** 2 * dx
+        self.metric = 4 * np.pi * r**2 * dx
         self.k_max = k.max()
 
     def laplacian(self, y, factor=1.0, exp=False):
         """Return the laplacian of `y` times `factor` or the
         exponential of this.
 
         Arguments
@@ -81,15 +81,15 @@
 
         return res
 
     def coulomb_kernel(self, k):
         """Form for the truncated Coulomb kernel."""
         D = 2 * self.R
         return (
-            4 * np.pi * np.ma.divide(1.0 - np.cos(k * D), k ** 2).filled(D ** 2 / 2.0)
+            4 * np.pi * np.ma.divide(1.0 - np.cos(k * D), k**2).filled(D**2 / 2.0)
         )
 
     def convolve_coulomb(self, y, form_factors=[]):
         """Modified Coulomb convolution to include form-factors (if provided).
 
         This version implemented a 3D spherically symmetric convolution.
         """
@@ -171,17 +171,18 @@
         memoization_GB=0.5,
         _test=False,
     ):
         self.symmetric_lattice = symmetric_lattice
         self.Nxyz = np.asarray(Nxyz)
         self.Lxyz = np.asarray(Lxyz)
         self.smoothing_cutoff = smoothing_cutoff
-        self.boost_pxyz = boost_pxyz
-        if boost_pxyz is not None:
-            self.boost_pxyz = np.asarray(boost_pxyz)
+        self.memoization_GB = memoization_GB
+        if boost_pxyz is None:
+            boost_pxyz = np.zeros_like(self.Lxyz)
+        self.boost_pxyz = np.asarray(boost_pxyz)
         if axes is None:
             axes = np.arange(-self.dim, 0)
         self.axes = np.asarray(axes)
         self.memoization_GB = memoization_GB
         self._test = _test
         super().__init__()
 
@@ -206,28 +207,28 @@
                 _p - _b
                 for (_p, _b) in zip(self._pxyz, self.xp.asarray(self.boost_pxyz))
             ]
 
         self.metric = np.prod(self.Lxyz / self.Nxyz)
         self.k_max = np.array([float(abs(_p).max()) for _p in self._pxyz])
 
-        x_GB = self.Nxyz[0] * np.dtype(float).itemsize / 1024 ** 3
-        yz_GB = np.prod(self.Nxyz[1:]) * np.dtype(float).itemsize / 1024 ** 3
-        xyz_GB = np.prod(self.Nxyz) * np.dtype(float).itemsize / 1024 ** 3
+        x_GB = self.Nxyz[0] * np.dtype(float).itemsize / 1024**3
+        yz_GB = np.prod(self.Nxyz[1:]) * np.dtype(float).itemsize / 1024**3
+        xyz_GB = np.prod(self.Nxyz) * np.dtype(float).itemsize / 1024**3
 
         # These computations can take a lot of memory if the state is big... we defer
         # unless actually needed.
         self.__pxyz_derivative = None  # Computed as needed: see _pxyz_derivative
         self.__smoothing_factor = None  # Computed as needed: see _cmoothing_factor
         # _k2 + _kx2 + _kyz2
         memoize_size_GB = xyz_GB + x_GB + yz_GB
         if memoize_size_GB < self.memoization_GB:
             # Memoize momentum sums for speed
             _kx2 = self._pxyz[0] ** 2
-            _kyz2 = sum(_p ** 2 for _p in self._pxyz[1:])
+            _kyz2 = sum(_p**2 for _p in self._pxyz[1:])
             _k2 = _kx2 + _kyz2
             self._k2_kx2_kyz2 = (_k2, _kx2, _kyz2)
         else:
             self._k2_kx2_kyz2 = None
 
     # These are some memoized properties
     @property
@@ -247,14 +248,15 @@
         if self.__smoothing_factor is None:
             p2_pc2 = sum(
                 (_p / (self.smoothing_cutoff * _p).max()) ** 2 for _p in self._pxyz
             )
             self.__smoothing_factor = self.xp.where(p2_pc2 < 1, 1, 0)
         return self._smoothing_factor
 
+    @property
     def kx(self):
         return self._pxyz[0]
 
     @property
     def Lx(self):
         return self.Lxyz[0]
 
@@ -264,15 +266,15 @@
 
     def _apply_K(self, yt, kx2=None, k2=None, exp=False, factor=1.0):
         """Apply `K` or `exp(K)` to the `yt=fftn(y)`."""
         if not exp and k2 is None and self._k2_kx2_kyz2 is None:
             # Special memory-limited processing... slow.
             if kx2 is None:
                 kx2 = self._pxyz[0] ** 2
-            k2s = [kx2] + [_p ** 2 for _p in self._pxyz[1:]]
+            k2s = [kx2] + [_p**2 for _p in self._pxyz[1:]]
             return -factor * sum(_k2 * yt for _k2 in k2s)
         elif k2 is None and self._k2_kx2_kyz2 is None:
             raise NotImplementedError("Must be able to memoize if exp=True")
         else:
             if k2 is None:
                 _k2, _kx2, _kyz2 = self._k2_kx2_kyz2
                 if kx2 is None:
@@ -401,27 +403,27 @@
         """Form for the Coulomb kernel.
 
         The normalization here is that the k=0 component is set to
         zero.  This means that the charge distribution has an overall
         constant background removed so that the net charge in the unit
         cell is zero.
         """
-        return 4 * np.pi * np.ma.divide(1.0, k ** 2).filled(0.0)
+        return 4 * np.pi * np.ma.divide(1.0, k**2).filled(0.0)
 
     def convolve_coulomb(self, y, form_factors=[]):
         """Periodic convolution with the Coulomb kernel."""
         y = np.asarray(y)
 
         # This broadcasts to the appropriate size if there are
         # multiple components.
         # dim = len(np.asarray(self.Lxyz))
         # N = np.asarray(y.shape)
         # b_cast = [None] * (dim - len(N)) + [slice(None)]*dim
 
-        k = np.sqrt(sum(_k ** 2 for _k in self._pxyz))
+        k = np.sqrt(sum(_k**2 for _k in self._pxyz))
         Ck = prod([_K(k) for _K in [self.coulomb_kernel] + form_factors])
         return self.ifftn(Ck * self.fftn(y))
 
     def convolve(self, y, C=None, Ck=None):
         """Return the periodic convolution `int(C(x-r)*y(r),r)`.
 
         Arguments
@@ -434,15 +436,15 @@
            If provided, then this function will be used instead directly in
            momentum space.  Assumed to be spherically symmetric (will be passed
            only the magnitude `k`)
         """
         if Ck is None:
             Ck = self.fftn(C)
         else:
-            k = np.sqrt(sum(_k ** 2 for _k in self._pxyz))
+            k = np.sqrt(sum(_k**2 for _k in self._pxyz))
             Ck = Ck(k)
         return self.ifftn(Ck * self.fftn(y))
 
     @property
     def dim(self):
         return len(self.Nxyz)
 
@@ -549,16 +551,16 @@
         N0[-dim:] = N[-dim:] // 3
 
         y0 = resample(y, N0)
         V = resample(
             self.convolve_coulomb_exact(y0, form_factors=form_factors, method="pad"), N
         )
         if correct:
-            k = np.sqrt(sum(_K ** 2 for _K in self._pxyz))
-            C = 4 * np.pi * np.ma.divide(1.0, k ** 2).filled(0.0)
+            k = np.sqrt(sum(_K**2 for _K in self._pxyz))
+            C = 4 * np.pi * np.ma.divide(1.0, k**2).filled(0.0)
             for F in form_factors:
                 C = C * F(k)
             dV = self.ifftn(C * self.fftn(y - resample(y0, N)))
             if np.issubdtype(V.dtype, np.complex128):
                 V += dV
             else:
                 assert np.allclose(0, V.imag)
@@ -591,18 +593,18 @@
 
         .. math::
            4\pi(1-\cos\sqrt{3}Lk)/k^2
         """
         y = np.asarray(y)
         L = np.asarray(self.Lxyz)
         dim = len(L)
-        D = np.sqrt((L ** 2).sum())  # Diameter of cell
+        D = np.sqrt((L**2).sum())  # Diameter of cell
 
         def C(k):
-            C = 4 * np.pi * np.ma.divide(1 - np.cos(D * k), k ** 2).filled(D ** 2 / 2.0)
+            C = 4 * np.pi * np.ma.divide(1 - np.cos(D * k), k**2).filled(D**2 / 2.0)
             for F in form_factors:
                 C = C * F(k)
             return C
 
         if method == "sum":
             # Sum with a loop.  Minimizes the memory usage, but will not
             # use multiple cores.
@@ -616,26 +618,26 @@
                 k = np.sqrt(sum((_k + _d) ** 2 for _k, _d in zip(K, delta)))
                 dV = exp_delta * self.ifftn(C(k) * self.fftn(y_delta))
                 if np.issubdtype(V.dtype, np.complex128):
                     V += dV
                 else:
                     assert np.allclose(0, V.imag)
                     V += dV.real
-            return V / dim ** 3
+            return V / dim**3
         elif method == "pad":
             N = np.asarray(y.shape[-dim:])
             N_padded = 3 * N
             L_padded = 3 * L
             shape = np.asarray(y.shape)
             shape_padded = shape.copy()
             shape_padded[-dim:] = N_padded
             y_padded = np.zeros(shape_padded, dtype=y.dtype)
             inds = tuple(slice(0, _N) for _N in shape)
             y_padded[inds] = y
-            k = np.sqrt(sum(_K ** 2 for _K in get_kxyz(N_padded, L_padded)))
+            k = np.sqrt(sum(_K**2 for _K in get_kxyz(N_padded, L_padded)))
 
             # This broadcasts to the appropriate size
             b_cast = (None,) * (dim - len(N)) + (slice(None),) * dim
             return self.ifftn(C(k)[b_cast] * self.fftn(y_padded))[inds]
         else:
             raise NotImplementedError(
                 "method=%s not implemented: use 'sum' or 'pad'" % (method,)
@@ -686,15 +688,15 @@
 
     def init(self):
         Lx, R = self.Lxr
         x = get_xyz(Nxyz=self.Nxr, Lxyz=self.Lxr, symmetric_lattice=self.symmetric_x)[0]
         kx0 = get_kxyz(Nxyz=self.Nxr, Lxyz=self.Lxr)[0]
         self.kx = kx0 + float(self.twist) / Lx - self.boost_px
         self._kx0 = kx0
-        self._kx2 = self.kx ** 2
+        self._kx2 = self.kx**2
 
         self.y_twist = np.exp(1j * self.twist * x / Lx)
 
         Nx, Nr = self.Nxr
 
         # For large n, the roots of the bessel function are approximately
         # z[n] = (n + 0.75)*pi, so R = r_max = z_max/k_max = (N-0.25)*pi/kmax
@@ -902,16 +904,16 @@
         w = 2.0 / (self._kmax * z * bessel.J(nu=nu, d=1)(z) ** 2)
 
         # DVR kinetic term for radial function:
         K = np.ma.divide(
             (-1.0) ** (n[i1] - n[i2]) * 8.0 * z[i1] * z[i2],
             (z[i1] ** 2 - z[i2] ** 2) ** 2,
         ).filled(0)
-        K[n, n] = 1.0 / 3.0 * (1.0 + 2.0 * (nu ** 2 - 1.0) / z ** 2)
-        K *= self._kmax ** 2
+        K[n, n] = 1.0 / 3.0 * (1.0 + 2.0 * (nu**2 - 1.0) / z**2)
+        K *= self._kmax**2
 
         # Here we convert from the wavefunction Psi(r) to the radial
         # function u(r) = sqrt(r)*Psi(r) and back with factors of
         # sqrt(wr).  This includes the integration weights (since K is
         # defined acting on the basis functions).
         # Note: this makes the matrix non-hermitian, so don't do this if you
         # want to diagonalize.
```

### Comparing `mmfutils-0.6.3/src/mmfutils/math/bases/interfaces.py` & `mmfutils-0.6.4/src/mmfutils/math/bases/interfaces.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/bases/utils.py` & `mmfutils-0.6.4/src/mmfutils/math/bases/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """General utility functions"""
-from distutils.version import StrictVersion
+# from distutils.version import StrictVersion as Version
+from packaging.version import Version
 import functools
 import operator
 
 import numpy as np
 from numpy.linalg import norm
 import scipy as sp
 
@@ -103,15 +104,15 @@
 def idst(F, axis=-1):
     """Return the Inverse Discrete Sine Transform (DST II) of `f`"""
     N = F.shape[-1]
     args = dict(type=2, axis=axis)
     return sp.fftpack.dst(F, **args) / (2.0 * N)
 
 
-if StrictVersion(sp.__version__) < StrictVersion("0.16.0"):
+if Version(sp.__version__) < Version("0.16.0"):
     # Scipy pre 0.16.0 cannot handle complex inputs.
     dst_real, idst_real = dst, idst
 
     def dst(f, axis=-1):
         """Return the Discrete Sine Transform (DST III) of `f`"""
         res = dst_real(f.real)
         if np.iscomplexobj(f):
```

### Comparing `mmfutils-0.6.3/src/mmfutils/math/differentiate.py` & `mmfutils-0.6.4/src/mmfutils/math/differentiate.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/integrate/__init__.py` & `mmfutils-0.6.4/src/mmfutils/math/integrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/integrate/_ssum_cython.c` & `mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.c`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/integrate/_ssum_cython.pyx` & `mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.pyx`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/linalg.py` & `mmfutils-0.6.4/src/mmfutils/math/linalg.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/math/special.py` & `mmfutils-0.6.4/src/mmfutils/math/special.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/optimize.py` & `mmfutils-0.6.4/src/mmfutils/optimize.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/parallel.py` & `mmfutils-0.6.4/src/mmfutils/parallel.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/performance/blas.py` & `mmfutils-0.6.4/src/mmfutils/performance/blas.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/performance/fft.py` & `mmfutils-0.6.4/src/mmfutils/performance/fft.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/performance/numexpr.py` & `mmfutils-0.6.4/src/mmfutils/performance/numexpr.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/performance/threads.py` & `mmfutils-0.6.4/src/mmfutils/performance/threads.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/animation.py` & `mmfutils-0.6.4/src/mmfutils/plot/animation.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,48 +17,50 @@
 
     1. Allowing user to store video when generating HTML video.
     2. Allow clean stopping between frames in a NoInterupt context.
     """
 
     def __init__(self, *v, **kw):
         self.interrupted = kw.pop("interrupted", False)
+        if not hasattr(kw, "save_count"):
+            kw.setdefault("cache_frame_data", False)
         FuncAnimation.__init__(self, *v, **kw)
 
     def new_frame_seq(self):
         for frame in FuncAnimation.new_frame_seq(self):
             if self.interrupted:
                 break
             yield frame
 
     def to_html5_video(self, embed_limit=None, filename=None, extra_args=None):
         """Convert the animation to an HTML5 ``<video>`` tag.
 
         This saves the animation as an h264 video, encoded in base64
-        directly into the HTML5 video tag. This respects :obj:`animation.writer`
-        and :obj:`animation.bitrate`. This also makes use of the
-        ``interval`` to control the speed, and uses the ``repeat``
+        directly into the HTML5 video tag. This respects :rc:`animation.writer`
+        and :rc:`animation.bitrate`. This also makes use of the
+        *interval* to control the speed, and uses the *repeat*
         parameter to decide whether to loop.
 
         Parameters
         ----------
         embed_limit : float, optional
             Limit, in MB, of the returned animation. No animation is created
             if the limit is exceeded.
-            Defaults to :obj:`embed_limit` = 20.0.
+            Defaults to :rc:`animation.embed_limit` = 20.0.
         filename : str, optional
            *(New)* If provided, save the movie in this file and keep it,
            otherwise the movie will be stored in a temporary directory
            and deleted after.
 
         Returns
         -------
         video_tag : str
             An HTML5 video tag with the animation embedded as base64 encoded
             h264 video.
-            If the :obj:`embed_limit` is exceeded, this returns the string
+            If the *embed_limit* is exceeded, this returns the string
             "Video too large to embed."
         """
         VIDEO_TAG = r"""<video {size} {options}>
   <source type="video/mp4" src="data:video/mp4;base64,{video}">
   Your browser does not support the video tag.
 </video>"""
         # Cache the rendering of the video as HTML
@@ -84,26 +86,20 @@
             if filename is None:
                 # Can't open a NamedTemporaryFile twice on Windows, so use a
                 # TemporaryDirectory instead.
                 with TemporaryDirectory() as tmpdir:
                     path = Path(tmpdir, "temp.m4v")
                     self.save(str(path), writer=writer)
                     # Now open and base64 encode.
-                    with open(str(path), "rb") as video:
-                        vid64 = encodebytes(video.read())
-                    # The following works on python 3 only
-                    # vid64 = encodebytes(path.read_bytes())
+                    vid64 = encodebytes(path.read_bytes())
             else:
                 path = Path(filename)
                 self.save(str(path), writer=writer)
                 # Now open and base64 encode.
-                with open(str(path), "rb") as video:
-                    vid64 = encodebytes(video.read())
-                # The following works on python 3 only
-                # vid64 = encodebytes(path.read_bytes())
+                vid64 = encodebytes(path.read_bytes())
 
             # End of modifications
             ########################################################
             vid_len = len(vid64)
             if vid_len >= embed_limit:
                 _log.warning(
                     "Animation movie is %s bytes, exceeding the limit of %s. "
@@ -119,15 +115,15 @@
 
         # If we exceeded the size, this attribute won't exist
         if hasattr(self, "_base64_video"):
             # Default HTML5 options are to autoplay and display video controls
             options = ["controls", "autoplay"]
 
             # If we're set to repeat, make it loop
-            if hasattr(self, "repeat") and self.repeat:
+            if getattr(self, "_repeat", False):
                 options.append("loop")
 
             return VIDEO_TAG.format(
                 video=self._base64_video,
                 size=self._video_size,
                 options=" ".join(options),
             )
@@ -164,15 +160,14 @@
     if display:
         from IPython.display import display, clear_output
 
     if fig is None:
         fig = plt.gcf()
 
     def _get_frames():
-
         nframe = 0
         for frame in get_frames():
             if nframe == 0:
                 # Initial frame used to setup figure.  This is not recorded in
                 # the movie.
                 yield frame
```

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/cmaps.py` & `mmfutils-0.6.4/src/mmfutils/plot/cmaps.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/colors.py` & `mmfutils-0.6.4/src/mmfutils/plot/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,11 +202,12 @@
 
     def _add_to_matplotlib(self):
         # Monkeypatch matplotlib to add the new color maps
         for cm in self:
             if not hasattr(matplotlib.cm, cm):
                 cmap = getattr(self, cm)
                 setattr(matplotlib.cm, cm, cmap)
-                matplotlib.cm.register_cmap(name=cm, cmap=cmap)
+                # matplotlib.cm.register_cmap(name=cm, cmap=cmap)
+                matplotlib.colormaps.register(cmap=cmap, name=cm)
 
 
 cm = Colormaps(**cmaps)
```

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/contour.py` & `mmfutils-0.6.4/src/mmfutils/plot/contour.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/errors.py` & `mmfutils-0.6.4/src/mmfutils/plot/errors.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/publish.py` & `mmfutils-0.6.4/src/mmfutils/plot/publish.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/plot/rasterize.py` & `mmfutils-0.6.4/src/mmfutils/plot/rasterize.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.3/src/mmfutils/solve/broyden.py` & `mmfutils-0.6.4/src/mmfutils/solve/broyden.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 
 import numpy as np
 
 # We import these here in case we want to change in future to use more
 # efficient implementations.
 from numpy import matmul
 
-import scipy.optimize.nonlin
+try:
+    from scipy.optimize import Jacobian as sp_Jacobian
+except ImportError:
+    try:
+        from scipy.optimize._nonlin import Jacobian as sp_Jacobian
+    except ImportError:
+        from scipy.optimize.nonlin import Jacobian as sp_Jacobian
+
 import scipy as sp
 
 from ..math.linalg import block_diag
 
 __all__ = ["DyadicSum"]
 
 
@@ -659,15 +666,15 @@
         if method == "good":
             dxB = self.__rmatmul__(np.asarray(dx))  # dx @ self
             self.add_dyad((dx - Bdf) / dx.dot(Bdf), dxB)
         else:
             self.add_dyad((dx - Bdf) / df.dot(df), df)
 
 
-class JacobianBFGS(sp.optimize.nonlin.Jacobian):
+class JacobianBFGS(sp_Jacobian):
     r"""Represent a symmetric matrix by a memory-limited L-BFGS approximation.
 
     This assumes that the Jacobian :math:`J_{ij} = \partial_i\partial_j f(x)` is
     symmetric, and stores a memory-limited representation of the Hessian :math:`H =
     J^{-1}`.  This should be used for optimization problems minimizing :math:`f(x)`.
 
     See Chapter 7 of [Nocedal:2006] (7.19) in particular.
@@ -685,15 +692,15 @@
 
     def __init__(self, alpha=1.0, n_max=20):
         self._dx = []
         self._df = []
         self._H0 = alpha
         self._last_x = self._last_f = None
         self.n_max = n_max
-        sp.optimize.nonlin.Jacobian.__init__(self)
+        sp_Jacobian.__init__(self)
 
     @property
     def H0(self):
         """Return the factor for the initial inverse Jacobian approximation.
 
         This default version uses equation (7.20) of [Nocedal:2006]
         """
@@ -772,26 +779,26 @@
 
     todense = toarray = dense_J
 
     def update(self, x, f):
         if self._last_x is not None:
             dx = x - self._last_x
             df = f - self._last_f
-            if np.allclose(0, df.dot(dx), atol=_EPS ** 2):
+            if np.allclose(0, df.dot(dx), atol=_EPS**2):
                 raise np.linalg.LinAlgError("Current step makes Jacobian singular.")
             self._dx.append(dx)
             self._df.append(df)
             if len(self._dx) > self.n_max:
                 self._dx = self._dx[-self.n_max :]
                 self._df = self._df[-self.n_max :]
         self._last_x, self._last_f = x, f
 
 
 class Jacobian(DyadicSum):
-    """Provides the `scipy.optimize.nonlin.Jacobian` interface."""
+    """Provides the `scipy.optimize.Jacobian` interface."""
 
     def __init__(self, method="good", *v, **kw):
         DyadicSum.__init__(self, *v, **kw)
         self.last_f = None
         self.last_x = None
         self.method = method
```

### Comparing `mmfutils-0.6.3/src/mmfutils/testing.py` & `mmfutils-0.6.4/src/mmfutils/testing.py`

 * *Files identical despite different names*

