# Comparing `tmp/horton-grid-0.0.1.tar.gz` & `tmp/horton-grid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horton-grid-0.0.1.tar", last modified: Tue May 23 15:53:18 2023, max compression
+gzip compressed data, was "horton-grid-0.0.2.tar", last modified: Thu May 25 11:16:44 2023, max compression
```

## Comparing `horton-grid-0.0.1.tar` & `horton-grid-0.0.2.tar`

### file list

```diff
@@ -1,271 +1,286 @@
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.599115 horton-grid-0.0.1/
--rw-r--r--   0 yxcheng    (501) staff       (20)     2544 2023-05-23 15:48:30.000000 horton-grid-0.0.1/.gitignore
--rw-r--r--   0 yxcheng    (501) staff       (20)      938 2023-05-22 15:47:51.000000 horton-grid-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 yxcheng    (501) staff       (20)      341 2023-05-23 15:50:37.000000 horton-grid-0.0.1/CHANGELOG.md
--rw-r--r--   0 yxcheng    (501) staff       (20)    35147 2023-05-21 14:52:28.000000 horton-grid-0.0.1/COPYING
--rw-r--r--   0 yxcheng    (501) staff       (20)      646 2023-05-23 15:47:30.000000 horton-grid-0.0.1/DEVELOPMENT.md
--rw-r--r--   0 yxcheng    (501) staff       (20)      779 2023-05-21 15:50:21.000000 horton-grid-0.0.1/HEADER
--rw-r--r--   0 yxcheng    (501) staff       (20)      123 2023-05-23 09:30:48.000000 horton-grid-0.0.1/MANIFEST.in
--rw-r--r--   0 yxcheng    (501) staff       (20)    42640 2023-05-23 15:53:18.598462 horton-grid-0.0.1/PKG-INFO
--rw-r--r--   0 yxcheng    (501) staff       (20)     1288 2023-05-23 09:46:21.000000 horton-grid-0.0.1/README.md
--rwxr-xr-x   0 yxcheng    (501) staff       (20)       75 2023-05-23 12:13:42.000000 horton-grid-0.0.1/cleancode.sh
--rw-r--r--   0 yxcheng    (501) staff       (20)     2534 2023-05-23 15:48:12.000000 horton-grid-0.0.1/pyproject.toml
--rw-r--r--   0 yxcheng    (501) staff       (20)       38 2023-05-23 15:53:18.599257 horton-grid-0.0.1/setup.cfg
--rwxr-xr-x   0 yxcheng    (501) staff       (20)     2902 2023-05-23 12:09:06.000000 horton-grid-0.0.1/setup.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.274448 horton-grid-0.0.1/src/
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.298254 horton-grid-0.0.1/src/horton_grid/
--rw-r--r--   0 yxcheng    (501) staff       (20)     1393 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/__init__.py
--rw-r--r--   0 yxcheng    (501) staff       (20)      160 2023-05-23 15:53:18.000000 horton-grid-0.0.1/src/horton_grid/_version.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    12945 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/cache.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    10939 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/cell.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     7764 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/cell.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1922 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/cell.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)      950 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/cext.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)    17345 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/cext.pyx
--rw-r--r--   0 yxcheng    (501) staff       (20)     1528 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/constants.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     2080 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/context.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     3472 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/context.py.bak
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.303825 horton-grid-0.0.1/src/horton_grid/data/
--rw-r--r--   0 yxcheng    (501) staff       (20)    15569 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/elements.csv
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.304745 horton-grid-0.0.1/src/horton_grid/data/examples/
--rwxr-xr-x   0 yxcheng    (501) staff       (20)     2153 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/examples/expectation_r.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.318955 horton-grid-0.0.1/src/horton_grid/data/grids/
--rw-r--r--   0 yxcheng    (501) staff       (20)    27767 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-3.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)    31311 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-4.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)    36583 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-5.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)    44540 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-6.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)    56040 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-7.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)    66265 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-8.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)    15117 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/references.bib
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.538064 horton-grid-0.0.1/src/horton_grid/data/test/
--rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-cc.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-ci.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-mp2.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-mp3.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      311 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)      403 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/CHGCAR.oxygen
--rw-r--r--   0 yxcheng    (501) staff       (20)      795 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/CHGCAR.water
--rw-r--r--   0 yxcheng    (501) staff       (20)    50057 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/F.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)     1622 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/FCIDUMP.molpro.h2
--rw-r--r--   0 yxcheng    (501) staff       (20)      470 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/FCIDUMP.molpro.h2-erf
--rw-r--r--   0 yxcheng    (501) staff       (20)    12745 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/FCIDUMP.psi4.h2
--rw-r--r--   0 yxcheng    (501) staff       (20)      402 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/LOCPOT.oxygen
--rw-r--r--   0 yxcheng    (501) staff       (20)      185 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/POSCAR.cubicbn_cartesian
--rw-r--r--   0 yxcheng    (501) staff       (20)      109 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/POSCAR.cubicbn_direct
--rw-r--r--   0 yxcheng    (501) staff       (20)      333 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/POSCAR.water
--rw-r--r--   0 yxcheng    (501) staff       (20)    26888 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/aelta.cube
--rw-r--r--   0 yxcheng    (501) staff       (20)     2497 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_001_001_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     2496 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_001_001_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     2260 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_001_002_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     2259 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_001_002_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3280 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_006_005_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3280 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_006_006_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3280 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_006_007_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4196 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_007_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4195 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_007_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4196 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_008_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4195 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_008_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4196 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_009_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4195 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_009_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3281 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_008_010_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3552 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_014_011_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     2879 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_014_012_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3552 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_014_013_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3552 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_014_014_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    31270 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_o.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    34024 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_om1.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    27300 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_om2.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    29326 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_op1.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    28840 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_op2.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    28241 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/atom_si.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    40364 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/benzene-sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    23477 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_ae_contracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    40688 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_ae_uncontracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    30130 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_pp_contracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    35812 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_pp_uncontracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    20949 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_ae_contracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    36105 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_ae_uncontracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    28684 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_pp_contracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)    34072 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_pp_uncontracted.cp2k.out
--rw-r--r--   0 yxcheng    (501) staff       (20)     8333 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/ch3_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     5240 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/ch3_rohf_sto3g_g03.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)  1037545 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/co_ccpv5z_cart_hf_g03.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)   548353 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/co_ccpv5z_pure_hf_g03.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    12517 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/co_pbe_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     4555 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/electron_repulsion_0_2_2_3.json
--rw-r--r--   0 yxcheng    (501) staff       (20)    35419 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/electron_repulsion_4_3_2_1.json
--rw-r--r--   0 yxcheng    (501) staff       (20)     4555 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/erf_repulsion_0_2_2_3.json
--rw-r--r--   0 yxcheng    (501) staff       (20)    35419 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/erf_repulsion_4_3_2_1.json
--rw-r--r--   0 yxcheng    (501) staff       (20)    24335 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/ethanol.mkl
--rw-r--r--   0 yxcheng    (501) staff       (20)      126 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)    91311 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2_ccpvqz.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)      607 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2_sto3g.mkl
--rw-r--r--   0 yxcheng    (501) staff       (20)    11936 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2o.molden.input
--rw-r--r--   0 yxcheng    (501) staff       (20)      149 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2o.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)    14169 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2o_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3032 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2o_sto3g.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     3034 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h2o_sto3g_decontracted.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     6002 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h3_hfs_321g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     6333 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h3_pbe_321g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     2545 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/h_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     1176 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he2_ghost_psi4_1.0.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)     9462 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_d_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      638 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_d_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     8660 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_p_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      518 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_p_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     9276 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_s_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      536 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_s_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     9372 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_s_virtual.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      958 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_s_virtual.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    10775 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_sp_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      694 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_sp_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    18495 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spd_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     1121 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spd_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    19091 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spdf_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     1151 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spdf_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    86688 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_orbital.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     2627 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    86688 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_virtual.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    56692 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_virtual.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     2041 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/helium_hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     3842 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/hf_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)       47 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/include_atomdb_cp2k_ppot.inc
--rw-r--r--   0 yxcheng    (501) staff       (20)      189 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/include_atomdb_cp2k_valence.inc
--rw-r--r--   0 yxcheng    (501) staff       (20)      177 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/include_atomdb_gaussian_basis.001_000_00
--rw-r--r--   0 yxcheng    (501) staff       (20)       19 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/include_atomdb_gaussian_basis.008_000_00
--rw-r--r--   0 yxcheng    (501) staff       (20)    62835 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/jbw_coarse_aedens.cube
--rw-r--r--   0 yxcheng    (501) staff       (20)   324639 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/li2.mkl
--rw-r--r--   0 yxcheng    (501) staff       (20)   623554 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/li2.molden.input
--rw-r--r--   0 yxcheng    (501) staff       (20)      125 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/li2.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)    10429 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/li_h_3-21G_hf_g09.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     1096 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/li_sp_orbital.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     3761 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/li_sp_virtual.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    15671 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/lif_fci.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)     6519 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/lih_cation_fci.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)      187 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/methyl.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)    15902 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/methyl_tpss_321g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    26317 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/monosilicic_acid_hf_lan.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     6088 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/n2_hfs_sto3g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)   120546 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/neon_turbomole_def2-qzvp.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    48355 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_molden_cart.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    45001 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_molden_pure.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    60017 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_molpro2012.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    68614 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_orca.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    68355 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_psi4.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    68355 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_psi4_1.0.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)    78981 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nh3_turbomole.molden
--rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-cc.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-ci.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-mp2.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-mp3.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)   126340 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/o2_cc_pvtz_cart.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    94384 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/o2_cc_pvtz_pure.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    21967 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/o2_uhf.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)   111391 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/o2_uhf_virtual.wfn
--rw-r--r--   0 yxcheng    (501) staff       (20)    15252 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/pro.atdens
--rw-r--r--   0 yxcheng    (501) staff       (20)      721 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/template_atomdb_cp2k.in
--rw-r--r--   0 yxcheng    (501) staff       (20)      137 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/template_atomdb_gaussian.in
--rw-r--r--   0 yxcheng    (501) staff       (20)       90 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/template_atomdb_orca.in
--rw-r--r--   0 yxcheng    (501) staff       (20)      141 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)    20579 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_ccpvdz_cart_hf_g03.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)    19365 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_ccpvdz_pure_hf_g03.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     9827 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_dimer_ghost.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      141 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_element.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)     8178 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_hfs_321g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     8005 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_m05_321g.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)      141 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_number.xyz
--rw-r--r--   0 yxcheng    (501) staff       (20)     5369 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/data/test/water_sto3g_hf_g03.fchk
--rw-r--r--   0 yxcheng    (501) staff       (20)     1366 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/exceptions.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.571125 horton-grid-0.0.1/src/horton_grid/grid/
--rw-r--r--   0 yxcheng    (501) staff       (20)     1176 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/__init__.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    18570 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/atgrid.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     6086 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/base.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5120 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/becke.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1116 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/becke.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1088 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/becke.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     1956 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/cext.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)    49806 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/cext.pyx
--rw-r--r--   0 yxcheng    (501) staff       (20)     9414 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/cubic_spline.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     9315 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/cubic_spline.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     2060 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/cubic_spline.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     5942 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/evaluate.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1368 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/evaluate.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1335 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/evaluate.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)   120189 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/lebedev_laikov.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1047 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/lebedev_laikov.h
--rw-r--r--   0 yxcheng    (501) staff       (20)      964 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/lebedev_laikov.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     8445 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/molgrid.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    11692 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/ode2.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1432 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/ode2.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1413 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/ode2.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     3025 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/ode2.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     3581 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/poisson.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     3038 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/radial.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5295 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/rtransform.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     8788 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/rtransform.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     2207 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/rtransform.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     5459 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/uniform.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     2281 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/uniform.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1448 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/uniform.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     5645 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/utils.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1385 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/utils.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1386 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/utils.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     3152 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/utils.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5623 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/grid/visual.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.575195 horton-grid-0.0.1/src/horton_grid/io/
--rw-r--r--   0 yxcheng    (501) staff       (20)     1382 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/io/__init__.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5419 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/io/cube.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     3583 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/io/internal.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     3644 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/io/lockedh5.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1690 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/io/utils.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     2414 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/io/xyz.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    25315 2023-05-23 12:31:49.000000 horton-grid-0.0.1/src/horton_grid/log.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     4439 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/moments.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1653 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/moments.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1179 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/moments.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)    28004 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/moments.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1555 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/nucpot.cpp
--rw-r--r--   0 yxcheng    (501) staff       (20)     1878 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/nucpot.h
--rw-r--r--   0 yxcheng    (501) staff       (20)     1061 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/nucpot.pxd
--rw-r--r--   0 yxcheng    (501) staff       (20)     9563 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/periodic.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    28186 2023-05-23 12:30:14.000000 horton-grid-0.0.1/src/horton_grid/quadprog.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     4378 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/units.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5365 2023-05-23 09:30:48.000000 horton-grid-0.0.1/src/horton_grid/utils.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.302274 horton-grid-0.0.1/src/horton_grid.egg-info/
--rw-r--r--   0 yxcheng    (501) staff       (20)    42640 2023-05-23 15:53:18.000000 horton-grid-0.0.1/src/horton_grid.egg-info/PKG-INFO
--rw-r--r--   0 yxcheng    (501) staff       (20)     9792 2023-05-23 15:53:18.000000 horton-grid-0.0.1/src/horton_grid.egg-info/SOURCES.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)        1 2023-05-23 15:53:18.000000 horton-grid-0.0.1/src/horton_grid.egg-info/dependency_links.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)       40 2023-05-23 15:53:18.000000 horton-grid-0.0.1/src/horton_grid.egg-info/requires.txt
--rw-r--r--   0 yxcheng    (501) staff       (20)       12 2023-05-23 15:53:18.000000 horton-grid-0.0.1/src/horton_grid.egg-info/top_level.txt
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.583795 horton-grid-0.0.1/tests/
--rw-r--r--   0 yxcheng    (501) staff       (20)      840 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/__init__.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    11856 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/common.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.595535 horton-grid-0.0.1/tests/grid/
--rw-r--r--   0 yxcheng    (501) staff       (20)     7304 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/2
--rw-r--r--   0 yxcheng    (501) staff       (20)      840 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/__init__.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1406 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/common.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    13985 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_atgrid.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    15394 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_base.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     2896 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_becke.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    14988 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_cubic_spline.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1861 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_lebedev_laikov.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5938 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_molgrid.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    16353 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_ode2.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     7453 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_poisson.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1756 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_radial.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    11094 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_rtransform.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     5014 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_uniform.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1349 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_utils.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     2398 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/grid/test_visual.py
-drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-23 15:53:18.597199 horton-grid-0.0.1/tests/io/
--rw-r--r--   0 yxcheng    (501) staff       (20)      840 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/io/__init__.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     2281 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/io/test_lockedh5.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     8471 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_cache.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    14070 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_cell.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     4041 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_context.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1134 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_log.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     9712 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_moments.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     4155 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_periodic.py
--rw-r--r--   0 yxcheng    (501) staff       (20)    72935 2023-05-23 12:29:47.000000 horton-grid-0.0.1/tests/test_quadprog.py
--rw-r--r--   0 yxcheng    (501) staff       (20)     1641 2023-05-23 09:30:48.000000 horton-grid-0.0.1/tests/test_utils.py
--rwxr-xr-x   0 yxcheng    (501) staff       (20)     4161 2023-05-23 09:30:48.000000 horton-grid-0.0.1/updateheaders.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.968759 horton-grid-0.0.2/
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2544 2023-05-23 15:48:30.000000 horton-grid-0.0.2/.gitignore
+-rw-r--r--   0 yxcheng    (501) staff       (20)      938 2023-05-22 15:47:51.000000 horton-grid-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 yxcheng    (501) staff       (20)      407 2023-05-25 11:15:25.000000 horton-grid-0.0.2/CHANGELOG.md
+-rw-r--r--   0 yxcheng    (501) staff       (20)    35147 2023-05-21 14:52:28.000000 horton-grid-0.0.2/COPYING
+-rw-r--r--   0 yxcheng    (501) staff       (20)      646 2023-05-23 15:47:30.000000 horton-grid-0.0.2/DEVELOPMENT.md
+-rw-r--r--   0 yxcheng    (501) staff       (20)      779 2023-05-21 15:50:21.000000 horton-grid-0.0.2/HEADER
+-rw-r--r--   0 yxcheng    (501) staff       (20)      123 2023-05-23 09:30:48.000000 horton-grid-0.0.2/MANIFEST.in
+-rw-r--r--   0 yxcheng    (501) staff       (20)    42640 2023-05-25 11:16:44.968267 horton-grid-0.0.2/PKG-INFO
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1288 2023-05-23 09:46:21.000000 horton-grid-0.0.2/README.md
+-rwxr-xr-x   0 yxcheng    (501) staff       (20)      110 2023-05-25 11:15:25.000000 horton-grid-0.0.2/cleancode.sh
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2534 2023-05-25 08:47:24.000000 horton-grid-0.0.2/pyproject.toml
+-rw-r--r--   0 yxcheng    (501) staff       (20)       38 2023-05-25 11:16:44.968859 horton-grid-0.0.2/setup.cfg
+-rwxr-xr-x   0 yxcheng    (501) staff       (20)     3480 2023-05-25 11:15:25.000000 horton-grid-0.0.2/setup.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.762652 horton-grid-0.0.2/src/
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.795184 horton-grid-0.0.2/src/horton_grid/
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1427 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)      160 2023-05-25 11:16:44.000000 horton-grid-0.0.2/src/horton_grid/_version.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    12945 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/cache.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    10939 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/cell.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     7764 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/cell.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1922 2023-05-25 08:20:17.000000 horton-grid-0.0.2/src/horton_grid/cell.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)      950 2023-05-25 08:15:10.000000 horton-grid-0.0.2/src/horton_grid/cext.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)    17345 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/cext.pyx
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1528 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/constants.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2080 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/context.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3472 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/context.py.bak
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.799685 horton-grid-0.0.2/src/horton_grid/data/
+-rw-r--r--   0 yxcheng    (501) staff       (20)    15569 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/elements.csv
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.800690 horton-grid-0.0.2/src/horton_grid/data/examples/
+-rwxr-xr-x   0 yxcheng    (501) staff       (20)     2153 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/examples/expectation_r.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.807492 horton-grid-0.0.2/src/horton_grid/data/grids/
+-rw-r--r--   0 yxcheng    (501) staff       (20)    27767 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-3.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)    31311 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-4.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)    36583 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-5.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)    44540 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-6.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)    56040 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-7.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)    66265 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-8.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)    15117 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/references.bib
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.917213 horton-grid-0.0.2/src/horton_grid/data/test/
+-rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-cc.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-ci.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-mp2.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    42617 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-mp3.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      311 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)      403 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/CHGCAR.oxygen
+-rw-r--r--   0 yxcheng    (501) staff       (20)      795 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/CHGCAR.water
+-rw-r--r--   0 yxcheng    (501) staff       (20)    50057 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/F.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1622 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/FCIDUMP.molpro.h2
+-rw-r--r--   0 yxcheng    (501) staff       (20)      470 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/FCIDUMP.molpro.h2-erf
+-rw-r--r--   0 yxcheng    (501) staff       (20)    12745 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/FCIDUMP.psi4.h2
+-rw-r--r--   0 yxcheng    (501) staff       (20)      402 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/LOCPOT.oxygen
+-rw-r--r--   0 yxcheng    (501) staff       (20)      185 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/POSCAR.cubicbn_cartesian
+-rw-r--r--   0 yxcheng    (501) staff       (20)      109 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/POSCAR.cubicbn_direct
+-rw-r--r--   0 yxcheng    (501) staff       (20)      333 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/POSCAR.water
+-rw-r--r--   0 yxcheng    (501) staff       (20)    26888 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/aelta.cube
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2497 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_001_001_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2496 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_001_001_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2260 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_001_002_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2259 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_001_002_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3280 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_006_005_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3280 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_006_006_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3280 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_006_007_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4196 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_007_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4195 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_007_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4196 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_008_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4195 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_008_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4196 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_009_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4195 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_009_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3281 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_008_010_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3552 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_014_011_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2879 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_014_012_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3552 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_014_013_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3552 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_014_014_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    31270 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_o.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    34024 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_om1.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    27300 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_om2.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    29326 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_op1.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    28840 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_op2.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    28241 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/atom_si.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    40364 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/benzene-sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    23477 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_ae_contracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    40688 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_ae_uncontracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    30130 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_pp_contracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    35812 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_pp_uncontracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    20949 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_ae_contracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    36105 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_ae_uncontracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    28684 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_pp_contracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)    34072 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_pp_uncontracted.cp2k.out
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8333 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/ch3_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5240 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/ch3_rohf_sto3g_g03.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)  1037545 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/co_ccpv5z_cart_hf_g03.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)   548353 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/co_ccpv5z_pure_hf_g03.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    12517 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/co_pbe_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4555 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/electron_repulsion_0_2_2_3.json
+-rw-r--r--   0 yxcheng    (501) staff       (20)    35419 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/electron_repulsion_4_3_2_1.json
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4555 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/erf_repulsion_0_2_2_3.json
+-rw-r--r--   0 yxcheng    (501) staff       (20)    35419 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/erf_repulsion_4_3_2_1.json
+-rw-r--r--   0 yxcheng    (501) staff       (20)    24335 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/ethanol.mkl
+-rw-r--r--   0 yxcheng    (501) staff       (20)      126 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)    91311 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2_ccpvqz.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)      607 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2_sto3g.mkl
+-rw-r--r--   0 yxcheng    (501) staff       (20)    11936 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2o.molden.input
+-rw-r--r--   0 yxcheng    (501) staff       (20)      149 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2o.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)    14169 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2o_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3032 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2o_sto3g.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3034 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h2o_sto3g_decontracted.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6002 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h3_hfs_321g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6333 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h3_pbe_321g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2545 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/h_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1176 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he2_ghost_psi4_1.0.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9462 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_d_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      638 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_d_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8660 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_p_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      518 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_p_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9276 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_s_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      536 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_s_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9372 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_s_virtual.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      958 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_s_virtual.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    10775 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_sp_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      694 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_sp_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    18495 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spd_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1121 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spd_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    19091 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spdf_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1151 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spdf_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    86688 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_orbital.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2627 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    86688 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_virtual.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    56692 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_virtual.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2041 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/helium_hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3842 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/hf_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)       47 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/include_atomdb_cp2k_ppot.inc
+-rw-r--r--   0 yxcheng    (501) staff       (20)      189 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/include_atomdb_cp2k_valence.inc
+-rw-r--r--   0 yxcheng    (501) staff       (20)      177 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/include_atomdb_gaussian_basis.001_000_00
+-rw-r--r--   0 yxcheng    (501) staff       (20)       19 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/include_atomdb_gaussian_basis.008_000_00
+-rw-r--r--   0 yxcheng    (501) staff       (20)    62835 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/jbw_coarse_aedens.cube
+-rw-r--r--   0 yxcheng    (501) staff       (20)   324639 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/li2.mkl
+-rw-r--r--   0 yxcheng    (501) staff       (20)   623554 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/li2.molden.input
+-rw-r--r--   0 yxcheng    (501) staff       (20)      125 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/li2.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)    10429 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/li_h_3-21G_hf_g09.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1096 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/li_sp_orbital.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3761 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/li_sp_virtual.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    15671 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/lif_fci.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6519 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/lih_cation_fci.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)      187 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/methyl.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)    15902 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/methyl_tpss_321g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    26317 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/monosilicic_acid_hf_lan.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6088 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/n2_hfs_sto3g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)   120546 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/neon_turbomole_def2-qzvp.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    48355 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_molden_cart.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    45001 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_molden_pure.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    60017 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_molpro2012.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    68614 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_orca.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    68355 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_psi4.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    68355 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_psi4_1.0.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)    78981 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nh3_turbomole.molden
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-cc.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-ci.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-mp2.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8975 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-mp3.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)   126340 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/o2_cc_pvtz_cart.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    94384 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/o2_cc_pvtz_pure.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    21967 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/o2_uhf.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)   111391 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/o2_uhf_virtual.wfn
+-rw-r--r--   0 yxcheng    (501) staff       (20)    15252 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/pro.atdens
+-rw-r--r--   0 yxcheng    (501) staff       (20)      721 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/template_atomdb_cp2k.in
+-rw-r--r--   0 yxcheng    (501) staff       (20)      137 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/template_atomdb_gaussian.in
+-rw-r--r--   0 yxcheng    (501) staff       (20)       90 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/template_atomdb_orca.in
+-rw-r--r--   0 yxcheng    (501) staff       (20)      141 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)    20579 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_ccpvdz_cart_hf_g03.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)    19365 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_ccpvdz_pure_hf_g03.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9827 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_dimer_ghost.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      141 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_element.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8178 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_hfs_321g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8005 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_m05_321g.fchk
+-rw-r--r--   0 yxcheng    (501) staff       (20)      141 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_number.xyz
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5369 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/data/test/water_sto3g_hf_g03.fchk
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.921495 horton-grid-0.0.2/src/horton_grid/espfit/
+-rw-r--r--   0 yxcheng    (501) staff       (20)      923 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6494 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/cext.pyx
+-rw-r--r--   0 yxcheng    (501) staff       (20)     7431 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/cost.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6343 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/electrostatics.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1544 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/electrostatics.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1594 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/electrostatics.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3253 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/mask.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1312 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/mask.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1279 2023-05-25 11:15:25.000000 horton-grid-0.0.2/src/horton_grid/espfit/mask.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1366 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/exceptions.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.943278 horton-grid-0.0.2/src/horton_grid/grid/
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1176 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    18570 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/grid/atgrid.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     6086 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/grid/base.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5120 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/becke.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1116 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/becke.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1088 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/becke.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1956 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/cext.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)    49806 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/grid/cext.pyx
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9414 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/cubic_spline.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9315 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/cubic_spline.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2060 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/cubic_spline.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5942 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/evaluate.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1368 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/evaluate.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1335 2023-05-25 08:17:04.000000 horton-grid-0.0.2/src/horton_grid/grid/evaluate.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)   120189 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/lebedev_laikov.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1047 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/lebedev_laikov.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)      964 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/lebedev_laikov.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8445 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/grid/molgrid.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    11692 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/ode2.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1432 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/ode2.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1413 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/ode2.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3025 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/ode2.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3581 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/grid/poisson.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3038 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/radial.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5295 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/rtransform.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8788 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/rtransform.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2207 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/rtransform.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5459 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/uniform.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2281 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/uniform.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1448 2023-05-25 08:17:04.000000 horton-grid-0.0.2/src/horton_grid/grid/uniform.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5645 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/utils.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1385 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/utils.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1386 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/utils.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3152 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/utils.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5623 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/grid/visual.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.946777 horton-grid-0.0.2/src/horton_grid/io/
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1382 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/io/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5419 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/io/cube.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3583 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/io/internal.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3644 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/io/lockedh5.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1690 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/io/utils.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2414 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/io/xyz.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    25315 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/log.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4439 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/moments.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1653 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/moments.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1179 2023-05-25 08:20:39.000000 horton-grid-0.0.2/src/horton_grid/moments.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)    28004 2023-05-23 09:30:48.000000 horton-grid-0.0.2/src/horton_grid/moments.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1555 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/nucpot.cpp
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1878 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/nucpot.h
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1061 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/nucpot.pxd
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9563 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/periodic.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    28186 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/quadprog.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4378 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/units.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5365 2023-05-25 08:47:24.000000 horton-grid-0.0.2/src/horton_grid/utils.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.798168 horton-grid-0.0.2/src/horton_grid.egg-info/
+-rw-r--r--   0 yxcheng    (501) staff       (20)    42640 2023-05-25 11:16:44.000000 horton-grid-0.0.2/src/horton_grid.egg-info/PKG-INFO
+-rw-r--r--   0 yxcheng    (501) staff       (20)    10211 2023-05-25 11:16:44.000000 horton-grid-0.0.2/src/horton_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)        1 2023-05-25 11:16:44.000000 horton-grid-0.0.2/src/horton_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)       40 2023-05-25 11:16:44.000000 horton-grid-0.0.2/src/horton_grid.egg-info/requires.txt
+-rw-r--r--   0 yxcheng    (501) staff       (20)       12 2023-05-25 11:16:44.000000 horton-grid-0.0.2/src/horton_grid.egg-info/top_level.txt
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.954358 horton-grid-0.0.2/tests/
+-rw-r--r--   0 yxcheng    (501) staff       (20)      840 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    11856 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/common.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.956931 horton-grid-0.0.2/tests/espfit/
+-rw-r--r--   0 yxcheng    (501) staff       (20)      807 2023-05-25 11:15:25.000000 horton-grid-0.0.2/tests/espfit/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1503 2023-05-25 11:15:25.000000 horton-grid-0.0.2/tests/espfit/test_cext.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    16552 2023-05-25 11:15:25.000000 horton-grid-0.0.2/tests/espfit/test_cost.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     3524 2023-05-25 11:15:25.000000 horton-grid-0.0.2/tests/espfit/test_mask.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.965905 horton-grid-0.0.2/tests/grid/
+-rw-r--r--   0 yxcheng    (501) staff       (20)     7304 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/2
+-rw-r--r--   0 yxcheng    (501) staff       (20)      840 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1406 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/common.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    13985 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/grid/test_atgrid.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    15394 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/grid/test_base.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2896 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_becke.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    14988 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_cubic_spline.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1861 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_lebedev_laikov.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5938 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_molgrid.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    16353 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_ode2.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8810 2023-05-25 11:15:25.000000 horton-grid-0.0.2/tests/grid/test_poisson.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1756 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_radial.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    11094 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_rtransform.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     5014 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_uniform.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1349 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_utils.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2398 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/grid/test_visual.py
+drwxr-xr-x   0 yxcheng    (501) staff       (20)        0 2023-05-25 11:16:44.967267 horton-grid-0.0.2/tests/io/
+-rw-r--r--   0 yxcheng    (501) staff       (20)      840 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/io/__init__.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     2281 2023-05-23 09:30:48.000000 horton-grid-0.0.2/tests/io/test_lockedh5.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     8471 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_cache.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    14070 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_cell.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4041 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_context.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1134 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_log.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     9712 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_moments.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     4155 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_periodic.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)    72935 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_quadprog.py
+-rw-r--r--   0 yxcheng    (501) staff       (20)     1641 2023-05-25 08:47:24.000000 horton-grid-0.0.2/tests/test_utils.py
+-rwxr-xr-x   0 yxcheng    (501) staff       (20)     4161 2023-05-23 09:30:48.000000 horton-grid-0.0.2/updateheaders.py
```

### Comparing `horton-grid-0.0.1/.gitignore` & `horton-grid-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/.pre-commit-config.yaml` & `horton-grid-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/COPYING` & `horton-grid-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/DEVELOPMENT.md` & `horton-grid-0.0.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/HEADER` & `horton-grid-0.0.2/HEADER`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/PKG-INFO` & `horton-grid-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horton-grid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Molecular grids used in computational chemistry
 Author-email: YingXing Cheng <yingxing.cheng@ugent.be>, Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `horton-grid-0.0.1/README.md` & `horton-grid-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/pyproject.toml` & `horton-grid-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/setup.py` & `horton-grid-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -64,14 +64,29 @@
             "src/horton_grid/moments.pxd",
             "src/horton_grid/moments.h",
         ],
         include_dirs=[np.get_include(), "src"],
         language="c++",
         extra_compile_args=["-std=c++11"],
     ),
+    Extension(
+        "horton_grid.espfit.cext",
+        sources=get_sources("src/horton_grid/espfit"),
+        # + ["src/horton_grid/cell.cpp", "src/horton_grid/grid/uniform.cpp"],
+        depends=get_depends("src/horton_grid/espfit")
+        + [
+            "src/horton_grid/cell.pxd",
+            "src/horton_grid/cell.h",
+            "src/horton_grid/grid/uniform.pxd",
+            "src/horton_grid/grid/uniform.h",
+        ],
+        include_dirs=[np.get_include(), "src", "src/horton_grid/grid"],
+        extra_compile_args=["-std=c++11"],
+        language="c++",
+    ),
 ]
 
 for e in ext_modules:
     e.cython_directives = {"embedsignature": True}
 
 if __name__ == "__main__":
     setup(
```

### Comparing `horton-grid-0.0.1/src/horton_grid/__init__.py` & `horton-grid-0.0.2/src/horton_grid/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,7 +35,9 @@
 from horton_grid.io import *
 from horton_grid.log import *
 from horton_grid.moments import *
 from horton_grid.periodic import *
 from horton_grid.quadprog import *
 from horton_grid.units import *
 from horton_grid.utils import *
+
+from horton_grid.espfit import *
```

### Comparing `horton-grid-0.0.1/src/horton_grid/cache.py` & `horton-grid-0.0.2/src/horton_grid/cache.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/cell.cpp` & `horton-grid-0.0.2/src/horton_grid/cell.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/cell.h` & `horton-grid-0.0.2/src/horton_grid/cell.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/cell.pxd` & `horton-grid-0.0.2/src/horton_grid/cell.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/cext.pxd` & `horton-grid-0.0.2/src/horton_grid/cext.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/cext.pyx` & `horton-grid-0.0.2/src/horton_grid/cext.pyx`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/constants.py` & `horton-grid-0.0.2/src/horton_grid/constants.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/context.py` & `horton-grid-0.0.2/src/horton_grid/context.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/context.py.bak` & `horton-grid-0.0.2/src/horton_grid/context.py.bak`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/elements.csv` & `horton-grid-0.0.2/src/horton_grid/data/elements.csv`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/examples/expectation_r.py` & `horton-grid-0.0.2/src/horton_grid/data/examples/expectation_r.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-3.txt` & `horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-3.txt`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-4.txt` & `horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-4.txt`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-5.txt` & `horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-5.txt`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-6.txt` & `horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-6.txt`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-7.txt` & `horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-7.txt`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/grids/tv-13.7-8.txt` & `horton-grid-0.0.2/src/horton_grid/data/grids/tv-13.7-8.txt`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/references.bib` & `horton-grid-0.0.2/src/horton_grid/data/references.bib`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-cc.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-cc.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-ci.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-ci.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-mp2.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-mp2.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/2h-azirine-mp3.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/2h-azirine-mp3.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/CHGCAR.water` & `horton-grid-0.0.2/src/horton_grid/data/test/CHGCAR.water`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/F.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/F.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/FCIDUMP.molpro.h2` & `horton-grid-0.0.2/src/horton_grid/data/test/FCIDUMP.molpro.h2`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/FCIDUMP.psi4.h2` & `horton-grid-0.0.2/src/horton_grid/data/test/FCIDUMP.psi4.h2`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/aelta.cube` & `horton-grid-0.0.2/src/horton_grid/data/test/aelta.cube`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_001_001_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_001_001_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_001_001_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_001_001_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_001_002_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_001_002_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_001_002_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_001_002_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_006_005_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_006_005_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_006_006_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_006_006_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_006_007_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_006_007_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_007_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_007_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_007_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_007_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_008_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_008_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_008_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_008_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_009_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_009_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_009_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_009_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_008_010_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_008_010_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_014_011_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_014_011_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_014_012_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_014_012_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_014_013_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_014_013_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_014_014_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_014_014_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_o.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_o.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_om1.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_om1.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_om2.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_om2.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_op1.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_op1.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_op2.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_op2.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/atom_si.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/atom_si.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/benzene-sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/benzene-sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_ae_contracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_ae_contracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_ae_uncontracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_ae_uncontracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_pp_contracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_pp_contracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_gs_pp_uncontracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_gs_pp_uncontracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_ae_contracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_ae_contracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_ae_uncontracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_ae_uncontracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_pp_contracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_pp_contracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/carbon_sc_pp_uncontracted.cp2k.out` & `horton-grid-0.0.2/src/horton_grid/data/test/carbon_sc_pp_uncontracted.cp2k.out`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/ch3_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/ch3_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/ch3_rohf_sto3g_g03.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/ch3_rohf_sto3g_g03.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/co_ccpv5z_cart_hf_g03.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/co_ccpv5z_cart_hf_g03.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/co_ccpv5z_pure_hf_g03.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/co_ccpv5z_pure_hf_g03.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/co_pbe_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/co_pbe_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/electron_repulsion_0_2_2_3.json` & `horton-grid-0.0.2/src/horton_grid/data/test/electron_repulsion_0_2_2_3.json`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/electron_repulsion_4_3_2_1.json` & `horton-grid-0.0.2/src/horton_grid/data/test/electron_repulsion_4_3_2_1.json`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/erf_repulsion_0_2_2_3.json` & `horton-grid-0.0.2/src/horton_grid/data/test/erf_repulsion_0_2_2_3.json`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/erf_repulsion_4_3_2_1.json` & `horton-grid-0.0.2/src/horton_grid/data/test/erf_repulsion_4_3_2_1.json`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/ethanol.mkl` & `horton-grid-0.0.2/src/horton_grid/data/test/ethanol.mkl`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h2_ccpvqz.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/h2_ccpvqz.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h2_sto3g.mkl` & `horton-grid-0.0.2/src/horton_grid/data/test/h2_sto3g.mkl`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h2o.molden.input` & `horton-grid-0.0.2/src/horton_grid/data/test/h2o.molden.input`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h2o_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/h2o_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h2o_sto3g.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/h2o_sto3g.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h2o_sto3g_decontracted.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/h2o_sto3g_decontracted.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h3_hfs_321g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/h3_hfs_321g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h3_pbe_321g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/h3_pbe_321g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/h_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/h_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he2_ghost_psi4_1.0.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/he2_ghost_psi4_1.0.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_d_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_d_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_d_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_d_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_p_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_p_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_p_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_p_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_s_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_s_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_s_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_s_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_s_virtual.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_s_virtual.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_s_virtual.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_s_virtual.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_sp_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_sp_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_sp_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_sp_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spd_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spd_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spd_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spd_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spdf_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spdf_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spdf_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spdf_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_orbital.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_orbital.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_virtual.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_virtual.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/he_spdfgh_virtual.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/he_spdfgh_virtual.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/helium_hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/helium_hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/hf_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/hf_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/jbw_coarse_aedens.cube` & `horton-grid-0.0.2/src/horton_grid/data/test/jbw_coarse_aedens.cube`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/li2.mkl` & `horton-grid-0.0.2/src/horton_grid/data/test/li2.mkl`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/li2.molden.input` & `horton-grid-0.0.2/src/horton_grid/data/test/li2.molden.input`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/li_h_3-21G_hf_g09.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/li_h_3-21G_hf_g09.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/li_sp_orbital.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/li_sp_orbital.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/li_sp_virtual.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/li_sp_virtual.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/lif_fci.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/lif_fci.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/lih_cation_fci.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/lih_cation_fci.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/methyl_tpss_321g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/methyl_tpss_321g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/monosilicic_acid_hf_lan.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/monosilicic_acid_hf_lan.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/n2_hfs_sto3g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/n2_hfs_sto3g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/neon_turbomole_def2-qzvp.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/neon_turbomole_def2-qzvp.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_molden_cart.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_molden_cart.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_molden_pure.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_molden_pure.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_molpro2012.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_molpro2012.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_orca.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_orca.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_psi4.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_psi4.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_psi4_1.0.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_psi4_1.0.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nh3_turbomole.molden` & `horton-grid-0.0.2/src/horton_grid/data/test/nh3_turbomole.molden`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-cc.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-cc.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-ci.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-ci.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-mp2.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-mp2.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/nitrogen-mp3.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/nitrogen-mp3.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/o2_cc_pvtz_cart.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/o2_cc_pvtz_cart.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/o2_cc_pvtz_pure.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/o2_cc_pvtz_pure.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/o2_uhf.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/o2_uhf.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/o2_uhf_virtual.wfn` & `horton-grid-0.0.2/src/horton_grid/data/test/o2_uhf_virtual.wfn`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/pro.atdens` & `horton-grid-0.0.2/src/horton_grid/data/test/pro.atdens`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/template_atomdb_cp2k.in` & `horton-grid-0.0.2/src/horton_grid/data/test/template_atomdb_cp2k.in`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/water_ccpvdz_cart_hf_g03.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/water_ccpvdz_cart_hf_g03.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/water_ccpvdz_pure_hf_g03.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/water_ccpvdz_pure_hf_g03.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/water_dimer_ghost.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/water_dimer_ghost.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/water_hfs_321g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/water_hfs_321g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/water_m05_321g.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/water_m05_321g.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/data/test/water_sto3g_hf_g03.fchk` & `horton-grid-0.0.2/src/horton_grid/data/test/water_sto3g_hf_g03.fchk`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/exceptions.py` & `horton-grid-0.0.2/src/horton_grid/exceptions.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/__init__.py` & `horton-grid-0.0.2/src/horton_grid/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/atgrid.py` & `horton-grid-0.0.2/src/horton_grid/grid/atgrid.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/base.py` & `horton-grid-0.0.2/src/horton_grid/grid/base.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/becke.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/becke.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/becke.h` & `horton-grid-0.0.2/src/horton_grid/grid/becke.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/becke.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/becke.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/cext.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/cext.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/cext.pyx` & `horton-grid-0.0.2/src/horton_grid/grid/cext.pyx`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/cubic_spline.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/cubic_spline.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/cubic_spline.h` & `horton-grid-0.0.2/src/horton_grid/grid/cubic_spline.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/cubic_spline.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/cubic_spline.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/evaluate.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/evaluate.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/evaluate.h` & `horton-grid-0.0.2/src/horton_grid/grid/evaluate.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/evaluate.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/evaluate.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/lebedev_laikov.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/lebedev_laikov.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/lebedev_laikov.h` & `horton-grid-0.0.2/src/horton_grid/grid/lebedev_laikov.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/lebedev_laikov.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/lebedev_laikov.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/molgrid.py` & `horton-grid-0.0.2/src/horton_grid/grid/molgrid.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/ode2.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/ode2.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/ode2.h` & `horton-grid-0.0.2/src/horton_grid/grid/ode2.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/ode2.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/ode2.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/ode2.py` & `horton-grid-0.0.2/src/horton_grid/grid/ode2.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/poisson.py` & `horton-grid-0.0.2/src/horton_grid/grid/poisson.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/radial.py` & `horton-grid-0.0.2/src/horton_grid/grid/radial.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/rtransform.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/rtransform.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/rtransform.h` & `horton-grid-0.0.2/src/horton_grid/grid/rtransform.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/rtransform.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/rtransform.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/uniform.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/uniform.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/uniform.h` & `horton-grid-0.0.2/src/horton_grid/grid/uniform.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/uniform.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/uniform.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/utils.cpp` & `horton-grid-0.0.2/src/horton_grid/grid/utils.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/utils.h` & `horton-grid-0.0.2/src/horton_grid/grid/utils.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/utils.pxd` & `horton-grid-0.0.2/src/horton_grid/grid/utils.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/utils.py` & `horton-grid-0.0.2/src/horton_grid/grid/utils.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/grid/visual.py` & `horton-grid-0.0.2/src/horton_grid/grid/visual.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/io/__init__.py` & `horton-grid-0.0.2/src/horton_grid/io/__init__.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/io/cube.py` & `horton-grid-0.0.2/src/horton_grid/io/cube.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/io/internal.py` & `horton-grid-0.0.2/src/horton_grid/io/internal.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/io/lockedh5.py` & `horton-grid-0.0.2/src/horton_grid/io/lockedh5.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/io/utils.py` & `horton-grid-0.0.2/src/horton_grid/io/utils.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/io/xyz.py` & `horton-grid-0.0.2/src/horton_grid/io/xyz.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/log.py` & `horton-grid-0.0.2/src/horton_grid/log.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/moments.cpp` & `horton-grid-0.0.2/src/horton_grid/moments.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/moments.h` & `horton-grid-0.0.2/src/horton_grid/moments.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/moments.pxd` & `horton-grid-0.0.2/src/horton_grid/moments.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/moments.py` & `horton-grid-0.0.2/src/horton_grid/moments.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/nucpot.cpp` & `horton-grid-0.0.2/src/horton_grid/nucpot.cpp`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/nucpot.h` & `horton-grid-0.0.2/src/horton_grid/nucpot.h`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/nucpot.pxd` & `horton-grid-0.0.2/src/horton_grid/nucpot.pxd`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/periodic.py` & `horton-grid-0.0.2/src/horton_grid/periodic.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/quadprog.py` & `horton-grid-0.0.2/src/horton_grid/quadprog.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/units.py` & `horton-grid-0.0.2/src/horton_grid/units.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid/utils.py` & `horton-grid-0.0.2/src/horton_grid/utils.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/src/horton_grid.egg-info/PKG-INFO` & `horton-grid-0.0.2/src/horton_grid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horton-grid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Molecular grids used in computational chemistry
 Author-email: YingXing Cheng <yingxing.cheng@ugent.be>, Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `horton-grid-0.0.1/src/horton_grid.egg-info/SOURCES.txt` & `horton-grid-0.0.2/src/horton_grid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,23 @@
 src/horton_grid/data/test/water_ccpvdz_pure_hf_g03.fchk
 src/horton_grid/data/test/water_dimer_ghost.fchk
 src/horton_grid/data/test/water_element.xyz
 src/horton_grid/data/test/water_hfs_321g.fchk
 src/horton_grid/data/test/water_m05_321g.fchk
 src/horton_grid/data/test/water_number.xyz
 src/horton_grid/data/test/water_sto3g_hf_g03.fchk
+src/horton_grid/espfit/__init__.py
+src/horton_grid/espfit/cext.pyx
+src/horton_grid/espfit/cost.py
+src/horton_grid/espfit/electrostatics.cpp
+src/horton_grid/espfit/electrostatics.h
+src/horton_grid/espfit/electrostatics.pxd
+src/horton_grid/espfit/mask.cpp
+src/horton_grid/espfit/mask.h
+src/horton_grid/espfit/mask.pxd
 src/horton_grid/grid/__init__.py
 src/horton_grid/grid/atgrid.py
 src/horton_grid/grid/base.py
 src/horton_grid/grid/becke.cpp
 src/horton_grid/grid/becke.h
 src/horton_grid/grid/becke.pxd
 src/horton_grid/grid/cext.pxd
@@ -232,14 +241,18 @@
 tests/test_cell.py
 tests/test_context.py
 tests/test_log.py
 tests/test_moments.py
 tests/test_periodic.py
 tests/test_quadprog.py
 tests/test_utils.py
+tests/espfit/__init__.py
+tests/espfit/test_cext.py
+tests/espfit/test_cost.py
+tests/espfit/test_mask.py
 tests/grid/2
 tests/grid/__init__.py
 tests/grid/common.py
 tests/grid/test_atgrid.py
 tests/grid/test_base.py
 tests/grid/test_becke.py
 tests/grid/test_cubic_spline.py
```

### Comparing `horton-grid-0.0.1/tests/__init__.py` & `horton-grid-0.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/common.py` & `horton-grid-0.0.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/2` & `horton-grid-0.0.2/tests/grid/2`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/__init__.py` & `horton-grid-0.0.2/tests/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/common.py` & `horton-grid-0.0.2/tests/grid/common.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_atgrid.py` & `horton-grid-0.0.2/tests/grid/test_atgrid.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_base.py` & `horton-grid-0.0.2/tests/grid/test_base.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_becke.py` & `horton-grid-0.0.2/tests/grid/test_becke.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_cubic_spline.py` & `horton-grid-0.0.2/tests/grid/test_cubic_spline.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_lebedev_laikov.py` & `horton-grid-0.0.2/tests/grid/test_lebedev_laikov.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_molgrid.py` & `horton-grid-0.0.2/tests/grid/test_molgrid.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_ode2.py` & `horton-grid-0.0.2/tests/grid/test_ode2.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_poisson.py` & `horton-grid-0.0.2/tests/grid/test_poisson.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,30 +25,62 @@
 from nose.plugins.attrib import attr
 
 from horton_grid import *  # pylint: disable=wildcard-import,unused-wildcard-import
 
 
 # @attr("slow")
 # def test_solve_poisson_becke_n2():
-#     mol = IOData.from_file(context.get_fn("test/n2_hfs_sto3g.fchk"))
+#
+#     import importlib
+#
+#     # Check if iodata is installed
+#     if importlib.util.find_spec("iodata") is None:
+#         print("iodata package is not installed.")
+#         assert False
+#     else:
+#         # Check if gbasis is installed
+#         if importlib.util.find_spec("gbasis") is None:
+#             print("gbasis package is not installed.")
+#             assert False
+#         else:
+#             # Import necessary modules
+#             from iodata import load_one
+#             import gbasis.evals.electrostatic_potential
+#             from gbasis.evals.eval import evaluate_basis
+#             from gbasis.wrappers import from_iodata
+#
+#     mol = load_one(context.get_fn("test/n2_hfs_sto3g.fchk"))
 #     lmaxmax = 4
 #
 #     # compute hartree potential on a molecular grid
 #     molgrid = BeckeMolGrid(
-#         mol.coordinates,
-#         mol.numbers,
-#         mol.pseudo_numbers,
+#         mol.atcoords,
+#         mol.atnums,
+#         mol.atcorenums,
 #         random_rotate=False,
 #         mode="keep",
 #     )
-#     dm_full = mol.get_dm_full()
-#     reference = mol.obasis.compute_grid_hartree_dm(dm_full, molgrid.points)
+#     dm_full = mol.one_rdms.get("post_scf", mol.one_rdms.get("scf"))
+#     # dm_full = mol.get_dm_full()
+#     # reference = mol.obasis.compute_grid_hartree_dm(dm_full, molgrid.points)
+#     basis, coord_types = from_iodata(mol)
+#     # TODO: fix here
+#     reference = gbasis.evals.electrostatic_potential.electrostatic_potential(
+#         basis,
+#         dm_full,
+#         molgrid.points,
+#         mol.atcoords,
+#         mol.atnums,
+#         coord_type="cartesian",
+#     )
 #
 #     # construct the same potential numerically with Becke's method
-#     rho = mol.obasis.compute_grid_density_dm(dm_full, molgrid.points)
+#     basis_grid = evaluate_basis(basis, molgrid.points, coord_type=coord_types)
+#     rho = np.einsum("ab,bp,ap->p", dm_full, basis_grid, basis_grid, optimize=True)
+#     # rho = mol.obasis.compute_grid_density_dm(dm_full, molgrid.points)
 #     begin = 0
 #     hds = []
 #     for i in range(mol.natom):
 #         atgrid = molgrid.subgrids[i]
 #         end = begin + atgrid.size
 #         becke_weights = molgrid.becke_weights[begin:end]
 #         density_decomposition = atgrid.get_spherical_decomposition(
@@ -60,15 +92,15 @@
 #
 #     # Evaluate the splines obtained with Becke's method on the molecular grid
 #     # Increasing angular momenta are used to check the convergence.
 #     last_error = None
 #     for lmax in range(0, lmaxmax + 1):
 #         result = molgrid.zeros()
 #         for i in range(mol.natom):
-#             molgrid.eval_decomposition(hds[i][: (lmax + 1) ** 2], mol.coordinates[i], result)
+#             molgrid.eval_decomposition(hds[i][: (lmax + 1) ** 2], mol.atcoords[i], result)
 #         potential_error = result - reference
 #         error = molgrid.integrate(potential_error, potential_error) ** 0.5
 #         if last_error is not None:
 #             assert error < last_error
 #         last_error = error
 #         if False:
 #             worst = molgrid.integrate(reference, reference) ** 0.5
@@ -87,16 +119,18 @@
 #             print()
 #     assert error < 6e-2
 #
 #     if False:
 #         # Plot stuff
 #         import matplotlib.pyplot as pt
 #
-#         linegrid = LineGrid(mol.coordinates[0], mol.coordinates[1], 500, 1)
-#         rho = mol.obasis.compute_grid_density_dm(dm_full, linegrid.points)
+#         linegrid = LineGrid(mol.atcoords[0], mol.atcoords[1], 500, 1)
+#         basis_grid = evaluate_basis(basis, molgrid.points, coord_type=coord_types)
+#         rho = np.einsum("ab,bp,ap->p", one_rdm, linegrid.points, linegrid.points, optimize=True)
+#         # rho = mol.obasis.compute_grid_density_dm(dm_full, linegrid.points)
 #         reference = mol.obasis.compute_grid_hartree_dm(dm_full, linegrid.points)
 #         for lmax in range(0, lmaxmax + 1):
 #             result = linegrid.zeros()
 #             for i in range(mol.natom):
 #                 linegrid.eval_decomposition(hds[i][: (lmax + 1) ** 2], mol.coordinates[i], result)
 #             pt.clf()
 #             # pt.plot(linegrid.x, reference)
```

### Comparing `horton-grid-0.0.1/tests/grid/test_radial.py` & `horton-grid-0.0.2/tests/grid/test_radial.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_rtransform.py` & `horton-grid-0.0.2/tests/grid/test_rtransform.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_uniform.py` & `horton-grid-0.0.2/tests/grid/test_uniform.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_utils.py` & `horton-grid-0.0.2/tests/grid/test_utils.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/grid/test_visual.py` & `horton-grid-0.0.2/tests/grid/test_visual.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/io/__init__.py` & `horton-grid-0.0.2/tests/io/__init__.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/io/test_lockedh5.py` & `horton-grid-0.0.2/tests/io/test_lockedh5.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_cache.py` & `horton-grid-0.0.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_cell.py` & `horton-grid-0.0.2/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_context.py` & `horton-grid-0.0.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_log.py` & `horton-grid-0.0.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_moments.py` & `horton-grid-0.0.2/tests/test_moments.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_periodic.py` & `horton-grid-0.0.2/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_quadprog.py` & `horton-grid-0.0.2/tests/test_quadprog.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/tests/test_utils.py` & `horton-grid-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `horton-grid-0.0.1/updateheaders.py` & `horton-grid-0.0.2/updateheaders.py`

 * *Files identical despite different names*

