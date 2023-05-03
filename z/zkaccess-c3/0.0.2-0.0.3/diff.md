# Comparing `tmp/zkaccess_c3-0.0.2.tar.gz` & `tmp/zkaccess_c3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkaccess_c3-0.0.2.tar", last modified: Sat Mar 25 22:12:57 2023, max compression
+gzip compressed data, was "zkaccess_c3-0.0.3.tar", last modified: Wed May  3 20:57:42 2023, max compression
```

## Comparing `zkaccess_c3-0.0.2.tar` & `zkaccess_c3-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:57.004872 zkaccess_c3-0.0.2/
--rwxr-xr-x   0 root         (0) root         (0)      209 2023-03-05 21:47:11.000000 zkaccess_c3-0.0.2/.dockerignore
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:56.333998 zkaccess_c3-0.0.2/.github/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:56.559262 zkaccess_c3-0.0.2/.github/workflows/
--rwxr-xr-x   0 root         (0) root         (0)      987 2023-03-24 22:36:02.000000 zkaccess_c3-0.0.2/.github/workflows/build_test.yml
--rwxr-xr-x   0 root         (0) root         (0)      698 2023-03-24 22:28:33.000000 zkaccess_c3-0.0.2/.github/workflows/publish.yml
--rwxr-xr-x   0 root         (0) root         (0)      757 2023-03-23 21:42:56.000000 zkaccess_c3-0.0.2/.gitignore
--rwxr-xr-x   0 root         (0) root         (0)      378 2023-03-24 22:01:26.000000 zkaccess_c3-0.0.2/Dockerfile
--rwxr-xr-x   0 root         (0) root         (0)    35823 2020-11-29 15:51:04.000000 zkaccess_c3-0.0.2/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)     6454 2023-03-25 22:12:56.999846 zkaccess_c3-0.0.2/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:56.709516 zkaccess_c3-0.0.2/c3/
--rwxr-xr-x   0 root         (0) root         (0)      168 2023-03-19 16:15:40.000000 zkaccess_c3-0.0.2/c3/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10658 2023-03-22 22:08:25.000000 zkaccess_c3-0.0.2/c3/consts.py
--rwxr-xr-x   0 root         (0) root         (0)     4312 2023-03-19 21:07:01.000000 zkaccess_c3-0.0.2/c3/controldevice.py
--rwxr-xr-x   0 root         (0) root         (0)    11118 2023-03-23 22:41:43.000000 zkaccess_c3-0.0.2/c3/core.py
--rwxr-xr-x   0 root         (0) root         (0)     1553 2023-03-19 16:01:25.000000 zkaccess_c3-0.0.2/c3/crc.py
--rwxr-xr-x   0 root         (0) root         (0)     7635 2023-03-22 22:02:20.000000 zkaccess_c3-0.0.2/c3/rtlog.py
--rwxr-xr-x   0 root         (0) root         (0)     1464 2023-03-13 21:38:32.000000 zkaccess_c3-0.0.2/c3/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:56.818362 zkaccess_c3-0.0.2/cli/
--rwxr-xr-x   0 root         (0) root         (0)      623 2023-03-19 16:03:02.000000 zkaccess_c3-0.0.2/cli/C3_CancelAlarms.py
--rwxr-xr-x   0 root         (0) root         (0)      597 2023-03-20 21:46:48.000000 zkaccess_c3-0.0.2/cli/C3_Discover.py
--rwxr-xr-x   0 root         (0) root         (0)     1182 2023-03-19 16:04:11.000000 zkaccess_c3-0.0.2/cli/C3_GetDeviceParam.py
--rwxr-xr-x   0 root         (0) root         (0)     1031 2023-03-23 21:35:58.000000 zkaccess_c3-0.0.2/cli/C3_GetRTLog.py
--rwxr-xr-x   0 root         (0) root         (0)     1589 2023-03-19 21:05:00.000000 zkaccess_c3-0.0.2/cli/C3_OutputOperation.py
--rwxr-xr-x   0 root         (0) root         (0)      919 2023-03-25 22:12:25.000000 zkaccess_c3-0.0.2/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)     6046 2023-03-24 21:28:47.000000 zkaccess_c3-0.0.2/readme.md
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 16:38:19.000000 zkaccess_c3-0.0.2/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-03-25 22:12:57.007244 zkaccess_c3-0.0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       41 2023-03-19 16:35:31.000000 zkaccess_c3-0.0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:56.913054 zkaccess_c3-0.0.2/tests/
--rwxr-xr-x   0 root         (0) root         (0)      456 2023-03-19 16:06:28.000000 zkaccess_c3-0.0.2/tests/test_consts.py
--rwxr-xr-x   0 root         (0) root         (0)     1522 2023-03-17 22:23:55.000000 zkaccess_c3-0.0.2/tests/test_controldevice.py
--rwxr-xr-x   0 root         (0) root         (0)     1673 2023-03-19 16:05:04.000000 zkaccess_c3-0.0.2/tests/test_crc16.py
--rwxr-xr-x   0 root         (0) root         (0)     2361 2023-03-23 21:44:29.000000 zkaccess_c3-0.0.2/tests/test_rtlog.py
--rwxr-xr-x   0 root         (0) root         (0)      872 2023-03-18 22:31:12.000000 zkaccess_c3-0.0.2/tests/test_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-25 22:12:56.983739 zkaccess_c3-0.0.2/zkaccess_c3.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     6454 2023-03-25 22:12:56.000000 zkaccess_c3-0.0.2/zkaccess_c3.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      611 2023-03-25 22:12:56.000000 zkaccess_c3-0.0.2/zkaccess_c3.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-03-25 22:12:56.000000 zkaccess_c3-0.0.2/zkaccess_c3.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)        3 2023-03-25 22:12:56.000000 zkaccess_c3-0.0.2/zkaccess_c3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.314217 zkaccess_c3-0.0.3/c3/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.314217 zkaccess_c3-0.0.3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_CancelAlarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_Discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_GetDeviceParam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_GetRTLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_OutputOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_crc16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/top_level.txt
```

### Comparing `zkaccess_c3-0.0.2/LICENSE` & `zkaccess_c3-0.0.3/LICENSE`

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

### Comparing `zkaccess_c3-0.0.2/PKG-INFO` & `zkaccess_c3-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess_c3
-Version: 0.0.2
+Version: 0.0.3
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `zkaccess_c3-0.0.2/c3/controldevice.py` & `zkaccess_c3-0.0.3/c3/controldevice.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from abc import ABC
-from c3 import consts
-
-
-# A ControlDevice is a binary message of 5 bytes send to the C3 access panel.
-# It changes the states of the doors, auxiliary relays and alarms.
-# All multibyte values are stored as Little-endian.
-#
-# Byte       0  1  2  3  4
-#            01:01:01:c8:00
-# Operation: |
-#            01 => 1 (1: output, 2: cancel alarm, 3: restart device, 4: enable/disable normal open state)
-# Param 1:      |
-# Param 2:         |
-# Param 3:            |
-# Param 4:               |
-#
-# The meaning of the parameters is depending on the Operation code.
-# Param 4 is reserved for future use (defaults to 0)
-# Operation 1: Output operation
-#   Param 1: Door number or auxiliary output number
-#   Param 2: The address type of output operation (1: Door output, 2: Auxiliary output)
-#   Param 3: Duration of the open operation, only for address type = 1 (door output).
-#            0: close, 255: normal open state, 1~254: normal open duration
-# Operation 2: Cancel alarm
-#   Param 1: 0 (null)
-#   Param 2: 0 (null)
-#   Param 3: 0 (null)
-# Operation 3: Restart device
-#   Param 1: 0 (null)
-#   Param 2: 0 (null)
-#   Param 3: 0 (null)
-# Operation 3: Enable/disable normal open state
-#   Param 1: Door number
-#   Param 2: Enable / disable (0: disable, 1: enable'
-#   Param 3: 0 (null)
-class ControlDeviceBase(ABC):
-    def __init__(self, operation: consts.ControlOperation, param1: int = None, param2: int = None, param3: int = None,
-                 param4: int = None):
-        self.operation: consts.ControlOperation = operation
-        self.param1: int = param1
-        self.param2: int = param2
-        self.param3: int = param3
-        self.param4: int = param4
-
-    @classmethod
-    def from_bytes(cls, data: bytes):
-        return ControlDeviceBase(*data)
-
-    def to_bytes(self) -> bytes:
-        return bytes([self.operation, self.param1 or 0, self.param2 or 0, self.param3 or 0, self.param4 or 0])
-
-    def __repr__(self):
-        return "\r\n".join([
-            "%-12s %-10s (%s)" % ("operation", self.operation, repr(self.operation)),
-            "%-12s %-10s" % ("param1", self.param1),
-            "%-12s %-10s" % ("param2", self.param2),
-            "%-12s %-10s" % ("param3", self.param3),
-            "%-12s %-10s" % ("param4", self.param4),
-        ])
-
-
-class ControlDeviceOutput(ControlDeviceBase):
-    def __init__(self, output_number: int, address: consts.ControlOutputAddress, duration: int):
-        ControlDeviceBase.__init__(self, consts.ControlOperation.OUTPUT, output_number, address, duration)
-
-    def __repr__(self):
-        return "\r\n".join([
-            "ControlDevice Output Operation:"
-            "%-12s %-10s (%s)" % ("operation", self.operation, repr(self.operation)),
-            "%-12s %-10s (Door/Aux Number)" % ("param1", self.param1),
-            "%-12s %-10s %s" % ("param2", self.param2, repr(consts.ControlOutputAddress(self.param2))),
-            "%-12s %-10s (Duration)" % ("param3", self.param3),
-        ])
-
-
-class ControlDeviceCancelAlarms(ControlDeviceBase):
-    def __init__(self):
-        ControlDeviceBase.__init__(self, consts.ControlOperation.CANCEL_ALARM)
-
-    def __repr__(self):
-        return "\r\n".join([
-            "ControlDevice Cancel Alarm Operation:",
-            ControlDeviceBase.__repr__(self)
-        ])
-
-
-class ControlDeviceNormalOpenStateEnable(ControlDeviceBase):
-    def __init__(self, door_number: int, enable: bool):
-        ControlDeviceBase.__init__(self, consts.ControlOperation.ENDIS_NO_STATE, door_number, enable)
-
-    def __repr__(self):
-        return "\r\n".join([
-            "ControlDevice Normal Open State Operation:"
-            "%-12s %-10s (%s)" % ("operation", self.operation, repr(self.operation)),
-            "%-12s %-10s (Door Number)" % ("param1", self.param1),
-            "%-12s %-10s %s" % ("param2", self.param2, "Enable" if self.param2 else "Disable"),
-        ])
-
-
-class ControlDeviceRestart(ControlDeviceBase):
-    def __init__(self):
-        ControlDeviceBase.__init__(self, consts.ControlOperation.RESTART_DEVICE)
-
-    def __repr__(self):
-        return "\r\n".join([
-            "ControlDevice Restart Operation:",
-            ControlDeviceBase.__repr__(self)
-        ])
+from abc import ABC
+from c3 import consts
+
+
+# A ControlDevice is a binary message of 5 bytes send to the C3 access panel.
+# It changes the states of the doors, auxiliary relays and alarms.
+# All multibyte values are stored as Little-endian.
+#
+# Byte       0  1  2  3  4
+#            01:01:01:c8:00
+# Operation: |
+#            01 => 1 (1: output, 2: cancel alarm, 3: restart device, 4: enable/disable normal open state)
+# Param 1:      |
+# Param 2:         |
+# Param 3:            |
+# Param 4:               |
+#
+# The meaning of the parameters is depending on the Operation code.
+# Param 4 is reserved for future use (defaults to 0)
+# Operation 1: Output operation
+#   Param 1: Door number or auxiliary output number
+#   Param 2: The address type of output operation (1: Door output, 2: Auxiliary output)
+#   Param 3: Duration of the open operation, only for address type = 1 (door output).
+#            0: close, 255: normal open state, 1~254: normal open duration
+# Operation 2: Cancel alarm
+#   Param 1: 0 (null)
+#   Param 2: 0 (null)
+#   Param 3: 0 (null)
+# Operation 3: Restart device
+#   Param 1: 0 (null)
+#   Param 2: 0 (null)
+#   Param 3: 0 (null)
+# Operation 3: Enable/disable normal open state
+#   Param 1: Door number
+#   Param 2: Enable / disable (0: disable, 1: enable'
+#   Param 3: 0 (null)
+class ControlDeviceBase(ABC):
+    def __init__(self, operation: consts.ControlOperation, param1: int = None, param2: int = None, param3: int = None,
+                 param4: int = None):
+        self.operation: consts.ControlOperation = operation
+        self.param1: int = param1
+        self.param2: int = param2
+        self.param3: int = param3
+        self.param4: int = param4
+
+    @classmethod
+    def from_bytes(cls, data: bytes):
+        return ControlDeviceBase(*data)
+
+    def to_bytes(self) -> bytes:
+        return bytes([self.operation, self.param1 or 0, self.param2 or 0, self.param3 or 0, self.param4 or 0])
+
+    def __repr__(self):
+        return "\r\n".join([
+            "%-12s %-10s (%s)" % ("operation", self.operation, repr(self.operation)),
+            "%-12s %-10s" % ("param1", self.param1),
+            "%-12s %-10s" % ("param2", self.param2),
+            "%-12s %-10s" % ("param3", self.param3),
+            "%-12s %-10s" % ("param4", self.param4),
+        ])
+
+
+class ControlDeviceOutput(ControlDeviceBase):
+    def __init__(self, output_number: int, address: consts.ControlOutputAddress, duration: int):
+        ControlDeviceBase.__init__(self, consts.ControlOperation.OUTPUT, output_number, address, duration)
+
+    def __repr__(self):
+        return "\r\n".join([
+            "ControlDevice Output Operation:"
+            "%-12s %-10s (%s)" % ("operation", self.operation, repr(self.operation)),
+            "%-12s %-10s (Door/Aux Number)" % ("param1", self.param1),
+            "%-12s %-10s %s" % ("param2", self.param2, repr(consts.ControlOutputAddress(self.param2))),
+            "%-12s %-10s (Duration)" % ("param3", self.param3),
+        ])
+
+
+class ControlDeviceCancelAlarms(ControlDeviceBase):
+    def __init__(self):
+        ControlDeviceBase.__init__(self, consts.ControlOperation.CANCEL_ALARM)
+
+    def __repr__(self):
+        return "\r\n".join([
+            "ControlDevice Cancel Alarm Operation:",
+            ControlDeviceBase.__repr__(self)
+        ])
+
+
+class ControlDeviceNormalOpenStateEnable(ControlDeviceBase):
+    def __init__(self, door_number: int, enable: bool):
+        ControlDeviceBase.__init__(self, consts.ControlOperation.ENDIS_NO_STATE, door_number, enable)
+
+    def __repr__(self):
+        return "\r\n".join([
+            "ControlDevice Normal Open State Operation:"
+            "%-12s %-10s (%s)" % ("operation", self.operation, repr(self.operation)),
+            "%-12s %-10s (Door Number)" % ("param1", self.param1),
+            "%-12s %-10s %s" % ("param2", self.param2, "Enable" if self.param2 else "Disable"),
+        ])
+
+
+class ControlDeviceRestart(ControlDeviceBase):
+    def __init__(self):
+        ControlDeviceBase.__init__(self, consts.ControlOperation.RESTART_DEVICE)
+
+    def __repr__(self):
+        return "\r\n".join([
+            "ControlDevice Restart Operation:",
+            ControlDeviceBase.__repr__(self)
+        ])
```

### Comparing `zkaccess_c3-0.0.2/c3/crc.py` & `zkaccess_c3-0.0.3/c3/crc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# Ported CRC-16 from libcrc.org
-# (https://github.com/lammertb/libcrc/blob/master/src/crc16.c)
-
-CRC_POLY_16 = 0xA001
-CRC_START_16 = 0x0000
-
-
-class Crc16Builder:
-    def __init__(self, crc: int = None):
-        self._crc = crc or CRC_START_16
-
-    @classmethod
-    def _calc_divisor(cls, byte):
-        poly = 0
-
-        for _ in range(8):
-            if ((poly ^ byte) & 0x0001) == 1:
-                poly = (poly >> 1) ^ CRC_POLY_16
-            else:
-                poly = poly >> 1
-
-            byte = byte >> 1
-
-        return poly
-
-    def add_byte(self, data: int):
-        data = data & 0xFF        # Limit data size to byte
-        crc = self._crc & 0xFFFF  # Truncate to 16bit
-        msb = crc >> 8            # Take msb from 16bit crc
-        self._crc = msb ^ self._calc_divisor(crc ^ data)
-
-    @property
-    def crc(self):
-        return self._crc & 0xFFFF
-
-
-def crc16(data, crc=None):
-    builder = Crc16Builder(crc)
-
-    if hasattr(data, '__iter__'):
-        for byte in data:
-            if isinstance(byte, int):
-                builder.add_byte(byte)
-            elif isinstance(byte, str):
-                if len(byte) == 1:
-                    builder.add_byte(ord(byte))
-                else:
-                    for char in byte:
-                        builder.add_byte(ord(char))
-            else:
-                raise TypeError("Data of type %s is not supported" % type(byte))
-    else:
-        raise TypeError("Data '%s' is not iterable" % data)
-
-    return builder.crc
+# Ported CRC-16 from libcrc.org
+# (https://github.com/lammertb/libcrc/blob/master/src/crc16.c)
+
+CRC_POLY_16 = 0xA001
+CRC_START_16 = 0x0000
+
+
+class Crc16Builder:
+    def __init__(self, crc: int = None):
+        self._crc = crc or CRC_START_16
+
+    @classmethod
+    def _calc_divisor(cls, byte):
+        poly = 0
+
+        for _ in range(8):
+            if ((poly ^ byte) & 0x0001) == 1:
+                poly = (poly >> 1) ^ CRC_POLY_16
+            else:
+                poly = poly >> 1
+
+            byte = byte >> 1
+
+        return poly
+
+    def add_byte(self, data: int):
+        data = data & 0xFF        # Limit data size to byte
+        crc = self._crc & 0xFFFF  # Truncate to 16bit
+        msb = crc >> 8            # Take msb from 16bit crc
+        self._crc = msb ^ self._calc_divisor(crc ^ data)
+
+    @property
+    def crc(self):
+        return self._crc & 0xFFFF
+
+
+def crc16(data, crc=None):
+    builder = Crc16Builder(crc)
+
+    if hasattr(data, '__iter__'):
+        for byte in data:
+            if isinstance(byte, int):
+                builder.add_byte(byte)
+            elif isinstance(byte, str):
+                if len(byte) == 1:
+                    builder.add_byte(ord(byte))
+                else:
+                    for char in byte:
+                        builder.add_byte(ord(char))
+            else:
+                raise TypeError("Data of type %s is not supported" % type(byte))
+    else:
+        raise TypeError("Data '%s' is not iterable" % data)
+
+    return builder.crc
```

### Comparing `zkaccess_c3-0.0.2/c3/rtlog.py` & `zkaccess_c3-0.0.3/c3/rtlog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,170 +1,171 @@
-from abc import ABC, abstractmethod
-from c3 import consts
-from c3.utils import C3DateTime
-
-
-class RTLogRecord(ABC):
-    @abstractmethod
-    def is_door_alarm(self) -> bool:
-        ...
-
-    @abstractmethod
-    def is_event(self) -> bool:
-        ...
-
-
-# An RTLog is a binary message of 16 bytes send by the C3 access panel.
-# If the value of byte 10 (the event type) is 255, the RTLog is a Door/Alarm Realtime Status.
-# If the value of byte 10 (the event type) is not 255, the RTLog is a Realtime Event.
-
-# Door/Alarm Realtime Status record
-# All multibyte values are stored as Little-endian.
-#
-# Byte:                    0  1  2  3  4  5  6  7  8  9  A  B  C  D  E  F
-#                          01:4f:86:00:99:92:98:00:04:01:00:00:a5:ad:ad:21
-# Alarm status (byte 4-7):             |
-#                                      99:92:98:00 => (big endian:) 00989299 = 9999001
-# DSS status (byte 0-3):   |
-#                          01:4f:86:00 => (big endian:) 00864f01 = 8802049
-# Verified (byte 8):                               |
-#                                                  04
-# Unused (byte 9):                                    |
-#                                                     01
-# EventType (byte 10):                                   |
-#                                                        00
-# Unused (byte 11):                                         |
-#                                                           00
-#                                                              |
-# Time_second (byte 12-15)                                     a5:ad:ad:21 => (big endian:) 21ADADA5 =
-#                                                                                           2017-7-30 16:51:49
-class DoorAlarmStatusRecord(RTLogRecord):
-    def __init__(self):
-        self.alarm_status = bytes(4)
-        self.dss_status = bytes(4)
-        self.verified: consts.VerificationMode = consts.VerificationMode.NONE
-        self.event_type: consts.EventType = consts.EventType.NA
-        self.time_second = 0
-
-    @classmethod
-    def from_bytes(cls, data: bytes):
-        record = DoorAlarmStatusRecord()
-        record.alarm_status = bytes(data[0:4])
-        record.dss_status = bytes(data[4:8])
-        record.verified = consts.VerificationMode(data[9])
-        record.event_type = consts.EventType(data[10])
-        record.time_second = C3DateTime.from_value(int.from_bytes(data[12:16], byteorder="little"))
-        return record
-
-    def is_door_alarm(self) -> bool:
-        return True
-
-    def is_event(self) -> bool:
-        return False
-
-    def get_alarms(self, door_nr: int) -> list[consts.AlarmStatus]:
-        alarms = []
-
-        for i in range(0, 3):
-            if i+1 == door_nr or not door_nr:
-                if self.alarm_status[i] & consts.AlarmStatus.ALARM:
-                    if alarms.count(consts.AlarmStatus.ALARM) == 0:
-                        alarms.append(consts.AlarmStatus.ALARM)
-                elif self.alarm_status[i] & consts.AlarmStatus.DOOR_OPEN_TIMEOUT:
-                    if alarms.count(consts.AlarmStatus.DOOR_OPEN_TIMEOUT) == 0:
-                        alarms.append(consts.AlarmStatus.DOOR_OPEN_TIMEOUT)
-
-        return alarms
-
-    def has_alarm(self, door_nr: int, status: consts.AlarmStatus = None):
-        return ((self.alarm_status[door_nr-1] & (status or 0)) == status) or \
-               ((self.alarm_status[door_nr-1] > 0) and status is None)
-
-    def door_is_open(self, door_nr: int):
-        is_open = None
-
-        if (self.dss_status[door_nr-1] & 0x0F) == consts.DoorSensorStatus.OPEN:
-            is_open = True
-        elif (self.dss_status[door_nr-1] & 0x0F) == consts.DoorSensorStatus.CLOSED:
-            is_open = False
-
-        return is_open
-
-    def __repr__(self):
-        repr_arr = ["Door/Alarm Realtime Status:",
-                    "%-12s %-10s" % ("time_second", self.time_second),
-                    "%-12s %-10s %s" % ("event_type", self.event_type, repr(self.event_type)),
-                    "%-12s %-10s %s" % ("verified", self.verified, repr(self.verified)),
-                    "%-12s %-10s" % ("alarm_status", self.alarm_status.hex(" "))]
-
-        for i in range(0, 4):
-            for status in consts.AlarmStatus:
-                if status != consts.AlarmStatus.NONE:
-                    if self.alarm_status[i] & status == status:
-                        repr_arr.append("    Door %-2s %-4s %s" % (i, status, repr(status)))
-
-        repr_arr.append("%-12s %-10s" % ("dss_status", self.dss_status.hex(" ")))
-        for i in range(0, 4):
-            repr_arr.append("    Door %-2s %-4s %s" % (i+1, self.dss_status[i],
-                                                       repr(consts.DoorSensorStatus(self.dss_status[i] & 0x0F))))
-
-        return "\r\n".join(repr_arr)
-
-
-# Realtime Event record
-# All multibyte values are stored as Little-endian.
-#
-# Byte:              0  1  2  3  4  5  6  7  8  9  A  B  C  D  E  F
-#                    01:4f:86:00:99:92:98:00:04:01:00:00:a5:ad:ad:21
-# Cardno (byte 4-7):             |
-#                                99:92:98:00 => (big endian:) 00989299 = 9999001
-# Pin (byte 0-3):    |
-#                    01:4f:86:00 => (big endian:) 00864f01 = 8802049
-# Verified (byte 8):                         |
-#                                            04
-# DoorID (byte 9):                              |
-#                                               01
-# EventType (byte 10):                             |
-#                                                  00
-# InOutState (byte 11):                               |
-#                                                     00
-#                                                        |
-# Time_second (byte 12-15)                               a5:ad:ad:21 => (big endian:) 21ADADA5 = 2017-7-30 16:51:49
-class EventRecord(RTLogRecord):
-    def __init__(self):
-        self.card_no = 0
-        self.pin = 0
-        self.verified: consts.VerificationMode = consts.VerificationMode.NONE
-        self.door_id = 0
-        self.event_type: consts.EventType = consts.EventType.NA
-        self.in_out_state: consts.InOutStatus = consts.InOutStatus.NONE
-        self.time_second = 0
-
-    @classmethod
-    def from_bytes(cls, data: bytes):
-        record = EventRecord()
-        record.card_no = int.from_bytes(data[0:4], byteorder="little")
-        record.pin = int.from_bytes(data[4:8], byteorder="little")
-        record.verified = consts.VerificationMode(data[8])
-        record.door_id = data[9]
-        record.event_type = consts.EventType(data[10])
-        record.in_out_state = consts.InOutStatus(data[11])
-        record.time_second = C3DateTime.from_value(int.from_bytes(data[12:16], byteorder="little"))
-        return record
-
-    def is_door_alarm(self) -> bool:
-        return False
-
-    def is_event(self) -> bool:
-        return True
-
-    def __repr__(self):
-        repr_arr = ["Realtime Event:",
-                    "%-12s %-10s" % ("time_second", self.time_second),
-                    "%-12s %-10s %s" % ("event_type", self.event_type, repr(self.event_type)),
-                    "%-12s %-10s %s" % ("in_out_state", self.in_out_state, repr(self.in_out_state)),
-                    "%-12s %-10s %s" % ("verified", self.verified, repr(self.verified)),
-                    "%-12s %-10s" % ("card_no", self.card_no),
-                    # "%-12s %-10s" % ("pin", self.pin),
-                    "%-12s %-10s" % ("door_id", self.door_id)]
-
-        return "\r\n".join(repr_arr)
+from __future__ import annotations
+from abc import ABC, abstractmethod
+from c3 import consts
+from c3.utils import C3DateTime
+
+
+class RTLogRecord(ABC):
+    @abstractmethod
+    def is_door_alarm(self) -> bool:
+        ...
+
+    @abstractmethod
+    def is_event(self) -> bool:
+        ...
+
+
+# An RTLog is a binary message of 16 bytes send by the C3 access panel.
+# If the value of byte 10 (the event type) is 255, the RTLog is a Door/Alarm Realtime Status.
+# If the value of byte 10 (the event type) is not 255, the RTLog is a Realtime Event.
+
+# Door/Alarm Realtime Status record
+# All multibyte values are stored as Little-endian.
+#
+# Byte:                    0  1  2  3  4  5  6  7  8  9  A  B  C  D  E  F
+#                          01:4f:86:00:99:92:98:00:04:01:00:00:a5:ad:ad:21
+# Alarm status (byte 4-7):             |
+#                                      99:92:98:00 => (big endian:) 00989299 = 9999001
+# DSS status (byte 0-3):   |
+#                          01:4f:86:00 => (big endian:) 00864f01 = 8802049
+# Verified (byte 8):                               |
+#                                                  04
+# Unused (byte 9):                                    |
+#                                                     01
+# EventType (byte 10):                                   |
+#                                                        00
+# Unused (byte 11):                                         |
+#                                                           00
+#                                                              |
+# Time_second (byte 12-15)                                     a5:ad:ad:21 => (big endian:) 21ADADA5 =
+#                                                                                           2017-7-30 16:51:49
+class DoorAlarmStatusRecord(RTLogRecord):
+    def __init__(self):
+        self.alarm_status = bytes(4)
+        self.dss_status = bytes(4)
+        self.verified: consts.VerificationMode = consts.VerificationMode.NONE
+        self.event_type: consts.EventType = consts.EventType.NA
+        self.time_second = 0
+
+    @classmethod
+    def from_bytes(cls, data: bytes):
+        record = DoorAlarmStatusRecord()
+        record.alarm_status = bytes(data[0:4])
+        record.dss_status = bytes(data[4:8])
+        record.verified = consts.VerificationMode(data[9])
+        record.event_type = consts.EventType(data[10])
+        record.time_second = C3DateTime.from_value(int.from_bytes(data[12:16], byteorder="little"))
+        return record
+
+    def is_door_alarm(self) -> bool:
+        return True
+
+    def is_event(self) -> bool:
+        return False
+
+    def get_alarms(self, door_nr: int) -> list[consts.AlarmStatus]:
+        alarms = []
+
+        for i in range(0, 3):
+            if i+1 == door_nr or not door_nr:
+                if self.alarm_status[i] & consts.AlarmStatus.ALARM:
+                    if alarms.count(consts.AlarmStatus.ALARM) == 0:
+                        alarms.append(consts.AlarmStatus.ALARM)
+                elif self.alarm_status[i] & consts.AlarmStatus.DOOR_OPEN_TIMEOUT:
+                    if alarms.count(consts.AlarmStatus.DOOR_OPEN_TIMEOUT) == 0:
+                        alarms.append(consts.AlarmStatus.DOOR_OPEN_TIMEOUT)
+
+        return alarms
+
+    def has_alarm(self, door_nr: int, status: consts.AlarmStatus = None):
+        return ((self.alarm_status[door_nr-1] & (status or 0)) == status) or \
+               ((self.alarm_status[door_nr-1] > 0) and status is None)
+
+    def door_is_open(self, door_nr: int):
+        is_open = None
+
+        if (self.dss_status[door_nr-1] & 0x0F) == consts.DoorSensorStatus.OPEN:
+            is_open = True
+        elif (self.dss_status[door_nr-1] & 0x0F) == consts.DoorSensorStatus.CLOSED:
+            is_open = False
+
+        return is_open
+
+    def __repr__(self):
+        repr_arr = ["Door/Alarm Realtime Status:",
+                    "%-12s %-10s" % ("time_second", self.time_second),
+                    "%-12s %-10s %s" % ("event_type", self.event_type, repr(self.event_type)),
+                    "%-12s %-10s %s" % ("verified", self.verified, repr(self.verified)),
+                    "%-12s %-10s" % ("alarm_status", self.alarm_status.hex())]
+
+        for i in range(0, 4):
+            for status in consts.AlarmStatus:
+                if status != consts.AlarmStatus.NONE:
+                    if self.alarm_status[i] & status == status:
+                        repr_arr.append("    Door %-2s %-4s %s" % (i, status, repr(status)))
+
+        repr_arr.append("%-12s %-10s" % ("dss_status", self.dss_status.hex()))
+        for i in range(0, 4):
+            repr_arr.append("    Door %-2s %-4s %s" % (i+1, self.dss_status[i],
+                                                       repr(consts.DoorSensorStatus(self.dss_status[i] & 0x0F))))
+
+        return "\r\n".join(repr_arr)
+
+
+# Realtime Event record
+# All multibyte values are stored as Little-endian.
+#
+# Byte:              0  1  2  3  4  5  6  7  8  9  A  B  C  D  E  F
+#                    01:4f:86:00:99:92:98:00:04:01:00:00:a5:ad:ad:21
+# Cardno (byte 4-7):             |
+#                                99:92:98:00 => (big endian:) 00989299 = 9999001
+# Pin (byte 0-3):    |
+#                    01:4f:86:00 => (big endian:) 00864f01 = 8802049
+# Verified (byte 8):                         |
+#                                            04
+# DoorID (byte 9):                              |
+#                                               01
+# EventType (byte 10):                             |
+#                                                  00
+# InOutState (byte 11):                               |
+#                                                     00
+#                                                        |
+# Time_second (byte 12-15)                               a5:ad:ad:21 => (big endian:) 21ADADA5 = 2017-7-30 16:51:49
+class EventRecord(RTLogRecord):
+    def __init__(self):
+        self.card_no = 0
+        self.pin = 0
+        self.verified: consts.VerificationMode = consts.VerificationMode.NONE
+        self.door_id = 0
+        self.event_type: consts.EventType = consts.EventType.NA
+        self.in_out_state: consts.InOutStatus = consts.InOutStatus.NONE
+        self.time_second = 0
+
+    @classmethod
+    def from_bytes(cls, data: bytes):
+        record = EventRecord()
+        record.card_no = int.from_bytes(data[0:4], byteorder="little")
+        record.pin = int.from_bytes(data[4:8], byteorder="little")
+        record.verified = consts.VerificationMode(data[8])
+        record.door_id = data[9]
+        record.event_type = consts.EventType(data[10])
+        record.in_out_state = consts.InOutStatus(data[11])
+        record.time_second = C3DateTime.from_value(int.from_bytes(data[12:16], byteorder="little"))
+        return record
+
+    def is_door_alarm(self) -> bool:
+        return False
+
+    def is_event(self) -> bool:
+        return True
+
+    def __repr__(self):
+        repr_arr = ["Realtime Event:",
+                    "%-12s %-10s" % ("time_second", self.time_second),
+                    "%-12s %-10s %s" % ("event_type", self.event_type, repr(self.event_type)),
+                    "%-12s %-10s %s" % ("in_out_state", self.in_out_state, repr(self.in_out_state)),
+                    "%-12s %-10s %s" % ("verified", self.verified, repr(self.verified)),
+                    "%-12s %-10s" % ("card_no", self.card_no),
+                    # "%-12s %-10s" % ("pin", self.pin),
+                    "%-12s %-10s" % ("door_id", self.door_id)]
+
+        return "\r\n".join(repr_arr)
```

### Comparing `zkaccess_c3-0.0.2/cli/C3_CancelAlarms.py` & `zkaccess_c3-0.0.3/cli/C3_CancelAlarms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-#!/usr/bin/env python3
-import argparse
-import logging
-import sys
-from c3 import C3
-from c3 import controldevice
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('host', help='C3 panel IP address or host name')
-    args = parser.parse_args()
-
-    print("Connecting to %s" % args.host)
-    panel = C3()
-    panel.log.addHandler(logging.StreamHandler(sys.stdout))
-    panel.log.setLevel(logging.DEBUG)
-
-    if panel.connect(args.host):
-        panel.control_device(controldevice.ControlDeviceCancelAlarms())
-
-    panel.disconnect()
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python3
+import argparse
+import logging
+import sys
+from c3 import C3
+from c3 import controldevice
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('host', help='C3 panel IP address or host name')
+    args = parser.parse_args()
+
+    print("Connecting to %s" % args.host)
+    panel = C3(args.host)
+    panel.log.addHandler(logging.StreamHandler(sys.stdout))
+    panel.log.setLevel(logging.DEBUG)
+
+    try:
+        if panel.connect():
+            panel.control_device(controldevice.ControlDeviceCancelAlarms())
+    except Exception as e:
+        print(f"Cancel alarms faied: {e}")
+    finally:
+        panel.disconnect()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zkaccess_c3-0.0.2/cli/C3_GetRTLog.py` & `zkaccess_c3-0.0.3/cli/C3_GetRTLog.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!/usr/bin/env python3
-import argparse
-import logging
-import sys
-import time
-from c3 import C3
-from c3 import rtlog
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('host', help='C3 panel IP address or host name')
-    args = parser.parse_args()
-
-    print("Connecting to %s" % args.host)
-    panel = C3()
-    panel.log.addHandler(logging.StreamHandler(sys.stdout))
-    panel.log.setLevel(logging.DEBUG)
-
-    if panel.connect(args.host):
-        try:
-            while True:
-                last_record_is_status = False
-
-                records = panel.get_rt_log()
-                for record in records:
-                    print(repr(record))
-                    if isinstance(record, rtlog.DoorAlarmStatusRecord):
-                        last_record_is_status = True
-
-                if last_record_is_status:
-                    time.sleep(10)
-        except KeyboardInterrupt:
-            pass
-
-    panel.disconnect()
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python3
+import argparse
+import logging
+import sys
+import time
+from c3 import C3
+from c3 import rtlog
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('host', help='C3 panel IP address or host name')
+    args = parser.parse_args()
+
+    print("Connecting to %s" % args.host)
+    panel = C3(args.host)
+    panel.log.addHandler(logging.StreamHandler(sys.stdout))
+    panel.log.setLevel(logging.DEBUG)
+
+    if panel.connect():
+        try:
+            while True:
+                last_record_is_status = False
+
+                records = panel.get_rt_log()
+                for record in records:
+                    print(repr(record))
+                    if isinstance(record, rtlog.DoorAlarmStatusRecord):
+                        last_record_is_status = True
+
+                if last_record_is_status:
+                    time.sleep(10)
+        except KeyboardInterrupt:
+            pass
+
+    panel.disconnect()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zkaccess_c3-0.0.2/pyproject.toml` & `zkaccess_c3-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-[project]
-name = "zkaccess_c3"
-version = "0.0.2"
-description = "A native Python library for communicating with the ZKAccess C3 Access Control Panels."
-authors = [
-    {name = "Vwout", email="vwout@users.noreply.github.com"},
-]
-#license = "GPL-3.0-or-later"
-readme = "readme.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/vwout/zkaccess-c3-py"
-"Bug Tracker" = "https://github.com/vwout/zkaccess-c3-py/issues"
-
-[build-system]
-requires = ["setuptools>=61.0", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
-include = ["c3"]
-exclude = [".github"]
-
-[tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
-
-[tool.pylint]
-max-line-length = 120
+[project]
+name = "zkaccess_c3"
+version = "0.0.3"
+description = "A native Python library for communicating with the ZKAccess C3 Access Control Panels."
+authors = [
+    {name = "Vwout", email="vwout@users.noreply.github.com"},
+]
+#license = "GPL-3.0-or-later"
+readme = "readme.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/vwout/zkaccess-c3-py"
+"Bug Tracker" = "https://github.com/vwout/zkaccess-c3-py/issues"
+
+[build-system]
+requires = ["setuptools>=61.0", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+include = ["c3"]
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
+
+[tool.pylint]
+max-line-length = 120
 disable = ["C0114", "C0115", "C0116", "C0209", "R0801"]
```

### Comparing `zkaccess_c3-0.0.2/readme.md` & `zkaccess_c3-0.0.3/readme.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# c3
-A native Python library for communicating with the ZKTeco ZKAccess C3 Access Control Panels.
-
-This library intends to implement the same functionality as provided by the ZKAccess C3 PullSDK API, but using native Python only.
-It is a port and extension of my (C3 Lua library)[../zkaccess-c3-lua].
-
-## Usage
-To use the library, import the main class:
-```
-from c3 import C3
-```
-A panel connection can be created from the main class `C3`:
-```
-    panel = C3()
-    if panel.connect(ip):
-      panel.get_device_param(["~SerialNumber", "LockCount")
-```
-To use the real-time log (RTLog), or control outputs, also include the helper classes from `controldevice` and `rtlog`.
-
-## Protocol
-The C3 access panels communicate using RS485 or TCP/IP.
-This library only support TCP/IP connections using IPv4.
-The connection is optionally secured by a password.
-Connections to C3 panels that use a password are not supported for this moment.
-
-The wire protocol for the access panels is binary, with the following datagram both for requests (from client to equipment) and responses:
-
-| Byte        | 0      | 1       | 2       | 3          | 4          | 5,6,7,8, ...  | n-2, n-1 | n       |
-|-------------|--------|---------|---------|------------|------------|---------------|----------|---------|
-| **Meaning** | Start  | Version | Command | Length Lsb | Length Msb | Data          | Checksum | End     |
-|  **Value**  | `0xAA` | `0x01`  |         |            |            |               |          | `0x55`  |
-
-The start bytes 0, 1 and last byte have a fixed value.
-The *Command* is one of the following (only listing commands supported by this library)
-
-| Code   | Command                                             |
-|--------|-----------------------------------------------------|
-| `0x76` | Connect (session initiation)                        |
-| `0x02` | Disconnection (session end)                         |
-| `0x05` | Device control command                              |
-| `0x0B` | Retrieve realtime log                               |
-| `0xC8` | Response (confirm successful execution of command)  |
-
-The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
-The *Data* field (as of byte 5) typically has at least 4 bytes:
-- Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
-- Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from 0 (the session initiation command) and is increased with every command send
-
-| Byte         | 5             | 6             | 7              | 8              | ...      |
-|--------------|---------------|---------------|----------------|----------------|----------|
-|  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
-
-The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
-
-## API
-### Connect
-```
-connect(host, port=4370)
-```
-The method is used to connect a C3 device using TCP. 
-RS485 is not supported,  neither is using a password to secure the connection.
-This method must be called before any other method and initializes a C3 session.
-Returns true in case of a successful connection.
-
-### Disconnect
-```
-disconnect()
-```
-
-Disconnects from the C3 access panel and ends the session.
-
-### Get RTLog (real-time log)
-```
-get_rt_log()
-```
-
-This method acquires the realtime event log generated by the access panel. 
-It contains the door and/or alarm status of the equipment.
-It returns an array of DoorAlarmStatusRecord and/or EventRecord objects.
-
-### Get Device Parameters
-```
-get_device_param(params_arr)
-```
-
-This method reads device parameters, both configuration and static parameters.
-The argument is a list of (maximum 30) strings with the parameter names for which the values need to be returned. Valid values are (reduced list):
-   ~SerialNumber, AntiPassback, AuxInCount, AuxOutCount, BackupTime, ComPwd, DateTime, DaylightSavingTime, DaylightSavingTimeOn, DLSTMode, Door{N}CancelKeepOpenDay, Door{N}CloseAndLock, Door{N}Detectortime, Door{N}Drivertime, Door{N}FirstCardOpenDoor, Door{N}ForcePassWord, Door{N}Intertime, Door{N}KeepOpenTimeZone, Door{N}MultiCardOpenDoor, Door{N}SensorType, Door{N}SupperPassWord, Door{N}ValidTZ, Door{N}VerifyType, GATEIPAddress, InBIOTowWay , InterLock, IPAddress, LockCount, NetMask, ReaderCount, Reboot, RS232BaudRate, StandardTime, WatchDog, WeekOfMonth{N},
-For the full list and the meaning of the returned value, refer to the PullSDK specification.
-The return value is a table of key/value pairs with the parameter name and value.
-
-### Control Device
-```
-control_device(control_command_object)
-```
-
-Sends a control command to the access panel to perform an action on the requipment. The control_command is an instance of one of the following objects:
-- `ControlDeviceOutput(output_number, address, duration)`: Open or close a door or auxiliary device
-  - *output_number*: The number of the door or auxiliary to control (1-4)
-  - *address*: Determines whether *door_number* is a door (*address* = 1) or an auxiliary (*address* = 2)
-  - *duration*: The duration for which the door will be open; 0 will close the door immediately, 1-254 will leave the door open for that number of seconds: 255 will leave the door open for an undetermined period
-- `ControlDeviceCancelAlarms()`: Cancel any triggered alarm
-- `ControlDeviceRestart()`: Reboot the access panel
-- `ControlDeviceNormalOpenStateEnable(door_number, enable_disable)`: Change the normal open/close state for the door controller
-  - *door_number*: The number of the door to control (1-4)
-  - *enable*: Enable normally open mode (*enable* = True) or disable normally open mode for the door (*enable_disable* = 0, default)
-
-### Set log level
-```
-log_level(level)
-```
-Sets the logging level, using the Python logging levels.
+# c3
+A native Python library for communicating with the ZKTeco ZKAccess C3 Access Control Panels.
+
+This library intends to implement the same functionality as provided by the ZKAccess C3 PullSDK API, but using native Python only.
+It is a port and extension of my (C3 Lua library)[../zkaccess-c3-lua].
+
+## Usage
+To use the library, import the main class:
+```
+from c3 import C3
+```
+A panel connection can be created from the main class `C3`:
+```
+    panel = C3()
+    if panel.connect(ip):
+      panel.get_device_param(["~SerialNumber", "LockCount")
+```
+To use the real-time log (RTLog), or control outputs, also include the helper classes from `controldevice` and `rtlog`.
+
+## Protocol
+The C3 access panels communicate using RS485 or TCP/IP.
+This library only support TCP/IP connections using IPv4.
+The connection is optionally secured by a password.
+Connections to C3 panels that use a password are not supported for this moment.
+
+The wire protocol for the access panels is binary, with the following datagram both for requests (from client to equipment) and responses:
+
+| Byte        | 0      | 1       | 2       | 3          | 4          | 5,6,7,8, ...  | n-2, n-1 | n       |
+|-------------|--------|---------|---------|------------|------------|---------------|----------|---------|
+| **Meaning** | Start  | Version | Command | Length Lsb | Length Msb | Data          | Checksum | End     |
+|  **Value**  | `0xAA` | `0x01`  |         |            |            |               |          | `0x55`  |
+
+The start bytes 0, 1 and last byte have a fixed value.
+The *Command* is one of the following (only listing commands supported by this library)
+
+| Code   | Command                                             |
+|--------|-----------------------------------------------------|
+| `0x76` | Connect (session initiation)                        |
+| `0x02` | Disconnection (session end)                         |
+| `0x05` | Device control command                              |
+| `0x0B` | Retrieve realtime log                               |
+| `0xC8` | Response (confirm successful execution of command)  |
+
+The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
+The *Data* field (as of byte 5) typically has at least 4 bytes:
+- Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
+- Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from 0 (the session initiation command) and is increased with every command send
+
+| Byte         | 5             | 6             | 7              | 8              | ...      |
+|--------------|---------------|---------------|----------------|----------------|----------|
+|  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
+
+The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
+
+## API
+### Connect
+```
+connect(host, port=4370)
+```
+The method is used to connect a C3 device using TCP. 
+RS485 is not supported,  neither is using a password to secure the connection.
+This method must be called before any other method and initializes a C3 session.
+Returns true in case of a successful connection.
+
+### Disconnect
+```
+disconnect()
+```
+
+Disconnects from the C3 access panel and ends the session.
+
+### Get RTLog (real-time log)
+```
+get_rt_log()
+```
+
+This method acquires the realtime event log generated by the access panel. 
+It contains the door and/or alarm status of the equipment.
+It returns an array of DoorAlarmStatusRecord and/or EventRecord objects.
+
+### Get Device Parameters
+```
+get_device_param(params_arr)
+```
+
+This method reads device parameters, both configuration and static parameters.
+The argument is a list of (maximum 30) strings with the parameter names for which the values need to be returned. Valid values are (reduced list):
+   ~SerialNumber, AntiPassback, AuxInCount, AuxOutCount, BackupTime, ComPwd, DateTime, DaylightSavingTime, DaylightSavingTimeOn, DLSTMode, Door{N}CancelKeepOpenDay, Door{N}CloseAndLock, Door{N}Detectortime, Door{N}Drivertime, Door{N}FirstCardOpenDoor, Door{N}ForcePassWord, Door{N}Intertime, Door{N}KeepOpenTimeZone, Door{N}MultiCardOpenDoor, Door{N}SensorType, Door{N}SupperPassWord, Door{N}ValidTZ, Door{N}VerifyType, GATEIPAddress, InBIOTowWay , InterLock, IPAddress, LockCount, NetMask, ReaderCount, Reboot, RS232BaudRate, StandardTime, WatchDog, WeekOfMonth{N},
+For the full list and the meaning of the returned value, refer to the PullSDK specification.
+The return value is a table of key/value pairs with the parameter name and value.
+
+### Control Device
+```
+control_device(control_command_object)
+```
+
+Sends a control command to the access panel to perform an action on the requipment. The control_command is an instance of one of the following objects:
+- `ControlDeviceOutput(output_number, address, duration)`: Open or close a door or auxiliary device
+  - *output_number*: The number of the door or auxiliary to control (1-4)
+  - *address*: Determines whether *door_number* is a door (*address* = 1) or an auxiliary (*address* = 2)
+  - *duration*: The duration for which the door will be open; 0 will close the door immediately, 1-254 will leave the door open for that number of seconds: 255 will leave the door open for an undetermined period
+- `ControlDeviceCancelAlarms()`: Cancel any triggered alarm
+- `ControlDeviceRestart()`: Reboot the access panel
+- `ControlDeviceNormalOpenStateEnable(door_number, enable_disable)`: Change the normal open/close state for the door controller
+  - *door_number*: The number of the door to control (1-4)
+  - *enable*: Enable normally open mode (*enable* = True) or disable normally open mode for the door (*enable_disable* = 0, default)
+
+### Set log level
+```
+log_level(level)
+```
+Sets the logging level, using the Python logging levels.
```

### Comparing `zkaccess_c3-0.0.2/tests/test_controldevice.py` & `zkaccess_c3-0.0.3/tests/test_controldevice.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from c3 import controldevice
-from c3 import consts
-
-
-def test_c3_device_control_message_output_door():
-    output_operation = controldevice.ControlDeviceOutput(1, consts.ControlOutputAddress.DOOR_OUTPUT, 200)
-    assert bytes([0x01, 0x01, 0x01, 0xc8, 0x00]) == output_operation.to_bytes()
-    print(repr(output_operation))
-
-
-def test_c3_device_control_message_output_door_int():
-    output_operation = controldevice.ControlDeviceOutput(3, 1, 200)
-    assert bytes([0x01, 0x03, 0x01, 0xc8, 0x00]) == output_operation.to_bytes()
-    print(repr(output_operation))
-
-
-def test_c3_device_control_message_output_aux():
-    output_operation = controldevice.ControlDeviceOutput(2, consts.ControlOutputAddress.AUX_OUTPUT, 100)
-    assert bytes([0x01, 0x02, 0x02, 0x64, 0x00]) == output_operation.to_bytes()
-    print(repr(output_operation))
-
-
-def test_c3_device_control_message_cancel():
-    output_operation = controldevice.ControlDeviceCancelAlarms()
-    assert bytes([0x02, 0x00, 0x00, 0x00, 0x00]) == output_operation.to_bytes()
-    print(repr(output_operation))
-
-
-def test_c3_device_control_message_restart():
-    output_operation = controldevice.ControlDeviceRestart()
-    assert bytes([0x03, 0x00, 0x00, 0x00, 0x00]) == output_operation.to_bytes()
-    print(repr(output_operation))
-
-
-def test_c3_device_control_message_nostate():
-    output_operation = controldevice.ControlDeviceNormalOpenStateEnable(2, 1)
-    assert bytes([0x04, 0x02, 0x01, 0x00, 0x00]) == output_operation.to_bytes()
+from c3 import controldevice
+from c3 import consts
+
+
+def test_c3_device_control_message_output_door():
+    output_operation = controldevice.ControlDeviceOutput(1, consts.ControlOutputAddress.DOOR_OUTPUT, 200)
+    assert bytes([0x01, 0x01, 0x01, 0xc8, 0x00]) == output_operation.to_bytes()
+    print(repr(output_operation))
+
+
+def test_c3_device_control_message_output_door_int():
+    output_operation = controldevice.ControlDeviceOutput(3, 1, 200)
+    assert bytes([0x01, 0x03, 0x01, 0xc8, 0x00]) == output_operation.to_bytes()
+    print(repr(output_operation))
+
+
+def test_c3_device_control_message_output_aux():
+    output_operation = controldevice.ControlDeviceOutput(2, consts.ControlOutputAddress.AUX_OUTPUT, 100)
+    assert bytes([0x01, 0x02, 0x02, 0x64, 0x00]) == output_operation.to_bytes()
+    print(repr(output_operation))
+
+
+def test_c3_device_control_message_cancel():
+    output_operation = controldevice.ControlDeviceCancelAlarms()
+    assert bytes([0x02, 0x00, 0x00, 0x00, 0x00]) == output_operation.to_bytes()
+    print(repr(output_operation))
+
+
+def test_c3_device_control_message_restart():
+    output_operation = controldevice.ControlDeviceRestart()
+    assert bytes([0x03, 0x00, 0x00, 0x00, 0x00]) == output_operation.to_bytes()
+    print(repr(output_operation))
+
+
+def test_c3_device_control_message_nostate():
+    output_operation = controldevice.ControlDeviceNormalOpenStateEnable(2, 1)
+    assert bytes([0x04, 0x02, 0x01, 0x00, 0x00]) == output_operation.to_bytes()
```

### Comparing `zkaccess_c3-0.0.2/tests/test_crc16.py` & `zkaccess_c3-0.0.3/tests/test_crc16.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from c3 import crc
-
-
-def test_crc_basic():
-    # Test data generated from https, http://www.lammertbies.nl/comm/info/crc-calculation.html
-    assert 0xBB3D == crc.crc16(b'123456789')
-    assert 0xBB3D == crc.crc16(["1", "2", "3", "4", "5", "6", "7", "8", "9"])
-    assert 0xBB3D == crc.crc16({49, 50, 51, 52, 53, 54, 55, 56, 57})
-    assert 0xE9D9 == crc.crc16(b"abcdefg")
-    assert 0x0F65 == crc.crc16(b"0123456789ABCDEF")
-    assert 0x0F65 == crc.crc16((["0123456789", "ABCDEF"]))
-
-
-def test_crc_connect():
-    # Request
-    assert 0x8fd7 == crc.crc16([0x01, 0x76, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00])
-    # Response
-    assert 0x3320 == crc.crc16((0x01, 0xc8, 0x04, 0x00, 0xd6, 0xcd, 0x00, 0x00))
-    # Response
-    assert 0x47c8 == crc.crc16([0x01, 0xc8, 0x04, 0x00, 0x54, 0xf1, 0x00, 0x00])
-
-
-def test_crc_real_log():
-    # Request
-    assert 0xf687 == crc.crc16([0x01, 0x0b, 0x04, 0x00, 0x3e, 0xe3, 0x02, 0x00])
-    # Response
-    assert 0xbf72 == crc.crc16(bytes.fromhex("01 0b 04 00 78 e5 02 00"))
-
-    # Request
-    assert 0xcd2c == crc.crc16([0x01, 0xc8, 0x14, 0x00, 0x78, 0xe5, 0x02, 0x00, 0x03, 0x00, 0x00, 0x00, 0x11, 0x00,
-                                0x00, 0x00, 0x00, 0x01, 0xff, 0x00, 0x00, 0x33, 0x75, 0x21])
-    # Response
-    assert 0x4f24 == crc.crc16(b'\x01\xc8\x14\x00\x54\xf1\x02\x00\x03\x00\x00\x00\x11\x00\x00\x00\x00\x01\xff\x00\xda'
-                               b'\x3e\x75\x21')
-
-
-def test_crc_disconnect():
-    # Request
-    assert 0x0fde == crc.crc16([0x01, 0x02, 0x04, 0x00, 0x3a, 0xcf, 0x02, 0x00])
-    # Request
-    assert 0x6a75 == crc.crc16([0x01, 0xc8, 0x04, 0x00, 0x3e, 0xe3, 0x03, 0x00])
+from c3 import crc
+
+
+def test_crc_basic():
+    # Test data generated from https, http://www.lammertbies.nl/comm/info/crc-calculation.html
+    assert 0xBB3D == crc.crc16(b'123456789')
+    assert 0xBB3D == crc.crc16(["1", "2", "3", "4", "5", "6", "7", "8", "9"])
+    assert 0xBB3D == crc.crc16({49, 50, 51, 52, 53, 54, 55, 56, 57})
+    assert 0xE9D9 == crc.crc16(b"abcdefg")
+    assert 0x0F65 == crc.crc16(b"0123456789ABCDEF")
+    assert 0x0F65 == crc.crc16((["0123456789", "ABCDEF"]))
+
+
+def test_crc_connect():
+    # Request
+    assert 0x8fd7 == crc.crc16([0x01, 0x76, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00])
+    # Response
+    assert 0x3320 == crc.crc16((0x01, 0xc8, 0x04, 0x00, 0xd6, 0xcd, 0x00, 0x00))
+    # Response
+    assert 0x47c8 == crc.crc16([0x01, 0xc8, 0x04, 0x00, 0x54, 0xf1, 0x00, 0x00])
+
+
+def test_crc_real_log():
+    # Request
+    assert 0xf687 == crc.crc16([0x01, 0x0b, 0x04, 0x00, 0x3e, 0xe3, 0x02, 0x00])
+    # Response
+    assert 0xbf72 == crc.crc16(bytes.fromhex("01 0b 04 00 78 e5 02 00"))
+
+    # Request
+    assert 0xcd2c == crc.crc16([0x01, 0xc8, 0x14, 0x00, 0x78, 0xe5, 0x02, 0x00, 0x03, 0x00, 0x00, 0x00, 0x11, 0x00,
+                                0x00, 0x00, 0x00, 0x01, 0xff, 0x00, 0x00, 0x33, 0x75, 0x21])
+    # Response
+    assert 0x4f24 == crc.crc16(b'\x01\xc8\x14\x00\x54\xf1\x02\x00\x03\x00\x00\x00\x11\x00\x00\x00\x00\x01\xff\x00\xda'
+                               b'\x3e\x75\x21')
+
+
+def test_crc_disconnect():
+    # Request
+    assert 0x0fde == crc.crc16([0x01, 0x02, 0x04, 0x00, 0x3a, 0xcf, 0x02, 0x00])
+    # Request
+    assert 0x6a75 == crc.crc16([0x01, 0xc8, 0x04, 0x00, 0x3e, 0xe3, 0x03, 0x00])
```

### Comparing `zkaccess_c3-0.0.2/tests/test_rtlog.py` & `zkaccess_c3-0.0.3/tests/test_rtlog.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from c3.rtlog import EventRecord, DoorAlarmStatusRecord
-from c3.utils import C3DateTime
-
-
-def test_c3_rtlog_event_decode1():
-    raw_data = bytes([0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xc8, 0x01, 0x66, 0x02, 0x32, 0x8f, 0xae, 0x21])
-    # assert 1501491250 == int.from_bytes(raw_data[12:16], byteorder="little") #11439922
-    # assert 1501491250 == int.from_bytes(raw_data[12:16], byteorder="big") #3313582
-    # assert 1501491250 == int.from_bytes(reversed(raw_data[12:16]), byteorder="little") # 3313582
-    # assert 1501491250 == int.from_bytes(reversed(raw_data[12:16]), byteorder="big") #11439922
-    record = EventRecord.from_bytes(raw_data)
-    # assert C3DateTime.from_value(1501491250) == record.time_second
-    assert C3DateTime(year=2017, month=7, day=31, hour=8, minute=54, second=10) == record.time_second
-    assert not record.is_door_alarm()
-    assert record.is_event()
-    print(repr(record))
-
-
-def test_c3_rtlog_event_decode2():
-    raw_data = bytes([0x17, 0x30, 0x64, 0x12, 0xe2, 0xb1, 0x04, 0x00, 0x04, 0x01, 0x00, 0x00, 0x74, 0x2c, 0xaf, 0x21])
-    record = EventRecord.from_bytes(raw_data)
-    # assert C3DateTime.from_value(1501531508) == record.time_second
-    assert not record.is_door_alarm()
-    assert record.is_event()
-    print(repr(record))
-
-
-def test_c3_rtlog_decode_status1():
-    raw_data = bytes([0x03, 0x00, 0x00, 0x00, 0x11, 0x00, 0x00, 0x00, 0x00, 0x01, 0xff, 0x00, 0xf2, 0x31, 0xb3, 0x21])
-    record = DoorAlarmStatusRecord.from_bytes(raw_data)
-    assert 0 < len(record.get_alarms(door_nr=None))
-    assert record.has_alarm(1)
-    assert not record.has_alarm(2)
-    assert record.has_alarm(1, 1)
-    assert record.has_alarm(1, 2)
-    # assert not record.has_alarm(1, 3)
-    assert False is record.door_is_open(1)
-    assert None is record.door_is_open(3)
-    assert record.is_door_alarm()
-    assert not record.is_event()
-    print(repr(record))
-
-
-def test_c3_rtlog_decode_status2():
-    raw_data = bytes([0x03, 0x00, 0x00, 0x00, 0x02, 0x00, 0x00, 0x00, 0x01, 0x01, 0xff, 0x00, 0xfc, 0x31, 0xb3, 0x21])
-    record = DoorAlarmStatusRecord.from_bytes(raw_data)
-    assert record.has_alarm(1)
-    assert record.door_is_open(1)
-    assert None is record.door_is_open(2)
-    assert record.is_door_alarm()
-    assert not record.is_event()
-    print(repr(record))
+from c3.rtlog import EventRecord, DoorAlarmStatusRecord
+from c3.utils import C3DateTime
+
+
+def test_c3_rtlog_event_decode1():
+    raw_data = bytes([0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xc8, 0x01, 0x66, 0x02, 0x32, 0x8f, 0xae, 0x21])
+    # assert 1501491250 == int.from_bytes(raw_data[12:16], byteorder="little") #11439922
+    # assert 1501491250 == int.from_bytes(raw_data[12:16], byteorder="big") #3313582
+    # assert 1501491250 == int.from_bytes(reversed(raw_data[12:16]), byteorder="little") # 3313582
+    # assert 1501491250 == int.from_bytes(reversed(raw_data[12:16]), byteorder="big") #11439922
+    record = EventRecord.from_bytes(raw_data)
+    # assert C3DateTime.from_value(1501491250) == record.time_second
+    assert C3DateTime(year=2017, month=7, day=31, hour=8, minute=54, second=10) == record.time_second
+    assert not record.is_door_alarm()
+    assert record.is_event()
+    print(repr(record))
+
+
+def test_c3_rtlog_event_decode2():
+    raw_data = bytes([0x17, 0x30, 0x64, 0x12, 0xe2, 0xb1, 0x04, 0x00, 0x04, 0x01, 0x00, 0x00, 0x74, 0x2c, 0xaf, 0x21])
+    record = EventRecord.from_bytes(raw_data)
+    # assert C3DateTime.from_value(1501531508) == record.time_second
+    assert not record.is_door_alarm()
+    assert record.is_event()
+    print(repr(record))
+
+
+def test_c3_rtlog_decode_status1():
+    raw_data = bytes([0x03, 0x00, 0x00, 0x00, 0x11, 0x00, 0x00, 0x00, 0x00, 0x01, 0xff, 0x00, 0xf2, 0x31, 0xb3, 0x21])
+    record = DoorAlarmStatusRecord.from_bytes(raw_data)
+    assert 0 < len(record.get_alarms(door_nr=None))
+    assert record.has_alarm(1)
+    assert not record.has_alarm(2)
+    assert record.has_alarm(1, 1)
+    assert record.has_alarm(1, 2)
+    # assert not record.has_alarm(1, 3)
+    assert False is record.door_is_open(1)
+    assert None is record.door_is_open(3)
+    assert record.is_door_alarm()
+    assert not record.is_event()
+    print(repr(record))
+
+
+def test_c3_rtlog_decode_status2():
+    raw_data = bytes([0x03, 0x00, 0x00, 0x00, 0x02, 0x00, 0x00, 0x00, 0x01, 0x01, 0xff, 0x00, 0xfc, 0x31, 0xb3, 0x21])
+    record = DoorAlarmStatusRecord.from_bytes(raw_data)
+    assert record.has_alarm(1)
+    assert record.door_is_open(1)
+    assert None is record.door_is_open(2)
+    assert record.is_door_alarm()
+    assert not record.is_event()
+    print(repr(record))
```

### Comparing `zkaccess_c3-0.0.2/tests/test_utils.py` & `zkaccess_c3-0.0.3/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from c3.utils import *
-
-
-def test_lsb():
-    assert 0xaa == lsb(0x123aa)
-    assert 0 == lsb(0xAB00)
-
-
-def test_msb():
-    assert 0 == msb(0xEF)
-    assert 0xcd == msb(0x12cd34)
-
-
-def test_c3_datetime_from_value():
-    c3_dt = C3DateTime.from_value(347748895)
-    assert 2010 == c3_dt.year
-    assert 10 == c3_dt.month
-    assert 54 == c3_dt.minute
-
-    assert C3DateTime(year=2017, month=7, day=30, hour=15, minute=24, second=32) == \
-           C3DateTime.from_value(int.from_bytes([0x21, 0xad, 0x99, 0x30], byteorder="big"))
-    assert C3DateTime(year=2013, month=10, day=8, hour=14, minute=38, second=32) == \
-           C3DateTime.from_value(int.from_bytes(reversed([0x1a, 0x61, 0x70, 0xe8]), byteorder="little"))
-
-
-def test_c3_datetime_to_value():
-    c3_dt = C3DateTime(2010, 10, 26, 20, 54, 55)
-    assert 347748895 == c3_dt.to_value()
+from c3.utils import *
+
+
+def test_lsb():
+    assert 0xaa == lsb(0x123aa)
+    assert 0 == lsb(0xAB00)
+
+
+def test_msb():
+    assert 0 == msb(0xEF)
+    assert 0xcd == msb(0x12cd34)
+
+
+def test_c3_datetime_from_value():
+    c3_dt = C3DateTime.from_value(347748895)
+    assert 2010 == c3_dt.year
+    assert 10 == c3_dt.month
+    assert 54 == c3_dt.minute
+
+    assert C3DateTime(year=2017, month=7, day=30, hour=15, minute=24, second=32) == \
+           C3DateTime.from_value(int.from_bytes([0x21, 0xad, 0x99, 0x30], byteorder="big"))
+    assert C3DateTime(year=2013, month=10, day=8, hour=14, minute=38, second=32) == \
+           C3DateTime.from_value(int.from_bytes(reversed([0x1a, 0x61, 0x70, 0xe8]), byteorder="little"))
+
+
+def test_c3_datetime_to_value():
+    c3_dt = C3DateTime(2010, 10, 26, 20, 54, 55)
+    assert 347748895 == c3_dt.to_value()
```

### Comparing `zkaccess_c3-0.0.2/zkaccess_c3.egg-info/PKG-INFO` & `zkaccess_c3-0.0.3/zkaccess_c3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess-c3
-Version: 0.0.2
+Version: 0.0.3
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

