# Comparing `tmp/python-sat-0.1.8.dev3.tar.gz` & `tmp/python-sat-0.1.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev3.tar", last modified: Fri Apr 21 08:08:39 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev4.tar", last modified: Thu May 25 02:35:20 2023, max compression
```

## Comparing `python-sat-0.1.8.dev3.tar` & `python-sat-0.1.8.dev4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.947493 python-sat-0.1.8.dev3/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-04-21 08:08:39.947572 python-sat-0.1.8.dev3/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev3/README.rst
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.920034 python-sat-0.1.8.dev3/allies/
--rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev3/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    13494 2023-04-21 08:07:34.000000 python-sat-0.1.8.dev3/allies/approxmc.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.922703 python-sat-0.1.8.dev3/cardenc/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev3/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.926142 python-sat-0.1.8.dev3/examples/
--rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev3/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20609 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev3/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev3/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    68707 2023-03-19 00:37:27.000000 python-sat-0.1.8.dev3/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.928663 python-sat-0.1.8.dev3/pysat/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      653 2023-04-21 07:53:10.000000 python-sat-0.1.8.dev3/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    90179 2023-01-30 23:39:56.000000 python-sat-0.1.8.dev3/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev3/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   169376 2023-03-05 04:20:33.000000 python-sat-0.1.8.dev3/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.930112 python-sat-0.1.8.dev3/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1863 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)        1 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       87 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       23 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/requirements.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      107 2023-04-21 08:08:39.947929 python-sat-0.1.8.dev3/setup.cfg
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev3/setup.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.937919 python-sat-0.1.8.dev3/solvers/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev3/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev3/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.944239 python-sat-0.1.8.dev3/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev3/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    66092 2023-03-06 01:41:40.000000 python-sat-0.1.8.dev3/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev3/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev3/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev3/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    25391 2023-03-06 01:41:50.000000 python-sat-0.1.8.dev3/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   214965 2023-03-05 04:21:31.000000 python-sat-0.1.8.dev3/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.947104 python-sat-0.1.8.dev3/tests/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev3/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev3/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev3/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev3/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev3/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.969249 python-sat-0.1.8.dev4/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-05-25 02:35:20.969327 python-sat-0.1.8.dev4/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev4/README.rst
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.953835 python-sat-0.1.8.dev4/allies/
+-rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev4/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev4/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.955968 python-sat-0.1.8.dev4/cardenc/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev4/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.957965 python-sat-0.1.8.dev4/examples/
+-rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev4/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20609 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev4/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev4/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    66919 2023-05-25 02:24:53.000000 python-sat-0.1.8.dev4/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.959266 python-sat-0.1.8.dev4/pysat/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      653 2023-05-25 02:26:56.000000 python-sat-0.1.8.dev4/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev4/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev4/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   169376 2023-03-05 04:20:33.000000 python-sat-0.1.8.dev4/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.960147 python-sat-0.1.8.dev4/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1863 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)        1 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       87 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       23 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      107 2023-05-25 02:35:20.969586 python-sat-0.1.8.dev4/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev4/setup.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.964551 python-sat-0.1.8.dev4/solvers/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev4/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev4/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.967531 python-sat-0.1.8.dev4/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev4/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    66092 2023-03-06 01:41:40.000000 python-sat-0.1.8.dev4/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev4/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev4/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev4/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    25391 2023-03-06 01:41:50.000000 python-sat-0.1.8.dev4/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   214965 2023-03-05 04:21:31.000000 python-sat-0.1.8.dev4/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.969106 python-sat-0.1.8.dev4/tests/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev4/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev4/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev4/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev4/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev4/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev3/LICENSE.txt` & `python-sat-0.1.8.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/PKG-INFO` & `python-sat-0.1.8.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev3
+Version: 0.1.8.dev4
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev3/README.rst` & `python-sat-0.1.8.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/allies/approxmc.py` & `python-sat-0.1.8.dev4/allies/approxmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,18 @@
         >>>
         >>> cnf = CNF(from_file='formula.cnf.xz')
         >>>
         >>> with Counter(cnf) as counter:
         ...     print(counter.counter(projection=range(1, 10))
         448
 
-    As can be seen in the above example, the counter supports *projected*
-    model counting, i.e. when one needs to approximate the number of models
-    with respect to a given list of variables rather than with respect to all
+    As can be seen in the above example, besides model counting across all the
+    variables in a given input formula, the counter supports *projected* model
+    counting, i.e. when one needs to approximate the number of models with
+    respect to a given list of variables rather than with respect to all
     variables appearing in the formula. This feature comes in handy when the
     formula is obtained, for example, through Tseitin transformation [3]_ with
     a number of auxiliary variables introduced.
 
     .. [3] G. S. Tseitin. *On the complexity of derivations in the
         propositional calculus*. Studies in Mathematics and Mathematical
         Logic, Part II. pp. 115–125, 1968
```

### Comparing `python-sat-0.1.8.dev3/cardenc/bitwise.hh` & `python-sat-0.1.8.dev4/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/card.hh` & `python-sat-0.1.8.dev4/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/clset.hh` & `python-sat-0.1.8.dev4/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/common.hh` & `python-sat-0.1.8.dev4/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/itot.hh` & `python-sat-0.1.8.dev4/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/ladder.hh` & `python-sat-0.1.8.dev4/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/mto.hh` & `python-sat-0.1.8.dev4/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/pairwise.hh` & `python-sat-0.1.8.dev4/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/ptypes.hh` & `python-sat-0.1.8.dev4/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/pycard.cc` & `python-sat-0.1.8.dev4/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev4/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/sortcard.hh` & `python-sat-0.1.8.dev4/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/cardenc/utils.hh` & `python-sat-0.1.8.dev4/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/fm.py` & `python-sat-0.1.8.dev4/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/genhard.py` & `python-sat-0.1.8.dev4/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/hitman.py` & `python-sat-0.1.8.dev4/examples/hitman.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/lbx.py` & `python-sat-0.1.8.dev4/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/lsu.py` & `python-sat-0.1.8.dev4/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/mcsls.py` & `python-sat-0.1.8.dev4/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/models.py` & `python-sat-0.1.8.dev4/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/musx.py` & `python-sat-0.1.8.dev4/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/optux.py` & `python-sat-0.1.8.dev4/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/examples/rc2.py` & `python-sat-0.1.8.dev4/examples/rc2.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 
         # other MaxSAT related stuff
         self.pool = IDPool(start_from=formula.nv + 1)
         self.wght = {}  # weights of soft clauses
         self.sums = []  # totalizer sum assumptions
         self.bnds = {}  # a mapping from sum assumptions to totalizer bounds
         self.tobj = {}  # a mapping from sum assumptions to totalizer objects
+        self.swgt = {}  # a mapping from sum assumptions to their core weights
         self.cost = 0
 
         # mappings between internal and external variables
         VariableMap = collections.namedtuple('VariableMap', ['e2i', 'i2e'])
         self.vmap = VariableMap(e2i={}, i2e={})
 
         # initialize SAT oracle with hard clauses only
@@ -667,15 +668,15 @@
 
                 # apply core exhaustion if required
                 b = self.exhaust_core(t) if self.exhaust else 1
 
                 if b:
                     # save the info about this sum and
                     # add its assumption literal
-                    self.set_bound(t, b)
+                    self.set_bound(t, b, self.minw)
                 else:
                     # impossible to satisfy any of these clauses
                     # they must become hard
                     for relv in self.rels:
                         self.oracle.add_clause([relv])
         else:
             # unit cores are treated differently
@@ -1000,24 +1001,16 @@
 
             # increase bound for the sum
             t, b = self.update_sum(l)
 
             # updating bounds and weights
             if b < len(t.rhs):
                 lnew = -t.rhs[b]
-                if lnew in self.garbage:
-                    # the previous bound l also participates in the core, i.e.
-                    # lnew is removed from garbage and keeps it weight (self.minw)
-                    self.garbage.remove(lnew)
-                elif lnew not in self.wght:
-                    # this is a newly created bound literal
-                    self.set_bound(t, b)
-                else:
-                    # a known literal whose weight should be inflated
-                    self.wght[lnew] += self.minw
+                if lnew not in self.swgt:
+                    self.set_bound(t, b, self.swgt[l])
 
             # put this assumption to relaxation vars
             self.rels.append(-l)
 
     def create_sum(self, bound=1):
         """
             Create a totalizer object encoding a cardinality
@@ -1124,15 +1117,15 @@
 
                 # a new at-most-b constraint
                 amb = [[-t.rhs[b]] * (rhs - b) + t.lits, rhs]
                 self.oracle.add_atmost(*amb)
 
         return t, b
 
-    def set_bound(self, tobj, rhs):
+    def set_bound(self, tobj, rhs, weight):
         """
             Given a totalizer sum and its right-hand side to be
             enforced, the method creates a new sum assumption literal,
             which will be used in the following SAT oracle calls.
 
             :param tobj: totalizer sum
             :param rhs: right-hand side
@@ -1140,15 +1133,16 @@
             :type tobj: :class:`.ITotalizer`
             :type rhs: int
         """
 
         # saving the sum and its weight in a mapping
         self.tobj[-tobj.rhs[rhs]] = tobj
         self.bnds[-tobj.rhs[rhs]] = rhs
-        self.wght[-tobj.rhs[rhs]] = self.minw
+        self.wght[-tobj.rhs[rhs]] = weight
+        self.swgt[-tobj.rhs[rhs]] = weight
 
         # adding a new assumption to force the sum to be at most rhs
         self.sums.append(-tobj.rhs[rhs])
 
     def filter_assumps(self):
         """
             Filter out unnecessary selectors and sums from the list of
@@ -1603,58 +1597,23 @@
 
             # increase bound for the sum
             t, b = self.update_sum(l)
 
             # updating bounds and weights
             if b < len(t.rhs):
                 lnew = -t.rhs[b]
-                if lnew in self.garbage:
-                    # the previous bound l also participates in the core, i.e.
-                    # lnew is removed from garbage and keeps it weight (self.minw)
-                    self.garbage.remove(lnew)
-                elif lnew not in self.wght:
-                    # this is a newly created bound literal
-                    self.set_bound(t, b)
-                else:
-                    # a known literal whose weight should be inflated
-                    self.inflate_sum(lnew)
+                if lnew not in self.swgt:
+                    self.set_bound(t, b, self.swgt[l])
 
             # put this assumption to relaxation vars
             self.rels.append(-l)
 
         # deactivating unnecessary sums
         self.sums = list(filter(lambda x: x not in to_deactivate, self.sums))
 
-    def inflate_sum(self, lit):
-        """
-            Bump up the weight for a next-bound sum literal if it already
-            exists while the previous-bound sum literal is split up such that
-            ``lit`` gets an additional weight. If the literal was inactive
-            earlier, it is activated at the current level.
-        """
-
-        wght = self.wght[lit]
-
-        if wght < self.blop[self.levl]:
-            # removing the literal from its current stratum
-            for lid in range(len(self.wstr[wght]) - 1, -1, -1):
-                if self.wstr[wght][lid] == lit:
-                    self.wstr[wght][lid] = self.wstr[wght][-1]
-                    self.wstr[wght].pop()
-                    break
-            else:
-                assert 0, 'no literal {0} in the stratum for {1}'.format(lit, wght)
-
-            # the sum literal should be activated now since it is
-            # guaranteed that self.minw >= self.blop[self.levl]
-            self.sums.append(lit)
-
-        # incrementing the weight
-        self.wght[lit] += self.minw
-
 
 #
 #==============================================================================
 def parse_options():
     """
         Parses command-line option
     """
```

### Comparing `python-sat-0.1.8.dev3/examples/usage.py` & `python-sat-0.1.8.dev4/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/pysat/__init__.py` & `python-sat-0.1.8.dev4/pysat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (0, 1, 8, "dev", 3)
+VERSION = (0, 1, 8, "dev", 4)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = "%d.%d.%d.%s%d" % VERSION if len(VERSION) == 5 else \
               "%d.%d.%d" % VERSION
```

### Comparing `python-sat-0.1.8.dev3/pysat/_fileio.py` & `python-sat-0.1.8.dev4/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/pysat/_utils.py` & `python-sat-0.1.8.dev4/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/pysat/card.py` & `python-sat-0.1.8.dev4/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/pysat/formula.py` & `python-sat-0.1.8.dev4/pysat/formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,20 @@
     def __init__(self, start_from=1, occupied=[]):
         """
             Constructor.
         """
 
         self.restart(start_from=start_from, occupied=occupied)
 
+    def __repr__(self):
+        """
+            State reproducible string representaion of object.
+        """
+        return f"IDPool(start_from={self.top+1}, occupied={self._occupied})"
+
     def restart(self, start_from=1, occupied=[]):
         """
             Restart the manager from scratch. The arguments replicate those of
             the constructor of :class:`IDPool`.
         """
 
         # initial ID
@@ -429,14 +435,21 @@
         elif from_string:
             self.from_string(from_string, comment_lead)
         elif from_clauses:
             self.from_clauses(from_clauses)
         elif from_aiger:
             self.from_aiger(from_aiger)
 
+    def __repr__(self):
+        """
+            State reproducible string representaion of object.
+        """
+        s = self.to_dimacs().replace('\n', '\\n')
+        return f"CNF(from_string=\"{s}\")"
+
     def from_file(self, fname, comment_lead=['c'], compressed_with='use_ext'):
         """
             Read a CNF formula from a file in the DIMACS format. A file name is
             expected as an argument. A default argument is ``comment_lead`` for
             parsing comment lines. A given file can be compressed by either
             gzip, bzip2, or lzma.
 
@@ -524,15 +537,15 @@
 
             Example:
 
             .. code-block:: python
 
                 >>> from pysat.formula import CNF
                 >>> cnf1 = CNF()
-                >>> cnf1.from_string(='p cnf 2 2\\n-1 2 0\\n1 -2 0')
+                >>> cnf1.from_string('p cnf 2 2\\n-1 2 0\\n1 -2 0')
                 >>> print(cnf1.clauses)
                 [[-1, 2], [1, -2]]
                 >>>
                 >>> cnf2 = CNF(from_string='p cnf 3 3\\n-1 2 0\\n-2 3 0\\n-3 0\\n')
                 >>> print(cnf2.clauses)
                 [[-1, 2], [-2, 3], [-3]]
                 >>> print(cnf2.nv)
@@ -730,14 +743,48 @@
                 print(c, file=file_pointer)
 
         print('p cnf', self.nv, len(self.clauses), file=file_pointer)
 
         for cl in self.clauses:
             print(' '.join(str(l) for l in cl), '0', file=file_pointer)
 
+    def to_dimacs(self):
+        """
+            Return the current state of the object in DIMACS format.
+
+            For example, if 'some-file.cnf' contains:
+
+            ::
+
+                c Example
+                p cnf 3 3
+                -1 2 0
+                -2 3 0
+                -3 0
+
+            Then you can obtain the DIMACS with:
+
+            .. code-block:: python
+
+                >>> from pysat.formula import CNF
+                >>> cnf = CNF(from_file='some-file.cnf')
+                >>> print(cnf.to_dimacs())
+                c Example
+                p cnf 3 3
+                -1 2 0
+                -2 3 0
+                -3 0
+
+        """
+        header_lines = [f"p cnf {self.nv} {len(self.clauses)}"]
+        comment_lines = [f"{comment}" for comment in self.comments]
+        clause_lines = [" ".join(map(str,clause)) + " 0" for clause in self.clauses]
+        lines = "\n".join(comment_lines + header_lines + clause_lines) + "\n"
+        return lines
+
     def to_alien(self, file_pointer, format='opb', comments=None):
         """
             The method can be used to dump a CNF formula into a file pointer
             in an alien file format, which at this point can either be LP,
             OPB, or SMT. The file pointer is expected as an argument.
             Additionally, the target format 'lp', 'opb', or 'smt' may be
             specified (equal to 'opb' by default). Finally, supplementary
@@ -1014,14 +1061,21 @@
         if from_file:
             self.from_file(from_file, comment_lead, compressed_with='use_ext')
         elif from_fp:
             self.from_fp(from_fp, comment_lead)
         elif from_string:
             self.from_string(from_string, comment_lead)
 
+    def __repr__(self):
+        """
+            State reproducible string representaion of object.
+        """
+        s = self.to_dimacs().replace('\n', '\\n')
+        return f"WCNF(from_string=\"{s}\")"
+
     def from_file(self, fname, comment_lead=['c'], compressed_with='use_ext'):
         """
             Read a WCNF formula from a file in the DIMACS format. A file name
             is expected as an argument. A default argument is ``comment_lead``
             for parsing comment lines. A given file can be compressed by either
             gzip, bzip2, or lzma.
 
@@ -1175,15 +1229,15 @@
 
             Example:
 
             .. code-block:: python
 
                 >>> from pysat.formula import WCNF
                 >>> cnf1 = WCNF()
-                >>> cnf1.from_string(='p wcnf 2 2 2\\n 2 -1 2 0\\n1 1 -2 0')
+                >>> cnf1.from_string('p wcnf 2 2 2\\n 2 -1 2 0\\n1 1 -2 0')
                 >>> print(cnf1.hard)
                 [[-1, 2]]
                 >>> print(cnf1.soft)
                 [[1, 2]]
                 >>>
                 >>> cnf2 = WCNF(from_string='p wcnf 3 3 2\\n2 -1 2 0\\n2 -2 3 0\\n1 -3 0\\n')
                 >>> print(cnf2.hard)
@@ -1310,14 +1364,49 @@
         # some tools (e.g. LBX) cannot count them properly
         for i, cl in enumerate(self.soft):
             print(self.wght[i], ' '.join(str(l) for l in cl), '0', file=file_pointer)
 
         for cl in self.hard:
             print(self.topw, ' '.join(str(l) for l in cl), '0', file=file_pointer)
 
+    def to_dimacs(self):
+        """
+            Return the current state of the object in extended DIMACS format.
+
+            For example, if 'some-file.cnf' contains:
+
+            ::
+
+                c Example
+                p wcnf 2 3 10
+                1 -1 0
+                2 -2 0
+                10 1 2 0
+
+            Then you can obtain the DIMACS with:
+
+            .. code-block:: python
+
+                >>> from pysat.formula import WCNF
+                >>> cnf = WCNF(from_file='some-file.cnf')
+                >>> print(cnf.to_dimacs())
+                c Example
+                p wcnf 2 3 10
+                10 1 2 0
+                1 -1 0
+                2 -2 0
+
+        """
+        header_lines = [f"p wcnf {self.nv} {len(self.hard)+len(self.soft)} {self.topw}"]
+        comment_lines = [f"{comment}" for comment in self.comments]
+        hard_lines = [f"{self.topw} " + " ".join(map(str,clause)) + " 0" for clause in self.hard]
+        soft_lines = [f"{weight} " + " ".join(map(str,clause)) + " 0" for clause, weight in zip(self.soft, self.wght)]
+        lines = "\n".join(comment_lines + header_lines + hard_lines + soft_lines) + "\n"
+        return lines
+
     def to_alien(self, file_pointer, format='opb', comments=None):
         """
             The method can be used to dump a WCNF formula into a file pointer
             in an alien file format, which at this point can either be LP,
             OPB, or SMT. The file pointer is expected as an argument.
             Additionally, the target format 'lp', 'opb', or 'smt' may be
             specified (equal to 'opb' by default). Finally, supplementary
@@ -1591,14 +1680,21 @@
         # atmost constraints are initially empty
         self.atmosts = []
 
         # calling the base class constructor
         super(CNFPlus, self).__init__(from_file=from_file, from_fp=from_fp,
                 from_string=from_string, comment_lead=comment_lead)
 
+    def __repr__(self):
+        """
+            State reproducible string representaion of object.
+        """
+        s = self.to_dimacs().replace('\n', '\\n')
+        return f"CNFPlus(from_string=\"{s}\")"
+
     def from_fp(self, file_pointer, comment_lead=['c']):
         """
             Read a CNF+ formula from a file pointer. A file pointer should be
             specified as an argument. The only default argument is
             ``comment_lead``, which can be used for parsing specific comment
             lines.
 
@@ -1688,14 +1784,49 @@
 
         for cl in self.clauses:
             print(' '.join(str(l) for l in cl), '0', file=file_pointer)
 
         for am in self.atmosts:
             print(' '.join(str(l) for l in am[0]), '<=', am[1], file=file_pointer)
 
+    def to_dimacs(self):
+        """
+            Return the current state of the object in extended DIMACS format.
+
+            For example, if 'some-file.cnf' contains:
+
+            ::
+
+                c Example
+                p cnf+ 7 3
+                1 -2 3 5 -7 <= 3
+                4 5 6 -7 >= 2
+                3 5 7 0
+
+            Then you can obtain the DIMACS with:
+
+            .. code-block:: python
+
+                >>> from pysat.formula import CNFPlus
+                >>> cnf = CNFPlus(from_file='some-file.cnf')
+                >>> print(cnf.to_dimacs())
+                c Example
+                p cnf+ 7 3
+                3 5 7 0
+                1 -2 3 5 -7 <= 3
+                -4 -5 -6 7 <= 2
+
+        """
+        header_lines = [f"p cnf+ {self.nv} {len(self.clauses) + len(self.atmosts)}"]
+        comment_lines = [f"{comment}" for comment in self.comments]
+        clause_lines = [" ".join(map(str,clause)) + " 0" for clause in self.clauses]
+        atmost_lines = [" ".join(map(str,clause)) + " <= " + str(most) for clause, most in self.atmosts]
+        lines = "\n".join(comment_lines + header_lines + clause_lines + atmost_lines) + "\n"
+        return lines
+
     def to_alien(self, file_pointer, format='opb', comments=None):
         """
             The method can be used to dump a CNF+ formula into a file pointer
             in an alien file format, which at this point can either be LP,
             OPB, or SMT. The file pointer is expected as an argument.
             Additionally, the target format 'lp', 'opb', or 'smt' may be
             specified (equal to 'opb' by default). Finally, supplementary
@@ -2023,14 +2154,21 @@
         # atmost constraints are initially empty
         self.atms = []
 
         # calling the base class constructor
         super(WCNFPlus, self).__init__(from_file=from_file, from_fp=from_fp,
                 from_string=from_string, comment_lead=comment_lead)
 
+    def __repr__(self):
+        """
+            State reproducible string representaion of object.
+        """
+        s = self.to_dimacs().replace('\n', '\\n')
+        return f"WCNFPlus(from_string=\"{s}\")"
+
     def from_fp(self, file_pointer, comment_lead=['c']):
         """
             Read a WCNF+ formula from a file pointer. A file pointer should be
             specified as an argument. The only default argument is
             ``comment_lead``, which can be used for parsing specific comment
             lines.
 
@@ -2164,14 +2302,51 @@
         for cl in self.hard:
             print(self.topw, ' '.join(str(l) for l in cl), '0', file=file_pointer)
 
         # atmost constraints are hard
         for am in self.atms:
             print(self.topw, ' '.join(str(l) for l in am[0]), '<=', am[1], file=file_pointer)
 
+    def to_dimacs(self):
+        """
+            Return the current state of the object in extended DIMACS format.
+
+            For example, if 'some-file.cnf' contains:
+
+            ::
+
+                c Example
+                p wcnf+ 7 3 10
+                10 1 -2 3 5 -7 <= 3
+                10 4 5 6 -7 >= 2
+                5 3 5 7 0
+
+            Then you can obtain the DIMACS with:
+
+            .. code-block:: python
+
+                >>> from pysat.formula import WCNFPlus
+                >>> cnf = WCNFPlus(from_file='some-file.cnf')
+                >>> print(cnf.to_dimacs())
+                c Example
+                p wcnf+ 7 4 10
+                10 -1 3 5 0
+                5 3 5 7 0
+                10 1 -2 3 5 -7 <= 3
+                10 -4 -5 -6 7 <= 2
+
+        """
+        header_lines = [f"p wcnf+ {self.nv} {len(self.hard)+len(self.soft)+len(self.atms)} {self.topw}"]
+        comment_lines = [f"{comment}" for comment in self.comments]
+        hard_lines = [f"{self.topw} " + " ".join(map(str,clause)) + " 0" for clause in self.hard]
+        soft_lines = [f"{weight} " + " ".join(map(str,clause)) + " 0" for clause, weight in zip(self.soft, self.wght)]
+        atmost_lines = [f"{self.topw} " + " ".join(map(str,clause)) + " <= " + str(most) for clause, most in self.atms]
+        lines = "\n".join(comment_lines + header_lines + hard_lines + soft_lines + atmost_lines) + "\n"
+        return lines
+
     def to_alien(self, file_pointer, format='opb', comments=None):
         """
             The method can be used to dump a WCNF+ formula into a file pointer
             in an alien file format, which at this point can either be LP,
             OPB, or SMT. The file pointer is expected as an argument.
             Additionally, the target format 'lp', 'opb', or 'smt' may be
             specified (equal to 'opb' by default). Finally, supplementary
```

### Comparing `python-sat-0.1.8.dev3/pysat/pb.py` & `python-sat-0.1.8.dev4/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/pysat/process.py` & `python-sat-0.1.8.dev4/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/pysat/solvers.py` & `python-sat-0.1.8.dev4/pysat/solvers.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev4/python_sat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev3
+Version: 0.1.8.dev4
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev3/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev4/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/setup.py` & `python-sat-0.1.8.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev4/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev4/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev4/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev4/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev4/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/maplechrono.zip` & `python-sat-0.1.8.dev4/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/maplecm.zip` & `python-sat-0.1.8.dev4/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/maplesat.zip` & `python-sat-0.1.8.dev4/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev4/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev4/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev4/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/minisatgh.zip` & `python-sat-0.1.8.dev4/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev4/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev4/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev4/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev4/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev4/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev4/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev4/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev4/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev4/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev4/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev4/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev4/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev4/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev4/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/prepare.py` & `python-sat-0.1.8.dev4/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/solvers/pysolvers.cc` & `python-sat-0.1.8.dev4/solvers/pysolvers.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_accum_stats.py` & `python-sat-0.1.8.dev4/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_atmost1.py` & `python-sat-0.1.8.dev4/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_atmostk.py` & `python-sat-0.1.8.dev4/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_cnfplus.py` & `python-sat-0.1.8.dev4/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_equals1.py` & `python-sat-0.1.8.dev4/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_process.py` & `python-sat-0.1.8.dev4/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_unique_model.py` & `python-sat-0.1.8.dev4/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_unique_mus.py` & `python-sat-0.1.8.dev4/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev3/tests/test_warmstart.py` & `python-sat-0.1.8.dev4/tests/test_warmstart.py`

 * *Files identical despite different names*

