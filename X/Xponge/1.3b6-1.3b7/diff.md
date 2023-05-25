# Comparing `tmp/Xponge-1.3b6.tar.gz` & `tmp/Xponge-1.3b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xponge-1.3b6.tar", last modified: Mon Feb 20 16:20:56 2023, max compression
+gzip compressed data, was "Xponge-1.3b7.tar", last modified: Wed Feb 22 23:30:30 2023, max compression
```

## Comparing `Xponge-1.3b6.tar` & `Xponge-1.3b7.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.785852 Xponge-1.3b6/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      804 2023-02-10 12:40:23.000000 Xponge-1.3b6/LICENSE
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     8276 2023-02-20 16:20:56.785852 Xponge-1.3b6/PKG-INFO
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     7956 2023-01-31 01:27:17.000000 Xponge-1.3b6/README.md
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.689851 Xponge-1.3b6/Xponge/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     7422 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    10712 2023-01-30 00:45:13.000000 Xponge-1.3b6/Xponge/__main__.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.689851 Xponge-1.3b6/Xponge/analysis/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1462 2023-01-30 00:45:13.000000 Xponge-1.3b6/Xponge/analysis/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    19842 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/analysis/md_analysis.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.697851 Xponge-1.3b6/Xponge/assign/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    42988 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/assign/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    17838 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/assign/bond_order.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      825 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/assign/gasteiger.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    13682 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/assign/resp.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    26741 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/build.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.701851 Xponge-1.3b6/Xponge/forcefield/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        0 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/__init__.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.741851 Xponge-1.3b6/Xponge/forcefield/amber/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    10962 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/OL15.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    48836 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/RNA.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   223650 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/RSFF2C.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3395 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3899 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/atomic_ions.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    48238 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/bsc1.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1796 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/bsc1.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    24570 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ff14SB.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   128338 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ff14SB.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3842 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ff14sb.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   137234 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ff19SB.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   128338 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ff19SB.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3936 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/ff19sb.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   497800 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/gaff.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    34227 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/gaff.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   536359 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/gaff2.dat
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.757851 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    65808 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/GLYCAM_06j.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1451 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   226197 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_furanose.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1972 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_furanose.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)  1045201 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_pyranose.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2311 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_pyranose.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    15635 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/glycoprotein.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1749 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/glycoprotein.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   226197 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_furanose.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1980 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_furanose.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)  1045201 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_pyranose.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2319 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_pyranose.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      822 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/terminal.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1523 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ions1lm_126_spce.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1523 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ions1lm_126_tip3p.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1568 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ions1lm_126_tip4pew.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     4949 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ions234lm_126_spce.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     4949 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ions234lm_126_tip3p.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     5096 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ions234lm_126_tip4pew.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      948 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ionsjc_spce.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      946 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ionsjc_tip3p.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      949 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ionsjc_tip4pew.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    25672 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/lipid14.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    53829 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/lipid14.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2205 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/lipid14.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    36564 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/lipid17.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   100128 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/lipid17.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2424 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/lipid17.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    48238 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/ol15.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1984 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/ol15.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1926 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/ol3.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      551 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/opc.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3025 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/opc.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    59507 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/parm10.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    65714 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/parm19.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     5979 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/amber/parmbsc1.frcmod
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     4073 2023-01-30 00:45:13.000000 Xponge-1.3b6/Xponge/forcefield/amber/rsff2c.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      477 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/spce.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2736 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/spce.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      477 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/tip3p.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2767 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/tip3p.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1600 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/tip4p.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      551 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/amber/tip4pew.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3053 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/forcefield/amber/tip4pew.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.757851 Xponge-1.3b6/Xponge/forcefield/base/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        0 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2760 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/angle_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2633 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/bond_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1800 2023-02-07 02:06:23.000000 Xponge-1.3b6/Xponge/forcefield/base/charge_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2122 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/base/cmap_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     6265 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/dihedral_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3730 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/exclude_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2821 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/improper_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     7788 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/lj_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      897 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/mass_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3758 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/nb14_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     5239 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/nb14_extra_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1274 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/soft_bond_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1911 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/ub_angle_base.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1430 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/base/virtual_atom_base.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.765852 Xponge-1.3b6/Xponge/forcefield/charmm27/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1827 2022-10-08 14:48:23.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      301 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/atomic_ions.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    38297 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/cmap.itp
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    71114 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/ffbonded.itp
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   134978 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/ffnonbonded.itp
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      768 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/forcefield.itp
--rw-rw-r--   0 dhx       (1000) dhx       (1000)   126888 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/protein.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3821 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/protein.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      477 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/tip3p.mol2
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1271 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/tip3p.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1073 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/charmm27/tips3p.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.765852 Xponge-1.3b6/Xponge/forcefield/special/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        0 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/special/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    29993 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/forcefield/special/fep.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3848 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/special/gb.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2316 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/forcefield/special/min.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.765852 Xponge-1.3b6/Xponge/forcefield/sybyl/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     6265 2023-02-10 12:40:23.000000 Xponge-1.3b6/Xponge/forcefield/sybyl/__init__.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.765852 Xponge-1.3b6/Xponge/helper/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    87080 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/helper/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     5286 2023-01-31 01:27:17.000000 Xponge-1.3b6/Xponge/helper/math.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     7015 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/helper/namespace.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     4615 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/helper/rdkit.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    44234 2023-01-31 03:13:01.000000 Xponge-1.3b6/Xponge/load.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.769852 Xponge-1.3b6/Xponge/mdrun/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        9 2023-02-13 02:49:32.000000 Xponge-1.3b6/Xponge/mdrun/BIN_PATH.dat
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     2165 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/mdrun/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)      183 2022-10-06 14:01:35.000000 Xponge-1.3b6/Xponge/mdrun/__main__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    33045 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/process.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.769852 Xponge-1.3b6/Xponge/tools/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)    26787 2023-02-20 15:14:24.000000 Xponge-1.3b6/Xponge/tools/__init__.py
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     3633 2023-02-17 03:48:48.000000 Xponge-1.3b6/Xponge/tools/ti.py
-drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-20 16:20:56.689851 Xponge-1.3b6/Xponge.egg-info/
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     8276 2023-02-20 16:20:56.000000 Xponge-1.3b6/Xponge.egg-info/PKG-INFO
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     4291 2023-02-20 16:20:56.000000 Xponge-1.3b6/Xponge.egg-info/SOURCES.txt
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        1 2023-02-20 16:20:56.000000 Xponge-1.3b6/Xponge.egg-info/dependency_links.txt
--rw-rw-r--   0 dhx       (1000) dhx       (1000)       90 2023-02-20 16:20:56.000000 Xponge-1.3b6/Xponge.egg-info/entry_points.txt
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        6 2023-02-20 16:20:56.000000 Xponge-1.3b6/Xponge.egg-info/requires.txt
--rw-rw-r--   0 dhx       (1000) dhx       (1000)        7 2023-02-20 16:20:56.000000 Xponge-1.3b6/Xponge.egg-info/top_level.txt
--rw-rw-r--   0 dhx       (1000) dhx       (1000)       38 2023-02-20 16:20:56.785852 Xponge-1.3b6/setup.cfg
--rw-rw-r--   0 dhx       (1000) dhx       (1000)     1165 2023-02-20 15:14:24.000000 Xponge-1.3b6/setup.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.478190 Xponge-1.3b7/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      804 2023-02-10 12:40:23.000000 Xponge-1.3b7/LICENSE
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     8276 2023-02-22 23:30:30.478190 Xponge-1.3b7/PKG-INFO
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     7956 2023-01-31 01:27:17.000000 Xponge-1.3b7/README.md
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.406189 Xponge-1.3b7/Xponge/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     7422 2023-02-22 01:14:37.000000 Xponge-1.3b7/Xponge/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    10687 2023-02-22 22:53:39.000000 Xponge-1.3b7/Xponge/__main__.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.406189 Xponge-1.3b7/Xponge/analysis/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1462 2023-01-30 00:45:13.000000 Xponge-1.3b7/Xponge/analysis/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    19842 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/analysis/md_analysis.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.410189 Xponge-1.3b7/Xponge/assign/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    44319 2023-02-22 01:14:37.000000 Xponge-1.3b7/Xponge/assign/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    17838 2023-02-20 15:14:24.000000 Xponge-1.3b7/Xponge/assign/bond_order.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      825 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/assign/gasteiger.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    13682 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/assign/resp.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    26741 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/build.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.414189 Xponge-1.3b7/Xponge/forcefield/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        0 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/__init__.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.458189 Xponge-1.3b7/Xponge/forcefield/amber/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    10962 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/OL15.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    48836 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/RNA.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   223650 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/RSFF2C.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3395 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3899 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/atomic_ions.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    48238 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/bsc1.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1796 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/bsc1.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    24570 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ff14SB.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   128338 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ff14SB.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3842 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ff14sb.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   137234 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ff19SB.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   128338 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ff19SB.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3936 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/ff19sb.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   497800 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/gaff.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    34227 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/gaff.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   536359 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/gaff2.dat
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.470189 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    65808 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/GLYCAM_06j.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1451 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   226197 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_furanose.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1972 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_furanose.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)  1045201 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_pyranose.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2311 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_pyranose.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    15635 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/glycoprotein.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1749 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/glycoprotein.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   226197 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_furanose.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1980 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_furanose.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)  1045201 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_pyranose.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2319 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_pyranose.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      822 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/terminal.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1523 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ions1lm_126_spce.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1523 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ions1lm_126_tip3p.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1568 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ions1lm_126_tip4pew.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     4949 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ions234lm_126_spce.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     4949 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ions234lm_126_tip3p.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     5096 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ions234lm_126_tip4pew.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      948 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ionsjc_spce.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      946 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ionsjc_tip3p.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      949 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ionsjc_tip4pew.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    25672 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/lipid14.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    53829 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/lipid14.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2205 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/lipid14.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    36564 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/lipid17.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   100128 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/lipid17.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2424 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/lipid17.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    48238 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/ol15.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1984 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/ol15.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1926 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/ol3.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      551 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/opc.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3025 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/opc.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    59507 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/parm10.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    65714 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/parm19.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     5979 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/amber/parmbsc1.frcmod
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     4073 2023-01-30 00:45:13.000000 Xponge-1.3b7/Xponge/forcefield/amber/rsff2c.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      477 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/spce.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2736 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/spce.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      477 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/tip3p.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2767 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/tip3p.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1600 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/tip4p.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      551 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/amber/tip4pew.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3053 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/forcefield/amber/tip4pew.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.470189 Xponge-1.3b7/Xponge/forcefield/base/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        0 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2760 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/angle_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2633 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/bond_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1800 2023-02-07 02:06:23.000000 Xponge-1.3b7/Xponge/forcefield/base/charge_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2122 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/base/cmap_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     6265 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/dihedral_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3730 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/exclude_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2821 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/improper_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     7788 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/lj_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      897 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/mass_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3758 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/nb14_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     5239 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/nb14_extra_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1274 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/soft_bond_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1911 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/ub_angle_base.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1430 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/base/virtual_atom_base.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.474190 Xponge-1.3b7/Xponge/forcefield/charmm27/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1827 2022-10-08 14:48:23.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      301 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/atomic_ions.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    38297 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/cmap.itp
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    71114 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/ffbonded.itp
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   134978 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/ffnonbonded.itp
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      768 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/forcefield.itp
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)   126888 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/protein.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3821 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/protein.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      477 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/tip3p.mol2
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1271 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/tip3p.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1073 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/charmm27/tips3p.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.474190 Xponge-1.3b7/Xponge/forcefield/special/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        0 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/special/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    29993 2023-02-20 15:14:24.000000 Xponge-1.3b7/Xponge/forcefield/special/fep.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3848 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/special/gb.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2316 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/forcefield/special/min.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.474190 Xponge-1.3b7/Xponge/forcefield/sybyl/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     6265 2023-02-10 12:40:23.000000 Xponge-1.3b7/Xponge/forcefield/sybyl/__init__.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.478190 Xponge-1.3b7/Xponge/helper/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    87080 2023-02-20 15:14:24.000000 Xponge-1.3b7/Xponge/helper/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     5286 2023-01-31 01:27:17.000000 Xponge-1.3b7/Xponge/helper/math.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     7015 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/helper/namespace.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     4940 2023-02-22 01:14:37.000000 Xponge-1.3b7/Xponge/helper/rdkit.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    44234 2023-01-31 03:13:01.000000 Xponge-1.3b7/Xponge/load.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.478190 Xponge-1.3b7/Xponge/mdrun/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        9 2023-02-13 02:49:32.000000 Xponge-1.3b7/Xponge/mdrun/BIN_PATH.dat
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     2165 2023-02-20 15:14:24.000000 Xponge-1.3b7/Xponge/mdrun/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)      183 2022-10-06 14:01:35.000000 Xponge-1.3b7/Xponge/mdrun/__main__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    33045 2023-02-20 15:14:24.000000 Xponge-1.3b7/Xponge/process.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.478190 Xponge-1.3b7/Xponge/tools/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)    26656 2023-02-22 22:53:39.000000 Xponge-1.3b7/Xponge/tools/__init__.py
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     3633 2023-02-17 03:48:48.000000 Xponge-1.3b7/Xponge/tools/ti.py
+drwxrwxr-x   0 dhx       (1000) dhx       (1000)        0 2023-02-22 23:30:30.406189 Xponge-1.3b7/Xponge.egg-info/
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     8276 2023-02-22 23:30:30.000000 Xponge-1.3b7/Xponge.egg-info/PKG-INFO
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     4291 2023-02-22 23:30:30.000000 Xponge-1.3b7/Xponge.egg-info/SOURCES.txt
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        1 2023-02-22 23:30:30.000000 Xponge-1.3b7/Xponge.egg-info/dependency_links.txt
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)       90 2023-02-22 23:30:30.000000 Xponge-1.3b7/Xponge.egg-info/entry_points.txt
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        6 2023-02-22 23:30:30.000000 Xponge-1.3b7/Xponge.egg-info/requires.txt
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)        7 2023-02-22 23:30:30.000000 Xponge-1.3b7/Xponge.egg-info/top_level.txt
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)       38 2023-02-22 23:30:30.478190 Xponge-1.3b7/setup.cfg
+-rw-rw-r--   0 dhx       (1000) dhx       (1000)     1165 2023-02-20 15:14:24.000000 Xponge-1.3b7/setup.py
```

### Comparing `Xponge-1.3b6/LICENSE` & `Xponge-1.3b7/LICENSE`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/PKG-INFO` & `Xponge-1.3b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xponge
-Version: 1.3b6
+Version: 1.3b7
 Summary: A Python package to perform pre- and post-processing of molecular simulations
 Home-page: https://gitee.com/gao_hyp_xyj_admin/xponge
 Author: Yijie Xia
 Author-email: yijiexia@pku.edu.cn
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `Xponge-1.3b6/README.md` & `Xponge-1.3b7/README.md`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/__init__.py` & `Xponge-1.3b7/Xponge/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 The atoms in a ``Residue`` or a ``ResidueType`` can be obtained by their names. For example::
 
     import Xponge.forcefield.amber.ff14sb
     print(ALA.CA)
 
 """
 
-__version__ = "1.3b6"
+__version__ = "1.3b7"
 
 import os
 import time
 import sys
 from collections import OrderedDict, deque
 from itertools import product, permutations
```

### Comparing `Xponge-1.3b6/Xponge/__main__.py` & `Xponge-1.3b7/Xponge/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,16 +130,16 @@
                          help="the residue index of the molecule to mutate")
     mol2rfe.add_argument("-nl", "-lambda_numbers", metavar=20, type=int, default=20,
                          help="the number of lambda groups - 1, default 20 for 0, 0.05, 0.10, 0.15..., 1.0")
 
     mol2rfe.add_argument("-dohmr", "-do_hydrogen_mass_repartition", action="store_true",
                          help="use the hydrogen mass repartition method")
     mol2rfe.add_argument("-ff", "-forcefield", help="Use this force field file instead of the default ff14SB and gaff")
-    mol2rfe.add_argument("-mi", "-min_mdin", nargs="*", help="Use the minimization mdin file(s) here \
-instead of the default ones")
+    mol2rfe.add_argument("-mi", "-min_mdin", nargs="*", help="Use this minimization mdin file \
+instead of the default one")
     mol2rfe.add_argument("-pi", "-pre_equilibrium_mdin", help="Use this pre-equilibrium mdin file \
 instead of the default one")
     mol2rfe.add_argument("-ei", "-equilibrium_mdin", help="Use this equilibrium mdin file instead of the default one")
     mol2rfe.add_argument("-ai", "-analysis_mdin", help="Use this analysis mdin file instead of the default one")
     mol2rfe.add_argument("-method", default="TI", choices=["TI"], help="the method to calculate the free energy")
     mol2rfe.add_argument("-temp", default="TMP", metavar="TMP", help="the temporary file name prefix")
 
@@ -147,26 +147,25 @@
                          help="the timeout parameter for max common structure in unit of second")
     mol2rfe.add_argument("-fmcs", default="mcs.png", type=str, metavar="mcs.png",
                          help="the file name for max common structure image")
     mol2rfe.add_argument("-lmcs", default=0.0, type=float, metavar="0.0",
                          help="minimum limitation of the Tanimoto coefficient of max common structure")
     mol2rfe.add_argument("-dt", default=2e-3, type=float, metavar="dt",
                          help="the dt used for simulation when mdin is not provided")
-    mol2rfe.add_argument("-msteps", type=int, nargs=6,
-                         help="""the minimization steps for all the lambda.
- Default 5000 for each minimization simulation. There are 6 minimization simulations.""",
-                         default=[5000, 5000, 5000, 5000, 5000, 5000])
+    mol2rfe.add_argument("-mstep", "-min_step", dest="min_step", default=5000, type=int,
+                         metavar="5000",
+                         help="the minimization step used for simulation when mdin is not provided")
     mol2rfe.add_argument("-pstep", "-pre_equilibrium_step", dest="pre_equilibrium_step", default=50000, type=int,
-                         metavar="pre_equilibrium_step",
+                         metavar="50000",
                          help="the pre-equilibrium step used for simulation when mdin is not provided")
     mol2rfe.add_argument("-estep", "-equilibrium_step", dest="equilibrium_step", default=500000, type=int,
                          metavar="500000", help="the equilibrium step used for simulation when mdin is not provided")
-    mol2rfe.add_argument("-thermostat", default="middle_langevin", metavar="middle_langevin",
+    mol2rfe.add_argument("-thermostat", default="middle_langevin", metavar="middle_langevin", choices=["middle_langevin"],
                          help="the thermostat used for simulation when mdin is not provided")
-    mol2rfe.add_argument("-barostat", default="andersen_barostat", metavar="andersen_barostat",
+    mol2rfe.add_argument("-barostat", default="andersen_barostat", metavar="andersen_barostat", choices=["andersen_barostat"],
                          help="the barostat used for simulation when mdin is not provided")
 
     mol2rfe.set_defaults(func=tools.mol2rfe)
 
 
 def main():
     """
```

### Comparing `Xponge-1.3b6/Xponge/analysis/__init__.py` & `Xponge-1.3b7/Xponge/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/analysis/md_analysis.py` & `Xponge-1.3b7/Xponge/analysis/md_analysis.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/assign/__init__.py` & `Xponge-1.3b7/Xponge/assign/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,16 +371,23 @@
 
     def add_index_to_name(self):
         """
         This **function** renames the atoms by adding the index to the element name
 
         :return: None
         """
+        count = Xdict()
         for i in range(self.atom_numbers):
-            self.names[i] = self.atoms[i] + str(i)
+            atom_name = self.names[i] if self.names[i] else self.atoms[i]
+            if atom_name not in count:
+                count[atom_name] = 0
+            else:
+                count[atom_name] += 1
+                atom_name += f"{count[atom_name]}"
+            self.names[i] = atom_name
 
     def atom_judge(self, atom, string):
         """
         This **function** helps judge whether the atom belongs to the mask. For example, "O2" means an oxygen atom \
 connected to two other atoms, "N4" means a nitrogen atom connected to four other atoms.
 
         :param atom: the index of the atom
@@ -482,14 +489,51 @@
         if not only1:
             self.bond_marker[atom2][atom1].add(marker)
             if marker in self.atom_marker[atom2]:
                 self.atom_marker[atom2][marker] += 1
             else:
                 self.atom_marker[atom2][marker] = 1
 
+    def delete_atom(self, atom):
+        """
+        This **function** deletes the atom
+
+        :param atom: the index of the atom to delete
+        :return: None
+        """
+        assert 0 <= atom < self.atom_numbers
+        self.built = False
+        self.element_details.pop(atom)
+        self.atoms.pop(atom)
+        self.names.pop(atom)
+        self.atom_types.pop(atom)
+        self.coordinate = np.delete(self.coordinate, atom, 0)
+        self.charge = np.delete(self.charge, atom, 0)
+        self.formal_charge.pop(atom)
+        self.atom_numbers -= 1
+        bond = self.bonds.pop(atom)
+        for btom in range(atom + 1, self.atom_numbers + 1):
+            self.bonds[btom - 1] = self.bonds[btom]
+        for btom in range(self.atom_numbers):
+            self.bond_marker[btom] = Xdict()
+            self.atom_marker[btom] = Xdict()
+        new_bonds = deepcopy(self.bonds)
+        for btom, bond in new_bonds.items():
+            for ctom in bond:
+                if ctom > atom:
+                    self.bonds[btom].pop(ctom, None)
+                    self.bonds[btom][ctom-1] = new_bonds[btom][ctom]
+                    self.bond_marker[btom][ctom-1] = set([])
+                elif ctom == atom:
+                    self.bonds[btom].pop(ctom)
+                else:
+                    self.bond_marker[btom][ctom-1] = set([])
+        self.bonds.pop(self.atom_numbers)
+
+
     def delete_bond(self, atom1, atom2):
         """
         This **function** deletes the bond between two atoms
 
         :param atom1: the index of the first atom
         :param atom2: the index of the the second atom
         :return: None
@@ -520,17 +564,19 @@
         :return: None
         """
         self.rings = _RING.get_rings(self)
         _RING.add_rings_basic_marker(self, self.rings)
         _RING.check_rings_type(self, self.rings)
 
         for atom in range(len(self.atoms)):
+            self.atom_marker[atom].clear()
             dlo = 0
             noto = 0
             for atom2, order in self.bonds[atom].items():
+                self.bond_marker[atom][atom2].clear()
                 if self.Atom_Judge(atom2, "O1"):
                     dlo += 1
                 else:
                     noto += 1
             if dlo >= 1 >= noto:
                 for atom2, order in self.bonds[atom].items():
                     if self.Atom_Judge(atom2, "O1"):
@@ -643,28 +689,17 @@
         """
         temp = ResidueType(name=name)
         if not charge:
             if self.charge is None:
                 charge = np.zeros(self.atom_numbers)
             else:
                 charge = self.charge
-        count = Xdict()
+        self.add_index_to_name()
         for i in range(self.atom_numbers):
-            assert self.atom_types[i] is not None
-            if self.names[i]:
-                atom_name = self.names[i]
-            elif self.atoms[i] in count.keys():
-                atom_name = self.atoms[i] + "%d" % count[self.atoms[i]]
-                self.names[i] = atom_name
-                count[self.atoms[i]] += 1
-            else:
-                count[self.atoms[i]] = 1
-                atom_name = self.atoms[i]
-                self.names[i] = atom_name
-            temp.Add_Atom(atom_name, self.atom_types[i], x=self.coordinate[i][0],
+            temp.Add_Atom(self.names[i], self.atom_types[i], x=self.coordinate[i][0],
                           y=self.coordinate[i][1], z=self.coordinate[i][2])
             temp.atoms[-1].charge = charge[i]
         for i, bondi in self.bonds.items():
             for j in bondi.keys():
                 temp.Add_Connectivity(temp.atoms[i], temp.atoms[j])
         set_real_global_variable(name, temp)
         return temp
```

### Comparing `Xponge-1.3b6/Xponge/assign/bond_order.py` & `Xponge-1.3b7/Xponge/assign/bond_order.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/assign/gasteiger.py` & `Xponge-1.3b7/Xponge/assign/gasteiger.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/assign/resp.py` & `Xponge-1.3b7/Xponge/assign/resp.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/build.py` & `Xponge-1.3b7/Xponge/build.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/OL15.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/OL15.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/RNA.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/RNA.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/RSFF2C.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/RSFF2C.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/__init__.py` & `Xponge-1.3b7/Xponge/forcefield/amber/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/atomic_ions.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/atomic_ions.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/bsc1.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/bsc1.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/bsc1.py` & `Xponge-1.3b7/Xponge/forcefield/amber/bsc1.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ff14SB.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ff14SB.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ff14SB.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/ff14SB.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ff14sb.py` & `Xponge-1.3b7/Xponge/forcefield/amber/ff14sb.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ff19SB.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ff19SB.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ff19SB.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/ff19SB.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ff19sb.py` & `Xponge-1.3b7/Xponge/forcefield/amber/ff19sb.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/gaff.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/gaff.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/gaff.py` & `Xponge-1.3b7/Xponge/forcefield/amber/gaff.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/gaff2.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/gaff2.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/GLYCAM_06j.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/GLYCAM_06j.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/__init__.py` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_furanose.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_furanose.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_furanose.py` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_furanose.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_pyranose.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_pyranose.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/d_pyranose.py` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/d_pyranose.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/glycoprotein.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/glycoprotein.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/glycoprotein.py` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/glycoprotein.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_furanose.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_furanose.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_furanose.py` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_furanose.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_pyranose.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_pyranose.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/l_pyranose.py` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/l_pyranose.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/glycam_06j/terminal.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/glycam_06j/terminal.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ions1lm_126_spce.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ions1lm_126_spce.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ions1lm_126_tip3p.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ions1lm_126_tip3p.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ions1lm_126_tip4pew.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ions1lm_126_tip4pew.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ions234lm_126_spce.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ions234lm_126_spce.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ions234lm_126_tip3p.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ions234lm_126_tip3p.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ions234lm_126_tip4pew.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ions234lm_126_tip4pew.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ionsjc_spce.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ionsjc_spce.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ionsjc_tip3p.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ionsjc_tip3p.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ionsjc_tip4pew.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/ionsjc_tip4pew.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/lipid14.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/lipid14.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/lipid14.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/lipid14.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/lipid14.py` & `Xponge-1.3b7/Xponge/forcefield/amber/lipid14.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/lipid17.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/lipid17.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/lipid17.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/lipid17.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/lipid17.py` & `Xponge-1.3b7/Xponge/forcefield/amber/lipid17.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ol15.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/ol15.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ol15.py` & `Xponge-1.3b7/Xponge/forcefield/amber/ol15.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/ol3.py` & `Xponge-1.3b7/Xponge/forcefield/amber/ol3.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/opc.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/opc.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/opc.py` & `Xponge-1.3b7/Xponge/forcefield/amber/opc.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/parm10.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/parm10.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/parm19.dat` & `Xponge-1.3b7/Xponge/forcefield/amber/parm19.dat`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/parmbsc1.frcmod` & `Xponge-1.3b7/Xponge/forcefield/amber/parmbsc1.frcmod`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/rsff2c.py` & `Xponge-1.3b7/Xponge/forcefield/amber/rsff2c.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/spce.py` & `Xponge-1.3b7/Xponge/forcefield/amber/spce.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/tip3p.py` & `Xponge-1.3b7/Xponge/forcefield/amber/tip3p.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/tip4p.py` & `Xponge-1.3b7/Xponge/forcefield/amber/tip4p.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/tip4pew.mol2` & `Xponge-1.3b7/Xponge/forcefield/amber/tip4pew.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/amber/tip4pew.py` & `Xponge-1.3b7/Xponge/forcefield/amber/tip4pew.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/angle_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/angle_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/bond_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/bond_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/charge_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/charge_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/cmap_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/cmap_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/dihedral_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/dihedral_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/exclude_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/exclude_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/improper_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/improper_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/lj_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/lj_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/mass_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/mass_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/nb14_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/nb14_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/nb14_extra_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/nb14_extra_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/soft_bond_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/soft_bond_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/ub_angle_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/ub_angle_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/base/virtual_atom_base.py` & `Xponge-1.3b7/Xponge/forcefield/base/virtual_atom_base.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/__init__.py` & `Xponge-1.3b7/Xponge/forcefield/charmm27/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/cmap.itp` & `Xponge-1.3b7/Xponge/forcefield/charmm27/cmap.itp`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/ffbonded.itp` & `Xponge-1.3b7/Xponge/forcefield/charmm27/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/ffnonbonded.itp` & `Xponge-1.3b7/Xponge/forcefield/charmm27/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/forcefield.itp` & `Xponge-1.3b7/Xponge/forcefield/charmm27/forcefield.itp`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/protein.mol2` & `Xponge-1.3b7/Xponge/forcefield/charmm27/protein.mol2`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/protein.py` & `Xponge-1.3b7/Xponge/forcefield/charmm27/protein.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/tip3p.py` & `Xponge-1.3b7/Xponge/forcefield/charmm27/tip3p.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/charmm27/tips3p.py` & `Xponge-1.3b7/Xponge/forcefield/charmm27/tips3p.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/special/fep.py` & `Xponge-1.3b7/Xponge/forcefield/special/fep.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/special/gb.py` & `Xponge-1.3b7/Xponge/forcefield/special/gb.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/special/min.py` & `Xponge-1.3b7/Xponge/forcefield/special/min.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/forcefield/sybyl/__init__.py` & `Xponge-1.3b7/Xponge/forcefield/sybyl/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/helper/__init__.py` & `Xponge-1.3b7/Xponge/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/helper/math.py` & `Xponge-1.3b7/Xponge/helper/math.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/helper/namespace.py` & `Xponge-1.3b7/Xponge/helper/namespace.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/helper/rdkit.py` & `Xponge-1.3b7/Xponge/helper/rdkit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 try:
     from rdkit import Chem
 except ModuleNotFoundError as exc:
     raise ModuleNotFoundError(
         "'rdkit' package needed. Maybe you need 'conda install -c rdkit rdkit'") from exc
 
-from . import Xdict
+from . import Xdict, Xprint
 from .namespace import set_global_alternative_names
 
 
 def assign_to_rdmol(assign, ignore_bond_type=False):
     """
     This **function** is used to convert an Xponge.Assign to a RDKit.rdMol
 
@@ -58,27 +58,35 @@
     assign = Assign()
 
     for atom in rdmol.GetAtoms():
         x, y, z = rdmol.GetConformer().GetAtomPosition(atom.GetIdx())
         assign.add_atom(atom.GetSymbol(), x=x, y=y, z=z)
         assign.formal_charge[-1] = atom.GetFormalCharge()
 
+    has_unknown_bond = False
     for bond in rdmol.GetBonds():
         temp_bond = bond.GetBondType()
         if temp_bond == Chem.BondType.UNSPECIFIED:
             temp_bond = -1
         elif temp_bond == Chem.BondType.SINGLE:
             temp_bond = 1
         elif temp_bond == Chem.BondType.DOUBLE:
             temp_bond = 2
         elif temp_bond == Chem.BondType.TRIPLE:
             temp_bond = 3
+        elif temp_bond == Chem.BondType.AROMATIC:
+            temp_bond = -1
+            has_unknown_bond = True
         else:
+            Xprint(f"Unknown bond type {temp_bond}", "ERROR")
             raise NotImplementedError
         assign.add_bond(bond.GetBeginAtomIdx(), bond.GetEndAtomIdx(), temp_bond)
+    assign.determine_ring_and_bond_type()
+    if has_unknown_bond:
+        assign.determine_bond_order()
 
     return assign
 
 def insert_atom_type_to_rdmol(mol, res, assign, atom_type_dict=None):
     """
     This **function** inserts the atom types in the force field to the RDKit.rdmol instance.
     This is done by setting the isotope of the atom, so it may not be compatible with the other packages.
```

### Comparing `Xponge-1.3b6/Xponge/load.py` & `Xponge-1.3b7/Xponge/load.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/mdrun/__init__.py` & `Xponge-1.3b7/Xponge/mdrun/__init__.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/process.py` & `Xponge-1.3b7/Xponge/process.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge/tools/__init__.py` & `Xponge-1.3b7/Xponge/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,65 +547,59 @@
             lambda_ = i / args.nl
             basic += f" -mode minimization -lambda_lj {lambda_} -cutoff 8 -write_information_interval 1000"
             basic += _mol2rfe_output_path("min", i, args.temp)
             dt_factor = 1e-4 + 1e-2 * random()
             inc_rate = 1 + random()
             if not args.mi:
                 cif = " -minimization_dynamic_dt 1"
-                exit_code = run(f"{basic} {cif} -step_limit {args.msteps[0]} -minimization_dt_factor {dt_factor} -minimization_dt_increasing_rate {inc_rate}")
+                exit_code = run(f"{basic} {cif} -step_limit {args.min_step} -minimization_dt_factor {dt_factor} -minimization_dt_increasing_rate {inc_rate}")
                 out = MdoutReader(f"{i}/min/{args.temp}.mdout").potential[-1]
                 min_time = 0
                 while (out > 0 or exit_code != 0) and min_time < 10:
                     dt_factor = 1e-4 + 1e-2 * random()
                     inc_rate = 1 + random() 
                     Xprint("Minimization will be repeated to reduce the potential to 0", "WARNING")
                     min_time += 1
-                    exit_code = run(f"{basic} {cif} -step_limit {args.msteps[0]}  -minimization_dt_factor {dt_factor} -minimization_dt_increasing_rate {inc_rate} -coordinate_in_file {i}/min/{args.temp}_coordinate.txt")
+                    exit_code = run(f"{basic} {cif} -step_limit {args.min_step}  -minimization_dt_factor {dt_factor} -minimization_dt_increasing_rate {inc_rate}")
                     out = MdoutReader(f"{i}/min/{args.temp}.mdout").potential[-1]
                 if min_time >= 10:
                     Xprint("Minimization has been repeated for 10 times and the potential still can not be reduced to 0", "ERROR")
                     sys.exit(1)
             else:
-                mdin = args.mi.pop(0)
-                cif = ""
-                run(f"{basic} {cif} -mdin {mdin}")
-                cif += " -coordinate_in_file {1}/min/{0}_coordinate.txt".format(args.temp, i)
-                for mdin in args.mi:
-                    run(f"{basic} {cif} -mdin {mdin}")
+                command += f" -mdin {args.mi}"
+                exit_code = run(command)
 
 
 def _mol2rfe_pre_equilibrium(args):
     """
 
     :param args:
     :return:
     """
     source("..")
-    from Xponge.analysis import MdoutReader
 
     if "pre_equilibrium" in args.do:
         for i in range(args.nl + 1):
             if os.path.exists("%d/pre_equilibrium" % i):
                 shutil.rmtree("%d/pre_equilibrium" % i)
             os.mkdir("%d/pre_equilibrium" % i)
             command = f"SPONGE -default_in_file_prefix {i}/{args.temp}"
             lambda_ = i / args.nl
             command += f" -lambda_lj {lambda_} -cutoff 8"
             command += _mol2rfe_output_path("pre_equilibrium", i, args.temp)
-
             command += f" -coordinate_in_file {i}/min/{args.temp}_coordinate.txt"
             if not args.pi:
                 command += f" -mode NPT -step_limit {args.pre_equilibrium_step} -dt {args.dt} -constrain_mode SHAKE"
-                command += f" -barostat {args.barostat} -thermostat {args.thermostat}"
+                command += f" -barostat andersen_barostat -thermostat middle_langevin -middle_langevin_gamma 10 -middle_langevin_velocity_max 20"
                 exit_code = run(command)
             else:
                 command += f" -mdin {args.pi}"
                 exit_code = run(command)
             if exit_code != 0:
-                Xprint(f"The command of lambda {i} exited with code {exit_code}", "ERROR")
+                Xprint(f"The pre_equilibrium of lambda {i} exited with code {exit_code}", "ERROR")
                 sys.exit(exit_code)
 
 
 def _mol2rfe_equilibrium(args):
     """
 
     :param args:
@@ -618,18 +612,18 @@
             if os.path.exists("%d/equilibrium" % i):
                 os.system("rm -rf %d/equilibrium" % i)
             os.mkdir("%d/equilibrium" % i)
             command = f"SPONGE -default_in_file_prefix {i}/{args.temp}"
             lambda_ = i / args.nl
             command += f" -lambda_lj {lambda_} -cutoff 8 -molecule_map_output 0"
             command += _mol2rfe_output_path("equilibrium", i, args.temp)
-            command += f" -coordinate_in_file {i}/pre_equilibrium/{args.temp}_coordinate.txt"
+            command += f" -coordinate_in_file {i}/pre_equilibrium/{args.temp}_coordinate.txt -velocity_in_file {i}/pre_equilibrium/{args.temp}_velocity.txt"
             if not args.ei:
                 command += f" -mode NPT -step_limit {args.equilibrium_step} -dt {args.dt} -constrain_mode SHAKE"
-                command += f" -barostat {args.barostat} -thermostat {args.thermostat}"
+                command += f" -barostat andersen_barostat -thermostat middle_langevin -middle_langevin_gamma 10 -middle_langevin_velocity_max 20"
                 command += f" -write_information_interval 100 -write_restart_file_interval {args.equilibrium_step}"
                 run(command)
             else:
                 command += f" -mdin {args.pi}"
                 run(command)
```

### Comparing `Xponge-1.3b6/Xponge/tools/ti.py` & `Xponge-1.3b7/Xponge/tools/ti.py`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/Xponge.egg-info/PKG-INFO` & `Xponge-1.3b7/Xponge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xponge
-Version: 1.3b6
+Version: 1.3b7
 Summary: A Python package to perform pre- and post-processing of molecular simulations
 Home-page: https://gitee.com/gao_hyp_xyj_admin/xponge
 Author: Yijie Xia
 Author-email: yijiexia@pku.edu.cn
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `Xponge-1.3b6/Xponge.egg-info/SOURCES.txt` & `Xponge-1.3b7/Xponge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Xponge-1.3b6/setup.py` & `Xponge-1.3b7/setup.py`

 * *Files identical despite different names*

