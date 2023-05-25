# Comparing `tmp/eFatura-1.0.5.tar.gz` & `tmp/eFatura-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.5.tar", last modified: Tue May 23 14:14:52 2023, max compression
+gzip compressed data, was "eFatura-1.0.6.tar", last modified: Thu May 25 11:22:21 2023, max compression
```

## Comparing `eFatura-1.0.5.tar` & `eFatura-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 14:14:26.000000 eFatura-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 14:14:52.895744 eFatura-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-23 14:14:26.000000 eFatura-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-23 14:14:26.000000 eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-23 14:14:26.000000 eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-23 14:14:26.000000 eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/eFatura/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/eFatura/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/eFatura/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/eFatura/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/eFatura/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:14:52.895744 eFatura-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-23 14:14:26.000000 eFatura-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.706045 eFatura-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 11:21:44.000000 eFatura-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-25 11:22:21.706045 eFatura-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-25 11:21:44.000000 eFatura-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.702045 eFatura-1.0.6/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 11:21:44.000000 eFatura-1.0.6/Shared/org.KekikAkademi.eFatura.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-25 11:21:44.000000 eFatura-1.0.6/Shared/org.KekikAkademi.eFatura.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-25 11:21:44.000000 eFatura-1.0.6/Shared/org.KekikAkademi.eFatura.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.702045 eFatura-1.0.6/eFatura/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.702045 eFatura-1.0.6/eFatura/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.702045 eFatura-1.0.6/eFatura/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.702045 eFatura-1.0.6/eFatura/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.706045 eFatura-1.0.6/eFatura/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-25 11:21:44.000000 eFatura-1.0.6/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:22:21.702045 eFatura-1.0.6/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-25 11:22:21.000000 eFatura-1.0.6/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 11:22:21.000000 eFatura-1.0.6/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:22:21.000000 eFatura-1.0.6/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 11:22:21.000000 eFatura-1.0.6/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 11:22:21.000000 eFatura-1.0.6/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 11:22:21.000000 eFatura-1.0.6/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:22:21.706045 eFatura-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-25 11:21:44.000000 eFatura-1.0.6/setup.py
```

### Comparing `eFatura-1.0.5/PKG-INFO` & `eFatura-1.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,20 @@
-Metadata-Version: 2.1
-Name: eFatura
-Version: 1.0.5
-Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
-Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: eFatura,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
-# 🔍 eFatura
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/Shared/org.KekikAkademi.eFatura.svg"></a> eFatura
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/releases)
 [![Fonksiyon Testleri ve PyPI Yükle](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml)
 [![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml)
 
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.eFatura)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.eFatura)
+
 [![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/eFatura)
 [![PyPI - Yüklenme](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/eFatura)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eFatura)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#)
@@ -46,14 +34,24 @@
 # Yüklemek
 pip install eFatura
 
 # Güncellemek
 pip install -U eFatura
 ```
 
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/flathub.svg"></a> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.KekikAkademi.eFatura
+
+# Çalıştırmak
+flatpak run org.KekikAkademi.eFatura
+```
+
 ## 📝 Kullanım
 
 ### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from eFatura import e_fatura
 
@@ -70,16 +68,19 @@
 # » [~] 11111111111 Numarası E-Fatura Mükellefi Değildir..
 ```
 
 ### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 eFaturaGUI
-```
 
+# veya
+
+flatpak run org.KekikAkademi.eFatura
+```
 
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
       <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
@@ -158,8 +159,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,58 +1,61 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.5 Summary: Vergi veya TC
-Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
-github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
-keyiflerolsun@gmail.com License: GPLv3+ Keywords:
-eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
-Production/Stable Classifier: License :: OSI Approved :: GNU General Public
-License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð eFatura
-[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/
-eFatura?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
-release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/
-keyiflerolsun/eFatura/releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://
-img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/
+# [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/Shared/
+org.KekikAkademi.eFatura.svg] eFatura [![Boyut](https://img.shields.io/github/
+repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#) [!
+[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)]
+(#) [https://img.shields.io/badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub]
+(https://img.shields.io/github/v/release/keyiflerolsun/
+eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/
+releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://img.shields.io/github/
+actions/workflow/status/keyiflerolsun/eFatura/
 test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml) [![Flatpak
 YÃ¼kleyici](https://img.shields.io/github/actions/workflow/status/
 keyiflerolsun/eFatura/
 flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
-github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [![PyPI]
-(https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)]
-(https://pypi.org/project/eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/
-pypi/dm/eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/
-project/eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [!
+[FlatHub](https://img.shields.io/flathub/v/
+org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=FlatHub)](https://
+flathub.org/tr/apps/org.KekikAkademi.eFatura) [![FlatHub - YÃ¼klenme](https://
+img.shields.io/flathub/downloads/
+org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:/
+/flathub.org/tr/apps/org.KekikAkademi.eFatura) [![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/
+eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/pypi/dm/
+eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
+eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
 eFatura) [![Python Version](https://img.shields.io/pypi/pyversions/
 eFatura?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#) [!
 [Durum](https://img.shields.io/pypi/status/
 eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#) *Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![eFatura](https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)](#)
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
 (https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
 GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg]
 PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install eFatura # GÃ¼ncellemek
-pip install -U eFatura ``` ## ð KullanÄ±m ### [https://
+pip install -U eFatura ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/eFatura/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.KekikAkademi.eFatura # ÃalÄ±ÅtÄ±rmak
+flatpak run org.KekikAkademi.eFatura ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg]
 Lib ```python from eFatura import e_fatura print(e_fatura("11111111111")) #
 Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg]
 CLI ```bash eFatura 11111111111 # Â» [~] 11111111111 NumarasÄ± E-Fatura
 MÃ¼kellefi DeÄildir.. ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg] UI ```bash eFaturaGUI
-``` ---   [https://raw.githubusercontent.com/keyiflerolsun/eFatura/
-main/.github/icons/buddy.svg] Kendiniz Paketlemek Ä°sterseniz (geniÅletmek
-iÃ§in tÄ±klayÄ±n!)
+# veya flatpak run org.KekikAkademi.eFatura ``` ---   [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg]
+Kendiniz Paketlemek Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/eFatura.git cd eFatura # Gerekli OrtamlarÄ± Kur pip install -
 U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
 rf build *.egg-info # ÃalÄ±ÅtÄ±r eFatura # CLI eFaturaGUI # GUI # Paketi
 KaldÄ±r pip uninstall eFatura ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/eFatura/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
```

### Comparing `eFatura-1.0.5/README.md` & `eFatura-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,35 @@
-# 🔍 eFatura
+Metadata-Version: 2.1
+Name: eFatura
+Version: 1.0.6
+Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
+Home-page: https://github.com/keyiflerolsun/eFatura
+Author: keyiflerolsun
+Author-email: keyiflerolsun@gmail.com
+License: GPLv3+
+Keywords: eFatura,KekikAkademi,keyiflerolsun
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/Shared/org.KekikAkademi.eFatura.svg"></a> eFatura
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/releases)
 [![Fonksiyon Testleri ve PyPI Yükle](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml)
 [![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml)
 
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.eFatura)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.eFatura)
+
 [![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/eFatura)
 [![PyPI - Yüklenme](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/eFatura)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eFatura)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#)
@@ -31,14 +49,24 @@
 # Yüklemek
 pip install eFatura
 
 # Güncellemek
 pip install -U eFatura
 ```
 
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/flathub.svg"></a> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.KekikAkademi.eFatura
+
+# Çalıştırmak
+flatpak run org.KekikAkademi.eFatura
+```
+
 ## 📝 Kullanım
 
 ### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from eFatura import e_fatura
 
@@ -55,16 +83,19 @@
 # » [~] 11111111111 Numarası E-Fatura Mükellefi Değildir..
 ```
 
 ### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 eFaturaGUI
-```
 
+# veya
+
+flatpak run org.KekikAkademi.eFatura
+```
 
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
       <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
@@ -143,8 +174,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,50 +1,69 @@
-# ð eFatura [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/
-eFatura?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
-release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/
-keyiflerolsun/eFatura/releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://
-img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.6 Summary: Vergi veya TC
+Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
+github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
+keyiflerolsun@gmail.com License: GPLv3+ Keywords:
+eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/Shared/
+org.KekikAkademi.eFatura.svg] eFatura [![Boyut](https://img.shields.io/github/
+repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#) [!
+[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)]
+(#) [https://img.shields.io/badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub]
+(https://img.shields.io/github/v/release/keyiflerolsun/
+eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/
+releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://img.shields.io/github/
+actions/workflow/status/keyiflerolsun/eFatura/
 test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml) [![Flatpak
 YÃ¼kleyici](https://img.shields.io/github/actions/workflow/status/
 keyiflerolsun/eFatura/
 flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
-github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [![PyPI]
-(https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)]
-(https://pypi.org/project/eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/
-pypi/dm/eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/
-project/eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [!
+[FlatHub](https://img.shields.io/flathub/v/
+org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=FlatHub)](https://
+flathub.org/tr/apps/org.KekikAkademi.eFatura) [![FlatHub - YÃ¼klenme](https://
+img.shields.io/flathub/downloads/
+org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:/
+/flathub.org/tr/apps/org.KekikAkademi.eFatura) [![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/
+eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/pypi/dm/
+eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
+eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
 eFatura) [![Python Version](https://img.shields.io/pypi/pyversions/
 eFatura?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#) [!
 [Durum](https://img.shields.io/pypi/status/
 eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#) *Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![eFatura](https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)](#)
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
 (https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
 GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg]
 PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install eFatura # GÃ¼ncellemek
-pip install -U eFatura ``` ## ð KullanÄ±m ### [https://
+pip install -U eFatura ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/eFatura/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.KekikAkademi.eFatura # ÃalÄ±ÅtÄ±rmak
+flatpak run org.KekikAkademi.eFatura ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg]
 Lib ```python from eFatura import e_fatura print(e_fatura("11111111111")) #
 Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg]
 CLI ```bash eFatura 11111111111 # Â» [~] 11111111111 NumarasÄ± E-Fatura
 MÃ¼kellefi DeÄildir.. ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg] UI ```bash eFaturaGUI
-``` ---   [https://raw.githubusercontent.com/keyiflerolsun/eFatura/
-main/.github/icons/buddy.svg] Kendiniz Paketlemek Ä°sterseniz (geniÅletmek
-iÃ§in tÄ±klayÄ±n!)
+# veya flatpak run org.KekikAkademi.eFatura ``` ---   [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg]
+Kendiniz Paketlemek Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/eFatura.git cd eFatura # Gerekli OrtamlarÄ± Kur pip install -
 U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
 rf build *.egg-info # ÃalÄ±ÅtÄ±r eFatura # CLI eFaturaGUI # GUI # Paketi
 KaldÄ±r pip uninstall eFatura ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/eFatura/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
```

### Comparing `eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.0.6/Shared/org.KekikAkademi.eFatura.appdata.xml`

 * *Files 13% similar despite different names*

#### Comparing `eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.0.6/Shared/org.KekikAkademi.eFatura.appdata.xml`

```diff
@@ -28,12 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.0.6" date="2023-5-23">
+      <p>Çeşitli iyileştirmeler yapıldı..</p>
+    </release>
     <release version="1.0.5" date="2023-5-23"/>
     <release version="0.0.1" date="2022-8-13"/>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.svg` & `eFatura-1.0.6/Shared/org.KekikAkademi.eFatura.svg`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/eFatura/Assets/logo.png` & `eFatura-1.0.6/eFatura/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/eFatura/Core/__init__.py` & `eFatura-1.0.6/eFatura/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/eFatura/GUI/__init__.py` & `eFatura-1.0.6/eFatura/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/eFatura/Libs/Oturum.py` & `eFatura-1.0.6/eFatura/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/eFatura/konsol.py` & `eFatura-1.0.6/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/eFatura.egg-info/PKG-INFO` & `eFatura-1.0.6/eFatura.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.5
+Version: 1.0.6
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
-Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
+Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# 🔍 eFatura
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/Shared/org.KekikAkademi.eFatura.svg"></a> eFatura
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/releases)
 [![Fonksiyon Testleri ve PyPI Yükle](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml)
 [![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml)
 
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.eFatura)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.eFatura)
+
 [![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/eFatura)
 [![PyPI - Yüklenme](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/eFatura)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eFatura)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#)
@@ -46,14 +49,24 @@
 # Yüklemek
 pip install eFatura
 
 # Güncellemek
 pip install -U eFatura
 ```
 
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/flathub.svg"></a> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.KekikAkademi.eFatura
+
+# Çalıştırmak
+flatpak run org.KekikAkademi.eFatura
+```
+
 ## 📝 Kullanım
 
 ### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from eFatura import e_fatura
 
@@ -70,16 +83,19 @@
 # » [~] 11111111111 Numarası E-Fatura Mükellefi Değildir..
 ```
 
 ### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 eFaturaGUI
-```
 
+# veya
+
+flatpak run org.KekikAkademi.eFatura
+```
 
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
       <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
```

#### html2text {}

```diff
@@ -1,58 +1,69 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.5 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.6 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
-github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
+github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð eFatura
-[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/
-eFatura?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
-release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/
-keyiflerolsun/eFatura/releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://
-img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/
+Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/Shared/
+org.KekikAkademi.eFatura.svg] eFatura [![Boyut](https://img.shields.io/github/
+repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#) [!
+[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)]
+(#) [https://img.shields.io/badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub]
+(https://img.shields.io/github/v/release/keyiflerolsun/
+eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/
+releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://img.shields.io/github/
+actions/workflow/status/keyiflerolsun/eFatura/
 test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml) [![Flatpak
 YÃ¼kleyici](https://img.shields.io/github/actions/workflow/status/
 keyiflerolsun/eFatura/
 flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
-github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [![PyPI]
-(https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)]
-(https://pypi.org/project/eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/
-pypi/dm/eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/
-project/eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [!
+[FlatHub](https://img.shields.io/flathub/v/
+org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=FlatHub)](https://
+flathub.org/tr/apps/org.KekikAkademi.eFatura) [![FlatHub - YÃ¼klenme](https://
+img.shields.io/flathub/downloads/
+org.KekikAkademi.eFatura?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:/
+/flathub.org/tr/apps/org.KekikAkademi.eFatura) [![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/
+eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/pypi/dm/
+eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
+eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
 eFatura) [![Python Version](https://img.shields.io/pypi/pyversions/
 eFatura?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#) [!
 [Durum](https://img.shields.io/pypi/status/
 eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#) *Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![eFatura](https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)](#)
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
 (https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
 GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg]
 PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install eFatura # GÃ¼ncellemek
-pip install -U eFatura ``` ## ð KullanÄ±m ### [https://
+pip install -U eFatura ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/eFatura/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.KekikAkademi.eFatura # ÃalÄ±ÅtÄ±rmak
+flatpak run org.KekikAkademi.eFatura ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg]
 Lib ```python from eFatura import e_fatura print(e_fatura("11111111111")) #
 Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ### [https://
 raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg]
 CLI ```bash eFatura 11111111111 # Â» [~] 11111111111 NumarasÄ± E-Fatura
 MÃ¼kellefi DeÄildir.. ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg] UI ```bash eFaturaGUI
-``` ---   [https://raw.githubusercontent.com/keyiflerolsun/eFatura/
-main/.github/icons/buddy.svg] Kendiniz Paketlemek Ä°sterseniz (geniÅletmek
-iÃ§in tÄ±klayÄ±n!)
+# veya flatpak run org.KekikAkademi.eFatura ``` ---   [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg]
+Kendiniz Paketlemek Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/eFatura.git cd eFatura # Gerekli OrtamlarÄ± Kur pip install -
 U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
 rf build *.egg-info # ÃalÄ±ÅtÄ±r eFatura # CLI eFaturaGUI # GUI # Paketi
 KaldÄ±r pip uninstall eFatura ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/eFatura/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
```

### Comparing `eFatura-1.0.5/eFatura.egg-info/SOURCES.txt` & `eFatura-1.0.6/eFatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.5/setup.py` & `eFatura-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.5",
-    url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
+    version      = "1.0.6",
+    url          = "https://github.com/keyiflerolsun/eFatura",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     license      = "GPLv3+",
```

