# Comparing `tmp/adsorption_file_parser-0.2.2.tar.gz` & `tmp/adsorption_file_parser-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsorption_file_parser-0.2.2.tar", last modified: Tue Oct 11 21:58:08 2022, max compression
+gzip compressed data, was "adsorption_file_parser-0.2.4.tar", last modified: Wed May 24 22:46:54 2023, max compression
```

## Comparing `adsorption_file_parser-0.2.2.tar` & `adsorption_file_parser-0.2.4.tar`

### file list

```diff
@@ -1,157 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.230159 adsorption_file_parser-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.202159 adsorption_file_parser-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.202159 adsorption_file_parser-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.202159 adsorption_file_parser-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.github/workflows/CI-CD.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-10-11 21:58:08.234159 adsorption_file_parser-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3431 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-10-11 21:58:08.234159 adsorption_file_parser-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.198159 adsorption_file_parser-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.202159 adsorption_file_parser-0.2.2/src/adsorption_file_parser/
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-11 21:58:08.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4755 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_dat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_excel.py
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/mic_excel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7997 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/qnt_txt.py
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/smsdvs_excel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/trp_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.206159 adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7144 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/unit_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.206159 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-10-11 21:58:08.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-10-11 21:58:08.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 21:58:08.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-11 21:58:08.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-11 21:58:08.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 21:57:53.000000 adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.206159 adsorption_file_parser-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.198159 adsorption_file_parser-0.2.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.210159 adsorption_file_parser-0.2.2/tests/data/3p/
--rw-r--r--   0 runner    (1001) docker     (121)    18274 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json
--rw-r--r--   0 runner    (1001) docker     (121)  1637702 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/3p/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.222159 adsorption_file_parser-0.2.2/tests/data/bel/
--rw-r--r--   0 runner    (1001) docker     (121)     5858 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/1.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    18337 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/1.json
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv
--rw-r--r--   0 runner    (1001) docker     (121)    12989 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json
--rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14915 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json
--rw-r--r--   0 runner    (1001) docker     (121)     8024 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv
--rw-r--r--   0 runner    (1001) docker     (121)    24728 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/CEP 3xx-2-B 120529.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     7768 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/CEP 3xx-2-B 120529.json
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-13-CH4-190K.csv
--rw-r--r--   0 runner    (1001) docker     (121)    15593 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-13-CH4-190K.json
--rw-r--r--   0 runner    (1001) docker     (121)     4451 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    13778 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K.json
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K_run2.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    13205 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K_run2.json
--rw-r--r--   0 runner    (1001) docker     (121)    14934 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-32-N2_77K(BelMax).csv
--rw-r--r--   0 runner    (1001) docker     (121)    45816 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-32-N2_77K(BelMax).json
--rw-r--r--   0 runner    (1001) docker     (121)     8180 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_Ar_87K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    26746 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_Ar_87K.json
--rw-r--r--   0 runner    (1001) docker     (121)     5343 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_N2_77K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    16663 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_N2_77K.json
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_273K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    16078 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_273K.json
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    14399 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67-N2_77K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    11182 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67-N2_77K.json
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_DCM_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_DCM_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_EtOH_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     4740 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_EtOH_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     5367 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_H2O_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_H2O_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_MeOH_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     5209 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_MeOH_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_acetone_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     6959 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_acetone_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_hexane_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     3961 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_hexane_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_isopropanol_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_isopropanol_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_toluol_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_toluol_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_wasser_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    14967 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_wasser_298K.json
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-8_zn_etoh_298k.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     7454 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/DUT-8_zn_etoh_298k.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Sample_C.json
--rw-r--r--   0 runner    (1001) docker     (121)    37376 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Sample_C.xls
--rw-r--r--   0 runner    (1001) docker     (121)    17421 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Sample_D.json
--rw-r--r--   0 runner    (1001) docker     (121)    63488 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Sample_D.xls
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Sample_E.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/bel/Sample_E.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.226159 adsorption_file_parser-0.2.2/tests/data/mic/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12912 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_A.json
--rw-r--r--   0 runner    (1001) docker     (121)   224768 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_A.xls
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_B.json
--rw-r--r--   0 runner    (1001) docker     (121)    28672 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_B.xls
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_C.json
--rw-r--r--   0 runner    (1001) docker     (121)    59904 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_C.xls
--rw-r--r--   0 runner    (1001) docker     (121)     7334 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_D.json
--rw-r--r--   0 runner    (1001) docker     (121)    57856 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_D.xls
--rw-r--r--   0 runner    (1001) docker     (121)     7905 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_E.json
--rw-r--r--   0 runner    (1001) docker     (121)    54784 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_E.xls
--rw-r--r--   0 runner    (1001) docker     (121)     7334 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_F.json
--rw-r--r--   0 runner    (1001) docker     (121)    57856 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_F.xls
--rw-r--r--   0 runner    (1001) docker     (121)    16359 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_G.json
--rw-r--r--   0 runner    (1001) docker     (121)   275456 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_G.xls
--rw-r--r--   0 runner    (1001) docker     (121)     8008 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_H.json
--rw-r--r--   0 runner    (1001) docker     (121)   153600 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_H.xls
--rw-r--r--   0 runner    (1001) docker     (121)    15139 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_I.json
--rw-r--r--   0 runner    (1001) docker     (121)    98816 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_I.xls
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_J.json
--rw-r--r--   0 runner    (1001) docker     (121)    61952 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_J.xls
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_K.json
--rw-r--r--   0 runner    (1001) docker     (121)    58880 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_K.xls
--rw-r--r--   0 runner    (1001) docker     (121)    20566 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_L.json
--rw-r--r--   0 runner    (1001) docker     (121)   270848 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/mic/Sample_L.xls
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.230159 adsorption_file_parser-0.2.2/tests/data/qnt/
--rw-r--r--   0 runner    (1001) docker     (121)    11990 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (121)     8451 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)    11086 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)    21541 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (121)    15455 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)    14624 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (121)    10413 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)    17699 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (121)    12720 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/RE-22 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/RE-22 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/qnt/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 21:58:08.230159 adsorption_file_parser-0.2.2/tests/data/smsdvs/
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/smsdvs/13X water 30c.json
--rw-r--r--   0 runner    (1001) docker     (121)    26372 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/smsdvs/13X water 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json
--rw-r--r--   0 runner    (1001) docker     (121)    26328 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/smsdvs/Takeda 5A water 30c.json
--rw-r--r--   0 runner    (1001) docker     (121)    18697 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/data/smsdvs/Takeda 5A water 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/test_3p.py
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/test_bel.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/test_mic.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/test_qnt.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/test_smsdvs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-10-11 21:57:43.000000 adsorption_file_parser-0.2.2/tests/test_unit_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.940466 adsorption_file_parser-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.900466 adsorption_file_parser-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.900466 adsorption_file_parser-0.2.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.900466 adsorption_file_parser-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.github/workflows/CI-CD.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-24 22:46:54.940466 adsorption_file_parser-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-24 22:46:54.940466 adsorption_file_parser-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.900466 adsorption_file_parser-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.904466 adsorption_file_parser-0.2.4/src/adsorption_file_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 22:46:54.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/mic_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/qnt_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/smsdvs_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/trp_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.904466 adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/unit_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.904466 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-24 22:46:54.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-24 22:46:54.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:46:54.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 22:46:54.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 22:46:54.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:46:40.000000 adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.908466 adsorption_file_parser-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.900466 adsorption_file_parser-0.2.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.912466 adsorption_file_parser-0.2.4/tests/data/3p/
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1637702 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/3p/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.928466 adsorption_file_parser-0.2.4/tests/data/bel/
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/1.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/200819-2_jis.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/200819-2_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/CEP 3xx-2-B 120529.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/CEP 3xx-2-B 120529.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-13-CH4-190K.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-13-CH4-190K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K_run2.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K_run2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-32-N2_77K(BelMax).csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-32-N2_77K(BelMax).json
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_Ar_87K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_Ar_87K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_N2_77K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_N2_77K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_273K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_273K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67-N2_77K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67-N2_77K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_DCM_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_DCM_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_EtOH_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_EtOH_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_H2O_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_H2O_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_MeOH_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_MeOH_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_acetone_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_acetone_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_hexane_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_hexane_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_isopropanol_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_isopropanol_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_toluol_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_toluol_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_wasser_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_wasser_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-8_zn_etoh_298k.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/DUT-8_zn_etoh_298k.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Sample_C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37376 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Sample_C.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Sample_D.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63488 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Sample_D.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Sample_E.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/bel/Sample_E.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.936466 adsorption_file_parser-0.2.4/tests/data/mic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_A.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224768 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_A.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_B.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_B.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59904 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_C.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_D.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57856 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_D.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_E.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54784 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_E.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57856 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_F.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_G.json
+-rw-r--r--   0 runner    (1001) docker     (123)   275456 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_G.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_H.json
+-rw-r--r--   0 runner    (1001) docker     (123)   153600 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_H.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_I.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_I.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61952 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_J.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_K.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58880 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_K.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_L.json
+-rw-r--r--   0 runner    (1001) docker     (123)   270848 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_L.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_M.json
+-rw-r--r--   0 runner    (1001) docker     (123)    62464 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_M.xls
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_N.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241152 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/mic/Sample_N.xls
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.940466 adsorption_file_parser-0.2.4/tests/data/qnt/
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/RE-22 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/RE-22 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/qnt/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:46:54.940466 adsorption_file_parser-0.2.4/tests/data/smsdvs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/smsdvs/13X water 30c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/smsdvs/13X water 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26328 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/smsdvs/Takeda 5A water 30c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/data/smsdvs/Takeda 5A water 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/test_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/test_bel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/test_mic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/test_qnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/test_smsdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-24 22:46:31.000000 adsorption_file_parser-0.2.4/tests/test_unit_parser.py
```

### Comparing `adsorption_file_parser-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `adsorption_file_parser-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/.github/workflows/CI-CD.yaml` & `adsorption_file_parser-0.2.4/.github/workflows/CI-CD.yaml`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/.gitignore` & `adsorption_file_parser-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/LICENSE` & `adsorption_file_parser-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/PKG-INFO` & `adsorption_file_parser-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsorption_file_parser
-Version: 0.2.2
+Version: 0.2.4
 Summary: Collection of parsers for (nearly) all commercial adsorption instrumentation.
 Home-page: https://github.com/AIF-development-team/adsorption-file-parser
 Author: AIF Dev Team
 Author-email: mail@pauliacomi.com
 License: MIT license
 Project-URL: Source Code, https://github.com/AIF-development-team/adsorption-file-parser
 Keywords: adsorption,characterization,porous materials,isotherms,sorption
```

### Comparing `adsorption_file_parser-0.2.2/README.rst` & `adsorption_file_parser-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/pyproject.toml` & `adsorption_file_parser-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/setup.cfg` & `adsorption_file_parser-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/__init__.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_common.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_common.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_csv.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_csv.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_dat.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_dat.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/bel_excel.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/bel_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/mic_excel.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/mic_excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,14 +195,16 @@
     # Abstract this sort of thing
     header = sheet.cell(row + header_row, final_column).value.lower()
     header_options = []
     for option in _DATA_DICT.values():
         header_options.extend(option['text'])
     while any(header.startswith(label) for label in header_options):
         final_column += 1
+        if final_column > sheet.ncols - 1:
+            break
         header = sheet.cell(row + header_row, final_column).value.lower()
 
     if col == final_column:
         # this means no header exists, can happen in some older files
         # the units might not be standard! TODO should check
         logger.warning('Default data headers supplied for file.')
         return [
@@ -262,18 +264,22 @@
         final_row = row + rowc
     else:
         start_row = row + (rowc + 1)
         final_row = row + (rowc + 1)
     point = sheet.cell(final_row, col).value
     while point:
         final_row += 1
+        if final_row > sheet.nrows - 1:
+            break
         point = sheet.cell(final_row, col).value
         # sometimes 1-row gaps are left for P0 measurement
         if not point:
             final_row += 1
+            if final_row > sheet.nrows - 1:
+                break
             point = sheet.cell(final_row, col).value
     return [
         sheet.cell(i, col).value for i in range(start_row, final_row) if sheet.cell(i, col).value
     ]
 
 
 def _parse_errors(sheet, row, col):
```

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/qnt_txt.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/qnt_txt.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/smsdvs_excel.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/smsdvs_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/trp_excel.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/trp_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/common_utils.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/unit_parsing.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/unit_parsing.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser/utils/units.py` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser/utils/units.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/PKG-INFO` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsorption-file-parser
-Version: 0.2.2
+Version: 0.2.4
 Summary: Collection of parsers for (nearly) all commercial adsorption instrumentation.
 Home-page: https://github.com/AIF-development-team/adsorption-file-parser
 Author: AIF Dev Team
 Author-email: mail@pauliacomi.com
 License: MIT license
 Project-URL: Source Code, https://github.com/AIF-development-team/adsorption-file-parser
 Keywords: adsorption,characterization,porous materials,isotherms,sorption
```

### Comparing `adsorption_file_parser-0.2.2/src/adsorption_file_parser.egg-info/SOURCES.txt` & `adsorption_file_parser-0.2.4/src/adsorption_file_parser.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 tests/test_smsdvs.py
 tests/test_unit_parser.py
 tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json
 tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx
 tests/data/3p/README.txt
 tests/data/bel/1.DAT
 tests/data/bel/1.json
+tests/data/bel/200819-2_jis.DAT
+tests/data/bel/200819-2_jis.json
 tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv
 tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json
 tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv
 tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json
 tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv
 tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json
 tests/data/bel/CEP 3xx-2-B 120529.DAT
@@ -116,14 +118,18 @@
 tests/data/mic/Sample_I.xls
 tests/data/mic/Sample_J.json
 tests/data/mic/Sample_J.xls
 tests/data/mic/Sample_K.json
 tests/data/mic/Sample_K.xls
 tests/data/mic/Sample_L.json
 tests/data/mic/Sample_L.xls
+tests/data/mic/Sample_M.json
+tests/data/mic/Sample_M.xls
+tests/data/mic/Sample_N.json
+tests/data/mic/Sample_N.xls
 tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json
 tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt
 tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json
 tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt
 tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json
 tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt
 tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json
```

### Comparing `adsorption_file_parser-0.2.2/tests/conftest.py` & `adsorption_file_parser-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json` & `adsorption_file_parser-0.2.4/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx` & `adsorption_file_parser-0.2.4/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/1.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/1.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/1.json` & `adsorption_file_parser-0.2.4/tests/data/bel/1.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv` & `adsorption_file_parser-0.2.4/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json` & `adsorption_file_parser-0.2.4/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv` & `adsorption_file_parser-0.2.4/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json` & `adsorption_file_parser-0.2.4/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv` & `adsorption_file_parser-0.2.4/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json` & `adsorption_file_parser-0.2.4/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/CEP 3xx-2-B 120529.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/CEP 3xx-2-B 120529.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/CEP 3xx-2-B 120529.json` & `adsorption_file_parser-0.2.4/tests/data/bel/CEP 3xx-2-B 120529.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-13-CH4-190K.csv` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-13-CH4-190K.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-13-CH4-190K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-13-CH4-190K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K_run2.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K_run2.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-13_CH4_111K_run2.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-13_CH4_111K_run2.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-32-N2_77K(BelMax).csv` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-32-N2_77K(BelMax).csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-32-N2_77K(BelMax).json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-32-N2_77K(BelMax).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_Ar_87K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_Ar_87K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_Ar_87K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_Ar_87K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_N2_77K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_N2_77K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_N2_77K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_N2_77K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_273K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_273K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_273K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_273K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-49_nbutane_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-49_nbutane_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67-N2_77K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67-N2_77K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67-N2_77K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67-N2_77K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_DCM_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_DCM_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_DCM_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_DCM_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_EtOH_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_EtOH_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_EtOH_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_EtOH_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_H2O_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_H2O_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_H2O_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_H2O_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_MeOH_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_MeOH_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_MeOH_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_MeOH_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_acetone_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_acetone_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_acetone_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_acetone_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_hexane_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_hexane_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_hexane_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_hexane_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_isopropanol_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_isopropanol_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_isopropanol_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_isopropanol_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_toluol_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_toluol_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_toluol_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_toluol_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_wasser_298K.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_wasser_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-67_wasser_298K.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-67_wasser_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-8_zn_etoh_298k.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-8_zn_etoh_298k.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/DUT-8_zn_etoh_298k.json` & `adsorption_file_parser-0.2.4/tests/data/bel/DUT-8_zn_etoh_298k.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Sample_C.json` & `adsorption_file_parser-0.2.4/tests/data/bel/Sample_C.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Sample_C.xls` & `adsorption_file_parser-0.2.4/tests/data/bel/Sample_C.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Sample_D.json` & `adsorption_file_parser-0.2.4/tests/data/bel/Sample_D.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Sample_D.xls` & `adsorption_file_parser-0.2.4/tests/data/bel/Sample_D.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Sample_E.DAT` & `adsorption_file_parser-0.2.4/tests/data/bel/Sample_E.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/bel/Sample_E.json` & `adsorption_file_parser-0.2.4/tests/data/bel/Sample_E.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_A.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_A.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_A.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_A.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_B.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_B.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_B.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_B.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_C.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_C.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_C.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_C.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_D.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_D.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_D.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_D.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_E.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_E.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_E.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_E.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_F.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_F.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_F.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_F.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_G.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_G.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_G.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_G.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_H.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_H.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_H.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_H.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_I.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_I.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_I.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_I.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_J.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_J.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_J.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_J.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_K.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_K.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_K.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_L.json` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_L.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/mic/Sample_L.xls` & `adsorption_file_parser-0.2.4/tests/data/mic/Sample_L.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.4/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.4/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.4/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.4/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.4/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.4/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.4/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.4/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.4/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.4/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/RE-22 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.4/tests/data/qnt/RE-22 (Raw Analysis Data).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/qnt/RE-22 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.4/tests/data/qnt/RE-22 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/smsdvs/13X water 30c.json` & `adsorption_file_parser-0.2.4/tests/data/smsdvs/13X water 30c.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/smsdvs/13X water 30c.xlsx` & `adsorption_file_parser-0.2.4/tests/data/smsdvs/13X water 30c.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json` & `adsorption_file_parser-0.2.4/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx` & `adsorption_file_parser-0.2.4/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/smsdvs/Takeda 5A water 30c.json` & `adsorption_file_parser-0.2.4/tests/data/smsdvs/Takeda 5A water 30c.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/data/smsdvs/Takeda 5A water 30c.xlsx` & `adsorption_file_parser-0.2.4/tests/data/smsdvs/Takeda 5A water 30c.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/test_3p.py` & `adsorption_file_parser-0.2.4/tests/test_3p.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/test_bel.py` & `adsorption_file_parser-0.2.4/tests/test_bel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/test_mic.py` & `adsorption_file_parser-0.2.4/tests/test_mic.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import adsorption_file_parser as afp
 
 from .conftest import DATA_MIC_XL
 from .conftest import RECREATE
 
 
 class TestMicromeritics():
-    """Test parsing of Micromeritics files"""
+    """Test parsing of Micromeritics files."""
     @pytest.mark.parametrize('path', DATA_MIC_XL)
     def test_read_excel_mic(self, path):
         """Test reading of micromeritics report files."""
         meta, data = afp.read(path=path, manufacturer='mic', fmt='xl')
         result_dict = {'meta': meta, 'data': data}
         json_path = path.with_suffix('.json')
```

### Comparing `adsorption_file_parser-0.2.2/tests/test_qnt.py` & `adsorption_file_parser-0.2.4/tests/test_qnt.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/test_smsdvs.py` & `adsorption_file_parser-0.2.4/tests/test_smsdvs.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.2/tests/test_unit_parser.py` & `adsorption_file_parser-0.2.4/tests/test_unit_parser.py`

 * *Files identical despite different names*

