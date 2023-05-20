# Comparing `tmp/czapi-0.1.7.tar.gz` & `tmp/czapi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czapi-0.1.7.tar", last modified: Sun Apr  2 16:00:49 2023, max compression
+gzip compressed data, was "dist\czapi-0.1.8.tar", last modified: Sat May 20 20:38:44 2023, max compression
```

## Comparing `czapi-0.1.7.tar` & `czapi-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 robertcurrie   (501) staff       (20)        0 2023-04-02 16:00:49.697128 czapi-0.1.7/
--rw-r--r--   0 robertcurrie   (501) staff       (20)     2348 2022-02-03 03:07:19.000000 czapi-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 robertcurrie   (501) staff       (20)    11357 2022-02-03 03:07:19.000000 czapi-0.1.7/LICENSE
--rw-r--r--   0 robertcurrie   (501) staff       (20)      111 2022-02-03 03:07:19.000000 czapi-0.1.7/MANIFEST.in
--rw-r--r--   0 robertcurrie   (501) staff       (20)    34031 2023-04-02 16:00:49.696445 czapi-0.1.7/PKG-INFO
--rw-r--r--   0 robertcurrie   (501) staff       (20)    33297 2023-04-02 12:33:13.000000 czapi-0.1.7/README.md
-drwxr-xr-x   0 robertcurrie   (501) staff       (20)        0 2023-04-02 16:00:49.684175 czapi-0.1.7/czapi/
--rw-r--r--   0 robertcurrie   (501) staff       (20)       22 2023-04-02 16:00:39.000000 czapi-0.1.7/czapi/__init__.py
--rw-r--r--   0 robertcurrie   (501) staff       (20)     1327 2023-04-02 12:33:04.000000 czapi-0.1.7/czapi/_nbdev.py
--rw-r--r--   0 robertcurrie   (501) staff       (20)      208 2023-04-02 12:33:04.000000 czapi-0.1.7/czapi/api.py
-drwxr-xr-x   0 robertcurrie   (501) staff       (20)        0 2023-04-02 16:00:49.693789 czapi-0.1.7/czapi/core/
--rw-r--r--   0 robertcurrie   (501) staff       (20)        0 2022-02-11 23:33:00.000000 czapi-0.1.7/czapi/core/__init__.py
--rw-r--r--   0 robertcurrie   (501) staff       (20)     1112 2023-04-02 12:33:04.000000 czapi-0.1.7/czapi/core/errors.py
-drwxr-xr-x   0 robertcurrie   (501) staff       (20)        0 2023-04-02 16:00:49.695195 czapi-0.1.7/czapi/core/scraping/
--rw-r--r--   0 robertcurrie   (501) staff       (20)        0 2022-02-03 03:07:19.000000 czapi-0.1.7/czapi/core/scraping/__init__.py
--rw-r--r--   0 robertcurrie   (501) staff       (20)    10751 2023-04-02 12:33:04.000000 czapi-0.1.7/czapi/core/scraping/base.py
--rw-r--r--   0 robertcurrie   (501) staff       (20)     1565 2023-04-02 12:33:04.000000 czapi-0.1.7/czapi/core/testing.py
--rw-r--r--   0 robertcurrie   (501) staff       (20)      602 2023-04-02 12:33:04.000000 czapi-0.1.7/czapi/core/utils.py
-drwxr-xr-x   0 robertcurrie   (501) staff       (20)        0 2023-04-02 16:00:49.690748 czapi-0.1.7/czapi.egg-info/
--rw-r--r--   0 robertcurrie   (501) staff       (20)    34031 2023-04-02 16:00:49.000000 czapi-0.1.7/czapi.egg-info/PKG-INFO
--rw-r--r--   0 robertcurrie   (501) staff       (20)      464 2023-04-02 16:00:49.000000 czapi-0.1.7/czapi.egg-info/SOURCES.txt
--rw-r--r--   0 robertcurrie   (501) staff       (20)        1 2023-04-02 16:00:49.000000 czapi-0.1.7/czapi.egg-info/dependency_links.txt
--rw-r--r--   0 robertcurrie   (501) staff       (20)       20 2023-04-02 16:00:49.000000 czapi-0.1.7/czapi.egg-info/entry_points.txt
--rw-r--r--   0 robertcurrie   (501) staff       (20)        1 2023-03-18 14:43:34.000000 czapi-0.1.7/czapi.egg-info/not-zip-safe
--rw-r--r--   0 robertcurrie   (501) staff       (20)       34 2023-04-02 16:00:49.000000 czapi-0.1.7/czapi.egg-info/requires.txt
--rw-r--r--   0 robertcurrie   (501) staff       (20)        6 2023-04-02 16:00:49.000000 czapi-0.1.7/czapi.egg-info/top_level.txt
--rw-r--r--   0 robertcurrie   (501) staff       (20)      585 2023-04-02 16:00:39.000000 czapi-0.1.7/settings.ini
--rw-r--r--   0 robertcurrie   (501) staff       (20)       38 2023-04-02 16:00:49.697333 czapi-0.1.7/setup.cfg
--rw-r--r--   0 robertcurrie   (501) staff       (20)     3094 2022-02-03 03:07:19.000000 czapi-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/
+-rw-rw-rw-   0        0        0     2381 2022-02-26 15:53:17.000000 czapi-0.1.8/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2022-02-26 15:53:17.000000 czapi-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      116 2022-02-26 15:53:17.000000 czapi-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    34990 2023-05-20 20:38:44.000000 czapi-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    34232 2023-05-20 20:34:08.000000 czapi-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi/
+-rw-rw-rw-   0        0        0       23 2023-05-20 20:38:16.000000 czapi-0.1.8/czapi/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/_nbdev.py
+-rw-rw-rw-   0        0        0      249 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/api.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi/core/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:45:51.000000 czapi-0.1.8/czapi/core/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi/core/scraping/
+-rw-rw-rw-   0        0        0        0 2022-12-21 13:02:35.000000 czapi-0.1.8/czapi/core/scraping/__init__.py
+-rw-rw-rw-   0        0        0    11339 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/scraping/base.py
+-rw-rw-rw-   0        0        0     1641 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/testing.py
+-rw-rw-rw-   0        0        0      633 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/
+-rw-rw-rw-   0        0        0    34990 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-02-26 16:04:21.000000 czapi-0.1.8/czapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      612 2023-05-20 20:38:16.000000 czapi-0.1.8/settings.ini
+-rw-rw-rw-   0        0        0       42 2023-05-20 20:38:44.000000 czapi-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     3158 2022-02-26 15:53:17.000000 czapi-0.1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `czapi-0.1.7/CONTRIBUTING.md` & `czapi-0.1.8/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# How to contribute
-
-## How to get started
-
-Before anything else, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:
-```
-nbdev_install_git_hooks
-```
-
-## Did you find a bug?
-
-* Ensure the bug was not already reported by searching on GitHub under Issues.
-* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
-* Be sure to add the complete error messages.
-
-#### Did you write a patch that fixes a bug?
-
-* Open a new GitHub pull request with the patch.
-* Ensure that your PR includes a test that fails without your patch, and pass with it.
-* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
-
-## PR submission guidelines
-
-* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
-* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
-* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
-* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
-* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.
-
-## Do you want to contribute to the documentation?
-
-* Docs are automatically created from the notebooks in the nbs folder.
-
+# How to contribute
+
+## How to get started
+
+Before anything else, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:
+```
+nbdev_install_git_hooks
+```
+
+## Did you find a bug?
+
+* Ensure the bug was not already reported by searching on GitHub under Issues.
+* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
+* Be sure to add the complete error messages.
+
+#### Did you write a patch that fixes a bug?
+
+* Open a new GitHub pull request with the patch.
+* Ensure that your PR includes a test that fails without your patch, and pass with it.
+* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
+
+## PR submission guidelines
+
+* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
+* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
+* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
+* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
+* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.
+
+## Do you want to contribute to the documentation?
+
+* Docs are automatically created from the notebooks in the nbs folder.
+
```

### Comparing `czapi-0.1.7/LICENSE` & `czapi-0.1.8/LICENSE`

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

### Comparing `czapi-0.1.7/czapi/_nbdev.py` & `czapi-0.1.8/czapi/_nbdev.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-# AUTOGENERATED BY NBDEV! DO NOT EDIT!
-
-__all__ = ["index", "modules", "custom_doc_links", "git_url"]
-
-index = {"generate_dict_from_table": "00_base.ipynb",
-         "normalize_scores": "00_base.ipynb",
-         "get_hammer_progressions": "00_base.ipynb",
-         "HalfBoxscore": "00_base.ipynb",
-         "NormalizedHalfBoxscore": "00_base.ipynb",
-         "generate_half_boxscore_pair": "00_base.ipynb",
-         "NormalizedBoxscore": "00_base.ipynb",
-         "Page": "00_base.ipynb",
-         "LinescorePage": "00_base.ipynb",
-         "BadLinescorePage": "00_base.ipynb",
-         "GameData": "00_base.ipynb",
-         "get_flat_boxscores_from": "00_base.ipynb",
-         "Event": "00_base.ipynb",
-         "DifferentScoreLengthError": "02_errors.ipynb",
-         "InvalidScoreError": "02_errors.ipynb",
-         "InvalidEventError": "02_errors.ipynb",
-         "make_request_from": "03_utils.ipynb",
-         "make_soup_from": "03_utils.ipynb",
-         "TagBase": "04_testing.ipynb",
-         "TagLike": "04_testing.ipynb"}
-
-modules = ["core/scraping/base.py",
-           "api.py",
-           "core/errors.py",
-           "core/utils.py",
-           "core/testing.py"]
-
-doc_url = "https://calicorob.github.io/czapi/"
-
-git_url = "https://github.com/calicorob/czapi/tree/master/"
-
-def custom_doc_links(name): return None
+# AUTOGENERATED BY NBDEV! DO NOT EDIT!
+
+__all__ = ["index", "modules", "custom_doc_links", "git_url"]
+
+index = {"generate_dict_from_table": "00_base.ipynb",
+         "normalize_scores": "00_base.ipynb",
+         "get_hammer_progressions": "00_base.ipynb",
+         "HalfBoxscore": "00_base.ipynb",
+         "NormalizedHalfBoxscore": "00_base.ipynb",
+         "generate_half_boxscore_pair": "00_base.ipynb",
+         "NormalizedBoxscore": "00_base.ipynb",
+         "Page": "00_base.ipynb",
+         "LinescorePage": "00_base.ipynb",
+         "BadLinescorePage": "00_base.ipynb",
+         "GameData": "00_base.ipynb",
+         "game_data_column_headers": "00_base.ipynb",
+         "get_flat_boxscores_from": "00_base.ipynb",
+         "Event": "00_base.ipynb",
+         "DifferentScoreLengthError": "02_errors.ipynb",
+         "InvalidScoreError": "02_errors.ipynb",
+         "InvalidEventError": "02_errors.ipynb",
+         "make_request_from": "03_utils.ipynb",
+         "make_soup_from": "03_utils.ipynb",
+         "TagBase": "04_testing.ipynb",
+         "TagLike": "04_testing.ipynb"}
+
+modules = ["core/scraping/base.py",
+           "api.py",
+           "core/errors.py",
+           "core/utils.py",
+           "core/testing.py"]
+
+doc_url = "https://calicorob.github.io/czapi/"
+
+git_url = "https://github.com/calicorob/czapi/tree/master/"
+
+def custom_doc_links(name): return None
```

### Comparing `czapi-0.1.7/czapi/core/errors.py` & `czapi-0.1.8/czapi/core/errors.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/02_errors.ipynb (unless otherwise specified).
-
-__all__ = []
-
-# Internal Cell
-
-class DifferentScoreLengthError(Exception):
-    def __init__(self,score_1_len:int,score_2_len)->None:
-        self.score_1_len = score_1_len
-        self.score_2_len = score_2_len
-
-        self.message = "Input scores have length %s and length %s and do not match."%(self.score_1_len,self.score_2_len)
-        super().__init__(self.message)
-
-class InvalidScoreError(Exception):
-    def __init__(self,idx:int,val_1:int,val_2:int)->None:
-
-        self.idx = idx
-        self.val_1 = val_1
-        self.val_2 = val_2
-        self.message = "Input end scores of %s and %s for end %s are both greater than 0 and the end score is not valid."%(self.val_1,self.val_2,self.idx)
-        super().__init__(self.message)
-
-class InvalidEventError(Exception):
-    def __init__(self,cz_event_id:int)->None:
-        self.cz_event_id = cz_event_id
-
-        self.message = "Inputted Event ID of %s is not valid, please check you have the right one."%self.cz_event_id
+# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/02_errors.ipynb (unless otherwise specified).
+
+__all__ = []
+
+# Internal Cell
+
+class DifferentScoreLengthError(Exception):
+    def __init__(self,score_1_len:int,score_2_len)->None:
+        self.score_1_len = score_1_len
+        self.score_2_len = score_2_len
+
+        self.message = "Input scores have length %s and length %s and do not match."%(self.score_1_len,self.score_2_len)
+        super().__init__(self.message)
+
+class InvalidScoreError(Exception):
+    def __init__(self,idx:int,val_1:int,val_2:int)->None:
+
+        self.idx = idx
+        self.val_1 = val_1
+        self.val_2 = val_2
+        self.message = "Input end scores of %s and %s for end %s are both greater than 0 and the end score is not valid."%(self.val_1,self.val_2,self.idx)
+        super().__init__(self.message)
+
+class InvalidEventError(Exception):
+    def __init__(self,cz_event_id:int)->None:
+        self.cz_event_id = cz_event_id
+
+        self.message = "Inputted Event ID of %s is not valid, please check you have the right one."%self.cz_event_id
         super().__init__(self.message)
```

### Comparing `czapi-0.1.7/czapi/core/scraping/base.py` & `czapi-0.1.8/czapi/core/scraping/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,359 +1,376 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/00_base.ipynb (unless otherwise specified).
-
-__all__ = ['LinescorePage', 'get_flat_boxscores_from', 'Event']
-
-# Cell
-
-from bs4 import Tag
-from abc import ABC, abstractproperty, abstractmethod
-from dataclasses import dataclass
-from typing import Optional, List, Any, Tuple
-from uuid import  uuid4
-from ..errors import DifferentScoreLengthError,InvalidScoreError,InvalidEventError
-from ..utils import make_request_from, make_soup_from
-from ..testing import TagLike
-from time import sleep
-
-# Internal Cell
-
-def generate_dict_from_table(
-
-     table : Tag
-    ,**kwargs
-
-)->dict:
-    """Helper function for returning the curling boxscore from a bs4 Tag object."""
-    d = {}
-    team = None
-
-    # TODO : add error handling for when no table is passed / None
-
-    if table is None:
-        raise ValueError('Table tag is NoneType.')
-
-    # loop through tags in table
-    for tag in table.find_all('td'):
-        if tag.attrs.get('class') == ['linescoreteam']:
-            team = tag.a.string
-            d[team] = {**kwargs}
-            d[team]['href'] = tag.a['href']
-            d[team]['score'] = list() # initiate score incase the game hasn't started
-
-        elif tag.attrs.get('class') == ['linescorehammer']:
-            d[team]['hammer'] = not bool(tag.string) # opposite for some reason
-        elif tag.attrs.get('class') == ['linescoreend']:
-            score = tag.string.strip()
-            if score: d[team]['score'].append(tag.string.strip()) # eliminates empty strings
-        elif tag.attrs.get('class') == ['linescorefinal']:
-            d[team]['finalscore'] = tag.b.string.strip()
-
-    return d
-
-# Internal Cell
-def normalize_scores(score_1 : List[str],score_2 : List[str])->Tuple[List[int],List[int]]:
-    """
-        Take two lists representing the end results of a boxscore and return the 'normalized' or relative scores.
-    """
-    score_1_len = len(score_1)
-    score_2_len = len(score_2)
-    if score_1_len != score_2_len:
-        raise DifferentScoreLengthError(score_1_len =score_1_len,score_2_len = score_2_len)
-
-
-    current_diff = 0
-    end_1 = [current_diff]
-
-    for i in range(score_1_len-1):
-        try:
-            val_1 = int(score_1[i])
-            val_2 = int(score_2[i])
-
-        except ValueError:
-            break
-
-        if val_1 > 0 and val_2 > 0:
-            raise InvalidScoreError(idx = i+1, val_1 = val_1,val_2=val_2)
-
-        new_current_diff = current_diff + val_1 - val_2
-        end_1.append(new_current_diff)
-        current_diff = new_current_diff
-
-    return end_1, list(map(lambda x: -1*x,end_1))
-
-# Internal Cell
-def get_hammer_progressions(hammer_start:bool,normalized_score:List[int])->Tuple[List[bool],List[bool]]:
-    current_hammer = hammer_start
-    current_score = 0
-    hammer_progression = [hammer_start]
-    for i in range(1,len(normalized_score)):
-        if current_hammer and (normalized_score[i] > current_score):
-            current_hammer = False
-        if not current_hammer and (normalized_score[i] < current_score):
-            current_hammer = True
-        current_score = normalized_score[i]
-        hammer_progression.append(current_hammer)
-
-    return hammer_progression, list(map(lambda x: not x, hammer_progression))
-
-# Internal Cell
-
-@dataclass
-class HalfBoxscore:
-    team_name : str
-    href : str
-    hammer : bool
-    score : List[str]
-    finalscore : str
-    draw_num : int
-    draw : str
-
-
-
-@dataclass
-class NormalizedHalfBoxscore(HalfBoxscore):
-    hammer_progression : List[bool]
-    normalized_score : List[int]
-
-# Internal Cell
-
-def generate_half_boxscore_pair(boxscore:dict)->Tuple[NormalizedHalfBoxscore]:
-    half_boxscores = [HalfBoxscore(team_name=team_name,**results) for team_name,results in boxscore.items()]
-
-    normalized_scores = normalize_scores(
-
-         score_1 = half_boxscores[0].score
-        ,score_2 = half_boxscores[1].score
-
-    )
-
-    hammer_progressions = get_hammer_progressions(
-
-         hammer_start = half_boxscores[0].hammer
-        ,normalized_score = normalized_scores[0]
-
-    )
-
-    return NormalizedHalfBoxscore(**half_boxscores[0].__dict__,hammer_progression = hammer_progressions[0],normalized_score = normalized_scores[0]),NormalizedHalfBoxscore(**half_boxscores[1].__dict__,hammer_progression = hammer_progressions[1],normalized_score = normalized_scores[1] )
-
-
-# Internal Cell
-
-@dataclass
-class NormalizedBoxscore:
-
-    boxscore: dict
-
-    def __post_init__(self)->None:
-        self.normalized_half_boxscore_pair = generate_half_boxscore_pair(boxscore=self.boxscore)
-        self.guid = uuid4().int
-        self.flattened_normalized_boxscore = [tuple(half_score.__dict__.values())+(self.guid,) for half_score in self.normalized_half_boxscore_pair]
-
-
-#     @property
-#     def flattened_normalized_boxscore(self)->List[List[Any]]:
-#         return [list(half_score.__dict__.values())+[self.guid] for half_score in self.normalized_half_boxscore_pair]
-
-
-# Internal Cell
-
-class Page(ABC):
-
-
-    @abstractproperty
-    def url(self)->str:
-        pass
-
-    @abstractproperty
-    def event_name(self)->str:
-        pass
-
-    @abstractproperty
-    def event_date(self)->str:
-        pass
-
-    @abstractproperty
-    def draw(self)->str:
-        pass
-
-    @abstractproperty
-    def draw_num(self)->int:
-        pass
-
-    @abstractproperty
-    def tables(self)->List[Tag]:
-        pass
-
-    @abstractmethod
-    def generate_boxscores(self)->List[dict]:
-        pass
-
-# Cell
-@dataclass
-class LinescorePage(Page):
-    """
-        Represents a CurlingZone linescore page.
-        Example page here: https://curlingzone.com/event.php?eventid=7795&view=Scores&showdrawid=25#1
-
-    """
-    cz_event_id : int
-    cz_draw_id: int
-
-
-    def __post_init__(self)->None:
-        response = make_request_from(url = self.url)
-        self.soup = make_soup_from(response=response)
-        self.boxscores = self.generate_boxscores()
-        self.normalized_boxscores = self.generate_normalized_boxscores()
-
-
-    @property
-    def url(self)->str:
-        return 'https://curlingzone.com/event.php?eventid=%s&view=Scores&showdrawid=%s#1'%(self.cz_event_id,self.cz_draw_id)
-
-    @property
-    def event_name(self)->str:
-        return self.soup.find('h3',attrs={'class':'entry-title-widget'}).string
-
-    @property
-    def event_date(self)->str:
-        return self.soup.find('div',attrs={'class':'badge-widget'}).string
-
-    @property
-    def draw_num(self)->int:
-        return self.soup.find(name='select').find_all(name='option').index(self.soup.find(name='option',attrs={'selected':'selected'}))+1
-
-    @property
-    def draw(self)->str:
-        return self.soup.find(name='option',attrs={'selected':'selected'}).string
-
-    @property
-    def tables(self)->List[Tag]:
-        return self.soup.find_all(name = 'table',attrs={'class':'linescorebox'})
-
-    def generate_boxscores(self)->List[dict]:
-        return [generate_dict_from_table(table=table,draw=self.draw,draw_num=self.draw_num) for table in self.tables]
-
-    def generate_normalized_boxscores(self)->List[NormalizedBoxscore]:
-        return [NormalizedBoxscore(boxscore=boxscore) for boxscore in self.boxscores]
-
-    def get_boxscore_from(self,cz_game_id : int)->dict:
-        if cz_game_id <= 0:
-            raise ValueError('cz_game_id must be 1 or greater.')
-
-        if cz_game_id > len(self.boxscores):
-            raise ValueError('') # TODO
-
-        return self.boxscores[cz_game_id - 1]
-
-    # repeated code but will re-factor later
-    def get_normalized_boxscore_from(self,cz_game_id : int)->NormalizedBoxscore:
-        if cz_game_id <= 0:
-            raise ValueError('cz_game_id must be 1 or greater.')
-
-        if cz_game_id > len(self.normalized_boxscores):
-            raise ValueError('') # TODO
-
-        return self.normalized_boxscores[cz_game_id - 1]
-
-
-# Internal Cell
-class BadLinescorePage(Page):
-
-    def __init__(self
-                 ,url:str=None
-                 ,event_name:str=None
-                 ,event_date:str=None
-                 ,draw:str=None
-                 ,draw_num:int=None
-                 ,tables:List[TagLike]=None
-                 ,boxscores:List[dict]=None
-                 ,normalized_boxscores:List[NormalizedBoxscore]=None
-                ):
-        self.url = url
-        self.event_name = event_name
-        self.event_date = event_date
-        self.draw = draw
-        self.draw_num = draw_num
-        self.tables = tables
-        self.boxscores = boxscores
-        self.normalized_boxscores = normalized_boxscores
-
-    def url(self)->str:
-        return ''
-
-
-    def event_name(self)->str:
-        return ''
-
-    def event_date(self)->str:
-        return ''
-
-    def draw_num(self)->int:
-        return 1
-
-    def draw(self)->str:
-        return ''
-
-    def tables(self)->List[Tag]:
-        pass
-
-    def generate_boxscores(self)->List[dict]:
-        return self.boxscores
-
-
-# Internal Cell
-
-GameData = List[Tuple[str,str,bool,List[str],str,int,str,List[bool],List[int],int]]
-def _get_flat_boxscores_from(linescore_page:LinescorePage)->GameData:
-    flattened_boxscores = [boxscore.flattened_normalized_boxscore for boxscore in linescore_page.normalized_boxscores]
-    return [(row[0],row[1],row[2],row[3],row[4],row[5],row[6],row[7],row[8],row[9]) for f in flattened_boxscores for row in f]
-
-# Cell
-
-def get_flat_boxscores_from(cz_event_id:int,cz_draw_id:int)->GameData:
-    """Returns a list of tuples of boxscore information on a linescore page."""
-    linescore_page = LinescorePage(cz_event_id = cz_event_id,cz_draw_id = cz_draw_id)
-    return _get_flat_boxscores_from(linescore_page = linescore_page)
-
-# Cell
-
-
-@dataclass
-class Event:
-    cz_event_id : int
-    delay : int =0
-    verbose: bool = False
-
-
-    def __post_init__(self)->None:
-        response = make_request_from(url = self.url)
-        self.soup = make_soup_from(response=response)
-
-        if not self.is_valid:
-            raise InvalidEventError(cz_event_id = self.cz_event_id)
-
-        pages = list()
-        for draw_id in range(self.draws):
-            if self.verbose:
-                print('Scraping draw %s.'%(draw_id+1))
-            pages.append(LinescorePage(cz_event_id = self.cz_event_id,cz_draw_id = draw_id+1))
-            sleep(self.delay)
-
-        self.pages = pages
-
-
-    @property
-    def is_valid(self)->bool:
-        return self.soup.find(name='select') is not None
-
-    @property
-    def url(self)->str:
-        return 'https://curlingzone.com/event.php?eventid=%s&view=Scores&showdrawid=1#1'%(self.cz_event_id)
-
-    @property
-    def draws(self)->int:
-        return len(self.soup.find(name='select').find_all(name='option'))
-
-
-    def get_flat_boxscores(self)->List[GameData]:
+# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/00_base.ipynb (unless otherwise specified).
+
+__all__ = ['LinescorePage', 'game_data_column_headers', 'get_flat_boxscores_from', 'Event']
+
+# Cell
+
+from bs4 import Tag
+from abc import ABC, abstractproperty, abstractmethod
+from dataclasses import dataclass
+from typing import Optional, List, Any, Tuple
+from uuid import  uuid4
+from ..errors import DifferentScoreLengthError,InvalidScoreError,InvalidEventError
+from ..utils import make_request_from, make_soup_from
+from ..testing import TagLike
+from time import sleep
+
+# Internal Cell
+
+def generate_dict_from_table(
+
+     table : Tag
+    ,**kwargs
+
+)->dict:
+    """Helper function for returning the curling boxscore from a bs4 Tag object."""
+    d = {}
+    team = None
+
+    # TODO : add error handling for when no table is passed / None
+
+    if table is None:
+        raise ValueError('Table tag is NoneType.')
+
+    # loop through tags in table
+    for tag in table.find_all('td'):
+        if tag.attrs.get('class') == ['linescoreteam']:
+            team = tag.a.string
+            d[team] = {**kwargs}
+            d[team]['href'] = tag.a['href']
+            d[team]['score'] = list() # initiate score incase the game hasn't started
+
+        elif tag.attrs.get('class') == ['linescorehammer']:
+            d[team]['hammer'] = not bool(tag.string) # opposite for some reason
+        elif tag.attrs.get('class') == ['linescoreend']:
+            score = tag.string.strip()
+            if score: d[team]['score'].append(tag.string.strip()) # eliminates empty strings
+        elif tag.attrs.get('class') == ['linescorefinal']:
+            d[team]['finalscore'] = tag.b.string.strip()
+
+    return d
+
+# Internal Cell
+def normalize_scores(score_1 : List[str],score_2 : List[str])->Tuple[List[int],List[int]]:
+    """
+        Take two lists representing the end results of a boxscore and return the 'normalized' or relative scores.
+    """
+    score_1_len = len(score_1)
+    score_2_len = len(score_2)
+    if score_1_len != score_2_len:
+        raise DifferentScoreLengthError(score_1_len =score_1_len,score_2_len = score_2_len)
+
+
+    current_diff = 0
+    end_1 = [current_diff]
+
+    for i in range(score_1_len-1):
+        try:
+            val_1 = int(score_1[i])
+            val_2 = int(score_2[i])
+
+        except ValueError:
+            break
+
+        if val_1 > 0 and val_2 > 0:
+            raise InvalidScoreError(idx = i+1, val_1 = val_1,val_2=val_2)
+
+        new_current_diff = current_diff + val_1 - val_2
+        end_1.append(new_current_diff)
+        current_diff = new_current_diff
+
+    return end_1, list(map(lambda x: -1*x,end_1))
+
+# Internal Cell
+def get_hammer_progressions(hammer_start:bool,normalized_score:List[int])->Tuple[List[bool],List[bool]]:
+    current_hammer = hammer_start
+    current_score = 0
+    hammer_progression = [hammer_start]
+    for i in range(1,len(normalized_score)):
+        if current_hammer and (normalized_score[i] > current_score):
+            current_hammer = False
+        if not current_hammer and (normalized_score[i] < current_score):
+            current_hammer = True
+        current_score = normalized_score[i]
+        hammer_progression.append(current_hammer)
+
+    return hammer_progression, list(map(lambda x: not x, hammer_progression))
+
+# Internal Cell
+
+@dataclass
+class HalfBoxscore:
+    team_name : str
+    href : str
+    hammer : bool
+    score : List[str]
+    finalscore : str
+    draw_num : int
+    draw : str
+
+
+
+@dataclass
+class NormalizedHalfBoxscore(HalfBoxscore):
+    hammer_progression : List[bool]
+    normalized_score : List[int]
+
+# Internal Cell
+
+def generate_half_boxscore_pair(boxscore:dict)->Tuple[NormalizedHalfBoxscore]:
+    half_boxscores = [HalfBoxscore(team_name=team_name,**results) for team_name,results in boxscore.items()]
+
+    normalized_scores = normalize_scores(
+
+         score_1 = half_boxscores[0].score
+        ,score_2 = half_boxscores[1].score
+
+    )
+
+    hammer_progressions = get_hammer_progressions(
+
+         hammer_start = half_boxscores[0].hammer
+        ,normalized_score = normalized_scores[0]
+
+    )
+
+    return NormalizedHalfBoxscore(**half_boxscores[0].__dict__,hammer_progression = hammer_progressions[0],normalized_score = normalized_scores[0]),NormalizedHalfBoxscore(**half_boxscores[1].__dict__,hammer_progression = hammer_progressions[1],normalized_score = normalized_scores[1] )
+
+
+# Internal Cell
+
+@dataclass
+class NormalizedBoxscore:
+
+    boxscore: dict
+
+    def __post_init__(self)->None:
+        self.normalized_half_boxscore_pair = generate_half_boxscore_pair(boxscore=self.boxscore)
+        self.guid = uuid4().int
+        self.flattened_normalized_boxscore = [tuple(half_score.__dict__.values())+(self.guid,) for half_score in self.normalized_half_boxscore_pair]
+
+
+#     @property
+#     def flattened_normalized_boxscore(self)->List[List[Any]]:
+#         return [list(half_score.__dict__.values())+[self.guid] for half_score in self.normalized_half_boxscore_pair]
+
+
+# Internal Cell
+
+class Page(ABC):
+
+
+    @abstractproperty
+    def url(self)->str:
+        pass
+
+    @abstractproperty
+    def event_name(self)->str:
+        pass
+
+    @abstractproperty
+    def event_date(self)->str:
+        pass
+
+    @abstractproperty
+    def draw(self)->str:
+        pass
+
+    @abstractproperty
+    def draw_num(self)->int:
+        pass
+
+    @abstractproperty
+    def tables(self)->List[Tag]:
+        pass
+
+    @abstractmethod
+    def generate_boxscores(self)->List[dict]:
+        pass
+
+# Cell
+@dataclass
+class LinescorePage(Page):
+    """
+        Represents a CurlingZone linescore page.
+        Example page here: https://curlingzone.com/event.php?eventid=7795&view=Scores&showdrawid=25#1
+
+    """
+    cz_event_id : int
+    cz_draw_id: int
+
+
+    def __post_init__(self)->None:
+        response = make_request_from(url = self.url)
+        self.soup = make_soup_from(response=response)
+        self.boxscores = self.generate_boxscores()
+        self.normalized_boxscores = self.generate_normalized_boxscores()
+
+
+    @property
+    def url(self)->str:
+        return 'https://curlingzone.com/event.php?eventid=%s&view=Scores&showdrawid=%s#1'%(self.cz_event_id,self.cz_draw_id)
+
+    @property
+    def event_name(self)->str:
+        return self.soup.find('h3',attrs={'class':'entry-title-widget'}).string
+
+    @property
+    def event_date(self)->str:
+        return self.soup.find('div',attrs={'class':'badge-widget'}).string
+
+    @property
+    def draw_num(self)->int:
+        return self.soup.find(name='select').find_all(name='option').index(self.soup.find(name='option',attrs={'selected':'selected'}))+1
+
+    @property
+    def draw(self)->str:
+        return self.soup.find(name='option',attrs={'selected':'selected'}).string
+
+    @property
+    def tables(self)->List[Tag]:
+        return self.soup.find_all(name = 'table',attrs={'class':'linescorebox'})
+
+    def generate_boxscores(self)->List[dict]:
+        return [generate_dict_from_table(table=table,draw=self.draw,draw_num=self.draw_num) for table in self.tables]
+
+    def generate_normalized_boxscores(self)->List[NormalizedBoxscore]:
+        return [NormalizedBoxscore(boxscore=boxscore) for boxscore in self.boxscores]
+
+    def get_boxscore_from(self,cz_game_id : int)->dict:
+        if cz_game_id <= 0:
+            raise ValueError('cz_game_id must be 1 or greater.')
+
+        if cz_game_id > len(self.boxscores):
+            raise ValueError('') # TODO
+
+        return self.boxscores[cz_game_id - 1]
+
+    # repeated code but will re-factor later
+    def get_normalized_boxscore_from(self,cz_game_id : int)->NormalizedBoxscore:
+        if cz_game_id <= 0:
+            raise ValueError('cz_game_id must be 1 or greater.')
+
+        if cz_game_id > len(self.normalized_boxscores):
+            raise ValueError('') # TODO
+
+        return self.normalized_boxscores[cz_game_id - 1]
+
+
+# Internal Cell
+class BadLinescorePage(Page):
+
+    def __init__(self
+                 ,url:str=None
+                 ,event_name:str=None
+                 ,event_date:str=None
+                 ,draw:str=None
+                 ,draw_num:int=None
+                 ,tables:List[TagLike]=None
+                 ,boxscores:List[dict]=None
+                 ,normalized_boxscores:List[NormalizedBoxscore]=None
+                ):
+        self.url = url
+        self.event_name = event_name
+        self.event_date = event_date
+        self.draw = draw
+        self.draw_num = draw_num
+        self.tables = tables
+        self.boxscores = boxscores
+        self.normalized_boxscores = normalized_boxscores
+
+    def url(self)->str:
+        return ''
+
+
+    def event_name(self)->str:
+        return ''
+
+    def event_date(self)->str:
+        return ''
+
+    def draw_num(self)->int:
+        return 1
+
+    def draw(self)->str:
+        return ''
+
+    def tables(self)->List[Tag]:
+        pass
+
+    def generate_boxscores(self)->List[dict]:
+        return self.boxscores
+
+
+# Internal Cell
+
+GameData = List[Tuple[str,str,bool,List[str],str,int,str,List[bool],List[int],int]]
+
+def _get_flat_boxscores_from(linescore_page:LinescorePage)->GameData:
+    flattened_boxscores = [boxscore.flattened_normalized_boxscore for boxscore in linescore_page.normalized_boxscores]
+    return [(row[0],row[1],row[2],row[3],row[4],row[5],row[6],row[7],row[8],row[9]) for f in flattened_boxscores for row in f]
+
+# Cell
+
+game_data_column_headers = (
+
+     'team_name'
+    ,'href'
+    ,'hammer_start'
+    ,'score'
+    ,'final_score'
+    ,'hammer_progression'
+    ,'relative_score'
+    ,'guid'
+
+
+)
+
+# Cell
+
+def get_flat_boxscores_from(cz_event_id:int,cz_draw_id:int)->GameData:
+    """Returns a list of tuples of boxscore information on a linescore page."""
+    linescore_page = LinescorePage(cz_event_id = cz_event_id,cz_draw_id = cz_draw_id)
+    return _get_flat_boxscores_from(linescore_page = linescore_page)
+
+# Cell
+
+
+@dataclass
+class Event:
+    cz_event_id : int
+    delay : int =0
+    verbose: bool = False
+
+
+    def __post_init__(self)->None:
+        response = make_request_from(url = self.url)
+        self.soup = make_soup_from(response=response)
+
+        if not self.is_valid:
+            raise InvalidEventError(cz_event_id = self.cz_event_id)
+
+        pages = list()
+        for draw_id in range(self.draws):
+            if self.verbose:
+                print('Scraping draw %s.'%(draw_id+1))
+            pages.append(LinescorePage(cz_event_id = self.cz_event_id,cz_draw_id = draw_id+1))
+            sleep(self.delay)
+
+        self.pages = pages
+
+
+    @property
+    def is_valid(self)->bool:
+        return self.soup.find(name='select') is not None
+
+    @property
+    def url(self)->str:
+        return 'https://curlingzone.com/event.php?eventid=%s&view=Scores&showdrawid=1#1'%(self.cz_event_id)
+
+    @property
+    def draws(self)->int:
+        return len(self.soup.find(name='select').find_all(name='option'))
+
+
+    def get_flat_boxscores(self)->List[GameData]:
         return [_get_flat_boxscores_from(linescore_page = linescore_page) for linescore_page in self.pages]
```

### Comparing `czapi-0.1.7/settings.ini` & `czapi-0.1.8/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[DEFAULT]
-host = github
-lib_name = czapi
-user = calicorob
-description = CurlingZone scraper API.
-keywords = curling, stats
-author = Robert Currie
-author_email = robert.art.currie@gmail.com
-copyright = Robert Currie
-branch = master
-version = 0.1.7
-min_python = 3.6
-audience = Developers
-language = English
-custom_sidebar = False
-license = apache2
-status = 2
-requirements = bs4 requests
-nbs_path = nbs
-doc_path = docs
-recursive = False
-doc_host = https://calicorob.github.io
-doc_baseurl = /czapi/
-git_url = https://github.com/calicorob/czapi/tree/master/
-lib_path = czapi
-title = czapi
-
+[DEFAULT]
+host = github
+lib_name = czapi
+user = calicorob
+description = CurlingZone scraper API.
+keywords = curling, stats
+author = Robert Currie
+author_email = robert.art.currie@gmail.com
+copyright = Robert Currie
+branch = master
+version = 0.1.8
+min_python = 3.6
+audience = Developers
+language = English
+custom_sidebar = False
+license = apache2
+status = 2
+requirements = bs4 requests
+nbs_path = nbs
+doc_path = docs
+recursive = False
+doc_host = https://calicorob.github.io
+doc_baseurl = /czapi/
+git_url = https://github.com/calicorob/czapi/tree/master/
+lib_path = czapi
+title = czapi
+
```

### Comparing `czapi-0.1.7/setup.py` & `czapi-0.1.8/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools,re,sys
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
-
-# note: all settings are in settings.ini; edit there, not here
-config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
-cfg = config['DEFAULT']
-
-cfg_keys = 'version description keywords author author_email'.split()
-expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
-for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
-
-if len(sys.argv)>1 and sys.argv[1]=='version':
-    print(setup_cfg['version'])
-    exit()
-
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8'.split()
-
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-min_python = cfg['min_python']
-
-requirements = ['pip', 'packaging']
-if cfg.get('requirements'): requirements += cfg.get('requirements','').split()
-if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
-dev_requirements = (cfg.get('dev_requirements') or '').split()
-
-long_description = open('README.md').read()
-# ![png](docs/images/output_13_0.png)
-for ext in ['png', 'svg']:
-    long_description = re.sub(r'!\['+ext+'\]\((.*)\)', '!['+ext+']('+'https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1)', long_description)
-    long_description = re.sub(r'src=\"(.*)\.'+ext+'\"', 'src=\"https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1.'+ext+'\"', long_description)
-
-setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
-    **setup_cfg)
-
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools,re,sys
+assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+# note: all settings are in settings.ini; edit there, not here
+config = ConfigParser(delimiters=['='])
+config.read('settings.ini')
+cfg = config['DEFAULT']
+
+cfg_keys = 'version description keywords author author_email'.split()
+expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
+for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
+setup_cfg = {o:cfg[o] for o in cfg_keys}
+
+if len(sys.argv)>1 and sys.argv[1]=='version':
+    print(setup_cfg['version'])
+    exit()
+
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8'.split()
+
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+min_python = cfg['min_python']
+
+requirements = ['pip', 'packaging']
+if cfg.get('requirements'): requirements += cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
+dev_requirements = (cfg.get('dev_requirements') or '').split()
+
+long_description = open('README.md').read()
+# ![png](docs/images/output_13_0.png)
+for ext in ['png', 'svg']:
+    long_description = re.sub(r'!\['+ext+'\]\((.*)\)', '!['+ext+']('+'https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1)', long_description)
+    long_description = re.sub(r'src=\"(.*)\.'+ext+'\"', 'src=\"https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1.'+ext+'\"', long_description)
+
+setuptools.setup(
+    name = cfg['lib_name'],
+    license = lic[0],
+    classifiers = [
+        'Development Status :: ' + statuses[int(cfg['status'])],
+        'Intended Audience :: ' + cfg['audience'].title(),
+        'Natural Language :: ' + cfg['language'].title(),
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
+    packages = setuptools.find_packages(),
+    include_package_data = True,
+    install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
+    **setup_cfg)
+
```

