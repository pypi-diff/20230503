# Comparing `tmp/jax-relax-0.1.2.tar.gz` & `tmp/jax-relax-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jax-relax-0.1.2.tar", last modified: Thu Apr  6 20:59:29 2023, max compression
+gzip compressed data, was "jax-relax-0.1.3.tar", last modified: Wed May  3 01:54:30 2023, max compression
```

## Comparing `jax-relax-0.1.2.tar` & `jax-relax-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-04-06 20:59:29.000000 jax-relax-0.1.2/
--rw-r--r--   0 birk      (1000) birk      (1000)     2348 2022-12-18 21:09:02.000000 jax-relax-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 birk      (1000) birk      (1000)    11357 2022-12-18 21:09:02.000000 jax-relax-0.1.2/LICENSE
--rw-r--r--   0 birk      (1000) birk      (1000)      111 2022-12-18 21:09:02.000000 jax-relax-0.1.2/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     3128 2023-04-06 20:59:29.000000 jax-relax-0.1.2/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     2288 2023-02-08 15:53:10.000000 jax-relax-0.1.2/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-04-06 20:59:29.000000 jax-relax-0.1.2/jax_relax.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     3128 2023-04-06 20:59:28.000000 jax-relax-0.1.2/jax_relax.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)      751 2023-04-06 20:59:28.000000 jax-relax-0.1.2/jax_relax.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-04-06 20:59:28.000000 jax-relax-0.1.2/jax_relax.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-04-06 20:59:28.000000 jax-relax-0.1.2/jax_relax.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2022-12-19 10:47:31.000000 jax-relax-0.1.2/jax_relax.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      188 2023-04-06 20:59:28.000000 jax-relax-0.1.2/jax_relax.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-04-06 20:59:28.000000 jax-relax-0.1.2/jax_relax.egg-info/top_level.txt
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-04-06 20:59:29.000000 jax-relax-0.1.2/relax/
--rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-04-06 20:59:06.000000 jax-relax-0.1.2/relax/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/_ckpt_manager.py
--rw-r--r--   0 birk      (1000) birk      (1000)    62848 2023-04-06 20:59:06.000000 jax-relax-0.1.2/relax/_modidx.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-04-06 20:59:29.000000 jax-relax-0.1.2/relax/data/
--rw-r--r--   0 birk      (1000) birk      (1000)      115 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/data/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-04-06 14:30:59.000000 jax-relax-0.1.2/relax/data/loader.py
--rw-r--r--   0 birk      (1000) birk      (1000)    17786 2023-04-06 14:30:59.000000 jax-relax-0.1.2/relax/data/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/data/scm.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-04-06 14:30:59.000000 jax-relax-0.1.2/relax/docs.py
--rw-r--r--   0 birk      (1000) birk      (1000)    15209 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/evaluate.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1262 2023-04-06 20:59:06.000000 jax-relax-0.1.2/relax/import_essentials.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/logger.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-04-06 20:59:29.000000 jax-relax-0.1.2/relax/methods/
--rw-r--r--   0 birk      (1000) birk      (1000)      192 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/methods/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1903 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/methods/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12118 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/methods/counternet.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6307 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/methods/diverse.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9255 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/methods/proto.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7475 2023-04-06 20:59:06.000000 jax-relax-0.1.2/relax/methods/sphere.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3963 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/methods/vanilla.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7583 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/plots.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4736 2023-04-06 14:31:00.000000 jax-relax-0.1.2/relax/trainer.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6761 2023-04-06 14:30:59.000000 jax-relax-0.1.2/relax/utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1101 2023-04-06 20:59:06.000000 jax-relax-0.1.2/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-04-06 20:59:29.000000 jax-relax-0.1.2/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     2541 2022-12-18 21:09:02.000000 jax-relax-0.1.2/setup.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/
+-rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-01-17 02:27:26.000000 jax-relax-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 birk      (1000) birk      (1000)    11558 2023-01-17 02:27:26.000000 jax-relax-0.1.3/LICENSE
+-rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-01-17 02:27:26.000000 jax-relax-0.1.3/MANIFEST.in
+-rw-r--r--   0 birk      (1000) birk      (1000)     3355 2023-05-03 01:54:30.571084 jax-relax-0.1.3/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     2515 2023-05-03 01:52:41.000000 jax-relax-0.1.3/README.md
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.561084 jax-relax-0.1.3/jax_relax.egg-info/
+-rw-r--r--   0 birk      (1000) birk      (1000)     3355 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/SOURCES.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/dependency_links.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/entry_points.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-17 02:38:00.000000 jax-relax-0.1.3/jax_relax.egg-info/not-zip-safe
+-rw-r--r--   0 birk      (1000) birk      (1000)      199 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/requires.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/top_level.txt
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/relax/
+-rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/_ckpt_manager.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    79877 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/_modidx.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/relax/data/
+-rw-r--r--   0 birk      (1000) birk      (1000)      117 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/loader.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    17786 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/scm.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/docs.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    15503 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/evaluate.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1296 2023-04-19 16:19:35.000000 jax-relax-0.1.3/relax/import_essentials.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/logger.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/relax/methods/
+-rw-r--r--   0 birk      (1000) birk      (1000)      196 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1959 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/base.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11115 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/cchvae.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    14082 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/clue.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12537 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/counternet.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6298 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/diverse.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9273 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/proto.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7548 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/sphere.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11112 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/vaecf.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3958 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/vanilla.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7736 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/plots.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4788 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/trainer.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6738 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/utils.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1112 2023-05-03 01:53:37.000000 jax-relax-0.1.3/settings.ini
+-rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-03 01:54:30.571084 jax-relax-0.1.3/setup.cfg
+-rw-r--r--   0 birk      (1000) birk      (1000)     2598 2023-01-17 02:27:26.000000 jax-relax-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jax-relax-0.1.2/CONTRIBUTING.md` & `jax-relax-0.1.3/CONTRIBUTING.md`

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

### Comparing `jax-relax-0.1.2/LICENSE` & `jax-relax-0.1.3/LICENSE`

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

### Comparing `jax-relax-0.1.2/PKG-INFO` & `jax-relax-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,70 @@
-Metadata-Version: 2.1
-Name: jax-relax
-Version: 0.1.2
-Summary: Jax-based Recourse Explanation Library
-Home-page: https://github.com/birkhoffg/relax/tree/master/
-Author: BirkhoffG
-Author-email: 26811230+BirkhoffG@users.noreply.github.com
-License: Apache Software License 2.0
-Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-ReLax
-================
+# ReLax
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ![Python](https://img.shields.io/pypi/pyversions/jax-relax.svg) ![CI
 status](https://github.com/BirkhoffG/ReLax/actions/workflows/test.yaml/badge.svg)
 ![Docs](https://github.com/BirkhoffG/ReLax/actions/workflows/deploy.yaml/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/jax-relax.svg) ![GitHub
 License](https://img.shields.io/github/license/BirkhoffG/ReLax.svg)
 
 [**Overview**](#overview) \| [**Installation**](#installation) \|
-[**Tutorials**](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html) \|
-[**Documentation**](https://birkhoffg.github.io/ReLax/) \| [**Citing
+[**Tutorials**](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html)
+\| [**Documentation**](https://birkhoffg.github.io/ReLax/) \| [**Citing
 ReLax**](#citing-relax)
 
 ## Overview
 
 `ReLax` (**Re**course Explanation **L**ibrary in J**ax**) is a library
 built on top of `jax` to generate counterfactual and recourse
-explanations. By leveraging *vectorization* though `vmap`/`pmap` and
-*just-in-time* compilation in `jax`, `ReLax` offers massive speed
-improvements in generating individual (or local) explanations.
+explanations for Machine Learning algorithms. By leveraging
+*vectorization* though `vmap`/`pmap` and *just-in-time* compilation in
+[jax](https://jax.readthedocs.io/en/latest/) (a high-performance
+auto-differentiation library). `ReLax` offers massive speed improvements
+in generating individual (or local) explanations for predictions made by
+Machine Learning algorithms.
 
-Some of the key features:
+Some of the key features are as follows:
 
 - 🏃 **Fast** recourse generation via `jax.jit`, `jax.vmap`/`jax.pmap`.
 
 - 🚀 **Accelerated** over `cpu`, `gpu`, `tpu`.
 
-- 🪓 **Extensive** recourse methods implemented for benchmarking.
+- 🪓 **Comprehensive** set of recourse methods implemented for
+  benchmarking.
+
+- 👐 **Customizable** API to enable the building of entire modeling
 
-- 👐 **Customizable** API to enable building entire modeling and
-  interpreting pipeline.
+- and interpretation pipelines for new recourse algorithms.
 
 ## Installation
 
 The latest `ReLax` release can directly be installed from PyPI:
 
 ``` bash
 pip install jax-relax
 ```
 
-or install directly from the repository:
+or installed directly from the repository:
 
 ``` bash
 pip install git+https://github.com/BirkhoffG/ReLax.git 
 ```
 
 To futher unleash the power of accelerators (i.e., GPU/TPU), we suggest
 to first install this library via `pip install jax-relax`. Then, follow
 steps in the [official install
 guidelines](https://github.com/google/jax#installation) to install the
 right version for GPU or TPU.
 
 ## An Example of using `ReLax`
 
-See [Getting Started with ReLax](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html).
+See [Getting Started with
+ReLax](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html).
 
 ## Citing `ReLax`
 
 To cite this repository:
 
 ``` latex
 @software{relax2023github,
```

### Comparing `jax-relax-0.1.2/jax_relax.egg-info/SOURCES.txt` & `jax-relax-0.1.3/jax_relax.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -24,12 +24,15 @@
 relax/utils.py
 relax/data/__init__.py
 relax/data/loader.py
 relax/data/module.py
 relax/data/scm.py
 relax/methods/__init__.py
 relax/methods/base.py
+relax/methods/cchvae.py
+relax/methods/clue.py
 relax/methods/counternet.py
 relax/methods/diverse.py
 relax/methods/proto.py
 relax/methods/sphere.py
+relax/methods/vaecf.py
 relax/methods/vanilla.py
```

### Comparing `jax-relax-0.1.2/relax/_ckpt_manager.py` & `jax-relax-0.1.3/relax/_ckpt_manager.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/_modidx.py` & `jax-relax-0.1.3/relax/_modidx.py`

 * *Files 18% similar despite different names*

```diff
@@ -239,14 +239,15 @@
                                 'relax.evaluate._AuxPredFn': ('evaluate.html#_auxpredfn', 'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn.__call__': ('evaluate.html#_auxpredfn.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn.__init__': ('evaluate.html#_auxpredfn.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate._check_aux_pred_fn_args': ('evaluate.html#_check_aux_pred_fn_args', 'relax/evaluate.py'),
                                 'relax.evaluate._check_pred_fn': ('evaluate.html#_check_pred_fn', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_acc': ('evaluate.html#_compute_acc', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_manifold_dist': ('evaluate.html#_compute_manifold_dist', 'relax/evaluate.py'),
+                                'relax.evaluate._compute_proximity': ('evaluate.html#_compute_proximity', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_spar': ('evaluate.html#_compute_spar', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_val': ('evaluate.html#_compute_val', 'relax/evaluate.py'),
                                 'relax.evaluate._create_second_order_cfs': ('evaluate.html#_create_second_order_cfs', 'relax/evaluate.py'),
                                 'relax.evaluate._get_metric': ('evaluate.html#_get_metric', 'relax/evaluate.py'),
                                 'relax.evaluate._prepare_module': ('evaluate.html#_prepare_module', 'relax/evaluate.py'),
                                 'relax.evaluate._train_parametric_module': ('evaluate.html#_train_parametric_module', 'relax/evaluate.py'),
                                 'relax.evaluate._validate_configs': ('evaluate.html#_validate_configs', 'relax/evaluate.py'),
@@ -287,153 +288,290 @@
                                                                                                       'relax/methods/base.py'),
                                     'relax.methods.base.BaseParametricCFModule.train': ( 'methods.base.html#baseparametriccfmodule.train',
                                                                                          'relax/methods/base.py'),
                                     'relax.methods.base.BasePredFnCFModule': ( 'methods.base.html#basepredfncfmodule',
                                                                                'relax/methods/base.py'),
                                     'relax.methods.base.BasePredFnCFModule.pred_fn': ( 'methods.base.html#basepredfncfmodule.pred_fn',
                                                                                        'relax/methods/base.py')},
-            'relax.methods.counternet': { 'relax.methods.counternet.CounterNet': ( 'methods.counternet.html#counternet',
+            'relax.methods.cchvae': { 'relax.methods.cchvae.CCHVAE': ('methods/cchvae.html#cchvae', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.__init__': ( 'methods/cchvae.html#cchvae.__init__',
+                                                                                'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE._is_module_trained': ( 'methods/cchvae.html#cchvae._is_module_trained',
+                                                                                          'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.generate_cfs': ( 'methods/cchvae.html#cchvae.generate_cfs',
+                                                                                    'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.train': ('methods/cchvae.html#cchvae.train', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAEConfigs': ( 'methods/cchvae.html#cchvaeconfigs',
+                                                                              'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE': ('methods/cchvae.html#chvae', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.__init__': ( 'methods/cchvae.html#chvae.__init__',
+                                                                               'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.__reparameterize': ( 'methods/cchvae.html#chvae.__reparameterize',
+                                                                                       'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE._training_step': ( 'methods/cchvae.html#chvae._training_step',
+                                                                                     'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.decode': ('methods/cchvae.html#chvae.decode', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.encode': ('methods/cchvae.html#chvae.encode', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.forward': ( 'methods/cchvae.html#chvae.forward',
+                                                                              'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.init_net_opt': ( 'methods/cchvae.html#chvae.init_net_opt',
+                                                                                   'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.loss': ('methods/cchvae.html#chvae.loss', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.training_step': ( 'methods/cchvae.html#chvae.training_step',
+                                                                                    'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.validation_step': ( 'methods/cchvae.html#chvae.validation_step',
+                                                                                      'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAEConfigs': ('methods/cchvae.html#chvaeconfigs', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.Decoder': ('methods/cchvae.html#decoder', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.Decoder.__call__': ( 'methods/cchvae.html#decoder.__call__',
+                                                                                 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.Decoder.__init__': ( 'methods/cchvae.html#decoder.__init__',
+                                                                                 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.Encoder': ('methods/cchvae.html#encoder', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.Encoder.__call__': ( 'methods/cchvae.html#encoder.__call__',
+                                                                                 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.Encoder.__init__': ( 'methods/cchvae.html#encoder.__init__',
+                                                                                 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae._cchvae_generate': ( 'methods/cchvae.html#_cchvae_generate',
+                                                                                 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae._hyper_sphere_coordindates': ( 'methods/cchvae.html#_hyper_sphere_coordindates',
+                                                                                           'relax/methods/cchvae.py')},
+            'relax.methods.clue': { 'relax.methods.clue.CLUE': ('methods/clue.html#clue', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.__init__': ('methods/clue.html#clue.__init__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE._is_module_trained': ( 'methods/clue.html#clue._is_module_trained',
+                                                                                    'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.generate_cf': ('methods/clue.html#clue.generate_cf', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.generate_cfs': ( 'methods/clue.html#clue.generate_cfs',
+                                                                              'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.train': ('methods/clue.html#clue.train', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUEConfigs': ('methods/clue.html#clueconfigs', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Decoder': ('methods/clue.html#decoder', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Decoder.__call__': ('methods/clue.html#decoder.__call__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Decoder.__init__': ('methods/clue.html#decoder.__init__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Encoder': ('methods/clue.html#encoder', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Encoder.__call__': ('methods/clue.html#encoder.__call__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Encoder.__init__': ('methods/clue.html#encoder.__init__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat': ('methods/clue.html#vaegausscat', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.__init__': ( 'methods/clue.html#vaegausscat.__init__',
+                                                                                 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat._training_step': ( 'methods/clue.html#vaegausscat._training_step',
+                                                                                       'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat._update_categorical_info': ( 'methods/clue.html#vaegausscat._update_categorical_info',
+                                                                                                 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.compute_loss': ( 'methods/clue.html#vaegausscat.compute_loss',
+                                                                                     'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.decode': ( 'methods/clue.html#vaegausscat.decode',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.encode': ( 'methods/clue.html#vaegausscat.encode',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.init_net_opt': ( 'methods/clue.html#vaegausscat.init_net_opt',
+                                                                                     'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample': ( 'methods/clue.html#vaegausscat.sample',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample_latent': ( 'methods/clue.html#vaegausscat.sample_latent',
+                                                                                      'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample_prior': ( 'methods/clue.html#vaegausscat.sample_prior',
+                                                                                     'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample_step': ( 'methods/clue.html#vaegausscat.sample_step',
+                                                                                    'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.training_step': ( 'methods/clue.html#vaegausscat.training_step',
+                                                                                      'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.validation_step': ( 'methods/clue.html#vaegausscat.validation_step',
+                                                                                        'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCatConfigs': ( 'methods/clue.html#vaegausscatconfigs',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue._clue_generate': ('methods/clue.html#_clue_generate', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.kl_divergence': ('methods/clue.html#kl_divergence', 'relax/methods/clue.py')},
+            'relax.methods.counternet': { 'relax.methods.counternet.CounterNet': ( 'methods/counternet.html#counternet',
                                                                                    'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.__init__': ( 'methods.counternet.html#counternet.__init__',
+                                          'relax.methods.counternet.CounterNet.__init__': ( 'methods/counternet.html#counternet.__init__',
                                                                                             'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet._is_module_trained': ( 'methods.counternet.html#counternet._is_module_trained',
+                                          'relax.methods.counternet.CounterNet._is_module_trained': ( 'methods/counternet.html#counternet._is_module_trained',
                                                                                                       'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.generate_cfs': ( 'methods.counternet.html#counternet.generate_cfs',
+                                          'relax.methods.counternet.CounterNet.generate_cfs': ( 'methods/counternet.html#counternet.generate_cfs',
                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.pred_fn': ( 'methods.counternet.html#counternet.pred_fn',
+                                          'relax.methods.counternet.CounterNet.pred_fn': ( 'methods/counternet.html#counternet.pred_fn',
                                                                                            'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.train': ( 'methods.counternet.html#counternet.train',
+                                          'relax.methods.counternet.CounterNet.train': ( 'methods/counternet.html#counternet.train',
                                                                                          'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetConfigs': ( 'methods.counternet.html#counternetconfigs',
+                                          'relax.methods.counternet.CounterNetConfigs': ( 'methods/counternet.html#counternetconfigs',
                                                                                           'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModel': ( 'methods.counternet.html#counternetmodel',
+                                          'relax.methods.counternet.CounterNetModel': ( 'methods/counternet.html#counternetmodel',
                                                                                         'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModel.__call__': ( 'methods.counternet.html#counternetmodel.__call__',
+                                          'relax.methods.counternet.CounterNetModel.__call__': ( 'methods/counternet.html#counternetmodel.__call__',
                                                                                                  'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModel.__init__': ( 'methods.counternet.html#counternetmodel.__init__',
+                                          'relax.methods.counternet.CounterNetModel.__init__': ( 'methods/counternet.html#counternetmodel.__init__',
                                                                                                  'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModelConfigs': ( 'methods.counternet.html#counternetmodelconfigs',
+                                          'relax.methods.counternet.CounterNetModelConfigs': ( 'methods/counternet.html#counternetmodelconfigs',
                                                                                                'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule': ( 'methods.counternet.html#counternettrainingmodule',
+                                          'relax.methods.counternet.CounterNetTrainingModule': ( 'methods/counternet.html#counternettrainingmodule',
                                                                                                  'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.__init__': ( 'methods.counternet.html#counternettrainingmodule.__init__',
+                                          'relax.methods.counternet.CounterNetTrainingModule.__init__': ( 'methods/counternet.html#counternettrainingmodule.__init__',
                                                                                                           'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._explainer_step': ( 'methods.counternet.html#counternettrainingmodule._explainer_step',
+                                          'relax.methods.counternet.CounterNetTrainingModule._explainer_step': ( 'methods/counternet.html#counternettrainingmodule._explainer_step',
                                                                                                                  'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._predictor_step': ( 'methods.counternet.html#counternettrainingmodule._predictor_step',
+                                          'relax.methods.counternet.CounterNetTrainingModule._predictor_step': ( 'methods/counternet.html#counternettrainingmodule._predictor_step',
                                                                                                                  'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._training_step': ( 'methods.counternet.html#counternettrainingmodule._training_step',
+                                          'relax.methods.counternet.CounterNetTrainingModule._training_step': ( 'methods/counternet.html#counternettrainingmodule._training_step',
                                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._training_step_logs': ( 'methods.counternet.html#counternettrainingmodule._training_step_logs',
+                                          'relax.methods.counternet.CounterNetTrainingModule._training_step_logs': ( 'methods/counternet.html#counternettrainingmodule._training_step_logs',
                                                                                                                      'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.exp_loss_fn': ( 'methods.counternet.html#counternettrainingmodule.exp_loss_fn',
+                                          'relax.methods.counternet.CounterNetTrainingModule.exp_loss_fn': ( 'methods/counternet.html#counternettrainingmodule.exp_loss_fn',
                                                                                                              'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.forward': ( 'methods.counternet.html#counternettrainingmodule.forward',
+                                          'relax.methods.counternet.CounterNetTrainingModule.forward': ( 'methods/counternet.html#counternettrainingmodule.forward',
                                                                                                          'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.generate_cfs': ( 'methods.counternet.html#counternettrainingmodule.generate_cfs',
+                                          'relax.methods.counternet.CounterNetTrainingModule.generate_cfs': ( 'methods/counternet.html#counternettrainingmodule.generate_cfs',
                                                                                                               'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.init_net_opt': ( 'methods.counternet.html#counternettrainingmodule.init_net_opt',
+                                          'relax.methods.counternet.CounterNetTrainingModule.init_net_opt': ( 'methods/counternet.html#counternettrainingmodule.init_net_opt',
                                                                                                               'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_1': ( 'methods.counternet.html#counternettrainingmodule.loss_fn_1',
+                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_1': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_1',
                                                                                                            'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_2': ( 'methods.counternet.html#counternettrainingmodule.loss_fn_2',
+                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_2': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_2',
                                                                                                            'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_3': ( 'methods.counternet.html#counternettrainingmodule.loss_fn_3',
+                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_3': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_3',
                                                                                                            'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.pred_loss_fn': ( 'methods.counternet.html#counternettrainingmodule.pred_loss_fn',
+                                          'relax.methods.counternet.CounterNetTrainingModule.pred_loss_fn': ( 'methods/counternet.html#counternettrainingmodule.pred_loss_fn',
                                                                                                               'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.predict': ( 'methods.counternet.html#counternettrainingmodule.predict',
+                                          'relax.methods.counternet.CounterNetTrainingModule.predict': ( 'methods/counternet.html#counternettrainingmodule.predict',
                                                                                                          'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.training_step': ( 'methods.counternet.html#counternettrainingmodule.training_step',
+                                          'relax.methods.counternet.CounterNetTrainingModule.training_step': ( 'methods/counternet.html#counternettrainingmodule.training_step',
                                                                                                                'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.validation_step': ( 'methods.counternet.html#counternettrainingmodule.validation_step',
+                                          'relax.methods.counternet.CounterNetTrainingModule.validation_step': ( 'methods/counternet.html#counternettrainingmodule.validation_step',
                                                                                                                  'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModuleConfigs': ( 'methods.counternet.html#counternettrainingmoduleconfigs',
+                                          'relax.methods.counternet.CounterNetTrainingModuleConfigs': ( 'methods/counternet.html#counternettrainingmoduleconfigs',
                                                                                                         'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.partition_trainable_params': ( 'methods.counternet.html#partition_trainable_params',
+                                          'relax.methods.counternet.partition_trainable_params': ( 'methods/counternet.html#partition_trainable_params',
                                                                                                    'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.project_immutable_features': ( 'methods.counternet.html#project_immutable_features',
+                                          'relax.methods.counternet.project_immutable_features': ( 'methods/counternet.html#project_immutable_features',
                                                                                                    'relax/methods/counternet.py')},
-            'relax.methods.diverse': { 'relax.methods.diverse.DiverseCF': ('methods.diverse.html#diversecf', 'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.DiverseCF.__init__': ( 'methods.diverse.html#diversecf.__init__',
+            'relax.methods.diverse': { 'relax.methods.diverse.DiverseCF': ('methods/diverse.html#diversecf', 'relax/methods/diverse.py'),
+                                       'relax.methods.diverse.DiverseCF.__init__': ( 'methods/diverse.html#diversecf.__init__',
                                                                                      'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.DiverseCF.generate_cf': ( 'methods.diverse.html#diversecf.generate_cf',
+                                       'relax.methods.diverse.DiverseCF.generate_cf': ( 'methods/diverse.html#diversecf.generate_cf',
                                                                                         'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.DiverseCF.generate_cfs': ( 'methods.diverse.html#diversecf.generate_cfs',
+                                       'relax.methods.diverse.DiverseCF.generate_cfs': ( 'methods/diverse.html#diversecf.generate_cfs',
                                                                                          'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.DiverseCFConfig': ( 'methods.diverse.html#diversecfconfig',
+                                       'relax.methods.diverse.DiverseCFConfig': ( 'methods/diverse.html#diversecfconfig',
                                                                                   'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.DiverseCFConfig.keys': ( 'methods.diverse.html#diversecfconfig.keys',
+                                       'relax.methods.diverse.DiverseCFConfig.keys': ( 'methods/diverse.html#diversecfconfig.keys',
                                                                                        'relax/methods/diverse.py'),
-                                       'relax.methods.diverse._compute_regularization_loss': ( 'methods.diverse.html#_compute_regularization_loss',
+                                       'relax.methods.diverse._compute_regularization_loss': ( 'methods/diverse.html#_compute_regularization_loss',
                                                                                                'relax/methods/diverse.py'),
-                                       'relax.methods.diverse._diverse_cf': ( 'methods.diverse.html#_diverse_cf',
+                                       'relax.methods.diverse._diverse_cf': ( 'methods/diverse.html#_diverse_cf',
                                                                               'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.dpp_style': ('methods.diverse.html#dpp_style', 'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.hinge_loss': ('methods.diverse.html#hinge_loss', 'relax/methods/diverse.py'),
-                                       'relax.methods.diverse.l1_mean': ('methods.diverse.html#l1_mean', 'relax/methods/diverse.py')},
-            'relax.methods.proto': { 'relax.methods.proto.AE': ('methods.prototype.html#ae', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.AE.__call__': ('methods.prototype.html#ae.__call__', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.AE.__init__': ('methods.prototype.html#ae.__init__', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.AEConfigs': ('methods.prototype.html#aeconfigs', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule': ( 'methods.prototype.html#aetrainingmodule',
+                                       'relax.methods.diverse.dpp_style': ('methods/diverse.html#dpp_style', 'relax/methods/diverse.py'),
+                                       'relax.methods.diverse.hinge_loss': ('methods/diverse.html#hinge_loss', 'relax/methods/diverse.py'),
+                                       'relax.methods.diverse.l1_mean': ('methods/diverse.html#l1_mean', 'relax/methods/diverse.py')},
+            'relax.methods.proto': { 'relax.methods.proto.AE': ('methods/prototype.html#ae', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.AE.__call__': ('methods/prototype.html#ae.__call__', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.AE.__init__': ('methods/prototype.html#ae.__init__', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.AEConfigs': ('methods/prototype.html#aeconfigs', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.AETrainingModule': ( 'methods/prototype.html#aetrainingmodule',
                                                                                'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.__init__': ( 'methods.prototype.html#aetrainingmodule.__init__',
+                                     'relax.methods.proto.AETrainingModule.__init__': ( 'methods/prototype.html#aetrainingmodule.__init__',
                                                                                         'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule._training_step': ( 'methods.prototype.html#aetrainingmodule._training_step',
+                                     'relax.methods.proto.AETrainingModule._training_step': ( 'methods/prototype.html#aetrainingmodule._training_step',
                                                                                               'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.encode': ( 'methods.prototype.html#aetrainingmodule.encode',
+                                     'relax.methods.proto.AETrainingModule.encode': ( 'methods/prototype.html#aetrainingmodule.encode',
                                                                                       'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.forward': ( 'methods.prototype.html#aetrainingmodule.forward',
+                                     'relax.methods.proto.AETrainingModule.forward': ( 'methods/prototype.html#aetrainingmodule.forward',
                                                                                        'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.init_net_opt': ( 'methods.prototype.html#aetrainingmodule.init_net_opt',
+                                     'relax.methods.proto.AETrainingModule.init_net_opt': ( 'methods/prototype.html#aetrainingmodule.init_net_opt',
                                                                                             'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.loss_fn': ( 'methods.prototype.html#aetrainingmodule.loss_fn',
+                                     'relax.methods.proto.AETrainingModule.loss_fn': ( 'methods/prototype.html#aetrainingmodule.loss_fn',
                                                                                        'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.training_step': ( 'methods.prototype.html#aetrainingmodule.training_step',
+                                     'relax.methods.proto.AETrainingModule.training_step': ( 'methods/prototype.html#aetrainingmodule.training_step',
                                                                                              'relax/methods/proto.py'),
-                                     'relax.methods.proto.AETrainingModule.validation_step': ( 'methods.prototype.html#aetrainingmodule.validation_step',
+                                     'relax.methods.proto.AETrainingModule.validation_step': ( 'methods/prototype.html#aetrainingmodule.validation_step',
                                                                                                'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF': ('methods.prototype.html#protocf', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.__init__': ( 'methods.prototype.html#protocf.__init__',
+                                     'relax.methods.proto.ProtoCF': ('methods/prototype.html#protocf', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.ProtoCF.__init__': ( 'methods/prototype.html#protocf.__init__',
                                                                                'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF._is_module_trained': ( 'methods.prototype.html#protocf._is_module_trained',
+                                     'relax.methods.proto.ProtoCF._is_module_trained': ( 'methods/prototype.html#protocf._is_module_trained',
                                                                                          'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.generate_cf': ( 'methods.prototype.html#protocf.generate_cf',
+                                     'relax.methods.proto.ProtoCF.generate_cf': ( 'methods/prototype.html#protocf.generate_cf',
                                                                                   'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.generate_cfs': ( 'methods.prototype.html#protocf.generate_cfs',
+                                     'relax.methods.proto.ProtoCF.generate_cfs': ( 'methods/prototype.html#protocf.generate_cfs',
                                                                                    'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.train': ( 'methods.prototype.html#protocf.train',
+                                     'relax.methods.proto.ProtoCF.train': ( 'methods/prototype.html#protocf.train',
                                                                             'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCFConfig': ( 'methods.prototype.html#protocfconfig',
+                                     'relax.methods.proto.ProtoCFConfig': ( 'methods/prototype.html#protocfconfig',
                                                                             'relax/methods/proto.py'),
-                                     'relax.methods.proto._proto_cf': ('methods.prototype.html#_proto_cf', 'relax/methods/proto.py')},
-            'relax.methods.sphere': { 'relax.methods.sphere.GSConfig': ('sphere.html#gsconfig', 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere': ('sphere.html#growingsphere', 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.__init__': ( 'sphere.html#growingsphere.__init__',
+                                     'relax.methods.proto._proto_cf': ('methods/prototype.html#_proto_cf', 'relax/methods/proto.py')},
+            'relax.methods.sphere': { 'relax.methods.sphere.GSConfig': ('methods/sphere.html#gsconfig', 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere': ( 'methods/sphere.html#growingsphere',
+                                                                              'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.__init__': ( 'methods/sphere.html#growingsphere.__init__',
                                                                                        'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.generate_cf': ( 'sphere.html#growingsphere.generate_cf',
+                                      'relax.methods.sphere.GrowingSphere.generate_cf': ( 'methods/sphere.html#growingsphere.generate_cf',
                                                                                           'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.generate_cfs': ( 'sphere.html#growingsphere.generate_cfs',
+                                      'relax.methods.sphere.GrowingSphere.generate_cfs': ( 'methods/sphere.html#growingsphere.generate_cfs',
                                                                                            'relax/methods/sphere.py'),
-                                      'relax.methods.sphere._growing_spheres': ('sphere.html#_growing_spheres', 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.apply_immutable': ('sphere.html#apply_immutable', 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.cat_sample': ('sphere.html#cat_sample', 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.hyper_sphere_coordindates': ( 'sphere.html#hyper_sphere_coordindates',
+                                      'relax.methods.sphere._growing_spheres': ( 'methods/sphere.html#_growing_spheres',
+                                                                                 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.apply_immutable': ( 'methods/sphere.html#apply_immutable',
+                                                                                'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.cat_sample': ('methods/sphere.html#cat_sample', 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.hyper_sphere_coordindates': ( 'methods/sphere.html#hyper_sphere_coordindates',
                                                                                           'relax/methods/sphere.py')},
-            'relax.methods.vanilla': { 'relax.methods.vanilla.VanillaCF': ('methods.vanilla.html#vanillacf', 'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.__init__': ( 'methods.vanilla.html#vanillacf.__init__',
+            'relax.methods.vaecf': { 'relax.methods.vaecf.Decoder': ('methods/vaecf.html#decoder', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.Decoder.__call__': ( 'methods/vaecf.html#decoder.__call__',
+                                                                               'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.Decoder.__init__': ( 'methods/vaecf.html#decoder.__init__',
+                                                                               'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.Encoder': ('methods/vaecf.html#encoder', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.Encoder.__call__': ( 'methods/vaecf.html#encoder.__call__',
+                                                                               'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.Encoder.__init__': ( 'methods/vaecf.html#encoder.__init__',
+                                                                               'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF': ('methods/vaecf.html#vaecf', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.__init__': ('methods/vaecf.html#vaecf.__init__', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF._is_module_trained': ( 'methods/vaecf.html#vaecf._is_module_trained',
+                                                                                       'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.generate_cfs': ( 'methods/vaecf.html#vaecf.generate_cfs',
+                                                                                 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.train': ('methods/vaecf.html#vaecf.train', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFConfigs': ('methods/vaecf.html#vaecfconfigs', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule': ('methods/vaecf.html#vaecfmodule', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.__init__': ( 'methods/vaecf.html#vaecfmodule.__init__',
+                                                                                   'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule._training_step': ( 'methods/vaecf.html#vaecfmodule._training_step',
+                                                                                         'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.compute_loss': ( 'methods/vaecf.html#vaecfmodule.compute_loss',
+                                                                                       'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.decode': ( 'methods/vaecf.html#vaecfmodule.decode',
+                                                                                 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.encode': ( 'methods/vaecf.html#vaecfmodule.encode',
+                                                                                 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.init_net_opt': ( 'methods/vaecf.html#vaecfmodule.init_net_opt',
+                                                                                       'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.sample': ( 'methods/vaecf.html#vaecfmodule.sample',
+                                                                                 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.sample_latent_code': ( 'methods/vaecf.html#vaecfmodule.sample_latent_code',
+                                                                                             'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.sample_step': ( 'methods/vaecf.html#vaecfmodule.sample_step',
+                                                                                      'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.training_step': ( 'methods/vaecf.html#vaecfmodule.training_step',
+                                                                                        'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModule.validation_step': ( 'methods/vaecf.html#vaecfmodule.validation_step',
+                                                                                          'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFModuleConfigs': ( 'methods/vaecf.html#vaecfmoduleconfigs',
+                                                                                 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.hindge_embedding_loss': ( 'methods/vaecf.html#hindge_embedding_loss',
+                                                                                    'relax/methods/vaecf.py')},
+            'relax.methods.vanilla': { 'relax.methods.vanilla.VanillaCF': ('methods/vanilla.html#vanillacf', 'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla.VanillaCF.__init__': ( 'methods/vanilla.html#vanillacf.__init__',
                                                                                      'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.generate_cf': ( 'methods.vanilla.html#vanillacf.generate_cf',
+                                       'relax.methods.vanilla.VanillaCF.generate_cf': ( 'methods/vanilla.html#vanillacf.generate_cf',
                                                                                         'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.generate_cfs': ( 'methods.vanilla.html#vanillacf.generate_cfs',
+                                       'relax.methods.vanilla.VanillaCF.generate_cfs': ( 'methods/vanilla.html#vanillacf.generate_cfs',
                                                                                          'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCFConfig': ( 'methods.vanilla.html#vanillacfconfig',
+                                       'relax.methods.vanilla.VanillaCFConfig': ( 'methods/vanilla.html#vanillacfconfig',
                                                                                   'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla._vanilla_cf': ( 'methods.vanilla.html#_vanilla_cf',
+                                       'relax.methods.vanilla._vanilla_cf': ( 'methods/vanilla.html#_vanilla_cf',
                                                                               'relax/methods/vanilla.py')},
             'relax.module': { 'relax.module.BaseNetwork': ('training_module.html#basenetwork', 'relax/module.py'),
                               'relax.module.BaseNetwork.__call__': ('training_module.html#basenetwork.__call__', 'relax/module.py'),
                               'relax.module.BaseTrainingModule': ('training_module.html#basetrainingmodule', 'relax/module.py'),
                               'relax.module.BaseTrainingModule.init_logger': ( 'training_module.html#basetrainingmodule.init_logger',
                                                                                'relax/module.py'),
                               'relax.module.BaseTrainingModule.init_net_opt': ( 'training_module.html#basetrainingmodule.init_net_opt',
@@ -464,14 +602,16 @@
                                                                                         'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.forward': ( 'training_module.html#predictivetrainingmodule.forward',
                                                                                  'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.init_net_opt': ( 'training_module.html#predictivetrainingmodule.init_net_opt',
                                                                                       'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.loss_fn': ( 'training_module.html#predictivetrainingmodule.loss_fn',
                                                                                  'relax/module.py'),
+                              'relax.module.PredictiveTrainingModule.pred_fn': ( 'training_module.html#predictivetrainingmodule.pred_fn',
+                                                                                 'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.training_step': ( 'training_module.html#predictivetrainingmodule.training_step',
                                                                                        'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.validation_step': ( 'training_module.html#predictivetrainingmodule.validation_step',
                                                                                          'relax/module.py'),
                               'relax.module.PredictiveTrainingModuleConfigs': ( 'training_module.html#predictivetrainingmoduleconfigs',
                                                                                 'relax/module.py')},
             'relax.plots': { 'relax.plots._barplot': ('plotting.html#_barplot', 'relax/plots.py'),
```

### Comparing `jax-relax-0.1.2/relax/data/loader.py` & `jax-relax-0.1.3/relax/data/loader.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/data/module.py` & `jax-relax-0.1.3/relax/data/module.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/data/scm.py` & `jax-relax-0.1.3/relax/data/scm.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/docs.py` & `jax-relax-0.1.3/relax/docs.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/evaluate.py` & `jax-relax-0.1.3/relax/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,20 +61,21 @@
 ):
     cf_module.hook_data_module(datamodule)
     return cf_module
 
 def _train_parametric_module(
     cf_module: BaseParametricCFModule,
     datamodule: TabularDataModule,
-    t_configs=None
+    t_configs=None,
+    pred_fn=None
 ):
     if not cf_module._is_module_trained():
         print(f'{type(cf_module).__name__} contains parametric models. '
             'Starts training before generating explanations...')
-        cf_module.train(datamodule, t_configs)
+        cf_module.train(datamodule, t_configs, pred_fn=pred_fn)
     return cf_module
 
 # %% ../nbs/06_evaluate.ipynb 9
 def _check_aux_pred_fn_args(pred_fn_args: dict | None):
     if pred_fn_args is None:
         return dict()
     elif isinstance(pred_fn_args, dict):
@@ -123,15 +124,15 @@
     """Generate CF explanations."""
 
     _validate_configs(cf_module, datamodule, pred_fn, t_configs)
     cf_module = _prepare_module(cf_module, datamodule)
 
     if isinstance(cf_module, BaseParametricCFModule):
         cf_module = _train_parametric_module(
-            cf_module, datamodule, t_configs=t_configs
+            cf_module, datamodule, t_configs=t_configs, pred_fn=pred_fn
         )
     X, _ = datamodule.test_dataset[:]
     
     # create `pred_fn` which only takes `x` as an input
     if pred_fn is not None:
         pred_fn = _AuxPredFn(pred_fn, pred_fn_args=pred_fn_args)
 
@@ -176,120 +177,128 @@
     label: jnp.DeviceArray, # label dim: [N] or [N, 1]
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
 ) -> float:
     y_pred = pred_fn(input).reshape(-1, 1).round()
     label = label.reshape(-1, 1)
     return accuracy(y_pred, label).item()
 
-# %% ../nbs/06_evaluate.ipynb 20
+# %% ../nbs/06_evaluate.ipynb 21
 class PredictiveAccuracy(BaseEvalMetrics):
     """Compute the accuracy of the predict function."""
     
     def __init__(self, name: str = "accuracy"):
         super().__init__(name=name)
 
     def __call__(self, cf_explanations: Explanation) -> float:
         X, y = cf_explanations.data_module.test_dataset[:]
         return _compute_acc(X, y, cf_explanations.pred_fn)
 
-# %% ../nbs/06_evaluate.ipynb 22
+# %% ../nbs/06_evaluate.ipynb 23
 def _compute_val(
     input: jnp.DeviceArray, # input dim: [N, k]
     cfs: jnp.DeviceArray, # cfs dim: [N, k]
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
 ):
     y_pred = pred_fn(input).reshape(-1, 1).round()
     y_prime = jnp.ones_like(y_pred) - y_pred
     cf_y = pred_fn(cfs).reshape(-1, 1).round()
     return accuracy(y_prime, cf_y).item()
 
-# %% ../nbs/06_evaluate.ipynb 23
+# %% ../nbs/06_evaluate.ipynb 25
 class Validity(BaseEvalMetrics):
     """Compute fraction of input instances on which CF explanation methods output valid CF examples."""
     
     def __init__(self, name: str = "validity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_val(
             X, cf_explanations.cfs, cf_explanations.pred_fn
         )
 
-# %% ../nbs/06_evaluate.ipynb 24
+# %% ../nbs/06_evaluate.ipynb 26
+def _compute_proximity(
+    inputs: jnp.DeviceArray, # input dim: [N, k]
+    cfs: jnp.DeviceArray, # cfs dim: [N, k]
+):
+    prox = jnp.linalg.norm(inputs - cfs, ord=1, axis=1).mean()
+    return prox.item()
+
+# %% ../nbs/06_evaluate.ipynb 28
 class Proximity(BaseEvalMetrics):
     """Compute L1 norm distance between input datasets and CF examples divided by the number of features."""
     def __init__(self, name: str = "proximity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
-        return proximity(X, cf_explanations.cfs).item()
+        return _compute_proximity(X, cf_explanations.cfs)
 
-# %% ../nbs/06_evaluate.ipynb 25
+# %% ../nbs/06_evaluate.ipynb 29
 def _compute_spar(
     input: jnp.DeviceArray,
     cfs: jnp.DeviceArray,
     cat_idx: int
 ):
     # calculate sparsity
     cat_sparsity = proximity(input[:, cat_idx:], cfs[:, cat_idx:]) / 2
     cont_sparsity = jnp.linalg.norm(
         jnp.abs(input[:, :cat_idx] - cfs[:, :cat_idx]), ord=0, axis=1
     ).mean()
     return (cont_sparsity + cat_sparsity).item()
 
 
-# %% ../nbs/06_evaluate.ipynb 26
+# %% ../nbs/06_evaluate.ipynb 30
 class Sparsity(BaseEvalMetrics):
     """Compute the number of feature changes between input datasets and CF examples."""
 
     def __init__(self, name: str = "sparsity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_spar(X, cf_explanations.cfs, cf_explanations.cat_idx)
 
-# %% ../nbs/06_evaluate.ipynb 27
+# %% ../nbs/06_evaluate.ipynb 31
 def _compute_manifold_dist(
     input: jnp.DeviceArray,
     cfs: jnp.DeviceArray,
     n_neighbors: int = 1,
     p: int = 2
 ):
     knn = NearestNeighbors(n_neighbors=n_neighbors, p=p)
     knn.fit(input)
     nearest_dist, nearest_points = knn.kneighbors(cfs, 1, return_distance=True)
     return jnp.mean(nearest_dist).item()
 
-# %% ../nbs/06_evaluate.ipynb 28
+# %% ../nbs/06_evaluate.ipynb 32
 class ManifoldDist(BaseEvalMetrics):
     """Compute the L1 distance to the n-nearest neighbor for all CF examples."""
     def __init__(self, n_neighbors: int = 1, p: int = 2, name: str = "manifold_dist"):
         super().__init__(name=name)
         self.n_neighbors = n_neighbors
         self.p = p
         
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_manifold_dist(
             X, cf_explanations.cfs, self.n_neighbors, self.p
         )
 
-# %% ../nbs/06_evaluate.ipynb 29
+# %% ../nbs/06_evaluate.ipynb 33
 class Runtime(BaseEvalMetrics):
     """Get the running time to generate CF examples."""
     def __init__(self, name: str = "runtime"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         return cf_explanations.total_time
 
-# %% ../nbs/06_evaluate.ipynb 31
+# %% ../nbs/06_evaluate.ipynb 35
 def _create_second_order_cfs(cf_results: CFExplanationResults, threshold: float = 2.0):
     X, y = cf_results.data_module.test_dataset[:]
     cfs = cf_results.cfs
     scaler = cf_results.data_module.normalizer
     cat_idx = cf_results.data_module.cat_idx
 
     # get normalized threshold = threshold / (max - min)
@@ -328,15 +337,15 @@
     cfs_hat = _create_second_order_cfs(cf_results, threshold)
     cf_results_so = deepcopy(cf_results)
     cf_results_so.cfs = cfs_hat
     compute_sparsity = Sparsity()
     return compute_sparsity(cf_results_so)
 
 
-# %% ../nbs/06_evaluate.ipynb 33
+# %% ../nbs/06_evaluate.ipynb 37
 def fake_explanations():
     """Generate sudo explanations for testing."""
     from relax.data import load_data
 
     dm = load_data("adult")
     X, y = dm.test_dataset[:]
     cfs = X
@@ -344,15 +353,15 @@
     pred_fn = lambda x: jax.random.bernoulli(jax.random.PRNGKey(0), 0.5, (x.shape[0], 1)).astype(float)
     assert y.shape == pred_fn(X).shape
     return Explanation(
         cf_name='sudo', data_module=dm, cfs=cfs, pred_fn=pred_fn, total_time=0.0, dataset_name=dn
     )
 
 
-# %% ../nbs/06_evaluate.ipynb 34
+# %% ../nbs/06_evaluate.ipynb 38
 # METRICS = dict(
 #     acc=PredictiveAccuracy(),
 #     accuracy=PredictiveAccuracy(),
 #     validity=Validity(),
 #     proximity=Proximity(),
 #     runtime=Runtime(),
 #     manifold_dist=ManifoldDist(),
@@ -370,15 +379,15 @@
     ManifoldDist(),
 ]
 
 METRICS = { m.name: m for m in METRICS_CALLABLE }
 
 DEFAULT_METRICS = ["acc", "validity", "proximity"]
 
-# %% ../nbs/06_evaluate.ipynb 36
+# %% ../nbs/06_evaluate.ipynb 40
 def _get_metric(metric: str | BaseEvalMetrics, cf_exp: Explanation):
     if isinstance(metric, str):
         if metric not in METRICS.keys():
             raise ValueError(f"'{metric}' is not supported. Must be one of {METRICS.keys()}")
         res = METRICS[metric](cf_exp)
     elif callable(metric):
         # f(cf_exp) not supported for now
@@ -388,15 +397,15 @@
     else:
         raise ValueError(f"{type(metric).__name__} is not supported as a metric.")
     
     if isinstance(res, jnp.ndarray) and res.shape == (1,):
         res = res.item()
     return res
 
-# %% ../nbs/06_evaluate.ipynb 38
+# %% ../nbs/06_evaluate.ipynb 42
 def evaluate_cfs(
     cf_exp: Explanation, # CF Explanations
     metrics: Iterable[Union[str, BaseEvalMetrics]] = None, # A list of Metrics. Can be `str` or a subclass of `BaseEvalMetrics`
     return_dict: bool = True, # return a dictionary or not (default: True)
     return_df: bool = False # return a pandas Dataframe or not (default: False)
 ):
     cf_name = cf_exp.cf_name
@@ -412,15 +421,15 @@
     result_df = pd.DataFrame.from_dict(result_dict, orient="index")
     
     if return_dict and return_df:
         return (result_dict, result_df)
     elif return_dict or return_df:
         return result_df if return_df else result_dict
 
-# %% ../nbs/06_evaluate.ipynb 40
+# %% ../nbs/06_evaluate.ipynb 44
 def benchmark_cfs(
     cf_results_list: Iterable[CFExplanationResults],
     metrics: Optional[Iterable[str]] = None,
 ):
     dfs = [
         evaluate_cfs(
             cf_exp=cf_results, metrics=metrics, return_dict=False, return_df=True
```

### Comparing `jax-relax-0.1.2/relax/logger.py` & `jax-relax-0.1.3/relax/logger.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/methods/base.py` & `jax-relax-0.1.3/relax/methods/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
 # %% ../../nbs/05_methods.base.ipynb 9
 class BaseParametricCFModule(ABC):
     @abstractmethod
     def train(
         self, 
         datamodule: TabularDataModule, # data module
-        t_configs: TrainingConfigs | dict = None # training configs; see docs in `TrainingConfigs`
+        t_configs: TrainingConfigs | dict = None, # training configs; see docs in `TrainingConfigs`
+        pred_fn: Callable = None # predictive function
     ): 
         pass
 
     @abstractmethod
     def _is_module_trained(self) -> bool: pass
 
 # %% ../../nbs/05_methods.base.ipynb 11
```

### Comparing `jax-relax-0.1.2/relax/methods/counternet.py` & `jax-relax-0.1.3/relax/methods/counternet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05d_methods.counternet.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/methods/04_counternet.ipynb.
 
-# %% ../../nbs/05d_methods.counternet.ipynb 3
+# %% ../../nbs/methods/04_counternet.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from ..module import MLP, BaseTrainingModule
 from .base import BaseCFModule, BaseParametricCFModule, BasePredFnCFModule
 from ..trainer import TrainingConfigs, train_model
 from ..data import TabularDataModule
 from ..utils import validate_configs, sigmoid, accuracy, proximity, make_model, init_net_opt, grad_update
 from functools import partial
 
 # %% auto 0
 __all__ = ['CounterNetModel', 'partition_trainable_params', 'project_immutable_features', 'CounterNetTrainingModuleConfigs',
            'CounterNetTrainingModule', 'CounterNetConfigs', 'CounterNet']
 
-# %% ../../nbs/05d_methods.counternet.ipynb 5
+# %% ../../nbs/methods/04_counternet.ipynb 5
 class CounterNetModelConfigs(BaseParser):
     """Configurator of `CounterNetModel`."""
 
     enc_sizes: List[int] = Field(description='Encoder sizes.')
     dec_sizes: List[int] = Field(description='Predictor sizes.')
     exp_sizes: List[int] = Field(description='CF generator sizes.')
     dropout_rate: float = Field(0.3, description='Dropout rate.')
 
-# %% ../../nbs/05d_methods.counternet.ipynb 6
+# %% ../../nbs/methods/04_counternet.ipynb 6
 class CounterNetModel(hk.Module):
     """CounterNet Model"""
     def __init__(
         self,
         m_config: Dict | CounterNetModelConfigs,  # Model configs which contain configs in `CounterNetModelConfigs`.
         name: str = None,  # Name of the module.
     ):
@@ -54,36 +54,36 @@
         cf = MLP(self.configs.exp_sizes, self.configs.dropout_rate, name="Explainer")(
             z_exp, is_training
         )
         cf = hk.Linear(input_shape, name="Explainer")(cf)
         return y_hat, cf
 
 
-# %% ../../nbs/05d_methods.counternet.ipynb 8
+# %% ../../nbs/methods/04_counternet.ipynb 8
 def partition_trainable_params(params: hk.Params, trainable_name: str):
     trainable_params, non_trainable_params = hk.data_structures.partition(
         lambda m, n, p: trainable_name in m, params
     )
     return trainable_params, non_trainable_params
 
 
-# %% ../../nbs/05d_methods.counternet.ipynb 9
+# %% ../../nbs/methods/04_counternet.ipynb 9
 def project_immutable_features(x, cf: jnp.DeviceArray, imutable_idx_list: List[int]):
     cf = cf.at[:, imutable_idx_list].set(x[:, imutable_idx_list])
     return cf
 
-# %% ../../nbs/05d_methods.counternet.ipynb 10
+# %% ../../nbs/methods/04_counternet.ipynb 10
 class CounterNetTrainingModuleConfigs(BaseParser):
     lr: float = 0.003
     lambda_1: float = 1.0
     lambda_2: float = 0.2
     lambda_3: float = 0.1
 
 
-# %% ../../nbs/05d_methods.counternet.ipynb 11
+# %% ../../nbs/methods/04_counternet.ipynb 11
 class CounterNetTrainingModule(BaseTrainingModule):
     _data_module: TabularDataModule
 
     def __init__(self, m_configs: Dict[str, Any]):
         self.save_hyperparameters(m_configs)
         self.net = make_model(m_configs, CounterNetModel)
         self.configs = validate_configs(m_configs, CounterNetTrainingModuleConfigs)
@@ -112,38 +112,44 @@
         y_pred, cf = self.net.apply(params, rng_key, x, is_training=is_training)
         cf = self._data_module.apply_constraints(x, cf, hard=not is_training)
 
         # second forward to calulate cf_y
         cf_y, _ = self.net.apply(params, rng_key, cf, is_training=is_training)
         return y_pred, cf, cf_y
 
+    @partial(jax.jit, static_argnames=["self"])
     def predict(self, params, rng_key, x):
         y_pred, _ = self.net.apply(params, rng_key, x, is_training=False)
         return y_pred
 
-    def generate_cfs(self, X: chex.ArrayBatched, params, rng_key) -> chex.ArrayBatched:
+    def generate_cfs(self, X: Array, params, rng_key) -> chex.ArrayBatched:
         y_pred, cfs = self.net.apply(params, rng_key, X, is_training=False)
         # cfs = cfs + X
         cfs = self._data_module.apply_constraints(X, cfs, hard=True)
         return cfs
 
+    @partial(jax.jit, static_argnames=["self"])
     def loss_fn_1(self, y_pred, y):
         return jnp.mean(vmap(optax.l2_loss)(y_pred, y))
 
+    @partial(jax.jit, static_argnames=["self"])
     def loss_fn_2(self, cf_y, y_prime):
         return jnp.mean(vmap(optax.l2_loss)(cf_y, y_prime))
 
+    @partial(jax.jit, static_argnames=["self"])
     def loss_fn_3(self, x, cf):
         return jnp.mean(vmap(optax.l2_loss)(x, cf))
 
+    @partial(jax.jit, static_argnames=["self", "is_training"])
     def pred_loss_fn(self, params, rng_key, batch, is_training: bool = True):
         x, y = batch
         y_pred, cf = self.net.apply(params, rng_key, x, is_training=is_training)
         return self.configs.lambda_1 * self.loss_fn_1(y_pred, y)
 
+    @partial(jax.jit, static_argnames=["self", "is_training"])
     def exp_loss_fn(
         self,
         trainable_params,
         non_trainable_params,
         rng_key,
         batch,
         is_training: bool = True,
@@ -152,19 +158,21 @@
         params = hk.data_structures.merge(trainable_params, non_trainable_params)
         x, y = batch
         y_pred, cf, cf_y = self.forward(params, rng_key, x, is_training=is_training)
         y_prime = 1 - jnp.round(y_pred)
         loss_2, loss_3 = self.loss_fn_2(cf_y, y_prime), self.loss_fn_3(x, cf)
         return self.configs.lambda_2 * loss_2 + self.configs.lambda_3 * loss_3
 
+    @partial(jax.jit, static_argnames=["self",])
     def _predictor_step(self, params, opt_state, rng_key, batch):
         grads = jax.grad(self.pred_loss_fn)(params, rng_key, batch)
         upt_params, opt_state = grad_update(grads, params, opt_state, self.opt_1)
         return upt_params, opt_state
 
+    @partial(jax.jit, static_argnames=["self",])
     def _explainer_step(self, params, opt_state, rng_key, batch):
         trainable_params, non_trainable_params = partition_trainable_params(
             params, trainable_name="counter_net_model/Explainer"
         )
         grads = jax.grad(self.exp_loss_fn)(
             trainable_params, non_trainable_params, rng_key, batch
         )
@@ -242,15 +250,15 @@
             "val/val_loss_2": loss_2,
             "val/val_loss_3": loss_3,
             "val/val_loss": loss_1 + loss_2 + loss_3,
         }
         self.log_dict(logs)
         return logs
 
-# %% ../../nbs/05d_methods.counternet.ipynb 16
+# %% ../../nbs/methods/04_counternet.ipynb 16
 class CounterNetConfigs(CounterNetTrainingModuleConfigs, CounterNetModelConfigs):
     """Configurator of `CounterNet`."""
 
     enc_sizes: List[int] = Field(
         [50,10], description="Sequence of layer sizes for encoder network."
     )
     dec_sizes: List[int] = Field(
@@ -273,15 +281,15 @@
         0.2, description=" $\lambda_2$ for balancing the prediction loss $\mathcal{L}_2$."
     ) 
     lambda_3: float = Field(
         0.1, description=" $\lambda_3$ for balancing the prediction loss $\mathcal{L}_3$."
     )
 
 
-# %% ../../nbs/05d_methods.counternet.ipynb 17
+# %% ../../nbs/methods/04_counternet.ipynb 17
 class CounterNet(BaseCFModule, BaseParametricCFModule, BasePredFnCFModule):
     """API for CounterNet Explanation Module."""
     params: hk.Params = None
     module: CounterNetTrainingModule
     name: str = 'CounterNet'
 
     def __init__(
@@ -294,15 +302,16 @@
 
     def _is_module_trained(self):
         return not (self.params is None)
     
     def train(
         self, 
         datamodule: TabularDataModule, # data module
-        t_configs: TrainingConfigs | dict = None # training configs
+        t_configs: TrainingConfigs | dict = None, # training configs
+        *args, **kwargs
     ):
         _default_t_configs = dict(
             n_epochs=100, batch_size=128
         )
         if t_configs is None: t_configs = _default_t_configs
         params, _ = train_model(self.module, datamodule, t_configs)
         self.params = params
```

### Comparing `jax-relax-0.1.2/relax/methods/diverse.py` & `jax-relax-0.1.3/relax/methods/diverse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05b_methods.diverse.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/methods/02_diverse.ipynb.
 
 # %% auto 0
 __all__ = ['DiverseCFConfig', 'DiverseCF']
 
-# %% ../../nbs/05b_methods.diverse.ipynb 3
+# %% ../../nbs/methods/02_diverse.ipynb 3
 from ..import_essentials import *
 from .base import BaseCFModule
 from ..utils import validate_configs, dist, grad_update
 
-# %% ../../nbs/05b_methods.diverse.ipynb 4
+# %% ../../nbs/methods/02_diverse.ipynb 4
 def hinge_loss(input: jnp.DeviceArray, target: jnp.DeviceArray):
     """
     reference:
     - https://github.com/interpretml/DiCE/blob/a772c8d4fcd88d1cab7f2e02b0bcc045dc0e2eab/dice_ml/explainer_interfaces/dice_pytorch.py#L196-L202
     - https://en.wikipedia.org/wiki/Hinge_loss
     """
     input = jnp.log((jnp.abs(input - 1e-6) / (1 - jnp.abs(input - 1e-6))))
     all_ones = jnp.ones_like(target)
     target = 2 * target - all_ones
     loss = all_ones - target * input
     loss = jax.nn.relu(loss)
     return jnp.linalg.norm(loss)
 
 
-# %% ../../nbs/05b_methods.diverse.ipynb 5
+# %% ../../nbs/methods/02_diverse.ipynb 5
 def l1_mean(X, cfs):
     x_mean = jnp.mean(jnp.abs(X))
     l1_loss = jnp.mean(jnp.abs(X - cfs))
     return l1_loss / x_mean
 
 
-# %% ../../nbs/05b_methods.diverse.ipynb 6
+# %% ../../nbs/methods/02_diverse.ipynb 6
 def dpp_style(cf: jnp.DeviceArray, n_cfs: int):
     det_entries = jnp.ones((n_cfs, n_cfs))
     for i in range(n_cfs):
         for j in range(n_cfs):
             det_entries.at[i, j].set(dist(cf[i], cf[j], ord=1))
 
     det_entries = 1.0 / (1.0 + det_entries)
     det_entries += jnp.eye(n_cfs) * 0.0001
     return jnp.linalg.det(det_entries)
 
 
-# %% ../../nbs/05b_methods.diverse.ipynb 7
+# %% ../../nbs/methods/02_diverse.ipynb 7
 def _compute_regularization_loss(cfs, cat_idx, cat_arrays, n_cfs):
     # cat_idx = len(self.model.continous_cols)
     regularization_loss = 0.0
     for i in range(n_cfs):
         for col in cat_arrays:
             cat_idx_end = cat_idx + len(col)
             regularization_loss += jnp.power(
                 (jnp.sum(cfs[i][cat_idx:cat_idx_end]) - 1.0), 2
             )
     return regularization_loss
 
 
-# %% ../../nbs/05b_methods.diverse.ipynb 8
+# %% ../../nbs/methods/02_diverse.ipynb 8
 def _diverse_cf(
     x: jnp.DeviceArray,  # `x` shape: (k,), where `k` is the number of features
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray],  # y = pred_fn(x)
     n_cfs: int,
     n_steps: int,
     lr: float,  # learning rate for each `cf` optimization step
     lambda_: float,  #  loss = validity_loss + lambda_params * cost
@@ -119,28 +119,28 @@
     opt_state = opt.init(cfs)
     for _ in tqdm(range(n_steps)):
         cfs, opt_state = gen_cf_step(x, cfs, opt_state)
     cf = projection_fn(x, cfs[:1, :], hard=True)
     return cf.reshape(x_size)
 
 
-# %% ../../nbs/05b_methods.diverse.ipynb 9
+# %% ../../nbs/methods/02_diverse.ipynb 9
 class DiverseCFConfig(BaseParser):
     n_cfs: int = 5
     n_steps: int = 1000
     lr: float = 0.01
     lambda_: float = 0.01  # loss = validity_loss + lambda_params * cost
     seed: int = 42
 
     @property
     def keys(self):
         return hk.PRNGSequence(self.seed)
 
 
-# %% ../../nbs/05b_methods.diverse.ipynb 10
+# %% ../../nbs/methods/02_diverse.ipynb 10
 class DiverseCF(BaseCFModule):
     name = "DiverseCF"
 
     def __init__(
         self,
         configs: Union[Dict[str, Any], DiverseCFConfig] = None,
     ):
```

### Comparing `jax-relax-0.1.2/relax/methods/proto.py` & `jax-relax-0.1.3/relax/methods/proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05c_methods.prototype.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/methods/03_prototype.ipynb.
 
-# %% ../../nbs/05c_methods.prototype.ipynb 3
+# %% ../../nbs/methods/03_prototype.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from .base import BaseCFModule, BaseParametricCFModule
 from ..data import TabularDataModule
 from ..module import BaseTrainingModule, MLP
 from ..trainer import train_model, TrainingConfigs
 from ..utils import validate_configs, binary_cross_entropy, make_model, init_net_opt, grad_update
 from functools import partial
 
 # %% auto 0
 __all__ = ['ProtoCFConfig', 'ProtoCF']
 
-# %% ../../nbs/05c_methods.prototype.ipynb 4
+# %% ../../nbs/methods/03_prototype.ipynb 4
 class AEConfigs(BaseParser):
     enc_sizes: List[int]
     dec_sizes: List[int]
     dropout_rate: float = 0.3
     lr: float = 0.001
 
 class AE(hk.Module):
@@ -36,15 +36,15 @@
     ) -> jnp.ndarray:
         input_shape = x.shape[-1]
         z = MLP(sizes=self.configs.enc_sizes, dropout_rate=self.configs.dropout_rate, name='Encoder')(x, is_training)
         x = MLP(sizes=self.configs.enc_sizes, dropout_rate=self.configs.dropout_rate, name='Decoder')(z, is_training)
         x = hk.Linear(input_shape, name='Decoder')(x)
         return x, z
 
-# %% ../../nbs/05c_methods.prototype.ipynb 5
+# %% ../../nbs/methods/03_prototype.ipynb 5
 class AETrainingModule(BaseTrainingModule):
     def __init__(
         self,
         m_configs: Dict[str, Any]
     ):
         self.save_hyperparameters(m_configs)
         self.net = make_model(m_configs, AE)
@@ -96,15 +96,15 @@
         x, y = batch
         loss = self.loss_fn(params, rng_key, batch, is_training=False)
         logs = {
             'val/val_loss': loss.item(),
         }
         self.log_dict(logs)
 
-# %% ../../nbs/05c_methods.prototype.ipynb 6
+# %% ../../nbs/methods/03_prototype.ipynb 6
 def _proto_cf(
     x: jnp.DeviceArray, # `x` shape: (k,), where `k` is the number of features
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray], # y = pred_fn(x)
     n_steps: int,
     lr: float, # learning rate for each `cf` optimization step
     lambda_: float, #  loss = validity_loss + lambda_params * cost
     ae: AETrainingModule,
@@ -162,29 +162,29 @@
     opt_state = opt.init(cf)
     for _ in tqdm(range(n_steps)):
         cf, opt_state = gen_cf_step(x, cf, opt_state)
 
     cf = apply_constraints_fn(x, cf, hard=True)
     return cf.reshape(x_size)
 
-# %% ../../nbs/05c_methods.prototype.ipynb 7
+# %% ../../nbs/methods/03_prototype.ipynb 7
 class ProtoCFConfig(BaseParser):
     
     n_steps: int = 1000
     lr: float = 0.01
     lambda_: float = 0.01 # loss = validity_loss + lambda_params * cost
     ae_configs: Dict[str, Any] = {
         "enc_sizes": [50, 10],
         "dec_sizes": [10, 50],
         "dropout_rate": 0.3,
         'lr': 0.03,
     }
 
 
-# %% ../../nbs/05c_methods.prototype.ipynb 8
+# %% ../../nbs/methods/03_prototype.ipynb 8
 class ProtoCF(BaseCFModule, BaseParametricCFModule):
     name = "ProtoCF"
     _ae_params: hk.Params = None
     _ae_module: AETrainingModule
 
     def __init__(
         self, 
@@ -193,15 +193,16 @@
         if configs is None:
             configs = ProtoCFConfig()
         self.configs = validate_configs(configs, ProtoCFConfig)
 
     def train(
         self, 
         data_module: TabularDataModule, # data module
-        t_configs: TrainingConfigs | dict = None # training configs
+        t_configs: TrainingConfigs | dict = None, # training configs
+        *args, **kwargs
     ):
         _default_t_configs = dict(n_epochs=10, batch_size=128)
         if t_configs is None: 
             t_configs = _default_t_configs
         t_configs = validate_configs(t_configs, TrainingConfigs)
         # train autoencoder
         self._ae_module = AETrainingModule(self.configs.ae_configs)
```

### Comparing `jax-relax-0.1.2/relax/methods/sphere.py` & `jax-relax-0.1.3/relax/methods/sphere.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05e_sphere.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/methods/05_sphere.ipynb.
 
-# %% ../../nbs/05e_sphere.ipynb 3
+# %% ../../nbs/methods/05_sphere.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from .base import BaseCFModule
 from ..utils import *
 
 # %% auto 0
 __all__ = ['hyper_sphere_coordindates', 'cat_sample', 'apply_immutable', 'GSConfig', 'GrowingSphere']
 
-# %% ../../nbs/05e_sphere.ipynb 4
+# %% ../../nbs/methods/05_sphere.ipynb 4
 def hyper_sphere_coordindates(
     rng_key: jrand.PRNGKey, # Random number generator key
     x: Array, # Input instance with only continuous features. Shape: (1, n_features)
     n_samples: int, # Number of samples
     high: float, # Upper bound
     low: float, # Lower bound
     p_norm: int = 2 # Norm
@@ -26,15 +26,15 @@
     norm_p = jnp.linalg.norm(delta, ord=p_norm, axis=1)
     d_norm = jnp.divide(dist, norm_p).reshape(-1, 1)  # rescale/normalize factor
     delta = jnp.multiply(delta, d_norm)
     candidates = x + delta
 
     return candidates
 
-# %% ../../nbs/05e_sphere.ipynb 5
+# %% ../../nbs/methods/05_sphere.ipynb 5
 def cat_sample(
     rng_key: jrand.PRNGKey, # Random number generator key
     x: Array, # Input instance with only categorical features. Shape: (1, n_features)
     cat_arrays: List[List[str]],  # A list of a list of each categorical feature name
     n_samples: int,  # Number of samples to sample
 ): 
     def sample_categorical(rng_key: jrand.PRNGKey, col: np.ndarray):
@@ -49,15 +49,15 @@
     # We cannot use lax.scan here because cat_arrays is List[List[str]], not and can't ben an Array
     for col in cat_arrays:
         rng_key, cat_sample = sample_categorical(rng_key, col)
         candidates.append(cat_sample)
     candidates = jnp.concatenate(candidates, axis=1)
     return candidates
 
-# %% ../../nbs/05e_sphere.ipynb 6
+# %% ../../nbs/methods/05_sphere.ipynb 6
 def _growing_spheres(
     rng_key: jrand.PRNGKey, # Random number generator key
     x: Array, # Input instance. Shape: (n_features)
     pred_fn: Callable, # Prediction function
     n_steps: int, # Number of steps
     n_samples: int,  # Number of samples to sample
     cat_idx: int, # Index of categorical features
@@ -129,32 +129,32 @@
     y_pred = pred_fn(x).round().reshape(-1)
     candidate_cf = jnp.ones_like(x) * jnp.inf
     count = 0
     state = (candidate_cf, count, rng_key)
     candidate_cf, _, _ = lax.while_loop(cond_fn, body_fn, state)
     # if `inf` is found, return the original input
     candidate_cf = jnp.where(jnp.isinf(candidate_cf), x, candidate_cf)
-    return candidate_cf
+    return candidate_cf.reshape(x_size)
 
-# %% ../../nbs/05e_sphere.ipynb 7
+# %% ../../nbs/methods/05_sphere.ipynb 7
 def apply_immutable(x: Array, cf: Array, immutable_idx: List[int]):
     if immutable_idx is not None:
         cf = cf.at[:, immutable_idx].set(x[:, immutable_idx])
     return cf
 
-# %% ../../nbs/05e_sphere.ipynb 8
+# %% ../../nbs/methods/05_sphere.ipynb 8
 class GSConfig(BaseParser):
     seed: int = 42
-    n_steps: int = 10
+    n_steps: int = 100
     n_samples: int = 1000
     step_size: float = 0.05
     p_norm: int = 2
     
 
-# %% ../../nbs/05e_sphere.ipynb 9
+# %% ../../nbs/methods/05_sphere.ipynb 9
 class GrowingSphere(BaseCFModule):
     name = "Growing Sphere"
 
     def __init__(
         self,
         configs: Dict | GSConfig = None
     ):
```

### Comparing `jax-relax-0.1.2/relax/methods/vanilla.py` & `jax-relax-0.1.3/relax/methods/vanilla.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05a_methods.vanilla.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/methods/01_vanilla.ipynb.
 
-# %% ../../nbs/05a_methods.vanilla.ipynb 3
+# %% ../../nbs/methods/01_vanilla.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from .base import BaseCFModule
 from ..utils import validate_configs, binary_cross_entropy, grad_update
 
 # %% auto 0
 __all__ = ['VanillaCFConfig', 'VanillaCF']
 
-# %% ../../nbs/05a_methods.vanilla.ipynb 4
+# %% ../../nbs/methods/01_vanilla.ipynb 4
 def _vanilla_cf(
     x: jnp.DeviceArray,  # `x` shape: (k,), where `k` is the number of features
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray],  # y = pred_fn(x)
     n_steps: int,
     lr: float,  # learning rate for each `cf` optimization step
     lambda_: float,  #  loss = validity_loss + lambda_params * cost
     apply_fn: Callable
@@ -58,22 +58,22 @@
     for _ in tqdm(range(n_steps)):
         cf, opt_state = gen_cf_step(x, cf, opt_state)
 
     cf = apply_fn(x, cf, hard=False)
     return cf.reshape(x_size)
 
 
-# %% ../../nbs/05a_methods.vanilla.ipynb 5
+# %% ../../nbs/methods/01_vanilla.ipynb 5
 class VanillaCFConfig(BaseParser):
     n_steps: int = 1000
     lr: float = 0.001
     lambda_: float = 0.01  # loss = validity_loss + lambda_ * cost
 
 
-# %% ../../nbs/05a_methods.vanilla.ipynb 6
+# %% ../../nbs/methods/01_vanilla.ipynb 6
 class VanillaCF(BaseCFModule):
     name = "VanillaCF"
 
     def __init__(
         self,
         configs: dict | VanillaCFConfig = None
     ):
```

### Comparing `jax-relax-0.1.2/relax/module.py` & `jax-relax-0.1.3/relax/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,42 +170,44 @@
             dropout_rate=self.configs.dropout_rate
         )
         self.opt = optax.adam(learning_rate=self.configs.lr)
 
     @partial(jax.jit, static_argnames=["self", "is_training"])
     def forward(self, params, rng_key, x, is_training: bool = True):
         return self.net.apply(params, rng_key, x, is_training=is_training)
+    
+    def pred_fn(self, x, params, rng_key):
+        return self.forward(params, rng_key, x, is_training=False)
 
     def init_net_opt(self, data_module, key):
         X, _ = data_module.train_dataset[:100]
         params, opt_state = init_net_opt(
             self.net, self.opt, X=X, key=key
         )
         return params, opt_state
 
+    @partial(jax.jit, static_argnames=["self", "is_training"])
     def loss_fn(self, params, rng_key, batch, is_training: bool = True):
         x, y = batch
         y_pred = self.net.apply(params, rng_key, x, is_training=is_training)
         return jnp.mean(vmap(optax.l2_loss)(y_pred, y))
 
     # def _training_step(self, params, opt_state, rng_key, batch):
     #     grads = jax.grad(self.loss_fn)(params, rng_key, batch)
     #     upt_params, opt_state = grad_update(grads, params, opt_state, self.opt)
     #     return upt_params, opt_state
 
     @partial(jax.jit, static_argnames=["self"])
     def _training_step(self, params, opt_state, rng_key, batch):
-        grads = jax.grad(self.loss_fn)(params, rng_key, batch)
+        loss, grads = jax.value_and_grad(self.loss_fn)(params, rng_key, batch)
         upt_params, opt_state = grad_update(grads, params, opt_state, self.opt)
-        return upt_params, opt_state
+        return upt_params, opt_state, loss
 
     def training_step(self, params, opt_state, rng_key, batch):
-        params, opt_state = self._training_step(params, opt_state, rng_key, batch)
-
-        loss = self.loss_fn(params, rng_key, batch)
+        params, opt_state, loss = self._training_step(params, opt_state, rng_key, batch)
         self.log_dict({"train/train_loss_1": loss.item()})
         return params, opt_state
 
     def validation_step(self, params, rng_key, batch):
         x, y = batch
         y_pred = self.net.apply(params, rng_key, x, is_training=False)
         loss = self.loss_fn(params, rng_key, batch, is_training=False)
```

### Comparing `jax-relax-0.1.2/relax/plots.py` & `jax-relax-0.1.3/relax/plots.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.2/relax/trainer.py` & `jax-relax-0.1.3/relax/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # define logger
     logger = TensorboardLogger(
         log_dir=t_configs.log_dir,
         name=t_configs.logger_name,
         on_step=t_configs.log_on_step,
     )
     logger.save_hyperparams(t_configs.dict())
-    if training_module.hparams:
+    if hasattr(training_module, "hparams") and training_module.hparams is not None:
         logger.save_hyperparams(training_module.hparams)
 
     training_module.init_logger(logger)
     # define checkpoint manageer
     if t_configs.monitor_metrics is None:
         monitor_metrics = None
     else:
```

### Comparing `jax-relax-0.1.2/relax/utils.py` & `jax-relax-0.1.3/relax/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from .import_essentials import *
 import nbdev
 from fastcore.basics import AttrDict
 from nbdev.showdoc import BasicMarkdownRenderer
 from inspect import isclass
 
 # %% auto 0
-__all__ = ['validate_configs', 'show_doc', 'cat_normalize', 'make_model', 'make_hk_module', 'init_net_opt', 'grad_update',
-           'check_cat_info', 'load_json', 'binary_cross_entropy', 'sigmoid', 'accuracy', 'dist', 'proximity',
-           'get_config']
+__all__ = ['validate_configs', 'cat_normalize', 'make_model', 'make_hk_module', 'init_net_opt', 'grad_update', 'check_cat_info',
+           'load_json', 'binary_cross_entropy', 'sigmoid', 'accuracy', 'dist', 'proximity', 'get_config']
 
 # %% ../nbs/00_utils.ipynb 5
 def validate_configs(
     configs: dict | BaseParser,  # A configuration of the model/dataset.
     config_cls: BaseParser,  # The desired configuration class.
 ) -> BaseParser:
     """return a valid configuration object."""
```

### Comparing `jax-relax-0.1.2/settings.ini` & `jax-relax-0.1.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 user = birkhoffg
 description = Jax-based Recourse Explanation Library
 keywords = Jax, Recourse, Explanation, Interpretability, Machine Learning
 author = BirkhoffG
 author_email = 26811230+BirkhoffG@users.noreply.github.com
 copyright = Birkhoff Guo
 branch = master
-version = 0.1.2
+version = 0.1.3
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = true
 license = apache2
 status = 2
 requirements = matplotlib seaborn scikit-learn>=1.0.2,<1.4.0 pandas nbdev jupyter dm-haiku test_tube jax[cpu] tqdm optax pydantic>=1.9.0,<2 deprecation networkx
-dev_requirements = torch>=1.7.0 causalgraphicalmodels
+dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host = https://birkhoffg.github.io
 doc_baseurl = /ReLax/
 git_url = https://github.com/birkhoffg/relax/tree/master/
 lib_path = relax
```

### Comparing `jax-relax-0.1.2/setup.py` & `jax-relax-0.1.3/setup.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools
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
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
-
-requirements = cfg.get('requirements','').split()
-if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
-min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-dev_requirements = (cfg.get('dev_requirements') or '').split()
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
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
-    **setup_cfg)
-
-
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools
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
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
+
+requirements = cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
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
+    dependency_links = cfg.get('dep_links','').split(),
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = open('README.md').read(),
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
+    **setup_cfg)
+
+
```

