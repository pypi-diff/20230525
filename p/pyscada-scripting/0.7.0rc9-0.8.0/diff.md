# Comparing `tmp/pyscada-scripting-0.7.0rc9.tar.gz` & `tmp/pyscada-scripting-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyscada-scripting-0.7.0rc9.tar", last modified: Fri Nov  9 10:05:09 2018, max compression
+gzip compressed data, was "pyscada-scripting-0.8.0.tar", last modified: Thu May 25 09:41:16 2023, max compression
```

## Comparing `pyscada-scripting-0.7.0rc9.tar` & `pyscada-scripting-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/
--rw-rw-r--   0 martin    (1000) martin    (1000)    35147 2018-07-08 23:18:13.000000 pyscada-scripting-0.7.0rc9/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      136 2018-07-08 23:18:13.000000 pyscada-scripting-0.7.0rc9/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     1412 2018-07-08 23:18:13.000000 pyscada-scripting-0.7.0rc9/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/migrations/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1108 2018-07-08 23:18:14.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/migrations/0001_initial.py
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2018-07-08 23:18:14.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/migrations/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    13678 2018-08-31 13:05:24.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/worker.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      335 2018-07-08 23:18:14.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/apps.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      486 2018-08-31 13:07:06.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      262 2018-07-08 23:18:14.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/admin.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1206 2018-07-09 12:06:06.000000 pyscada-scripting-0.7.0rc9/pyscada/scripting/models.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)       56 2018-07-09 12:05:59.000000 pyscada-scripting-0.7.0rc9/pyscada/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2041 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      287 2018-08-31 13:07:06.000000 pyscada-scripting-0.7.0rc9/CHANGELOG.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      761 2018-07-08 23:18:13.000000 pyscada-scripting-0.7.0rc9/README.rst
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)        8 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2018-07-08 23:18:13.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/not-zip-safe
--rw-rw-r--   0 martin    (1000) martin    (1000)        8 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     2041 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      600 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        8 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/namespace_packages.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2018-11-09 10:05:09.000000 pyscada-scripting-0.7.0rc9/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      153 2018-07-08 23:18:13.000000 pyscada-scripting-0.7.0rc9/AUTHORS
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      197 2023-04-05 09:03:09.000000 pyscada-scripting-0.8.0/AUTHORS
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      287 2019-11-20 08:26:37.000000 pyscada-scripting-0.8.0/CHANGELOG.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)    34523 2023-03-27 14:51:28.000000 pyscada-scripting-0.8.0/LICENSE
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      137 2023-04-05 08:57:41.000000 pyscada-scripting-0.8.0/MANIFEST.in
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     2067 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/PKG-INFO
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      770 2023-04-05 08:57:41.000000 pyscada-scripting-0.8.0/README.rst
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/pyscada/
+-rwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)       75 2023-04-05 09:03:09.000000 pyscada-scripting-0.8.0/pyscada/__init__.py
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/pyscada/scripting/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      613 2023-04-05 13:35:35.000000 pyscada-scripting-0.8.0/pyscada/scripting/__init__.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      489 2021-11-26 14:43:08.000000 pyscada-scripting-0.8.0/pyscada/scripting/admin.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      526 2023-04-05 09:27:41.000000 pyscada-scripting-0.8.0/pyscada/scripting/apps.py
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/pyscada/scripting/migrations/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1108 2019-11-20 08:26:37.000000 pyscada-scripting-0.8.0/pyscada/scripting/migrations/0001_initial.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        0 2019-11-20 08:26:37.000000 pyscada-scripting-0.8.0/pyscada/scripting/migrations/__init__.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1072 2022-05-04 12:43:26.000000 pyscada-scripting-0.8.0/pyscada/scripting/models.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1524 2022-06-01 16:17:22.000000 pyscada-scripting-0.8.0/pyscada/scripting/signals.py
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)    15729 2022-05-26 21:26:46.000000 pyscada-scripting-0.8.0/pyscada/scripting/worker.py
+drwxr-xr-x   0 clavayssiere  (1000) clavayssiere  (1000)        0 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     2067 2023-05-25 09:41:16.000000 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/PKG-INFO
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)      579 2023-05-25 09:41:16.000000 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/SOURCES.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        1 2023-05-25 09:41:16.000000 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/dependency_links.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        1 2019-11-20 08:26:37.000000 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/not-zip-safe
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)       15 2023-05-25 09:41:16.000000 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/requires.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)        8 2023-05-25 09:41:16.000000 pyscada-scripting-0.8.0/pyscada_scripting.egg-info/top_level.txt
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)       38 2023-05-25 09:41:16.834434 pyscada-scripting-0.8.0/setup.cfg
+-rw-r--r--   0 clavayssiere  (1000) clavayssiere  (1000)     1391 2023-05-25 09:40:12.000000 pyscada-scripting-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyscada-scripting-0.7.0rc9/LICENSE` & `pyscada-scripting-0.8.0/LICENSE`

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

### Comparing `pyscada-scripting-0.7.0rc9/pyscada/scripting/migrations/0001_initial.py` & `pyscada-scripting-0.8.0/pyscada/scripting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyscada-scripting-0.7.0rc9/pyscada/scripting/worker.py` & `pyscada-scripting-0.8.0/pyscada/scripting/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,19 @@
     # Python 3.5+
     from importlib.util import spec_from_file_location, module_from_spec
     from types import MethodType
 
     def import_module_from_file(inst, file_name, func_name):
         spec = spec_from_file_location('pyscada.scripting.user_script', file_name)
         mod = module_from_spec(spec)
-        spec.loader.exec_module(mod)
+        try:
+            spec.loader.exec_module(mod)
+        except FileNotFoundError:
+            logger.warning("Script file not found : " + str(spec.origin))
+            return None
         if not hasattr(mod, func_name):
             return None
         return MethodType(getattr(mod, func_name), inst)
 
 except:
     try:
         # Python 3.3, 3.4
@@ -82,15 +86,15 @@
         :param value:
         :return:
         """
         self.data[instance.name] = [timestamp, value]
 
     def read_values_from_db(self, variable_names, time_from=None, time_to=None, mean_value_period=0,
                             no_mean_value=True, add_latest_value=True, query_first_value=True,
-                            current_value_only=False):
+                            current_value_only=False, blow_up=False):
         """
         read data from the database
         :param current_value_only:
         :param variable_names:
         :param time_from:
         :param time_to:
         :param mean_value_period:
@@ -113,22 +117,25 @@
         """
         data = RecordedData.objects.get_values_in_time_range(
             variable__in=variables,
             time_min=time_from,
             time_max=time_to,
             query_first_value=query_first_value,
             key_is_variable_name=True,
-            blow_up=True,
+            blow_up=blow_up,
             add_latest_value=add_latest_value,
             mean_value_period=mean_value_period if mean_value_period != 0 else 5.0,
             no_mean_value=True if mean_value_period != 0 else no_mean_value
         )
         if current_value_only:
             for key, item in data.items():
-                data[key] = item[-1]
+                if len(item) > 0:
+                    data[key] = item[-1]
+                else:
+                    logger.debug('Variable (Current value only) %s has no value in time range [%s,%s]' %(key, time_from, time_to))
             return data
 
         for key, item in data.items():
             data[key] = np.asarray(item),
 
         return data
 
@@ -155,15 +162,15 @@
         if not variable:
             # todo throw exception
             return False
         if not variable.writeable:
             # todo throw exception
             return False
         dwt = DeviceWriteTask(variable=variable, value=value, start=time_start, user=user)
-        dwt.save()
+        dwt.create_and_notificate(dwt)
         if blocking:
             timeout = max(time(), time_start) + timeout
             while timeout < time():
                 dwt.refresh_from_db()
                 if dwt.done():
                     return True
             return False
@@ -272,14 +279,18 @@
             if self.shutdown is not None:
                 self.shutdown()
         except:
             logger.error('%s(%d), unhandled exception in shutdown\n%s' % (self.label, getpid(), traceback.format_exc()))
         # delete the background process entry
         BackgroundProcess.objects.filter(pk=self.process_id).delete()
 
+    def restart(self):
+        self.signal(self.SIGNALS[0])
+        return True
+
     def script(self):
         """
         to be overwritten by the script
         :return:
         """
         pass
 
@@ -303,67 +314,101 @@
     handle the registration of new script tasks, and monitor running script tasks
     """
 
     def __init__(self, dt=5, **kwargs):
         super(MasterProcess, self).__init__(dt=dt, **kwargs)
         self.SCRIPT_PROCESSES = []
 
+    def _add_process_to_list(self, script_process):
+        bp = BackgroundProcess(label='pyscada.scripting-%d' % script_process.pk,
+                               message='waiting..',
+                               enabled=True,
+                               parent_process_id=self.process_id,
+                               process_class='pyscada.scripting.worker.ScriptingProcess',
+                               process_class_kwargs=json.dumps({"script_id": script_process.pk,
+                                                                'script_file': script_process.script_file,
+                                                                'dt_set': script_process.interval}))
+        bp.save()
+        self.SCRIPT_PROCESSES.append({'id': bp.id,
+                                      'script_id': script_process.pk,
+                                      'failed': 0})
+
     def init_process(self):
+        """
         for process in BackgroundProcess.objects.filter(parent_process__pk=self.process_id, done=False):
             try:
                 kill(process.pid, 0)
             except OSError as e:
                 if e.errno == errno.ESRCH:
                     process.delete()
                     continue
             logger.debug('process %d is alive' % process.pk)
             process.stop()
 
         # clean up
         BackgroundProcess.objects.filter(parent_process__pk=self.process_id, done=False).delete()
-
+        """
         for script_process in Script.objects.filter(active=True):
-            bp = BackgroundProcess(label='pyscada.scripting.ScriptingProcess-%d' % script_process.pk,
-                                   message='waiting..',
-                                   enabled=True,
-                                   parent_process_id=self.process_id,
-                                   process_class='pyscada.scripting.worker.ScriptingProcess',
-                                   process_class_kwargs=json.dumps({"script_id": script_process.pk,
-                                                                    'script_file': script_process.script_file,
-                                                                    'dt_set': script_process.interval}))
-            bp.save()
-            self.SCRIPT_PROCESSES.append({'id': bp.id,
-                                          'script_id':script_process.pk,
-                                          'failed': 0})
+            self._add_process_to_list(script_process)
 
     def loop(self):
         """
 
         """
-        # check if all modbus processes are running
+        #logger.debug(self.SCRIPT_PROCESSES)
+        #logger.debug(Script.objects.filter(active=True))
+        # add new active scripts
+        for s in Script.objects.filter(active=True):
+            script_found = False
+            for script_process in self.SCRIPT_PROCESSES:
+                if s.pk == script_process['script_id']:
+                    script_found = True
+            if not script_found:
+                logger.info("%s not found - add script to %s" % (s.label, self.label))
+                self._add_process_to_list(s)
+
+        #logger.debug("script master loop")
+
+        # check if all scripting processes are running
         for script_process in self.SCRIPT_PROCESSES:
             try:
-                BackgroundProcess.objects.get(pk=script_process['id'])
-            except BackgroundProcess.DoesNotExist or BackgroundProcess.MultipleObjectsReturned:
+                bp = BackgroundProcess.objects.get(pk=script_process['id'])
+                # stop deactivated script and remove from list
+                try:
+                    if not Script.objects.get(pk=script_process['script_id']).active:
+                        bp.stop(cleanup=True)
+                        logger.debug("stop %s" % bp)
+                        logger.debug("remove %s" % script_process)
+                        self.SCRIPT_PROCESSES.remove(script_process)
+                except Script.DoesNotExist:
+                    bp.stop(cleanup=True)
+                    logger.debug("stop %s" % bp)
+                    logger.debug("remove %s" % script_process)
+                    self.SCRIPT_PROCESSES.remove(script_process)
+            except (BackgroundProcess.DoesNotExist, BackgroundProcess.MultipleObjectsReturned):
                 # Process is dead, spawn new instance
                 if script_process['failed'] < 3:
-                    script = Script.objects.get(pk=script_process['script_id'])
-                    bp = BackgroundProcess(label='pyscada.scripting.ScriptingProcess-%d' % script.pk,
-                                           message='waiting..',
-                                           enabled=True,
-                                           parent_process_id=self.process_id,
-                                           process_class='pyscada.scripting.worker.ScriptingProcess',
-                                           process_class_kwargs=json.dumps({"script_id": script.pk,
-                                                                            'script_file': script.script_file,
-                                                                            'dt_set': script.interval}))
-                    bp.save()
-                    script_process['id'] = bp.id
-                    script_process['failed'] += 1
+                    try:
+                        script = Script.objects.get(pk=script_process['script_id'], active=True)
+                        bp = BackgroundProcess(label='pyscada.scripting-%d' % script.pk,
+                                               message='waiting..',
+                                               enabled=True,
+                                               parent_process_id=self.process_id,
+                                               process_class='pyscada.scripting.worker.ScriptingProcess',
+                                               process_class_kwargs=json.dumps({"script_id": script.pk,
+                                                                                'script_file': script.script_file,
+                                                                                'dt_set': script.interval}))
+                        bp.save()
+                        script_process['id'] = bp.id
+                        script_process['failed'] += 1
+                    except Script.DoesNotExist:
+                        logger.debug("removing %s from list" % script_process)
+                        self.SCRIPT_PROCESSES.remove(script_process)
                 else:
-                    logger.error('process pyscada.scripting.user_script-%d failed more then 3 times' % script_process['script_id'])
+                    logger.error('process pyscada.scripting.user_script-%d failed more than 3 times' % script_process['script_id'])
             except:
                 logger.debug('%s, unhandled exception\n%s' % (self.label, traceback.format_exc()))
 
         return 1, None
 
     def cleanup(self):
         # todo cleanup
@@ -374,8 +419,7 @@
             try:
                 bp = BackgroundProcess.objects.get(pk=script_process['id'])
                 bp.restart()
             except:
                 logger.debug('%s, unhandled exception\n%s' % (self.label, traceback.format_exc()))
 
         return False
-
```

### Comparing `pyscada-scripting-0.7.0rc9/pyscada/scripting/models.py` & `pyscada-scripting-0.8.0/pyscada/scripting/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 
 from django.db import models
-from django.utils.encoding import python_2_unicode_compatible
-from os import getpid
-import traceback
 
 import logging
 logger = logging.getLogger(__name__)
 
 
-@python_2_unicode_compatible
 class Script(models.Model):
     id = models.AutoField(primary_key=True)
     label = models.CharField(max_length=255,default='', blank=True)
     active = models.BooleanField(default=True)
     interval_choices = (
         (0.1, '100 Milliseconds'),
         (0.5, '500 Milliseconds'),
@@ -34,11 +30,7 @@
         (3600.0, '1 Hour'),
     )
     interval = models.FloatField(default=5, choices=interval_choices)
     script_file = models.CharField(max_length=255, default='', help_text='')
 
     def __str__(self):
         return '%s: (%s)'%(self.label,self.script_file)
-
-
-
-
```

### Comparing `pyscada-scripting-0.7.0rc9/PKG-INFO` & `pyscada-scripting-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: pyscada-scripting
-Version: 0.7.0rc9
+Version: 0.8.0
 Summary: Scripting extension for PyScada a Python and Django based Open Source SCADA System
-Home-page: http://www.github.com/trombastic/PyScada-Scripting
-Author: Martin Schröder
-Author-email: info@martin-schroeder.net
-License: GPL version 3
+Home-page: http://www.github.com/pyscada/PyScada-Scripting
+Author: Martin Schröder, Camille Lavayssiere
+Author-email: team@pyscada.org
+License: AGPLv3
 Description: PyScada Scripting Extension
         ===========================
         
         This is a extension for PyScada to support periodically executing scripts. For more information see the example script
         (extras/sample_script).
         
         
@@ -32,31 +32,31 @@
         
          - pip install pyscada-scripting
         
         
         Contribute
         ----------
         
-         - Issue Tracker: https://github.com/trombastic/PyScada-Scripting/issues
-         - Source Code: https://github.com/trombastic/PyScada-Scripting
+         - Issue Tracker: https://github.com/pyscada/PyScada-Scripting/issues
+         - Source Code: https://github.com/pyscada/PyScada-Scripting
          
         
         License
         -------
         
-        The project is licensed under the _GNU General Public License v3 (GPLv3)_.
+        The project is licensed under the _GNU AFFERO GENERAL PUBLIC LICENSE Version 3 (AGPLv3)_.
         -
         
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

### Comparing `pyscada-scripting-0.7.0rc9/README.rst` & `pyscada-scripting-0.8.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
  - pip install pyscada-scripting
 
 
 Contribute
 ----------
 
- - Issue Tracker: https://github.com/trombastic/PyScada-Scripting/issues
- - Source Code: https://github.com/trombastic/PyScada-Scripting
+ - Issue Tracker: https://github.com/pyscada/PyScada-Scripting/issues
+ - Source Code: https://github.com/pyscada/PyScada-Scripting
  
 
 License
 -------
 
-The project is licensed under the _GNU General Public License v3 (GPLv3)_.
+The project is licensed under the _GNU AFFERO GENERAL PUBLIC LICENSE Version 3 (AGPLv3)_.
 -
```

### Comparing `pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/PKG-INFO` & `pyscada-scripting-0.8.0/pyscada_scripting.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: pyscada-scripting
-Version: 0.7.0rc9
+Version: 0.8.0
 Summary: Scripting extension for PyScada a Python and Django based Open Source SCADA System
-Home-page: http://www.github.com/trombastic/PyScada-Scripting
-Author: Martin Schröder
-Author-email: info@martin-schroeder.net
-License: GPL version 3
+Home-page: http://www.github.com/pyscada/PyScada-Scripting
+Author: Martin Schröder, Camille Lavayssiere
+Author-email: team@pyscada.org
+License: AGPLv3
 Description: PyScada Scripting Extension
         ===========================
         
         This is a extension for PyScada to support periodically executing scripts. For more information see the example script
         (extras/sample_script).
         
         
@@ -32,31 +32,31 @@
         
          - pip install pyscada-scripting
         
         
         Contribute
         ----------
         
-         - Issue Tracker: https://github.com/trombastic/PyScada-Scripting/issues
-         - Source Code: https://github.com/trombastic/PyScada-Scripting
+         - Issue Tracker: https://github.com/pyscada/PyScada-Scripting/issues
+         - Source Code: https://github.com/pyscada/PyScada-Scripting
          
         
         License
         -------
         
-        The project is licensed under the _GNU General Public License v3 (GPLv3)_.
+        The project is licensed under the _GNU AFFERO GENERAL PUBLIC LICENSE Version 3 (AGPLv3)_.
         -
         
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

### Comparing `pyscada-scripting-0.7.0rc9/pyscada_scripting.egg-info/SOURCES.txt` & `pyscada-scripting-0.8.0/pyscada_scripting.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 README.rst
 setup.py
 pyscada/__init__.py
 pyscada/scripting/__init__.py
 pyscada/scripting/admin.py
 pyscada/scripting/apps.py
 pyscada/scripting/models.py
+pyscada/scripting/signals.py
 pyscada/scripting/worker.py
 pyscada/scripting/migrations/0001_initial.py
 pyscada/scripting/migrations/__init__.py
 pyscada_scripting.egg-info/PKG-INFO
 pyscada_scripting.egg-info/SOURCES.txt
 pyscada_scripting.egg-info/dependency_links.txt
-pyscada_scripting.egg-info/namespace_packages.txt
 pyscada_scripting.egg-info/not-zip-safe
 pyscada_scripting.egg-info/requires.txt
 pyscada_scripting.egg-info/top_level.txt
```

