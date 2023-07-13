# Comparing `tmp/mrob-0.0.7-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.whl.zip` & `tmp/mrob-0.0.8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,17 @@
-Zip file size: 1312249 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1129 b- defN 21-Jun-30 13:41 mrob/__init__.py
--rwxr-xr-x  2.0 unx   568512 b- defN 21-Jun-30 13:45 mrob/libFGraph.so
--rwxr-xr-x  2.0 unx   395168 b- defN 21-Jun-30 13:45 mrob/libPCRegistration.so
--rwxr-xr-x  2.0 unx    70624 b- defN 21-Jun-30 13:41 mrob/libSE3.so
--rwxr-xr-x  2.0 unx    77968 b- defN 21-Jun-30 13:41 mrob/libcommon.so
--rwxr-xr-x  2.0 unx   380776 b- defN 21-Jun-30 13:45 mrob/mrob.cpython-310-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   413496 b- defN 21-Jun-30 13:45 mrob/mrob.cpython-36m-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   413528 b- defN 21-Jun-30 13:45 mrob/mrob.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   380776 b- defN 21-Jun-30 13:45 mrob/mrob.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   380776 b- defN 21-Jun-30 13:45 mrob/mrob.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     9239 b- defN 21-Jun-30 13:45 mrob-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2784 b- defN 21-Jun-30 13:45 mrob-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx      168 b- defN 21-Jun-30 13:45 mrob-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 21-Jun-30 13:45 mrob-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1532 b- defN 21-Jun-30 13:45 mrob-0.0.7.dist-info/RECORD
--rwxr-xr-x  2.0 unx    85936 b- defN 21-Jun-30 13:45 mrob.libs/libcommon-8cf4fd1c.so
--rwxr-xr-x  2.0 unx    79456 b- defN 21-Jun-30 13:45 mrob.libs/libSE3-f4499c09.so
--rwxr-xr-x  2.0 unx   613008 b- defN 21-Jun-30 13:45 mrob.libs/libFGraph-3fd5da2c.so
-18 files, 3874881 bytes uncompressed, 1309807 bytes compressed:  66.2%
+Zip file size: 1021528 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat   292864 b- defN 22-Feb-11 12:39 mrob/FGraph.dll
+-rw-rw-rw-  2.0 fat   435712 b- defN 22-Feb-11 12:40 mrob/PCRegistration.dll
+-rw-rw-rw-  2.0 fat   116224 b- defN 22-Feb-11 12:38 mrob/SE3.dll
+-rw-rw-rw-  2.0 fat     1680 b- defN 22-Feb-11 12:37 mrob/__init__.py
+-rw-rw-rw-  2.0 fat   105472 b- defN 22-Feb-11 12:38 mrob/common.dll
+-rw-rw-rw-  2.0 fat   389120 b- defN 22-Feb-11 12:41 mrob/mrob.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   396288 b- defN 22-Feb-11 12:42 mrob/mrob.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   396288 b- defN 22-Feb-11 12:43 mrob/mrob.cp37-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   389120 b- defN 22-Feb-11 12:44 mrob/mrob.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   346112 b- defN 22-Feb-11 12:45 mrob/mrob.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     9310 b- defN 22-Feb-11 12:45 mrob-0.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3822 b- defN 22-Feb-11 12:45 mrob-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 22-Feb-11 12:45 mrob-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 22-Feb-11 12:45 mrob-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1180 b- defN 22-Feb-11 12:45 mrob-0.0.8.dist-info/RECORD
+15 files, 2883295 bytes uncompressed, 1019634 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,55 +1,46 @@
-Filename: mrob/__init__.py
-Comment: 
-
-Filename: mrob/libFGraph.so
-Comment: 
-
-Filename: mrob/libPCRegistration.so
-Comment: 
-
-Filename: mrob/libSE3.so
+Filename: mrob/FGraph.dll
 Comment: 
 
-Filename: mrob/libcommon.so
+Filename: mrob/PCRegistration.dll
 Comment: 
 
-Filename: mrob/mrob.cpython-310-x86_64-linux-gnu.so
+Filename: mrob/SE3.dll
 Comment: 
 
-Filename: mrob/mrob.cpython-36m-x86_64-linux-gnu.so
+Filename: mrob/__init__.py
 Comment: 
 
-Filename: mrob/mrob.cpython-37m-x86_64-linux-gnu.so
+Filename: mrob/common.dll
 Comment: 
 
-Filename: mrob/mrob.cpython-38-x86_64-linux-gnu.so
+Filename: mrob/mrob.cp310-win_amd64.pyd
 Comment: 
 
-Filename: mrob/mrob.cpython-39-x86_64-linux-gnu.so
+Filename: mrob/mrob.cp36-win_amd64.pyd
 Comment: 
 
-Filename: mrob-0.0.7.dist-info/LICENSE
+Filename: mrob/mrob.cp37-win_amd64.pyd
 Comment: 
 
-Filename: mrob-0.0.7.dist-info/METADATA
+Filename: mrob/mrob.cp38-win_amd64.pyd
 Comment: 
 
-Filename: mrob-0.0.7.dist-info/WHEEL
+Filename: mrob/mrob.cp39-win_amd64.pyd
 Comment: 
 
-Filename: mrob-0.0.7.dist-info/top_level.txt
+Filename: mrob-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: mrob-0.0.7.dist-info/RECORD
+Filename: mrob-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: mrob.libs/libcommon-8cf4fd1c.so
+Filename: mrob-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: mrob.libs/libSE3-f4499c09.so
+Filename: mrob-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mrob.libs/libFGraph-3fd5da2c.so
+Filename: mrob-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mrob/__init__.py

```diff
@@ -1,36 +1,49 @@
-# Copyright (c) 2018, Skolkovo Institute of Science and Technology (Skoltech)
-# 
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-# 
-# 
-#  __init__.py
-# 
-#  Created on: Nov 11, 2020
-#       Author: Lyubov Miloserdova
-#               miloslubov@gmail.com
-#
-
-from mrob import mrob
-
-FGraph = mrob.FGraph
-GN = mrob.GN
-LEVENBERG_MARQUARDT_ELLIP = mrob.LEVENBERG_MARQUARDT_ELLIP
-LEVENBERG_MARQUARDT_SPHER = mrob.LEVENBERG_MARQUARDT_SPHER 
-LM = mrob.LM
-NEWTON_RAPHSON = mrob.NEWTON_RAPHSON
-geometry = mrob.geometry
-optimMethod = mrob.optimMethod 
-ostream_redirect = mrob.ostream_redirect
-registration = mrob.registration
-
-del(mrob)
+# Copyright (c) 2018, Skolkovo Institute of Science and Technology (Skoltech)
+# 
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# 
+# 
+#  __init__.py
+# 
+#  Created on: Nov 11, 2020
+#       Author: Lyubov Miloserdova
+#               miloslubov@gmail.com
+#
+
+try:
+    from . import mrob
+
+    from pkg_resources import get_distribution
+
+    __version__ = get_distribution('mrob').version
+
+    for module in dir(mrob):
+        n = len(module) - 1
+        if not (module[:2] == '__' and module[n:n-2:-1] == '__') and module.count('.') == 0:
+            globals()[module] = getattr(mrob, module)
+
+    del mrob
+except ImportError:
+    import platform
+    
+    if platform.system() == "Windows":
+        import sys
+        
+        sys.tracebacklimit = 0
+        raise ImportError(
+            "Maybe you don't have Microsoft Visual C++ Redistributable package installed. " + 
+            "Please follow the link and install redistributable " +
+            "package: https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-160" +
+            "#visual-studio-2015-2017-2019-and-2022") from None
+    
+    raise
```

## Comparing `mrob-0.0.7.dist-info/LICENSE` & `mrob-0.0.8.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-Apache License
-Version 2.0, January 2004
-http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-2. Grant of Copyright License.
-
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License.
-
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-4. Redistribution.
-
-You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-    You must give any other recipients of the Work or Derivative Works a copy of this License; and
-    You must cause any modified files to carry prominent notices stating that You changed the files; and
-    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-5. Submission of Contributions.
-
-Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-6. Trademarks.
-
-This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty.
-
-Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability.
-
-In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability.
-
-While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
-
-END OF TERMS AND CONDITIONS
-
-
-Copyright (c) 2018, Skolkovo Institute of Science and Technology (Skoltech)
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+
+"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+
+"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+
+"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+
+"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+
+"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+
+"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+
+2. Grant of Copyright License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+
+4. Redistribution.
+
+You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+
+    You must give any other recipients of the Work or Derivative Works a copy of this License; and
+    You must cause any modified files to carry prominent notices stating that You changed the files; and
+    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+
+You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+
+5. Submission of Contributions.
+
+Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+
+6. Trademarks.
+
+This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty.
+
+Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability.
+
+In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability.
+
+While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
+
+
+Copyright (c) 2018, Skolkovo Institute of Science and Technology (Skoltech)
```

## Comparing `mrob-0.0.7.dist-info/METADATA` & `mrob-0.0.8.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: mrob
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
+Summary: The Skoltech Mobile Robotics library (mrob) is a framework for implementing robotics research and projects.
 Home-page: https://github.com/MobileRoboticsSkoltech/mrob
+Download-URL: https://github.com/MobileRoboticsSkoltech/mrob
+Author: Gonzalo Ferrer
+Author-email: G.Ferrer@skoltech.ru
 Maintainer: Gonzalo Ferrer
 Maintainer-email: G.Ferrer@skoltech.ru
 License: Apache-2.0
-Platform: UNKNOWN
+Platform: any
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPi version](https://img.shields.io/pypi/v/mrob.svg)](https://pypi.org/project/mrob/)
 [![PyPi downloads](https://img.shields.io/pypi/dm/mrob.svg)](https://pypi.org/project/mrob/)
+[![Documentation Status](https://readthedocs.org/projects/mrob/badge/?version=latest)](https://mrob.readthedocs.io/en/latest/?badge=latest)
 
 <p align="center">
   <img src="https://sites.skoltech.ru/app/data/uploads/sites/50/2018/02/mr_animate1.gif" width="450">
 </p>
 
 # MROB: Mobile Robotics library
 The Skoltech Mobile Robotics library (mrob) is our common framework for implementing our robotics research and projects. It includes a core set of functionalities such as geometric transformations (SE3), factor graphs for general state estimation, optimization, 3D point cloud registration and more to come.
@@ -37,14 +41,15 @@
 The present library is meant to be a self-contained library. However, there are few dependencies:
 * C++'14
 * CMake
 * [Eigen](https://gitlab.com/libeigen/eigen) (included as a submodule)
 * [pybind11](https://github.com/pybind/pybind11) (included as a submodule)
   - python3-distutils
   - python3-dev
+* [Catch2 v2.x branch](https://github.com/catchorg/Catch2/tree/v2.x) (included as a submodule)
 
 This is the list of required packages to install:
 `sudo apt install build-essential cmake python3-distutils python3-dev`
 
 
 ## Repository 
 Standard github cloning, adding the recursive term for submodules.
@@ -60,14 +65,23 @@
 cd mrob
 mkdir build
 cd build
 cmake ..
 make -j
 ```
 
+If you need to use this library in Python code, you can install it using pip:
+`pip install mrob`
+
+**Note:** If your OS is Windows and you don't have Microsoft Visual C++ Redistributable package installed, 
+then you need to [install it](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-160#visual-studio-2015-2017-2019-and-2022) additionally.
+If you are using a 32-bit Python, then install the package for the X86 architecture. 
+If you are using 64-bit Python, then install the package for the X64 architecture. 
+Don't be afraid to install both packages.
+
 
 ## License
 Apache-2.0 License
```

