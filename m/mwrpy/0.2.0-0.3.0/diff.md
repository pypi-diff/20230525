# Comparing `tmp/mwrpy-0.2.0.tar.gz` & `tmp/mwrpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.2.0.tar", last modified: Tue May 16 13:55:09 2023, max compression
+gzip compressed data, was "mwrpy-0.3.0.tar", last modified: Thu May 25 10:22:43 2023, max compression
```

## Comparing `mwrpy-0.2.0.tar` & `mwrpy-0.3.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 13:54:56.000000 mwrpy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 13:54:56.000000 mwrpy-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-16 13:55:09.427990 mwrpy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-16 13:54:56.000000 mwrpy-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.419990 mwrpy-0.2.0/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.419990 mwrpy-0.2.0/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    14642 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)  1208422 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/mwrpy/site_config/lindenberg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15747 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.419990 mwrpy-0.2.0/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:55:09.427990 mwrpy-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 13:54:56.000000 mwrpy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-25 10:22:33.000000 mwrpy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 10:22:33.000000 mwrpy-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-25 10:22:43.312654 mwrpy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-25 10:22:33.000000 mwrpy-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23328 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51810 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.308654 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)  1208422 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.308654 mwrpy-0.3.0/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/mwrpy/site_config/lindenberg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-25 10:22:33.000000 mwrpy-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:22:43.312654 mwrpy-0.3.0/setup.cfg
```

### Comparing `mwrpy-0.2.0/LICENSE` & `mwrpy-0.3.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) 2023 University of Cologne
+Copyright (c) 2021-2023 University of Cologne
+Copyright (c) 2023 Finnish Meteorological Institute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mwrpy-0.2.0/mwrpy/atmos.py` & `mwrpy-0.3.0/mwrpy/atmos.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         tb[(lev1["pointing_flag"][:] == 1) | (elevation_angle[:] < 89.0)] = np.nan
         ind = utils.time_to_datetime_index(lev1["time"][:])
         tb_df = pd.DataFrame({"Tb": tb}, index=ind)
         tb_std = tb_df.rolling("2min", center=True, min_periods=10).std()
         tb_mx = tb_std.rolling("20min", center=True, min_periods=100).max()
 
         if "irt" in lev1:
-            tb_thres = 0.1
+            tb_thres = 0.15
             irt = lev1["irt"][:, :]
             irt[irt == -999.0] = np.nan
             irt = np.nanmean(irt, axis=1)
             irt[(lev1["pointing_flag"][:] == 1) | (elevation_angle[:] < 89.0)] = np.nan
             irt_df = pd.DataFrame({"Irt": irt[:]}, index=ind)
             irt_mx = irt_df.rolling("20min", center=True, min_periods=100).max()
             index[(irt_mx["Irt"] > 263.15) & (tb_mx["Tb"] > tb_thres)] = 1.0
```

### Comparing `mwrpy-0.2.0/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.3.0/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/level1/met_quality_control.py` & `mwrpy-0.3.0/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/level1/quality_control.py` & `mwrpy-0.3.0/mwrpy/level1/quality_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import ephem
 import netCDF4 as nc
 import numpy as np
 import pandas as pd
 from numpy import ma
 
-from mwrpy.level1.rpg_bin import RpgBin
 from mwrpy.level2.get_ret_coeff import get_mvr_coeff
 from mwrpy.level2.write_lev2_nc import retrieval_input
 from mwrpy.utils import get_coeff_list, read_yaml_config, setbit
 
 Fill_Value_Float = -999.0
 Fill_Value_Int = -99
 
@@ -193,14 +192,15 @@
     abs_diff = ma.masked_all(data["tb"].shape, dtype=np.float32)
     rpg_dat = {}
     rpg_dat["tb_spectrum"] = np.ones(data["tb"].shape) * np.nan
     global_attributes, _ = read_yaml_config(site)
 
     c_list = get_coeff_list(site, "spc")
     if len(c_list) > 0:
+        # pylint: disable=unbalanced-tuple-unpacking
         (
             coeff,
             input_scale,
             input_offset,
             output_scale,
             output_offset,
             weights1,
```

### Comparing `mwrpy-0.2.0/mwrpy/level1/rpg_bin.py` & `mwrpy-0.3.0/mwrpy/level1/rpg_bin.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.3.0/mwrpy/level1/write_lev1_nc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module for writing Level 1 netCDF files"""
 import datetime
+import logging
 from collections.abc import Callable
 from itertools import groupby
 from typing import TypeAlias
 
 import numpy as np
 from numpy import ma
 
@@ -65,14 +66,16 @@
     params: dict,
     site: str,
 ) -> RpgBin:
     """Load and prepare data for netCDF writing"""
 
     if data_type in ("1B01", "1C01"):
         brt_files = get_file_list(path_to_files, "BRT")
+        if len(brt_files) == 0:
+            raise FileNotFoundError("No BRT files found")
         rpg_bin = RpgBin(brt_files)
         rpg_bin.data["tb"] = rpg_bin.data["tb"][:, np.argsort(params["bandwidth"])]
         rpg_bin.data["frequency"] = rpg_bin.header["_f"][
             np.argsort(params["bandwidth"])
         ]
         fields = [
             "bandwidth",
@@ -89,15 +92,15 @@
         )
         rpg_bin.data["pointing_flag"] = np.zeros(len(rpg_bin.data["time"]), np.int32)
 
         if data_type == "1B01":
             (
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
-            ) = atmos.find_lwcl_free(rpg_bin.data, np.arange(len(rpg_bin.data["time"])))
+            ) = atmos.find_lwcl_free(rpg_bin.data)
         else:
             (
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
             ) = np.ones(len(rpg_bin.data["time"]), np.int32) * 2, np.ones(
                 len(rpg_bin.data["time"]), np.int32
             )
@@ -117,19 +120,17 @@
             rpg_hkd.data["status"][ind_hkd], params
         )
         if params["scan_time"] != Fill_Value_Int:
             file_list_bls = []
             try:
                 file_list_bls = get_file_list(path_to_files, "BLS")
             except RuntimeError:
-                print(
-                    [
-                        "No binary files with extension bls found in directory "
-                        + path_to_files
-                    ]
+                logging.error(
+                    "No binary files with extension bls found in directory "
+                    + path_to_files
                 )
             if len(file_list_bls) > 0:
                 rpg_bls = RpgBin(file_list_bls)
                 _add_bls(rpg_bin, rpg_bls, rpg_hkd, params)
             else:
                 file_list_blb = get_file_list(path_to_files, "BLB")
                 rpg_blb = RpgBin(file_list_blb)
@@ -143,15 +144,15 @@
             ) % 360
 
         if data_type == "1C01":
             if params["ir_flag"]:
                 try:
                     file_list_irt = get_file_list(path_to_files, "IRT")
                 except RuntimeError as err:
-                    print(err)
+                    logging.error(err)
                 if len(file_list_irt) > 0:
                     rpg_irt = RpgBin(file_list_irt)
                     rpg_irt.data["irt"][rpg_irt.data["irt"] <= 125.5] = Fill_Value_Float
                     rpg_bin.data["ir_wavelength"] = rpg_irt.header["_f"] * 1e-6
                     rpg_bin.data["ir_bandwidth"] = params["ir_bandwidth"] * 1e-6
                     rpg_bin.data["ir_beamwidth"] = params["ir_beamwidth"]
                     add_interpol1d(
@@ -174,15 +175,15 @@
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
             ) = atmos.find_lwcl_free(rpg_bin.data)
 
             try:
                 file_list_met = get_file_list(path_to_files, "MET")
             except RuntimeError as err:
-                print(err)
+                logging.error(err)
             rpg_met = RpgBin(file_list_met)
             add_interpol1d(
                 rpg_bin.data,
                 rpg_met.data["air_temperature"],
                 rpg_met.data["time"],
                 "air_temperature",
             )
```

### Comparing `mwrpy-0.2.0/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.3.0/mwrpy/level2/get_ret_coeff.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.3.0/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/level2/lwp_offset.py` & `mwrpy-0.3.0/mwrpy/level2/lwp_offset.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,24 +19,27 @@
 
     if "elevation_angle" in lev1:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
     lwcl_i = lev1["liquid_cloud_flag"][index]
-    lwp = np.copy(lwp_org)
-    lwp[(lwcl_i != 0) | (lwp > 0.04) | (elevation_angle[index] < 89.0)] = np.nan
     ind = utils.time_to_datetime_index(lev1["time"][index])
-    lwp_df = pd.DataFrame({"Lwp": lwp}, index=ind)
+    lwp_df = pd.DataFrame({"Lwp": lwp_org}, index=ind)
     lwp_std = lwp_df.rolling("2min", center=True, min_periods=10).std()
     lwp_max = lwp_std.rolling("20min", center=True, min_periods=100).max()
-    lwp_df[lwp_max > 0.002] = np.nan
+    lwp = np.copy(lwp_org)
+    lwp[
+        (lwcl_i != 0)
+        | (lwp > 0.04)
+        | (elevation_angle[index] < 89.0)
+        | (lwp_max["Lwp"][:] > 0.003)
+    ] = np.nan
+    lwp_df = pd.DataFrame({"Lwp": lwp}, index=ind)
     lwp_offset = lwp_df.rolling("20min", center=True, min_periods=100).mean()
 
-    if np.isnan(lwp_offset["Lwp"][-1]):
-        lwp_offset["Lwp"][-1] = 0.0
     lwp_offset = lwp_offset.interpolate(method="linear")
     lwp_offset = lwp_offset.fillna(method="bfill")
     lwp_offset["Lwp"][np.isnan(lwp_offset["Lwp"])] = 0.0
     lwp_org -= lwp_offset["Lwp"].values
 
     return lwp_org, lwp_offset["Lwp"].values
```

### Comparing `mwrpy-0.2.0/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.3.0/mwrpy/level2/write_lev2_nc.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 Fill_Value_Float = -999.0
 Fill_Value_Int = -99
 
 
 def lev2_to_nc(
     site: str,
     data_type: str,
-    lev1_path: str,
+    lev1_file: str,
     output_file: str,
     temp_file: str | None = None,
     hum_file: str | None = None,
 ):
     """This function reads Level 1 files,
     applies retrieval coefficients for Level 2 products
     and writes it into a netCDF file.
 
     Args:
         site: Name of site.
         data_type: Data type of the netCDF file.
-        lev1_path: Path of Level 1 file.
+        lev1_file: Path of Level 1 file.
         output_file: Name of output file.
         temp_file: Name of temperature product file.
         hum_file: Name of humidity product file.
 
     """
 
     if data_type not in (
@@ -52,39 +52,37 @@
         "2P03",
         "2P04",
         "2P07",
         "2P08",
         "2I01",
         "2I02",
     ):
-        raise RuntimeError(
-            ["Data type " + data_type + " not supported for file writing."]
-        )
+        raise ValueError(f"Data type {data_type} not recognised")
+
+    global_attributes, params = read_yaml_config(site)
 
-    with nc.Dataset(lev1_path) as lev1:
+    with nc.Dataset(lev1_file) as lev1:
         if data_type == "2P02":
             bl_scan = _test_bl_scan(site, lev1)
             if not bl_scan:
                 data_type = "2P01"
         if data_type in ("2P04", "2P07", "2P08"):
             bl_scan = _test_bl_scan(site, lev1)
             t_product = "2P02"
             if not bl_scan:
                 t_product = "2P01"
             for d_type in [t_product, "2P03"]:
-                global_attributes, params = read_yaml_config(site)
                 rpg_dat, coeff, index = get_products(
                     site, lev1, d_type, params, temp_file=temp_file, hum_file=hum_file
                 )
                 _combine_lev1(lev1, rpg_dat, index, d_type, params)
                 hatpro = rpg_mwr.Rpg(rpg_dat)
                 hatpro.data = get_data_attributes(hatpro.data, d_type)
                 rpg_mwr.save_rpg(hatpro, output_file, global_attributes, d_type)
 
-        global_attributes, params = read_yaml_config(site)
         rpg_dat, coeff, index = get_products(
             site, lev1, data_type, params, temp_file=temp_file, hum_file=hum_file
         )
         _combine_lev1(lev1, rpg_dat, index, data_type, params)
         _add_att(global_attributes, coeff)
         hatpro = rpg_mwr.Rpg(rpg_dat)
         hatpro.data = get_data_attributes(hatpro.data, data_type)
@@ -105,25 +103,23 @@
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
     rpg_dat, coeff, index = {}, {}, np.empty(0)
 
     if data_type in ("2I01", "2I02"):
-        if data_type == "2I01":
-            product = "lwp"
-        else:
-            product = "iwv"
+        product = "lwp" if data_type == "2I01" else "iwv"
 
         coeff = get_mvr_coeff(site, product, lev1["frequency"][:])
         if coeff[0]["RT"] < 2:
             coeff, offset, lin, quad = get_mvr_coeff(
                 site, product, lev1["frequency"][:]
             )
         else:
+            # pylint: disable-next=unbalanced-tuple-unpacking
             (
                 coeff,
                 input_scale,
                 input_offset,
                 output_scale,
                 output_offset,
                 weights1,
@@ -212,14 +208,15 @@
         else:
             product, ret = "absolute_humidity", "hpt"
 
         coeff = get_mvr_coeff(site, ret, lev1["frequency"][:])
         if coeff[0]["RT"] < 2:
             coeff, offset, lin, quad = get_mvr_coeff(site, ret, lev1["frequency"][:])
         else:
+            # pylint: disable-next=unbalanced-tuple-unpacking
             (
                 coeff,
                 input_scale,
                 input_offset,
                 output_scale,
                 output_offset,
                 weights1,
@@ -297,14 +294,15 @@
                 rpg_dat[product] = rpg_dat[product] / 1000.0
 
     elif data_type == "2P02":
         coeff = get_mvr_coeff(site, "tpb", lev1["frequency"][:])
         if coeff[0]["RT"] < 2:
             coeff, offset, lin, quad = get_mvr_coeff(site, "tpb", lev1["frequency"][:])
         else:
+            # pylint: disable-next=unbalanced-tuple-unpacking
             coeff, _, _, _, _, _, _, _ = get_mvr_coeff(
                 site, "tpb", lev1["frequency"][:]
             )
 
         coeff["AG"] = np.sort(coeff["AG"])
         _, freq_ind, _ = np.intersect1d(
             lev1["frequency"][:],
@@ -486,15 +484,15 @@
                 try:
                     rpg_dat[ivars] = lev1[ivars][index]
                 except IndexError:
                     rpg_dat[ivars] = lev1[ivars][:]
 
 
 def _add_att(global_attributes: dict, coeff: dict) -> None:
-    "add retrieval and calibration attributes"
+    """Add retrieval and calibration attributes"""
     fields = [
         "retrieval_type",
         "retrieval_elevation_angles",
         "retrieval_frequencies",
         "retrieval_auxiliary_input",
         "retrieval_description",
     ]
@@ -509,15 +507,15 @@
     att_names = global_attributes.keys()
     for name in list(att_names):
         if any(x in name for x in att_del):
             del global_attributes[name]
 
 
 def load_product(filename: str):
-    """load existing lev2 file for deriving other products"""
+    """Load existing lev2 file for deriving other products"""
     file = nc.Dataset(filename)
     ret_freq = get_ret_freq(filename)
     ret_ang = get_ret_ang(filename)
     return file, ret_freq, ret_ang
 
 
 def _test_bl_scan(site: str, lev1: nc.Dataset) -> bool:
```

### Comparing `mwrpy-0.2.0/mwrpy/plots/generate_plots.py` & `mwrpy-0.3.0/mwrpy/plots/generate_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,18 @@
 
 def generate_figure(
     nc_file: str,
     field_names: list,
     show: bool = False,
     save_path: str = None,
     max_y: int = 5,
-    ele_range: list = [0.0, 91.0],
+    ele_range: tuple[float, float] = (
+        0.0,
+        91.0,
+    ),
     pointing: int = 0,
     dpi: int = 120,
     image_name: str | None = None,
     sub_title: bool = True,
     title: bool = True,
 ) -> tuple[Dimensions, str]:
     """Generates a mwrpy figure.
@@ -252,15 +255,15 @@
     #     raise ValueError("No fields to be plotted")
     return valid_data, valid_names
 
 
 def _is_height_dimension(full_path: str) -> bool:
     """Checks for height dimension in netCDF file."""
     with netCDF4.Dataset(full_path) as nc:
-        is_height = "altitude" in nc.variables
+        is_height = "height" in nc.variables
     return is_height
 
 
 def _elevation_filter(full_path: str, data_field: ndarray, ele_range: tuple) -> ndarray:
     """Filters data for specified range of elevation angles."""
     with netCDF4.Dataset(full_path) as nc:
         if "elevation_angle" in nc.variables:
@@ -1373,16 +1376,17 @@
             color=_COLORS["darkgray"],
             markersize=3,
             label="Abs. hum.",
         )
 
         yl = ax.get_ylim()
         yl2 = ax2.get_ylim()
-        f = lambda x: yl2[0] + (x - yl[0]) / (yl[1] - yl[0]) * (yl2[1] - yl2[0])
-        ticks = f(ax.get_yticks())
+
+        ticks = _calculate_ticks(ax.get_yticks(), yl, yl2)
+
         ax2.yaxis.set_major_locator(FixedLocator(ticks))
         ax2.yaxis.set_major_formatter(FormatStrFormatter("%.4f"))
         ax3 = ax.twinx()
         ax3.plot(time, data, ".", alpha=0.8, color=_COLORS["darksky"], markersize=1)
         ax3.plot(
             time,
             rolling_mean,
@@ -1420,30 +1424,35 @@
             min_y=0.0,
         )
         if np.nanmax(data) <= 2.0:
             minorLocator = MultipleLocator(0.5)
             ax.yaxis.set_major_locator(minorLocator)
         yl = ax.get_ylim()
         yl2 = ax2.get_ylim()
-        f = lambda x: yl2[0] + (x - yl[0]) / (yl[1] - yl[0]) * (yl2[1] - yl2[0])
-        ticks = f(ax.get_yticks())
+
+        ticks = _calculate_ticks(ax.get_yticks(), yl, yl2)
+
         ax2.yaxis.set_major_locator(FixedLocator(ticks))
         ax2.yaxis.set_major_formatter(FormatStrFormatter("%.3f"))
         _set_ax(ax, vmax, "rain rate (" + ylabel + ")", min_y=vmin)
         ax3 = ax.twinx()
         ax3.plot(time, data, ".", alpha=0.8, color=_COLORS["darksky"], markersize=1)
         ax3.plot(
             time, rolling_mean, "o", fillstyle="full", color="darkblue", markersize=3
         )
         _set_ax(ax3, vmax, "", min_y=vmin)
         ax3.set_yticklabels([])
         ax3.set_yticks([])
         ax3.set_frame_on(False)
 
 
+def _calculate_ticks(x, yl, yl2):
+    return yl2[0] + (x - yl[0]) / (yl[1] - yl[0]) * (yl2[1] - yl2[0])
+
+
 def _plot_int(ax, data_in: ma.MaskedArray, name: str, time: ndarray, nc_file: str):
     """Plot for integrated quantities (LWP, IWV)."""
 
     flag = _get_ret_flag(nc_file, time)
     data0, time0 = data_in[flag == 0], time[flag == 0]
     if len(data0) == 0:
         data0, time0 = data_in, time
```

### Comparing `mwrpy-0.2.0/mwrpy/plots/plot_meta.py` & `mwrpy-0.3.0/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/plots/plot_utils.py` & `mwrpy-0.3.0/mwrpy/plots/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     if threshold is not None:
         threshold = im.norm(threshold)
     else:
         threshold = im.norm(data.max()) / 2.0
 
     # Set default alignment to center, but allow it to be
     # overwritten by textkw.
-    kw = dict(horizontalalignment="center", verticalalignment="center")
+    kw = {"horizontalalignment": "center", "verticalalignment": "center"}
     kw.update(textkw)
 
     # Get the formatter in case a string is supplied
     if isinstance(valfmt, str):
         valfmt = ticker.StrMethodFormatter(valfmt)
 
     # Loop over the data and create a `Text` for each "pixel".
```

### Comparing `mwrpy-0.2.0/mwrpy/rpg_mwr.py` & `mwrpy-0.3.0/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.3.0/mwrpy/site_config/hatpro.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,179 +1,203 @@
 # Config file for all HATPRO instruments
 
 params:
-    receiver_nb: [1, 2]
-    receiver: [1, 1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2]
-
-    # bandwidth of the central frequency in MHz (center frequency of single of upper side-band)
-    bandwidth: [230., 230., 230., 230., 230., 230., 230., 230., 230., 230., 230., 600., 1000., 2000.]
-
-    # 56.xx +/- X +/- Y
-    n_sidebands: [1, 1]
-    sideband_IF_separation: [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]
-
-    # Beam width (3 dB) of the microwave radiometer
-    beam_width: 2.
-
-    # offset correction for TBs, i.e. adjustement of observation to nominal frequency:
-    # Note: RPG offers a frequency shift within the radiometer software.
-    # This shift will modify the TBs calculated with the RPG software.
-    # Original TBs CANNOT be reconstructed, unless you have recorded the voltages & calibration parameters and possess adequate software routines to perform a re-calibration.
-    # Hence, the authors of actris_mwr_pro DO NOT recommend to apply the frequency shifts in general.
-    # If you have applied these frequency shifts, you may still give these to protocol so that they are contained in the resulting level1 netcdf files.
-    # The variable freq_shift specifies the frequency shifts applied [in MHz].
-    # Set all to 0 if no frequency shifts were applied.
-    freq_shift: [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]
-
-    # [lower, upper] bound threshold of TB quality flags in K
-    TB_threshold: [2.7, 330.]
-
-    # IRT parameters
-    ir_bandwidth: 1.9
-    ir_beamwidth: 2.64
-
-    # solar angle flagging:
-    # saf parameter lets the user determine within what angular region (in deg) around the sun the MWR TBs and products are flagged,
-    # e.g. saf = 5 means that all values with +-5 deg elevation and +-5 deg azimuth will be flagged.
-    # Note that this flag only works if radiometer position is correctly specified and the radiometer is aligned towards thebandwidth North.
-    saf: 7.
-
-    # thresholds for met quality flags
-    # air_temperature [K]
-    # relative_humidity [1]
-    # air_pressure [hPa]
-    # rainfall_rate [mm/h]
-    # wind_direction [°]
-    # wind_speed [m/s]
-    met_thresholds: [[213.15, 333.15], [0., 1.], [90000., 110000.], [0., 300.], [0., 360.], [0., 100.]]
+  receiver_nb: [1, 2]
+  receiver: [1, 1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2]
 
+  # bandwidth of the central frequency in MHz (center frequency of single of upper side-band)
+  bandwidth:
+    [
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      230.,
+      600.,
+      1000.,
+      2000.,
+    ]
+
+  # 56.xx +/- X +/- Y
+  n_sidebands: [1, 1]
+  sideband_IF_separation:
+    [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]
+
+  # Beam width (3 dB) of the microwave radiometer
+  beam_width: 2.
+
+  # offset correction for TBs, i.e. adjustement of observation to nominal frequency:
+  # Note: RPG offers a frequency shift within the radiometer software.
+  # This shift will modify the TBs calculated with the RPG software.
+  # Original TBs CANNOT be reconstructed, unless you have recorded the voltages & calibration parameters and possess adequate software routines to perform a re-calibration.
+  # Hence, the authors of actris_mwr_pro DO NOT recommend to apply the frequency shifts in general.
+  # If you have applied these frequency shifts, you may still give these to protocol so that they are contained in the resulting level1 netcdf files.
+  # The variable freq_shift specifies the frequency shifts applied [in MHz].
+  # Set all to 0 if no frequency shifts were applied.
+  freq_shift: [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]
+
+  # [lower, upper] bound threshold of TB quality flags in K
+  TB_threshold: [2.7, 330.]
+
+  # IRT parameters
+  ir_bandwidth: 1.9
+  ir_beamwidth: 2.64
+
+  # solar angle flagging:
+  # saf parameter lets the user determine within what angular region (in deg) around the sun the MWR TBs and products are flagged,
+  # e.g. saf = 5 means that all values with +-5 deg elevation and +-5 deg azimuth will be flagged.
+  # Note that this flag only works if radiometer position is correctly specified and the radiometer is aligned towards thebandwidth North.
+  saf: 7.
+
+  # thresholds for met quality flags
+  # air_temperature [K]
+  # relative_humidity [1]
+  # air_pressure [hPa]
+  # rainfall_rate [mm/h]
+  # wind_direction [°]
+  # wind_speed [m/s]
+  met_thresholds:
+    [
+      [213.15, 333.15],
+      [0., 1.],
+      [90000., 110000.],
+      [0., 300.],
+      [0., 360.],
+      [0., 100.],
+    ]
 
 # Missing entries are filled with site specific config file
 global_specs:
-    # Name of the conventions followed by the dataset
-    conventions: CF-1.8
+  # Name of the conventions followed by the dataset
+  conventions: CF-1.8
 
-    # A succinct description of what is in the dataset, composed of instrument type and site name
-    title:
+  # A succinct description of what is in the dataset, composed of instrument type and site name
+  title:
 
-    # Versioning of the datasets (containing date and software version)
-    history:
+  # Versioning of the datasets (containing date and software version)
+  history:
 
-    # Where the original data was produced
-    institution:
+  # Where the original data was produced
+  institution:
 
-    # The method of production of the original data
-    source: Ground Based Remote Sensing
+  # The method of production of the original data
+  source: Ground Based Remote Sensing
 
-    # Miscellaneous Information about the dataset or methods used to produce it
-    comment:
+  # Miscellaneous Information about the dataset or methods used to produce it
+  comment:
 
-    # References that describe the data or methods used to produce it
-    references:
+  # References that describe the data or methods used to produce it
+  references:
 
-    # Name of measurement station
-    site_location:
+  # Name of measurement station
+  site_location:
 
-    # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
-    instrument_id:
+  # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
+  instrument_id:
 
-    # WIGOS Station identifier acording to WIGOS convention
-    wigos_station_id:
+  # WIGOS Station identifier acording to WIGOS convention
+  wigos_station_id:
 
-    # Department responsible for the instrument
-    principal_investigator:
+  # Department responsible for the instrument
+  principal_investigator:
 
-    # Manufacturer of the instrument
-    instrument_manufacturer: Radiometer Physics (RPG)
+  # Manufacturer of the instrument
+  instrument_manufacturer: Radiometer Physics (RPG)
 
-    # Instrument model
-    instrument_model: HATPRO
+  # Instrument model
+  instrument_model: HATPRO
 
-    # Instrument generation
-    instrument_generation:
+  # Instrument generation
+  instrument_generation:
 
-    # Specific to mainboard
-    instrument_hw_id:
+  # Specific to mainboard
+  instrument_hw_id:
 
-    # Name of network(s) that instrument may be part of
-    network_name:
+  # Name of network(s) that instrument may be part of
+  network_name:
 
-    # Name of campaign instrument may collect data for
-    campaign_name:
+  # Name of campaign instrument may collect data for
+  campaign_name:
 
-    # List of files the data set is depending on
-    dependencies:
+  # List of files the data set is depending on
+  dependencies:
 
-    # Data license
-    license:
+  # Data license
+  license:
 
-    # Status of instrument absolute calibration
-    instrument_calibration_status:
+  # Status of instrument absolute calibration
+  instrument_calibration_status:
 
-    # Time of last (automatic or manual) absolute calibration of receiver 1
-    receiver1_date_of_last_absolute_calibration:
+  # Time of last (automatic or manual) absolute calibration of receiver 1
+  receiver1_date_of_last_absolute_calibration:
 
-    # Type of last (automatic or manual) absolute calibration of receiver 1
-    receiver1_type_of_last_absolute_calibration:
+  # Type of last (automatic or manual) absolute calibration of receiver 1
+  receiver1_type_of_last_absolute_calibration:
 
-    # Time of last (automatic or manual) absolute calibration of receiver 2
-    receiver2_date_of_last_absolute_calibration:
+  # Time of last (automatic or manual) absolute calibration of receiver 2
+  receiver2_date_of_last_absolute_calibration:
 
-    # Type of last (automatic or manual) absolute calibration of receiver 2
-    receiver2_type_of_last_absolute_calibration:
+  # Type of last (automatic or manual) absolute calibration of receiver 2
+  receiver2_type_of_last_absolute_calibration:
 
-    # Type of automatic calibrations performed for receiver 1
-    receiver1_type_of_automatic_calibrations: calibration with ambient temperature target and noise diode with high-frequency noise switching
+  # Type of automatic calibrations performed for receiver 1
+  receiver1_type_of_automatic_calibrations: calibration with ambient temperature target and noise diode with high-frequency noise switching
 
-    # Type of automatic calibrations performed for receiver 2
-    receiver2_type_of_automatic_calibrations: calibration with ambient temperature target and noise diode with high-frequency noise switching
+  # Type of automatic calibrations performed for receiver 2
+  receiver2_type_of_automatic_calibrations: calibration with ambient temperature target and noise diode with high-frequency noise switching
 
-    # Time of last covariance update as YYYYMMDD
-    date_of_last_covariance_matrix:
+  # Time of last covariance update as YYYYMMDD
+  date_of_last_covariance_matrix:
 
-    # Logbook repair/replacement work performed
-    instrument_history:
+  # Logbook repair/replacement work performed
+  instrument_history:
 
-    # Manufacturer of the infrared radiometer
-    ir_instrument_manufacturer: Heitronics
+  # Manufacturer of the infrared radiometer
+  ir_instrument_manufacturer: Heitronics
 
-    # Infrared radiometer model
-    ir_instrument_model: KT19.85
+  # Infrared radiometer model
+  ir_instrument_model: KT19.85
 
-    # Fabrication year of the infrared radiometer
-    ir_instrument_fabrication_year:
+  # Fabrication year of the infrared radiometer
+  ir_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    ir_instrument_history:
+  # Logbook repair/replacement work performed
+  ir_instrument_history:
 
-    # Total absolute calibration uncertainty of infrared brightness temperature, one standard deviation.
-    ir_accuracy: 1 K
+  # Total absolute calibration uncertainty of infrared brightness temperature, one standard deviation.
+  ir_accuracy: 1 K
 
-    # Manufacturer of the weather station
-    met_instrument_manufacturer: Vaisala
+  # Manufacturer of the weather station
+  met_instrument_manufacturer: Vaisala
 
-    # Weather station model
-    met_instrument_model: WXT536
+  # Weather station model
+  met_instrument_model: WXT536
 
-    # Fabrication year of the weather station
-    met_instrument_fabrication_year:
+  # Fabrication year of the weather station
+  met_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    met_instrument_history:
+  # Logbook repair/replacement work performed
+  met_instrument_history:
 
-    # Air temperature accuracy. Unit: K.
-    air_temperature_accuracy: 0.3 K
+  # Air temperature accuracy. Unit: K.
+  air_temperature_accuracy: 0.3 K
 
-    # Relative humidity accuracy. Unit: 1.
-    relative_humidity_accuracy: 3-5%
+  # Relative humidity accuracy. Unit: 1.
+  relative_humidity_accuracy: 3-5%
 
-    # Air pressure accuracy. Unit: hPa.
-    air_pressure_accuracy: 0.5 hPa
+  # Air pressure accuracy. Unit: hPa.
+  air_pressure_accuracy: 0.5 hPa
 
-    # Rain rate accuracy. Unit: mm/h.
-    rainfall_rate_accuracy: < 5%
+  # Rain rate accuracy. Unit: mm/h.
+  rainfall_rate_accuracy: < 5%
 
-    # Wind direction accuracy. Unit: degrees.
-    wind_direction_accuracy: 3 degrees
+  # Wind direction accuracy. Unit: degrees.
+  wind_direction_accuracy: 3 degrees
 
-    # Wind speed accuracy. Unit: m/s.
-    wind_speed_accuracy: 0.3 m/s
+  # Wind speed accuracy. Unit: m/s.
+  wind_speed_accuracy: 0.3 m/s
```

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.3.0/mwrpy/site_config/hyytiala/config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,103 @@
 # Site config file
 
 type: hatpro
 
 params:
-    altitude: 174.
-    longitude: 24.288
-    latitude: 61.844
-
-    # path to level1 data and path for processed files
-    data_in: /home/tmarke/Dokumente/ACTRIS/mwr_pro_actris/data/
-    data_out: /home/tmarke/Dokumente/ACTRIS/mwr_pro_actris/data/
-
-    # path to ABSCAL.HIS file
-    path_to_cal: /home/tmarke/Dokumente/ACTRIS/mwr_pro_actris/
-
-    # integration time for BL scans in seconds
-    scan_time: 100.
-
-    # integration time of measurements in seconds
-    int_time: 1
-
-    # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
-    # If you do not want to transform the coordinates set azi_cor to -999.
-    azi_cor: -999.
-    # Azimuth correction:
-    # Set az_cor to the angle that RPG software gives when instrument is pointing to the North.
-    const_azi: -999.
-
-    # quality flag status for level 1 data; 0: flag active
-    # Bit 1: missing_tb
-    # Bit 2: tb_below_threshold
-    # Bit 3: tb_above_threshold
-    # Bit 4: spectral_consistency_above_threshold
-    # Bit 5: receiver_sanity_failed
-    # Bit 6: rain_detected
-    # Bit 7: sun_moon_in_beam
-    # Bit 8: tb_offset_above_threshold
-    flag_status: [0, 0, 0, 1, 0, 0, 0, 1]
-
-    # availability of IR
-    ir_flag: True
+  altitude: 174.
+  longitude: 24.288
+  latitude: 61.844
+
+  # path to level1 data and path for processed files
+  data_in: /tmp/data/
+  data_out: /tmp/data/
+
+  # path to ABSCAL.HIS file
+  path_to_cal: /home/tmarke/Dokumente/ACTRIS/mwr_pro_actris/
+
+  # integration time for BL scans in seconds
+  scan_time: 100.
+
+  # integration time of measurements in seconds
+  int_time: 1
+
+  # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
+  # If you do not want to transform the coordinates set azi_cor to -999.
+  azi_cor: -999.
+  # Azimuth correction:
+  # Set az_cor to the angle that RPG software gives when instrument is pointing to the North.
+  const_azi: -999.
+
+  # quality flag status for level 1 data; 0: flag active
+  # Bit 1: missing_tb
+  # Bit 2: tb_below_threshold
+  # Bit 3: tb_above_threshold
+  # Bit 4: spectral_consistency_above_threshold
+  # Bit 5: receiver_sanity_failed
+  # Bit 6: rain_detected
+  # Bit 7: sun_moon_in_beam
+  # Bit 8: tb_offset_above_threshold
+  flag_status: [0, 0, 0, 1, 0, 0, 0, 1]
 
+  # availability of IR
+  ir_flag: True
 
 global_specs:
-    # A succinct description of what is in the dataset, composed of instrument type and site name
-    title: HATPRO G5 MWR at Hyytiala, Finland
+  # A succinct description of what is in the dataset, composed of instrument type and site name
+  title: HATPRO G5 MWR at Hyytiala, Finland
 
-    # Versioning of the datasets (containing date and software version)
-    history:
+  # Versioning of the datasets (containing date and software version)
+  history:
 
-    # Where the original data was produced
-    institution: University of Helsinki
+  # Where the original data was produced
+  institution: University of Helsinki
 
-    # Miscellaneous Information about the dataset or methods used to produce it
-    comment:
+  # Miscellaneous Information about the dataset or methods used to produce it
+  comment:
 
-    # References that describe the data or methods used to produce it
-    references:
+  # References that describe the data or methods used to produce it
+  references:
 
-    # Name of measurement station
-    site_location: hyytiala
+  # Name of measurement station
+  site_location: hyytiala
 
-    # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
-    instrument_id: A
+  # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
+  instrument_id: A
 
-    # WIGOS Station identifier acording to WIGOS convention
-    wigos_station_id: XXX
+  # WIGOS Station identifier acording to WIGOS convention
+  wigos_station_id: XXX
 
-    # Department responsible for the instrument
-    principal_investigator:
+  # Department responsible for the instrument
+  principal_investigator:
 
-    # Instrument generation
-    instrument_generation: G5
+  # Instrument generation
+  instrument_generation: G5
 
-    # Specific to mainboard
-    instrument_hw_id:
+  # Specific to mainboard
+  instrument_hw_id:
 
-    # Name of network(s) that instrument may be part of
-    network_name:
+  # Name of network(s) that instrument may be part of
+  network_name:
 
-    # Name of campaign instrument may collect data for
-    campaign_name:
+  # Name of campaign instrument may collect data for
+  campaign_name:
 
-    # List of files the data set is depending on
-    dependencies:
+  # List of files the data set is depending on
+  dependencies:
 
-    # Data license
-    license:
+  # Data license
+  license:
 
-    # Logbook repair/replacement work performed
-    instrument_history:
+  # Logbook repair/replacement work performed
+  instrument_history:
 
-    # Fabrication year of the infrared radiometer
-    ir_instrument_fabrication_year:
+  # Fabrication year of the infrared radiometer
+  ir_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    ir_instrument_history:
+  # Logbook repair/replacement work performed
+  ir_instrument_history:
 
-    # Fabrication year of the weather station
-    met_instrument_fabrication_year:
+  # Fabrication year of the weather station
+  met_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    met_instrument_history:
+  # Logbook repair/replacement work performed
+  met_instrument_history:
```

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/juelich/config.yaml` & `mwrpy-0.3.0/mwrpy/site_config/juelich/config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,103 @@
 # Site config file
 
 type: hatpro
 
 params:
-    altitude: 108.
-    longitude: 6.407
-    latitude: 50.906
-
-    # path to level1 data and path for processed files
-    data_in: /data/obs/site/jue/tophat/l1/
-    data_out: /data/obs/site/jue/tophat/actris/
-
-    # path to ABSCAL.HIS file
-    path_to_cal: /data/obs/site/jue/tophat/calibration/LOG_TRANSFER/CALIB/
-
-    # integration time for BL scans in seconds
-    scan_time: 50.
-
-    # integration time of measurements in seconds
-    int_time: 1
-
-    # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
-    # If you do not want to transform the coordinates set azi_cor to -999.
-    azi_cor: -999.
-    # Azimuth correction:
-    # Set az_cor to the angle that RPG software gives when instrument is pointing to the North.
-    const_azi: -999.
-
-    # quality flag status for level 1 data; 0: flag active
-    # Bit 1: missing_tb
-    # Bit 2: tb_below_threshold
-    # Bit 3: tb_above_threshold
-    # Bit 4: spectral_consistency_above_threshold
-    # Bit 5: receiver_sanity_failed
-    # Bit 6: rain_detected
-    # Bit 7: sun_moon_in_beam
-    # Bit 8: tb_offset_above_threshold
-    flag_status: [0, 0, 0, 0, 0, 0, 0, 1]
-
-    # availability of IR
-    ir_flag: True
+  altitude: 108.
+  longitude: 6.407
+  latitude: 50.906
+
+  # path to level1 data and path for processed files
+  data_in: /data/obs/site/jue/tophat/l1/
+  data_out: /data/obs/site/jue/tophat/actris/
+
+  # path to ABSCAL.HIS file
+  path_to_cal: /data/obs/site/jue/tophat/calibration/LOG_TRANSFER/CALIB/
+
+  # integration time for BL scans in seconds
+  scan_time: 50.
+
+  # integration time of measurements in seconds
+  int_time: 1
+
+  # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
+  # If you do not want to transform the coordinates set azi_cor to -999.
+  azi_cor: -999.
+  # Azimuth correction:
+  # Set az_cor to the angle that RPG software gives when instrument is pointing to the North.
+  const_azi: -999.
+
+  # quality flag status for level 1 data; 0: flag active
+  # Bit 1: missing_tb
+  # Bit 2: tb_below_threshold
+  # Bit 3: tb_above_threshold
+  # Bit 4: spectral_consistency_above_threshold
+  # Bit 5: receiver_sanity_failed
+  # Bit 6: rain_detected
+  # Bit 7: sun_moon_in_beam
+  # Bit 8: tb_offset_above_threshold
+  flag_status: [0, 0, 0, 0, 0, 0, 0, 1]
 
+  # availability of IR
+  ir_flag: True
 
 global_specs:
-    # A succinct description of what is in the dataset, composed of instrument type and site name
-    title: HATPRO G5 MWR at Juelich, Germany
+  # A succinct description of what is in the dataset, composed of instrument type and site name
+  title: HATPRO G5 MWR at Juelich, Germany
 
-    # Versioning of the datasets (containing date and software version)
-    history:
+  # Versioning of the datasets (containing date and software version)
+  history:
 
-    # Where the original data was produced
-    institution: University of Cologne
+  # Where the original data was produced
+  institution: University of Cologne
 
-    # Miscellaneous Information about the dataset or methods used to produce it
-    comment:
+  # Miscellaneous Information about the dataset or methods used to produce it
+  comment:
 
-    # References that describe the data or methods used to produce it
-    references:
+  # References that describe the data or methods used to produce it
+  references:
 
-    # Name of measurement station
-    site_location: juelich
+  # Name of measurement station
+  site_location: juelich
 
-    # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
-    instrument_id:
+  # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
+  instrument_id:
 
-    # WIGOS Station identifier acording to WIGOS convention
-    wigos_station_id: 0-276-0-10508
+  # WIGOS Station identifier acording to WIGOS convention
+  wigos_station_id: 0-276-0-10508
 
-    # Department responsible for the instrument
-    principal_investigator: Institute for Geophysics and Meteorology (IGMK)
+  # Department responsible for the instrument
+  principal_investigator: Institute for Geophysics and Meteorology (IGMK)
 
-    # Instrument generation
-    instrument_generation: G5
+  # Instrument generation
+  instrument_generation: G5
 
-    # Specific to mainboard
-    instrument_hw_id:
+  # Specific to mainboard
+  instrument_hw_id:
 
-    # Name of network(s) that instrument may be part of
-    network_name: ACTRIS
+  # Name of network(s) that instrument may be part of
+  network_name: ACTRIS
 
-    # Name of campaign instrument may collect data for
-    campaign_name:
+  # Name of campaign instrument may collect data for
+  campaign_name:
 
-    # List of files the data set is depending on
-    dependencies:
+  # List of files the data set is depending on
+  dependencies:
 
-    # Data license
-    license:
+  # Data license
+  license:
 
-    # Logbook repair/replacement work performed
-    instrument_history:
+  # Logbook repair/replacement work performed
+  instrument_history:
 
-    # Fabrication year of the infrared radiometer
-    ir_instrument_fabrication_year:
+  # Fabrication year of the infrared radiometer
+  ir_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    ir_instrument_history:
+  # Logbook repair/replacement work performed
+  ir_instrument_history:
 
-    # Fabrication year of the weather station
-    met_instrument_fabrication_year:
+  # Fabrication year of the weather station
+  met_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    met_instrument_history:
+  # Logbook repair/replacement work performed
+  met_instrument_history:
```

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.2.0/mwrpy/site_config/lindenberg/config.yaml` & `mwrpy-0.3.0/mwrpy/site_config/lindenberg/config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,103 @@
 # Site config file
 
 type: hatpro
 
 params:
-    altitude: 104.
-    longitude: 14.118
-    latitude: 52.208
-
-    # path to level1 data and path for processed files
-    data_in: /data/obs/site/lin/linhat/l1/
-    data_out: /data/obs/site/lin/linhat/actris/
-
-    # path to ABSCAL.HIS file
-    path_to_cal: /data/obs/site/lin/linhat/
-
-    # integration time for BL scans in seconds
-    scan_time: 100.
-
-    # integration time of measurements in seconds
-    int_time: 1
-
-    # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
-    # If you do not want to transform the coordinates set azi_cor to -999.
-    azi_cor: -999.
-    # Azimuth correction:
-    # Set az_cor to the angle that RPG software gives when instrument is pointing to the North.
-    const_azi: -999.
-
-    # quality flag status for level 1 data; 0: flag active
-    # Bit 1: missing_tb
-    # Bit 2: tb_below_threshold
-    # Bit 3: tb_above_threshold
-    # Bit 4: spectral_consistency_above_threshold
-    # Bit 5: receiver_sanity_failed
-    # Bit 6: rain_detected
-    # Bit 7: sun_moon_in_beam
-    # Bit 8: tb_offset_above_threshold
-    flag_status: [0, 0, 0, 0, 0, 0, 0, 1]
-
-    # availability of IR
-    ir_flag: True
+  altitude: 104.
+  longitude: 14.118
+  latitude: 52.208
+
+  # path to level1 data and path for processed files
+  data_in: /data/obs/site/lin/linhat/l1/
+  data_out: /data/obs/site/lin/linhat/actris/
+
+  # path to ABSCAL.HIS file
+  path_to_cal: /data/obs/site/lin/linhat/
+
+  # integration time for BL scans in seconds
+  scan_time: 100.
+
+  # integration time of measurements in seconds
+  int_time: 1
+
+  # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
+  # If you do not want to transform the coordinates set azi_cor to -999.
+  azi_cor: -999.
+  # Azimuth correction:
+  # Set az_cor to the angle that RPG software gives when instrument is pointing to the North.
+  const_azi: -999.
+
+  # quality flag status for level 1 data; 0: flag active
+  # Bit 1: missing_tb
+  # Bit 2: tb_below_threshold
+  # Bit 3: tb_above_threshold
+  # Bit 4: spectral_consistency_above_threshold
+  # Bit 5: receiver_sanity_failed
+  # Bit 6: rain_detected
+  # Bit 7: sun_moon_in_beam
+  # Bit 8: tb_offset_above_threshold
+  flag_status: [0, 0, 0, 0, 0, 0, 0, 1]
 
+  # availability of IR
+  ir_flag: True
 
 global_specs:
-    # A succinct description of what is in the dataset, composed of instrument type and site name
-    title: HATPRO G5 MWR at Lindenberg, Germany
+  # A succinct description of what is in the dataset, composed of instrument type and site name
+  title: HATPRO G5 MWR at Lindenberg, Germany
 
-    # Versioning of the datasets (containing date and software version)
-    history:
+  # Versioning of the datasets (containing date and software version)
+  history:
 
-    # Where the original data was produced
-    institution: DWD
+  # Where the original data was produced
+  institution: DWD
 
-    # Miscellaneous Information about the dataset or methods used to produce it
-    comment:
+  # Miscellaneous Information about the dataset or methods used to produce it
+  comment:
 
-    # References that describe the data or methods used to produce it
-    references:
+  # References that describe the data or methods used to produce it
+  references:
 
-    # Name of measurement station
-    site_location: lindenberg
+  # Name of measurement station
+  site_location: lindenberg
 
-    # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
-    instrument_id: A
+  # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
+  instrument_id: A
 
-    # WIGOS Station identifier acording to WIGOS convention
-    wigos_station_id: 0-20000-0-10393
+  # WIGOS Station identifier acording to WIGOS convention
+  wigos_station_id: 0-20000-0-10393
 
-    # Department responsible for the instrument
-    principal_investigator:
+  # Department responsible for the instrument
+  principal_investigator:
 
-    # Instrument generation
-    instrument_generation: G5
+  # Instrument generation
+  instrument_generation: G5
 
-    # Specific to mainboard
-    instrument_hw_id:
+  # Specific to mainboard
+  instrument_hw_id:
 
-    # Name of network(s) that instrument may be part of
-    network_name: ACTRIS
+  # Name of network(s) that instrument may be part of
+  network_name: ACTRIS
 
-    # Name of campaign instrument may collect data for
-    campaign_name:
+  # Name of campaign instrument may collect data for
+  campaign_name:
 
-    # List of files the data set is depending on
-    dependencies:
+  # List of files the data set is depending on
+  dependencies:
 
-    # Data license
-    license:
+  # Data license
+  license:
 
-    # Logbook repair/replacement work performed
-    instrument_history:
+  # Logbook repair/replacement work performed
+  instrument_history:
 
-    # Fabrication year of the infrared radiometer
-    ir_instrument_fabrication_year:
+  # Fabrication year of the infrared radiometer
+  ir_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    ir_instrument_history:
+  # Logbook repair/replacement work performed
+  ir_instrument_history:
 
-    # Fabrication year of the weather station
-    met_instrument_fabrication_year:
+  # Fabrication year of the weather station
+  met_instrument_fabrication_year:
 
-    # Logbook repair/replacement work performed
-    met_instrument_history:
+  # Logbook repair/replacement work performed
+  met_instrument_history:
```

### Comparing `mwrpy-0.2.0/mwrpy/utils.py` & `mwrpy-0.3.0/mwrpy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for general helper functions."""
 
+import datetime
 import glob
+import logging
 import os
 import re
 import time
-from datetime import date, datetime, timedelta, timezone
 from typing import Any, Iterator, NamedTuple
 
 import netCDF4
 import numpy as np
 import pandas as pd
 import yaml
 from numpy import ma
@@ -54,20 +55,24 @@
         epoch_time (ndarray): 1-D array of seconds since (2001,1,1,0,0,0)
 
     Returns:
         ndarray: Unix time in seconds since (1970,1,1,0,0,0).
 
     """
 
-    delta = (datetime(*epoch) - datetime(1970, 1, 1, 0, 0, 0)).total_seconds()
+    delta = (
+        datetime.datetime(*epoch) - datetime.datetime(1970, 1, 1, 0, 0, 0)
+    ).total_seconds()
     unix_time = epoch_time + int(delta)
     if time_ref == 0:
         for index, _ in enumerate(unix_time):
             unix_time[index] = time.mktime(
-                datetime.fromtimestamp(unix_time[index], timezone.utc).timetuple()
+                datetime.datetime.fromtimestamp(
+                    unix_time[index], datetime.timezone.utc
+                ).timetuple()
             )
     return unix_time
 
 
 def isscalar(array: Any) -> bool:
     """Tests if input is scalar.
     By "scalar" we mean that array has a single value.
@@ -158,16 +163,15 @@
             mask = ~values.mask
             if ma.any(values[mask]):
                 result[:, ind] = np.interp(x_new, x_in[mask], values[mask])
         else:
             result[:, ind] = np.interp(x_new, x_in, values)
     result[~np.isfinite(result)] = 0
     masked = ma.make_mask(result)
-
-    return ma.array(result, mask=~masked)
+    return ma.array(result, mask=np.invert(masked))
 
 
 def add_interpol1d(
     data0: dict, data1: np.ndarray, time1: np.ndarray, output_name: str
 ) -> None:
     """Adds interpolated 1d field to dict
     Args:
@@ -192,17 +196,23 @@
     Args:
         time_in_seconds: Seconds since some epoch.
         epoch: Epoch, default is (1970, 1, 1) (UTC).
     Returns:
         [year, month, day, hours, minutes, seconds] formatted as '05' etc (UTC).
     """
 
-    epoch_in_seconds = datetime.timestamp(datetime(*epoch, tzinfo=timezone.utc))
+    epoch_in_seconds = datetime.datetime.timestamp(
+        datetime.datetime(*epoch, tzinfo=datetime.timezone.utc)
+    )
     timestamp = time_in_seconds + epoch_in_seconds
-    return datetime.utcfromtimestamp(timestamp).strftime("%Y %m %d %H %M %S").split()
+    return (
+        datetime.datetime.utcfromtimestamp(timestamp)
+        .strftime("%Y %m %d %H %M %S")
+        .split()
+    )
 
 
 def str_to_numeric(value: str) -> int | float:
     """Converts string to number (int or float)."""
     try:
         return int(value)
     except ValueError:
@@ -231,75 +241,59 @@
         ),
     ]
     c_list = [x for x in s_list if x]
 
     if len(c_list) > 0:
         c_list = sorted(c_list[0])
     else:
-        print(
-            [
-                "No coefficient files for product "
-                + prefix
-                + " found in directory "
-                + "/site_config/"
-                + site
-                + "/coefficients/"
-            ]
+        logging.warning(
+            "No coefficient files for product "
+            + prefix
+            + " found in directory "
+            + "/site_config/"
+            + site
+            + "/coefficients/"
         )
     return c_list
 
 
 def get_file_list(path_to_files: str, extension: str):
     """Returns file list for specified path."""
     f_list = sorted(glob.glob(path_to_files + "/*." + extension))
     if len(f_list) == 0:
         f_list = sorted(glob.glob(path_to_files + "/*." + extension.lower()))
     if len(f_list) == 0:
-        print(
-            [
-                "Error: no binary files with extension "
-                + extension
-                + " found in directory "
-                + path_to_files
-            ]
+        logging.warning(
+            "Error: no binary files with extension "
+            + extension
+            + " found in directory "
+            + path_to_files
         )
     return f_list
 
 
 def read_yaml_config(site: str) -> tuple[dict, dict]:
     """Reads config yaml files."""
-    dir_name = os.path.dirname(__file__)
-    site_config_file = os.path.join(dir_name, "site_config", site, "config.yaml")
-    if not os.path.exists(site_config_file):
-        raise NotImplementedError(
-            f"Site config file {site_config_file} does not exist."
-        )
-
-    with open(site_config_file, "r", encoding="utf8") as f:
-        params = yaml.load(f, Loader=SafeLoader)["params"]
-
-    global_specs = {
-        "title": "HATPRO Level 1B data",
-    }
-    site_config = {
-        "global_specs": global_specs,
-        "params": params,
-    }
-    inst_file = os.path.join(dir_name, "site_config/hatpro.yaml")
+    dir_name = os.path.dirname(os.path.realpath(__file__))
+    site_file = os.path.join(dir_name, "site_config", site, "config.yaml")
+    with open(site_file, "r", encoding="utf8") as f:
+        site_config = yaml.load(f, Loader=SafeLoader)
+    inst_file = os.path.join(dir_name, "site_config", f"{site_config['type']}.yaml")
     with open(inst_file, "r", encoding="utf8") as f:
         inst_config = yaml.load(f, Loader=SafeLoader)
     inst_config["global_specs"].update(site_config["global_specs"])
     for name in inst_config["params"].keys():
         site_config["params"][name] = inst_config["params"][name]
 
     return inst_config["global_specs"], site_config["params"]
 
 
 def update_lev1_attributes(attributes: dict, data_type: str) -> None:
     """Removes attributes that are not needed for specified Level 1 data type"""
+
     if data_type == "1B01":
         att_del = ["ir_instrument", "met_instrument", "_accuracy"]
         key = " "
     elif data_type == "1B11":
         att_del = [
             "instrument_manufacturer",
             "instrument_model",
@@ -442,32 +436,32 @@
 
     return result
 
 
 def date_string_to_date(date_string: str) -> datetime.date:
     """Convert YYYY-MM-DD to Python date."""
     date_arr = [int(x) for x in date_string.split("-")]
-    return date(*date_arr)
+    return datetime.date(*date_arr)
 
 
 def get_time() -> str:
     """Returns current UTC-time."""
-    return f"{datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')} +00:00"
+    return f"{datetime.datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')} +00:00"
 
 
 def get_date_from_past(n: int, reference_date: str | None = None) -> str:
     """Return date N-days ago.
     Args:
         n: Number of days to skip (can be negative, when it means the future).
         reference_date: Date as "YYYY-MM-DD". Default is the current date.
     Returns:
         str: Date as "YYYY-MM-DD".
     """
     reference = reference_date or get_time().split()[0]
-    the_date = date_string_to_date(reference) - timedelta(n)
+    the_date = date_string_to_date(reference) - datetime.timedelta(n)
     return str(the_date)
 
 
 def get_processing_dates(args) -> tuple[str, str]:
     """Returns processing dates."""
     if args.date is not None:
         start_date = args.date
@@ -477,21 +471,21 @@
         stop_date = args.stop
     start_date = str(date_string_to_date(start_date))
     stop_date = str(date_string_to_date(stop_date))
     return start_date, stop_date
 
 
 def isodate2date(date_str: str) -> datetime.date:
-    return datetime.strptime(date_str, "%Y-%m-%d").date()
+    return datetime.datetime.strptime(date_str, "%Y-%m-%d").date()
 
 
 def date_range(
     start_date: datetime.date, end_date: datetime.date
 ) -> Iterator[datetime.date]:
     """Returns range between two dates (datetimes)."""
     for n in range(int((end_date - start_date).days)):
-        yield start_date + timedelta(n)
+        yield start_date + datetime.timedelta(n)
 
 
 def time_to_datetime_index(time_array: np.ndarray) -> pd.DatetimeIndex:
     time_units = "s" if max(time_array) > 25 else "h"
     return pd.to_datetime(time_array, unit=time_units)
```

### Comparing `mwrpy-0.2.0/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.3.0/mwrpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 mwrpy/__init__.py
 mwrpy/atmos.py
 mwrpy/cli.py
 mwrpy/constants.py
 mwrpy/process_mwrpy.py
 mwrpy/py.typed
 mwrpy/rpg_mwr.py
```

