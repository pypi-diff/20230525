# Comparing `tmp/ramanchada2-0.0.5.tar.gz` & `tmp/ramanchada2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanchada2-0.0.5.tar", last modified: Thu May  4 11:00:05 2023, max compression
+gzip compressed data, was "ramanchada2-0.0.6.tar", last modified: Mon May 15 23:58:25 2023, max compression
```

## Comparing `ramanchada2-0.0.5.tar` & `ramanchada2-0.0.6.tar`

### file list

```diff
@@ -1,242 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.547141 ramanchada2-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/README.pypi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:00:05.547141 ramanchada2-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.491141 ramanchada2-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.503141 ramanchada2-0.0.5/src/ramanchada2/
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.503141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.503141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.503141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.507141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/
--rw-r--r--   0 runner    (1001) docker     (123)   185598 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184263 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187339 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187743 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   190431 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189952 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187633 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187638 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   191297 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187259 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.519141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35649 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171476 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35658 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171859 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35712 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171856 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16841 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171894 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35718 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171856 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35694 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171844 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171846 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35695 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171923 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35687 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171889 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.527141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/
--rw-r--r--   0 runner    (1001) docker     (123)   182699 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184528 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   182774 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184434 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174788 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175407 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175468 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174802 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175123 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174660 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175356 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174887 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174718 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   173754 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   176673 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   177120 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174707 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175243 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.531141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/
--rw-r--r--   0 runner    (1001) docker     (123)   184364 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185045 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185328 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189806 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   201634 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189411 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189005 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187207 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187573 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   186787 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189400 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189244 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   188792 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185773 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185317 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184476 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   183722 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184176 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184535 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184428 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184511 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184796 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/
--rw-r--r--   0 runner    (1001) docker     (123)   101150 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101182 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101185 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101119 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101189 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101169 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101184 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101184 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101413 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/HSDS.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/bw_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/read_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/experimental/two_column_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/output/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/output/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/simulated/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/simulated/crystal/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/crystal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/lines_from_raw_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/read_simulated_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/io/simulated/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.535141 ramanchada2-0.0.5/src/ramanchada2/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    23672 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/plottable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/dynamically_added.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/spectrum_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/misc/types/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/fit_peaks_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/peak_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/positive_not_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/pydantic_base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/misc/types/spectrum/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/spectrum/applied_processings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/types/spectrum/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/misc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/utils/argmin2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/misc/utils/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/spectral_components/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/spectral_components/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/baseline/analytical.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/baseline/baseline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/baseline/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/voigt.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/spectral_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/spectral_component_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectral_components/spectral_peak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/spectrum/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/spectrum/arithmetics/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/arithmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/arithmetics/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/arithmetics/mul.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/arithmetics/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/arithmetics/truediv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.539141 ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/baseline_rc1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/moving_minimum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/src/ramanchada2/spectrum/calc/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calc/central_moments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/by_deltas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/change_x_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/scale_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/scale_yaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/set_new_xaxis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_cache_or_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_chada.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_delta_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_test_spe.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_theoretical_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/add_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/add_poisson_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/drop_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/pad_zeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/sharpen_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/trim_axes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/spectrum/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.543141 ramanchada2-0.0.5/src/ramanchada2/theoretical_lines/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/theoretical_lines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-04 10:59:54.000000 ramanchada2-0.0.5/src/ramanchada2/theoretical_lines/model_from_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:05.503141 ramanchada2-0.0.5/src/ramanchada2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 11:00:05.000000 ramanchada2-0.0.5/src/ramanchada2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-04 11:00:05.000000 ramanchada2-0.0.5/src/ramanchada2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:00:05.000000 ramanchada2-0.0.5/src/ramanchada2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 11:00:05.000000 ramanchada2-0.0.5/src/ramanchada2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 11:00:05.000000 ramanchada2-0.0.5/src/ramanchada2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.410306 ramanchada2-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-15 23:58:25.410306 ramanchada2-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 23:58:25.410306 ramanchada2-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.338305 ramanchada2-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.346305 ramanchada2-0.0.6/src/ramanchada2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.346305 ramanchada2-0.0.6/src/ramanchada2/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.346305 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.346305 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.354306 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/
+-rw-r--r--   0 runner    (1001) docker     (123)   185598 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184263 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187339 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187743 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   190431 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   189952 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187633 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187638 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   191297 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187259 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.362305 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/
+-rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35649 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171476 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35658 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171859 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35712 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171856 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16841 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171894 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35718 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171856 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35694 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171844 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171846 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35695 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171923 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35687 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171889 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.366306 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/
+-rw-r--r--   0 runner    (1001) docker     (123)   182699 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184528 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   182774 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184434 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   174788 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175407 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175468 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   174802 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175123 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   174660 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175356 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   174887 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   174718 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   173754 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   176673 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   177120 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   174707 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175243 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.378306 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/
+-rw-r--r--   0 runner    (1001) docker     (123)   184364 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   185045 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   185328 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   189806 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   201634 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   189411 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   189005 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187207 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   187573 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   186787 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   189400 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   189244 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   188792 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   185773 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   185317 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184476 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   183722 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184176 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184535 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184428 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184511 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   184796 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.382306 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/
+-rw-r--r--   0 runner    (1001) docker     (123)   101150 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101182 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101185 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101119 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101189 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101169 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101184 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101184 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101413 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.382306 ramanchada2-0.0.6/src/ramanchada2/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/HSDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.382306 ramanchada2-0.0.6/src/ramanchada2/io/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/bw_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.386306 ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/read_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/experimental/two_column_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.386306 ramanchada2-0.0.6/src/ramanchada2/io/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/output/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.386306 ramanchada2-0.0.6/src/ramanchada2/io/simulated/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.390306 ramanchada2-0.0.6/src/ramanchada2/io/simulated/crystal/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/crystal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/lines_from_raw_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/read_simulated_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.390306 ramanchada2-0.0.6/src/ramanchada2/io/simulated/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.390306 ramanchada2-0.0.6/src/ramanchada2/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23672 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/plottable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.390306 ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/dynamically_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/spectrum_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.394306 ramanchada2-0.0.6/src/ramanchada2/misc/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/fit_peaks_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/peak_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/positive_not_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/pydantic_base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.398306 ramanchada2-0.0.6/src/ramanchada2/misc/types/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/spectrum/applied_processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/types/spectrum/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.398306 ramanchada2-0.0.6/src/ramanchada2/misc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/utils/argmin2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/misc/utils/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.402306 ramanchada2-0.0.6/src/ramanchada2/spectral_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.402306 ramanchada2-0.0.6/src/ramanchada2/spectral_components/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/baseline/analytical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/baseline/baseline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/baseline/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.402306 ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/voigt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/spectral_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/spectral_component_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectral_components/spectral_peak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.402306 ramanchada2-0.0.6/src/ramanchada2/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.402306 ramanchada2-0.0.6/src/ramanchada2/spectrum/arithmetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/arithmetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/arithmetics/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/arithmetics/mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/arithmetics/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/arithmetics/truediv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.406306 ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/baseline_rc1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/moving_minimum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.406306 ramanchada2-0.0.6/src/ramanchada2/spectrum/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calc/central_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.406306 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/by_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/change_x_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/scale_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/scale_yaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/set_new_xaxis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.406306 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_cache_or_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_chada.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_delta_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_test_spe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_theoretical_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.410306 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/add_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/add_poisson_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/drop_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/pad_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/sharpen_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/trim_axes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.410306 ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/spectrum/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.410306 ramanchada2-0.0.6/src/ramanchada2/theoretical_lines/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/theoretical_lines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-15 23:58:12.000000 ramanchada2-0.0.6/src/ramanchada2/theoretical_lines/model_from_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:25.346305 ramanchada2-0.0.6/src/ramanchada2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-15 23:58:25.000000 ramanchada2-0.0.6/src/ramanchada2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-15 23:58:25.000000 ramanchada2-0.0.6/src/ramanchada2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:58:25.000000 ramanchada2-0.0.6/src/ramanchada2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 23:58:25.000000 ramanchada2-0.0.6/src/ramanchada2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 23:58:25.000000 ramanchada2-0.0.6/src/ramanchada2.egg-info/top_level.txt
```

### Comparing `ramanchada2-0.0.5/LICENSE` & `ramanchada2-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/PKG-INFO` & `ramanchada2-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanchada2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Harmonising Raman Spectroscopy
 Home-page: https://github.com/h2020charisma/ramanchada2
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ramanchada2-0.0.5/README.md` & `ramanchada2-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/README.pypi` & `ramanchada2-0.0.6/README.pypi`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/setup.py` & `ramanchada2-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/__init__.py` & `ramanchada2-0.0.6/src/ramanchada2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 """
 
 from __future__ import annotations
 
 from . import spectrum
 from . import theoretical_lines
 __all__ = ['spectrum', 'theoretical_lines']
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 
 import logging
 
 
 class CustomFormatter(logging.Formatter):
     green = "\x1b[32m"
```

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py` & `ramanchada2-0.0.6/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/HSDS.py` & `ramanchada2-0.0.6/src/ramanchada2/io/HSDS.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/bw_format.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/bw_format.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/io.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/io.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/read_csv.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/read_csv.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/experimental/read_txt.py` & `ramanchada2-0.0.6/src/ramanchada2/io/experimental/read_txt.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py` & `ramanchada2-0.0.6/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py` & `ramanchada2-0.0.6/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/simulated/read_simulated_lines.py` & `ramanchada2-0.0.6/src/ramanchada2/io/simulated/read_simulated_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py` & `ramanchada2-0.0.6/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/base_class.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/base_class.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/constants.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/constants.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/types/fit_peaks_result.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/types/fit_peaks_result.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/types/peak_candidates.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/types/peak_candidates.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/types/positive_not_multiple.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/types/positive_not_multiple.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/types/spectrum/applied_processings.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/types/spectrum/applied_processings.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/types/spectrum/metadata.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/types/spectrum/metadata.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/utils/__init__.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/utils/argmin2d.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/utils/argmin2d.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py` & `ramanchada2-0.0.6/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/delta.py` & `ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/delta.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectral_components/peak_profile/gauss.py` & `ramanchada2-0.0.6/src/ramanchada2/spectral_components/peak_profile/gauss.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectral_components/spectral_component_collection.py` & `ramanchada2-0.0.6/src/ramanchada2/spectral_components/spectral_component_collection.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectral_components/spectral_peak.py` & `ramanchada2-0.0.6/src/ramanchada2/spectral_components/spectral_peak.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/__init__.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from .creators.from_chada import from_chada
 from .creators.from_local_file import from_local_file
 from .creators.from_simulation import from_simulation
 from .creators.from_theoretical_lines import from_theoretical_lines
 from .creators.from_spectral_component_collection import from_spectral_component_collection
 from .creators.from_delta_lines import from_delta_lines
 from .creators.from_test_spe import from_test_spe
+from .creators.hdr_from_multi_exposure import hdr_from_multi_exposure
 
 
 __all__ = ['Spectrum',
            'from_cache_or_calc',
            'from_chada',
            'from_local_file',
            'from_simulation',
            'from_test_spe',
            'from_theoretical_lines',
            'from_spectral_component_collection',
            'from_delta_lines',
+           'hdr_from_multi_exposure',
            ]
```

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/add_baseline.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/add_baseline.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/baseline_rc1.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/baseline_rc1.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/baseline/moving_minimum.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/baseline/moving_minimum.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/calc/central_moments.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/calc/central_moments.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/by_deltas.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/by_deltas.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/change_x_units.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/change_x_units.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/normalize.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/normalize.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/scale_xaxis.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/scale_xaxis.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/calibration/set_new_xaxis.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/calibration/set_new_xaxis.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_cache_or_calc.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_cache_or_calc.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_delta_lines.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_delta_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_local_file.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_local_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,74 @@
 #!/usr/bin/env python3
 """Create spectrum from local files."""
 
 from typing import Literal, Union
 
 from pydantic import validate_arguments
 
+import os
 from ..spectrum import Spectrum
 from ramanchada2.misc.types import SpeMetadataModel
 from ramanchada2.misc.spectrum_deco import add_spectrum_constructor
 from ramanchada2.io.experimental import read_txt, read_csv, rc1_parser
 
 
 @add_spectrum_constructor()
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
 def from_local_file(
         in_file_name: str,
         filetype: Union[None, Literal['spc', 'sp', 'spa', '0', '1', '2',
                                       'wdf', 'ngs', 'jdx', 'dx',
                                       'txt', 'txtr', 'csv', 'prn', 'rruf']] = None,
-        backend: Literal['native', 'rc1_parser'] = 'rc1_parser'):
+        backend: Union[None, Literal['native', 'rc1_parser']] = None):
     """
     Read experimental spectrum from a local file.
 
     Parameters
     ----------
     in_file_name : str
         path to a local file, containing a spectrum
     filetype : optional, default is None
         Specify the filetype. Filetype can be any of:
         `spc`, `sp`, `spa`, `0`, `1`, `2`, `wdf`, `ngs`, `jdx`,
         `dx`, `txt`, `txtr`, `csv`, `prn`, `rruf` or `None`
         `None` used to determine by extension of the file.
-    backend : Literal['native', 'rc1_parser'], default 'native'
+    backend : Literal['native', 'rc1_parser'], default None==both
 
     Raises
     ------
     ValueError
         When called with unsupported file formats
     """
-    if backend == 'native':
-        if filetype in {'txt', 'txtr', 'prn', 'rruf'}:
+    def load_native():
+        if filetype is None:
+            ft = os.path.splitext(in_file_name)[1][1:]
+        else:
+            ft = filetype
+        if ft in {'txt', 'txtr', 'prn', 'rruf'}:
             with open(in_file_name) as fp:
                 x, y, meta = read_txt(fp)
-                spe = Spectrum(x=x, y=y, metadata=meta)  # type: ignore
-        elif filetype in {'csv'}:
+        elif ft in {'csv'}:
             with open(in_file_name) as fp:
                 x, y, meta = read_csv(fp)
-                spe = Spectrum(x=x, y=y, metadata=meta)  # type: ignore
         else:
-            raise ValueError(f'filetype {filetype} not supported')
-    elif backend == 'rc1_parser':
+            raise ValueError(f'filetype {ft} not supported')
+        meta["Original file"] = os.path.basename(in_file_name)
+        spe = Spectrum(x=x, y=y, metadata=meta)  # type: ignore
+        return spe
+
+    def load_rc1():
         x, y, meta = rc1_parser.parse(in_file_name, filetype)
         spe = Spectrum(x=x, y=y, metadata=SpeMetadataModel.parse_obj(meta))
+        return spe
+
+    if backend == 'native':
+        spe = load_native()
+    elif backend == 'rc1_parser':
+        spe = load_rc1()
+    elif backend is None:
+        try:
+            spe = load_native()
+        except Exception:
+            spe = load_rc1()
     spe._sort_x()
     return spe
```

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_simulation.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_simulation.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_test_spe.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_test_spe.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/creators/from_theoretical_lines.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/creators/from_theoretical_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/add_gaussian_noise.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/add_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/add_poisson_noise.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/add_poisson_noise.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/convolve.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/convolve.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/drop_spikes.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/drop_spikes.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/moving_average.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/moving_average.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/pad_zeros.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/pad_zeros.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/resampling.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/sharpen_lines.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/sharpen_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/smoothing.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/smoothing.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/filters/trim_axes.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/filters/trim_axes.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/find_peaks.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/fit_peaks.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/fit_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/spectrum/spectrum.py` & `ramanchada2-0.0.6/src/ramanchada2/spectrum/spectrum.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2/theoretical_lines/model_from_lines.py` & `ramanchada2-0.0.6/src/ramanchada2/theoretical_lines/model_from_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.5/src/ramanchada2.egg-info/PKG-INFO` & `ramanchada2-0.0.6/src/ramanchada2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanchada2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Harmonising Raman Spectroscopy
 Home-page: https://github.com/h2020charisma/ramanchada2
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ramanchada2-0.0.5/src/ramanchada2.egg-info/SOURCES.txt` & `ramanchada2-0.0.6/src/ramanchada2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 src/ramanchada2/spectrum/creators/from_chada.py
 src/ramanchada2/spectrum/creators/from_delta_lines.py
 src/ramanchada2/spectrum/creators/from_local_file.py
 src/ramanchada2/spectrum/creators/from_simulation.py
 src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
 src/ramanchada2/spectrum/creators/from_test_spe.py
 src/ramanchada2/spectrum/creators/from_theoretical_lines.py
+src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py
 src/ramanchada2/spectrum/filters/__init__.py
 src/ramanchada2/spectrum/filters/add_gaussian_noise.py
 src/ramanchada2/spectrum/filters/add_poisson_noise.py
 src/ramanchada2/spectrum/filters/convolve.py
 src/ramanchada2/spectrum/filters/drop_spikes.py
 src/ramanchada2/spectrum/filters/moving_average.py
 src/ramanchada2/spectrum/filters/pad_zeros.py
```

