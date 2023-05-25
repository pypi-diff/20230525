# Comparing `tmp/pyscada-gpio-0.7.0rc8.tar.gz` & `tmp/pyscada-gpio-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyscada-gpio-0.7.0rc8.tar", last modified: Mon Dec  3 13:09:17 2018, max compression
+gzip compressed data, was "pyscada-gpio-0.8.0.tar", last modified: Thu May 25 12:22:03 2023, max compression
```

## Comparing `pyscada-gpio-0.7.0rc8.tar` & `pyscada-gpio-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/
--rw-rw-r--   0 martin    (1000) martin    (1000)    35147 2018-07-08 23:18:13.000000 pyscada-gpio-0.7.0rc8/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      106 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     1397 2018-07-08 23:18:13.000000 pyscada-gpio-0.7.0rc8/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/
--rw-rw-r--   0 martin    (1000) martin    (1000)      662 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/__init__.pyc
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/migrations/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1508 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/migrations/0002_add_device_protocol.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2871 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/migrations/0001_initial.py
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/migrations/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3344 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/worker.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      320 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/apps.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      487 2018-12-03 12:56:46.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2516 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/admin.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2329 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/device.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2263 2018-07-08 23:18:14.000000 pyscada-gpio-0.7.0rc8/pyscada/gpio/models.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)       56 2018-07-09 12:10:37.000000 pyscada-gpio-0.7.0rc8/pyscada/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1817 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      190 2018-07-08 23:18:13.000000 pyscada-gpio-0.7.0rc8/CHANGELOG.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      581 2018-07-08 23:18:13.000000 pyscada-gpio-0.7.0rc8/README.rst
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)       17 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2018-07-08 23:18:13.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/not-zip-safe
--rw-rw-r--   0 martin    (1000) martin    (1000)        8 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1817 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      631 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        8 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/namespace_packages.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2018-12-03 13:09:17.000000 pyscada-gpio-0.7.0rc8/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      153 2018-07-08 23:18:13.000000 pyscada-gpio-0.7.0rc8/AUTHORS
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 12:22:03.615375 pyscada-gpio-0.8.0/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      197 2023-04-05 08:57:41.000000 pyscada-gpio-0.8.0/AUTHORS
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      190 2019-11-20 08:26:35.000000 pyscada-gpio-0.8.0/CHANGELOG.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)    34523 2023-03-27 14:51:28.000000 pyscada-gpio-0.8.0/LICENSE
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      132 2023-04-05 08:57:41.000000 pyscada-gpio-0.8.0/MANIFEST.in
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1839 2023-05-25 12:22:03.611375 pyscada-gpio-0.8.0/PKG-INFO
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      581 2019-11-20 08:26:35.000000 pyscada-gpio-0.8.0/README.rst
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 12:22:03.611375 pyscada-gpio-0.8.0/pyscada/
+-rwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)       75 2023-04-05 09:03:09.000000 pyscada-gpio-0.8.0/pyscada/__init__.py
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 12:22:03.611375 pyscada-gpio-0.8.0/pyscada/gpio/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      642 2023-04-05 09:41:23.000000 pyscada-gpio-0.8.0/pyscada/gpio/__init__.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     2208 2023-04-05 09:44:42.000000 pyscada-gpio-0.8.0/pyscada/gpio/admin.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      522 2023-04-05 09:27:41.000000 pyscada-gpio-0.8.0/pyscada/gpio/apps.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     2536 2021-05-19 13:00:02.000000 pyscada-gpio-0.8.0/pyscada/gpio/device.py
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 12:22:03.611375 pyscada-gpio-0.8.0/pyscada/gpio/migrations/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     2871 2019-11-20 08:26:36.000000 pyscada-gpio-0.8.0/pyscada/gpio/migrations/0001_initial.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1508 2023-04-05 09:44:37.000000 pyscada-gpio-0.8.0/pyscada/gpio/migrations/0002_add_device_protocol.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      423 2020-02-11 17:21:45.000000 pyscada-gpio-0.8.0/pyscada/gpio/migrations/0003_auto_20200211_1721.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      437 2022-01-05 10:13:09.000000 pyscada-gpio-0.8.0/pyscada/gpio/migrations/0004_auto_20220105_1013.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        0 2019-11-20 08:26:36.000000 pyscada-gpio-0.8.0/pyscada/gpio/migrations/__init__.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     2167 2022-05-04 10:09:16.000000 pyscada-gpio-0.8.0/pyscada/gpio/models.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1190 2023-04-05 09:44:48.000000 pyscada-gpio-0.8.0/pyscada/gpio/signals.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      514 2023-04-05 09:45:44.000000 pyscada-gpio-0.8.0/pyscada/gpio/worker.py
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 12:22:03.611375 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1839 2023-05-25 12:22:03.000000 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/PKG-INFO
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      686 2023-05-25 12:22:03.000000 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/SOURCES.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        1 2023-05-25 12:22:03.000000 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/dependency_links.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        1 2019-11-20 08:26:35.000000 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/not-zip-safe
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)       24 2023-05-25 12:22:03.000000 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/requires.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        8 2023-05-25 12:22:03.000000 pyscada-gpio-0.8.0/pyscada_gpio.egg-info/top_level.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)       38 2023-05-25 12:22:03.615375 pyscada-gpio-0.8.0/setup.cfg
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1406 2023-05-25 12:00:15.000000 pyscada-gpio-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyscada-gpio-0.7.0rc8/LICENSE` & `pyscada-gpio-0.8.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -631,44 +629,33 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
+    it under the terms of the GNU Affero General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `pyscada-gpio-0.7.0rc8/setup.py` & `pyscada-gpio-0.8.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 import os
-from pyscada import gpio
+from pyscada import gpio as pyscada_app
 
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Environment :: Web Environment',
     'Environment :: Console',
     'Framework :: Django',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
-    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+    'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
     'Operating System :: POSIX',
     'Operating System :: MacOS :: MacOS X',
     'Programming Language :: Python',
     'Programming Language :: JavaScript',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Scientific/Engineering :: Visualization'
 ]
 setup(
-    author=gpio.__author__,
-    author_email="info@martin-schroeder.net",
-    name='pyscada-gpio',
-    version=gpio.__version__,
-    description='GPIO extension for PyScada a Python and Django based Open Source SCADA System',
+    author=pyscada_app.__author__,
+    author_email=pyscada_app.__email__,
+    name='pyscada-' + pyscada_app.__app_name__.lower(),
+    version=pyscada_app.__version__,
+    description=pyscada_app.__description__,
     long_description=open(os.path.join(os.path.dirname(__file__), 'README.rst')).read(),
-    url='http://www.github.com/trombastic/PyScada',
-    license='GPL version 3',
+    url='http://www.github.com/pyscada/PyScada-' + pyscada_app.__app_name__,
+    license='AGPLv3',
     platforms=['OS Independent'],
     classifiers=CLASSIFIERS,
     install_requires=[
-        'pyscada',
+        'pyscada>=0.8.0',
         'rpi.gpio',
     ],
     packages=find_packages(exclude=["project", "project.*"]),
     include_package_data=True,
     zip_safe=False,
-    test_suite='runtests.main',
-    namespace_packages=['pyscada']
+    test_suite='runtests.main'
 )
```

### Comparing `pyscada-gpio-0.7.0rc8/pyscada/gpio/migrations/0002_add_device_protocol.py` & `pyscada-gpio-0.8.0/pyscada/gpio/migrations/0002_add_device_protocol.py`

 * *Files identical despite different names*

### Comparing `pyscada-gpio-0.7.0rc8/pyscada/gpio/migrations/0001_initial.py` & `pyscada-gpio-0.8.0/pyscada/gpio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyscada-gpio-0.7.0rc8/pyscada/gpio/admin.py` & `pyscada-gpio-0.8.0/pyscada/gpio/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 from pyscada.gpio import PROTOCOL_ID
-from pyscada.gpio.models import GPIODevice
-from pyscada.gpio.models import GPIOVariable
+from pyscada.gpio.models import GPIODevice, ExtendedGPIODevice
+from pyscada.gpio.models import GPIOVariable, ExtendedGPIOVariable
 from pyscada.admin import DeviceAdmin
 from pyscada.admin import VariableAdmin
 from pyscada.admin import admin_site
 from pyscada.models import Device, DeviceProtocol
-from pyscada.models import Variable
 from django.contrib import admin
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-class ExtendedGPIODevice(Device):
-    class Meta:
-        proxy = True
-        verbose_name = 'GPIO Device'
-        verbose_name_plural = 'GPIO Devices'
-
-
 class GPIODeviceAdminInline(admin.StackedInline):
     model = GPIODevice
 
 
 class GPIODeviceAdmin(DeviceAdmin):
     def formfield_for_foreignkey(self, db_field, request, **kwargs):
         if db_field.name == 'protocol':
@@ -39,21 +31,14 @@
         return qs.filter(protocol_id=PROTOCOL_ID)
 
     inlines = [
         GPIODeviceAdminInline
     ]
 
 
-class ExtendedGPIOVariable(Variable):
-    class Meta:
-        proxy = True
-        verbose_name = 'GPIO Variable'
-        verbose_name_plural = 'GPIO Variables'
-
-
 class GPIOVariableAdminInline(admin.StackedInline):
     model = GPIOVariable
 
 
 class GPIOVariableAdmin(VariableAdmin):
     list_display = ('id', 'name', 'description', 'unit', 'device_name', 'value_class', 'active', 'writeable')
     list_editable = ('active', 'writeable',)
@@ -71,9 +56,9 @@
         return qs.filter(device__protocol_id=PROTOCOL_ID)
 
     inlines = [
         GPIOVariableAdminInline
     ]
 
 
-admin_site.register(ExtendedGPIODevice, GPIODeviceAdmin)
-admin_site.register(ExtendedGPIOVariable, GPIOVariableAdmin)
+# admin_site.register(ExtendedGPIODevice, GPIODeviceAdmin)
+# admin_site.register(ExtendedGPIOVariable, GPIOVariableAdmin)
```

### Comparing `pyscada-gpio-0.7.0rc8/pyscada/gpio/device.py` & `pyscada-gpio-0.8.0/pyscada/gpio/device.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
-import pyscada
+import logging
+
+logger = logging.getLogger(__name__)
+_debug = 1
 
 try:
     import RPi.GPIO as GPIO
     _DRIVER_RPI_OK = True
-except ImportError:
+except (ImportError, RuntimeError):
+    logger.warning("Trying to import RPi.GPIO : not on a RPi or library not installed")
+    GPIO = None
     _DRIVER_RPI_OK = False
 
-from math import isnan, isinf
 from time import time
-import sys
-
-
-import logging
-
-logger = logging.getLogger(__name__)
-_debug = 1
 
 
 class Device:
     """
     GPIO device
     """
 
-    class Device:
-        def __init__(self, device):
-            self.variables = []
-            self.device = device
+    def __init__(self, device):
+        self.variables = []
+        self.device = device
+        if _DRIVER_RPI_OK:
+            GPIO.setmode(GPIO.BOARD)
+            # todo add cleanup
+
             for var in device.variable_set.filter(active=1):
                 if not hasattr(var, 'gpiovariable'):
                     continue
                 self.variables.append(var)
-                if var.gpiovariable.gpio_mode_choices == 'input_pull_up':
+                if var.gpiovariable.gpio_mode == 'input_pull_up':
                     GPIO.setup(int(var.gpiovariable.gpio_pin), GPIO.IN, pull_up_down=GPIO.PUD_UP)
-                elif var.gpiovariable.gpio_mode_choices == 'input_pull_down':
+                elif var.gpiovariable.gpio_mode == 'input_pull_down':
                     GPIO.setup(int(var.gpiovariable.gpio_pin), GPIO.IN, pull_up_down=GPIO.PUD_DOWN)
-                elif var.gpiovariable.gpio_mode_choices == 'input':
+                elif var.gpiovariable.gpio_mode == 'input':
                     GPIO.setup(int(var.gpiovariable.gpio_pin), GPIO.IN)
-                elif var.gpiovariable.gpio_mode_choices == 'output':
+                elif var.gpiovariable.gpio_mode == 'output':
                     GPIO.setup(int(var.gpiovariable.gpio_pin), GPIO.OUT)
 
-            if _DRIVER_RPI_OK:
-                GPIO.setmode(GPIO.BOARD)
-            #todo add cleanup
-
-        def request_data(self):
-            if not _DRIVER_RPI_OK:
-                return None
-            output = []
-            for item in self.variables:
-                timestamp = time()
-                #value = None
-
-                value = GPIO.input(int(item.gpiovariable.gpio_pin))
-                if value is not None and item.update_value(value, timestamp):
+    def request_data(self):
+        if not _DRIVER_RPI_OK:
+            return None
+        output = []
+        for item in self.variables:
+            if item.gpiovariable.gpio_mode == 'output':
+                continue
+
+            timestamp = time()
+            # value = None
+
+            value = GPIO.input(int(item.gpiovariable.gpio_pin))
+            if value is not None and item.update_value(value, timestamp):
+                output.append(item.create_recorded_data_element())
+
+        return output
+
+    def write_data(self, variable_id, value, task):
+        """
+        write value to single gpio pin
+        """
+        if not _DRIVER_RPI_OK:
+            return None
+
+        output = []
+
+        for item in self.variables:
+            if item.id == variable_id:
+                if not item.gpiovariable.gpio_mode == 'output' or not item.writeable:
+                    return False
+                GPIO.output(int(item.gpiovariable.gpio_pin), int(value))
+                if value is not None and item.update_value(value, time()):
                     output.append(item.create_recorded_data_element())
-
-            return output
-
-        def write_data(self, variable_id, value, task):
-            """
-            write value to single gpio pin
-            """
-            if not self.variables[variable_id].writeable:
-                return False
-
-            if not self.variables[variable_id].gpiovariable.gpio_mode_choices == 'output':
-                return False
-
-            GPIO.output(int(self.variables[variable_id].gpiovariable.gpio_pin), value)
-            return True
-
+        return output
```

### Comparing `pyscada-gpio-0.7.0rc8/pyscada/gpio/models.py` & `pyscada-gpio-0.8.0/pyscada/gpio/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
+from . import PROTOCOL_ID
 
 from pyscada.models import Device
 from pyscada.models import Variable
 
 from django.db import models
-from django.db.models.signals import post_save
-from django.dispatch import receiver
-from django.utils.encoding import python_2_unicode_compatible
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-@python_2_unicode_compatible
 class GPIODevice(models.Model):
-    gpio_device = models.OneToOneField(Device, null=True, blank=True)
+    gpio_device = models.OneToOneField(Device, null=True, blank=True, on_delete=models.CASCADE)
     board_choices = (('rpi', 'Raspberry Pi'),)
-    board = models.CharField(max_length=254, choices=board_choices, default='rpi')
+    board = models.CharField(max_length=254, default='rpi', choices=board_choices)
+
+    protocol_id = PROTOCOL_ID
+
+    def parent_device(self):
+        try:
+            return self.gpio_device
+        except:
+            return None
 
     def __str__(self):
         return self.gpio_device.short_name
 
 
-@python_2_unicode_compatible
 class GPIOVariable(models.Model):
-    gpio_variable = models.OneToOneField(Variable, null=True, blank=True)
+    gpio_variable = models.OneToOneField(Variable, null=True, blank=True, on_delete=models.CASCADE)
     gpio_mode_choices = (
         ('Polling', (('input', 'Input'),
                      ('input_pull_up', 'Input Pull Up'),
                      ('input_pull_down', 'Input Pull Down'),
                      ('output', 'Output'),),),
         ('Interupt Rising Edge (not implemented)',
          (('input_pull_up_rising', 'Input Pull Up'), ('input_pull_down_rising', 'Input Pull Down'),),),
@@ -37,21 +41,25 @@
          (('input_pull_up_falling', 'Input Pull Up'), ('input_pull_down_falling', 'Input Pull Down'),),),
         ('Interupt Both Edges (not implemented)',
          (('input_pull_up_both', 'Input Pull Up'), ('input_pull_down_both', 'Input Pull Down'),),),
     )
     gpio_mode = models.CharField(max_length=254, choices=gpio_mode_choices)
     gpio_pin = models.CharField(max_length=254, help_text="pin number in Board notation (pin number of the pin header)")
 
+    protocol_id = PROTOCOL_ID
+
     def __str__(self):
-        return self.gpio_device.short_name
+        return self.gpio_variable.name
+
+
+class ExtendedGPIODevice(Device):
+    class Meta:
+        proxy = True
+        verbose_name = 'GPIO Device'
+        verbose_name_plural = 'GPIO Devices'
 
 
-@receiver(post_save, sender=GPIODevice)
-@receiver(post_save, sender=GPIOVariable)
-def _reinit_daq_daemons(sender, instance, **kwargs):
-    """
-    update the daq daemon configuration when changes be applied in the models
-    """
-    if type(instance) is GPIODevice:
-        post_save.send_robust(sender=Device, instance=instance.gpio_device)
-    elif type(instance) is GPIOVariable:
-        post_save.send_robust(sender=Variable, instance=instance.gpio_variable)
+class ExtendedGPIOVariable(Variable):
+    class Meta:
+        proxy = True
+        verbose_name = 'GPIO Variable'
+        verbose_name_plural = 'GPIO Variables'
```

### Comparing `pyscada-gpio-0.7.0rc8/PKG-INFO` & `pyscada-gpio-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: pyscada-gpio
-Version: 0.7.0rc8
+Version: 0.8.0
 Summary: GPIO extension for PyScada a Python and Django based Open Source SCADA System
-Home-page: http://www.github.com/trombastic/PyScada
-Author: Martin Schröder
-Author-email: info@martin-schroeder.net
-License: GPL version 3
+Home-page: http://www.github.com/pyscada/PyScada-GPIO
+Author: Martin Schröder, Camille Lavayssiere
+Author-email: team@pyscada.org
+License: AGPLv3
 Description: PyScada GPIO Extension
         ======================
         
         This is a extension for PyScada to support read and write of GPIO Pins.
         
         
         What is Working
@@ -46,14 +46,14 @@
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `pyscada-gpio-0.7.0rc8/README.rst` & `pyscada-gpio-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/PKG-INFO` & `pyscada-gpio-0.8.0/pyscada_gpio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: pyscada-gpio
-Version: 0.7.0rc8
+Version: 0.8.0
 Summary: GPIO extension for PyScada a Python and Django based Open Source SCADA System
-Home-page: http://www.github.com/trombastic/PyScada
-Author: Martin Schröder
-Author-email: info@martin-schroeder.net
-License: GPL version 3
+Home-page: http://www.github.com/pyscada/PyScada-GPIO
+Author: Martin Schröder, Camille Lavayssiere
+Author-email: team@pyscada.org
+License: AGPLv3
 Description: PyScada GPIO Extension
         ======================
         
         This is a extension for PyScada to support read and write of GPIO Pins.
         
         
         What is Working
@@ -46,14 +46,14 @@
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `pyscada-gpio-0.7.0rc8/pyscada_gpio.egg-info/SOURCES.txt` & `pyscada-gpio-0.8.0/pyscada_gpio.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 CHANGELOG.txt
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 pyscada/__init__.py
 pyscada/gpio/__init__.py
-pyscada/gpio/__init__.pyc
 pyscada/gpio/admin.py
 pyscada/gpio/apps.py
 pyscada/gpio/device.py
 pyscada/gpio/models.py
+pyscada/gpio/signals.py
 pyscada/gpio/worker.py
 pyscada/gpio/migrations/0001_initial.py
 pyscada/gpio/migrations/0002_add_device_protocol.py
+pyscada/gpio/migrations/0003_auto_20200211_1721.py
+pyscada/gpio/migrations/0004_auto_20220105_1013.py
 pyscada/gpio/migrations/__init__.py
 pyscada_gpio.egg-info/PKG-INFO
 pyscada_gpio.egg-info/SOURCES.txt
 pyscada_gpio.egg-info/dependency_links.txt
-pyscada_gpio.egg-info/namespace_packages.txt
 pyscada_gpio.egg-info/not-zip-safe
 pyscada_gpio.egg-info/requires.txt
 pyscada_gpio.egg-info/top_level.txt
```

