# Comparing `tmp/pyhyypapihawkmod-0.0.0.6.tar.gz` & `tmp/pyhyypapihawkmod-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-0.0.0.6.tar", last modified: Mon May 22 15:01:42 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-0.0.0.7.tar", last modified: Thu May 25 18:50:11 2023, max compression
```

## Comparing `pyhyypapihawkmod-0.0.0.6.tar` & `pyhyypapihawkmod-0.0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/
--rw-rw-rw-   0        0        0    11357 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0       19 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1178 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 15:01:42.717686 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      412 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      146 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     4682 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2780 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2825 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    25351 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     3869 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      235 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7492 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    15720 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:50:11.521609 pyhyypapihawkmod-0.0.0.7/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-05-25 18:50:11.520596 pyhyypapihawkmod-0.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2023-05-24 19:47:40.000000 pyhyypapihawkmod-0.0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 18:50:11.508441 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     6750 2023-05-25 18:41:13.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    26159 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:50:11.518574 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 18:50:11.521609 pyhyypapihawkmod-0.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-05-25 18:39:15.000000 pyhyypapihawkmod-0.0.0.7/setup.py
```

### Comparing `pyhyypapihawkmod-0.0.0.6/LICENSE.md` & `pyhyypapihawkmod-0.0.0.7/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `pyhyypapihawkmod-0.0.0.6/PKG-INFO` & `pyhyypapihawkmod-0.0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.6/README.md` & `pyhyypapihawkmod-0.0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. THis fixes the issues on newer versions of home assistant.
-
-# pyHyypApi
-API for ADT Secure Home and IDS Hyyp. There could be more variants but it's easy to add package names to the constants.py file.
-
-How to use:
-
-  1. Install:
-
-```pip install pyhyypapihawkmod```
-
-  2.1. Login (ADT Secure Home):
-
-
-```
-import pyhyypapihawkmod
-import json
-client = pyhyypapihawkmod.hyypclient(email="",password="")
-client.login()
-```
-
-**OR**
-
-  2.2. Login (IDT Hyyp):
-
-```
-import pyhyypapihawkmod
-import json
-client = pyhyypapihawkmod.hyypclient(email="",password="",pkg=pyhyypapihawkmod.HyypPkg.IDS_HYYP_GENERIC.value)
-client.login()
-
-```
-
-
-3. Get site/partition/user/zone info:
-
-```
-print(json.dumps(client.get_sync_info(),indent=2))
-
-```
-
-TO Do:
-
-- CLI usage. (GCF client is there, just needs some more automation.)
-- Capture panic api...for obvious reasons.
-- What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
+This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. THis fixes the issues on newer versions of home assistant.
+
+# pyHyypApi
+API for ADT Secure Home and IDS Hyyp. There could be more variants but it's easy to add package names to the constants.py file.
+
+How to use:
+
+  1. Install:
+
+```pip install pyhyypapihawkmod```
+
+  2.1. Login (ADT Secure Home):
+
+
+```
+import pyhyypapihawkmod
+import json
+client = pyhyypapihawkmod.HyypClient(email="",password="")
+client.login()
+```
+
+**OR**
+
+  2.2. Login (IDT Hyyp):
+
+```
+import pyhyypapihawkmod
+import json
+client = pyhyypapihawkmod.HyypClient(email="",password="",pkg=pyhyypapihawkmod.HyypPkg.IDS_HYYP_GENERIC.value)
+client.login()
+
+```
+
+
+3. Get site/partition/user/zone info:
+
+```
+print(json.dumps(client.get_sync_info(),indent=2))
+
+```
+
+TO Do:
+
+- CLI usage. (GCF client is there, just needs some more automation.)
+- Capture panic api...for obvious reasons.
+- What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
```

### Comparing `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: android_checkin.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61ndroid_checkin.proto\x12\rcheckin_proto\"\x8a\x03\n\x10\x43hromeBuildProto\x12:\n\x08platform\x18\x01 \x01(\x0e\x32(.checkin_proto.ChromeBuildProto.Platform\x12\x16\n\x0e\x63hrome_version\x18\x02 \x01(\t\x12\x38\n\x07\x63hannel\x18\x03 \x01(\x0e\x32\'.checkin_proto.ChromeBuildProto.Channel\"}\n\x08Platform\x12\x10\n\x0cPLATFORM_WIN\x10\x01\x12\x10\n\x0cPLATFORM_MAC\x10\x02\x12\x12\n\x0ePLATFORM_LINUX\x10\x03\x12\x11\n\rPLATFORM_CROS\x10\x04\x12\x10\n\x0cPLATFORM_IOS\x10\x05\x12\x14\n\x10PLATFORM_ANDROID\x10\x06\"i\n\x07\x43hannel\x12\x12\n\x0e\x43HANNEL_STABLE\x10\x01\x12\x10\n\x0c\x43HANNEL_BETA\x10\x02\x12\x0f\n\x0b\x43HANNEL_DEV\x10\x03\x12\x12\n\x0e\x43HANNEL_CANARY\x10\x04\x12\x13\n\x0f\x43HANNEL_UNKNOWN\x10\x05\"\xf6\x01\n\x13\x41ndroidCheckinProto\x12\x19\n\x11last_checkin_msec\x18\x02 \x01(\x03\x12\x15\n\rcell_operator\x18\x06 \x01(\t\x12\x14\n\x0csim_operator\x18\x07 \x01(\t\x12\x0f\n\x07roaming\x18\x08 \x01(\t\x12\x13\n\x0buser_number\x18\t \x01(\x05\x12:\n\x04type\x18\x0c \x01(\x0e\x32\x19.checkin_proto.DeviceType:\x11\x44\x45VICE_ANDROID_OS\x12\x35\n\x0c\x63hrome_build\x18\r \x01(\x0b\x32\x1f.checkin_proto.ChromeBuildProto*g\n\nDeviceType\x12\x15\n\x11\x44\x45VICE_ANDROID_OS\x10\x01\x12\x11\n\rDEVICE_IOS_OS\x10\x02\x12\x19\n\x15\x44\x45VICE_CHROME_BROWSER\x10\x03\x12\x14\n\x10\x44\x45VICE_CHROME_OS\x10\x04\x42\x02H\x03')
-
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_checkin_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_DEVICETYPE']._serialized_start=686
-  _globals['_DEVICETYPE']._serialized_end=789
-  _globals['_CHROMEBUILDPROTO']._serialized_start=41
-  _globals['_CHROMEBUILDPROTO']._serialized_end=435
-  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_start=203
-  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_end=328
-  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_start=330
-  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_end=435
-  _globals['_ANDROIDCHECKINPROTO']._serialized_start=438
-  _globals['_ANDROIDCHECKINPROTO']._serialized_end=684
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: android_checkin.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61ndroid_checkin.proto\x12\rcheckin_proto\"\x8a\x03\n\x10\x43hromeBuildProto\x12:\n\x08platform\x18\x01 \x01(\x0e\x32(.checkin_proto.ChromeBuildProto.Platform\x12\x16\n\x0e\x63hrome_version\x18\x02 \x01(\t\x12\x38\n\x07\x63hannel\x18\x03 \x01(\x0e\x32\'.checkin_proto.ChromeBuildProto.Channel\"}\n\x08Platform\x12\x10\n\x0cPLATFORM_WIN\x10\x01\x12\x10\n\x0cPLATFORM_MAC\x10\x02\x12\x12\n\x0ePLATFORM_LINUX\x10\x03\x12\x11\n\rPLATFORM_CROS\x10\x04\x12\x10\n\x0cPLATFORM_IOS\x10\x05\x12\x14\n\x10PLATFORM_ANDROID\x10\x06\"i\n\x07\x43hannel\x12\x12\n\x0e\x43HANNEL_STABLE\x10\x01\x12\x10\n\x0c\x43HANNEL_BETA\x10\x02\x12\x0f\n\x0b\x43HANNEL_DEV\x10\x03\x12\x12\n\x0e\x43HANNEL_CANARY\x10\x04\x12\x13\n\x0f\x43HANNEL_UNKNOWN\x10\x05\"\xf6\x01\n\x13\x41ndroidCheckinProto\x12\x19\n\x11last_checkin_msec\x18\x02 \x01(\x03\x12\x15\n\rcell_operator\x18\x06 \x01(\t\x12\x14\n\x0csim_operator\x18\x07 \x01(\t\x12\x0f\n\x07roaming\x18\x08 \x01(\t\x12\x13\n\x0buser_number\x18\t \x01(\x05\x12:\n\x04type\x18\x0c \x01(\x0e\x32\x19.checkin_proto.DeviceType:\x11\x44\x45VICE_ANDROID_OS\x12\x35\n\x0c\x63hrome_build\x18\r \x01(\x0b\x32\x1f.checkin_proto.ChromeBuildProto*g\n\nDeviceType\x12\x15\n\x11\x44\x45VICE_ANDROID_OS\x10\x01\x12\x11\n\rDEVICE_IOS_OS\x10\x02\x12\x19\n\x15\x44\x45VICE_CHROME_BROWSER\x10\x03\x12\x14\n\x10\x44\x45VICE_CHROME_OS\x10\x04\x42\x02H\x03')
+
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_checkin_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'H\003'
+  _globals['_DEVICETYPE']._serialized_start=686
+  _globals['_DEVICETYPE']._serialized_end=789
+  _globals['_CHROMEBUILDPROTO']._serialized_start=41
+  _globals['_CHROMEBUILDPROTO']._serialized_end=435
+  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_start=203
+  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_end=328
+  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_start=330
+  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_end=435
+  _globals['_ANDROIDCHECKINPROTO']._serialized_start=438
+  _globals['_ANDROIDCHECKINPROTO']._serialized_end=684
+# @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/checkin_pb2.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: checkin.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from . import android_checkin_pb2 as android__checkin__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcheckin.proto\x12\rcheckin_proto\x1a\x15\x61ndroid_checkin.proto\"/\n\x10GservicesSetting\x12\x0c\n\x04name\x18\x01 \x02(\x0c\x12\r\n\x05value\x18\x02 \x02(\x0c\"\xcb\x03\n\x15\x41ndroidCheckinRequest\x12\x0c\n\x04imei\x18\x01 \x01(\t\x12\x0c\n\x04meid\x18\n \x01(\t\x12\x10\n\x08mac_addr\x18\t \x03(\t\x12\x15\n\rmac_addr_type\x18\x13 \x03(\t\x12\x15\n\rserial_number\x18\x10 \x01(\t\x12\x0b\n\x03\x65sn\x18\x11 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x12\n\nlogging_id\x18\x07 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x33\n\x07\x63heckin\x18\x04 \x02(\x0b\x32\".checkin_proto.AndroidCheckinProto\x12\x15\n\rdesired_build\x18\x05 \x01(\t\x12\x16\n\x0emarket_checkin\x18\x08 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_cookie\x18\x0b \x03(\t\x12\x11\n\ttime_zone\x18\x0c \x01(\t\x12\x16\n\x0esecurity_token\x18\r \x01(\x06\x12\x0f\n\x07version\x18\x0e \x01(\x05\x12\x10\n\x08ota_cert\x18\x0f \x03(\t\x12\x10\n\x08\x66ragment\x18\x14 \x01(\x05\x12\x11\n\tuser_name\x18\x15 \x01(\t\x12\x1a\n\x12user_serial_number\x18\x16 \x01(\x05\"\x83\x02\n\x16\x41ndroidCheckinResponse\x12\x10\n\x08stats_ok\x18\x01 \x02(\x08\x12\x11\n\ttime_msec\x18\x03 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x04 \x01(\t\x12\x15\n\rsettings_diff\x18\t \x01(\x08\x12\x16\n\x0e\x64\x65lete_setting\x18\n \x03(\t\x12\x30\n\x07setting\x18\x05 \x03(\x0b\x32\x1f.checkin_proto.GservicesSetting\x12\x11\n\tmarket_ok\x18\x06 \x01(\x08\x12\x12\n\nandroid_id\x18\x07 \x01(\x06\x12\x16\n\x0esecurity_token\x18\x08 \x01(\x06\x12\x14\n\x0cversion_info\x18\x0b \x01(\tB\x02H\x03')
-
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'checkin_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_GSERVICESSETTING']._serialized_start=55
-  _globals['_GSERVICESSETTING']._serialized_end=102
-  _globals['_ANDROIDCHECKINREQUEST']._serialized_start=105
-  _globals['_ANDROIDCHECKINREQUEST']._serialized_end=564
-  _globals['_ANDROIDCHECKINRESPONSE']._serialized_start=567
-  _globals['_ANDROIDCHECKINRESPONSE']._serialized_end=826
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: checkin.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from . import android_checkin_pb2 as android__checkin__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcheckin.proto\x12\rcheckin_proto\x1a\x15\x61ndroid_checkin.proto\"/\n\x10GservicesSetting\x12\x0c\n\x04name\x18\x01 \x02(\x0c\x12\r\n\x05value\x18\x02 \x02(\x0c\"\xcb\x03\n\x15\x41ndroidCheckinRequest\x12\x0c\n\x04imei\x18\x01 \x01(\t\x12\x0c\n\x04meid\x18\n \x01(\t\x12\x10\n\x08mac_addr\x18\t \x03(\t\x12\x15\n\rmac_addr_type\x18\x13 \x03(\t\x12\x15\n\rserial_number\x18\x10 \x01(\t\x12\x0b\n\x03\x65sn\x18\x11 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x12\n\nlogging_id\x18\x07 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x33\n\x07\x63heckin\x18\x04 \x02(\x0b\x32\".checkin_proto.AndroidCheckinProto\x12\x15\n\rdesired_build\x18\x05 \x01(\t\x12\x16\n\x0emarket_checkin\x18\x08 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_cookie\x18\x0b \x03(\t\x12\x11\n\ttime_zone\x18\x0c \x01(\t\x12\x16\n\x0esecurity_token\x18\r \x01(\x06\x12\x0f\n\x07version\x18\x0e \x01(\x05\x12\x10\n\x08ota_cert\x18\x0f \x03(\t\x12\x10\n\x08\x66ragment\x18\x14 \x01(\x05\x12\x11\n\tuser_name\x18\x15 \x01(\t\x12\x1a\n\x12user_serial_number\x18\x16 \x01(\x05\"\x83\x02\n\x16\x41ndroidCheckinResponse\x12\x10\n\x08stats_ok\x18\x01 \x02(\x08\x12\x11\n\ttime_msec\x18\x03 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x04 \x01(\t\x12\x15\n\rsettings_diff\x18\t \x01(\x08\x12\x16\n\x0e\x64\x65lete_setting\x18\n \x03(\t\x12\x30\n\x07setting\x18\x05 \x03(\x0b\x32\x1f.checkin_proto.GservicesSetting\x12\x11\n\tmarket_ok\x18\x06 \x01(\x08\x12\x12\n\nandroid_id\x18\x07 \x01(\x06\x12\x16\n\x0esecurity_token\x18\x08 \x01(\x06\x12\x14\n\x0cversion_info\x18\x0b \x01(\tB\x02H\x03')
+
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'checkin_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'H\003'
+  _globals['_GSERVICESSETTING']._serialized_start=55
+  _globals['_GSERVICESSETTING']._serialized_end=102
+  _globals['_ANDROIDCHECKINREQUEST']._serialized_start=105
+  _globals['_ANDROIDCHECKINREQUEST']._serialized_end=564
+  _globals['_ANDROIDCHECKINRESPONSE']._serialized_start=567
+  _globals['_ANDROIDCHECKINRESPONSE']._serialized_end=826
+# @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/constants.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-"""Hyyp API constants."""
-from enum import Enum
-
-DEFAULT_TIMEOUT = 25
-MAX_RETRIES = 3
-GCF_SENDER_ID = 87969245803
-REQUEST_HEADER = {
-    "User-Agent": "okhttp/3.12.1",
-}  # Standard android header.
-STD_PARAMS = {
-    "imei": "152419714130158",  # Alphabet soup starts at 0
-    "appVersionCode": "401",
-    "_appVersionCode": "401",
-    "deviceOS": "12.0",
-    "deviceName": "Python API",
-    "pkg": "za.co.adt.securehome.android",
-    "_appVersionName": "3.5.19",
-    "token": None,
-}  # Standard request parameters.
-
-# Rpc to name mapping. Used in push notifications.
-RpcCodes = {
-    "202": "IMEI unknown to SMART platform. Registration failed.",
-    "203": "Command failed",
-    "204": "VALUE is invalid",
-    "205": "User code invalid",
-    "206": "Unit busy",
-    "207": "Command was older than abort command time",
-    "208": "Communications timeout to peripheral attached to Hub",
-    "209": "Invalid PID in topic",
-    "210": "Serial code mismatch",
-}
-
-# EventCategory to name mapping.
-# Used in notifications.
-EventCategory = {"1": "Emergency", "2": "User", "3": "Trouble", "4": "Information"}
-
-
-class HyypPkg(Enum):
-    """Supported hyyp skins/rebranding."""
-
-    ADT_SECURE_HOME = "za.co.adt.securehome.android"
-    IDS_HYYP_GENERIC = "com.hyyp247.home"
-
-
-# EventNumber to name mapping.
-EventNumber = {
-    "50": "AC clock",
-    "13": "AC fail",
-    "24": "AC Restore",
-    "3": "Alarm cancel",
-    "7": "Armed with bypassed zone",
-    "43": "Auto arm cancel",
-    "0": "Away arm",
-    "17": "Battery low",
-    "28": "Battery low restore",
-    "20": "Box tamper",
-    "31": "Box tamper restore",
-    "22": "Bus comms fail",
-    "33": "Bus comms restore",
-    "23": "Bus device battery low",
-    "34": "Bus device battery restore",
-    "21": "Bus device tamper",
-    "32": "Bus device tamper restore",
-    "14": "Comms fail",
-    "25": "Comm restore",
-    "53": "Crossed zone alarm",
-    "89": "Cross zone trigger",
-    "51": "Crystal oscillator clock",
-    "35": "Dedicated panic",
-    "2": "Disarm",
-    "54": "Disarm from stay",
-    "37": "Download access",
-    "66": "DTMF login",
-    "38": "Duress",
-    "18": "12V fuse fail",
-    "29": "12V fuse restore",
-    "19": "Engineer reset",
-    "30": "Engineer reset restore",
-    "88": "Entry delay",
-    "85": "Exit delay",
-    "67": "Failed IDSwift login",
-    "90": "Forced door",
-    "52": "Installer code changed",
-    "45": "Installer mode",
-    "40": "Keypad fire",
-    "42": "Keypad lockout",
-    "41": "Keypad medical",
-    "39": "Keypad panic",
-    "79": "MPS AC fail",
-    "82": "MPS AC restore",
-    "80": "MPS batt low",
-    "83": "MPS Batt restore",
-    "81": "MPS Fuse fail",
-    "84": "MPS Fuse restore",
-    "48": "Panel defaulted",
-    "26": "Phone line restore",
-    "15": "Phone line tamper",
-    "47": "Power up",
-    "92": "Remote arming request",
-    "93": "Remote panic",
-    "49": "Reserved",
-    "72": "RF Detector batt restore",
-    "68": "RF Detector low batt",
-    "69": "RF Detector supervision loss",
-    "73": "RF Detector supervision restore",
-    "70": "RF Jam",
-    "74": "RF Jam restore",
-    "71": "Rf RSSI low",
-    "75": "RF RSSI restore",
-    "27": "Siren restore",
-    "16": "Siren tamper",
-    "1": "Stay arm",
-    "77": "Stay zone report",
-    "230": "System trouble",
-    "231": "System trouble restore",
-    "91": "TAG arming request",
-    "94": "Tamper alarm",
-    "100": "User trigger",
-    "101": "User panic",
-    "36": "Test report",
-    "78": "Time stamp",
-    "65": "User bypassed zones",
-    "46": "User codes defaulted",
-    "44": "User code changed",
-    "76": "User menu accessed",
-    "87": "User unbypassed zones",
-    "86": "Voice login lockout",
-    "8": "Force armed",
-    "6": "Zone restore",
-    "11": "Zone shutdown",
-    "12": "Zone shutdown restore",
-    "9": "Zone tamper",
-    "10": "Zone tamper restore",
-    "5": "Zone violation alarm",
-}
+"""Hyyp API constants."""
+from enum import Enum
+
+DEFAULT_TIMEOUT = 25
+MAX_RETRIES = 3
+GCF_SENDER_ID = 87969245803
+REQUEST_HEADER = {
+    "User-Agent": "okhttp/3.12.1",
+}  # Standard android header.
+STD_PARAMS = {
+    "imei": "152419714130158",  # Alphabet soup starts at 0
+    "appVersionCode": "401",
+    "_appVersionCode": "401",
+    "deviceOS": "12.0",
+    "deviceName": "Python API",
+    "pkg": "za.co.adt.securehome.android",
+    "_appVersionName": "3.5.19",
+    "token": None,
+}  # Standard request parameters.
+
+# Rpc to name mapping. Used in push notifications.
+RpcCodes = {
+    "202": "IMEI unknown to SMART platform. Registration failed.",
+    "203": "Command failed",
+    "204": "VALUE is invalid",
+    "205": "User code invalid",
+    "206": "Unit busy",
+    "207": "Command was older than abort command time",
+    "208": "Communications timeout to peripheral attached to Hub",
+    "209": "Invalid PID in topic",
+    "210": "Serial code mismatch",
+}
+
+# EventCategory to name mapping.
+# Used in notifications.
+EventCategory = {"1": "Emergency", "2": "User", "3": "Trouble", "4": "Information"}
+
+
+class HyypPkg(Enum):
+    """Supported hyyp skins/rebranding."""
+
+    ADT_SECURE_HOME = "za.co.adt.securehome.android"
+    IDS_HYYP_GENERIC = "com.hyyp247.home"
+
+
+# EventNumber to name mapping.
+EventNumber = {
+    "50": "AC clock",
+    "13": "AC fail",
+    "24": "AC Restore",
+    "3": "Alarm cancel",
+    "7": "Armed with bypassed zone",
+    "43": "Auto arm cancel",
+    "0": "Away arm",
+    "17": "Battery low",
+    "28": "Battery low restore",
+    "20": "Box tamper",
+    "31": "Box tamper restore",
+    "22": "Bus comms fail",
+    "33": "Bus comms restore",
+    "23": "Bus device battery low",
+    "34": "Bus device battery restore",
+    "21": "Bus device tamper",
+    "32": "Bus device tamper restore",
+    "14": "Comms fail",
+    "25": "Comm restore",
+    "53": "Crossed zone alarm",
+    "89": "Cross zone trigger",
+    "51": "Crystal oscillator clock",
+    "35": "Dedicated panic",
+    "2": "Disarm",
+    "54": "Disarm from stay",
+    "37": "Download access",
+    "66": "DTMF login",
+    "38": "Duress",
+    "18": "12V fuse fail",
+    "29": "12V fuse restore",
+    "19": "Engineer reset",
+    "30": "Engineer reset restore",
+    "88": "Entry delay",
+    "85": "Exit delay",
+    "67": "Failed IDSwift login",
+    "90": "Forced door",
+    "52": "Installer code changed",
+    "45": "Installer mode",
+    "40": "Keypad fire",
+    "42": "Keypad lockout",
+    "41": "Keypad medical",
+    "39": "Keypad panic",
+    "79": "MPS AC fail",
+    "82": "MPS AC restore",
+    "80": "MPS batt low",
+    "83": "MPS Batt restore",
+    "81": "MPS Fuse fail",
+    "84": "MPS Fuse restore",
+    "48": "Panel defaulted",
+    "26": "Phone line restore",
+    "15": "Phone line tamper",
+    "47": "Power up",
+    "92": "Remote arming request",
+    "93": "Remote panic",
+    "49": "Reserved",
+    "72": "RF Detector batt restore",
+    "68": "RF Detector low batt",
+    "69": "RF Detector supervision loss",
+    "73": "RF Detector supervision restore",
+    "70": "RF Jam",
+    "74": "RF Jam restore",
+    "71": "Rf RSSI low",
+    "75": "RF RSSI restore",
+    "27": "Siren restore",
+    "16": "Siren tamper",
+    "1": "Stay arm",
+    "77": "Stay zone report",
+    "230": "System trouble",
+    "231": "System trouble restore",
+    "91": "TAG arming request",
+    "94": "Tamper alarm",
+    "100": "User trigger",
+    "101": "User panic",
+    "36": "Test report",
+    "78": "Time stamp",
+    "65": "User bypassed zones",
+    "46": "User codes defaulted",
+    "44": "User code changed",
+    "76": "User menu accessed",
+    "87": "User unbypassed zones",
+    "86": "Voice login lockout",
+    "8": "Force armed",
+    "6": "Zone restore",
+    "11": "Zone shutdown",
+    "12": "Zone shutdown restore",
+    "9": "Zone tamper",
+    "10": "Zone tamper restore",
+    "5": "Zone violation alarm",
+}
```

### Comparing `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/mcs_pb2.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: mcs.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tmcs.proto\x12\tmcs_proto\"S\n\rHeartbeatPing\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"R\n\x0cHeartbeatAck\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"a\n\tErrorInfo\x12\x0c\n\x04\x63ode\x18\x01 \x02(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\'\n\textension\x18\x04 \x01(\x0b\x32\x14.mcs_proto.Extension\"&\n\x07Setting\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"A\n\rHeartbeatStat\x12\n\n\x02ip\x18\x01 \x02(\t\x12\x0f\n\x07timeout\x18\x02 \x02(\x08\x12\x13\n\x0binterval_ms\x18\x03 \x02(\x05\"G\n\x0fHeartbeatConfig\x12\x13\n\x0bupload_stat\x18\x01 \x01(\x08\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x13\n\x0binterval_ms\x18\x03 \x01(\x05\"\xd3\x02\n\x0b\x43lientEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.mcs_proto.ClientEvent.Type\x12\x1f\n\x17number_discarded_events\x18\x64 \x01(\r\x12\x15\n\x0cnetwork_type\x18\xc8\x01 \x01(\x05\x12#\n\x1atime_connection_started_ms\x18\xca\x01 \x01(\x04\x12!\n\x18time_connection_ended_ms\x18\xcb\x01 \x01(\x04\x12\x13\n\nerror_code\x18\xcc\x01 \x01(\x05\x12\'\n\x1etime_connection_established_ms\x18\xac\x02 \x01(\x04\"[\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x14\n\x10\x44ISCARDED_EVENTS\x10\x01\x12\x15\n\x11\x46\x41ILED_CONNECTION\x10\x02\x12\x19\n\x15SUCCESSFUL_CONNECTION\x10\x03\"\xed\x03\n\x0cLoginRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06\x64omain\x18\x02 \x02(\t\x12\x0c\n\x04user\x18\x03 \x02(\t\x12\x10\n\x08resource\x18\x04 \x02(\t\x12\x12\n\nauth_token\x18\x05 \x02(\t\x12\x11\n\tdevice_id\x18\x06 \x01(\t\x12\x13\n\x0blast_rmq_id\x18\x07 \x01(\x03\x12#\n\x07setting\x18\x08 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x1e\n\x16received_persistent_id\x18\n \x03(\t\x12\x1a\n\x12\x61\x64\x61ptive_heartbeat\x18\x0c \x01(\x08\x12\x30\n\x0eheartbeat_stat\x18\r \x01(\x0b\x32\x18.mcs_proto.HeartbeatStat\x12\x10\n\x08use_rmq2\x18\x0e \x01(\x08\x12\x12\n\naccount_id\x18\x0f \x01(\x03\x12\x39\n\x0c\x61uth_service\x18\x10 \x01(\x0e\x32#.mcs_proto.LoginRequest.AuthService\x12\x14\n\x0cnetwork_type\x18\x11 \x01(\x05\x12\x0e\n\x06status\x18\x12 \x01(\x03\x12,\n\x0c\x63lient_event\x18\x16 \x03(\x0b\x32\x16.mcs_proto.ClientEvent\"\x1d\n\x0b\x41uthService\x12\x0e\n\nANDROID_ID\x10\x02\"\xf6\x01\n\rLoginResponse\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0b\n\x03jid\x18\x02 \x01(\t\x12#\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12#\n\x07setting\x18\x04 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x11\n\tstream_id\x18\x05 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x06 \x01(\x05\x12\x34\n\x10heartbeat_config\x18\x07 \x01(\x0b\x32\x1a.mcs_proto.HeartbeatConfig\x12\x18\n\x10server_timestamp\x18\x08 \x01(\x03\"/\n\x11StreamErrorStanza\x12\x0c\n\x04type\x18\x01 \x02(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"\x07\n\x05\x43lose\"%\n\tExtension\x12\n\n\x02id\x18\x01 \x02(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x02(\x0c\"\xdd\x02\n\x08IqStanza\x12\x0e\n\x06rmq_id\x18\x01 \x01(\x03\x12(\n\x04type\x18\x02 \x02(\x0e\x32\x1a.mcs_proto.IqStanza.IqType\x12\n\n\x02id\x18\x03 \x02(\t\x12\x0c\n\x04\x66rom\x18\x04 \x01(\t\x12\n\n\x02to\x18\x05 \x01(\t\x12#\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12\'\n\textension\x18\x07 \x01(\x0b\x32\x14.mcs_proto.Extension\x12\x15\n\rpersistent_id\x18\x08 \x01(\t\x12\x11\n\tstream_id\x18\t \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\n \x01(\x05\x12\x12\n\naccount_id\x18\x0b \x01(\x03\x12\x0e\n\x06status\x18\x0c \x01(\x03\"4\n\x06IqType\x12\x07\n\x03GET\x10\x00\x12\x07\n\x03SET\x10\x01\x12\n\n\x06RESULT\x10\x02\x12\x0c\n\x08IQ_ERROR\x10\x03\"%\n\x07\x41ppData\x12\x0b\n\x03key\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"\xf4\x02\n\x11\x44\x61taMessageStanza\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04\x66rom\x18\x03 \x02(\t\x12\n\n\x02to\x18\x04 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x05 \x02(\t\x12\r\n\x05token\x18\x06 \x01(\t\x12$\n\x08\x61pp_data\x18\x07 \x03(\x0b\x32\x12.mcs_proto.AppData\x12\x1b\n\x13\x66rom_trusted_server\x18\x08 \x01(\x08\x12\x15\n\rpersistent_id\x18\t \x01(\t\x12\x11\n\tstream_id\x18\n \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x0b \x01(\x05\x12\x0e\n\x06reg_id\x18\r \x01(\t\x12\x16\n\x0e\x64\x65vice_user_id\x18\x10 \x01(\x03\x12\x0b\n\x03ttl\x18\x11 \x01(\x05\x12\x0c\n\x04sent\x18\x12 \x01(\x03\x12\x0e\n\x06queued\x18\x13 \x01(\x05\x12\x0e\n\x06status\x18\x14 \x01(\x03\x12\x10\n\x08raw_data\x18\x15 \x01(\x0c\x12\x15\n\rimmediate_ack\x18\x18 \x01(\x08\"\x0b\n\tStreamAck\"\x1a\n\x0cSelectiveAck\x12\n\n\x02id\x18\x01 \x03(\tB\x02H\x03')
-
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mcs_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_HEARTBEATPING']._serialized_start=24
-  _globals['_HEARTBEATPING']._serialized_end=107
-  _globals['_HEARTBEATACK']._serialized_start=109
-  _globals['_HEARTBEATACK']._serialized_end=191
-  _globals['_ERRORINFO']._serialized_start=193
-  _globals['_ERRORINFO']._serialized_end=290
-  _globals['_SETTING']._serialized_start=292
-  _globals['_SETTING']._serialized_end=330
-  _globals['_HEARTBEATSTAT']._serialized_start=332
-  _globals['_HEARTBEATSTAT']._serialized_end=397
-  _globals['_HEARTBEATCONFIG']._serialized_start=399
-  _globals['_HEARTBEATCONFIG']._serialized_end=470
-  _globals['_CLIENTEVENT']._serialized_start=473
-  _globals['_CLIENTEVENT']._serialized_end=812
-  _globals['_CLIENTEVENT_TYPE']._serialized_start=721
-  _globals['_CLIENTEVENT_TYPE']._serialized_end=812
-  _globals['_LOGINREQUEST']._serialized_start=815
-  _globals['_LOGINREQUEST']._serialized_end=1308
-  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_start=1279
-  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_end=1308
-  _globals['_LOGINRESPONSE']._serialized_start=1311
-  _globals['_LOGINRESPONSE']._serialized_end=1557
-  _globals['_STREAMERRORSTANZA']._serialized_start=1559
-  _globals['_STREAMERRORSTANZA']._serialized_end=1606
-  _globals['_CLOSE']._serialized_start=1608
-  _globals['_CLOSE']._serialized_end=1615
-  _globals['_EXTENSION']._serialized_start=1617
-  _globals['_EXTENSION']._serialized_end=1654
-  _globals['_IQSTANZA']._serialized_start=1657
-  _globals['_IQSTANZA']._serialized_end=2006
-  _globals['_IQSTANZA_IQTYPE']._serialized_start=1954
-  _globals['_IQSTANZA_IQTYPE']._serialized_end=2006
-  _globals['_APPDATA']._serialized_start=2008
-  _globals['_APPDATA']._serialized_end=2045
-  _globals['_DATAMESSAGESTANZA']._serialized_start=2048
-  _globals['_DATAMESSAGESTANZA']._serialized_end=2420
-  _globals['_STREAMACK']._serialized_start=2422
-  _globals['_STREAMACK']._serialized_end=2433
-  _globals['_SELECTIVEACK']._serialized_start=2435
-  _globals['_SELECTIVEACK']._serialized_end=2461
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: mcs.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tmcs.proto\x12\tmcs_proto\"S\n\rHeartbeatPing\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"R\n\x0cHeartbeatAck\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"a\n\tErrorInfo\x12\x0c\n\x04\x63ode\x18\x01 \x02(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\'\n\textension\x18\x04 \x01(\x0b\x32\x14.mcs_proto.Extension\"&\n\x07Setting\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"A\n\rHeartbeatStat\x12\n\n\x02ip\x18\x01 \x02(\t\x12\x0f\n\x07timeout\x18\x02 \x02(\x08\x12\x13\n\x0binterval_ms\x18\x03 \x02(\x05\"G\n\x0fHeartbeatConfig\x12\x13\n\x0bupload_stat\x18\x01 \x01(\x08\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x13\n\x0binterval_ms\x18\x03 \x01(\x05\"\xd3\x02\n\x0b\x43lientEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.mcs_proto.ClientEvent.Type\x12\x1f\n\x17number_discarded_events\x18\x64 \x01(\r\x12\x15\n\x0cnetwork_type\x18\xc8\x01 \x01(\x05\x12#\n\x1atime_connection_started_ms\x18\xca\x01 \x01(\x04\x12!\n\x18time_connection_ended_ms\x18\xcb\x01 \x01(\x04\x12\x13\n\nerror_code\x18\xcc\x01 \x01(\x05\x12\'\n\x1etime_connection_established_ms\x18\xac\x02 \x01(\x04\"[\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x14\n\x10\x44ISCARDED_EVENTS\x10\x01\x12\x15\n\x11\x46\x41ILED_CONNECTION\x10\x02\x12\x19\n\x15SUCCESSFUL_CONNECTION\x10\x03\"\xed\x03\n\x0cLoginRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06\x64omain\x18\x02 \x02(\t\x12\x0c\n\x04user\x18\x03 \x02(\t\x12\x10\n\x08resource\x18\x04 \x02(\t\x12\x12\n\nauth_token\x18\x05 \x02(\t\x12\x11\n\tdevice_id\x18\x06 \x01(\t\x12\x13\n\x0blast_rmq_id\x18\x07 \x01(\x03\x12#\n\x07setting\x18\x08 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x1e\n\x16received_persistent_id\x18\n \x03(\t\x12\x1a\n\x12\x61\x64\x61ptive_heartbeat\x18\x0c \x01(\x08\x12\x30\n\x0eheartbeat_stat\x18\r \x01(\x0b\x32\x18.mcs_proto.HeartbeatStat\x12\x10\n\x08use_rmq2\x18\x0e \x01(\x08\x12\x12\n\naccount_id\x18\x0f \x01(\x03\x12\x39\n\x0c\x61uth_service\x18\x10 \x01(\x0e\x32#.mcs_proto.LoginRequest.AuthService\x12\x14\n\x0cnetwork_type\x18\x11 \x01(\x05\x12\x0e\n\x06status\x18\x12 \x01(\x03\x12,\n\x0c\x63lient_event\x18\x16 \x03(\x0b\x32\x16.mcs_proto.ClientEvent\"\x1d\n\x0b\x41uthService\x12\x0e\n\nANDROID_ID\x10\x02\"\xf6\x01\n\rLoginResponse\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0b\n\x03jid\x18\x02 \x01(\t\x12#\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12#\n\x07setting\x18\x04 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x11\n\tstream_id\x18\x05 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x06 \x01(\x05\x12\x34\n\x10heartbeat_config\x18\x07 \x01(\x0b\x32\x1a.mcs_proto.HeartbeatConfig\x12\x18\n\x10server_timestamp\x18\x08 \x01(\x03\"/\n\x11StreamErrorStanza\x12\x0c\n\x04type\x18\x01 \x02(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"\x07\n\x05\x43lose\"%\n\tExtension\x12\n\n\x02id\x18\x01 \x02(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x02(\x0c\"\xdd\x02\n\x08IqStanza\x12\x0e\n\x06rmq_id\x18\x01 \x01(\x03\x12(\n\x04type\x18\x02 \x02(\x0e\x32\x1a.mcs_proto.IqStanza.IqType\x12\n\n\x02id\x18\x03 \x02(\t\x12\x0c\n\x04\x66rom\x18\x04 \x01(\t\x12\n\n\x02to\x18\x05 \x01(\t\x12#\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12\'\n\textension\x18\x07 \x01(\x0b\x32\x14.mcs_proto.Extension\x12\x15\n\rpersistent_id\x18\x08 \x01(\t\x12\x11\n\tstream_id\x18\t \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\n \x01(\x05\x12\x12\n\naccount_id\x18\x0b \x01(\x03\x12\x0e\n\x06status\x18\x0c \x01(\x03\"4\n\x06IqType\x12\x07\n\x03GET\x10\x00\x12\x07\n\x03SET\x10\x01\x12\n\n\x06RESULT\x10\x02\x12\x0c\n\x08IQ_ERROR\x10\x03\"%\n\x07\x41ppData\x12\x0b\n\x03key\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"\xf4\x02\n\x11\x44\x61taMessageStanza\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04\x66rom\x18\x03 \x02(\t\x12\n\n\x02to\x18\x04 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x05 \x02(\t\x12\r\n\x05token\x18\x06 \x01(\t\x12$\n\x08\x61pp_data\x18\x07 \x03(\x0b\x32\x12.mcs_proto.AppData\x12\x1b\n\x13\x66rom_trusted_server\x18\x08 \x01(\x08\x12\x15\n\rpersistent_id\x18\t \x01(\t\x12\x11\n\tstream_id\x18\n \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x0b \x01(\x05\x12\x0e\n\x06reg_id\x18\r \x01(\t\x12\x16\n\x0e\x64\x65vice_user_id\x18\x10 \x01(\x03\x12\x0b\n\x03ttl\x18\x11 \x01(\x05\x12\x0c\n\x04sent\x18\x12 \x01(\x03\x12\x0e\n\x06queued\x18\x13 \x01(\x05\x12\x0e\n\x06status\x18\x14 \x01(\x03\x12\x10\n\x08raw_data\x18\x15 \x01(\x0c\x12\x15\n\rimmediate_ack\x18\x18 \x01(\x08\"\x0b\n\tStreamAck\"\x1a\n\x0cSelectiveAck\x12\n\n\x02id\x18\x01 \x03(\tB\x02H\x03')
+
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mcs_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'H\003'
+  _globals['_HEARTBEATPING']._serialized_start=24
+  _globals['_HEARTBEATPING']._serialized_end=107
+  _globals['_HEARTBEATACK']._serialized_start=109
+  _globals['_HEARTBEATACK']._serialized_end=191
+  _globals['_ERRORINFO']._serialized_start=193
+  _globals['_ERRORINFO']._serialized_end=290
+  _globals['_SETTING']._serialized_start=292
+  _globals['_SETTING']._serialized_end=330
+  _globals['_HEARTBEATSTAT']._serialized_start=332
+  _globals['_HEARTBEATSTAT']._serialized_end=397
+  _globals['_HEARTBEATCONFIG']._serialized_start=399
+  _globals['_HEARTBEATCONFIG']._serialized_end=470
+  _globals['_CLIENTEVENT']._serialized_start=473
+  _globals['_CLIENTEVENT']._serialized_end=812
+  _globals['_CLIENTEVENT_TYPE']._serialized_start=721
+  _globals['_CLIENTEVENT_TYPE']._serialized_end=812
+  _globals['_LOGINREQUEST']._serialized_start=815
+  _globals['_LOGINREQUEST']._serialized_end=1308
+  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_start=1279
+  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_end=1308
+  _globals['_LOGINRESPONSE']._serialized_start=1311
+  _globals['_LOGINRESPONSE']._serialized_end=1557
+  _globals['_STREAMERRORSTANZA']._serialized_start=1559
+  _globals['_STREAMERRORSTANZA']._serialized_end=1606
+  _globals['_CLOSE']._serialized_start=1608
+  _globals['_CLOSE']._serialized_end=1615
+  _globals['_EXTENSION']._serialized_start=1617
+  _globals['_EXTENSION']._serialized_end=1654
+  _globals['_IQSTANZA']._serialized_start=1657
+  _globals['_IQSTANZA']._serialized_end=2006
+  _globals['_IQSTANZA_IQTYPE']._serialized_start=1954
+  _globals['_IQSTANZA_IQTYPE']._serialized_end=2006
+  _globals['_APPDATA']._serialized_start=2008
+  _globals['_APPDATA']._serialized_end=2045
+  _globals['_DATAMESSAGESTANZA']._serialized_start=2048
+  _globals['_DATAMESSAGESTANZA']._serialized_end=2420
+  _globals['_STREAMACK']._serialized_start=2422
+  _globals['_STREAMACK']._serialized_end=2433
+  _globals['_SELECTIVEACK']._serialized_start=2435
+  _globals['_SELECTIVEACK']._serialized_end=2461
+# @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

