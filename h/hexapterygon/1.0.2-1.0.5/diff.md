# Comparing `tmp/hexapterygon-1.0.2.tar.gz` & `tmp/hexapterygon-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexapterygon-1.0.2.tar", last modified: Thu Apr 27 19:59:50 2023, max compression
+gzip compressed data, was "hexapterygon-1.0.5.tar", last modified: Thu May 25 13:36:10 2023, max compression
```

## Comparing `hexapterygon-1.0.2.tar` & `hexapterygon-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-04-26 16:34:05.000000 hexapterygon-1.0.2/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)     6338 2023-04-26 18:32:42.000000 hexapterygon-1.0.2/README.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/hexapterygon/
--rw-r--r--   0 xou       (1000) xou       (1000)     1442 2023-04-04 21:25:43.000000 hexapterygon-1.0.2/hexapterygon/DeviceEvents.py
--rw-r--r--   0 xou       (1000) xou       (1000)    10725 2023-04-27 19:56:14.000000 hexapterygon-1.0.2/hexapterygon/DeviceOverlay.py
--rw-r--r--   0 xou       (1000) xou       (1000)      691 2023-04-26 17:13:52.000000 hexapterygon-1.0.2/hexapterygon/HexaGlobals.py
--rw-r--r--   0 xou       (1000) xou       (1000)    14230 2023-04-26 18:52:35.000000 hexapterygon-1.0.2/hexapterygon/HexaTUI.py
--rw-r--r--   0 xou       (1000) xou       (1000)     1506 2023-04-19 11:46:33.000000 hexapterygon-1.0.2/hexapterygon/InsortForOldPython.py
--rw-r--r--   0 xou       (1000) xou       (1000)      324 2023-04-15 09:36:08.000000 hexapterygon-1.0.2/hexapterygon/StateEnums.py
--rw-r--r--   0 xou       (1000) xou       (1000)    17981 2023-04-14 03:20:33.000000 hexapterygon-1.0.2/hexapterygon/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)     4209 2023-04-27 19:57:26.000000 hexapterygon-1.0.2/hexapterygon/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     2260 2023-04-26 18:36:02.000000 hexapterygon-1.0.2/hexapterygon/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/hexapterygon.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      495 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       60 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       38 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)      962 2023-04-27 19:57:34.000000 hexapterygon-1.0.2/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-05-25 13:36:10.164663 hexapterygon-1.0.5/
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-04-26 16:34:05.000000 hexapterygon-1.0.5/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-05-25 13:36:10.164663 hexapterygon-1.0.5/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)     7369 2023-05-25 13:20:31.000000 hexapterygon-1.0.5/README.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-05-25 13:36:10.161330 hexapterygon-1.0.5/hexapterygon/
+-rw-r--r--   0 xou       (1000) xou       (1000)     1442 2023-04-04 21:25:43.000000 hexapterygon-1.0.5/hexapterygon/DeviceEvents.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    11276 2023-05-25 13:20:31.000000 hexapterygon-1.0.5/hexapterygon/DeviceOverlay.py
+-rw-r--r--   0 xou       (1000) xou       (1000)      691 2023-04-26 17:13:52.000000 hexapterygon-1.0.5/hexapterygon/HexaGlobals.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    14046 2023-05-25 13:30:26.000000 hexapterygon-1.0.5/hexapterygon/HexaTUI.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1506 2023-04-19 11:46:33.000000 hexapterygon-1.0.5/hexapterygon/InsortForOldPython.py
+-rw-r--r--   0 xou       (1000) xou       (1000)      324 2023-04-15 09:36:08.000000 hexapterygon-1.0.5/hexapterygon/StateEnums.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    17981 2023-04-14 03:20:33.000000 hexapterygon-1.0.5/hexapterygon/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     4209 2023-05-25 13:20:31.000000 hexapterygon-1.0.5/hexapterygon/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     2260 2023-04-26 18:36:02.000000 hexapterygon-1.0.5/hexapterygon/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-05-25 13:36:10.164663 hexapterygon-1.0.5/hexapterygon.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-05-25 13:36:10.000000 hexapterygon-1.0.5/hexapterygon.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      530 2023-05-25 13:36:10.000000 hexapterygon-1.0.5/hexapterygon.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-05-25 13:36:10.000000 hexapterygon-1.0.5/hexapterygon.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       60 2023-05-25 13:36:10.000000 hexapterygon-1.0.5/hexapterygon.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-05-25 13:36:10.000000 hexapterygon-1.0.5/hexapterygon.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-05-25 13:36:10.000000 hexapterygon-1.0.5/hexapterygon.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       38 2023-05-25 13:36:10.164663 hexapterygon-1.0.5/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)      962 2023-05-25 13:20:31.000000 hexapterygon-1.0.5/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-05-25 13:36:10.164663 hexapterygon-1.0.5/tests/
+-rw-r--r--   0 xou       (1000) xou       (1000)     2400 2023-04-26 16:34:49.000000 hexapterygon-1.0.5/tests/test.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     3104 2023-04-26 16:34:49.000000 hexapterygon-1.0.5/tests/test_thread.py
```

### Comparing `hexapterygon-1.0.2/LICENSE` & `hexapterygon-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.2/README.md` & `hexapterygon-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,34 @@
 <h1></h1>
 </div>
 
 Less bloatware, less spyware, improved privacy and performance from within the experience of your stock ROM. **A user-friendly** all-in-one cross-platform, *([uni-curses](https://github.com/unicurses/unicurses) compatible component, module and uitility)* software for orchestrating and debloating your Android devices from unwanted pre-installed crap.
 
 
 # 📦 Features
-- [Uni-curses](https://github.com/unicurses/unicurses) compatible component
-- Auto removes-installs-executes
-- User-friendly \ easy-to-use
-- Can be used as a module
-- Cross-platform
+- ***Current:***
+- - [Uni-curses](https://github.com/unicurses/unicurses) compatible component
+- - Auto removes-installs-executes
+- - User-friendly \ easy-to-use
+- - Fixed-version pkg control
+- - Can be used as a module
+- - Cross-platform
+- ***Future:***
+- - Rooting
+- - Restoring 
+- - Better Security
+- - Better User-Interface
+- - [More auto-debloating lists](https://github.com/GiorgosXou/hexapterygon/tree/main/device_repo_lists)
 
 
 # ⚙️ Configure
 
 Before begining the process of debloating, make sure you:
 
+- Backed-up your personal data *(Advised)*
 - `pip install hexapterygon --upgrade`
 - Have [Android SDK Platform Tools](https://developer.android.com/studio/releases/platform-tools) installed 
 - Enabled `developer mode` & `USB debugging` *(under settings)*
 - Enabled [Security settings](## 'Allow granting permissions and simulating input via USB (if possible)') & [Install via USB](## '[INSTALL] installing won\'t work if it is not enabled') *(optionally, [usually necessary])*
 - Disabled services under `setting > ... > Device admin apps` *(optionally)*
 
 *<sup>[click here for more informations](#💭-questions)</sup>*
@@ -46,36 +55,39 @@
 ```
 ```terminal
 $ hexapterygon ./my_debloating_list.txt
 ```
 ```terminal
 $ hexapterygon ./folder_full_of_lists_named_by_type_identifier_txt
 ```
-<sup>[*(Lists should be in this form)*](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-debloating-list/blob/main/devices/Xiaomi%20Redmi%205A%20riva.txt)</sup>
+[📝 *(Lists should be in this form)*](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-debloating-list/blob/main/devices/Xiaomi%20Redmi%205A%20riva.txt) | 📱 [Demonstration of results](https://odysee.com/hexapterygon:9)
 
+<img style="center" src="./imgs/Peek.gif">
 
 # 🫴 Contribute
 ### 📜 Debloating lists
 Your lists is what makes this tool actually powerfull and user-friendly, without your list-contributions this tool can't work standalone. To contribute a list you just need to:
 
 - ***Create a new repository with a folder called `devices` where you:***
 - - Create your debloating-list(s) in the form of `{type_identifier}.txt` 
 - - - (use: `hexapterygon --getid` to get the `{type_identifier}`)
-- - - (Take as an example this list)
+- - - [(Take this list as an example)](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-debloating-list/blob/main/devices/Xiaomi%20Redmi%205A%20riva.txt)
 - ***Make a pull-request or open an issue and:*** 
 - - ask to add your repo (see `device_repo_lists`)
 
 And you are done
 
 ### 💻 To the code
 Propose whatever you want, just don't mess up with my weird indentation :P
 
 # 🗺️ Documentation
 The only documentation that you need is the code itself. JK, it is under construction 🛠️🏗️
 
+# 🔍 Research
+My research can be found under my personal debloating list [here](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-debloating-list/#research) 
 
 # 💭 Questions
 
 > How do I install [Android SDK Platform Tools](https://developer.android.com/studio/releases/platform-tools)?
 
 You either manually download the tools from the link above and install them or use your package manager to install them like for example: `sudo pacman -S android-tools` *(following this [video for windows](https://www.youtube.com/watch?v=26GI3z6tI3E))*
 
@@ -95,15 +107,15 @@
 > How do i get the {type_identifier}?
 
 Just run the command `hexapterygon --getid` *(while your authorized device is connected)*
 
 
 
 
-<!-- # 🔍 Research --> :P no! i have done way more reasearch 
+<!-- # 🔍 Research :P no! i have done way more reasearch --> 
 <!-- - ***ADB Related:*** -->
 <!-- - - ***Python Libraries:*** -->
 <!-- - - - [pure-python-adb *(Currently using)*](https://github.com/Swind/pure-python-adb) -->
 <!-- - - - [adbutils](https://github.com/openatx/adbutils) -->
 <!-- - - - [adb_shell](https://github.com/JeffLIrion/adb_shell) -->
 <!-- - - - [python-adb](https://github.com/google/python-adb) -->
 <!-- - - ***Questions:*** -->
@@ -117,16 +129,17 @@
 <!---->
 
 # 💗 Donate
 - ***[PayPal Address](https://www.paypal.com/donate/?hosted_button_id=XLWAVDMHBYACY)***
 - ***Monero Address:*** `83dxyGp3oemQvPBNKiBy61eFX9GZWruEjcNyNH2Dmgiu3HDaZ8REaoYVpGTb3AHR5ccitoKtH53wdQUN3tBJN8aMFMxhWAt`
 
 # 🕳️ Outro
-This is part 1/3 of a software series project called "beyond self destruction" which rises from within one's self
+This is part 1/3 of a software series project called "beyond self destruction" which rises from within one's self. For those wondering: "Debloating Android Devices" = "Uninstalling\Deleting preinstalled unwanted data-collecting\spyware apps and etc." = "better performance" = "Unleashing the power of self destruction"
 
-Just some reminders:
+Just some reminders *(related to phone companies)*:
+- [Greek wiretapping case 2004–05](https://en.wikipedia.org/wiki/Greek_wiretapping_case_2004%E2%80%9305)
 - [Huawei Security Scandal](https://www.forbes.com/sites/kateoflahertyuk/2019/02/26/huawei-security-scandal-everything-you-need-to-know/?sh=4a1946e473a5)
 - [(Apple's) Batterygate](https://en.wikipedia.org/wiki/Batterygate)
 
 <!-- Disable all permissions for as many apps as possibly you can. -->
 <!-- https://www.instagram.com/p/Cq0V-twIIej/ -->
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_whtme4xf_/tmp0otb5tpr_TarContainer/0/3.md", line 5, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_whtme4xf_/tmp0otb5tpr_TarContainer/0/3.md", line 5, column 2: Levels of opening and closing headings don't match*

```diff
@@ -3,63 +3,77 @@
 hexapterygon?color=%4dc71f&label=Last%20Commit&logo=github&style=flat-square]
 [https://img.shields.io/github/license/GiorgosXou/
 hexapterygon?label=License&logo=GNU&style=flat-square]
 Less bloatware, less spyware, improved privacy and performance from within the
 experience of your stock ROM. **A user-friendly** all-in-one cross-platform, *(
 [uni-curses](https://github.com/unicurses/unicurses) compatible component,
 module and uitility)* software for orchestrating and debloating your Android
-devices from unwanted pre-installed crap. # ð¦ Features - [Uni-curses](https:
-//github.com/unicurses/unicurses) compatible component - Auto removes-installs-
-executes - User-friendly \ easy-to-use - Can be used as a module - Cross-
-platform # âï¸ Configure Before begining the process of debloating, make
-sure you: - `pip install hexapterygon --upgrade` - Have [Android SDK Platform
-Tools](https://developer.android.com/studio/releases/platform-tools) installed
-- Enabled `developer mode` & `USB debugging` *(under settings)* - Enabled
-[Security settings](## 'Allow granting permissions and simulating input via USB
-(if possible)') & [Install via USB](## '[INSTALL] installing won\'t work if it
-is not enabled') *(optionally, [usually necessary])* - Disabled services under
+devices from unwanted pre-installed crap. # ð¦ Features - ***Current:*** - -
+[Uni-curses](https://github.com/unicurses/unicurses) compatible component - -
+Auto removes-installs-executes - - User-friendly \ easy-to-use - - Fixed-
+version pkg control - - Can be used as a module - - Cross-platform - ***Future:
+*** - - Rooting - - Restoring - - Better Security - - Better User-Interface - -
+[More auto-debloating lists](https://github.com/GiorgosXou/hexapterygon/tree/
+main/device_repo_lists) # âï¸ Configure Before begining the process of
+debloating, make sure you: - Backed-up your personal data *(Advised)* - `pip
+install hexapterygon --upgrade` - Have [Android SDK Platform Tools](https://
+developer.android.com/studio/releases/platform-tools) installed - Enabled
+`developer mode` & `USB debugging` *(under settings)* - Enabled [Security
+settings](## 'Allow granting permissions and simulating input via USB (if
+possible)') & [Install via USB](## '[INSTALL] installing won\'t work if it is
+not enabled') *(optionally, [usually necessary])* - Disabled services under
 `setting > ... > Device admin apps` *(optionally)* *[click here for more
 informations](#ð­-questions)* # ð¥ Debloat To begin the proccess of
 debloating you either just run `hexapterygon` in your terminal *(while your
 device is connected and configured)* or `hexapterygon` and the path-*
 (file\folder)* or repository to you debloating list(s) like: ```terminal $
 hexapterygon username/my_repository ``` ```terminal $ hexapterygon ./
 my_debloating_list.txt ``` ```terminal $ hexapterygon ./
-folder_full_of_lists_named_by_type_identifier_txt ``` [*(Lists should be in
-this form)*](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-debloating-
-list/blob/main/devices/Xiaomi%20Redmi%205A%20riva.txt) # ð«´ Contribute ###
-ð Debloating lists Your lists is what makes this tool actually powerfull and
-user-friendly, without your list-contributions this tool can't work standalone.
-To contribute a list you just need to: - ***Create a new repository with a
-folder called `devices` where you:*** - - Create your debloating-list(s) in the
-form of `{type_identifier}.txt` - - - (use: `hexapterygon --getid` to get the `
-{type_identifier}`) - - - (Take as an example this list) - ***Make a pull-
-request or open an issue and:*** - - ask to add your repo (see
+folder_full_of_lists_named_by_type_identifier_txt ``` [ð *(Lists should be
+in this form)*](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-
+debloating-list/blob/main/devices/Xiaomi%20Redmi%205A%20riva.txt) | ð±
+[Demonstration of results](https://odysee.com/hexapterygon:9) [./imgs/Peek.gif]
+# ð«´ Contribute ### ð Debloating lists Your lists is what makes this tool
+actually powerfull and user-friendly, without your list-contributions this tool
+can't work standalone. To contribute a list you just need to: - ***Create a new
+repository with a folder called `devices` where you:*** - - Create your
+debloating-list(s) in the form of `{type_identifier}.txt` - - - (use:
+`hexapterygon --getid` to get the `{type_identifier}`) - - - [(Take this list
+as an example)](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-5A-riva-
+debloating-list/blob/main/devices/Xiaomi%20Redmi%205A%20riva.txt) - ***Make a
+pull-request or open an issue and:*** - - ask to add your repo (see
 `device_repo_lists`) And you are done ### ð» To the code Propose whatever you
 want, just don't mess up with my weird indentation :P # ðºï¸ Documentation
 The only documentation that you need is the code itself. JK, it is under
-construction ð ï¸ðï¸ # ð­ Questions > How do I install [Android SDK
-Platform Tools](https://developer.android.com/studio/releases/platform-tools)?
-You either manually download the tools from the link above and install them or
-use your package manager to install them like for example: `sudo pacman -
-S android-tools` *(following this [video for windows](https://www.youtube.com/
+construction ð ï¸ðï¸ # ð Research My research can be found under my
+personal debloating list [here](https://github.com/GiorgosXou/Our-Xiaomi-Redmi-
+5A-riva-debloating-list/#research) # ð­ Questions > How do I install [Android
+SDK Platform Tools](https://developer.android.com/studio/releases/platform-
+tools)? You either manually download the tools from the link above and install
+them or use your package manager to install them like for example: `sudo pacman
+-S android-tools` *(following this [video for windows](https://www.youtube.com/
 watch?v=26GI3z6tI3E))* > How do I make sure [Android SDK Platform Tools](https:
 //developer.android.com/studio/releases/platform-tools) and `adb` are
 installed? Just run `hexapterygon` or the command `adb shell` while the phone
 is connected *(with `USB debugging` already enabled)*, a pop-up message on you
 phone should show-up, to allow the computer to connect to it > Where are
 `Device admin apps` and what do I disable? Somewhere under settings, depends on
 the device. > Why do I get a
 `github.GithubException.RateLimitExceededException` and what can I do? Most
 probably because you exceeded the github's limit for requests without a token.
 To solve this, you can either restart your rooter or provide a classic github-
 token *(without any special permissions checked)* > How do i get the
 {type_identifier}? Just run the command `hexapterygon --getid` *(while your
-authorized device is connected)*  :P no! i have done way more reasearch
-# ð Donate - ***[PayPal Address](https://www.paypal.com/donate/
-?hosted_button_id=XLWAVDMHBYACY)*** - ***Monero Address:***
+authorized device is connected)*                 # ð Donate - ***[PayPal
+Address](https://www.paypal.com/donate/?hosted_button_id=XLWAVDMHBYACY)*** -
+***Monero Address:***
 `83dxyGp3oemQvPBNKiBy61eFX9GZWruEjcNyNH2Dmgiu3HDaZ8REaoYVpGTb3AHR5ccitoKtH53wdQUN3tBJN8aMFMxhWAt`
 # ð³ï¸ Outro This is part 1/3 of a software series project called "beyond
-self destruction" which rises from within one's self Just some reminders: -
-[Huawei Security Scandal](https://www.forbes.com/sites/kateoflahertyuk/2019/02/
-26/huawei-security-scandal-everything-you-need-to-know/?sh=4a1946e473a5) - [
-(Apple's) Batterygate](https://en.wikipedia.org/wiki/Batterygate)
+self destruction" which rises from within one's self. For those wondering:
+"Debloating Android Devices" = "Uninstalling\Deleting preinstalled unwanted
+data-collecting\spyware apps and etc." = "better performance" = "Unleashing the
+power of self destruction" Just some reminders *(related to phone companies)*:
+- [Greek wiretapping case 2004â05](https://en.wikipedia.org/wiki/
+Greek_wiretapping_case_2004%E2%80%9305) - [Huawei Security Scandal](https://
+www.forbes.com/sites/kateoflahertyuk/2019/02/26/huawei-security-scandal-
+everything-you-need-to-know/?sh=4a1946e473a5) - [(Apple's) Batterygate](https:/
+/en.wikipedia.org/wiki/Batterygate)
```

### Comparing `hexapterygon-1.0.2/hexapterygon/DeviceEvents.py` & `hexapterygon-1.0.5/hexapterygon/DeviceEvents.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.2/hexapterygon/DeviceOverlay.py` & `hexapterygon-1.0.5/hexapterygon/DeviceOverlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,28 +72,38 @@
             if content_file.type == "file" or content_file.path != 'devices': continue
             for content_file in repo.get_contents("devices"):
                 if content_file.type == "dir" or content_file.path[8:] != f'{self.type_identifier}.txt': continue
                 return True
         return False
 
 
-    def get_available_repos(self): # TODO: Maybe add a limit because of the github's limit for requests (without key) [if too many lists for one device] | Maybe add recursion with 'device' -> 'devices' if list 
+    def get_summary(self, repo): # meh
+        config = repo.get_contents(f"devices/{self.type_identifier}.txt")
+        lines = config.decoded_content.decode().splitlines() # Eww
+        if lines[0].strip() != '[SUMMARY]': return []
+        summary = ['']
+        for ln in lines[1:]:
+            if ln.strip() == '': return summary
+            summary.append(ln.strip())
+
+
+    def get_available_repos(self, get_summary=False): # TODO: Maybe add a limit because of the github's limit for requests (without key) [if too many lists for one device] | Maybe add recursion with 'device' -> 'devices' if list 
         try:
             repo = g.GIT.get_repo(self.config) 
             config = repo.get_contents(f'device_repo_lists/{self.type_identifier}.txt')
         except UnknownObjectException as e:
             return []
         config = config.decoded_content.decode()
         repos = []
         for repo_line in config.splitlines():
             try:
                 split_repo_line = repo_line.split('|')
                 repo = g.GIT.get_repo(split_repo_line[0].strip())
                 if not self.is_repo_valid(repo): continue
-                if repo: insort_left(repos, (repo.stargazers_count, repo.full_name, split_repo_line[1] if len(split_repo_line) > 1 else split_repo_line[0]), key=lambda x: -x[0]) # ('|')[1] = Description
+                if repo: insort_left(repos, (repo.stargazers_count, repo.full_name, split_repo_line[1] if len(split_repo_line) > 1 else split_repo_line[0], self.get_summary(repo) if get_summary else []), key=lambda x: -x[0]) # ('|')[1] = Description
             except UnknownObjectException as e:
                 continue # ignore the bad repository or list them ?
         return repos
 
 
     def get_online_config_instructions(self):
         if self.config == g.SERVER_REPO: # no need for 'else' because self.config
@@ -193,15 +203,16 @@
 
     __temp_instriction_call = None
     def __perform(self, instruction): # 3-7 if statements i think they are faster than a built-in hash map in this case
         if not instruction                 : return 
         elif   instruction == '[UNINSTALL]': self.__temp_instriction_call = self.uninstall
         elif   instruction == '[INSTALL]'  : self.__temp_instriction_call = self.install
         elif   instruction == '[SHELL]'    : self.__temp_instriction_call = self.__shell 
-        else: # TODO: Add extra instruction called EXTERNAL (or something) for external shell commands if user allows so by arg
+        elif   instruction == '[SUMMARY]'  : self.__temp_instriction_call = None
+        elif self.__temp_instriction_call: # TODO: Add extra instruction called EXTERNAL (or something) for external shell commands if user allows so by arg
             tmp_split   = instruction.split('#')
             comment     = tmp_split[len(tmp_split)-1].strip()
             instruction = tmp_split[0].strip()
             self.event_debloat(instruction, comment)
             self.__temp_instriction_call(instruction)
```

### Comparing `hexapterygon-1.0.2/hexapterygon/HexaGlobals.py` & `hexapterygon-1.0.5/hexapterygon/HexaGlobals.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.2/hexapterygon/HexaTUI.py` & `hexapterygon-1.0.5/hexapterygon/HexaTUI.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,66 +12,70 @@
 
 class HexaTUI(Parent): # And a Component that can be used stand alone as it is with a uni-curses project | uni-curses compatible component
 
     def on_debloat(self, instruction, comment):
         self.comment = comment
 
 
+    def __append_instruction_text(self, text):
+        self.textbox_instructions.text = text + '\n' + self.textbox_instructions.text
+
+
     def on_install(self, package, output):
         if output == InstallState.INSTALLED:
-            self.textbox_instructions.text = f'│ ✓  [INSTALLED] {self.comment}\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ✓  [INSTALLED] {self.comment}')
         elif output == InstallState.ALREADY_INSTALLED:
-            self.textbox_instructions.text = f'│ ○  [INSTALLED] {self.comment}\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ○  [INSTALLED] {self.comment}')
         else: # BLOCKED
-            self.textbox_instructions.text = f'│ ✗  [BLOCKED] Skipping installation\n' + self.textbox_instructions.text # TIMESTAMP TOOOOO
+            self.__append_instruction_text(f'│ ✗  [BLOCKED] Skipping installation') # TIMESTAMP TOOOOO
         self.refresh()
 
 
     def on_shell(self, output): # TODO: Show output only if user passes arg  | if it contains Error then show x else tick maybe
         if not output: 
-            self.textbox_instructions.text = f'│ ○  [SHELL] {self.comment}\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ○  [SHELL] {self.comment}')
             self.refresh()
             return
-        self.textbox_instructions.text = f'│ ○  └─ [SHELL] {self.comment}\n' + self.textbox_instructions.text 
+        self.__append_instruction_text(f'│ ○  └─ [SHELL] {self.comment}')
         lines = output.split('\n')
         if len(lines) >=2:
             lines = lines[:-1]
         for ln in lines:
-            self.textbox_instructions.text = f'│ ○  ├─ {ln}\n' + self.textbox_instructions.text
-        self.textbox_instructions.text = f'│ ○  ┌───────────────────────────────────┐\n' + self.textbox_instructions.text # long pipi energy
+            self.__append_instruction_text(f'│ ○  ├─ {ln}')
+        self.__append_instruction_text(f'│ ○  ┌───────────────────────────────────┐') # long pipi energy
         self.refresh()
 
 
     def on_downloading(self,package, i, total_length): # TODO: replace the first line as an update
         percentage =  int((i)*100/total_length)
         steps = int((i)*30/total_length)
         blanks = 30-steps 
-        if i == 1 : self.textbox_instructions.text = f"│ ○  ├─ {'━'*steps}{' '*blanks} {percentage}%\n" + self.textbox_instructions.text
-        lines = self.textbox_instructions.text.split('\n')  
+        if i == 1 : self.__append_instruction_text(f"│ ○  ├─ {'━'*steps}{' '*blanks} {percentage}%")
+        lines = self.textbox_instructions.text.split('\n') 
         self.textbox_instructions.text = f"│ ○  ├─ {'━'*steps}{' '*blanks} {percentage}%\n" + '\n'.join(lines[1:])
         self.refresh()
 
 
     def on_download(self, package, output):
         if output == DownloadState.BEGINS:
-            self.textbox_instructions.text = f'│ ○  └─ [DOWNLOADING] {self.comment}\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ○  └─ [DOWNLOADING] {self.comment}')
         elif output == DownloadState.SUCCEEDED:
-            self.textbox_instructions.text = f'│ ✓  ┌─ Successfully downloaded\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ✓  ┌─ Successfully downloaded')
         elif output == DownloadState.FAILED:
-            self.textbox_instructions.text = f'│ ✗  ┌─ Failed to download\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ✗  ┌─ Failed to download')
         self.refresh()
 
 
     def on_uninstall(self, package, output):
         if output == UninstallState.UNINSTALLED:
-            self.textbox_instructions.text = f'│ ✓  [UNINSTALLED] {self.comment}\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ✓  [UNINSTALLED] {self.comment}')
         elif output == UninstallState.ALREADY_UNINSTALLED:
-            self.textbox_instructions.text = f'│ ○  [ALREADY UNINSTALLED] {self.comment}\n' + self.textbox_instructions.text 
+            self.__append_instruction_text(f'│ ○  [ALREADY UNINSTALLED] {self.comment}')
         else:
-            self.textbox_instructions.text = f'│ ✗  Failed to uninstall {package}\n' + self.textbox_instructions.text # TIMESTAMP TOOOOO
+            self.__append_instruction_text(f'│ ✗  Failed to uninstall {package}') # TIMESTAMP TOOOOO
         self.refresh()
 
 
     def __add_components(self, win, color_pair_offset): # │
         self.label_device          = Label(1,2,'⟡ Informations: ', (False,False, True,True), width = self.columns-4, win = win, color_pair_offset = color_pair_offset)
         self.label_info            = Label(self.lines-2 ,2,'● Press ESC to exit  ░▒▓██▓▒░ HEXAPTERYGON 2023 ░▒▓██▓▒░', (False,True, True,True), width = self.columns-4, win = win, color_pair_offset = color_pair_offset)
         self.textbox_instructions  = TextBox(3,2, self.lines -6, self.columns -4 , ' ', (True,True, True,True),  win = win, color_pair_offset = color_pair_offset) #│ ✓  Press ESC to exit\n│ █▓▒░ Press ESC to exit ░▒▓█
@@ -80,26 +84,27 @@
         self.label_info.color_pair = 2    
         patterns = [ # lol another piece of code for which I feel guilty for all the enviromental disaster it will create | CPU goes brrr
             Highlight(re.compile( r'[0-9]+%')                         , 5 , uc.A_BOLD  ),
             Highlight(re.compile( r'(?<=│ ✓  )\[DONE\]')              , 5 , uc.A_BOLD  ),
             Highlight(re.compile( r'(?<=│ ✗  )\[FAILED\]')            , 3 , uc.A_BOLD  ),
             Highlight(re.compile( r'[0-9]+\.')                        , 2 , uc.A_BOLD  ),
             Highlight(re.compile( r'"(.*?)"')                         , 1 , uc.A_ITALIC),
+            Highlight(re.compile( r'^│(?= ░)')                        , 2),
             Highlight(re.compile( r'^│ ✓')                            , 5),
             Highlight(re.compile( r'^│ ✗')                            , 3),
             Highlight(re.compile( r'^│ ○')                            , 2),
             Highlight(re.compile( r'^│ ★')                            , 2),
             Highlight(re.compile( r'\[[0-9]+( )+Stars\]')             , 2),
             Highlight(re.compile( r'(Failed|Error|INVALID)')          , 3),
             Highlight(re.compile( r' (━){1,5}')                       , 3),
             Highlight(re.compile( r'(?<= ━━━━━)(━){1,12}')            , 2),
             Highlight(re.compile( r'(?<= ━━━━━━━━━━━━━━━━━)(━){1,8}') , 5),
             Highlight(re.compile( r'Successfully')                    , 5),
             Highlight(re.compile( r'(┌───────────────────────────────────┐|└─|┌─|├─)'), 1, uc.A_DIM),
-            Highlight(re.compile( r'(LOADING|DOWNLOADING|ALREADY UNINSTALLED|UNINSTALLED|INSTALLED|SHELL|BLOCKED)'), 1, uc.A_DIM),
+            Highlight(re.compile( r'(LOADING|DOWNLOADING|ALREADY UNINSTALLED|UNINSTALLED|INSTALLED|SHELL|BLOCKED|UNINSTALLS|INSTALLS|DISABLES|IMPORTANT)'), 1, uc.A_DIM),
         ]
         self.textbox_instructions.set_inline_highlight_patterns(patterns)
 
 
     def __init__(self, debloater: hexapterygon, win=None, color_pair_offset=0, is_focused=False): # TODO: I might need to create a function for is_focused ?
         super().__init__(win or uc.stdscr)
         self.is_focused                  = is_focused
@@ -129,51 +134,56 @@
         self.feedback  = msg
         sys.excepthook = self.killAll
         kill(getpid(), SIGINT)
 
 
     def __print_result_for(self, device, output):
         if output:
-            self.textbox_instructions.text = '│ ✓  [DONE]\n' + self.textbox_instructions.text
+            self.__append_instruction_text('│ ✓  [DONE]')
         else:
-            self.textbox_instructions.text = f'│ ✗  [FAILED] No available debloating-list for "{device.type_identifier}" under "{device.config}"\n' + self.textbox_instructions.text
+            self.__append_instruction_text(f'│ ✗  [FAILED] No available debloating-list for "{device.type_identifier}" under "{device.config}"') 
         self.refresh()
 
 
-    def __get_len_of_int(self, num): return int(log10(num))+1 if not num == 0 else 0
+    def __get_len_of_int(self, num): return int(log10(num))+1 if not num == 0 else 1
 
 
     def __validate_feedback(self, repos): # TODO: Expand
         if not (1 <= int(self.feedback) <= len(repos)):
-            self.textbox_instructions.text = f'│ ✗  [INVALID] Out of range INPUT {self.feedback}\n' + self.textbox_instructions.text
+            self.__append_instruction_text(f'│ ✗  [INVALID] Out of range INPUT {self.feedback}')
             self.feedback = ''
             self.refresh()
             return True
         return False
 
 
     feedback = ''
     def __choose_available_repo_if_needed_for(self, device): # WHY SUCH A LONG NAME FOR AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
         if device.locally or device.config != g.SERVER_REPO: return None # aahh whatever double checking for g.SERVER_REPO for no reason because I HAVE NO TIME TO EVEN THINK CLEARLY! F@CKING MONEY
         self.feedback = '' # this line was above, just in case, a reminder lol
-        self.textbox_instructions.text = f'│ ○  Gathering available repositories\n' + self.textbox_instructions.text
+        self.__append_instruction_text(f'│ ○  Gathering available repositories')
         self.refresh()
-        repos = device.get_available_repos()
+        repos = device.get_available_repos(get_summary=True)
         if not repos: return None # None because it is being handled by DeviceOverlay later and we don't want to interapt the debloating proccess of the next devices in case there is a config for them | self.__exit_with_reason(f'No available debloating-list for "{device.type_identifier}"')
         digit_len_of_most_started_repo = self.__get_len_of_int(repos[0][0])
         i = len(repos)
         for repo in reversed(repos):
             stars = repo[0]
             digit_len_of_repo = self.__get_len_of_int(stars)
-            self.textbox_instructions.text = f'│ ★  {i}. ' + f'[{stars} ' + ' '* (digit_len_of_most_started_repo - digit_len_of_repo) + f'Stars] "{repo[2].strip()}"\n' + self.textbox_instructions.text 
+            description_summarry = f'│ ★  {i}. ' + f'[{stars} ' + ' '* (digit_len_of_most_started_repo - digit_len_of_repo) + f'Stars] "{repo[2].strip()}"'
+            if repo[3]:
+                description_summarry += '\n│ ░  ┌─'
+                description_summarry += '\n│ ░  ├─ '.join(repo[3])
+                description_summarry += '\n│ ░  └─\n'
+            self.__append_instruction_text(description_summarry)
             i -=1
         self.label_device.text = f'⟡ Select a debloating-list for {device.type_identifier}:'; self.refresh()
         while not self.feedback or self.__validate_feedback(repos) : sleep(1) # I thought about it before looking into there https://superfastpython.com/thread-wait-for-result/ | feedback - no need for validation if int as of now
         repo = repos[int(self.feedback)-1]
-        self.textbox_instructions.text = f'│ ○  [LOADING] "{repo[2].strip()}"\n' + self.textbox_instructions.text; self.refresh()
+        self.__append_instruction_text(f'│ ○  [LOADING] "{repo[2].strip()}"\n'); self.refresh()
         device.config = repo[1]
 
 
     def __reset_device_label_style(self):
         self.label_device.style      = uc.A_BOLD | uc.A_ITALIC
         self.label_device.color_pair = 2
 
@@ -199,15 +209,15 @@
     def __async_begin(self):
         self.textbox_instructions.text = '│ ○  Checking for available devices'
         self.__check_for_unauthorized_devices()
         devices = self.debloater.get_devices()
         if not devices: self.__exit_with_reason('No connected devices found')
         for device in devices:
             self.__reset_device_label_style()
-            self.__choose_available_repo_if_needed_for(device) 
+            self.__choose_available_repo_if_needed_for(device)
             self.label_device.text = f'⟡ Debloating, {device.type_identifier}:'; self.refresh()
             self.__print_result_for(device, next(self.debloater.debloat(device)))
 
 
     def begin(self):
         threading.excepthook = self.__exit_with_reason # ahh whatever
         t = threading.Thread(target=self.__async_begin)
@@ -230,15 +240,15 @@
             self.label_info.style = uc.A_DIM
             self.label_info.text  = '● Press ESC to exit  ░▒▓██▓▒░ HEXAPTERYGON 2023 ░▒▓██▓▒░'
 
 
     def handle_feedback_over_thread(self, event):
         self.escape_event_consumed = False
         if  47 < event < 58: 
-            self.__feedback      += uc.RCCHAR(event) 
+            self.__feedback      += uc.RCCHAR(event)
             self.label_info.style = uc.A_BOLD
             self.label_info.text  = f'INPUT: {self.__feedback}'
         elif self.__feedback and event == 27: 
             self.escape_event_consumed = True
             self.__reset_feedback()
         elif event == uc.KEY_BACKSPACE:
             if self.__feedback:
@@ -255,12 +265,12 @@
         if event == uc.KEY_RESIZE: self.handle_resize(redraw_parent)
         if not self.is_focused: return
         self.textbox_instructions.handle_events(event)
         self.handle_feedback_over_thread(event)
 
 
     def refresh(self):
-        uc.wrefresh(self.win) 
+        uc.wrefresh(self.win)
         self.label_info          .refresh()
         self.label_device        .refresh()
         self.textbox_instructions.refresh()
```

### Comparing `hexapterygon-1.0.2/hexapterygon/InsortForOldPython.py` & `hexapterygon-1.0.5/hexapterygon/InsortForOldPython.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.2/hexapterygon/TUItilities.py` & `hexapterygon-1.0.5/hexapterygon/TUItilities.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.2/hexapterygon/__init__.py` & `hexapterygon-1.0.5/hexapterygon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .DeviceOverlay import DeviceOverlay
 from github         import Github
 import hexapterygon.HexaGlobals as g
 from shutil import rmtree
 
 
 
-__version__ = '1.0.2'
+__version__ = '1.0.5'
 def get_global_server_repo(): return g.SERVER_REPO
 def set_global_server_repo(value): g.SERVER_REPO = value
 def set_github_token      (value): g.GIT         = Github(login_or_token=value)
 
 
 
 class Hexapterygon(DeviceEvents): # TODO: restore via cmd package install-existing <package>
```

### Comparing `hexapterygon-1.0.2/hexapterygon/__main__.py` & `hexapterygon-1.0.5/hexapterygon/__main__.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.2/setup.py` & `hexapterygon-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #def readfile(filename):
 #    with open(filename, 'r+') as f:
 #        return f.read()
 
 
 setup(
     name="hexapterygon",
-    version="1.0.2",
+    version="1.0.5",
     description="A user-friendly all-in-one cross-platform, (uni-curses compatible component, module and uitility) software for orchestrating and debloating your Android devices from unwanted pre-installed crap.",
     #long_description=readfile('README.md'),
     author="George Chousos",
     author_email="gxousos@gmail.com",
     url="https://github.com/GiorgosXou/hexapterygon",
     packages=['hexapterygon'],
     install_requires=['uni-curses', 'pure-python-adb', 'PyGithub'],
```

