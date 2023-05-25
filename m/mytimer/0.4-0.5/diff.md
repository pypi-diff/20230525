# Comparing `tmp/mytimer-0.4.tar.gz` & `tmp/mytimer-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytimer-0.4.tar", last modified: Fri Feb 10 16:36:11 2023, max compression
+gzip compressed data, was "mytimer-0.5.tar", last modified: Thu May 25 15:11:52 2023, max compression
```

## Comparing `mytimer-0.4.tar` & `mytimer-0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:36:11.692937 mytimer-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-10 16:36:00.000000 mytimer-0.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-10 16:36:00.000000 mytimer-0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-02-10 16:36:00.000000 mytimer-0.4/FACES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-10 16:36:00.000000 mytimer-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-10 16:36:00.000000 mytimer-0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-02-10 16:36:11.692937 mytimer-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-02-10 16:36:00.000000 mytimer-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-10 16:36:00.000000 mytimer-0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:36:11.692937 mytimer-0.4/mytimer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-10 16:36:00.000000 mytimer-0.4/mytimer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-02-10 16:36:00.000000 mytimer-0.4/mytimer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-10 16:36:00.000000 mytimer-0.4/mytimer/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-10 16:36:00.000000 mytimer-0.4/mytimer/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:36:11.692937 mytimer-0.4/mytimer/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)   602412 2023-02-10 16:36:00.000000 mytimer-0.4/mytimer/sounds/alarm.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:36:11.692937 mytimer-0.4/mytimer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-02-10 16:36:11.000000 mytimer-0.4/mytimer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-10 16:36:11.000000 mytimer-0.4/mytimer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 16:36:11.000000 mytimer-0.4/mytimer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-10 16:36:11.000000 mytimer-0.4/mytimer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-10 16:36:11.000000 mytimer-0.4/mytimer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-10 16:36:11.000000 mytimer-0.4/mytimer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-10 16:36:00.000000 mytimer-0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-10 16:36:11.692937 mytimer-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-10 16:36:00.000000 mytimer-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.089664 mytimer-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 15:11:39.000000 mytimer-0.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-25 15:11:39.000000 mytimer-0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-25 15:11:39.000000 mytimer-0.5/FACES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:11:39.000000 mytimer-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 15:11:39.000000 mytimer-0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-25 15:11:52.089664 mytimer-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-25 15:11:39.000000 mytimer-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 15:11:39.000000 mytimer-0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.085664 mytimer-0.5/mytimer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.085664 mytimer-0.5/mytimer/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)   602412 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/sounds/alarm.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.085664 mytimer-0.5/mytimer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 15:11:52.000000 mytimer-0.5/mytimer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 15:11:39.000000 mytimer-0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:11:52.089664 mytimer-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-25 15:11:39.000000 mytimer-0.5/setup.py
```

### Comparing `mytimer-0.4/CHANGELOG.md` & `mytimer-0.5/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.5] - 2023-05-25
+### Added
+- 5 new faces
+- `--message` argument
+### Changed
+- `play_sound` function modified
+- `playsound` removed from `requirements.txt`
+- `README.md` updated
 ## [0.4] - 2023-02-10
 ### Added
 - 4 new faces
 - Infinite timer mode
 ### Changed
 - `README.md` updated
 - Parameters moved to `params.py`
@@ -28,15 +36,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...dev
+[0.5]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

### Comparing `mytimer-0.4/FACES.md` & `mytimer-0.5/FACES.md`

 * *Files 19% similar despite different names*

```diff
@@ -156,7 +156,54 @@
 
 ## 16
 
 ```
 '|~)o~//| o|~ / 
  |/_o_)~|~o_)(_)
 ```
+
+## 17
+
+```                              
+ #  ###     ### # #     ### ### 
+##    #  #    # # #  #  #   #   
+ #  ###      ## ###     ### ### 
+ #  #    #    #   #  #    # # # 
+### ###     ###   #     ### ### 
+
+```
+
+## 18
+
+```
+'| '~).'~)|_|.L~ / 
+.|. /_.._)  |._)(_)
+```
+
+## 19
+
+```
+ ___,  __,   __,  __,  ____,  __,  ____,   ___, 
+(-/|  (- )  (-o  (-_) (-/_|_,(-o  (-|_    (-/_  
+ '_|,  ,'_,  _o   __)    _|,  _o    __)   _(__) 
+ (    (     (    (      (    (     (     (      
+
+```
+
+## 20
+
+```
+ __  ___  _  ___   __   _  ___   _  
+(  )(__ \(_)(__ ) / ,) (_)/ __) / ) 
+ )( / __/ _  (_ \(_  _) _ \__ \/ , \
+(__)\___)(_)(___/  (_) (_)(___/\___/
+
+```
+
+## 21
+
+```
+::|  ::~~:\    /:'`:,:| :|     :::::|,::::\
+ :|    ,:/ ::)   |:< :::::|::) `:::\ ::---,
+:::| /::::|::) \:,,:'   :| ::) ,:::/ `::::'
+
+```
```

### Comparing `mytimer-0.4/LICENSE` & `mytimer-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mytimer-0.4/PKG-INFO` & `mytimer-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mytimer
-Version: 0.4
+Version: 0.5
 Summary: Simple Timer for Your Terminal
 Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.4
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.5
 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir
 License: MIT
 Project-URL: Source, https://github.com/sepandhaghighi/mytimer
 Keywords: python3 python timer terminal stopwatch
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -111,22 +111,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 0.4](https://github.com/sepandhaghighi/mytimer/archive/v0.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
-- `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
-- `python3 setup.py install` or `python setup.py install` (Need root access)				
+- Download [Version 0.5](https://github.com/sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==0.4` or `pip3 install mytimer==0.4` (Need root access)							
+- `pip install mytimer==0.5` (Need root access)							
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -176,14 +175,22 @@
 ### Face
 
 
 ```console
 mytimer --minute=7 --second=30 --face=3
 ```
 * [Faces List](https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
+
+
+### Message
+
+
+```console
+mytimer --minute=7 --second=30 --message="Test message"
+```
 		
 
 <div align="center">
 
 <img src="https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif">
 <p>Screen Record</p>
 
@@ -240,14 +247,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.5] - 2023-05-25
+### Added
+- 5 new faces
+- `--message` argument
+### Changed
+- `play_sound` function modified
+- `playsound` removed from `requirements.txt`
+- `README.md` updated
 ## [0.4] - 2023-02-10
 ### Added
 - 4 new faces
 - Infinite timer mode
 ### Changed
 - `README.md` updated
 - Parameters moved to `params.py`
@@ -267,15 +282,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...dev
+[0.5]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: mytimer Version: 0.4 Summary: Simple Timer for Your
+Metadata-Version: 2.1 Name: mytimer Version: 0.5 Summary: Simple Timer for Your
 Terminal Home-page: https://github.com/sepandhaghighi/mytimer Download-URL:
-https://github.com/sepandhaghighi/mytimer/tarball/v0.4 Author: Sepand Haghighi
+https://github.com/sepandhaghighi/mytimer/tarball/v0.5 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir License: MIT Project-URL: Source, https://
 github.com/sepandhaghighi/mytimer Keywords: python3 python timer terminal
 stopwatch Classifier: Development Status :: 4 - Beta Classifier: Natural
 Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -48,31 +48,30 @@
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI         mytimer/workflows/CI/               mytimer/workflows/CI/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           [https://app.codacy.com/project/
 Code Quality [CodeFactor]           badge/Grade/            [codebeat_badge]
                           1bf28500431a498998ac79891cd79cda]
-## Installation ### Source Code - Download [Version 0.4](https://github.com/
-sepandhaghighi/mytimer/archive/v0.4.zip) or [Latest Source ](https://
-github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install -
-r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
-`python3 setup.py install` or `python setup.py install` (Need root access) ###
-PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - `pip install mytimer==0.4` or `pip3 install mytimer==0.4` (Need
-root access) ## Usage â ï¸ You can use `mytimer` or `python -m mytimer` to
-run this program ### Version ```console mytimer --version ``` ### Basic â ï¸
-Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit ```console
-mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --minute=20 ```
-### Timer Mode â ï¸ The default mode is `count-up` ```console mytimer --
-minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --second=30
---countup ``` ### Alarm â ï¸ This mode may not be supported on all systems
-```console mytimer --minute=7 --second=30 --countdown --alarm ``` ### Face
-```console mytimer --minute=7 --second=30 --face=3 ``` * [Faces List](https://
-github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
+## Installation ### Source Code - Download [Version 0.5](https://github.com/
+sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://
+github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI -
+Check [Python Packaging User Guide](https://packaging.python.org/installing/) -
+`pip install mytimer==0.5` (Need root access) ## Usage â ï¸ You can use
+`mytimer` or `python -m mytimer` to run this program ### Version ```console
+mytimer --version ``` ### Basic â ï¸ Press `Ctrl + C` to exit ```console
+mytimer ``` ### Time Limit ```console mytimer --minute=7 --second=30 ```
+```console mytimer --hour=2 --minute=20 ``` ### Timer Mode â ï¸ The default
+mode is `count-up` ```console mytimer --minute=7 --second=30 --countdown ```
+```console mytimer --minute=7 --second=30 --countup ``` ### Alarm â ï¸ This
+mode may not be supported on all systems ```console mytimer --minute=7 --
+second=30 --countdown --alarm ``` ### Face ```console mytimer --minute=7 --
+second=30 --face=3 ``` * [Faces List](https://github.com/sepandhaghighi/
+mytimer/blob/main/FACES.md) ### Message ```console mytimer --minute=7 --
+second=30 --message="Test message" ```
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif]
                                  Screen Record
 ## Issues & Bug Reports Just fill an issue and describe it. We'll check it
 ASAP! - Please complete the issue template ## References
      1- Mixkit_Free_Alarm_Sound_Effects
 ## Show your support
 **** Star this repo ****
@@ -101,19 +100,23 @@
 *** Zilliqa ***
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 *** Coffeete ***
 [http://www.coffeete.ir/images/buttons/lemonchiffon.png] # Changelog All
 notable changes to this project will be documented in this file. The format is
 based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
 project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
-## [Unreleased] ## [0.4] - 2023-02-10 ### Added - 4 new faces - Infinite timer
-mode ### Changed - `README.md` updated - Parameters moved to `params.py` ##
-[0.3] - 2022-11-25 ### Added - `--face` argument - `FACES.md` ### Changed -
-`README.md` updated - Minimum `art` library version changed from `1.8` to `2.9`
-## [0.2] - 2022-11-03 ### Added - `--version` flag ### Changed - Test system
-modified - `countdown_timer` function modified - `countup_timer` function
-modified ## [0.1] - 2022-10-18 ### Added - Countdown mode - Count-up mode -
-Alarm [Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/
-v0.4...dev [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
-[0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3 [0.2]:
-https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2 [0.1]: https://
-github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
+## [Unreleased] ## [0.5] - 2023-05-25 ### Added - 5 new faces - `--message`
+argument ### Changed - `play_sound` function modified - `playsound` removed
+from `requirements.txt` - `README.md` updated ## [0.4] - 2023-02-10 ### Added -
+4 new faces - Infinite timer mode ### Changed - `README.md` updated -
+Parameters moved to `params.py` ## [0.3] - 2022-11-25 ### Added - `--face`
+argument - `FACES.md` ### Changed - `README.md` updated - Minimum `art` library
+version changed from `1.8` to `2.9` ## [0.2] - 2022-11-03 ### Added - `--
+version` flag ### Changed - Test system modified - `countdown_timer` function
+modified - `countup_timer` function modified ## [0.1] - 2022-10-18 ### Added -
+Countdown mode - Count-up mode - Alarm [Unreleased]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.5...dev [0.5]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.4...v0.5 [0.4]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.3...v0.4 [0.3]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.2...v0.3 [0.2]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.1...v0.2 [0.1]: https://github.com/
+sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

### Comparing `mytimer-0.4/README.md` & `mytimer-0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -77,22 +77,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 0.4](https://github.com/sepandhaghighi/mytimer/archive/v0.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
-- `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
-- `python3 setup.py install` or `python setup.py install` (Need root access)				
+- Download [Version 0.5](https://github.com/sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==0.4` or `pip3 install mytimer==0.4` (Need root access)							
+- `pip install mytimer==0.5` (Need root access)							
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -142,14 +141,22 @@
 ### Face
 
 
 ```console
 mytimer --minute=7 --second=30 --face=3
 ```
 * [Faces List](https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
+
+
+### Message
+
+
+```console
+mytimer --minute=7 --second=30 --message="Test message"
+```
 		
 
 <div align="center">
 
 <img src="https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif">
 <p>Screen Record</p>
```

#### html2text {}

```diff
@@ -30,31 +30,30 @@
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI         mytimer/workflows/CI/               mytimer/workflows/CI/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           [https://app.codacy.com/project/
 Code Quality [CodeFactor]           badge/Grade/            [codebeat_badge]
                           1bf28500431a498998ac79891cd79cda]
-## Installation ### Source Code - Download [Version 0.4](https://github.com/
-sepandhaghighi/mytimer/archive/v0.4.zip) or [Latest Source ](https://
-github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install -
-r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
-`python3 setup.py install` or `python setup.py install` (Need root access) ###
-PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - `pip install mytimer==0.4` or `pip3 install mytimer==0.4` (Need
-root access) ## Usage â ï¸ You can use `mytimer` or `python -m mytimer` to
-run this program ### Version ```console mytimer --version ``` ### Basic â ï¸
-Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit ```console
-mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --minute=20 ```
-### Timer Mode â ï¸ The default mode is `count-up` ```console mytimer --
-minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --second=30
---countup ``` ### Alarm â ï¸ This mode may not be supported on all systems
-```console mytimer --minute=7 --second=30 --countdown --alarm ``` ### Face
-```console mytimer --minute=7 --second=30 --face=3 ``` * [Faces List](https://
-github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
+## Installation ### Source Code - Download [Version 0.5](https://github.com/
+sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://
+github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI -
+Check [Python Packaging User Guide](https://packaging.python.org/installing/) -
+`pip install mytimer==0.5` (Need root access) ## Usage â ï¸ You can use
+`mytimer` or `python -m mytimer` to run this program ### Version ```console
+mytimer --version ``` ### Basic â ï¸ Press `Ctrl + C` to exit ```console
+mytimer ``` ### Time Limit ```console mytimer --minute=7 --second=30 ```
+```console mytimer --hour=2 --minute=20 ``` ### Timer Mode â ï¸ The default
+mode is `count-up` ```console mytimer --minute=7 --second=30 --countdown ```
+```console mytimer --minute=7 --second=30 --countup ``` ### Alarm â ï¸ This
+mode may not be supported on all systems ```console mytimer --minute=7 --
+second=30 --countdown --alarm ``` ### Face ```console mytimer --minute=7 --
+second=30 --face=3 ``` * [Faces List](https://github.com/sepandhaghighi/
+mytimer/blob/main/FACES.md) ### Message ```console mytimer --minute=7 --
+second=30 --message="Test message" ```
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif]
                                  Screen Record
 ## Issues & Bug Reports Just fill an issue and describe it. We'll check it
 ASAP! - Please complete the issue template ## References
      1- Mixkit_Free_Alarm_Sound_Effects
 ## Show your support
 **** Star this repo ****
```

### Comparing `mytimer-0.4/mytimer/__main__.py` & `mytimer-0.5/mytimer/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 
 def main():
     """
     CLI main function.
 
     :return: None
     """
-    params = {"minute": 0, "hour": 0, "second": 0, "alarm": 0, "face": 1}
+    params = {
+        "minute": 0,
+        "hour": 0,
+        "second": 0,
+        "alarm": 0,
+        "face": 1,
+        "message": ""}
     parser = argparse.ArgumentParser()
     parser.add_argument('--minute', help='minute', type=float)
     parser.add_argument('--second', help='second', type=float)
     parser.add_argument('--hour', help='hour', type=float)
+    parser.add_argument('--message', help='message', type=str)
     parser.add_argument(
         '--face',
         help='face',
         type=int,
         choices=list(
             FACES_MAP.keys()))
     parser.add_argument(
```

### Comparing `mytimer-0.4/mytimer/functions.py` & `mytimer-0.5/mytimer/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """mytimer functions."""
 import os
 import sys
+import subprocess
 import time
 from mytimer.params import *
 from art import tprint
 
 
 def check_null_time(args):
     """
@@ -25,40 +26,45 @@
     """
     Input check decorator for timer functions.
 
     :param func: input function
     :type func: function
     :return: inner function
     """
-    def inner_function(hour, minute, second, alarm, face):
+    def inner_function(hour, minute, second, alarm, face, message):
         """
         Inner function.
 
         :param hour: hour
         :type hour: int
         :param minute: minute
         :type minute: int
         :param second: second
         :type second: int
         :param alarm: alarm flag
         :type alarm: bool
         :param face: face number
         :type face: int
+        :param message: message
+        :type message: str
         :return: None
         """
+        message = message.strip()
+        if len(message) > 0:
+            message = MESSAGE_TEMPLATE.format(message)
         font = FACES_MAP[face]
         items_list = [hour, minute, second]
         if sum(items_list) != 0 and all(map(lambda x: x >= 0, items_list)):
             if second >= 60:
                 minute += second // 60
                 second %= 60
             if minute >= 60:
                 hour += minute // 60
                 minute %= 60
-            func(hour, minute, second, alarm, font)
+            func(hour, minute, second, alarm, font, message)
         else:
             print(WRONG_INPUT_ERROR)
             print(INPUT_EXAMPLE)
     return inner_function
 
 
 def clear_screen():
@@ -83,44 +89,60 @@
     """
     cd, _ = os.path.split(__file__)
     return os.path.join(cd, "sounds", sound_name)
 
 
 def play_sound(sound_path):
     """
-    Play sound asynchronous in a thread.
+    Play sound.
 
     :param sound_path: sound path
     :type sound_path: str
-    :param debug: debug mode flag
-    :type debug: bool
     :return: None
     """
     try:
-        import playsound
-        playsound.playsound(sound_path)
+        sys_platform = sys.platform
+        if sys_platform == "win32":
+            import winsound
+            winsound.PlaySound(sound_path, winsound.SND_FILENAME)
+        elif sys_platform == "darwin":
+            _ = subprocess.check_call(["afplay",
+                                       sound_path],
+                                      shell=False,
+                                      stderr=subprocess.PIPE,
+                                      stdin=subprocess.PIPE,
+                                      stdout=subprocess.PIPE)
+        else:
+            _ = subprocess.check_call(["aplay",
+                                       sound_path],
+                                      shell=False,
+                                      stderr=subprocess.PIPE,
+                                      stdin=subprocess.PIPE,
+                                      stdout=subprocess.PIPE)
     except Exception:
         print(SOUND_ERROR_MESSAGE)
 
 
 @input_check
-def countup_timer(hour, minute, second, alarm, font=FACES_MAP[1]):
+def countup_timer(hour, minute, second, alarm, font=FACES_MAP[1], message=""):
     """
     Count-up timer function.
 
     :param hour: hour
     :type hour: int
     :param minute: minute
     :type minute: int
     :param second: second
     :type second: int
     :param alarm: alarm flag
     :type alarm: bool
     :param font: font name
     :type font: str
+    :param message: message
+    :type message: str
     :return: None
     """
     timer_second = 0
     timer_minute = 0
     timer_hour = 0
     while True:
         start = time.perf_counter()
@@ -128,16 +150,17 @@
         print('\n' * 5)
         tprint(
             '\t\t\t\t  %d : %d : %d ' %
             (timer_hour,
              timer_minute,
              timer_second),
             font=font)
+        print(message)
         if timer_hour == hour and timer_minute == minute and timer_second == second:
-            tprint("End!")
+            print("End!")
             if alarm:
                 play_sound(get_sound_path("alarm.wav"))
             break
         timer_second += 1
         if timer_second == 60:
             timer_second = 0
             timer_minute += 1
@@ -145,43 +168,52 @@
             timer_minute = 0
             timer_hour += 1
         end = time.perf_counter()
         time.sleep(max(0, 1 - (end - start)))
 
 
 @input_check
-def countdown_timer(hour, minute, second, alarm, font=FACES_MAP[1]):
+def countdown_timer(
+        hour,
+        minute,
+        second,
+        alarm,
+        font=FACES_MAP[1],
+        message=""):
     """
     Countdown timer function.
 
     :param hour: hour
     :type hour: int
     :param minute: minute
     :type minute: int
     :param second: second
     :type second: int
     :param alarm: alarm flag
     :type alarm: bool
     :param font: font name
     :type font: str
+    :param message: message
+    :type message: str
     :return: None
     """
     while True:
         start = time.perf_counter()
         clear_screen()
         print('\n' * 5)
         tprint('\t\t\t\t  %d : %d : %d ' %
                (hour, minute, second), font=font)
+        print(message)
         second -= 1
         if second == -1:
             second = 59
             minute -= 1
         if minute == -1:
             minute = 59
             hour -= 1
         if hour == -1:
-            tprint("End!")
+            print("End!")
             if alarm:
                 play_sound(get_sound_path("alarm.wav"))
             break
         end = time.perf_counter()
         time.sleep(max(0, 1 - (end - start)))
```

### Comparing `mytimer-0.4/mytimer/sounds/alarm.wav` & `mytimer-0.5/mytimer/sounds/alarm.wav`

 * *Files identical despite different names*

### Comparing `mytimer-0.4/mytimer.egg-info/PKG-INFO` & `mytimer-0.5/mytimer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mytimer
-Version: 0.4
+Version: 0.5
 Summary: Simple Timer for Your Terminal
 Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.4
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.5
 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir
 License: MIT
 Project-URL: Source, https://github.com/sepandhaghighi/mytimer
 Keywords: python3 python timer terminal stopwatch
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -111,22 +111,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 0.4](https://github.com/sepandhaghighi/mytimer/archive/v0.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
-- `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
-- `python3 setup.py install` or `python setup.py install` (Need root access)				
+- Download [Version 0.5](https://github.com/sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==0.4` or `pip3 install mytimer==0.4` (Need root access)							
+- `pip install mytimer==0.5` (Need root access)							
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -176,14 +175,22 @@
 ### Face
 
 
 ```console
 mytimer --minute=7 --second=30 --face=3
 ```
 * [Faces List](https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
+
+
+### Message
+
+
+```console
+mytimer --minute=7 --second=30 --message="Test message"
+```
 		
 
 <div align="center">
 
 <img src="https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif">
 <p>Screen Record</p>
 
@@ -240,14 +247,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.5] - 2023-05-25
+### Added
+- 5 new faces
+- `--message` argument
+### Changed
+- `play_sound` function modified
+- `playsound` removed from `requirements.txt`
+- `README.md` updated
 ## [0.4] - 2023-02-10
 ### Added
 - 4 new faces
 - Infinite timer mode
 ### Changed
 - `README.md` updated
 - Parameters moved to `params.py`
@@ -267,15 +282,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...dev
+[0.5]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: mytimer Version: 0.4 Summary: Simple Timer for Your
+Metadata-Version: 2.1 Name: mytimer Version: 0.5 Summary: Simple Timer for Your
 Terminal Home-page: https://github.com/sepandhaghighi/mytimer Download-URL:
-https://github.com/sepandhaghighi/mytimer/tarball/v0.4 Author: Sepand Haghighi
+https://github.com/sepandhaghighi/mytimer/tarball/v0.5 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir License: MIT Project-URL: Source, https://
 github.com/sepandhaghighi/mytimer Keywords: python3 python timer terminal
 stopwatch Classifier: Development Status :: 4 - Beta Classifier: Natural
 Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -48,31 +48,30 @@
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI         mytimer/workflows/CI/               mytimer/workflows/CI/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           [https://app.codacy.com/project/
 Code Quality [CodeFactor]           badge/Grade/            [codebeat_badge]
                           1bf28500431a498998ac79891cd79cda]
-## Installation ### Source Code - Download [Version 0.4](https://github.com/
-sepandhaghighi/mytimer/archive/v0.4.zip) or [Latest Source ](https://
-github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install -
-r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
-`python3 setup.py install` or `python setup.py install` (Need root access) ###
-PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - `pip install mytimer==0.4` or `pip3 install mytimer==0.4` (Need
-root access) ## Usage â ï¸ You can use `mytimer` or `python -m mytimer` to
-run this program ### Version ```console mytimer --version ``` ### Basic â ï¸
-Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit ```console
-mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --minute=20 ```
-### Timer Mode â ï¸ The default mode is `count-up` ```console mytimer --
-minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --second=30
---countup ``` ### Alarm â ï¸ This mode may not be supported on all systems
-```console mytimer --minute=7 --second=30 --countdown --alarm ``` ### Face
-```console mytimer --minute=7 --second=30 --face=3 ``` * [Faces List](https://
-github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
+## Installation ### Source Code - Download [Version 0.5](https://github.com/
+sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://
+github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI -
+Check [Python Packaging User Guide](https://packaging.python.org/installing/) -
+`pip install mytimer==0.5` (Need root access) ## Usage â ï¸ You can use
+`mytimer` or `python -m mytimer` to run this program ### Version ```console
+mytimer --version ``` ### Basic â ï¸ Press `Ctrl + C` to exit ```console
+mytimer ``` ### Time Limit ```console mytimer --minute=7 --second=30 ```
+```console mytimer --hour=2 --minute=20 ``` ### Timer Mode â ï¸ The default
+mode is `count-up` ```console mytimer --minute=7 --second=30 --countdown ```
+```console mytimer --minute=7 --second=30 --countup ``` ### Alarm â ï¸ This
+mode may not be supported on all systems ```console mytimer --minute=7 --
+second=30 --countdown --alarm ``` ### Face ```console mytimer --minute=7 --
+second=30 --face=3 ``` * [Faces List](https://github.com/sepandhaghighi/
+mytimer/blob/main/FACES.md) ### Message ```console mytimer --minute=7 --
+second=30 --message="Test message" ```
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif]
                                  Screen Record
 ## Issues & Bug Reports Just fill an issue and describe it. We'll check it
 ASAP! - Please complete the issue template ## References
      1- Mixkit_Free_Alarm_Sound_Effects
 ## Show your support
 **** Star this repo ****
@@ -101,19 +100,23 @@
 *** Zilliqa ***
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 *** Coffeete ***
 [http://www.coffeete.ir/images/buttons/lemonchiffon.png] # Changelog All
 notable changes to this project will be documented in this file. The format is
 based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
 project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
-## [Unreleased] ## [0.4] - 2023-02-10 ### Added - 4 new faces - Infinite timer
-mode ### Changed - `README.md` updated - Parameters moved to `params.py` ##
-[0.3] - 2022-11-25 ### Added - `--face` argument - `FACES.md` ### Changed -
-`README.md` updated - Minimum `art` library version changed from `1.8` to `2.9`
-## [0.2] - 2022-11-03 ### Added - `--version` flag ### Changed - Test system
-modified - `countdown_timer` function modified - `countup_timer` function
-modified ## [0.1] - 2022-10-18 ### Added - Countdown mode - Count-up mode -
-Alarm [Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/
-v0.4...dev [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
-[0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3 [0.2]:
-https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2 [0.1]: https://
-github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
+## [Unreleased] ## [0.5] - 2023-05-25 ### Added - 5 new faces - `--message`
+argument ### Changed - `play_sound` function modified - `playsound` removed
+from `requirements.txt` - `README.md` updated ## [0.4] - 2023-02-10 ### Added -
+4 new faces - Infinite timer mode ### Changed - `README.md` updated -
+Parameters moved to `params.py` ## [0.3] - 2022-11-25 ### Added - `--face`
+argument - `FACES.md` ### Changed - `README.md` updated - Minimum `art` library
+version changed from `1.8` to `2.9` ## [0.2] - 2022-11-03 ### Added - `--
+version` flag ### Changed - Test system modified - `countdown_timer` function
+modified - `countup_timer` function modified ## [0.1] - 2022-10-18 ### Added -
+Countdown mode - Count-up mode - Alarm [Unreleased]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.5...dev [0.5]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.4...v0.5 [0.4]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.3...v0.4 [0.3]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.2...v0.3 [0.2]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.1...v0.2 [0.1]: https://github.com/
+sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

### Comparing `mytimer-0.4/setup.py` & `mytimer-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     except Exception:
         return '''Simple Timer for Your Terminal'''
 
 
 setup(
     name='mytimer',
     packages=['mytimer'],
-    version='0.4',
+    version='0.5',
     description='Simple Timer for Your Terminal',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='Sepand Haghighi',
     author_email='sepand@pyrgg.ir',
     url='https://github.com/sepandhaghighi/mytimer',
-    download_url='https://github.com/sepandhaghighi/mytimer/tarball/v0.4',
+    download_url='https://github.com/sepandhaghighi/mytimer/tarball/v0.5',
     keywords="python3 python timer terminal stopwatch",
     project_urls={
         'Source': 'https://github.com/sepandhaghighi/mytimer'
     },
     install_requires=get_requires(),
     python_requires='>=3.5',
     classifiers=[
```

