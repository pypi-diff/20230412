# Comparing `tmp/vysion-1.0.3.tar.gz` & `tmp/vysion-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vysion-1.0.3.tar", max compression
+gzip compressed data, was "vysion-1.0.4.tar", max compression
```

## Comparing `vysion-1.0.3.tar` & `vysion-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rwxr-xr-x   0        0        0    11556 2022-06-15 15:19:09.136069 vysion-1.0.3/LICENSE
--rwxr-xr-x   0        0        0     2038 2022-09-27 10:20:26.005811 vysion-1.0.3/README.md
--rwxr-xr-x   0        0        0     1017 2023-01-17 17:58:04.907665 vysion-1.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      727 2023-01-11 19:58:04.643273 vysion-1.0.3/vysion/__init__.py
--rwxr-xr-x   0        0        0      649 2022-09-27 10:20:26.024418 vysion-1.0.3/vysion/client/__init__.py
--rwxr-xr-x   0        0        0    10714 2023-01-11 19:58:04.644935 vysion-1.0.3/vysion/client/client.py
--rwxr-xr-x   0        0        0     1212 2023-01-11 19:58:04.644935 vysion-1.0.3/vysion/client/error.py
--rwxr-xr-x   0        0        0      622 2023-01-11 19:58:04.652890 vysion-1.0.3/vysion/dto/__init__.py
--rwxr-xr-x   0        0        0     7078 2023-01-17 17:53:28.314477 vysion-1.0.3/vysion/dto/dto.py
--rwxr-xr-x   0        0        0     1499 2023-01-11 19:58:04.654984 vysion-1.0.3/vysion/dto/tag.py
--rwxr-xr-x   0        0        0     4288 2023-01-11 19:58:04.663765 vysion-1.0.3/vysion/dto/util.py
--rwxr-xr-x   0        0        0      645 2023-01-11 19:58:04.669788 vysion-1.0.3/vysion/model/__init__.py
--rwxr-xr-x   0        0        0      711 2023-01-11 19:58:04.672098 vysion-1.0.3/vysion/model/enum/__init__.py
--rwxr-xr-x   0        0        0     4393 2023-01-11 19:58:04.677447 vysion-1.0.3/vysion/model/enum/languages.py
--rwxr-xr-x   0        0        0      818 2023-01-11 19:58:04.686390 vysion-1.0.3/vysion/model/enum/networks.py
--rwxr-xr-x   0        0        0     1583 2023-01-11 19:58:04.689914 vysion-1.0.3/vysion/model/enum/ransom_groups.py
--rwxr-xr-x   0        0        0     5860 2023-01-11 19:58:04.702109 vysion-1.0.3/vysion/model/enum/services.py
--rwxr-xr-x   0        0        0     5150 2023-01-11 19:58:04.702109 vysion-1.0.3/vysion/model/model.py
--rwxr-xr-x   0        0        0      654 2022-09-27 10:20:26.032519 vysion-1.0.3/vysion/taxonomy/__init__.py
--rwxr-xr-x   0        0        0     2442 2022-09-27 10:20:26.033516 vysion-1.0.3/vysion/taxonomy/flavours.py
--rwxr-xr-x   0        0        0    12788 2022-09-27 10:20:26.034514 vysion-1.0.3/vysion/taxonomy/taxonomy.py
--rwxr-xr-x   0        0        0      628 2023-01-11 19:58:04.702109 vysion-1.0.3/vysion/version.py
--rw-r--r--   0        0        0     2858 2023-01-17 18:00:34.777796 vysion-1.0.3/setup.py
--rw-r--r--   0        0        0     2912 2023-01-17 18:00:34.778150 vysion-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-12 11:01:34.010455 vysion-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1976 2023-04-12 11:01:34.010455 vysion-1.0.4/README.md
+-rw-r--r--   0        0        0      977 2023-04-12 11:34:08.041449 vysion-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/client/__init__.py
+-rw-r--r--   0        0        0    10354 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/client/client.py
+-rw-r--r--   0        0        0     1176 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/client/error.py
+-rw-r--r--   0        0        0      605 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/__init__.py
+-rw-r--r--   0        0        0     6809 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/dto.py
+-rw-r--r--   0        0        0     1441 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/tag.py
+-rw-r--r--   0        0        0     4169 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/dto/util.py
+-rw-r--r--   0        0        0      627 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-12 11:11:50.831436 vysion-1.0.4/vysion/model/enum/languages.py
+-rw-r--r--   0        0        0      789 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/networks.py
+-rw-r--r--   0        0        0     1527 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/ransom_groups.py
+-rw-r--r--   0        0        0     5569 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/enum/services.py
+-rw-r--r--   0        0        0     4961 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/model/model.py
+-rw-r--r--   0        0        0      635 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/taxonomy/__init__.py
+-rw-r--r--   0        0        0     2347 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/taxonomy/flavours.py
+-rw-r--r--   0        0        0    12263 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/taxonomy/taxonomy.py
+-rw-r--r--   0        0        0      610 2023-04-12 11:01:34.010455 vysion-1.0.4/vysion/version.py
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 vysion-1.0.4/PKG-INFO
```

### Comparing `vysion-1.0.3/LICENSE` & `vysion-1.0.4/LICENSE`

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
    limitations under the License.
```

### Comparing `vysion-1.0.3/README.md` & `vysion-1.0.4/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-
-# References
-
-- https://pydantic-docs.helpmanual.io/
-- https://python-patterns.guide/
-- https://docs.pytest.org/en/7.1.x/getting-started.html#get-started
-- https://github.com/samuelcolvin/pydantic
-- https://python-poetry.org/docs/pyproject
-- https://github.com/wemake-services/wemake-python-package
-
-## Style
-
-- https://code.visualstudio.com/docs/languages/python
-- https://code.visualstudio.com/docs/python/linting
-- https://code.visualstudio.com/api/language-extensions/snippet-guide
-- https://semver.org/
-- https://snyk.io/blog/python-poetry-package-manager/
-
-### Taxonomy
-
-- https://github.com/MISP/misp-taxonomies/blob/main/tools/machinetag.py
-- https://www.misp-project.org/taxonomies.html#_mapping_of_taxonomies
-- https://github.com/MISP/misp-taxonomies
-- https://github.com/MISP/misp-taxonomies/blob/main/tools/docs/images/taxonomy-explanation.png
-
-## Entorno
-
-- vs-code
-    - Extensiones:
-        - snyk
-        - flake8
-
-## The Zen of Python
-
-```python
-import this
-> The Zen of Python, by Tim Peters
-> 
-> Beautiful is better than ugly.
-> Explicit is better than implicit.
-> Simple is better than complex.
-> Complex is better than complicated.
-> Flat is better than nested.
-> Sparse is better than dense.
-> Readability counts.
-> Special cases aren't special enough to break the rules.
-> Although practicality beats purity.
-> Errors should never pass silently.
-> Unless explicitly silenced.
-> In the face of ambiguity, refuse the temptation to guess.
-> There should be one-- and preferably only one --obvious way to do it.
-> Although that way may not be obvious at first unless you're Dutch.
-> Now is better than never.
-> Although never is often better than *right* now.
-> If the implementation is hard to explain, it's a bad idea.
-> If the implementation is easy to explain, it may be a good idea.
-> Namespaces are one honking great idea -- let's do more of those!
-```
-
-# Ackowledgement
-
-We really appreciate the documentation of https://github.com/VirusTotal/vt-py
+
+# References
+
+- https://pydantic-docs.helpmanual.io/
+- https://python-patterns.guide/
+- https://docs.pytest.org/en/7.1.x/getting-started.html#get-started
+- https://github.com/samuelcolvin/pydantic
+- https://python-poetry.org/docs/pyproject
+- https://github.com/wemake-services/wemake-python-package
+
+## Style
+
+- https://code.visualstudio.com/docs/languages/python
+- https://code.visualstudio.com/docs/python/linting
+- https://code.visualstudio.com/api/language-extensions/snippet-guide
+- https://semver.org/
+- https://snyk.io/blog/python-poetry-package-manager/
+
+### Taxonomy
+
+- https://github.com/MISP/misp-taxonomies/blob/main/tools/machinetag.py
+- https://www.misp-project.org/taxonomies.html#_mapping_of_taxonomies
+- https://github.com/MISP/misp-taxonomies
+- https://github.com/MISP/misp-taxonomies/blob/main/tools/docs/images/taxonomy-explanation.png
+
+## Entorno
+
+- vs-code
+    - Extensiones:
+        - snyk
+        - flake8
+
+## The Zen of Python
+
+```python
+import this
+> The Zen of Python, by Tim Peters
+> 
+> Beautiful is better than ugly.
+> Explicit is better than implicit.
+> Simple is better than complex.
+> Complex is better than complicated.
+> Flat is better than nested.
+> Sparse is better than dense.
+> Readability counts.
+> Special cases aren't special enough to break the rules.
+> Although practicality beats purity.
+> Errors should never pass silently.
+> Unless explicitly silenced.
+> In the face of ambiguity, refuse the temptation to guess.
+> There should be one-- and preferably only one --obvious way to do it.
+> Although that way may not be obvious at first unless you're Dutch.
+> Now is better than never.
+> Although never is often better than *right* now.
+> If the implementation is hard to explain, it's a bad idea.
+> If the implementation is easy to explain, it may be a good idea.
+> Namespaces are one honking great idea -- let's do more of those!
+```
+
+# Ackowledgement
+
+We really appreciate the documentation of https://github.com/VirusTotal/vt-py
```

### Comparing `vysion-1.0.3/pyproject.toml` & `vysion-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-[tool.poetry]
-name = "vysion"
-version = "1.0.3"
-description = "The official Python client library for Vysion"
-homepage = "https://vysion.ai"
-repository = "https://gitlab.com/byronlabs/vysion/vysion-py"
-documentation = "https://developers.vysion.ai"
-authors = [
-  "Javier Junquera-Sánchez <javier.junquera@byronlabs.io>"
-]
-license = "Apache-2.0"
-readme = "README.md"
-classifiers=[
-   "Programming Language :: Python :: 3",
-   "License :: OSI Approved :: Apache Software License",
-   "Operating System :: OS Independent"
-]
-# packages = [vysion', 'vysion.client', 'vysion.model',  'vysion.dto', 'vysion.taxonomy'],
-
-[tool.poetry.dependencies]
-python = "^3.7.0"
-
-pydantic = "1.10.3"
-pymisp = "2.4.159"
-softenum = "1.0.1"
-requests = "^2.28.1"
-
-[tool.poetry.dev-dependencies]
-pytest = "7.1.2"
-python-dotenv = "0.19.2"
-
-flake8 = "4.0.1"
-pyflakes = "2.4.0"
-mypy = "^0.961"
-black = "^22.6.0"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
+[tool.poetry]
+name = "vysion"
+version = "1.0.4"
+description = "The official Python client library for Vysion"
+homepage = "https://vysion.ai"
+repository = "https://gitlab.com/byronlabs/vysion/vysion-py"
+documentation = "https://developers.vysion.ai"
+authors = [
+  "Javier Junquera-Sánchez <javier.junquera@byronlabs.io>"
+]
+license = "Apache-2.0"
+readme = "README.md"
+classifiers=[
+   "Programming Language :: Python :: 3",
+   "License :: OSI Approved :: Apache Software License",
+   "Operating System :: OS Independent"
+]
+# packages = [vysion', 'vysion.client', 'vysion.model',  'vysion.dto', 'vysion.taxonomy'],
+
+[tool.poetry.dependencies]
+python = "^3.7.0"
+
+pydantic = "1.10.3"
+pymisp = "2.4.159"
+softenum = "1.0.1"
+requests = "^2.28.1"
+
+[tool.poetry.dev-dependencies]
+pytest = "7.1.2"
+python-dotenv = "0.19.2"
+
+flake8 = "4.0.1"
+pyflakes = "2.4.0"
+mypy = "^0.961"
+black = "^22.6.0"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
```

### Comparing `vysion-1.0.3/vysion/__init__.py` & `vysion-1.0.4/vysion/client/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from . import client
-from . import taxonomy
-from . import model
-from . import dto
-
-from .version import __version__
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from .client import *
+from . import error
```

### Comparing `vysion-1.0.3/vysion/client/__init__.py` & `vysion-1.0.4/vysion/model/enum/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from .client import *
-from . import error
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from .languages import *
+from .services import *
+from .networks import *
+from .ransom_groups import *
```

### Comparing `vysion-1.0.3/vysion/client/client.py` & `vysion-1.0.4/vysion/client/client.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,360 +1,360 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-# TODO Referenciar vt-py
-
-from datetime import datetime, timedelta
-import logging
-from typing import Union
-from urllib.parse import urljoin, urlencode
-
-# from pydantic import validate_arguments
-import requests
-from vysion.client.error import APIError
-
-import vysion.dto as dto
-from vysion.dto import VysionError
-from vysion.version import __version__ as vysion_version
-
-_API_HOST = "https://api.vysion.ai"
-
-# All API endpoints start with this prefix, you don't need to include the
-# prefix in the paths you request as it's prepended automatically.
-_ENDPOINT_PREFIX = "/api/v1/"
-
-_BASE_API = urljoin(_API_HOST, _ENDPOINT_PREFIX)
-
-LOGGER = logging.getLogger("vysion-py")
-LOGGER.setLevel(logging.INFO)
-
-# __all__ = []
-
-
-class BaseClient:
-
-    # __attrs__ = []
-
-    # @validate_arguments #
-    def __init__(self, api_key: str = None, headers: dict = dict(), proxy: dict = None):
-
-        assert api_key is not None, "API key MUST be provided"
-        assert isinstance(api_key, str), "API key MUST be a string"
-
-        self.api_key = api_key
-        self.proxy = proxy  # TODO Rename proxy to proxies
-        self.headers = headers
-
-    def __get_session__(self) -> requests.Session:
-
-        # TODO Configure proxy
-
-        # If session is undefined
-        try:
-            self._session
-        except (NameError, AttributeError):
-
-            headers = self.headers.copy()
-            headers.update(
-                {
-                    "X-API-KEY": self.api_key,
-                    "User-Agent": "vysion-py/%s" % vysion_version,
-                }
-            )
-
-            self._session: requests.Session = requests.Session()
-            self._session.headers.update(headers)
-            self._session.proxies = self.proxy
-
-        return self._session
-
-    def _build_api_url__(self, endpoint, param, **query_params):
-
-        base = urljoin(_BASE_API, f"{endpoint}/{param}")
-
-        query_params_initialzed = query_params.copy()
-
-        keys = list(query_params.keys())
-        keys.sort()
-
-        for i in keys:
-
-            v = query_params[i]
-
-            if v is None:
-                del query_params_initialzed[i]
-
-        query = "?" + urlencode(query_params_initialzed)
-
-        return urljoin(base, query)
-
-    def _make_request(self, url: str) -> dto.VysionResponse:
-
-        session = self.__get_session__()
-        r = session.get(url)
-
-        # TODO Improve this
-        if r.status_code != 200:
-            try:
-                err = r.json()
-                code = err.get("code")
-                message = err.get("message")
-            except:
-                code = r.status_code
-                message = r.text
-
-            raise APIError(code, message)
-
-        payload = r.json()
-
-        result = dto.VysionResponse.parse_obj(payload)
-
-        return result
-
-
-def vysion_error_manager(method) -> Union[dto.Result, VysionError]:
-
-    def manage(*args, **kwargs):
-        try:
-            result = method(*args, **kwargs)
-            return result
-        except APIError as e:
-            return VysionError(code=e.code, message=e.message)
-        except Exception as e:
-            LOGGER.error(e)
-            return VysionError()
-
-    return manage
-
-
-class Client(BaseClient):
-
-    # def add_url(self, url:str, type:VysionURL.Type):
-    #     """Add a Tor URL to be analyzed by PARCHE.
-
-    #     :param url: URL to be scanned.
-    #     :param type: Instance of :class:`VysionURL.Type`
-    #     :returns: An instance of :class:`VysionResponse`
-    #     """
-    #     pass
-
-    # def find_onion(self):
-    #   pass
-
-    # def add_onion(self):
-    #   pass
-
-    # def consume_feed(self):
-    #   pass
-
-    @vysion_error_manager
-    def status(self):
-        # TODO Check API status
-        pass
-
-    @vysion_error_manager
-    def search(
-        self,
-        query: str,
-        exact: bool = False,
-        network: dto.Network = None,
-        language: dto.Language = None,
-        page: int = 1,
-        before: datetime = None,
-        after: datetime = None,
-    ) -> dto.Result:
-
-        url = self._build_api_url__(
-            "search",
-            query,
-            exact=exact,
-            network=network,
-            language=language,
-            page=page,
-            before=before,
-            after=after,
-        )
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_btc(
-        self, btc: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__("btc", btc, page=page, before=before, after=after)
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_eth(
-        self, eth: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__("eth", eth, page=page, before=before, after=after)
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_dot(
-        self, dot: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__("dot", dot, page=page, before=before, after=after)
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_xrp(
-        self, xrp: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__("xrp", xrp, page=page, before=before, after=after)
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_xmr(
-        self, xmr: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__("xmr", xmr, page=page, before=before, after=after)
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_zec(
-        self, zec: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__("zec", zec, page=page, before=before, after=after)
-
-        result = self._make_request(url)
-        return result.data
-
-    # TODO find_domain?
-    @vysion_error_manager
-    def find_url(
-        self,
-        query_url: str,
-        page: int = 1,
-        before: datetime = None,
-        after: datetime = None,
-    ) -> dto.Result:
-
-        url = self._build_api_url__(
-            "url", query_url, page=page, before=before, after=after
-        )
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def find_email(
-        self, email: str, page: int = 1, before: datetime = None, after: datetime = None
-    ) -> dto.Result:
-
-        url = self._build_api_url__(
-            "email", email, page=page, before=before, after=after
-        )
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def get_document(self, document_id: str) -> dto.Result:
-
-        url = self._build_api_url__("document", document_id)
-
-        result = self._make_request(url)
-        return result.data
-
-    @vysion_error_manager
-    def get_tag(self, tag: str) -> dto.Result:
-
-        url = self._build_api_url__("tag", tag)
-
-        result = self._make_request(url)
-        return result.data
-
-    # FEEDS
-    @vysion_error_manager
-    def consume_feed_ransomware(self, batch_day: datetime = datetime.today()):
-        pass
-
-
-# TODO Develop feeds logic
-# Example: https://github.com/VirusTotal/vt-py/blob/master/vt/feed.py
-class DaylyFeed(Client):
-    def _consume_batch(self, start_time, end_time):
-        raise NotImplementedError()
-
-    def consume(self, batch_day: datetime = datetime.today()):
-        start_time = datetime(datetime.year, datetime.month, datetime.day)
-        end_time = start_time + timedelta(days=1)
-        return self._consume_batch(start_time, end_time)
-
-
-class RansomwareFeed(DaylyFeed):
-    def _consume_batch(self, start_time, end_time):
-
-        days = (datetime.now() - start_time).days
-        pages = (end_time - start_time).days
-
-        for page in range(pages):
-            url = self._build_api_url__("feed", "ransomware", days=days, page=page + 1)
-            yield self._make_request(url)
-
-
-"""TODO Transform response
-{
-  "total": {
-    "value": 26,
-    "relation": "eq"
-  },
-  "max_score": null,
-  "hits": [
-    {
-      "_index": "ransomware-62022",
-      "_id": "dab4447fbd8440251d41e31b8ab1770186f429e46d9cd6903fbe17367efcba23",
-      "_score": null,
-      "_ignored": [
-        "info.keyword"
-      ],
-      "_source": {
-        "company": "RG Alliance Group",
-        "link": "http://quantum445bh3gzuyilxdzs5xdepf3b7lkcupswvkryf3n7hgzpxebid.onion/target/rgalliancegroup",
-        "date": "2022-06-16T00:00:00",
-        "group": "Quantum",
-        "info": "1.2TB 3.6K visibility\n2022-06-16\nInfo Post About: \"RG Alliance Group\"\nCompany Name\nRG Alliance Group\nCompany Website\nOfficial Link\nTotal Revenue\n$9M\nLast Updated:\n2022-06-16\nVolume Of Data Uploaded\n0% (announcement)\n- Complete databases of clients of the accounting program QuickBooks, including tax, payroll and banking information of Client Companies.\n- Contracts, Accounting.Ballances, Scans, invoices, etc. Client companies\n- Email correspondence with client companies\n- Personal information (Scans+SSN+Bank info+etc) of employees of Client Companies\n- Personal information (Scans+SSN+Bank info+etc) of RG Alliance Group employees\n- Outlook .pst backups of RG Alliance Group employees\nYour Feedback\nAuthor\nMessage\nSUBMIT",
-        "company_link": "http://www.rgalliance.com/"
-      },
-      "sort": [
-        1655337600000
-      ]
-    }
-    ...
-  ]
-}
-"""
-
-# TODO /api/v1/feeds
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+# TODO Referenciar vt-py
+
+from datetime import datetime, timedelta
+import logging
+from typing import Union
+from urllib.parse import urljoin, urlencode
+
+# from pydantic import validate_arguments
+import requests
+from vysion.client.error import APIError
+
+import vysion.dto as dto
+from vysion.dto import VysionError
+from vysion.version import __version__ as vysion_version
+
+_API_HOST = "https://api.vysion.ai"
+
+# All API endpoints start with this prefix, you don't need to include the
+# prefix in the paths you request as it's prepended automatically.
+_ENDPOINT_PREFIX = "/api/v1/"
+
+_BASE_API = urljoin(_API_HOST, _ENDPOINT_PREFIX)
+
+LOGGER = logging.getLogger("vysion-py")
+LOGGER.setLevel(logging.INFO)
+
+# __all__ = []
+
+
+class BaseClient:
+
+    # __attrs__ = []
+
+    # @validate_arguments #
+    def __init__(self, api_key: str = None, headers: dict = dict(), proxy: dict = None):
+
+        assert api_key is not None, "API key MUST be provided"
+        assert isinstance(api_key, str), "API key MUST be a string"
+
+        self.api_key = api_key
+        self.proxy = proxy  # TODO Rename proxy to proxies
+        self.headers = headers
+
+    def __get_session__(self) -> requests.Session:
+
+        # TODO Configure proxy
+
+        # If session is undefined
+        try:
+            self._session
+        except (NameError, AttributeError):
+
+            headers = self.headers.copy()
+            headers.update(
+                {
+                    "X-API-KEY": self.api_key,
+                    "User-Agent": "vysion-py/%s" % vysion_version,
+                }
+            )
+
+            self._session: requests.Session = requests.Session()
+            self._session.headers.update(headers)
+            self._session.proxies = self.proxy
+
+        return self._session
+
+    def _build_api_url__(self, endpoint, param, **query_params):
+
+        base = urljoin(_BASE_API, f"{endpoint}/{param}")
+
+        query_params_initialzed = query_params.copy()
+
+        keys = list(query_params.keys())
+        keys.sort()
+
+        for i in keys:
+
+            v = query_params[i]
+
+            if v is None:
+                del query_params_initialzed[i]
+
+        query = "?" + urlencode(query_params_initialzed)
+
+        return urljoin(base, query)
+
+    def _make_request(self, url: str) -> dto.VysionResponse:
+
+        session = self.__get_session__()
+        r = session.get(url)
+
+        # TODO Improve this
+        if r.status_code != 200:
+            try:
+                err = r.json()
+                code = err.get("code")
+                message = err.get("message")
+            except:
+                code = r.status_code
+                message = r.text
+
+            raise APIError(code, message)
+
+        payload = r.json()
+
+        result = dto.VysionResponse.parse_obj(payload)
+
+        return result
+
+
+def vysion_error_manager(method) -> Union[dto.Result, VysionError]:
+
+    def manage(*args, **kwargs):
+        try:
+            result = method(*args, **kwargs)
+            return result
+        except APIError as e:
+            return VysionError(code=e.code, message=e.message)
+        except Exception as e:
+            LOGGER.error(e)
+            return VysionError()
+
+    return manage
+
+
+class Client(BaseClient):
+
+    # def add_url(self, url:str, type:VysionURL.Type):
+    #     """Add a Tor URL to be analyzed by PARCHE.
+
+    #     :param url: URL to be scanned.
+    #     :param type: Instance of :class:`VysionURL.Type`
+    #     :returns: An instance of :class:`VysionResponse`
+    #     """
+    #     pass
+
+    # def find_onion(self):
+    #   pass
+
+    # def add_onion(self):
+    #   pass
+
+    # def consume_feed(self):
+    #   pass
+
+    @vysion_error_manager
+    def status(self):
+        # TODO Check API status
+        pass
+
+    @vysion_error_manager
+    def search(
+        self,
+        query: str,
+        exact: bool = False,
+        network: dto.Network = None,
+        language: dto.Language = None,
+        page: int = 1,
+        before: datetime = None,
+        after: datetime = None,
+    ) -> dto.Result:
+
+        url = self._build_api_url__(
+            "search",
+            query,
+            exact=exact,
+            network=network,
+            language=language,
+            page=page,
+            before=before,
+            after=after,
+        )
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_btc(
+        self, btc: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__("btc", btc, page=page, before=before, after=after)
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_eth(
+        self, eth: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__("eth", eth, page=page, before=before, after=after)
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_dot(
+        self, dot: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__("dot", dot, page=page, before=before, after=after)
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_xrp(
+        self, xrp: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__("xrp", xrp, page=page, before=before, after=after)
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_xmr(
+        self, xmr: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__("xmr", xmr, page=page, before=before, after=after)
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_zec(
+        self, zec: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__("zec", zec, page=page, before=before, after=after)
+
+        result = self._make_request(url)
+        return result.data
+
+    # TODO find_domain?
+    @vysion_error_manager
+    def find_url(
+        self,
+        query_url: str,
+        page: int = 1,
+        before: datetime = None,
+        after: datetime = None,
+    ) -> dto.Result:
+
+        url = self._build_api_url__(
+            "url", query_url, page=page, before=before, after=after
+        )
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def find_email(
+        self, email: str, page: int = 1, before: datetime = None, after: datetime = None
+    ) -> dto.Result:
+
+        url = self._build_api_url__(
+            "email", email, page=page, before=before, after=after
+        )
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def get_document(self, document_id: str) -> dto.Result:
+
+        url = self._build_api_url__("document", document_id)
+
+        result = self._make_request(url)
+        return result.data
+
+    @vysion_error_manager
+    def get_tag(self, tag: str) -> dto.Result:
+
+        url = self._build_api_url__("tag", tag)
+
+        result = self._make_request(url)
+        return result.data
+
+    # FEEDS
+    @vysion_error_manager
+    def consume_feed_ransomware(self, batch_day: datetime = datetime.today()):
+        pass
+
+
+# TODO Develop feeds logic
+# Example: https://github.com/VirusTotal/vt-py/blob/master/vt/feed.py
+class DaylyFeed(Client):
+    def _consume_batch(self, start_time, end_time):
+        raise NotImplementedError()
+
+    def consume(self, batch_day: datetime = datetime.today()):
+        start_time = datetime(datetime.year, datetime.month, datetime.day)
+        end_time = start_time + timedelta(days=1)
+        return self._consume_batch(start_time, end_time)
+
+
+class RansomwareFeed(DaylyFeed):
+    def _consume_batch(self, start_time, end_time):
+
+        days = (datetime.now() - start_time).days
+        pages = (end_time - start_time).days
+
+        for page in range(pages):
+            url = self._build_api_url__("feed", "ransomware", days=days, page=page + 1)
+            yield self._make_request(url)
+
+
+"""TODO Transform response
+{
+  "total": {
+    "value": 26,
+    "relation": "eq"
+  },
+  "max_score": null,
+  "hits": [
+    {
+      "_index": "ransomware-62022",
+      "_id": "dab4447fbd8440251d41e31b8ab1770186f429e46d9cd6903fbe17367efcba23",
+      "_score": null,
+      "_ignored": [
+        "info.keyword"
+      ],
+      "_source": {
+        "company": "RG Alliance Group",
+        "link": "http://quantum445bh3gzuyilxdzs5xdepf3b7lkcupswvkryf3n7hgzpxebid.onion/target/rgalliancegroup",
+        "date": "2022-06-16T00:00:00",
+        "group": "Quantum",
+        "info": "1.2TB 3.6K visibility\n2022-06-16\nInfo Post About: \"RG Alliance Group\"\nCompany Name\nRG Alliance Group\nCompany Website\nOfficial Link\nTotal Revenue\n$9M\nLast Updated:\n2022-06-16\nVolume Of Data Uploaded\n0% (announcement)\n- Complete databases of clients of the accounting program QuickBooks, including tax, payroll and banking information of Client Companies.\n- Contracts, Accounting.Ballances, Scans, invoices, etc. Client companies\n- Email correspondence with client companies\n- Personal information (Scans+SSN+Bank info+etc) of employees of Client Companies\n- Personal information (Scans+SSN+Bank info+etc) of RG Alliance Group employees\n- Outlook .pst backups of RG Alliance Group employees\nYour Feedback\nAuthor\nMessage\nSUBMIT",
+        "company_link": "http://www.rgalliance.com/"
+      },
+      "sort": [
+        1655337600000
+      ]
+    }
+    ...
+  ]
+}
+"""
+
+# TODO /api/v1/feeds
```

### Comparing `vysion-1.0.3/vysion/client/error.py` & `vysion-1.0.4/vysion/client/error.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-from vysion.dto import VysionError
-
-
-class APIError(Exception):
-    """Class that encapsules errors returned by the Vysion API."""
-
-    @classmethod
-    def from_dict(cls, dict_error):
-        return cls(dict_error["code"], dict_error.get("message"))
-
-    def __init__(self, code: int, message: str):
-
-        super().__init__()
-
-        if code not in [i.value for i in VysionError.StatusCode]:
-            self.code = VysionError.StatusCode.UNK
-            self.message = f"{message} (Original code: {code})"
-        else:
-            self.code = code
-            self.message = message
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+from vysion.dto import VysionError
+
+
+class APIError(Exception):
+    """Class that encapsules errors returned by the Vysion API."""
+
+    @classmethod
+    def from_dict(cls, dict_error):
+        return cls(dict_error["code"], dict_error.get("message"))
+
+    def __init__(self, code: int, message: str):
+
+        super().__init__()
+
+        if code not in [i.value for i in VysionError.StatusCode]:
+            self.code = VysionError.StatusCode.UNK
+            self.message = f"{message} (Original code: {code})"
+        else:
+            self.code = code
+            self.message = message
```

### Comparing `vysion-1.0.3/vysion/dto/__init__.py` & `vysion-1.0.4/vysion/taxonomy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 ByronLabs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-from .dto import *
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from .taxonomy import *
+from . import flavours
```

### Comparing `vysion-1.0.3/vysion/dto/dto.py` & `vysion-1.0.4/vysion/dto/dto.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,269 +1,269 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 ByronLabs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-from enum import Enum
-import hashlib
-
-from datetime import datetime
-from vysion.model import enum
-
-from vysion.taxonomy import Monero_Address, Ripple_Address
-
-try:
-    from types import NoneType
-except:
-    NoneType: type = type(None)
-
-from typing import List, Optional, Union
-from urllib.parse import urlparse
-
-from pydantic import BaseModel, Field # , constr
-from .tag import *
-
-from urllib.parse import urlparse
-from vysion import taxonomy as vystaxonomy
-from vysion.model import URL as URL_model
-from vysion.model.enum import Services, Network, Language, RansomGroup
-
-
-class Email(BaseModel):
-
-    _taxonomy = [vystaxonomy.Email]
-
-    # RFC 5322 Official Standard (https://www.emailregex.com/)
-    # value: constr(regex=r'''(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])''') # TODO Añadir que es str
-    value: str  # TODO Fix regex to allow caps
-
-
-class Paste(BaseModel):
-
-    _taxonomy = [vystaxonomy.Pastebin, vystaxonomy.JustPaste]
-
-    value: str  # TODO Regex
-
-
-class Skype(BaseModel):
-
-    _taxonomy = [vystaxonomy.Skype]
-
-    value: str  # TODO Regex
-
-
-class Telegram(BaseModel):
-
-    _taxonomy = [vystaxonomy.Telegram]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class BitcoinAddress(BaseModel):
-
-    _taxonomy = [vystaxonomy.Bitcoin_Address]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class PolkadotAddress(BaseModel):
-
-    _taxonomy = [vystaxonomy.Polkadot_Address]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class EthereumAddress(BaseModel):
-
-    _taxonomy = [vystaxonomy.Ethereum_Address]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class MoneroAddress(BaseModel):
-
-    _taxonomy = [vystaxonomy.Monero_Address]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class RippleAddress(BaseModel):
-
-    _taxonomy = [vystaxonomy.Ripple_Address]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class ZcashAddress(BaseModel):
-
-    _taxonomy = [vystaxonomy.Zcash_Address]  # TODO Create Telegram URL
-
-    value: str  # TODO Regex
-
-
-class WhatsApp(BaseModel):
-
-    _taxonomy = [vystaxonomy.WhatsApp]
-
-    value: str  # TODO Regex
-
-
-class URL(BaseModel):
-
-    _taxonomy = [vystaxonomy.URL]
-
-    protocol: Optional[str]
-    domain: Optional[str]
-    port: Optional[int]
-    path: Optional[str]
-    signature: str
-    network: Network = Field(default_factory=lambda: Network.clearnet)
-
-    @classmethod
-    def parse(cls, url):
-
-        # TODO Save this parsed in a private variable? (e.g., _pared_)
-        parsed = URL_model.parse(url)
-        print(parsed)
-        tmp_result = cls(
-            protocol=parsed.protocol,
-            domain=parsed.domain,
-            port=parsed.port,
-            path=parsed.path,
-            signature=str(parsed.signature) # TODO Replace signature: str --> UUID
-        )
-
-        return tmp_result
-
-    def build(self) -> str:
-        return f"{self.protocol}://{self.domain}:{self.port}{self.path}"
-
-
-class Page(BaseModel):
-
-    id: str
-    url: URL
-    parent: str = None
-    title: str = None  # TODO Revisar si None o str()
-    language: Optional[Language]
-    html: str = None
-    sha1sum: str = None
-    sha256sum: str = None
-    ssdeep: str = None
-    date: datetime = None
-    chunk: bool = False
-
-
-class RansomwarePage(BaseModel):
-
-    id: str
-    url: URL
-    # title: str = None  
-    group: RansomGroup
-    company: Optional[str]
-    company_address: Optional[str]
-    company_link: Optional[str]
-    info: Optional[str]
-    html: Optional[str]
-    country: Optional[str]
-    sha256sum: str = None
-    ssdeep: str = None
-    date: datetime 
-    chunk: bool = False
-
-
-class RansomwareHit(BaseModel):
-    page: RansomwarePage
-
-
-class Hit(BaseModel):
-
-    page: Page
-    tag: List[Tag]
-    email: List[Email] = Field(default_factory=lambda: [])
-    paste: List[Paste] = Field(default_factory=lambda: [])
-    skype: List[Skype] = Field(default_factory=lambda: [])
-    telegram: List[Telegram] = Field(default_factory=lambda: [])
-    whatsapp: List[WhatsApp] = Field(default_factory=lambda: [])
-    bitcoin_address: List[BitcoinAddress] = Field(default_factory=lambda: [])
-    polkadot_address: List[PolkadotAddress] = Field(default_factory=lambda: [])
-    ethereum_address: List[EthereumAddress] = Field(default_factory=lambda: [])
-    monero_address: List[MoneroAddress] = Field(default_factory=lambda: [])
-    ripple_address: List[RippleAddress] = Field(default_factory=lambda: [])
-    zcash_address: List[ZcashAddress] = Field(default_factory=lambda: [])
-
-
-class RansomFeedHit(BaseModel):
-
-    id: str
-    company: Optional[str]
-    company_link: Optional[str]
-    link: str
-    group: RansomGroup
-    date: datetime
-    info: Optional[str]
-    country: Optional[str]
-
-
-class TelegramFeedHit(BaseModel):
-
-    id: str
-    telegram: List[str]
-    date: datetime
-    url: str
-    path: str
-    network: str
-
-
-class Result(BaseModel):
-
-    # TODO Añadir paginación, query, etc?
-    total: int = 0
-    hits: Union[List[Hit], List[RansomFeedHit], List[TelegramFeedHit], List[RansomwareHit]] = Field(
-        default_factory=lambda: [])
-        
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        if self.total <= 0:
-            self.total = len(self.hits)
-
-    def get_type(self) -> type:
-
-        if len(self.hits) <= 0:
-            return NoneType
-
-        return type(self.hits[0])
-
-
-# TODO Move API responses to other class
-class VysionResponse(BaseModel):
-    """
-    VysionResponse is a json:api flavoured response from the API
-    """
-
-    data: Result  # TODO Add type to all JSON:API responses
-
-
-class VysionError(BaseModel):
-
-    class StatusCode(int, Enum):
-
-        UNK = 000
-        OK = 200
-        REQ_ERROR = 400
-        UNAUTHORIZED = 403
-        NOT_FOUND = 404
-        INTERNAL_ERROR = 500
-
-    code: StatusCode = StatusCode.UNK
-    message: str = "UNK_ERR"
+#!/usr/bin/env python3
+"""
+Copyright 2022 ByronLabs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+from enum import Enum
+import hashlib
+
+from datetime import datetime
+from vysion.model import enum
+
+from vysion.taxonomy import Monero_Address, Ripple_Address
+
+try:
+    from types import NoneType
+except:
+    NoneType: type = type(None)
+
+from typing import List, Optional, Union
+from urllib.parse import urlparse
+
+from pydantic import BaseModel, Field # , constr
+from .tag import *
+
+from urllib.parse import urlparse
+from vysion import taxonomy as vystaxonomy
+from vysion.model import URL as URL_model
+from vysion.model.enum import Services, Network, Language, RansomGroup
+
+
+class Email(BaseModel):
+
+    _taxonomy = [vystaxonomy.Email]
+
+    # RFC 5322 Official Standard (https://www.emailregex.com/)
+    # value: constr(regex=r'''(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])''') # TODO Añadir que es str
+    value: str  # TODO Fix regex to allow caps
+
+
+class Paste(BaseModel):
+
+    _taxonomy = [vystaxonomy.Pastebin, vystaxonomy.JustPaste]
+
+    value: str  # TODO Regex
+
+
+class Skype(BaseModel):
+
+    _taxonomy = [vystaxonomy.Skype]
+
+    value: str  # TODO Regex
+
+
+class Telegram(BaseModel):
+
+    _taxonomy = [vystaxonomy.Telegram]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class BitcoinAddress(BaseModel):
+
+    _taxonomy = [vystaxonomy.Bitcoin_Address]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class PolkadotAddress(BaseModel):
+
+    _taxonomy = [vystaxonomy.Polkadot_Address]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class EthereumAddress(BaseModel):
+
+    _taxonomy = [vystaxonomy.Ethereum_Address]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class MoneroAddress(BaseModel):
+
+    _taxonomy = [vystaxonomy.Monero_Address]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class RippleAddress(BaseModel):
+
+    _taxonomy = [vystaxonomy.Ripple_Address]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class ZcashAddress(BaseModel):
+
+    _taxonomy = [vystaxonomy.Zcash_Address]  # TODO Create Telegram URL
+
+    value: str  # TODO Regex
+
+
+class WhatsApp(BaseModel):
+
+    _taxonomy = [vystaxonomy.WhatsApp]
+
+    value: str  # TODO Regex
+
+
+class URL(BaseModel):
+
+    _taxonomy = [vystaxonomy.URL]
+
+    protocol: Optional[str]
+    domain: Optional[str]
+    port: Optional[int]
+    path: Optional[str]
+    signature: str
+    network: Network = Field(default_factory=lambda: Network.clearnet)
+
+    @classmethod
+    def parse(cls, url):
+
+        # TODO Save this parsed in a private variable? (e.g., _pared_)
+        parsed = URL_model.parse(url)
+        print(parsed)
+        tmp_result = cls(
+            protocol=parsed.protocol,
+            domain=parsed.domain,
+            port=parsed.port,
+            path=parsed.path,
+            signature=str(parsed.signature) # TODO Replace signature: str --> UUID
+        )
+
+        return tmp_result
+
+    def build(self) -> str:
+        return f"{self.protocol}://{self.domain}:{self.port}{self.path}"
+
+
+class Page(BaseModel):
+
+    id: str
+    url: URL
+    parent: str = None
+    title: str = None  # TODO Revisar si None o str()
+    language: Optional[Language]
+    html: str = None
+    sha1sum: str = None
+    sha256sum: str = None
+    ssdeep: str = None
+    date: datetime = None
+    chunk: bool = False
+
+
+class RansomwarePage(BaseModel):
+
+    id: str
+    url: URL
+    # title: str = None  
+    group: RansomGroup
+    company: Optional[str]
+    company_address: Optional[str]
+    company_link: Optional[str]
+    info: Optional[str]
+    html: Optional[str]
+    country: Optional[str]
+    sha256sum: str = None
+    ssdeep: str = None
+    date: datetime 
+    chunk: bool = False
+
+
+class RansomwareHit(BaseModel):
+    page: RansomwarePage
+
+
+class Hit(BaseModel):
+
+    page: Page
+    tag: List[Tag]
+    email: List[Email] = Field(default_factory=lambda: [])
+    paste: List[Paste] = Field(default_factory=lambda: [])
+    skype: List[Skype] = Field(default_factory=lambda: [])
+    telegram: List[Telegram] = Field(default_factory=lambda: [])
+    whatsapp: List[WhatsApp] = Field(default_factory=lambda: [])
+    bitcoin_address: List[BitcoinAddress] = Field(default_factory=lambda: [])
+    polkadot_address: List[PolkadotAddress] = Field(default_factory=lambda: [])
+    ethereum_address: List[EthereumAddress] = Field(default_factory=lambda: [])
+    monero_address: List[MoneroAddress] = Field(default_factory=lambda: [])
+    ripple_address: List[RippleAddress] = Field(default_factory=lambda: [])
+    zcash_address: List[ZcashAddress] = Field(default_factory=lambda: [])
+
+
+class RansomFeedHit(BaseModel):
+
+    id: str
+    company: Optional[str]
+    company_link: Optional[str]
+    link: str
+    group: RansomGroup
+    date: datetime
+    info: Optional[str]
+    country: Optional[str]
+
+
+class TelegramFeedHit(BaseModel):
+
+    id: str
+    telegram: List[str]
+    date: datetime
+    url: str
+    path: str
+    network: str
+
+
+class Result(BaseModel):
+
+    # TODO Añadir paginación, query, etc?
+    total: int = 0
+    hits: Union[List[Hit], List[RansomFeedHit], List[TelegramFeedHit], List[RansomwareHit]] = Field(
+        default_factory=lambda: [])
+        
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if self.total <= 0:
+            self.total = len(self.hits)
+
+    def get_type(self) -> type:
+
+        if len(self.hits) <= 0:
+            return NoneType
+
+        return type(self.hits[0])
+
+
+# TODO Move API responses to other class
+class VysionResponse(BaseModel):
+    """
+    VysionResponse is a json:api flavoured response from the API
+    """
+
+    data: Result  # TODO Add type to all JSON:API responses
+
+
+class VysionError(BaseModel):
+
+    class StatusCode(int, Enum):
+
+        UNK = 000
+        OK = 200
+        REQ_ERROR = 400
+        UNAUTHORIZED = 403
+        NOT_FOUND = 404
+        INTERNAL_ERROR = 500
+
+    code: StatusCode = StatusCode.UNK
+    message: str = "UNK_ERR"
```

### Comparing `vysion-1.0.3/vysion/dto/util.py` & `vysion-1.0.4/vysion/dto/util.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-import json
-from pymisp import MISPAttribute, MISPEvent, MISPObject, MISPTag
-
-try:
-    from types import NoneType
-except:
-    NoneType = type(None)
-
-import vysion.dto as dto
-from vysion.dto import Hit, RansomFeedHit, Page, URL
-
-
-class MISPProcessor:
-
-    def __init__(self):
-        self.misp_event = MISPEvent()
-
-    def parse_hit(self, hit: Hit, ref_attribute: MISPAttribute = None, **_):
-
-        page: Page = hit.page
-
-        # TODO Add more page parameters
-        misp_object = MISPObject("vysion-page")
-        misp_object.template_uuid = "4d0b66f1-5268-47e0-9d29-f2e4f3db8e7f"
-
-        page_id = page.id
-        misp_object.add_attribute("id", type="text", value=page_id)
-
-        url: URL = page.url
-        misp_object.add_attribute("url", type="url", value=url.build())
-
-        network = url.network
-        misp_object.add_attribute("network", type="text", value=network)
-
-        title = page.title
-        misp_object.add_attribute("title", type="text", value=title)
-
-        if ref_attribute is not None:
-            misp_object.add_reference(ref_attribute.uuid, "associated-to")
-  
-        self.misp_event.add_object(misp_object)
-
-        vysion_reference_id = misp_object.uuid
-
-        # TODO Remove this addition when the vysion-page object works
-        self.misp_event.add_attribute("url", value=url.build())
-
-        self.misp_event.add_attribute("domain", value=url.domain)
-
-        for email in hit.email:
-            self.misp_event.add_attribute("email", value=email.value)
-
-        for btc in hit.bitcoin_address:
-            self.misp_event.add_attribute("btc", value=btc.value)
-
-        for dot in hit.polkadot_address:
-            self.misp_event.add_attribute("dot", value=dot.value)
-
-        for eth in hit.ethereum_address:
-            self.misp_event.add_attribute("eth", value=eth.value)
-
-        for xmr in hit.monero_address:
-            self.misp_event.add_attribute("xmr", value=xmr.value)
-
-        for xrp in hit.ripple_address:
-            self.misp_event.add_attribute("xrp", value=xmr.value)
-
-        for zec in hit.zcash_address:
-            self.misp_event.add_attribute("zec", value=zec.value)
-
-        for tag in hit.tag:
-            self.misp_event.add_tag(str(tag))
-
-    def parse_ransom_feed_hit(self, hit: RansomFeedHit, **kwargs):
-
-        # TODO Add event info!
-
-        misp_object = MISPObject("vysion-ransomware-feed")
-        misp_object.template_uuid = "e0bfa994-c184-4894-bfaa-73b1350746e1"
-        misp_object["meta-category"] = "misc" # TODO Esto se tiene que poder hacer de otra manera... Y sólo es necesario en los feeds
-
-        misp_object.add_attribute("id", type="text", value=hit.id)
-        misp_object.add_attribute("company", type="target-org", value=hit.company)
-        misp_object.add_attribute("company_link", type="link", value=hit.company_link)
-        misp_object.add_attribute("link", type="link", value=hit.link)
-        misp_object.add_attribute("group", type="threat-actor", value=hit.group)
-        misp_object.add_attribute("date", type="datetime", value=hit.date)
-        misp_object.add_attribute("info", type="text", value=hit.info)
-        misp_object.add_attribute("country", type="text", value=hit.country)
-
-        self.misp_event.add_object(misp_object)
-
-    def process(self, result: dto.Result, **kwargs) -> MISPEvent:
-
-        processor = {
-            Hit: self.parse_hit,
-            RansomFeedHit: self.parse_ransom_feed_hit,
-        }.get(result.get_type(), lambda *_, **__: {})
-
-        for hit in result.hits:
-            processor(hit, **kwargs)
-
-        return self.misp_event
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+import json
+from pymisp import MISPAttribute, MISPEvent, MISPObject, MISPTag
+
+try:
+    from types import NoneType
+except:
+    NoneType = type(None)
+
+import vysion.dto as dto
+from vysion.dto import Hit, RansomFeedHit, Page, URL
+
+
+class MISPProcessor:
+
+    def __init__(self):
+        self.misp_event = MISPEvent()
+
+    def parse_hit(self, hit: Hit, ref_attribute: MISPAttribute = None, **_):
+
+        page: Page = hit.page
+
+        # TODO Add more page parameters
+        misp_object = MISPObject("vysion-page")
+        misp_object.template_uuid = "4d0b66f1-5268-47e0-9d29-f2e4f3db8e7f"
+
+        page_id = page.id
+        misp_object.add_attribute("id", type="text", value=page_id)
+
+        url: URL = page.url
+        misp_object.add_attribute("url", type="url", value=url.build())
+
+        network = url.network
+        misp_object.add_attribute("network", type="text", value=network)
+
+        title = page.title
+        misp_object.add_attribute("title", type="text", value=title)
+
+        if ref_attribute is not None:
+            misp_object.add_reference(ref_attribute.uuid, "associated-to")
+  
+        self.misp_event.add_object(misp_object)
+
+        vysion_reference_id = misp_object.uuid
+
+        # TODO Remove this addition when the vysion-page object works
+        self.misp_event.add_attribute("url", value=url.build())
+
+        self.misp_event.add_attribute("domain", value=url.domain)
+
+        for email in hit.email:
+            self.misp_event.add_attribute("email", value=email.value)
+
+        for btc in hit.bitcoin_address:
+            self.misp_event.add_attribute("btc", value=btc.value)
+
+        for dot in hit.polkadot_address:
+            self.misp_event.add_attribute("dot", value=dot.value)
+
+        for eth in hit.ethereum_address:
+            self.misp_event.add_attribute("eth", value=eth.value)
+
+        for xmr in hit.monero_address:
+            self.misp_event.add_attribute("xmr", value=xmr.value)
+
+        for xrp in hit.ripple_address:
+            self.misp_event.add_attribute("xrp", value=xmr.value)
+
+        for zec in hit.zcash_address:
+            self.misp_event.add_attribute("zec", value=zec.value)
+
+        for tag in hit.tag:
+            self.misp_event.add_tag(str(tag))
+
+    def parse_ransom_feed_hit(self, hit: RansomFeedHit, **kwargs):
+
+        # TODO Add event info!
+
+        misp_object = MISPObject("vysion-ransomware-feed")
+        misp_object.template_uuid = "e0bfa994-c184-4894-bfaa-73b1350746e1"
+        misp_object["meta-category"] = "misc" # TODO Esto se tiene que poder hacer de otra manera... Y sólo es necesario en los feeds
+
+        misp_object.add_attribute("id", type="text", value=hit.id)
+        misp_object.add_attribute("company", type="target-org", value=hit.company)
+        misp_object.add_attribute("company_link", type="link", value=hit.company_link)
+        misp_object.add_attribute("link", type="link", value=hit.link)
+        misp_object.add_attribute("group", type="threat-actor", value=hit.group)
+        misp_object.add_attribute("date", type="datetime", value=hit.date)
+        misp_object.add_attribute("info", type="text", value=hit.info)
+        misp_object.add_attribute("country", type="text", value=hit.country)
+
+        self.misp_event.add_object(misp_object)
+
+    def process(self, result: dto.Result, **kwargs) -> MISPEvent:
+
+        processor = {
+            Hit: self.parse_hit,
+            RansomFeedHit: self.parse_ransom_feed_hit,
+        }.get(result.get_type(), lambda *_, **__: {})
+
+        for hit in result.hits:
+            processor(hit, **kwargs)
+
+        return self.misp_event
```

### Comparing `vysion-1.0.3/vysion/model/__init__.py` & `vysion-1.0.4/vysion/dto/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-from .model import *
-from . import enum
+#!/usr/bin/env python3
+"""
+Copyright 2022 ByronLabs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+from .dto import *
```

### Comparing `vysion-1.0.3/vysion/model/enum/languages.py` & `vysion-1.0.4/vysion/model/enum/languages.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,210 +1,211 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from enum import Enum
-
-
-class Language(str, Enum):
-
-    """
-    Using names from ISO 639-1
-    """
-
-    avaric = "av"
-    swati = "ss"
-    russian = "ru"
-    lingala = "ln"
-    afar = "aa"
-    mongolian = "mn"
-    tahitian = "ty"
-    somali = "so"
-    gaelic = "gd"
-    uighur = "ug"
-    pushto = "ps"
-    akan = "ak"
-    abkhazian = "ab"
-    tamil = "ta"
-    micmac = "Mi"
-    kannada = "kn"
-    cree = "cr"
-    ndonga = "ng"
-    aymara = "ay"
-    italian = "it"
-    latvian = "lv"
-    ukrainian = "uk"
-    malay = "ms"
-    ganda = "lg"
-    finnish = "fi"
-    tswana = "tn"
-    telugu = "te"
-    chuvash = "cv"
-    ewe = "ee"
-    azerbaijani = "az"
-    lao = "lo"
-    sindhi = "sd"
-    sardinian = "sc"
-    thai = "th"
-    haitian = "ht"
-    bihariLanguages = "bh"
-    romansh = "rm"
-    bashkir = "ba"
-    volapük = "vo"
-    yiddish = "yi"
-    guarani = "gn"
-    croatian = "hr"
-    bambara = "bm"
-    belarusian = "be"
-    sundanese = "su"
-    kongo = "kg"
-    kirghiz = "ky"
-    nepali = "ne"
-    icelandic = "is"
-    herero = "hz"
-    lithuanian = "lt"
-    fulah = "ff"
-    swahili = "sw"
-    manx = "gv"
-    marathi = "mr"
-    sinhala = "si"
-    tajik = "tg"
-    marshallese = "mh"
-    aragonese = "an"
-    dutch = "nl"
-    hindi = "hi"
-    ido = "io"
-    tagalog = "tl"
-    japanese = "ja"
-    centralKhmer = "km"
-    greek = "el"
-    maori = "mi"
-    luxembourgish = "lb"
-    slovenian = "sl"
-    maltese = "mt"
-    kikuyu = "ki"
-    tatar = "tt"
-    lubaKatanga = "lu"
-    swedish = "sv"
-    panjabi = "pa"
-    kashmiri = "ks"
-    divehi = "dv"
-    indonesian = "id"
-    malagasy = "mg"
-    oriya = "or"
-    kuanyama = "kj"
-    sango = "sg"
-    westernFrisian = "fy"
-    zhuang = "za"
-    arabic = "ar"
-    afrikaans = "af"
-    cornish = "kw"
-    xhosa = "xh"
-    armenian = "hy"
-    malayalam = "ml"
-    sotho = "st"
-    esperanto = "eo"
-    latin = "la"
-    korean = "ko"
-    interlingua = "ia"
-    albanian = "sq"
-    catalan = "ca"
-    norwegianNynorsk = "nn"
-    galician = "gl"
-    kurdish = "ku"
-    igbo = "ig"
-    twi = "tw"
-    inuktitut = "iu"
-    hungarian = "hu"
-    yoruba = "yo"
-    tsonga = "ts"
-    slovak = "sk"
-    dzongkha = "dz"
-    churchSlavicc = "cu"
-    quechua = "qu"
-    romanian = "ro"
-    fijian = "fj"
-    chechen = "ce"
-    amharic = "am"
-    burmese = "my"
-    gujarati = "gu"
-    samoan = "sm"
-    chamorro = "ch"
-    irish = "ga"
-    french = "fr"
-    ndebele = "nd"
-    pali = "pi"
-    vietnamese = "vi"
-    kazakh = "kk"
-    navajo = "nv"
-    inupiaq = "ik"
-    avestan = "ae"
-    nauru = "na"
-    danish = "da"
-    breton = "br"
-    persian = "fa"
-    serbian = "sr"
-    georgian = "ka"
-    english = "en"
-    sichuanYi = "ii"
-    oromo = "om"
-    northernSami = "se"
-    venda = "ve"
-    chinese = "zh"
-    norwegian = "no"
-    interlingue = "ie"
-    rundi = "rn"
-    bislama = "bi"
-    hiriMotu = "ho"
-    faroese = "fo"
-    shona = "sn"
-    bengali = "bn"
-    kalaallisut = "kl"
-    bokmål = "nb"
-    occitan = ("oc",)
-    polish = "pl"
-    bulgarian = "bg"
-    assamese = "as"
-    limburgan = "li"
-    turkish = "tr"
-    zulu = "zu"
-    corsican = "co"
-    kanuri = "kr"
-    ojibwa = "oj"
-    tonga = ("to",)
-    sanskrit = "sa"
-    hebrew = "he"
-    wolof = "wo"
-    kinyarwanda = "rw"
-    turkmen = "tk"
-    uzbek = "uz"
-    ossetian = "os"
-    tibetan = "bo"
-    komi = "kv"
-    portuguese = "pt"
-    macedonian = "mk"
-    javanese = "jv"
-    basque = "eu"
-    urdu = "ur"
-    tigrinya = "ti"
-    bosnian = "bs"
-    estonian = "et"
-    hausa = "ha"
-    walloon = "wa"
-    welsh = "cy"
-    czech = "cs"
-    german = "de"
-    spanish = "es"
-
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from enum import Enum
+
+
+class Language(str, Enum):
+
+    """
+    Using names from ISO 639-1
+    """
+
+    avaric = "av"
+    swati = "ss"
+    russian = "ru"
+    lingala = "ln"
+    afar = "aa"
+    mongolian = "mn"
+    tahitian = "ty"
+    somali = "so"
+    gaelic = "gd"
+    uighur = "ug"
+    pushto = "ps"
+    akan = "ak"
+    abkhazian = "ab"
+    tamil = "ta"
+    micmac = "Mi"
+    kannada = "kn"
+    cree = "cr"
+    ndonga = "ng"
+    aymara = "ay"
+    italian = "it"
+    latvian = "lv"
+    ukrainian = "uk"
+    malay = "ms"
+    ganda = "lg"
+    finnish = "fi"
+    tswana = "tn"
+    telugu = "te"
+    chuvash = "cv"
+    ewe = "ee"
+    azerbaijani = "az"
+    lao = "lo"
+    sindhi = "sd"
+    sardinian = "sc"
+    thai = "th"
+    haitian = "ht"
+    bihariLanguages = "bh"
+    romansh = "rm"
+    bashkir = "ba"
+    volapük = "vo"
+    yiddish = "yi"
+    guarani = "gn"
+    croatian = "hr"
+    bambara = "bm"
+    belarusian = "be"
+    sundanese = "su"
+    kongo = "kg"
+    kirghiz = "ky"
+    nepali = "ne"
+    icelandic = "is"
+    herero = "hz"
+    lithuanian = "lt"
+    fulah = "ff"
+    swahili = "sw"
+    manx = "gv"
+    marathi = "mr"
+    sinhala = "si"
+    tajik = "tg"
+    marshallese = "mh"
+    aragonese = "an"
+    dutch = "nl"
+    hindi = "hi"
+    ido = "io"
+    tagalog = "tl"
+    japanese = "ja"
+    centralKhmer = "km"
+    greek = "el"
+    maori = "mi"
+    luxembourgish = "lb"
+    slovenian = "sl"
+    maltese = "mt"
+    kikuyu = "ki"
+    tatar = "tt"
+    lubaKatanga = "lu"
+    swedish = "sv"
+    panjabi = "pa"
+    kashmiri = "ks"
+    divehi = "dv"
+    indonesian = "id"
+    malagasy = "mg"
+    oriya = "or"
+    kuanyama = "kj"
+    sango = "sg"
+    westernFrisian = "fy"
+    zhuang = "za"
+    arabic = "ar"
+    afrikaans = "af"
+    cornish = "kw"
+    xhosa = "xh"
+    armenian = "hy"
+    malayalam = "ml"
+    sotho = "st"
+    esperanto = "eo"
+    latin = "la"
+    korean = "ko"
+    interlingua = "ia"
+    albanian = "sq"
+    catalan = "ca"
+    norwegianNynorsk = "nn"
+    galician = "gl"
+    kurdish = "ku"
+    igbo = "ig"
+    twi = "tw"
+    inuktitut = "iu"
+    hungarian = "hu"
+    yoruba = "yo"
+    tsonga = "ts"
+    slovak = "sk"
+    dzongkha = "dz"
+    churchSlavicc = "cu"
+    quechua = "qu"
+    romanian = "ro"
+    fijian = "fj"
+    chechen = "ce"
+    amharic = "am"
+    burmese = "my"
+    gujarati = "gu"
+    samoan = "sm"
+    chamorro = "ch"
+    irish = "ga"
+    french = "fr"
+    ndebele = "nd"
+    pali = "pi"
+    vietnamese = "vi"
+    kazakh = "kk"
+    navajo = "nv"
+    inupiaq = "ik"
+    avestan = "ae"
+    nauru = "na"
+    danish = "da"
+    breton = "br"
+    persian = "fa"
+    serbian = "sr"
+    georgian = "ka"
+    english = "en"
+    sichuanYi = "ii"
+    oromo = "om"
+    northernSami = "se"
+    venda = "ve"
+    chinese = "zh"
+    norwegian = "no"
+    interlingue = "ie"
+    rundi = "rn"
+    bislama = "bi"
+    hiriMotu = "ho"
+    faroese = "fo"
+    shona = "sn"
+    bengali = "bn"
+    kalaallisut = "kl"
+    bokmål = "nb"
+    occitan = ("oc",)
+    polish = "pl"
+    bulgarian = "bg"
+    assamese = "as"
+    limburgan = "li"
+    turkish = "tr"
+    zulu = "zu"
+    corsican = "co"
+    kanuri = "kr"
+    ojibwa = "oj"
+    tonga = ("to",)
+    sanskrit = "sa"
+    hebrew = "he"
+    wolof = "wo"
+    kinyarwanda = "rw"
+    turkmen = "tk"
+    uzbek = "uz"
+    ossetian = "os"
+    tibetan = "bo"
+    komi = "kv"
+    portuguese = "pt"
+    macedonian = "mk"
+    javanese = "jv"
+    basque = "eu"
+    urdu = "ur"
+    tigrinya = "ti"
+    bosnian = "bs"
+    estonian = "et"
+    hausa = "ha"
+    walloon = "wa"
+    welsh = "cy"
+    czech = "cs"
+    german = "de"
+    spanish = "es"
+    cotedivoire = "ci"
+
```

### Comparing `vysion-1.0.3/vysion/model/enum/networks.py` & `vysion-1.0.4/vysion/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,18 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from enum import Enum
-
-
-class Network(str, Enum):
-
-    tor = "tor"
-    i2p = "i2p"
-    zeronet = "zeronet"
-    freenet = "freenet"
-    paste = "paste"
-    clearnet = "clearnet"
-    graynet = "graynet"
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+__version__ = "1.0.0"
```

### Comparing `vysion-1.0.3/vysion/model/enum/services.py` & `vysion-1.0.4/vysion/model/enum/services.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from enum import IntEnum
-
-
-class Services(IntEnum):
-
-    acr_nema = 104
-    afpovertcp = 548
-    afs3_bos = 7007
-    afs3_callback = 7001
-    afs3_fileserver = 7000
-    afs3_kaserver = 7004
-    afs3_prserver = 7002
-    afs3_rmtsys = 7009
-    afs3_update = 7008
-    afs3_vlserver = 7003
-    afs3_volser = 7005
-    amanda = 10080
-    amandaidx = 10082
-    amidxtape = 10083
-    amqp = 5672
-    amqps = 5671
-    asf_rmcp = 623
-    asp = 27374
-    auth = 113
-    babel = 6696
-    bacula_dir = 9101
-    bacula_fd = 9102
-    bacula_sd = 9103
-    bbs = 7000
-    bgp = 179
-    bgpd = 2605
-    biff = 512
-    binkp = 24554
-    bootpc = 68
-    bootps = 67
-    canna = 5680
-    cfengine = 5308
-    chargen = 19
-    cisco_sccp = 2000
-    clc_build_daemon = 8990
-    clearcase = 371
-    cmip_agent = 164
-    cmip_man = 163
-    codaauth2 = 370
-    codasrv = 2432
-    codasrv_se = 2433
-    csync2 = 30865
-    cvspserver = 2401
-    daap = 3689
-    datametrics = 1645
-    daytime = 13
-    db_lsp = 17500
-    dcap = 22125
-    dhcpv6_client = 546
-    dhcpv6_server = 547
-    dicom = 11112
-    dict = 2628
-    dircproxy = 57000
-    discard = 9
-    distcc = 3632
-    domain = 53
-    domain_s = 853
-    echo = 7
-    epmap = 135
-    epmd = 4369
-    exec = 512
-    f5_globalsite = 2792
-    f5_iquery = 4353
-    fax = 4557
-    fido = 60179
-    finger = 79
-    font_service = 7100
-    freeciv = 5556
-    fsp = 21
-    ftp = 21
-    ftp_data = 20
-    ftps = 990
-    ftps_data = 989
-    gdomap = 538
-    gds_db = 3050
-    git = 9418
-    gnunet = 2086
-    gnutella_rtr = 6347
-    gnutella_svc = 6346
-    gopher = 70
-    gpsd = 2947
-    gris = 2135
-    groupwise = 1677
-    gsidcap = 22128
-    gsiftp = 2811
-    gsigatekeeper = 2119
-    hkp = 11371
-    http = 80
-    http_alt = 8080
-    https = 443
-    hylafax = 4559
-    iax = 4569
-    icpv2 = 3130
-    imap2 = 143
-    imaps = 993
-    ingreslock = 1524
-    ipp = 631
-    iprop = 2121
-    ipsec_nat_t = 4500
-    ipx = 213
-    ircd = 6667
-    ircs_u = 6697
-    isakmp = 500
-    iscsi_target = 3260
-    isisd = 2608
-    isns = 3205
-    iso_tsap = 102
-    kamanda = 10081
-    kerberos = 88
-    kerberos4 = 750
-    kerberos_adm = 749
-    kerberos_master = 751
-    kermit = 1649
-    klogin = 543
-    kpasswd = 464
-    krb_prop = 754
-    kshell = 544
-    l2f = 1701
-    ldap = 389
-    ldaps = 636
-    ldp = 646
-    login = 513
-    lotusnote = 1352
-    mailq = 174
-    mdns = 5353
-    microsoft_ds = 445
-    moira_db = 775
-    moira_update = 777
-    moira_ureg = 779
-    mon = 2583
-    ms_sql_m = 1434
-    ms_sql_s = 1433
-    ms_wbt_server = 3389
-    mtn = 4691
-    munin = 4949
-    mysql = 3306
-    mysql_proxy = 6446
-    nbd = 10809
-    nbp = 2
-    netbios_dgm = 138
-    netbios_ns = 137
-    netbios_ssn = 139
-    netstat = 15
-    nfs = 2049
-    nntp = 119
-    nntps = 563
-    nqs = 607
-    nrpe = 5666
-    nsca = 5667
-    ntalk = 518
-    ntp = 123
-    ntske = 4460
-    nut = 3493
-    omniorb = 8088
-    openvpn = 1194
-    ospf6d = 2606
-    ospfapi = 2607
-    ospfd = 2604
-    passwd_server = 752
-    pawserv = 345
-    pop3 = 110
-    pop3s = 995
-    poppassd = 106
-    postgresql = 5432
-    predict = 1210
-    printer = 515
-    proofd = 1093
-    ptp_event = 319
-    ptp_general = 320
-    puppet = 8140
-    qmqp = 628
-    qmtp = 209
-    qotd = 17
-    radius = 1812
-    radius_acct = 1813
-    radmin_port = 4899
-    redis = 6379
-    remctl = 4373
-    ripd = 2602
-    ripngd = 2603
-    rmiregistry = 1099
-    rmtcfg = 1236
-    rootd = 1094
-    route = 520
-    rpc2portmap = 369
-    rplay = 5555
-    rsync = 873
-    rtcm_sc104 = 2101
-    rtmp = 1
-    rtsp = 554
-    saft = 487
-    sa_msg_port = 1646
-    sane_port = 6566
-    sge_execd = 6445
-    sge_qmaster = 6444
-    sgi_cad = 17004
-    sgi_cmsd = 17001
-    sgi_crsd = 17002
-    sgi_gcd = 17003
-    shell = 514
-    sieve = 4190
-    silc = 706
-    sip = 5060
-    sip_tls = 5061
-    skkserv = 1178
-    smtp = 25
-    smux = 199
-    snmp = 161
-    snmp_trap = 162
-    snpp = 444
-    socks = 1080
-    spamd = 783
-    ssh = 22
-    submission = 587
-    submissions = 465
-    sunrpc = 111
-    supfiledbg = 1127
-    supfilesrv = 871
-    suucp = 4031
-    svn = 3690
-    svrloc = 427
-    syslog = 514
-    syslog_tls = 6514
-    sysrqd = 4094
-    systat = 11
-    tacacs = 49
-    talk = 517
-    tcpmux = 1
-    telnet = 23
-    telnets = 992
-    tfido = 60177
-    tftp = 69
-    time = 37
-    tinc = 655
-    tproxy = 8081
-    uucp = 540
-    venus = 2430
-    venus_se = 2431
-    webmin = 10000
-    who = 513
-    whois = 43
-    wnn6 = 22273
-    x11 = 6000
-    x11_1 = 6001
-    x11_2 = 6002
-    x11_3 = 6003
-    x11_4 = 6004
-    x11_5 = 6005
-    x11_6 = 6006
-    x11_7 = 6007
-    xdmcp = 177
-    xinetd = 9098
-    xmms2 = 9667
-    xmpp_client = 5222
-    xmpp_server = 5269
-    xtel = 1313
-    xtelw = 1314
-    z3950 = 210
-    zabbix_agent = 10050
-    zabbix_trapper = 10051
-    zebra = 2601
-    zebrasrv = 2600
-    zephyr_clt = 2103
-    zephyr_hm = 2104
-    zephyr_srv = 2102
-    zip = 6
-    zope = 9673
-    zope_ftp = 8021
-    zserv = 346
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from enum import IntEnum
+
+
+class Services(IntEnum):
+
+    acr_nema = 104
+    afpovertcp = 548
+    afs3_bos = 7007
+    afs3_callback = 7001
+    afs3_fileserver = 7000
+    afs3_kaserver = 7004
+    afs3_prserver = 7002
+    afs3_rmtsys = 7009
+    afs3_update = 7008
+    afs3_vlserver = 7003
+    afs3_volser = 7005
+    amanda = 10080
+    amandaidx = 10082
+    amidxtape = 10083
+    amqp = 5672
+    amqps = 5671
+    asf_rmcp = 623
+    asp = 27374
+    auth = 113
+    babel = 6696
+    bacula_dir = 9101
+    bacula_fd = 9102
+    bacula_sd = 9103
+    bbs = 7000
+    bgp = 179
+    bgpd = 2605
+    biff = 512
+    binkp = 24554
+    bootpc = 68
+    bootps = 67
+    canna = 5680
+    cfengine = 5308
+    chargen = 19
+    cisco_sccp = 2000
+    clc_build_daemon = 8990
+    clearcase = 371
+    cmip_agent = 164
+    cmip_man = 163
+    codaauth2 = 370
+    codasrv = 2432
+    codasrv_se = 2433
+    csync2 = 30865
+    cvspserver = 2401
+    daap = 3689
+    datametrics = 1645
+    daytime = 13
+    db_lsp = 17500
+    dcap = 22125
+    dhcpv6_client = 546
+    dhcpv6_server = 547
+    dicom = 11112
+    dict = 2628
+    dircproxy = 57000
+    discard = 9
+    distcc = 3632
+    domain = 53
+    domain_s = 853
+    echo = 7
+    epmap = 135
+    epmd = 4369
+    exec = 512
+    f5_globalsite = 2792
+    f5_iquery = 4353
+    fax = 4557
+    fido = 60179
+    finger = 79
+    font_service = 7100
+    freeciv = 5556
+    fsp = 21
+    ftp = 21
+    ftp_data = 20
+    ftps = 990
+    ftps_data = 989
+    gdomap = 538
+    gds_db = 3050
+    git = 9418
+    gnunet = 2086
+    gnutella_rtr = 6347
+    gnutella_svc = 6346
+    gopher = 70
+    gpsd = 2947
+    gris = 2135
+    groupwise = 1677
+    gsidcap = 22128
+    gsiftp = 2811
+    gsigatekeeper = 2119
+    hkp = 11371
+    http = 80
+    http_alt = 8080
+    https = 443
+    hylafax = 4559
+    iax = 4569
+    icpv2 = 3130
+    imap2 = 143
+    imaps = 993
+    ingreslock = 1524
+    ipp = 631
+    iprop = 2121
+    ipsec_nat_t = 4500
+    ipx = 213
+    ircd = 6667
+    ircs_u = 6697
+    isakmp = 500
+    iscsi_target = 3260
+    isisd = 2608
+    isns = 3205
+    iso_tsap = 102
+    kamanda = 10081
+    kerberos = 88
+    kerberos4 = 750
+    kerberos_adm = 749
+    kerberos_master = 751
+    kermit = 1649
+    klogin = 543
+    kpasswd = 464
+    krb_prop = 754
+    kshell = 544
+    l2f = 1701
+    ldap = 389
+    ldaps = 636
+    ldp = 646
+    login = 513
+    lotusnote = 1352
+    mailq = 174
+    mdns = 5353
+    microsoft_ds = 445
+    moira_db = 775
+    moira_update = 777
+    moira_ureg = 779
+    mon = 2583
+    ms_sql_m = 1434
+    ms_sql_s = 1433
+    ms_wbt_server = 3389
+    mtn = 4691
+    munin = 4949
+    mysql = 3306
+    mysql_proxy = 6446
+    nbd = 10809
+    nbp = 2
+    netbios_dgm = 138
+    netbios_ns = 137
+    netbios_ssn = 139
+    netstat = 15
+    nfs = 2049
+    nntp = 119
+    nntps = 563
+    nqs = 607
+    nrpe = 5666
+    nsca = 5667
+    ntalk = 518
+    ntp = 123
+    ntske = 4460
+    nut = 3493
+    omniorb = 8088
+    openvpn = 1194
+    ospf6d = 2606
+    ospfapi = 2607
+    ospfd = 2604
+    passwd_server = 752
+    pawserv = 345
+    pop3 = 110
+    pop3s = 995
+    poppassd = 106
+    postgresql = 5432
+    predict = 1210
+    printer = 515
+    proofd = 1093
+    ptp_event = 319
+    ptp_general = 320
+    puppet = 8140
+    qmqp = 628
+    qmtp = 209
+    qotd = 17
+    radius = 1812
+    radius_acct = 1813
+    radmin_port = 4899
+    redis = 6379
+    remctl = 4373
+    ripd = 2602
+    ripngd = 2603
+    rmiregistry = 1099
+    rmtcfg = 1236
+    rootd = 1094
+    route = 520
+    rpc2portmap = 369
+    rplay = 5555
+    rsync = 873
+    rtcm_sc104 = 2101
+    rtmp = 1
+    rtsp = 554
+    saft = 487
+    sa_msg_port = 1646
+    sane_port = 6566
+    sge_execd = 6445
+    sge_qmaster = 6444
+    sgi_cad = 17004
+    sgi_cmsd = 17001
+    sgi_crsd = 17002
+    sgi_gcd = 17003
+    shell = 514
+    sieve = 4190
+    silc = 706
+    sip = 5060
+    sip_tls = 5061
+    skkserv = 1178
+    smtp = 25
+    smux = 199
+    snmp = 161
+    snmp_trap = 162
+    snpp = 444
+    socks = 1080
+    spamd = 783
+    ssh = 22
+    submission = 587
+    submissions = 465
+    sunrpc = 111
+    supfiledbg = 1127
+    supfilesrv = 871
+    suucp = 4031
+    svn = 3690
+    svrloc = 427
+    syslog = 514
+    syslog_tls = 6514
+    sysrqd = 4094
+    systat = 11
+    tacacs = 49
+    talk = 517
+    tcpmux = 1
+    telnet = 23
+    telnets = 992
+    tfido = 60177
+    tftp = 69
+    time = 37
+    tinc = 655
+    tproxy = 8081
+    uucp = 540
+    venus = 2430
+    venus_se = 2431
+    webmin = 10000
+    who = 513
+    whois = 43
+    wnn6 = 22273
+    x11 = 6000
+    x11_1 = 6001
+    x11_2 = 6002
+    x11_3 = 6003
+    x11_4 = 6004
+    x11_5 = 6005
+    x11_6 = 6006
+    x11_7 = 6007
+    xdmcp = 177
+    xinetd = 9098
+    xmms2 = 9667
+    xmpp_client = 5222
+    xmpp_server = 5269
+    xtel = 1313
+    xtelw = 1314
+    z3950 = 210
+    zabbix_agent = 10050
+    zabbix_trapper = 10051
+    zebra = 2601
+    zebrasrv = 2600
+    zephyr_clt = 2103
+    zephyr_hm = 2104
+    zephyr_srv = 2102
+    zip = 6
+    zope = 9673
+    zope_ftp = 8021
+    zserv = 346
```

### Comparing `vysion-1.0.3/vysion/model/model.py` & `vysion-1.0.4/vysion/model/model.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 ByronLabs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-from .enum import Enum
-import hashlib
-import uuid
-from datetime import datetime
-
-try:
-    from types import NoneType
-except:
-    NoneType: type = type(None)
-
-from typing import List, Optional, Union
-
-from pydantic import BaseModel, Field # , constr
-
-from .enum import Services, Network
-
-import re
-
-NULL_UUID = uuid.UUID("00000000-0000-0000-0000-000000000000")
-
-class URL(BaseModel):
-
-    protocol: Optional[str] 
-    domain: Optional[str]   
-    port: Optional[int] = Field(default_factory=lambda: -1)
-    path: Optional[str]
-    signature: uuid.UUID = Field(default_factory=lambda: NULL_UUID)
-    
-    raw: str
-
-    @staticmethod
-    def _parse_(url):
-        
-        """
-        RFC3986
-            scheme    = $2
-            authority = $4
-            path      = $5
-            query     = $7
-            fragment  = $9
-        """
-        regex = r"^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?"
-        
-        res = re.match(regex, url)
-        
-        scheme = res[2]
-        authority = res[4]
-        path = res[5]
-        query = res[7]
-        fragment = res[9]
-
-        return dict(
-            scheme=scheme,
-            authority=authority,
-            path=path,
-            query=query,
-            fragment=fragment
-        )
-
-    def _generate_signature_(self) -> uuid.UUID:
-        return uuid.uuid5(uuid.NAMESPACE_URL, self.build())
-
-    @classmethod
-    def parse(cls, url, fix=False):
-
-        # Saving the original url
-        raw = url
-
-        parsed = cls._parse_(url)
-        
-        # Elements
-        scheme = parsed["scheme"]
-        netloc = parsed["authority"]
-        path = parsed["path"]
-        query = parsed["query"]
-        fragment = parsed["fragment"]
-
-        # Build domain:port
-        if netloc is not None:
-            domain_port = (netloc.split(":") + [None])[:2]
-        else:
-            domain_port = [None, None]
-        
-        domain = domain_port[0]
-        port = domain_port[1]
-
-        # Normalize path: /path?query#fragment
-        # Parse a URL into 6 components:
-        # <protocol>://<domain>:<port>/<path>
-        if query is not None:
-
-            # Normalize query
-            query_parts = [param.split("=") for param in query.split("&")]
-            query_dict = {}
-            for part in query_parts:
-                if len(part) <= 1:
-                    query_dict[part[0]] = str()
-                else:
-                    query_dict[part[0]] = part[1]
-
-            query_keys = list(query_dict.keys())
-            query_keys.sort()
-            res_query_parts = [f"{k}={query_dict[k]}" for k in query_keys]
-
-            res_query = "?" + "&".join(res_query_parts)
-        
-            path += res_query
-        
-        if fragment is not None:
-            path += f"#{fragment}"
-
-        # TODO Adapt restalker.link_extractors.UUF logic to fix URLs
-        # TODO Detect network?
-        result = cls(
-            protocol=scheme,
-            domain=domain,
-            port=port,
-            path=path,
-            raw=raw
-        )
-
-        if fix:
-            result._fix()
-
-        return result
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.signature = self._generate_signature_()
-
-    def build(self) -> str:
-        
-        url = self.path
-
-        if self.domain is not None:
-            
-            if self.port is not None:
-                url = f":{self.port}" + url
-            
-            url = f"{self.domain}" + url
-
-        if self.protocol is not None:
-
-            url = f"{self.protocol}://" + url
-            
-        return url
-
-    def _fix(self, default_protocol=Services.http) -> None:
-
-        if self.protocol is None:
-            if self.port is None:
-                self.protocol = default_protocol.name
-            else:
-                self.protocol = Services(self.port).name
-
-        if self.port is None:
-            self.port = Services[self.protocol].value
-
-        if self.domain is None:
-            path = self.path
-            if path[0] == "/":
-                path = path[1:]
-            path_parts = path.split('/')
-            self.domain = path_parts[0]
-            self.path = "/" + "/".join(path_parts[1:])
-        
-        self.signature = self._generate_signature_()
-
-    def __str__(self) -> str:
-        return self.build()
-
-    def __repr__(self):
-        return self.build()
+#!/usr/bin/env python3
+"""
+Copyright 2022 ByronLabs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+from .enum import Enum
+import hashlib
+import uuid
+from datetime import datetime
+
+try:
+    from types import NoneType
+except:
+    NoneType: type = type(None)
+
+from typing import List, Optional, Union
+
+from pydantic import BaseModel, Field # , constr
+
+from .enum import Services, Network
+
+import re
+
+NULL_UUID = uuid.UUID("00000000-0000-0000-0000-000000000000")
+
+class URL(BaseModel):
+
+    protocol: Optional[str] 
+    domain: Optional[str]   
+    port: Optional[int] = Field(default_factory=lambda: -1)
+    path: Optional[str]
+    signature: uuid.UUID = Field(default_factory=lambda: NULL_UUID)
+    
+    raw: str
+
+    @staticmethod
+    def _parse_(url):
+        
+        """
+        RFC3986
+            scheme    = $2
+            authority = $4
+            path      = $5
+            query     = $7
+            fragment  = $9
+        """
+        regex = r"^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?"
+        
+        res = re.match(regex, url)
+        
+        scheme = res[2]
+        authority = res[4]
+        path = res[5]
+        query = res[7]
+        fragment = res[9]
+
+        return dict(
+            scheme=scheme,
+            authority=authority,
+            path=path,
+            query=query,
+            fragment=fragment
+        )
+
+    def _generate_signature_(self) -> uuid.UUID:
+        return uuid.uuid5(uuid.NAMESPACE_URL, self.build())
+
+    @classmethod
+    def parse(cls, url, fix=False):
+
+        # Saving the original url
+        raw = url
+
+        parsed = cls._parse_(url)
+        
+        # Elements
+        scheme = parsed["scheme"]
+        netloc = parsed["authority"]
+        path = parsed["path"]
+        query = parsed["query"]
+        fragment = parsed["fragment"]
+
+        # Build domain:port
+        if netloc is not None:
+            domain_port = (netloc.split(":") + [None])[:2]
+        else:
+            domain_port = [None, None]
+        
+        domain = domain_port[0]
+        port = domain_port[1]
+
+        # Normalize path: /path?query#fragment
+        # Parse a URL into 6 components:
+        # <protocol>://<domain>:<port>/<path>
+        if query is not None:
+
+            # Normalize query
+            query_parts = [param.split("=") for param in query.split("&")]
+            query_dict = {}
+            for part in query_parts:
+                if len(part) <= 1:
+                    query_dict[part[0]] = str()
+                else:
+                    query_dict[part[0]] = part[1]
+
+            query_keys = list(query_dict.keys())
+            query_keys.sort()
+            res_query_parts = [f"{k}={query_dict[k]}" for k in query_keys]
+
+            res_query = "?" + "&".join(res_query_parts)
+        
+            path += res_query
+        
+        if fragment is not None:
+            path += f"#{fragment}"
+
+        # TODO Adapt restalker.link_extractors.UUF logic to fix URLs
+        # TODO Detect network?
+        result = cls(
+            protocol=scheme,
+            domain=domain,
+            port=port,
+            path=path,
+            raw=raw
+        )
+
+        if fix:
+            result._fix()
+
+        return result
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.signature = self._generate_signature_()
+
+    def build(self) -> str:
+        
+        url = self.path
+
+        if self.domain is not None:
+            
+            if self.port is not None:
+                url = f":{self.port}" + url
+            
+            url = f"{self.domain}" + url
+
+        if self.protocol is not None:
+
+            url = f"{self.protocol}://" + url
+            
+        return url
+
+    def _fix(self, default_protocol=Services.http) -> None:
+
+        if self.protocol is None:
+            if self.port is None:
+                self.protocol = default_protocol.name
+            else:
+                self.protocol = Services(self.port).name
+
+        if self.port is None:
+            self.port = Services[self.protocol].value
+
+        if self.domain is None:
+            path = self.path
+            if path[0] == "/":
+                path = path[1:]
+            path_parts = path.split('/')
+            self.domain = path_parts[0]
+            self.path = "/" + "/".join(path_parts[1:])
+        
+        self.signature = self._generate_signature_()
+
+    def __str__(self) -> str:
+        return self.build()
+
+    def __repr__(self):
+        return self.build()
```

### Comparing `vysion-1.0.3/vysion/taxonomy/__init__.py` & `vysion-1.0.4/vysion/model/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 Byron Labs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from .taxonomy import *
-from . import flavours
+#!/usr/bin/env python3
+"""
+Copyright 2022 Byron Labs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+from .model import *
+from . import enum
```

### Comparing `vysion-1.0.3/vysion/taxonomy/flavours.py` & `vysion-1.0.4/vysion/taxonomy/flavours.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python3
-"""
-Copyright 2022 ByronLabs S.L.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-
-class Flavour:
-
-    _reference: str = None
-    _version: str = None
-
-    def __init_subclass__(cls) -> None:
-
-        super().__init_subclass__()
-
-        assert cls._reference is not None, f"{cls.__name__} class needs reference field"
-        assert cls._version is not None, f"{cls.__name__} class needs_version field"
-
-    def __init__(self, namespace: str, predicate: str, value: str):
-
-        self._namespace = namespace
-        self.predicate = predicate
-        self.value = value
-
-    def __repr__(self):
-        return f'{self._namespace}:{self.predicate}:"{self.value}"'
-
-
-class EmptyFlavour(Flavour):
-
-    _reference = "nil"
-    _version = "0.0"
-
-    def __init__(self):
-        super().__init__(None, None, None)
-
-
-class DBSafe(Flavour):
-
-    # TODO ¿Por ejemplo?
-    _reference = "https://peps.python.org/pep-0008/#naming-conventions"
-    _version = "2001"
-
-
-class MISP(Flavour):
-
-    _reference = "https://github.com/MISP/misp-taxonomies"
-    _version = "20220609"
-
-
-# class STIX(Flavour):
-#     pass
-
-
-# class CASE(Flavour):
-#     pass
-
-
-class Vysion(Flavour):
-
-    _reference = "api.vysion.io"
-    _version = "0.0.1"
-
-    def __init__(self, namespace, predicate, value, description=None):
-
-        super().__init__(namespace, predicate, value)
-        self.description = description
-
-
-class Flavours:
-    def __init__(self, vysion=None, misp=None, stix=None, case=None, dbsafe=None):
-
-        assert None not in (vysion, misp, stix, case, dbsafe)
-
-        # TODO Each one should contain a list of names?
-        self.vysion = vysion
-        self.misp = misp
-        self.stix = stix
-        self.case = case
-        self.dbsafe = dbsafe
-
-    def get_flavours(self):
-        return [self.vysion, self.misp, self.stix, self.case, self.dbsafe]
+#!/usr/bin/env python3
+"""
+Copyright 2022 ByronLabs S.L.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+
+class Flavour:
+
+    _reference: str = None
+    _version: str = None
+
+    def __init_subclass__(cls) -> None:
+
+        super().__init_subclass__()
+
+        assert cls._reference is not None, f"{cls.__name__} class needs reference field"
+        assert cls._version is not None, f"{cls.__name__} class needs_version field"
+
+    def __init__(self, namespace: str, predicate: str, value: str):
+
+        self._namespace = namespace
+        self.predicate = predicate
+        self.value = value
+
+    def __repr__(self):
+        return f'{self._namespace}:{self.predicate}:"{self.value}"'
+
+
+class EmptyFlavour(Flavour):
+
+    _reference = "nil"
+    _version = "0.0"
+
+    def __init__(self):
+        super().__init__(None, None, None)
+
+
+class DBSafe(Flavour):
+
+    # TODO ¿Por ejemplo?
+    _reference = "https://peps.python.org/pep-0008/#naming-conventions"
+    _version = "2001"
+
+
+class MISP(Flavour):
+
+    _reference = "https://github.com/MISP/misp-taxonomies"
+    _version = "20220609"
+
+
+# class STIX(Flavour):
+#     pass
+
+
+# class CASE(Flavour):
+#     pass
+
+
+class Vysion(Flavour):
+
+    _reference = "api.vysion.io"
+    _version = "0.0.1"
+
+    def __init__(self, namespace, predicate, value, description=None):
+
+        super().__init__(namespace, predicate, value)
+        self.description = description
+
+
+class Flavours:
+    def __init__(self, vysion=None, misp=None, stix=None, case=None, dbsafe=None):
+
+        assert None not in (vysion, misp, stix, case, dbsafe)
+
+        # TODO Each one should contain a list of names?
+        self.vysion = vysion
+        self.misp = misp
+        self.stix = stix
+        self.case = case
+        self.dbsafe = dbsafe
+
+    def get_flavours(self):
+        return [self.vysion, self.misp, self.stix, self.case, self.dbsafe]
```

### Comparing `vysion-1.0.3/PKG-INFO` & `vysion-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: vysion
-Version: 1.0.3
+Version: 1.0.4
 Summary: The official Python client library for Vysion
 Home-page: https://vysion.ai
 License: Apache-2.0
 Author: Javier Junquera-Sánchez
 Author-email: javier.junquera@byronlabs.io
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: pydantic (==1.10.3)
 Requires-Dist: pymisp (==2.4.159)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: softenum (==1.0.1)
 Project-URL: Documentation, https://developers.vysion.ai
 Project-URL: Repository, https://gitlab.com/byronlabs/vysion/vysion-py
 Description-Content-Type: text/markdown
```

