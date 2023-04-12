# Comparing `tmp/opencmiss.maths-0.2.0.tar.gz` & `tmp/opencmiss.maths-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.maths-0.2.0.tar", last modified: Thu Feb 23 19:02:24 2023, max compression
+gzip compressed data, was "opencmiss.maths-0.2.1.tar", last modified: Wed Apr 12 03:40:41 2023, max compression
```

## Comparing `opencmiss.maths-0.2.0.tar` & `opencmiss.maths-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-23 19:02:24.672385 opencmiss.maths-0.2.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2021-06-16 00:43:01.000000 opencmiss.maths-0.2.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12091 2023-02-23 19:02:24.672020 opencmiss.maths-0.2.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      384 2021-09-08 08:57:39.000000 opencmiss.maths-0.2.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-02-23 19:02:24.672471 opencmiss.maths-0.2.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1401 2021-09-08 08:57:39.000000 opencmiss.maths-0.2.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-23 19:02:24.666979 opencmiss.maths-0.2.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-23 19:02:24.668273 opencmiss.maths-0.2.0/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      123 2021-09-08 08:54:15.000000 opencmiss.maths-0.2.0/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-23 19:02:24.671608 opencmiss.maths-0.2.0/src/opencmiss/maths/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2023-02-23 19:01:49.000000 opencmiss.maths-0.2.0/src/opencmiss/maths/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1521 2022-07-25 06:37:47.000000 opencmiss.maths-0.2.0/src/opencmiss/maths/algorithms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7726 2023-02-23 18:59:53.000000 opencmiss.maths-0.2.0/src/opencmiss/maths/vectorops.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-23 19:02:24.670445 opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12091 2023-02-23 19:02:24.000000 opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      366 2023-02-23 19:02:24.000000 opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-02-23 19:02:24.000000 opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-09-08 08:59:27.000000 opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2023-02-23 19:02:24.000000 opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-12 03:40:41.801276 opencmiss.maths-0.2.1/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2023-04-12 03:30:32.000000 opencmiss.maths-0.2.1/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    13643 2023-04-12 03:40:41.800976 opencmiss.maths-0.2.1/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      180 2023-04-12 03:39:50.000000 opencmiss.maths-0.2.1/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-12 03:40:41.800572 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    13643 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      221 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-12 03:40:41.801365 opencmiss.maths-0.2.1/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1054 2023-04-12 03:37:32.000000 opencmiss.maths-0.2.1/setup.py
```

### Comparing `opencmiss.maths-0.2.0/LICENSE` & `opencmiss.maths-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencmiss.maths-0.2.0/PKG-INFO` & `opencmiss.maths-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,235 +1,227 @@
 Metadata-Version: 2.1
 Name: opencmiss.maths
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenCMISS Math functions.
 Home-page: https://github.com/OpenCMISS-Bindings/opencmiss.maths
 Author: Hugh Sorby
 Author-email: h.sorby@auckland.ac.nz
 License: Apache Software License
+Description: 
+        ===============
+        OpenCMISS Maths
+        ===============
+        
+        This package has been renamed. Use :code:`pip install cmlibs.maths` instead.
+        New package: https://pypi.org/project/cmlibs.maths/
+        
+        
+        License
+        =======
+        
+        ::
+        
+                                         Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
 Platform: UNKNOWN
+Classifier: Development Status :: 7 - Inactive
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-
-===============
-OpenCMISS Maths
-===============
-
-OpenCMISS maths functions.  This software can be found on PyPi and installed with the following command::
-
-  pip install opencmiss.maths
-
-Distribution
-============
-
-This software uses regex to extract the version number information from the package. The version number for this package is stored in 'src/opencmiss/maths/__init__.py'
-
-
-License
-=======
-
-::
-
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
-
-
```

### Comparing `opencmiss.maths-0.2.0/setup.py` & `opencmiss.maths-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,14 @@
 import os
 import re
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(here, 'src', 'opencmiss', 'maths', '__init__.py')) as fd:
-    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        fd.read(), re.MULTILINE).group(1)
-
-if not version:
-    raise RuntimeError('Cannot find version information')
-
 
 def readfile(filename, split=False):
     with io.open(filename, encoding="utf-8") as stream:
         if split:
             return stream.read().split("\n")
         return stream.read()
 
@@ -27,27 +20,23 @@
 readme.append('')
 readme.append('::')
 readme.append('')
 readme.append('')
 
 software_licence = readfile("LICENSE")
 
-requires = []
+requires = ["cmlibs.maths"]
 
 setup(
     name='opencmiss.maths',
-    version=version,
+    version="0.2.1",
     description='OpenCMISS Math functions.',
     long_description='\n'.join(readme) + software_licence,
     long_description_content_type='text/x-rst',
-    classifiers=[],
+    classifiers=["Development Status :: 7 - Inactive"],
     author='Hugh Sorby',
     author_email='h.sorby@auckland.ac.nz',
     url='https://github.com/OpenCMISS-Bindings/opencmiss.maths',
     license='Apache Software License',
     license_files=("LICENSE",),
-    packages=find_packages("src"),
-    package_dir={"": "src"},
-    include_package_data=True,
-    zip_safe=False,
     install_requires=requires,
 )
```

### Comparing `opencmiss.maths-0.2.0/src/opencmiss.maths.egg-info/PKG-INFO` & `opencmiss.maths-0.2.1/opencmiss.maths.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,235 +1,227 @@
 Metadata-Version: 2.1
 Name: opencmiss.maths
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenCMISS Math functions.
 Home-page: https://github.com/OpenCMISS-Bindings/opencmiss.maths
 Author: Hugh Sorby
 Author-email: h.sorby@auckland.ac.nz
 License: Apache Software License
+Description: 
+        ===============
+        OpenCMISS Maths
+        ===============
+        
+        This package has been renamed. Use :code:`pip install cmlibs.maths` instead.
+        New package: https://pypi.org/project/cmlibs.maths/
+        
+        
+        License
+        =======
+        
+        ::
+        
+                                         Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
 Platform: UNKNOWN
+Classifier: Development Status :: 7 - Inactive
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-
-===============
-OpenCMISS Maths
-===============
-
-OpenCMISS maths functions.  This software can be found on PyPi and installed with the following command::
-
-  pip install opencmiss.maths
-
-Distribution
-============
-
-This software uses regex to extract the version number information from the package. The version number for this package is stored in 'src/opencmiss/maths/__init__.py'
-
-
-License
-=======
-
-::
-
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
-
-
```

