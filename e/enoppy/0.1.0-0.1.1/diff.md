# Comparing `tmp/enoppy-0.1.0.tar.gz` & `tmp/enoppy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\enoppy-0.1.0.tar", last modified: Sat May 20 08:47:30 2023, max compression
+gzip compressed data, was "enoppy-0.1.1.tar", last modified: Sat May 20 17:09:36 2023, max compression
```

## Comparing `enoppy-0.1.0.tar` & `enoppy-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 08:47:30.662184 enoppy-0.1.0/
--rw-rw-rw-   0        0        0     3433 2020-08-04 06:14:52.000000 enoppy-0.1.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     4075 2023-05-20 03:40:15.000000 enoppy-0.1.0/ChangeLog.md
--rw-rw-rw-   0        0        0    35823 2022-07-13 08:41:23.000000 enoppy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      113 2023-05-20 03:40:15.000000 enoppy-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10246 2023-05-20 08:47:30.661186 enoppy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6160 2023-05-20 03:55:34.000000 enoppy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 08:47:30.643234 enoppy-0.1.0/enoppy/
--rw-rw-rw-   0        0        0      915 2023-05-20 04:12:46.000000 enoppy-0.1.0/enoppy/__init__.py
--rw-rw-rw-   0        0        0     7109 2023-05-20 04:17:14.000000 enoppy-0.1.0/enoppy/engineer.py
-drwxrwxrwx   0        0        0        0 2023-05-20 08:47:30.658194 enoppy-0.1.0/enoppy/paper_based/
--rw-rw-rw-   0        0        0      399 2022-07-30 15:11:54.000000 enoppy-0.1.0/enoppy/paper_based/__init__.py
--rw-rw-rw-   0        0        0     8307 2023-05-20 02:29:54.000000 enoppy-0.1.0/enoppy/paper_based/ihaoavoa_2022.py
--rw-rw-rw-   0        0        0    16947 2023-05-20 02:30:19.000000 enoppy-0.1.0/enoppy/paper_based/moeosma_2023.py
-drwxrwxrwx   0        0        0        0 2023-05-20 08:47:30.661186 enoppy-0.1.0/enoppy/utils/
--rw-rw-rw-   0        0        0      399 2023-05-20 02:33:42.000000 enoppy-0.1.0/enoppy/utils/__init__.py
--rw-rw-rw-   0        0        0     2385 2023-05-11 08:26:30.000000 enoppy-0.1.0/enoppy/utils/encoder.py
--rw-rw-rw-   0        0        0    10326 2022-07-13 08:41:24.000000 enoppy-0.1.0/enoppy/utils/operator.py
--rw-rw-rw-   0        0        0     3739 2022-10-02 10:35:18.000000 enoppy-0.1.0/enoppy/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-20 08:47:30.656199 enoppy-0.1.0/enoppy.egg-info/
--rw-rw-rw-   0        0        0    10246 2023-05-20 08:47:30.000000 enoppy-0.1.0/enoppy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-20 08:47:30.000000 enoppy-0.1.0/enoppy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 08:47:30.000000 enoppy-0.1.0/enoppy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-05-20 08:47:30.000000 enoppy-0.1.0/enoppy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-20 08:47:30.000000 enoppy-0.1.0/enoppy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6397 2023-05-20 02:30:19.000000 enoppy-0.1.0/examples.md
--rw-rw-rw-   0        0        0       42 2023-05-20 08:47:30.662184 enoppy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3499 2023-05-20 03:40:15.000000 enoppy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:09:36.672065 enoppy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-20 17:08:55.000000 enoppy-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 17:08:55.000000 enoppy-0.1.1/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 17:08:55.000000 enoppy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 17:08:55.000000 enoppy-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-20 17:09:36.672065 enoppy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-20 17:08:55.000000 enoppy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:09:36.668065 enoppy-0.1.1/enoppy/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/engineer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:09:36.668065 enoppy-0.1.1/enoppy/paper_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/paper_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/paper_based/ihaoavoa_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/paper_based/moeosma_2023.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/paper_based/pdo_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/paper_based/rwco_2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:09:36.672065 enoppy-0.1.1/enoppy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-20 17:08:55.000000 enoppy-0.1.1/enoppy/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:09:36.668065 enoppy-0.1.1/enoppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-20 17:09:36.000000 enoppy-0.1.1/enoppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-20 17:09:36.000000 enoppy-0.1.1/enoppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:09:36.000000 enoppy-0.1.1/enoppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-20 17:09:36.000000 enoppy-0.1.1/enoppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 17:09:36.000000 enoppy-0.1.1/enoppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:09:36.672065 enoppy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-20 17:08:55.000000 enoppy-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:09:36.672065 enoppy-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-20 17:08:55.000000 enoppy-0.1.1/tests/test_benchmark.py
```

### Comparing `enoppy-0.1.0/CODE_OF_CONDUCT.md` & `enoppy-0.1.1/CODE_OF_CONDUCT.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, sex characteristics, gender identity and expression,
-level of experience, education, socio-economic status, nationality, personal
-appearance, race, religion, or sexual identity and orientation.
-
-## Our Standards
-
-Examples of behavior that contributes to creating a positive environment
-include:
-
-* Using welcoming and inclusive language
-* Being respectful of differing viewpoints and experiences
-* Gracefully accepting constructive criticism
-* Focusing on what is best for the community
-* Showing empathy towards other community members
-
-Examples of unacceptable behavior by participants include:
-
-* The use of sexualized language or imagery and unwelcome sexual attention or
- advances
-* Trolling, insulting/derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or electronic
- address, without explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
- professional setting
-
-## Our Responsibilities
-
-Project maintainers are responsible for clarifying the standards of acceptable
-behavior and are expected to take appropriate and fair corrective action in
-response to any instances of unacceptable behavior.
-
-Project maintainers have the right and responsibility to remove, edit, or
-reject comments, commits, code, wiki edits, issues, and other contributions
-that are not aligned to this Code of Conduct, or to ban temporarily or
-permanently any contributor for other behaviors that they deem inappropriate,
-threatening, offensive, or harmful.
-
-## Scope
-
-This Code of Conduct applies both within project spaces and in public spaces
-when an individual is representing the project or its community. Examples of
-representing a project or community include using an official project e-mail
-address, posting via an official social media account, or acting as an appointed
-representative at an online or offline event. Representation of a project may be
-further defined and clarified by project maintainers.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported by contacting the project team at nguyenthieu2102@gmail.com. All
-complaints will be reviewed and investigated and will result in a response that
-is deemed necessary and appropriate to the circumstances. The project team is
-obligated to maintain confidentiality with regard to the reporter of an incident.
-Further details of specific enforcement policies may be posted separately.
-
-Project maintainers who do not follow or enforce the Code of Conduct in good
-faith may face temporary or permanent repercussions as determined by other
-members of the project's leadership.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
-available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
-
-[homepage]: https://www.contributor-covenant.org
-
-For answers to common questions about this code of conduct, see
-https://www.contributor-covenant.org/faq
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+In the interest of fostering an open and welcoming environment, we as
+contributors and maintainers pledge to making participation in our project and
+our community a harassment-free experience for everyone, regardless of age, body
+size, disability, ethnicity, sex characteristics, gender identity and expression,
+level of experience, education, socio-economic status, nationality, personal
+appearance, race, religion, or sexual identity and orientation.
+
+## Our Standards
+
+Examples of behavior that contributes to creating a positive environment
+include:
+
+* Using welcoming and inclusive language
+* Being respectful of differing viewpoints and experiences
+* Gracefully accepting constructive criticism
+* Focusing on what is best for the community
+* Showing empathy towards other community members
+
+Examples of unacceptable behavior by participants include:
+
+* The use of sexualized language or imagery and unwelcome sexual attention or
+ advances
+* Trolling, insulting/derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or electronic
+ address, without explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+ professional setting
+
+## Our Responsibilities
+
+Project maintainers are responsible for clarifying the standards of acceptable
+behavior and are expected to take appropriate and fair corrective action in
+response to any instances of unacceptable behavior.
+
+Project maintainers have the right and responsibility to remove, edit, or
+reject comments, commits, code, wiki edits, issues, and other contributions
+that are not aligned to this Code of Conduct, or to ban temporarily or
+permanently any contributor for other behaviors that they deem inappropriate,
+threatening, offensive, or harmful.
+
+## Scope
+
+This Code of Conduct applies both within project spaces and in public spaces
+when an individual is representing the project or its community. Examples of
+representing a project or community include using an official project e-mail
+address, posting via an official social media account, or acting as an appointed
+representative at an online or offline event. Representation of a project may be
+further defined and clarified by project maintainers.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported by contacting the project team at nguyenthieu2102@gmail.com. All
+complaints will be reviewed and investigated and will result in a response that
+is deemed necessary and appropriate to the circumstances. The project team is
+obligated to maintain confidentiality with regard to the reporter of an incident.
+Further details of specific enforcement policies may be posted separately.
+
+Project maintainers who do not follow or enforce the Code of Conduct in good
+faith may face temporary or permanent repercussions as determined by other
+members of the project's leadership.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
+available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
+
+[homepage]: https://www.contributor-covenant.org
+
+For answers to common questions about this code of conduct, see
+https://www.contributor-covenant.org/faq
```

### Comparing `enoppy-0.1.0/LICENSE` & `enoppy-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
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
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
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
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `enoppy-0.1.0/enoppy/__init__.py` & `enoppy-0.1.1/enoppy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 11:23, 16/03/2020 ----------%
-#       Email: nguyenthieu2102@gmail.com            %
-#       Github: https://github.com/thieu1995        %
-# --------------------------------------------------%
-#
-# Examples:
-# >>> from enoppy.paper_based import moeosma_2023
-#
-# >>> p1 = moeosma_2023.SpeedReducerProblem()
-#
-# >>> print(p1.get_paras())
-# >>> print(p1.bounds)
-# >>> print(p1.n_dims)
-# >>> print(p1.n_objs)
-# >>> print(p1.n_cons)
-# >>> print(p1.lb)
-# >>> print(p1.ub)
-#
-# >>> x0 = p1.create_solution()
-# >>> print(x0)
-# >>> x0 = p1.amend_position(x0)
-#
-# >>> print(p1.get_objs(x0)) # Get all objectives
-# >>> print(p1.get_cons(x0)) # Get all constraints
-# >>> print(p1.evaluate(x0)) # Evaluate the x0 (calculate fitness value with objectives and constraints combination)
-
-__version__ = "0.1.0"
-
-import inspect
-import re
-from .utils import *
+#!/usr/bin/env python
+# Created by "Thieu" at 11:23, 16/03/2020 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
+# --------------------------------------------------%
+#
+# Examples:
+# >>> from enoppy.paper_based import moeosma_2023
+#
+# >>> p1 = moeosma_2023.SpeedReducerProblem()
+#
+# >>> print(p1.get_paras())
+# >>> print(p1.bounds)
+# >>> print(p1.n_dims)
+# >>> print(p1.n_objs)
+# >>> print(p1.n_cons)
+# >>> print(p1.lb)
+# >>> print(p1.ub)
+#
+# >>> x0 = p1.create_solution()
+# >>> print(x0)
+# >>> x0 = p1.amend_position(x0)
+#
+# >>> print(p1.get_objs(x0)) # Get all objectives
+# >>> print(p1.get_cons(x0)) # Get all constraints
+# >>> print(p1.evaluate(x0)) # Evaluate the x0 (calculate fitness value with objectives and constraints combination)
+
+__version__ = "0.1.1"
+
+import inspect
+import re
+from .utils import *
```

### Comparing `enoppy-0.1.0/enoppy/engineer.py` & `enoppy-0.1.1/enoppy/engineer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,218 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 16:39, 05/05/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-from abc import ABC, abstractmethod
-
-
-class Engineer(ABC):
-    """
-    Defines an abstract class for engineering design problems.
-
-    All subclasses should implement the ``evaluate`` method for a particular optimization problem.
-
-    Attributes
-    ----------
-    bounds : list
-        The lower/upper bounds of the problem. This a 2D-matrix of [lower, upper] array that contain the lower and upper bounds.
-        By default, each problem has its own bounds. But user can try to put different bounds to test the problem.
-    n_dims : int
-        The dimensionality of the problem. It is calculated from bounds
-    lb : np.ndarray
-        The lower bounds for the problem
-    ub : np.ndarray
-        The upper bounds for the problem
-    f_global : float
-        The global optimum of the evaluated function.
-    x_global : np.ndarray
-        A list of vectors that provide the locations of the global minimum.
-        Note that some problems have multiple global minima, not all of which may be listed.
-    n_fe : int
-        The number of function evaluations that the object has been asked to calculate.
-    dim_changeable : bool
-        Whether we can change the benchmark function `x` variable length (i.e., the dimensionality of the problem)
-    """
-
-    name = "Benchmark name"
-    latex_formula = r'f(\mathbf{x})'
-    latex_formula_dimension = r'd \in \mathbb{N}_{+}^{*}'
-    latex_formula_bounds = r'x_i \in [-2\pi, 2\pi], \forall i \in \llbracket 1, d\rrbracket'
-    latex_formula_global_optimum = r'f(0, ..., 0)=-1, \text{ for}, m=5, \beta=15'
-    continuous = True
-    linear = False
-    convex = True
-    unimodal = False
-    separable = False
-
-    differentiable = True
-    scalable = True
-    randomized_term = False
-    parametric = True
-
-    modality = True  # Number of ambiguous peaks, unknown # peaks
-    # n_basins = 1
-    # n_valleys = 1
-
-    def __init__(self):
-        self._bounds = None
-        self._n_dims = None
-        self._n_objs = 1
-        self._n_cons = 0
-        self._n_ineq_cons = -1
-        self._n_eq_cons = -1
-
-        self.f_penalty = None
-        self.f_global = None
-        self.x_global = None
-        self.n_fe = 0
-        self.paras = {}
-        self.epsilon = 1e-8
-        self.w = 1e8
-
-    def get_objs(self, x):
-        """
-        Compute the values of the objective functions for a given set of input values.
-        """
-        pass
-
-    def get_cons(self, x):
-        """
-        Compute the values of the constraint functions for a given set of input values.
-        """
-        pass
-
-    def get_eq_cons(self, x):
-        """
-        Compute the values of the equality constraint functions for a given set of input values.
-        """
-        pass
-
-    def get_ineq_cons(self, x):
-        """
-        Compute the values of the inequality constraint functions for a given set of input values.
-        """
-        pass
-
-    def get_paras(self):
-        """
-        Return the parameters of the problem. Depended on function
-        """
-        default = {"bounds": self._bounds, "n_dims": self._n_dims, }
-        return {**default, **self.paras}
-
-    @property
-    def bounds(self):
-        """
-        The lower/upper bounds to be used for optimization problem. This a 2D-matrix of [lower, upper] array that contain the lower and upper
-        bounds for the problem. The problem should not be asked for evaluation outside these bounds. ``len(bounds) == n_dims``.
-        """
-        return self._bounds
-
-    @property
-    def n_dims(self):
-        """
-        The dimensionality of the problem.
-        """
-        return self._n_dims
-
-    @property
-    def n_objs(self):
-        """
-        The number of objective functions of the problem.
-        """
-        return self._n_objs
-
-    @property
-    def n_cons(self):
-        """
-        The number of constraint functions of the problem.
-        """
-        return self._n_cons
-
-    @property
-    def n_eq_cons(self):
-        """
-        The number of equality constraint functions of the problem.
-        """
-        return self._n_eq_cons
-
-    @property
-    def n_ineq_cons(self):
-        """
-        The number of inequality constraint functions of the problem.
-        """
-        return self._n_ineq_cons
-
-    @property
-    def lb(self):
-        """
-        The lower bounds for the problem
-
-        Returns
-        -------
-        lb : 1D-vector
-            The lower bounds for the problem
-        """
-        return np.array([x[0] for x in self.bounds])
-
-    @property
-    def ub(self):
-        """
-        The upper bounds for the problem
-
-        Returns
-        -------
-        ub : 1D-vector
-            The upper bounds for the problem
-        """
-        return np.array([x[1] for x in self.bounds])
-
-    def amend_position(self, x, lb=None, ub=None):
-        """
-        Amend position to fit the format of the problem
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The current position (solution)
-        """
-        return x
-
-    def create_solution(self):
-        """
-        Create a random solution for the current problem
-
-        Returns
-        -------
-        solution: np.ndarray
-            The random solution
-        """
-        return np.random.uniform(self.lb, self.ub)
-
-    def check_solution(self, x):
-        """
-        Raise the error if the problem size is not equal to the solution length
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The solution
-        """
-        if len(x) != self._n_dims:
-            raise ValueError(f"The length of solution should has {self._n_dims} variables!")
-
-    def default_penalty(self, list_objs=None, list_cons=None):
-        list_objs_new = np.zeros_like(list_objs)
-        for idx, val in enumerate(list_objs):
-            temp = val + self.w * np.sum([max(0, f_con) for f_con in list_cons])
-            list_objs_new[idx] = temp
-        return list_objs_new
-
-    def check_penalty_func(self, func=None):
-        if callable(func):
-            self.f_penalty = func
-        else:
-            self.f_penalty = self.default_penalty
-
-    def evaluate(self, x):
-        """
-        Evaluation of the benchmark function.
-
-        Parameters
-        ----------
-        x : np.ndarray, list, tuple
-            The candidate vector for evaluating the benchmark problem. Must have ``len(x) == self.n_dims``.
-
-        Returns
-        -------
-        val : float
-              the evaluated benchmark function
-        """
-        pass
+#!/usr/bin/env python
+# Created by "Thieu" at 16:39, 05/05/2023 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+from abc import ABC
+
+
+class Engineer(ABC):
+    """
+    Defines an abstract class for engineering design problems.
+
+    All subclasses should implement the ``evaluate`` method for a particular problem.
+
+    Attributes
+    ----------
+    bounds : list
+        The lower/upper bounds of the problem. This a 2D-matrix of [lower, upper] array that contain the lower and upper bounds.
+        By default, each problem has its own bounds. But user can try to put different bounds to test the problem.
+    n_dims : int
+        The dimensionality of the problem. It is calculated from bounds
+    lb : np.ndarray
+        The lower bounds for the problem
+    ub : np.ndarray
+        The upper bounds for the problem
+    f_global : float
+        The global optimum of the evaluated function.
+    x_global : np.ndarray
+        A list of vectors that provide the locations of the global minimum.
+        Note that some problems have multiple global minima, not all of which may be listed.
+    n_fe : int
+        The number of function evaluations that the object has been asked to calculate.
+    """
+
+    name = "Benchmark name"
+    linear = False
+    convex = True
+    differentiable = True
+    parametric = True
+
+    def __init__(self):
+        self._bounds = None
+        self._n_dims = None
+        self._n_objs = 1
+        self._n_cons = 0
+        self._n_ineq_cons = -1
+        self._n_eq_cons = -1
+
+        self.f_penalty = None
+        self.f_global = None
+        self.x_global = None
+        self.n_fe = 0
+        self.paras = {}
+        self.epsilon = 1e-8
+        self.w = 1e8
+
+    def get_objs(self, x):
+        """
+        Compute the values of the objective functions for a given set of input values.
+        """
+        pass
+
+    def get_cons(self, x):
+        """
+        Compute the values of the constraint functions for a given set of input values.
+        """
+        pass
+
+    def get_eq_cons(self, x):
+        """
+        Compute the values of the equality constraint functions for a given set of input values.
+        """
+        pass
+
+    def get_ineq_cons(self, x):
+        """
+        Compute the values of the inequality constraint functions for a given set of input values.
+        """
+        pass
+
+    def get_paras(self):
+        """
+        Return the parameters of the problem. Depended on function
+        """
+        default = {"bounds": self._bounds, "n_dims": self._n_dims, }
+        return {**default, **self.paras}
+
+    @property
+    def bounds(self):
+        """
+        The lower/upper bounds to be used for optimization problem. This a 2D-matrix of [lower, upper] array that contain the lower and upper
+        bounds for the problem. The problem should not be asked for evaluation outside these bounds. ``len(bounds) == n_dims``.
+        """
+        return self._bounds
+
+    @property
+    def n_dims(self):
+        """
+        The dimensionality of the problem.
+        """
+        return self._n_dims
+
+    @property
+    def n_objs(self):
+        """
+        The number of objective functions of the problem.
+        """
+        return self._n_objs
+
+    @property
+    def n_cons(self):
+        """
+        The number of constraint functions of the problem.
+        """
+        return self._n_cons
+
+    @property
+    def n_eq_cons(self):
+        """
+        The number of equality constraint functions of the problem.
+        """
+        return self._n_eq_cons
+
+    @property
+    def n_ineq_cons(self):
+        """
+        The number of inequality constraint functions of the problem.
+        """
+        return self._n_ineq_cons
+
+    @property
+    def lb(self):
+        """
+        The lower bounds for the problem
+
+        Returns
+        -------
+        lb : 1D-vector
+            The lower bounds for the problem
+        """
+        return np.array([x[0] for x in self.bounds])
+
+    @property
+    def ub(self):
+        """
+        The upper bounds for the problem
+
+        Returns
+        -------
+        ub : 1D-vector
+            The upper bounds for the problem
+        """
+        return np.array([x[1] for x in self.bounds])
+
+    def amend_position(self, x, lb=None, ub=None):
+        """
+        Amend position to fit the format of the problem
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The current position (solution)
+        """
+        return x
+
+    def create_solution(self):
+        """
+        Create a random solution for the current problem
+
+        Returns
+        -------
+        solution: np.ndarray
+            The random solution
+        """
+        return np.random.uniform(self.lb, self.ub)
+
+    def check_solution(self, x):
+        """
+        Raise the error if the problem size is not equal to the solution length
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The solution
+        """
+        if len(x) != self._n_dims:
+            raise ValueError(f"The length of solution should has {self._n_dims} variables!")
+
+    def default_penalty(self, list_objs=None, list_cons=None):
+        list_objs_new = np.zeros_like(list_objs)
+        for idx, val in enumerate(list_objs):
+            temp = val + self.w * np.sum([max(0, f_con) for f_con in list_cons])
+            list_objs_new[idx] = temp
+        return list_objs_new
+
+    def check_penalty_func(self, func=None):
+        if callable(func):
+            self.f_penalty = func
+        else:
+            self.f_penalty = self.default_penalty
+
+    def evaluate(self, x):
+        """
+        Evaluation of the benchmark function.
+
+        Parameters
+        ----------
+        x : np.ndarray, list, tuple
+            The candidate vector for evaluating the benchmark problem. Must have ``len(x) == self.n_dims``.
+
+        Returns
+        -------
+        val : float
+              the evaluated benchmark function
+        """
+        pass
```

### Comparing `enoppy-0.1.0/enoppy/paper_based/ihaoavoa_2022.py` & `enoppy-0.1.1/enoppy/paper_based/ihaoavoa_2022.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,237 +1,237 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 16:25, 09/05/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-# Paper: IHAOAVOA: An improved hybrid aquila optimizer and African vultures optimization algorithm for global optimization problems
-
-import numpy as np
-from enoppy.engineer import Engineer
-
-
-class TensionCompressionSpringProblem(Engineer):
-    """
-    x = [x1, x2, x3] = [d, D, N]
-    """
-
-    name = "Tension/compression spring design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 3
-        self._n_objs = 1
-        self._n_cons = 4
-        self._bounds = [(0.05, 2.0), (0.25, 1.3), (2.0, 15.0)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        f1 = (x[2] + 2) * x[1]*x[0]**2
-        return np.array([f1, ])
-
-    def get_cons(self, x):
-        g1 = 1 - (x[1]**3 * x[2]) / (71785 * x[0]**4)
-        g2 = (4*x[1]**2 - x[0]*x[1])/(12566 * (x[1]*x[0]**3 - x[0]**4)) + 1. / (5108 * x[0]**2)
-        g3 = 1 - 140.45*x[0] / (x[1]**2 * x[2])
-        g4 = (x[0] + x[1]) / 1.5 - 1
-        return np.array([g1, g2, g3, g4])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class WeldedBeamProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4] = [h, l, t, b]
-    """
-
-    name = "Welded beam design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 4
-        self._n_objs = 1
-        self._n_cons = 7
-        self._bounds = [(0.1, 2.0), (0.1, 10.), (0.1, 10.), (0.1, 2.0)]
-        self.L = 14
-        self.E = 30*10**6
-        self.G = 12*10**6
-        self.theta_max = 0.25
-        self.tau_max = 13600
-        self.xichma_max = 30000
-        self.P = 6000
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        f1 = 1.10471 * x[0]**2 * x[1] + 0.04811 * x[2] * x[3] * (14 + x[1])
-        return np.array([f1, ])
-
-    def get_cons(self, x):
-        Pc = 4.013*self.E*np.sqrt(x[2]**2 * x[3]**6 / 36) / self.L**2 * (1 - x[2]*np.sqrt(self.E/(4*self.G)) / (2*self.L))
-        theta_z = 6 * self.P * self.L**3 / (self.E * x[2]**2 * x[3])
-        xichma_z = 6*self.P*self.L / (self.E * x[2]**2 * x[3])
-        jj = 2*np.sqrt(2)*x[0]*x[1]*(x[1]**2 / 4 + ((x[0] + x[2])/2)**2)
-        R = np.sqrt(x[1]**2/4 + (x[0]+x[2])**2 / 4)
-        M = self.P * (self.L + x[1]/2)
-        tau2 = M * R / jj
-        tau1 = self.P / (np.sqrt(2) * x[0]*x[1])
-        tau = np.sqrt(tau1**2 + 2*tau1*tau2*x[1]/(2*R) + tau2**2)
-
-        g1 = tau - self.tau_max
-        g2 = xichma_z - self.xichma_max
-        g3 = theta_z - self.theta_max
-        g4 = x[0] - x[3]
-        g5 = self.P - Pc
-        g6 = 0.125 - x[0]
-        g7 = 1.10471 * x[0]**2 + 0.04811 * x[2]*x[3]*(14 + x[1]) - 5
-        return np.array([g1, g2, g3, g4, g5, g6, g7])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class CantileverBeamProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4, x5]
-    """
-
-    name = "Cantilever beam design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 5
-        self._n_objs = 1
-        self._n_cons = 1
-        self._bounds = [(0.01, 100.0), ] * 5
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        f1 = 0.6224 * np.sum(x)
-        return np.array([f1, ])
-
-    def get_cons(self, x):
-        g1 = 61 / x[0]**3 + 27/x[1]**3 + 19/x[2]**3 + 7/x[3]**3 + 1/x[4]**3
-        return np.array([g1, ])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class SpeedReducerProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4, x5, x6, x7]
-
-    Ref: https://www.hindawi.com/journals/mpe/2013/419043/
-    """
-
-    name = "Speed reducer design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 7
-        self._n_objs = 1
-        self._n_cons = 11
-        self._bounds = [(2.6, 3.6), (0.7, 0.8), (17, 28), (7.3, 8.3), (7.8, 8.3), (2.9, 3.9), (5.0, 5.5)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        f1 = 0.7584*x[0]*x[1]**2*(3.3333*x[2]**2 + 14.9334*x[2]-43.0934) - 1.508*x[0]*(x[5]**2+x[6]**2) + 7.4777*(x[5]**3 + x[6]**3) + 0.7854*(x[3]*x[5]**2 + x[4]*x[6]**2)
-        return np.array([f1, ])
-
-    def get_cons(self, x):
-        g1 = 27/(x[0]*x[1]**2*x[2]) - 1
-        g2 = 397.5 / (x[0]*x[1]**2*x[2]**2) - 1
-        g3 = 1.93*x[3]**3/ (x[1] * x[2]*x[5]**4) - 1
-        g4 = 1.93 * x[4]**3 / (x[1] * x[2] * x[6]**4) - 1
-        g5 = np.sqrt((745*x[3]/(x[1]*x[2]))**2 + 16.9*10**6) / (110*x[5]**3) - 1
-        g6 = np.sqrt((745*x[4]/(x[1]*x[2]))**2 - 157.5*10**6) / (85 * x[6]**3) - 1
-        g7 = x[1]*x[2]/40 - 1
-        g8 = 5*x[1]/x[0] - 1
-        g9 = x[0]/(12 * x[1]) - 1
-        g10 = (1.5*x[5] + 1.9) / x[3] - 1
-        g11 = (1.1*x[6] + 1.9) / x[4] -1
-        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9, g10, g11])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class RollingElementBearingProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4, x5, x6, x7, x8, x9, x10] = [Dm, Db, Z, fi, f0, Kdmin, Kdmax, theta, e, C]
-    """
-
-    name = "Rolling element bearing design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 10
-        self._n_objs = 1
-        self._n_cons = 9
-        self.D = 160
-        self.d = 90
-        self.Bw = 30
-        self.ri = self.ro = 11.033
-        self._bounds = [(125., 150.), (10.5, 31.5), (4, 50), (0.515, 0.6), (0.515, 0.6), (0.4, 0.5), (0.6, 0.7), (0.3, 0.4), (0.02, 0.1), (0.6, 0.85)]
-        self.check_penalty_func(f_penalty)
-
-    def amend_position(self, x, lb=None, ub=None):
-        x[2] = int(x[2])
-        return x
-
-    def get_objs(self, x):
-        gama = x[1] / x[0]
-        t1 = 37.91*(1+(1.04*((1-gama)/(1+gama))**1.72*(x[3]/x[4] * (2*x[4] - 1)/(2*x[3] - 1))**0.41)**(10./3))**(-0.3)
-        fc = t1 * (gama**0.3 *(1 - gama)**1.39 / ((1+gama)**(1./3))) * (2*x[3]/(2*x[3] - 1))**0.41
-        if x[1] <= 25.4:
-            f1 = fc * x[2]**(2./3) * x[1]**1.8
-        else:
-            f1 = 3.647 * fc * x[2]**(2./3) * x[1]**1.4
-        return np.array([f1, ])
-
-    def get_cons(self, x):
-        T = self.D - self.d - 2*x[1]
-        xx = ((self.D - self.d) / 2 - 3 * (T/4))**2 + (self.D/2 - T/4 - x[1])**2 - (self.d/2 + T/4)**2
-        yy = 2*((self.D - self.d)/2 - 3*T/4)*(self.D/2 - T/4 - x[1])
-        theta0 = 2*np.pi - 1. / np.cos(xx / yy)
-
-        g1 = theta0 / (2. / np.sin(x[1] / x[0])) - x[2] + 1
-        g2 = x[5]*(self.D - self.d) - 2*x[1]
-        g3 = 2*x[1] - x[6]*(self.D - self.d)
-        g4 = x[-1]*self.Bw - x[1]
-        g5 = 0.5*(self.D + self.d) - x[0]
-        g6 = x[0] - (0.5 + x[-2])*(self.D + self.d)
-        g7 = x[-3]*x[1] - 0.5*(self.D - x[0] - x[1])
-        g8 = 0.515 - x[3]
-        g9 = 0.515 - x[4]
-        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-TCSP = TensionCompressionSpringProblem
-WBP = WeldedBeamProblem
-CBP = CantileverBeamProblem
-SRP = SpeedReducerProblem
-REBP = RollingElementBearingProblem
+#!/usr/bin/env python
+# Created by "Thieu" at 16:25, 09/05/2023 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+# Paper: IHAOAVOA: An improved hybrid aquila optimizer and African vultures optimization algorithm for global optimization problems
+
+import numpy as np
+from enoppy.engineer import Engineer
+
+
+class TensionCompressionSpringProblem(Engineer):
+    """
+    x = [x1, x2, x3] = [d, D, N]
+    """
+
+    name = "Tension/compression spring design problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 3
+        self._n_objs = 1
+        self._n_cons = 4
+        self._bounds = [(0.05, 2.0), (0.25, 1.3), (2.0, 15.0)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = (x[2] + 2) * x[1]*x[0]**2
+        return np.array([f1, ])
+
+    def get_cons(self, x):
+        g1 = 1 - (x[1]**3 * x[2]) / (71785 * x[0]**4)
+        g2 = (4*x[1]**2 - x[0]*x[1])/(12566 * (x[1]*x[0]**3 - x[0]**4)) + 1. / (5108 * x[0]**2)
+        g3 = 1 - 140.45*x[0] / (x[1]**2 * x[2])
+        g4 = (x[0] + x[1]) / 1.5 - 1
+        return np.array([g1, g2, g3, g4])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class WeldedBeamProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4] = [h, l, t, b]
+    """
+
+    name = "Welded beam design problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 7
+        self._bounds = [(0.1, 2.0), (0.1, 10.), (0.1, 10.), (0.1, 2.0)]
+        self.L = 14
+        self.E = 30*10**6
+        self.G = 12*10**6
+        self.theta_max = 0.25
+        self.tau_max = 13600
+        self.xichma_max = 30000
+        self.P = 6000
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 1.10471 * x[0]**2 * x[1] + 0.04811 * x[2] * x[3] * (14 + x[1])
+        return np.array([f1, ])
+
+    def get_cons(self, x):
+        Pc = 4.013*self.E*np.sqrt(x[2]**2 * x[3]**6 / 36) / self.L**2 * (1 - x[2]*np.sqrt(self.E/(4*self.G)) / (2*self.L))
+        theta_z = 6 * self.P * self.L**3 / (self.E * x[2]**2 * x[3])
+        xichma_z = 6*self.P*self.L / (self.E * x[2]**2 * x[3])
+        jj = 2*np.sqrt(2)*x[0]*x[1]*(x[1]**2 / 4 + ((x[0] + x[2])/2)**2)
+        R = np.sqrt(x[1]**2/4 + (x[0]+x[2])**2 / 4)
+        M = self.P * (self.L + x[1]/2)
+        tau2 = M * R / jj
+        tau1 = self.P / (np.sqrt(2) * x[0]*x[1])
+        tau = np.sqrt(tau1**2 + 2*tau1*tau2*x[1]/(2*R) + tau2**2)
+
+        g1 = tau - self.tau_max
+        g2 = xichma_z - self.xichma_max
+        g3 = theta_z - self.theta_max
+        g4 = x[0] - x[3]
+        g5 = self.P - Pc
+        g6 = 0.125 - x[0]
+        g7 = 1.10471 * x[0]**2 + 0.04811 * x[2]*x[3]*(14 + x[1]) - 5
+        return np.array([g1, g2, g3, g4, g5, g6, g7])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class CantileverBeamProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4, x5]
+    """
+
+    name = "Cantilever beam design problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 5
+        self._n_objs = 1
+        self._n_cons = 1
+        self._bounds = [(0.01, 100.0), ] * 5
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 0.6224 * np.sum(x)
+        return np.array([f1, ])
+
+    def get_cons(self, x):
+        g1 = 61 / x[0]**3 + 27/x[1]**3 + 19/x[2]**3 + 7/x[3]**3 + 1/x[4]**3
+        return np.array([g1, ])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class SpeedReducerProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4, x5, x6, x7]
+
+    Ref: https://www.hindawi.com/journals/mpe/2013/419043/
+    """
+
+    name = "Speed reducer design problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 7
+        self._n_objs = 1
+        self._n_cons = 11
+        self._bounds = [(2.6, 3.6), (0.7, 0.8), (17, 28), (7.3, 8.3), (7.8, 8.3), (2.9, 3.9), (5.0, 5.5)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 0.7584*x[0]*x[1]**2*(3.3333*x[2]**2 + 14.9334*x[2]-43.0934) - 1.508*x[0]*(x[5]**2+x[6]**2) + 7.4777*(x[5]**3 + x[6]**3) + 0.7854*(x[3]*x[5]**2 + x[4]*x[6]**2)
+        return np.array([f1, ])
+
+    def get_cons(self, x):
+        g1 = 27/(x[0]*x[1]**2*x[2]) - 1
+        g2 = 397.5 / (x[0]*x[1]**2*x[2]**2) - 1
+        g3 = 1.93*x[3]**3/ (x[1] * x[2]*x[5]**4) - 1
+        g4 = 1.93 * x[4]**3 / (x[1] * x[2] * x[6]**4) - 1
+        g5 = np.sqrt((745*x[3]/(x[1]*x[2]))**2 + 16.9*10**6) / (110*x[5]**3) - 1
+        g6 = np.sqrt((745*x[4]/(x[1]*x[2]))**2 - 157.5*10**6) / (85 * x[6]**3) - 1
+        g7 = x[1]*x[2]/40 - 1
+        g8 = 5*x[1]/x[0] - 1
+        g9 = x[0]/(12 * x[1]) - 1
+        g10 = (1.5*x[5] + 1.9) / x[3] - 1
+        g11 = (1.1*x[6] + 1.9) / x[4] -1
+        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9, g10, g11])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class RollingElementBearingProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4, x5, x6, x7, x8, x9, x10] = [Dm, Db, Z, fi, f0, Kdmin, Kdmax, theta, e, C]
+    """
+
+    name = "Rolling element bearing design problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 10
+        self._n_objs = 1
+        self._n_cons = 9
+        self.D = 160
+        self.d = 90
+        self.Bw = 30
+        self.ri = self.ro = 11.033
+        self._bounds = [(125., 150.), (10.5, 31.5), (4, 50), (0.515, 0.6), (0.515, 0.6), (0.4, 0.5), (0.6, 0.7), (0.3, 0.4), (0.02, 0.1), (0.6, 0.85)]
+        self.check_penalty_func(f_penalty)
+
+    def amend_position(self, x, lb=None, ub=None):
+        x[2] = int(x[2])
+        return x
+
+    def get_objs(self, x):
+        gama = x[1] / x[0]
+        t1 = 37.91*(1+(1.04*((1-gama)/(1+gama))**1.72*(x[3]/x[4] * (2*x[4] - 1)/(2*x[3] - 1))**0.41)**(10./3))**(-0.3)
+        fc = t1 * (gama**0.3 *(1 - gama)**1.39 / ((1+gama)**(1./3))) * (2*x[3]/(2*x[3] - 1))**0.41
+        if x[1] <= 25.4:
+            f1 = fc * x[2]**(2./3) * x[1]**1.8
+        else:
+            f1 = 3.647 * fc * x[2]**(2./3) * x[1]**1.4
+        return np.array([f1, ])
+
+    def get_cons(self, x):
+        T = self.D - self.d - 2*x[1]
+        xx = ((self.D - self.d) / 2 - 3 * (T/4))**2 + (self.D/2 - T/4 - x[1])**2 - (self.d/2 + T/4)**2
+        yy = 2*((self.D - self.d)/2 - 3*T/4)*(self.D/2 - T/4 - x[1])
+        theta0 = 2*np.pi - 1. / np.cos(xx / yy)
+
+        g1 = theta0 / (2. / np.sin(x[1] / x[0])) - x[2] + 1
+        g2 = x[5]*(self.D - self.d) - 2*x[1]
+        g3 = 2*x[1] - x[6]*(self.D - self.d)
+        g4 = x[-1]*self.Bw - x[1]
+        g5 = 0.5*(self.D + self.d) - x[0]
+        g6 = x[0] - (0.5 + x[-2])*(self.D + self.d)
+        g7 = x[-3]*x[1] - 0.5*(self.D - x[0] - x[1])
+        g8 = 0.515 - x[3]
+        g9 = 0.515 - x[4]
+        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+TCSP = TensionCompressionSpringProblem
+WBP = WeldedBeamProblem
+CBP = CantileverBeamProblem
+SRP = SpeedReducerProblem
+REBP = RollingElementBearingProblem
```

### Comparing `enoppy-0.1.0/enoppy/paper_based/moeosma_2023.py` & `enoppy-0.1.1/enoppy/paper_based/pdo_2022.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,469 +1,513 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 16:38, 05/05/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-# Paper: Multi‑objective equilibrium optimizer slime mould algorithm and its application in solving engineering problems
-
-import numpy as np
-from enoppy.engineer import Engineer
-from enoppy.utils.encoder import LabelEncoder
-
-
-class SpeedReducerProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4, x5, x6, x7] = [b, m, z, l1, l2, d1, d2]
-    """
-
-    name = "Speed Reducer Design Problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 7
-        self._n_objs = 2
-        self._n_cons = 11
-        self._bounds = [(2.6, 3.6), (0.7, 0.8), (17, 28), (7.3, 8.3), (7.3, 8.3), (2.9, 3.9), (5.0, 5.5)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        f1 = 0.7854*x[0]*x[1]**2*(14.9334*x[2] + 3.3333*x[2]**2 - 43.0934) - 1.508*x[0]*(x[5]**2 + x[6]**2) \
-            + 0.7854*(x[3]*x[5]**2 + x[4]*x[6]**2) + 7.4777*(x[5]**3 + x[6]**3)
-        f2 = np.sqrt((745*x[3]/(x[1]*x[2]))**2 + 16.9*10**6)/(0.1*x[5]**3)
-        return np.array([f1, f2])
-
-    def get_cons(self, x):
-        g1 = 27 / (x[0]*x[2]*x[1]**2) - 1
-        g2 = 397.5 / (x[0]*x[1]**2*x[2]**2) - 1
-        g3 = 1.93*x[3]**3 / (x[1]*x[2]*x[5]**4) - 1
-        g4 = 1.93*x[4]**3 / (x[1]*x[2]*x[6]**4) - 1
-        g5 = x[1]*x[2] / 40 - 1
-        g6 = x[0] / (12*x[1]) - 1
-        g7 = 5*x[1] / x[0] - 1
-        g8 = (1.5*x[5] + 1.9) / x[3] - 1
-        g9 = (1.1*x[6] + 1.9) / x[4] - 1
-        g10 = np.sqrt((745*x[3]/(x[1]*x[2]))**2 + 16.9*10**6)/(0.1*x[5]**3) - 1100 - 1
-        g11 = np.sqrt((745*x[4]/(x[1]*x[2]))**2 + 157.5*10**6)/(0.1*x[6]**3) - 850 - 1
-        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9, g10, g11])
-
-    def amend_position(self, x, lb=None, ub=None):
-        x[2] = int(x[2])
-        return x
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class SpringProblem(Engineer):
-    """
-    x = [x1, x2, x3] = [d, D, N]
-    """
-
-    name = "Spring Design Problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 3
-        self._n_objs = 2
-        self._n_cons = 8
-        self.x0 = [0.009, 0.0095, 0.0104, 0.0118, 0.0128, 0.0132, 0.014,
-              0.015, 0.0162, 0.0173, 0.018, 0.020, 0.023, 0.025,
-              0.028, 0.032, 0.035, 0.041, 0.047, 0.054, 0.063,
-              0.072, 0.080, 0.092, 0.0105, 0.120, 0.135, 0.148,
-              0.162, 0.177, 0.192, 0.207, 0.225, 0.244, 0.263,
-              0.283, 0.307, 0.331, 0.362, 0.394, 0.4375, 0.500]
-        self.le = LabelEncoder()
-        self.le.fit(self.x0)
-        self._bounds = [(0, 41.99), (1.0, 30.0), (1, 32)]
-        self.check_penalty_func(f_penalty)
-
-    def amend_position(self, x, lb=None, ub=None):
-        x[0] = self.le.inverse_transform([int(x[0])])
-        x[2] = int(x[2])
-        return x
-
-    def get_objs(self, x):
-        d, D, N = x
-        G = 11.5 * 10 ** 6
-        K = G * (d ** 4) / (8 * N * (D ** 3))
-        lf = 1.05 * d * (N + 2) + 1000 / K
-        C = D / d
-        cf = (4 * C - 1) / (4 * C - 4) + 0.615 / C
-        f1 =  0.25 * np.pi ** 2 * (d ** 2) * D * (N + 2)
-        f2 = 8000 * cf * D / (np.pi * d ** 3)
-        return np.array([f1, f2])
-
-    def get_cons(self, x):
-        G = 11.5 * 10 ** 6
-        K = G * (x[0] ** 4) / (8 * x[2] * (x[1] ** 3))
-        lf = 1.05 * x[0] * (x[2] + 2) + 1000 / K
-        C = x[0] / x[0]
-        cf = (4 * C - 1) / (4 * C - 4) + 0.615 / C
-        f1 = 0.25 * np.pi ** 2 * (x[0] ** 2) * x[1] * (x[2] + 2)
-        f2 = 8000 * cf * x[1] / (np.pi * x[0] ** 3)
-        g1 = 0.25 * np.pi**2 * x[0]**2 * x[1]*(x[2] + 2) - 30
-        g2 = f2 - 189000
-        g3 = lf - 14
-        g4 = 0.2 - x[0]
-        g5 = x[0] + x[1] - 3
-        g6 = 3 - C
-        g7 = 300 / K - 6
-        g8 = 1.25 - 700/K
-        return np.array([g1, g2, g3, g4, g5, g6, g7, g8])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        if type(x[0]) != int:
-            x = self.amend_position(x, self.lb, self.ub)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class HydrostaticThrustBearingProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4] = [R, R0, mu, Q]
-    """
-
-    name = "Hydrostatic thrust bearing design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 4
-        self._n_objs = 2
-        self._n_cons = 7
-        self.gamma = 0.0307
-        self.g = 386.4
-        self.N = 750
-        self.Ws = 101000
-        self.Pmax = 1000
-        self.DeltaTmax = 50
-        self.hmin = 0.001
-        self.C = 0.5
-        self.C1 = 10.04
-        self.n = -3.55
-        self._bounds = [(1., 16.), (1., 16.), (1e-6, 16e-6), (1., 16.)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        R, R0, mu, Q = x
-        P0 = 6 * mu * Q
-        W = np.pi * P0 / 2
-        P = (np.log10(np.log10(8.122 * 10**6 * mu + 0.8)) - self.C1) / self.n
-        DeltaT = 2 * (10**P - 560)
-        Ef = 9336 * Q * self.gamma * self.C * DeltaT
-        h = (2*np.pi*self.N/60)**2 * 2*np.pi*mu / Ef * (R**4 - R0**4)/4
-        f1 = 1. / 12 * (Q * P0 / 0.7 + Ef)
-        f2 = self.gamma / (self.g * P0) * (Q / (2 * np.pi * R * h))
-        return np.array([f1, f2])
-
-    def get_cons(self, x):
-        R, R0, mu, Q = x
-        P0 = 6 * mu * Q * np.log(R / R0)
-        W = np.pi * P0 / 2
-        P = (np.log10(np.log10(8.122 * 10 ** 6 * mu + 0.8)) - self.C1) / self.n
-        DeltaT = 2 * (10 ** P - 560)
-        Ef = 9336 * Q * self.gamma * self.C * DeltaT
-        h = (2 * np.pi * self.N / 60) ** 2 * 2 * np.pi * mu / Ef * (R ** 4 - R0 ** 4) / 4
-        g1 = self.Ws - W
-        g2 =  P0 - self.Pmax
-        g3 = DeltaT - self.DeltaTmax
-        g4 = self.hmin - h
-        g5 = R0 - R
-        g6 = self.gamma / (self.g * P0) * (Q / (2 * np.pi * R * h)) - 0.001
-        g7 = W / (np.pi * (R ** 2 - R0 ** 2)) - 5000
-        return np.array([g1, g2, g3, g4, g5, g6, g7])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class VibratingPlatformProblem(Engineer):
-    """
-    x = [d1, d2, d3, b, L] = [x0, x1, x2, x3, x4]
-
-    Original Ref: On improving multiobjective genetic algorithms for design optimization
-    """
-
-    name = "Vibrating platform design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 5
-        self._n_objs = 2
-        self._n_cons = 5
-        # Define constants
-        self.E1 = 70 * 10 ** 9
-        self.E2 = 1.6 * 10 ** 9
-        self.E3 = 200 * 10 ** 9
-        self.rho1 = 2770
-        self.rho2 = 100
-        self.rho3 = 7780
-        self.c1 = 1500
-        self.c2 = 500
-        self.c3 = 800
-        self._bounds = [(0.05, 0.5), (0.2, 0.5), (0.2, 0.6), (0.35, 0.5), (3, 6)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        d1, d2, d3, b, L = x
-        EI = (2*b/3)*(self.E1*d1**3 - self.E2*(d1**3 - d2**3) - self.E3*(d2**3 - d3**3))
-        mu = 2*b*(self.rho1*d1 - self.rho2*(d1 - d2) - self.rho3*(d2 - d3))
-        f1 = -np.pi/(2*L**2) * np.sqrt(EI / mu)
-        f2 = 2 * b * L * (self.c1 * d1 - self.c2 * (d1 - d2) - self.c3 * (d2 - d3))
-        return np.array([f1, f2])
-
-    def get_cons(self, x):
-        d1, d2, d3, b, L = x
-        mu = 2 * b * (self.rho1 * d1 - self.rho2 * (d1 - d2) - self.rho3 * (d2 - d3))
-        g1 = mu * L - 2800
-        g2 = d1 - d2
-        g3 = d2 - d1 - 0.15
-        g4 = d2 - d3
-        g5 = d3 - d2 - 0.01
-        return np.array([g1, g2, g3, g4, g5])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class CarSideImpactProblem(Engineer):
-    """
-    x = [x1, x2, x3, x4, x5, x6, x7]
-
-    Original Ref:
-    """
-
-    name = "Car side impact design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 7
-        self._n_objs = 3
-        self._n_cons = 10
-        self._bounds = [(0.5, 1.5), (0.45, 1.35), (0.5, 1.5), (0.5, 1.5), (0.875, 2.625), (0.4, 1.2), (0.4, 1.2)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        c1 = np.array([4.90, 6.67, 6.98, 4.01, 1.78, 1e-5, 2.73])
-        V_mbp = 10.58 - 0.67275 * x[1] - 0.674 * x[0] * x[1]
-        V_fd = 16.45 - 0.489 * x[2] * x[6] - 0.843 * x[4]*x[5]
-        f1 = np.dot(c1, x) + 1.98
-        f2 = 4.72 - 0.19 * x[1] * x[2] - 0.5*x[3]
-        f3 = 0.5 * (V_mbp + V_fd)
-        return np.array([f1, f2, f3])
-
-    def get_cons(self, x):
-        V_mbp = 10.58 - 0.67275 * x[1] - 0.674 * x[0] * x[1]
-        V_fd = 16.45 - 0.489 * x[2] * x[6] - 0.843 * x[4] * x[5]
-        g1 = 1.16 - 0.0092928 * x[2] - 0.3717 * x[1] * x[3] - 1
-        g2 = 0.261 - 0.06486 * x[0] + 0.0154464 * x[5] - 0.0159 * x[0] * x[1] - 0.019 * x[1] * x[6] + 0.0144 * x[2] * x[4] - 0.32
-        g3 = 0.214 - 0.0587118 * x[0] + 0.018 * x[1]**2 + 0.030408 * x[2] + 0.00817 * x[4] + 0.03099 * x[1] * x[5] - 0.018 * x[1] * x[6] - 0.00364 * x[4] * x[5] - 0.32
-        g4 = 0.74 - 0.61 * x[1] + 0.227 * x[1]**2 - 0.031296 * x[2] - 0.031872 * x[6] - 0.32
-        g5 = 28.98 + 3.818 * x[2] + 1.27296 * x[5] - 2.68065 * x[6] - 4.2 * x[0] * x[1] - 32
-        g6 = 33.86 - 3.795 * x[1] + 2.95 * x[2] - 3.4431 * x[6] - 5.057 * x[0] * x[1] + 1.45728 - 32
-        g7 = 46.36 - 4.4505 * x[0] - 9.9 * x[1] - 32
-        g8 = 4.72 - 0.19 * x[1] * x[2] - 0.5*x[3] - 4
-        g9 = V_mbp - 9.9
-        g10 = V_fd - 15.7
-        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9, g10])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class WaterResourceManagementProblem(Engineer):
-    """
-    x =  [x1, x2, x3]
-
-    Original Ref:
-    """
-
-    name = "Water resource management problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 3
-        self._n_objs = 5
-        self._n_cons = 7
-        self._bounds = [(0.01, 0.45), (0.01, 0.1), (0.01, 0.1)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        f1 = 106780.37*(x[1] + x[2]) + 61704.67
-        f2 = 3000*x[0]
-        f3 = 30570 * 2289*x[1]/ (0.06 * 2289)**0.65
-        f4 = 250 * 2289 * np.exp(2.74 - 39.75*x[1] + 9.9*x[2])
-        f5 = 25*(1.39/ (x[0]*x[1]) + 4940*x[2] - 80)
-        return np.array([f1, f2, f3, f4, f5])
-
-    def get_cons(self, x):
-        t = x[0] * x[1]
-        g1 = 4.94*x[2] + 0.00139/ t - 1.08
-        g2 = 1.082*x[2] + 0.000306/ t - 1.0986
-        g3 = 49408.24*x[2] + 12.307/t - 54051.02
-        g4 = 8046.33*x[2] + 2.098 / t - 16696.71
-        g5 = 7883.39*x[2] + 2.138/t - 10705.04
-        g6 = 1721.26*x[2] + 0.417*t - 2136.54
-        g7 = 631.13*x[2] + 0.164/t - 604.48
-        return np.array([g1, g2, g3, g4, g5, g6, g7])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class BulkCarriersProblem(Engineer):
-    """
-    x = [L, B, D, T, Vk, CB] = [x1, x2, x3, x4, x5, x6]
-
-    Original Ref:
-    """
-
-    name = "Bulk carriers design problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 6
-        self._n_objs = 3
-        self._n_cons = 9
-        self._bounds = [(150, 274.32), (20, 32.31), (13, 25), (10, 11.71), (14., 18.), (0.63, 0.75)]
-        self.check_penalty_func(f_penalty)
-
-    def get_objs(self, x):
-        L, B, D, T, Vk, CB = x
-        # Calculate intermediate variables
-        Sd = 5000 * Vk / 24
-        Ws = 0.034 * L ** 1.7 * B ** 0.7 * D ** 0.4 * CB ** 0.5
-        Wo = L ** 0.8 * B ** 0.6 * D ** 0.3 * CB ** 0.1
-        a = 4456.51 - 8105.61 * CB + 4977.06 * CB ** 2
-        b = -6960.32 + 12817 * CB - 10847.2 * CB ** 2
-        Fn = 0.5144 * Vk / (9.8065 * L) ** 0.5
-        P = (1.025 * L * B * T * CB) ** (2. / 3) * Vk ** 3 / (a + b * Fn)
-        Wm = 0.17 * P ** 0.9
-        Wls = Ws + Wo + Wm
-        Dwt = 1.025 * L * B * T * CB - Wls
-        Dc = 0.19 * 24 * P / 1000 + 0.2
-        Dcwt = Dwt - Dc * (Sd + 5) - 2 * Dwt ** 0.5
-        Rtpa = 350 / (Sd + 2 * Dcwt / 8000 + 2 * 0.5)
-        Ca = Dcwt * Rtpa
-        Cv = Rtpa * (105 * Dc * Sd + 6.3 * Dwt ** 0.8)
-        Cr = 40000 * Dwt ** 0.3
-        Cc = 2.6 * (2000 * Ws ** 0.85 + 3500 * Wo + 2400 * P ** 0.8)
-        # Calculate objective functions
-        f1 = (Cc + Cr + Cv) / Ca
-        f2 = Wls
-        f3 = -Ca
-        return np.array([f1, f2, f3])
-
-    def get_cons(self, x):
-        L, B, D, T, Vk, CB = x
-        Ws = 0.034 * L ** 1.7 * B ** 0.7 * D ** 0.4 * CB ** 0.5
-        Wo = L ** 0.8 * B ** 0.6 * D ** 0.3 * CB ** 0.1
-        a = 4456.51 - 8105.61 * CB + 4977.06 * CB ** 2
-        b = -6960.32 + 12817 * CB - 10847.2 * CB ** 2
-        Fn = 0.5144 * Vk / (9.8065 * L) ** 0.5
-        P = (1.025 * L * B * T * CB) ** (2. / 3) * Vk ** 3 / (a + b * Fn)
-        Wm = 0.17 * P ** 0.9
-        Wls = Ws + Wo + Wm
-        Dwt = 1.025 * L * B * T * CB - Wls
-        g1 = -L / B + 6
-        g2 = L / D - 15
-        g3 = -L / T - 19
-        g4 = T - 0.45 * Dwt ** 0.31
-        g5 = T - 0.7 * D - 0.7
-        g6 = Fn - 0.32
-        g7 = -0.53 * T - ((0.085 * CB - 0.002) * B ** 2) / (T * CB) + (1 + 0.52 * D) + 0.07 * B
-        g8 = -Dwt + 3000
-        g9 = Dwt - 500000
-        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-class MultiProductBatchPlantProblem(Engineer):
-    """
-    x = [N1, N2, N3, V1, V2, V3, TL1, TL2, B1, B2] = [x1, x2, x3, x4, x5, x6, x7, x8, x9, x10]
-
-    Original Ref:
-    """
-
-    name = "Multi-product batch plant problem"
-
-    def __init__(self, f_penalty=None):
-        super().__init__()
-        self._n_dims = 10
-        self._n_objs = 3
-        self._n_cons = 3
-        self.N = 2
-        self.M = 3
-        self.alpha = np.array([250, 250, 250])
-        self.beta = np.array([0.6, 0.6, 0.6])
-        self.H = 6000
-        self.Q = np.array([40000, 20000])
-        self.S = np.array([[2, 3, 4], [4, 6, 3]])
-        self.t = np.array([[8, 20, 8], [16, 4, 4]])
-        self._bounds = [(1, 3.99)] * self.N + [(250, 2500)] * self.M + [(6, 20), (4, 16), (40, 700), (10, 450)]
-        self.check_penalty_func(f_penalty)
-
-    def amend_position(self, x, lb=None, ub=None):
-        x[0] = int(x[0])
-        x[1] = int(x[1])
-        x[2] = int(x[2])
-        return x
-
-    def get_objs(self, x):
-        f1 = np.sum(self.alpha * x[:self.M] * (x[self.M:2*self.M] ** self.beta))
-        f2 = 65 * (self.Q[0]/x[8] + self.Q[1]/x[9]) + 0.08*self.Q[0] + 0.1*self.Q[1]
-        f3 = self.Q[0] * x[6] / x[8] + self.Q[2] * x[7] / x[9]
-        return np.array([f1, f2, f3])
-
-    def get_cons(self, x):
-        g1 = self.Q[0] * x[6] / x[8] + self.Q[2] * x[7] / x[9] - self.H
-        b = np.array(x[-2:])
-        v = np.array(x[self.M:2*self.M])
-        g2 = np.sum(b*self.S - v)
-        g3 = np.sum([self.t[i,j] - x[j] * x[2*self.M+i+self.N] for i in range(self.N) for j in range(self.N, 2*self.M)])
-        return np.array([g1, g2, g3])
-
-    def evaluate(self, x):
-        self.n_fe += 1
-        self.check_solution(x)
-        list_objs = self.get_objs(x)
-        list_cons = self.get_cons(x)
-        return self.f_penalty(list_objs, list_cons)
-
-
-SRP = SpeedReducerProblem
-SP = SpringProblem
-HTBP = HydrostaticThrustBearingProblem
-VPP = VibratingPlatformProblem
-CSP = CarSideImpactProblem
-WRMP = WaterResourceManagementProblem
-BCP = BulkCarriersProblem
-MPBPP = MultiProductBatchPlantProblem
+#!/usr/bin/env python
+# Created by "Thieu" at 15:00, 29/07/2022 ----------%
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+# Paper: Prairie Dog Optimization Algorithm (PDO-2022)
+
+import numpy as np
+from enoppy.engineer import Engineer
+from enoppy.utils.encoder import LabelEncoder
+
+
+class WeldedBeamProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4]
+
+    WBD is subjected to 4 design constraints: shear, beam blending stress, bar buckling load beam, and deflection
+    variables: h=x1, l=x2, t=x3, b=x4
+    l: length, h: height, t: thickness, b: weld thickness of the bar
+
+    https://sci-hub.se/10.1016/s0166-3615(99)00046-9
+    """
+
+    name = "Welded Beam Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 11
+        self._bounds = [(0.1, 2.), (0.1, 10.), (0.1, 10.), (0.1, 2.)]
+        self.xichma_max = 30000
+        self.P = 6000
+        self.L = 14
+        self.delta_max = 0.25
+        self.E = 30 * 10 ** 6
+        self.theta_max = 13600
+        self.G = 12 * 10 ** 6
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = x[0] ** 2 * x[1] * 1.10471 + 0.04811 * x[2] * x[3] * (14.0 + x[1])
+        return np.array([f1])
+
+    def get_cons(self, x):
+        Pc_X = 4.013 * self.E * np.sqrt(x[2] ** 2 * x[3] ** 6 / 36) / self.L ** 2 * (1. - x[2] * np.sqrt(self.E / (4 * self.G)) / (2 * self.L))
+        J = 2 * (np.sqrt(2) * x[0] * x[1] * (x[1] ** 2 / 4 + (x[0] + x[2] / 2) ** 2))
+        M = self.P * (self.L + x[1] / 2)
+        R = np.sqrt(x[1] ** 2 / 4 + (x[0] + x[2]) ** 2 / 4)
+        t2 = M * R / J
+        t1 = self.P / (np.sqrt(2) * x[0] * x[1])
+        t_X = np.sqrt(t1 ** 2 + 2 * t1 * t2 * x[1] / (2 * R) + t2 ** 2)
+        xichma_X = 6 * self.P * self.L / (x[3] * x[2] ** 2)
+        delta_X = 4 * self.P * self.L ** 3 / (self.E * x[2] ** 3 * x[3])
+        g1 = t_X - self.theta_max
+        g2 = xichma_X - self.xichma_max
+        g3 = x[0] - x[3]
+        g4 = 0.10471 * x[0] ** 2 + 0.04811 * x[2] * x[3] * (14.0 + x[1]) - 5.0
+        g5 = 0.125 - x[0]
+        g6 = delta_X - self.delta_max
+        g7 = self.P - Pc_X
+        return np.array([g1, g2, g3, g4, g5, g6, g7])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class PressureVesselProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4]
+
+    Variables: the inner radius (R=x3), the thickness of the head (Th=x2),
+        the length of the cylindrical section of the vessel (L=x4), and the thickness of the shell (Ts=x1)
+
+    https://sci-hub.se/10.1115/1.2912596
+    """
+
+    name = "Pressure Vessel Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 4
+        self._bounds = [(0., 99.), (0., 99.), (10., 200.), (10., 200.)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 0.6224 * x[2] * x[0] * x[3] + 1.7781 * x[2] ** 2 * x[1] + 3.1611 * x[0] ** 2 * x[3] + 19.8621 * x[2] * x[0] ** 2
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = -x[0] + 0.0193 * x[2]
+        g2 = -x[2] + 0.00954 * x[2]
+        g3 = -np.pi * x[1] ** 2 * x[3] - 4. / 3 * np.pi * x[2] ** 3 + 750 * 1728
+        g4 = -240 + x[3]
+        return np.array([g1, g2, g3, g4])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class CompressionSpringProblem(Engineer):
+    """
+    x = [x1, x2, x3, x4]
+
+    CSD aims to minimize the weight of a tension/compression spring given the values of 3 parameters:
+        the wire diameter (d=x1), number of active coils (P=x3), and mean coil diameter (D=x2).
+
+    https://sci-hub.se/10.1016/s0166-3615(99)00046-9
+    """
+
+    name = "Compression Spring Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 3
+        self._n_objs = 1
+        self._n_cons = 4
+        self._bounds = [(0.05, 2.), (0.25, 1.3), (2., 15.)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = (x[2] + 2)*x[1]*x[0]**2
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = 1 - x[1] ** 3 * x[2] / (71785 * x[0] ** 4)
+        g2 = (4 * x[1] ** 2 - x[0] * x[1]) / (12566 * (x[2] * x[0] ** 3 - x[0] ** 4)) + 1. / (5108 * x[0] ** 2) - 1
+        g3 = 1 - 140.45 * x[0] / (x[1] ** 2 * x[2])
+        g4 = (x[0] + x[1]) / 1.5 - 1
+        return np.array([g1, g2, g3, g4])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class SpeedReducerProblem(Engineer):
+    """
+    Depicts a gearbox that sits between the propeller and engine of an aeroplane
+    [x1, x2, x3, x4, x5, x6, x7] = [b, m, z, l1, l2, d1, d2]
+    """
+
+    name = "Speed Reducer Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 7
+        self._n_objs = 1
+        self._n_cons = 11
+        self._bounds = [(2.6, 3.6), (0.7, 0.8), (17, 28.99), (7.3, 8.3), (7.3, 8,3), (2.9, 3.9), (5.0, 5.5)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 0.7854*x[0]*x[1]**2*(3.3333*x[2]**2 + 14.9334*x[2] - 43.0934) - 1.508*x[0]*(x[5]**2 + x[6]**2) +\
+            7.4777*(x[5]**3 + x[6]**3) + 0.7854*(x[3]*x[5]**2 + x[4]*x[6]**2)
+        return np.array([f1])
+
+    def amend_position(self, x, lb=None, ub=None):
+        x[2] = int(x[2])
+        return x
+
+    def get_cons(self, x):
+        g1 = 27. / (x[0] * x[1] ** 2 * x[2]) - 1
+        g2 = 397.5 / (x[0] * x[1] ** 2 * x[2] ** 2) - 1
+        g3 = 1.93 * x[3] ** 2 / (x[1] * x[5] ** 4 * x[2]) - 1
+        g4 = 1.93 * x[4] ** 2 / (x[1] * x[6] ** 4 * x[2]) - 1
+        g5 = np.sqrt((745 * x[3] / (x[1] * x[2])) ** 2 + 16 * 10 ** 6) / (110 * x[5] ** 3) - 1
+        g6 = np.sqrt((745 * x[4] / (x[1] * x[2])) ** 2 + 157.5 * 10 ** 6) / (85 * x[6] ** 3) - 1
+        g7 = x[1] * x[2] / 40 - 1
+        g8 = 5 * x[1] / x[0] - 1
+        g9 = x[0] / (12. * x[1]) - 1
+        g10 = (1.5 * x[5] + 1.9) / x[3] - 1
+        g11 = (1.1 * x[6] + 1.9) / x[4] - 1
+        return np.array([g1, g2, g3, g4, g5, g6, g7, g8, g9, g10, g11])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class ThreeBarTrussProblem(Engineer):
+    """
+    Minimize three-bar structure weight subject to supporting a total load P acting vertically downwards
+
+    [x1, x2]
+    """
+
+    name = "Three Bar Truss Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 2
+        self._n_objs = 1
+        self._n_cons = 3
+        self._bounds = [(0., 1.0), (0., 1.)]
+        self.L = 100
+        self.P = 2
+        self.xichma = 2
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = (2*np.sqrt(2)*x[0] + x[1]) * self.L
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = (np.sqrt(2) * x[0] + x[1]) / (np.sqrt(2) * x[0] ** 2 + 2 * x[0] * x[1]) * self.P - self.xichma
+        g2 = x[1] * self.P / (np.sqrt(x[0] ** 2 + 2 * x[0] * x[1])) - self.xichma
+        g3 = self.P / (np.sqrt(2) * x[1] + x[0]) - self.xichma
+        return np.array([g1, g2, g3])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class GearTrainProblem(Engineer):
+    """
+    Unconstrained discrete design optimization problem
+        [x1, x2, x3, x4] = [n_A, n_B, n_C, n_D]
+    """
+
+    name = "Gear Train Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 0
+        self._bounds = [(12, 60.99), (12, 60.99), (12, 60.99), (12, 60.99)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = (1. / 6.931 - x[2]*x[1] / (x[0] * x[3]))**2
+        return np.array([f1])
+
+    def amend_position(self, x, lb=None, ub=None):
+        return np.asarray(x, int)
+
+    def get_cons(self, x):
+        return np.array([])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class CantileverBeamProblem(Engineer):
+    """
+    Minimize a cantilever beam's weight.
+        [x1, x2, x3, x4, x5]
+    """
+
+    name = "Cantilever Beam Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 5
+        self._n_objs = 1
+        self._n_cons = 1
+        self._bounds = [(0.01, 100.),] * 5
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 0.0624 * np.sum(x)
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = 61./x[0]**3 + 37./x[1]**3 + 19./x[2]**3 + 7./x[3]**3 + 1./x[4]**3 - 1
+        return np.array([g1, ])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class IBeamProblem(Engineer):
+    """
+    Minimizes the vertical deflection of a beam
+        [x1, x2, x3, x4] = [b, h, t_w, t_f]
+    """
+
+    name = "I Beam Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 2
+        self._bounds = [(10, 50.), (10, 80.), (0.9, 5.), (0.9, 5.)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 500. / ( (x[2]*(x[1]-2*x[3])**3)/12 + (x[0]*x[3]**3/6) + 2*x[0]*x[3]*(x[1] - x[3])**2 )
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = 2 * x[0] * x[2] + x[2] * (x[1] - 2 * x[3]) - 300
+        g2 = (18 * x[1] * 10 ** 4) / (x[2] * (x[1] - 2 * x[3]) ** 3 + 2 * x[0] * x[2] * (4 * x[3] ** 2 + 3 * x[1] * (x[1] - 2 * x[3]))) + \
+             15 * x[0] * 10 ** 3 / ((x[1] - 2 * x[3]) * x[2] ** 2 + 2 * x[2] * x[0] ** 3) - 56
+        return np.array([g1, g2])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class TubularColumnProblem(Engineer):
+    """
+    [x1, x2] = [d, t]
+
+    https://apmonitor.com/me575/index.php/Main/TubularColumn
+    """
+
+    name = "Tubular Column Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 2
+        self._n_objs = 1
+        self._n_cons = 6
+        self._bounds = [(2., 14.), (0.2, 0.8)]
+        self.xichma_y = 450
+        self.E = 0.65 * 10 ** 6
+        self.P = 2300
+        self.pro = 0.002
+        self.L = 300
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 9.8*x[0]*x[1] + 2*x[0]
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = self.P / (np.pi * x[0] * x[1] * self.xichma_y) - 1
+        g2 = (8 * self.P * self.L ** 2) / (np.pi ** 3 * self.E * x[0] * x[1] * (x[0] ** 2 + x[1] ** 2)) - 1
+        g3 = 2. / x[0] - 1
+        g4 = x[0] / 14 - 1
+        g5 = 0.2 / x[1] - 1
+        g6 = x[1] / 8 - 1
+        return np.array([g1, g2, g3, g4, g5, g6])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class PistonLeverProblem(Engineer):
+    """
+    [x1, x2, x3, x4] = [H, B, D, X]
+    """
+
+    name = "Piston Lever Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 4
+        self._bounds = [(0.05, 500), (0.05, 500.), (0.05, 120.), (0.05, 500.)]
+        self.L = 240
+        self.M_max = 1.8 * 10 ** 6
+        self.P = 1500
+        self.Q = 10000
+        self.theta = np.pi / 4
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        L1 = np.sqrt((x[3] - x[1]) ** 2 + x[0] ** 2)
+        L2 = np.sqrt((x[3] * np.sin(self.theta) + x[0]) ** 2 + (x[1] - x[3] * np.cos(self.theta)) ** 2)
+        f1 = 0.25*np.pi*x[2]**2 * (L2 - L1)
+        return np.array([f1])
+
+    def get_cons(self, x):
+        L1 = np.sqrt((x[3] - x[1]) ** 2 + x[0] ** 2)
+        L2 = np.sqrt((x[3] * np.sin(self.theta) + x[0]) ** 2 + (x[1] - x[3] * np.cos(self.theta)) ** 2)
+        R = np.abs(-x[3] * (x[3] * np.sin(self.theta) + x[0]) + x[0] * (x[1] - x[3] * np.cos(self.theta))) / np.sqrt((x[3] - x[1]) ** 2 + x[0] ** 2)
+        F = np.pi * self.P * x[2] ** 2 / 4
+        g1 = self.Q * self.L * np.cos(self.theta) - R * F
+        g2 = self.Q * (self.L - x[3]) - self.M_max
+        g3 = 1.2 * (L2 - L1) - L1
+        g4 = x[2] / 2 - x[1]
+        return np.array([g1, g2, g3, g4])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class CorrugatedBulkheadProblem(Engineer):
+    """
+    [x1, x2, x3, x4] = [width, depth, length, thickness]
+    """
+
+    name = "Corrugated Bulkhead Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 4
+        self._n_objs = 1
+        self._n_cons = 6
+        self._bounds = [(0., 100), (0., 100.), (0., 100.), (0., 5.)]
+        self.check_penalty_func(f_penalty)
+
+    def get_objs(self, x):
+        f1 = 5.885*x[3]*(x[0] + x[2]) / (x[0] + np.sqrt(np.abs(x[2]**2 - x[1]**2)))
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = -x[3] * x[2] * (0.4 * x[0] + x[2] / 6) + 8.94 * (x[0] + np.sqrt(np.abs(x[2] ** 2 - x[1] ** 2)))
+        g2 = -x[3] * x[1] ** 2 * (0.2 * x[0] + x[2] / 12) + 2.2 * (8.94 * (x[0] + np.sqrt(np.abs(x[2] ** 2 - x[1] ** 2)))) ** (4. / 3)
+        g3 = -x[3] + 0.0156 * x[0] + 0.15
+        g4 = -x[3] + 0.0156 * x[2] + 0.15
+        g5 = -x[3] + 1.05
+        g6 = -x[2] + x[1]
+        return np.array([g1, g2, g3, g4, g5, g6])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+class ReinforcedConcreateBeamProblem(Engineer):
+    """
+    [x1, x2, x3]
+    """
+
+    name = "Reinforced Concreate Beam Design Problem"
+
+    def __init__(self, f_penalty=None):
+        super().__init__()
+        self._n_dims = 3
+        self._n_objs = 1
+        self._n_cons = 2
+        self.x0 = [6.0, 6.16, 6.32, 6.6, 7.0, 7.11, 7.2, 7.8, 7.9, 8.0, 8.4]
+        self.le = LabelEncoder()
+        self.le.fit(self.x0)
+        self._bounds = [(0., 10.99), (28., 40.99), (5., 10.)]
+        self.check_penalty_func(f_penalty)
+
+    def amend_position(self, x, lb=None, ub=None):
+        x[0] = self.le.inverse_transform([int(x[0])])
+        x[1] = int(x[1])
+        return x
+
+    def get_objs(self, x):
+        f1 = 2.9*x[0] + 0.6*x[1]*x[2]
+        return np.array([f1])
+
+    def get_cons(self, x):
+        g1 = x[1] / x[2] - 4
+        g2 = 180 + 7.375 * x[0] ** 2 / x[2] - x[0] * x[1]
+        return np.array([g1, g2])
+
+    def evaluate(self, x):
+        self.n_fe += 1
+        self.check_solution(x)
+        if type(x[0]) != int:
+            x = self.amend_position(x, self.lb, self.ub)
+        list_objs = self.get_objs(x)
+        list_cons = self.get_cons(x)
+        return self.f_penalty(list_objs, list_cons)
+
+
+WBP = WeldedBeamProblem
+PVP = PressureVesselProblem
+CSP = CompressionSpringProblem
+SRD = SpeedReducerProblem
+TBTD = ThreeBarTrussProblem
+GTD = GearTrainProblem
+CBD = CantileverBeamProblem
+IBD = IBeamProblem
+TCD = TubularColumnProblem
+PLD = PistonLeverProblem
+CBHD = CorrugatedBulkheadProblem
+RCB = ReinforcedConcreateBeamProblem
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `enoppy-0.1.0/enoppy/utils/encoder.py` & `enoppy-0.1.1/enoppy/utils/encoder.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 13:58, 09/05/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-
-
-class LabelEncoder:
-    """
-    Encode categorical features as integer labels.
-    """
-
-    def __init__(self):
-        self.unique_labels = None
-        self.label_to_index = {}
-
-    def fit(self, y):
-        """
-        Fit label encoder to a given set of labels.
-
-        Parameters:
-        -----------
-        y : array-like
-            Labels to encode.
-        """
-        self.unique_labels = np.unique(y)
-        self.label_to_index = {label: i for i, label in enumerate(self.unique_labels)}
-
-    def transform(self, y):
-        """
-        Transform labels to encoded integer labels.
-
-        Parameters:
-        -----------
-        y : array-like
-            Labels to encode.
-
-        Returns:
-        --------
-        encoded_labels : array-like
-            Encoded integer labels.
-        """
-        if self.unique_labels is None:
-            raise ValueError("Label encoder has not been fit yet.")
-        return np.array([self.label_to_index[label] for label in y])
-
-    def fit_transform(self, y):
-        """Fit label encoder and return encoded labels.
-
-        Parameters
-        ----------
-        y : array-like of shape (n_samples,)
-            Target values.
-
-        Returns
-        -------
-        y : array-like of shape (n_samples,)
-            Encoded labels.
-        """
-        self.fit(y)
-        return self.transform(y)
-
-    def inverse_transform(self, y):
-        """
-        Transform integer labels to original labels.
-
-        Parameters:
-        -----------
-        y : array-like
-            Encoded integer labels.
-
-        Returns:
-        --------
-        original_labels : array-like
-            Original labels.
-        """
-        if self.unique_labels is None:
-            raise ValueError("Label encoder has not been fit yet.")
-        return np.array([self.unique_labels[i] if i in self.label_to_index.values() else "unknown" for i in y])
+#!/usr/bin/env python
+# Created by "Thieu" at 13:58, 09/05/2023 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+
+
+class LabelEncoder:
+    """
+    Encode categorical features as integer labels.
+    """
+
+    def __init__(self):
+        self.unique_labels = None
+        self.label_to_index = {}
+
+    def fit(self, y):
+        """
+        Fit label encoder to a given set of labels.
+
+        Parameters:
+        -----------
+        y : array-like
+            Labels to encode.
+        """
+        self.unique_labels = np.unique(y)
+        self.label_to_index = {label: i for i, label in enumerate(self.unique_labels)}
+
+    def transform(self, y):
+        """
+        Transform labels to encoded integer labels.
+
+        Parameters:
+        -----------
+        y : array-like
+            Labels to encode.
+
+        Returns:
+        --------
+        encoded_labels : array-like
+            Encoded integer labels.
+        """
+        if self.unique_labels is None:
+            raise ValueError("Label encoder has not been fit yet.")
+        return np.array([self.label_to_index[label] for label in y])
+
+    def fit_transform(self, y):
+        """Fit label encoder and return encoded labels.
+
+        Parameters
+        ----------
+        y : array-like of shape (n_samples,)
+            Target values.
+
+        Returns
+        -------
+        y : array-like of shape (n_samples,)
+            Encoded labels.
+        """
+        self.fit(y)
+        return self.transform(y)
+
+    def inverse_transform(self, y):
+        """
+        Transform integer labels to original labels.
+
+        Parameters:
+        -----------
+        y : array-like
+            Encoded integer labels.
+
+        Returns:
+        --------
+        original_labels : array-like
+            Original labels.
+        """
+        if self.unique_labels is None:
+            raise ValueError("Label encoder has not been fit yet.")
+        return np.array([self.unique_labels[i] if i in self.label_to_index.values() else "unknown" for i in y])
```

### Comparing `enoppy-0.1.0/enoppy/utils/validator.py` & `enoppy-0.1.1/enoppy/utils/validator.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 21:39, 29/06/2022 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import operator
-import numpy as np
-
-
-def is_in_bound(value, bound):
-    ops = None
-    if type(bound) is tuple:
-        ops = operator.lt
-    elif type(bound) is list:
-        ops = operator.le
-    if bound[0] == float("-inf") and bound[1] == float("inf"):
-        return True
-    elif bound[0] == float("-inf") and ops(value, bound[1]):
-        return True
-    elif ops(bound[0], value) and bound[1] == float("inf"):
-        return True
-    elif ops(bound[0], value) and ops(value, bound[1]):
-        return True
-    return False
-
-
-def is_str_in_list(value: str, my_list: list):
-    if type(value) == str and my_list is not None:
-        return True if value in my_list else False
-    return False
-
-
-def check_int(name: str, value: int, bound=None):
-    if type(value) in [int, float]:
-        if bound is None:
-            return int(value)
-        elif is_in_bound(value, bound):
-            return int(value)
-    bound = "" if bound is None else f"and value should be in range: {bound}"
-    raise ValueError(f"'{name}' is an integer {bound}.")
-
-
-def check_float(name: str, value: int, bound=None):
-    if type(value) in [int, float]:
-        if bound is None:
-            return float(value)
-        elif is_in_bound(value, bound):
-            return float(value)
-    bound = "" if bound is None else f"and value should be in range: {bound}"
-    raise ValueError(f"'{name}' is a float {bound}.")
-
-
-def check_str(name: str, value: str, bound=None):
-    if type(value) is str:
-        if bound is None or is_str_in_list(value, bound):
-            return value
-    bound = "" if bound is None else f"and value should be one of this: {bound}"
-    raise ValueError(f"'{name}' is a string {bound}.")
-
-
-def check_bool(name: str, value: bool, bound=(True, False)):
-    if type(value) is bool:
-        if value in bound:
-            return value
-    bound = "" if bound is None else f"and value should be one of this: {bound}"
-    raise ValueError(f"'{name}' is a boolean {bound}.")
-
-
-def check_tuple_int(name: str, values: tuple, bounds=None):
-    if type(values) in [tuple, list] and len(values) > 1:
-        value_flag = [type(item) == int for item in values]
-        if np.all(value_flag):
-            if bounds is not None and len(bounds) == len(values):
-                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
-                if np.all(value_flag):
-                    return values
-            else:
-                return values
-    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
-    raise ValueError(f"'{name}' are integer {bounds}.")
-
-
-def check_tuple_float(name: str, values: tuple, bounds=None):
-    if type(values) in [tuple, list] and len(values) > 1:
-        value_flag = [type(item) in [int, float] for item in values]
-        if np.all(value_flag):
-            if bounds is not None and len(bounds) == len(values):
-                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
-                if np.all(value_flag):
-                    return values
-            else:
-                return values
-    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
-    raise ValueError(f"'{name}' are float {bounds}.")
+#!/usr/bin/env python
+# Created by "Thieu" at 21:39, 29/06/2022 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import operator
+import numpy as np
+
+
+def is_in_bound(value, bound):
+    ops = None
+    if type(bound) is tuple:
+        ops = operator.lt
+    elif type(bound) is list:
+        ops = operator.le
+    if bound[0] == float("-inf") and bound[1] == float("inf"):
+        return True
+    elif bound[0] == float("-inf") and ops(value, bound[1]):
+        return True
+    elif ops(bound[0], value) and bound[1] == float("inf"):
+        return True
+    elif ops(bound[0], value) and ops(value, bound[1]):
+        return True
+    return False
+
+
+def is_str_in_list(value: str, my_list: list):
+    if type(value) == str and my_list is not None:
+        return True if value in my_list else False
+    return False
+
+
+def check_int(name: str, value: int, bound=None):
+    if type(value) in [int, float]:
+        if bound is None:
+            return int(value)
+        elif is_in_bound(value, bound):
+            return int(value)
+    bound = "" if bound is None else f"and value should be in range: {bound}"
+    raise ValueError(f"'{name}' is an integer {bound}.")
+
+
+def check_float(name: str, value: int, bound=None):
+    if type(value) in [int, float]:
+        if bound is None:
+            return float(value)
+        elif is_in_bound(value, bound):
+            return float(value)
+    bound = "" if bound is None else f"and value should be in range: {bound}"
+    raise ValueError(f"'{name}' is a float {bound}.")
+
+
+def check_str(name: str, value: str, bound=None):
+    if type(value) is str:
+        if bound is None or is_str_in_list(value, bound):
+            return value
+    bound = "" if bound is None else f"and value should be one of this: {bound}"
+    raise ValueError(f"'{name}' is a string {bound}.")
+
+
+def check_bool(name: str, value: bool, bound=(True, False)):
+    if type(value) is bool:
+        if value in bound:
+            return value
+    bound = "" if bound is None else f"and value should be one of this: {bound}"
+    raise ValueError(f"'{name}' is a boolean {bound}.")
+
+
+def check_tuple_int(name: str, values: tuple, bounds=None):
+    if type(values) in [tuple, list] and len(values) > 1:
+        value_flag = [type(item) == int for item in values]
+        if np.all(value_flag):
+            if bounds is not None and len(bounds) == len(values):
+                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
+                if np.all(value_flag):
+                    return values
+            else:
+                return values
+    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
+    raise ValueError(f"'{name}' are integer {bounds}.")
+
+
+def check_tuple_float(name: str, values: tuple, bounds=None):
+    if type(values) in [tuple, list] and len(values) > 1:
+        value_flag = [type(item) in [int, float] for item in values]
+        if np.all(value_flag):
+            if bounds is not None and len(bounds) == len(values):
+                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
+                if np.all(value_flag):
+                    return values
+            else:
+                return values
+    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
+    raise ValueError(f"'{name}' are float {bounds}.")
```

### Comparing `enoppy-0.1.0/setup.py` & `enoppy-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 13:24, 27/02/2022 ----------%
-#       Email: nguyenthieu2102@gmail.com            %
-#       Github: https://github.com/thieu1995        %
-# --------------------------------------------------%
-
-from setuptools import setup, find_packages
-
-
-def readme():
-    with open('README.md', encoding='utf-8') as f:
-        README = f.read()
-    return README
-
-
-setup(
-    name="enoppy",
-    version="0.1.0",
-    author="Thieu",
-    author_email="nguyenthieu2102@gmail.com",
-    description="ENOPPY: A Python Library for Engineering Optimization Problems",
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    keywords=["optimization", "metaheuristics", "MHA", "mathematical optimization", "nature-inspired algorithms",
-              "evolutionary computation", "soft computing", "population-based algorithms",
-              "Stochastic optimization", "Global optimization", "Convergence analysis", "Search space exploration",
-              "Local search", "Computational intelligence", "Black-box optimization", "Robust optimization",
-              "Hybrid algorithms", "Benchmark functions", "Metaheuristic design", "Performance analysis",
-              "Exploration versus exploitation", "Self-adaptation", "Constrained optimization",
-              "Intelligent optimization", "Adaptive search", "Simulations", "Algorithm selection"],
-    url="https://github.com/thieu1995/enoppy",
-    project_urls={
-        'Documentation': 'https://enoppy.readthedocs.io/',
-        'Source Code': 'https://github.com/thieu1995/enoppy',
-        'Bug Tracker': 'https://github.com/thieu1995/enoppy/issues',
-        'Change Log': 'https://github.com/thieu1995/enoppy/blob/master/ChangeLog.md',
-        'Forum': 'https://t.me/+fRVCJGuGJg1mNDg1',
-    },
-    packages=find_packages(exclude=['tests*', 'examples*']),
-    include_package_data=True,
-    license="GPLv3",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "Intended Audience :: Information Technology",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: System :: Benchmark",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Mathematics",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-        "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Scientific/Engineering :: Visualization",
-        "Topic :: Scientific/Engineering :: Bio-Informatics",
-        "Topic :: Software Development :: Build Tools",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Utilities",
-    ],
-    install_requires=["numpy>=1.16.5", "matplotlib>=3.3.0", "scipy>=1.7.1", "mealpy>=2.5.3", "opfunu>=1.0.0"],
-    extras_require={
-        "dev": ["pytest>=7.0", "twine>=4.0.1"],
-    },
-    python_requires='>=3.7',
-)
+#!/usr/bin/env python
+# Created by "Thieu" at 13:24, 27/02/2022 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
+# --------------------------------------------------%
+
+from setuptools import setup, find_packages
+
+
+def readme():
+    with open('README.md', encoding='utf-8') as f:
+        README = f.read()
+    return README
+
+
+setup(
+    name="enoppy",
+    version="0.1.1",
+    author="Thieu",
+    author_email="nguyenthieu2102@gmail.com",
+    description="ENOPPY: A Python Library for Engineering Optimization Problems",
+    long_description=readme(),
+    long_description_content_type="text/markdown",
+    keywords=["engineering optimization problems", "mathematical optimization",
+              "Tension/compression spring design problem", "Welded beam design problem",
+              "Industrial chemical process problems", "Process design and synthesis problems",
+              "Mechanical design problems", "Power system problems",
+              "Power electronics: synchronous optimal pulse-width modulation", "Livestock feed ration optimization",
+              "Rolling element bearing design problem", "multi-objectives optimization problems",
+              "Constrained optimization", "Stochastic optimization", "Global optimization",
+              "Convergence analysis", "Search space exploration",
+              "Local search", "Computational intelligence", "Robust optimization",
+              "Benchmark functions", "Performance analysis", "Self-adaptation", "Intelligent optimization", "Simulations"],
+    url="https://github.com/thieu1995/enoppy",
+    project_urls={
+        'Documentation': 'https://enoppy.readthedocs.io/',
+        'Source Code': 'https://github.com/thieu1995/enoppy',
+        'Bug Tracker': 'https://github.com/thieu1995/enoppy/issues',
+        'Change Log': 'https://github.com/thieu1995/enoppy/blob/master/ChangeLog.md',
+        'Forum': 'https://t.me/+fRVCJGuGJg1mNDg1',
+    },
+    packages=find_packages(exclude=['tests*', 'examples*']),
+    include_package_data=True,
+    license="GPLv3",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: System :: Benchmark",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Mathematics",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Visualization",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
+        "Topic :: Software Development :: Build Tools",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Utilities",
+    ],
+    install_requires=["numpy>=1.17.1", "matplotlib>=3.3.0", "scipy>=1.7.1", "mealpy>=2.5.3", "opfunu>=1.0.0"],
+    extras_require={
+        "dev": ["pytest>=7.0", "twine>=4.0.1"],
+    },
+    python_requires='>=3.7',
+)
```

