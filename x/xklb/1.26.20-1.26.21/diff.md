# Comparing `tmp/xklb-1.26.20.tar.gz` & `tmp/xklb-1.26.21.tar.gz`

## Comparing `xklb-1.26.20.tar` & `xklb-1.26.21.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.20/.gitattributes
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 xklb-1.26.20/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.20/Windows.md
--rw-r--r--   0        0        0   413285 2020-02-02 00:00:00.000000 xklb-1.26.20/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.20/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.20/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.20/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.20/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 xklb-1.26.20/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/__init__.py
--rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/av.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/books.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/consts.py
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/dl_config.py
--rw-r--r--   0        0        0    14860 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/dl_extract.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/fs_extract.py
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/gui.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/hn_extract.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/lb.py
--rw-r--r--   0        0        0    35724 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/play_actions.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/playback.py
--rw-r--r--   0        0        0    26699 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/player.py
--rw-r--r--   0        0        0    14748 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/stats.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21740 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/tube_backend.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/tube_extract.py
--rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.20/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.20/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.20/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.20/LICENSE
--rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.20/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 xklb-1.26.20/pyproject.toml
--rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.20/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.21/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.21/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.21/Windows.md
+-rw-r--r--   0        0        0   420713 2020-02-02 00:00:00.000000 xklb-1.26.21/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.21/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/books.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/lb.py
+-rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/playback.py
+-rw-r--r--   0        0        0    26772 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.21/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.21/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.21/LICENSE
+-rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.21/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.21/pyproject.toml
+-rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.21/PKG-INFO
```

### Comparing `xklb-1.26.20/Windows.md` & `xklb-1.26.21/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/pdm.lock` & `xklb-1.26.21/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -792,16 +792,16 @@
 [[package]]
 name = "rebulk"
 version = "3.2.0"
 summary = "Rebulk - Define simple search patterns in bulk to perform advanced matching on any string."
 
 [[package]]
 name = "regex"
-version = "2023.3.23"
-requires_python = ">=3.8"
+version = "2023.5.4"
+requires_python = ">=3.6"
 summary = "Alternative regular expression module, to replace re."
 
 [[package]]
 name = "requests"
 version = "2.24.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "Python HTTP for Humans."
@@ -821,15 +821,15 @@
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.263"
+version = "0.0.264"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -2472,102 +2472,130 @@
     {url = "https://files.pythonhosted.org/packages/0c/2f/894bc187ce40367f2e878ced196e1b5a9bc66cb553a062ed955d4f7dcbab/rarfile-4.0.tar.gz", hash = "sha256:67548769229c5bda0827c1663dce3f54644f9dbfba4ae86d4da2b2afd3e602a1"},
     {url = "https://files.pythonhosted.org/packages/95/f4/c92fab227c7457e3b76a4096ccb655ded9deac869849cb03afbe55dfdc1e/rarfile-4.0-py3-none-any.whl", hash = "sha256:1094869119012f95c31a6f22cc3a9edbdca61861b805241116adbe2d737b68f8"},
 ]
 "rebulk 3.2.0" = [
     {url = "https://files.pythonhosted.org/packages/84/4d/df073d593f7e7e4a5a7e19148b2e9b4ae63b4ddcbb863f1e7bb2b6f19c62/rebulk-3.2.0-py3-none-any.whl", hash = "sha256:6bc31ae4b37200623c5827d2f539f9ec3e52b50431322dad8154642a39b0a53e"},
     {url = "https://files.pythonhosted.org/packages/f2/06/24c69f8d707c9eefc1108a64e079da56b5f351e3f59ed76e8f04b9f3e296/rebulk-3.2.0.tar.gz", hash = "sha256:0d30bf80fca00fa9c697185ac475daac9bde5f646ce3338c9ff5d5dc1ebdfebc"},
 ]
-"regex 2023.3.23" = [
-    {url = "https://files.pythonhosted.org/packages/03/86/4a27b8135ec8e1e16ee1fcabe5123d879064eabf20aacf22daf794988474/regex-2023.3.23-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:cde09c4fdd070772aa2596d97e942eb775a478b32459e042e1be71b739d08b77"},
-    {url = "https://files.pythonhosted.org/packages/06/64/ae837863a7490e30b5da4659f5d9709980e45031f1563c5a4d4bb6668a36/regex-2023.3.23-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:6560776ec19c83f3645bbc5db64a7a5816c9d8fb7ed7201c5bcd269323d88072"},
-    {url = "https://files.pythonhosted.org/packages/07/dc/5366a12c377a1cf905d936a31139d80d279110a4616a14b24cc48e658eae/regex-2023.3.23-cp38-cp38-win32.whl", hash = "sha256:fffe57312a358be6ec6baeb43d253c36e5790e436b7bf5b7a38df360363e88e9"},
-    {url = "https://files.pythonhosted.org/packages/1b/cc/628702b6b71d4e3c84dedd7c37210e30e58e235b826dbc0320f51cdbe1d5/regex-2023.3.23-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:22720024b90a6ba673a725dcc62e10fb1111b889305d7c6b887ac7466b74bedb"},
-    {url = "https://files.pythonhosted.org/packages/1f/28/5d339d983a3398047b568435b88a32e5c30887bd3e331f61d78e52d9969a/regex-2023.3.23-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:ef3f528fe1cc3d139508fe1b22523745aa77b9d6cb5b0bf277f48788ee0b993f"},
-    {url = "https://files.pythonhosted.org/packages/22/bd/d891dfcc9ebbdc60535ac2b0de076f928202553268030c73e246a0bd84ea/regex-2023.3.23-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4c49552dc938e3588f63f8a78c86f3c9c75301e813bca0bef13bdb4b87ccf364"},
-    {url = "https://files.pythonhosted.org/packages/24/f5/9e07cde4587dc3d5612ed39980ac3379359a971405a78837065bffa1dbe0/regex-2023.3.23-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:086afe222d58b88b62847bdbd92079b4699350b4acab892f88a935db5707c790"},
-    {url = "https://files.pythonhosted.org/packages/26/30/1b061ad1f85d6147ee2d181e8e36503996bf386ef9fb1d5ff8afa88d7c70/regex-2023.3.23-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:c37df2a060cb476d94c047b18572ee2b37c31f831df126c0da3cd9227b39253d"},
-    {url = "https://files.pythonhosted.org/packages/29/36/3d50a5f45efec70e4480de50a591e272d60c8cc1f4fce95298fc3fc66257/regex-2023.3.23-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:4479f9e2abc03362df4045b1332d4a2b7885b245a30d4f4b051c4083b97d95d8"},
-    {url = "https://files.pythonhosted.org/packages/29/90/804db81268636547e25004404587e75a269fd6f7a38aa2d9e1209ed61544/regex-2023.3.23-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b7006105b10b59971d3b248ad75acc3651c7e4cf54d81694df5a5130a3c3f7ea"},
-    {url = "https://files.pythonhosted.org/packages/2b/c2/12f0de728011be620421cec5884f41b651176821487b67631cc093585215/regex-2023.3.23-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:dd7200b4c27b68cf9c9646da01647141c6db09f48cc5b51bc588deaf8e98a797"},
-    {url = "https://files.pythonhosted.org/packages/2d/8b/2b012e1f4c0f5e1fc2e96a9bd6dab0f2f4bc4dfb61b969916cfd436d7843/regex-2023.3.23-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1b1fc2632c01f42e06173d8dd9bb2e74ab9b0afa1d698058c867288d2c7a31f3"},
-    {url = "https://files.pythonhosted.org/packages/32/14/cef8e14cf732f723951ad2bcf38965b01acd3819204831116a96946690d6/regex-2023.3.23-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e152461e9a0aedec7d37fc66ec0fa635eca984777d3d3c3e36f53bf3d3ceb16e"},
-    {url = "https://files.pythonhosted.org/packages/34/b1/be831936f5acf8127d2624a300e89a5c0dc5c3a76a335be8d85534cc7728/regex-2023.3.23-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:c125a02d22c555e68f7433bac8449992fa1cead525399f14e47c2d98f2f0e467"},
-    {url = "https://files.pythonhosted.org/packages/3a/f7/d073dc0914c89b97bbcf6b087f9e83c913853d96795a934d958099552196/regex-2023.3.23-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:db034255e72d2995cf581b14bb3fc9c00bdbe6822b49fcd4eef79e1d5f232618"},
-    {url = "https://files.pythonhosted.org/packages/41/59/3a725abd03da0a10555b9afcc954a80e5cd6d040f2bbc0e81a944715b63d/regex-2023.3.23-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:845a5e2d84389c4ddada1a9b95c055320070f18bb76512608374aca00d22eca8"},
-    {url = "https://files.pythonhosted.org/packages/42/60/1694cef16929dc1c7831fee0d8a25d81de741d7baf424b633e8c9597ebbb/regex-2023.3.23-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:cf86b4328c204c3f315074a61bc1c06f8a75a8e102359f18ce99fbcbbf1951f0"},
-    {url = "https://files.pythonhosted.org/packages/47/ac/7631ae51893aca9478cc26422ce66563682880b849c27af1cf0e2695e20b/regex-2023.3.23-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d895b4c863059a4934d3e874b90998df774644a41b349ebb330f85f11b4ef2c0"},
-    {url = "https://files.pythonhosted.org/packages/4f/5e/aa17cfd9e4cf1451622f02a0dde488d23ed01110327b303f56cc4140d4e8/regex-2023.3.23-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:a81c9ec59ca2303acd1ccd7b9ac409f1e478e40e96f8f79b943be476c5fdb8bb"},
-    {url = "https://files.pythonhosted.org/packages/4f/bf/3177bc0051029df278ed9cfc6de94753b2968b0d82bc9246a3e37a652dfa/regex-2023.3.23-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:93f3f1aa608380fe294aa4cb82e2afda07a7598e828d0341e124b8fd9327c715"},
-    {url = "https://files.pythonhosted.org/packages/58/82/ff6778eb678d5758df44fa3a51cbacbe4352d05386c0957b44203e574628/regex-2023.3.23-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:2848bf76673c83314068241c8d5b7fa9ad9bed866c979875a0e84039349e8fa7"},
-    {url = "https://files.pythonhosted.org/packages/59/ed/8a4bc1983cc95fdb19b8627ffc44361a281dcc03da0bfdde4e6a07113a5b/regex-2023.3.23-cp310-cp310-win32.whl", hash = "sha256:9d764514d19b4edcc75fd8cb1423448ef393e8b6cbd94f38cab983ab1b75855d"},
-    {url = "https://files.pythonhosted.org/packages/5a/e1/c191c9752d1d66daf9fb6443db13c1d3c5405a4b2b0136cbb86126b8758c/regex-2023.3.23-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:787954f541ab95d8195d97b0b8cf1dc304424adb1e07365967e656b92b38a699"},
-    {url = "https://files.pythonhosted.org/packages/5d/85/524279048b9405be3d3318a5926b142b4d75f40083fed40fb21c957df480/regex-2023.3.23-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0b8eb1e3bca6b48dc721818a60ae83b8264d4089a4a41d62be6d05316ec38e15"},
-    {url = "https://files.pythonhosted.org/packages/64/7e/5f748fb16ac16c919a6ee9c5623d622914fe4bf99a0f51f8524a88a9f421/regex-2023.3.23-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:9bf4a5626f2a0ea006bf81e8963f498a57a47d58907eaa58f4b3e13be68759d8"},
-    {url = "https://files.pythonhosted.org/packages/6b/2b/d3a33a47805c64e15f3a3b092ce4a55c8720249b80aa5f72b77b541b0df5/regex-2023.3.23-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:79e29fd62fa2f597a6754b247356bda14b866131a22444d67f907d6d341e10f3"},
-    {url = "https://files.pythonhosted.org/packages/6c/58/4e5e33e944f54dfe48e1fe7a1be6bde30e6553d4e0ba059ba4b111359515/regex-2023.3.23-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:e2396e0678167f2d0c197da942b0b3fb48fee2f0b5915a0feb84d11b6686afe6"},
-    {url = "https://files.pythonhosted.org/packages/72/18/dc772b16749461cd3ec24573934f040f9814d84c6559a8ca4da9ac6b8ae1/regex-2023.3.23-cp311-cp311-win_amd64.whl", hash = "sha256:5ccfafd98473e007cebf7da10c1411035b7844f0f204015efd050601906dbb53"},
-    {url = "https://files.pythonhosted.org/packages/73/98/b96802c10f51d81770496812489854014578616ae62e874e2fd2a4aa4556/regex-2023.3.23-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e76b6fc0d8e9efa39100369a9b3379ce35e20f6c75365653cf58d282ad290f6f"},
-    {url = "https://files.pythonhosted.org/packages/74/71/abf5df0be7a29b6920d4ae85eb685584afbe84610631b70fe366b2857801/regex-2023.3.23-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:86b036f401895e854de9fefe061518e78d506d8a919cc250dc3416bca03f6f9a"},
-    {url = "https://files.pythonhosted.org/packages/79/67/f9a546833ed75af00e8e5163ec0fe2771bf224410b914d7f95fbb7808d25/regex-2023.3.23-cp310-cp310-win_amd64.whl", hash = "sha256:11d1f2b7a0696dc0310de0efb51b1f4d813ad4401fe368e83c0c62f344429f98"},
-    {url = "https://files.pythonhosted.org/packages/79/f9/073a75ba8732b5f2352b7a0a9bf2fcbe0a546cf9be568879c4b27ca13986/regex-2023.3.23-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5fc33b27b1d800fc5b78d7f7d0f287e35079ecabe68e83d46930cf45690e1c8c"},
-    {url = "https://files.pythonhosted.org/packages/7c/3e/ad079974cbfc00ed6d355e4c26cb733ed19abd5418b3784f989d6c86303a/regex-2023.3.23-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:3cd9f5dd7b821f141d3a6ca0d5d9359b9221e4f051ca3139320adea9f1679691"},
-    {url = "https://files.pythonhosted.org/packages/80/38/0cb4cb0ba49f7bbf25225689ae58d8232997a33fe193950025f7df733474/regex-2023.3.23-cp38-cp38-win_amd64.whl", hash = "sha256:dbb3f87e15d3dd76996d604af8678316ad2d7d20faa394e92d9394dfd621fd0c"},
-    {url = "https://files.pythonhosted.org/packages/80/a5/964f6cf453c806fd46c97fa2ba432eff91767d1e5fd9d0d49ff9c97edc05/regex-2023.3.23-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:75f288c60232a5339e0ff2fa05779a5e9c74e9fc085c81e931d4a264501e745b"},
-    {url = "https://files.pythonhosted.org/packages/84/72/9e6273be7027630c65650b43f964845888cc10152fd92a087007197685f1/regex-2023.3.23-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7868b8f218bf69a2a15402fde08b08712213a1f4b85a156d90473a6fb6b12b09"},
-    {url = "https://files.pythonhosted.org/packages/84/eb/24dd2a4b708a3032673f8c459d14adb441456aa65630cb2d68085176b7c9/regex-2023.3.23-cp311-cp311-win32.whl", hash = "sha256:25f0532fd0c53e96bad84664171969de9673b4131f2297f1db850d3918d58858"},
-    {url = "https://files.pythonhosted.org/packages/9c/31/c22dc60971e0dddaf86375502fcf171cfce33013f58a7407529fecab6d8c/regex-2023.3.23-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:cd1671e9d5ac05ce6aa86874dd8dfa048824d1dbe73060851b310c6c1a201a96"},
-    {url = "https://files.pythonhosted.org/packages/a3/ad/e6ff08c482396fc063858c7919618235300455bd86add3ab26def9c7d5e7/regex-2023.3.23-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2472428efc4127374f494e570e36b30bb5e6b37d9a754f7667f7073e43b0abdd"},
-    {url = "https://files.pythonhosted.org/packages/a5/b6/9324c6da8957c9faaaccbaa734710bb5d57fa1e7b6e2c6a4167ebf4843ee/regex-2023.3.23-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:55ae114da21b7a790b90255ea52d2aa3a0d121a646deb2d3c6a3194e722fc762"},
-    {url = "https://files.pythonhosted.org/packages/a7/69/275f20553b194755c4a5e36f337862eccf6942ec55f794341f62e93dba65/regex-2023.3.23-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:8a9c63cde0eaa345795c0fdeb19dc62d22e378c50b0bc67bf4667cd5b482d98b"},
-    {url = "https://files.pythonhosted.org/packages/aa/12/153b4ff30a3aa3adca197040fba7e5167ed04a75cc0c0df297a4a2399b82/regex-2023.3.23-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:fdf7ad455f1916b8ea5cdbc482d379f6daf93f3867b4232d14699867a5a13af7"},
-    {url = "https://files.pythonhosted.org/packages/b5/77/4e41254b2d6286d8a3e231480f11e79ea3cee7632f283063f24d9483e1a3/regex-2023.3.23-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:c869260aa62cee21c5eb171a466c0572b5e809213612ef8d495268cd2e34f20d"},
-    {url = "https://files.pythonhosted.org/packages/b6/c0/7ac01da1fbe7c92a3684757476f3b2b060d7f21ab4cb70ed1fedb63719eb/regex-2023.3.23-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c88e8c226473b5549fe9616980ea7ca09289246cfbdf469241edf4741a620004"},
-    {url = "https://files.pythonhosted.org/packages/bb/4f/65c14619af6e6640d8eac947a8322582207beed27fb29fbb927653a51b38/regex-2023.3.23-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:20abe0bdf03630fe92ccafc45a599bca8b3501f48d1de4f7d121153350a2f77d"},
-    {url = "https://files.pythonhosted.org/packages/c6/0d/1ccc866a040c968ab331370e20b5ac48165459f76577c89f06e0f89c4dc4/regex-2023.3.23-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:d5bbe0e1511b844794a3be43d6c145001626ba9a6c1db8f84bdc724e91131d9d"},
-    {url = "https://files.pythonhosted.org/packages/c6/25/76a877c64d2677d6ea0b4011db4c3966eba1c473d342e5a2e0d8dcb70752/regex-2023.3.23-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:87d9951f5a538dd1d016bdc0dcae59241d15fa94860964833a54d18197fcd134"},
-    {url = "https://files.pythonhosted.org/packages/c6/4e/1aa518dd6dc23b1e1a7763d3f31fbd900146eada71d8dad0a1d7758302ac/regex-2023.3.23-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:a610e0adfcb0fc84ea25f6ea685e39e74cbcd9245a72a9a7aab85ff755a5ed27"},
-    {url = "https://files.pythonhosted.org/packages/d0/c3/3d59eddb6fe745f5152a5da4f666125e9a2aae1609797cb5cd2d0a4141eb/regex-2023.3.23-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:df45fac182ebc3c494460c644e853515cc24f5ad9da05f8ffb91da891bfee879"},
-    {url = "https://files.pythonhosted.org/packages/d4/09/3e487710dec97906fd18df0ed93040b477e9c3ff6cdbc5f99caa256c891a/regex-2023.3.23-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6572ff287176c0fb96568adb292674b421fa762153ed074d94b1d939ed92c253"},
-    {url = "https://files.pythonhosted.org/packages/d6/00/cc5e8fde1042bbea9aee31e420b269655ae570cb85f3e52a6586cfaa1492/regex-2023.3.23-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6b190a339090e6af25f4a5fd9e77591f6d911cc7b96ecbb2114890b061be0ac1"},
-    {url = "https://files.pythonhosted.org/packages/d8/29/bd8de07107bc952e0e2783243024e1c125e787fd685725a622e4ac7aeb3c/regex-2023.3.23.tar.gz", hash = "sha256:dc80df325b43ffea5cdea2e3eaa97a44f3dd298262b1c7fe9dbb2a9522b956a7"},
-    {url = "https://files.pythonhosted.org/packages/e1/0b/8f4c19f0ced880501f96906e65f484ef1b42fe6bd93f79c9b5c1914f2618/regex-2023.3.23-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:11d00c31aeab9a6e0503bc77e73ed9f4527b3984279d997eb145d7c7be6268fd"},
-    {url = "https://files.pythonhosted.org/packages/e2/00/092e2537588afa89928fa98d0b7363461336bda5b57479158fb6c4ffbdfd/regex-2023.3.23-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c07ce8e9eee878a48ebeb32ee661b49504b85e164b05bebf25420705709fdd31"},
-    {url = "https://files.pythonhosted.org/packages/e5/51/7a33a1a655fbd127d7ae2ab542d26530ec51e244169e371c91b256b39927/regex-2023.3.23-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:37ae17d3be44c0b3f782c28ae9edd8b47c1f1776d4cabe87edc0b98e1f12b021"},
-    {url = "https://files.pythonhosted.org/packages/e7/59/8d84338a75457e1450a648e3c588efe35191157ecf3ef7d46deac3af0347/regex-2023.3.23-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:78ac8dd8e18800bb1f97aad0d73f68916592dddf233b99d2b5cabc562088503a"},
-    {url = "https://files.pythonhosted.org/packages/f4/29/950eeaafdc6165b4d2212ae52f34da0f8035ca351877e45622d04afaa953/regex-2023.3.23-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:539dd010dc35af935b32f248099e38447bbffc10b59c2b542bceead2bed5c325"},
-    {url = "https://files.pythonhosted.org/packages/fb/55/98d7ff983be33d572a1bbe073b6b1b5db249f467dcff2bb8d516b66c9848/regex-2023.3.23-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:ea3c0cb56eadbf4ab2277e7a095676370b3e46dbfc74d5c383bd87b0d6317910"},
-    {url = "https://files.pythonhosted.org/packages/fe/68/63349d423d856993cbe1939f9189c826e757a4bb08fda931e6e7bfeb70cd/regex-2023.3.23-cp39-cp39-win32.whl", hash = "sha256:7304863f3a652dab5e68e6fb1725d05ebab36ec0390676d1736e0571ebb713ef"},
-    {url = "https://files.pythonhosted.org/packages/fe/b3/afcb0c6fde8c5ee24c7cb5d29d0caafb9b57dd4b1400ca66cfc12d67e2b4/regex-2023.3.23-cp39-cp39-win_amd64.whl", hash = "sha256:54c3fa855a3f7438149de3211738dd9b5f0c733f48b54ae05aa7fce83d48d858"},
+"regex 2023.5.4" = [
+    {url = "https://files.pythonhosted.org/packages/01/1a/4fb1c70672600cca37ba7e11c072ddaa1ecdc96e9c1d7eab0f7a9703e99b/regex-2023.5.4-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:50e00ab84396bfbeb1bede61eff6641f957b6532e74e02be480d71914e20e2ac"},
+    {url = "https://files.pythonhosted.org/packages/03/cc/ba5ea5adbc905457657003a32121c01e6576385e6cec223bc31f922e950b/regex-2023.5.4-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:12be293d718e05f7304f715980b1a25b16e34a1ff2121740592559d066f91e67"},
+    {url = "https://files.pythonhosted.org/packages/05/3a/0ffbdf689acc1efb09e025de44230e100881572b1ee6541c6e81a10d430b/regex-2023.5.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:49a77f0b62a4122cf578d1194658973c435e6d2a9611013be11b6750056a5930"},
+    {url = "https://files.pythonhosted.org/packages/06/90/83e9bbd99f9aca188c717f11609c809b932ca30444eb911f7876f2e366c8/regex-2023.5.4-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:70bd0c121b3c4e641e5c4e633c4581059acad774a1a62bcb15fea3470c2a61cc"},
+    {url = "https://files.pythonhosted.org/packages/09/fd/fde7450d2e63eff77540df7d1d597ef82dafc0940e0813f191eb00e2b8c9/regex-2023.5.4-cp38-cp38-win_amd64.whl", hash = "sha256:6f02105d4a511f550dcd63f750937d1607a1f6dc253c798c4adf36aba89215a3"},
+    {url = "https://files.pythonhosted.org/packages/0a/32/0ac260cfcddbd0421976e85f4f7eb1b7c9eee94520fa451d0d0c3c43f158/regex-2023.5.4-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:b87d38717ed855583ae1693f6095fc9c06b7dde4ddec782b41aa92931dd60e7c"},
+    {url = "https://files.pythonhosted.org/packages/0a/e7/7c13b09b81bb6c6baef2a53fc658784b01f874d2309a0e4e3d5399568769/regex-2023.5.4-cp39-cp39-win32.whl", hash = "sha256:97fd2885df308edcdf96baa632192a4291f3ed5b072c0bc3f29dc1e6de40ffa4"},
+    {url = "https://files.pythonhosted.org/packages/0f/9e/09c6e02652cec2233f0f01633d3ab7ed916f688ebd5b51b62b77822c8201/regex-2023.5.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:0eee66c4ce6ced2e9d5d4497a569bab6257a6d118eb43dd57cceb61ba00b62d8"},
+    {url = "https://files.pythonhosted.org/packages/10/17/b87bb3cb3752e6dfd55b8590c991a8c92c1bf4dd2674c0132124272e2e1a/regex-2023.5.4-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a419384c6c80d58532016c3cf6a3aca009bfb7661f33e119ba7f77ec0e28222a"},
+    {url = "https://files.pythonhosted.org/packages/10/45/e2d8ef3e5ad225937b793111bb7ad0c6825a57454fb9bc916f5b21240b69/regex-2023.5.4-cp310-cp310-win32.whl", hash = "sha256:c455d886838dd5a248e7f06e5573275fc854febd206eb937cf632082a06a939f"},
+    {url = "https://files.pythonhosted.org/packages/13/bb/f63e8a0e38a6892f3f5ed6202b6e24c50a8598120ed2daf75c8415bdbd68/regex-2023.5.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d28933aa1242814ed737b569b2baf96e4d236c52be454b5dc17afd36bf893c12"},
+    {url = "https://files.pythonhosted.org/packages/1c/65/2d0ed6c73ea9ecc371d403a51ae0e0859c0970122fd94d1c4b8d8e48cf43/regex-2023.5.4-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:2762750332f57820c0f38ade87ce4ebe671b178892faed0112f574f0b42801cf"},
+    {url = "https://files.pythonhosted.org/packages/1f/82/5a8e0486a7b66934169b6745be39ea3b69d76d2f0503b12ae59c56f89ca0/regex-2023.5.4-cp311-cp311-win32.whl", hash = "sha256:21b653c1538cbbc1c58f6d6f3ccb4a5ce56491f0ab370ec057c1c64a152eb48c"},
+    {url = "https://files.pythonhosted.org/packages/21/e6/46feb3e69d6147750e2799a685ca45e09c77842b9fff8208571f8f282f89/regex-2023.5.4-cp311-cp311-win_amd64.whl", hash = "sha256:336fb3f585e239362d4f26dd6f904b15d91febfc980f47ed706858f5cee20ce6"},
+    {url = "https://files.pythonhosted.org/packages/21/ff/4ca3dcab09b13b0e9bb002e528987c6ce3310e6e1c92c5fbc28716371031/regex-2023.5.4-cp37-cp37m-win_amd64.whl", hash = "sha256:6469c2baf450fd1e648752b113a1fc1d67dfbad359f6171be954bacf7b09d126"},
+    {url = "https://files.pythonhosted.org/packages/26/d7/8f2a8078a379f3c6ec3ca5d13b9f27249e1f4883349ac28676d5fb554776/regex-2023.5.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9322797fddd51ec0312a8b649d9a3ebfabf4826a204ef8e1cc11801013005323"},
+    {url = "https://files.pythonhosted.org/packages/2e/9d/e4880bab2c00f1354b1db70fd84cf360badfdb57e94c1f0ba2b67037d23c/regex-2023.5.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5fda1fc36dd923aee070d7aab3a85b448c8b62930900c615bb67db829281103b"},
+    {url = "https://files.pythonhosted.org/packages/31/93/f9f9b6f9c25a5086b83385fb400b408893856b667bd535f15c80a91e91ab/regex-2023.5.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5a98814d42282153c30d674ee34ea114a03ea8d32fd5d9b924d46fbeb2c7eb15"},
+    {url = "https://files.pythonhosted.org/packages/32/b2/506a122fe479f58a6614214909be2168cbfd3d9d3598ab232ed2ad60571f/regex-2023.5.4-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:dbcb49036a6a6065035ac2acc1ad6a918f9e09ef2d0f9392dc90b8756f789f95"},
+    {url = "https://files.pythonhosted.org/packages/36/db/93cef84a8af277c8866c435dab0a2d4045d20549acc5f73593f6264c5fe3/regex-2023.5.4-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:24db1c0fc20850db47977824a99fdae81d6764adaf8192dd874185d9e7166dbb"},
+    {url = "https://files.pythonhosted.org/packages/38/47/a429a1d00496171362b8ae109a295b902824dd548ec24b92155a383836b0/regex-2023.5.4-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:c40f7e8c02b287550166a3e36dbb89f9387db86a71101f6242668e3ef979cd2a"},
+    {url = "https://files.pythonhosted.org/packages/39/86/86117b7889e38dee695dc60fd0f569fe47d8ff318318b1f421801a5e9154/regex-2023.5.4-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0130a2fdd6f033c3e3710d0b950cc6abd3133c5af88c40c78e77641cb6f6cf8a"},
+    {url = "https://files.pythonhosted.org/packages/39/93/38f46dd02c89fc373c31f14a5df945384e040407a391365d5d9c8f49e180/regex-2023.5.4-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ad84e1d4be3504e7dcd6370b3e847eaf05d5d35cb0818d0bd2d1a26b58c0abd2"},
+    {url = "https://files.pythonhosted.org/packages/41/2d/33169d1bb13ed2b68150f27675e897f1fc24d4c80a313fb5d800e7bbc5ed/regex-2023.5.4-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:1dc5e9a847613679ac8bd0386a0e54f2958441a0fcc123778637e433041aa763"},
+    {url = "https://files.pythonhosted.org/packages/48/a5/56010ba4cab8a1c50f25f7a108fb114d7ae828e06bb19de97641ff15924d/regex-2023.5.4-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5a7ab3440f0c653dee8b42af858da6e07615c64ba86a6b3509a0ecf44eabdb11"},
+    {url = "https://files.pythonhosted.org/packages/4b/81/ec8e57e1981f71598b1750cadbfb40f067dbf83cf6dc255d838af22ddb50/regex-2023.5.4-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d0ac14c36d91b191d1cb073fb5ac49937d88a5c8b051ced3875321a525202c34"},
+    {url = "https://files.pythonhosted.org/packages/4c/06/bf3ed4b16c629b63768d51e5a4e239feea1607ae5be46279aa5c83e267d8/regex-2023.5.4-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:953ba37dd83c424c2cf699c64a8477645fc7c7403ffd2eb1417189eddbbfb4a7"},
+    {url = "https://files.pythonhosted.org/packages/4c/cf/e97d56347b8876b12ac527e1f141bed66f6aba01f8a76e0072e375f01d76/regex-2023.5.4-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:6ccd0d7557c4e76303a6429ec9de55cd87334809cda66c0f101831e2ce9073c1"},
+    {url = "https://files.pythonhosted.org/packages/54/16/bc7cdeaa8bd3b335c0bf381c99f735e0c349db61fee2a903f1852f1b93d3/regex-2023.5.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0c731522eaf74166066fcf91fe7fe3c3617cc5e8df0c150132282d0dd5225afc"},
+    {url = "https://files.pythonhosted.org/packages/58/af/f6d7b31c8a5932b39a6cdc75906f612c5e1dae222a73780c5806a5ad86c0/regex-2023.5.4-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:770f825c7751ce43aae2088fee94f2e60f95e181223642a0bb35cbaeea92001c"},
+    {url = "https://files.pythonhosted.org/packages/5a/9c/48adaa6e0c65afc49a27f3439feb58c9a36a6a710647ab48d087f4014c70/regex-2023.5.4-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:ccd0c918971f79bd9a883f13f91343dd2eaefbafd4344aadfe5134a65fb821c3"},
+    {url = "https://files.pythonhosted.org/packages/5b/47/1e1f5d045021d0695f4269124d0d1030729bd0000702ff36d9a865d4312f/regex-2023.5.4-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:63a92f28a3f285dae06aae83227cb66cc87256db040aaf26c1c48ae5221eccde"},
+    {url = "https://files.pythonhosted.org/packages/5c/1e/eb14946b6e78024c9371d4b834a165ca065391ee242d478aef674c6c3256/regex-2023.5.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0d5a0edefdf800aeef6cf559af75e614fb2eb2d0388f0b132af805fdefcf8ec6"},
+    {url = "https://files.pythonhosted.org/packages/5d/86/e34d9cfa857258deba9c79c8011bcaae3a8ad31a581b8d951a9953836969/regex-2023.5.4-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:1ad00c9aae6090d052c0ee16a2737a7154031793e6c7b58a629eed8d8aa77e31"},
+    {url = "https://files.pythonhosted.org/packages/5f/24/46cd7ea6169df6e15ba10d4947e490e6e952bd00c2de44afe7fbf3aba525/regex-2023.5.4-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b132e4507c6404faece005329de7b2b97653ddfeeaf84f058fe820791160dcda"},
+    {url = "https://files.pythonhosted.org/packages/5f/25/6f7de88e18d4a2ce7ef5dc4e95401f85fdc54b1ecd1cb46f6c95cf4792d8/regex-2023.5.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9b887d87188489859411d0c7e741f7dfe8a3ca5946b0db8b3c9e5daecc089b62"},
+    {url = "https://files.pythonhosted.org/packages/62/6d/e63fbfc497042bc63b67e78290711378ea4cb0fff17dabf9609948508d7d/regex-2023.5.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:dbc47670e0424a566084e15af9a253b85f90fa26e60fa07e1b10c90df4c8fd07"},
+    {url = "https://files.pythonhosted.org/packages/63/b8/9412699b5c16d7e99946c5cc9f96a921b77cdb2af8c3c469bee574166804/regex-2023.5.4-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:797bab57e1317c940030f3c15d48c01e1f16d12ba0f6a807ee0bebdc1cfe3f2d"},
+    {url = "https://files.pythonhosted.org/packages/72/e0/36de8c428cfb1f711816470fa9da28ea68f495254dc62e3017f6b0c32cbb/regex-2023.5.4-cp310-cp310-win_amd64.whl", hash = "sha256:e87450db3c444f41e3ac6a09b7a10ddfe54fa1e98bf60ee299fe6d11097540cd"},
+    {url = "https://files.pythonhosted.org/packages/75/6e/664a14843220cef3b593371a51f4a26fd2fc439475d9be3002cef468ecbe/regex-2023.5.4-cp36-cp36m-win_amd64.whl", hash = "sha256:027d4962340dbd84979fd1c40bfd7ca8362030abfbbff25f1327bbf4867f047c"},
+    {url = "https://files.pythonhosted.org/packages/78/9a/df8680ae2117c4513f68dd0f90ac431551a4276450ab395571b244795518/regex-2023.5.4-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:89f54d4bbd452a5ee01dc31ec918f7b1f32483f13d3598af1acf5ea82ad82ad3"},
+    {url = "https://files.pythonhosted.org/packages/7c/9d/3f4271429150cf60817d2800b5dcdb8ec75cd698935a35007ac4ba8085da/regex-2023.5.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:db5d5c9c7bbcf9cbc541f8adba8c92a7a7abd0de4f0343da4e96fb78ffe9d1a1"},
+    {url = "https://files.pythonhosted.org/packages/7f/f4/2ae63513814b16204371d216d0e7534d6c4421b3db2bb8f62dbdc0a71f4a/regex-2023.5.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8c704e7062c59d2f7e2eebda2c0c0b69bd807ca6579c3a21fc4b1d8505cfc090"},
+    {url = "https://files.pythonhosted.org/packages/84/82/76e3e8422ddaacc5700f6597839ef30809843e9c13e74082a5d2c15bb216/regex-2023.5.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:fbc5b23b569d96b8c831574c93098b68c6d7ff2509f31268c968152ca4f2ecd0"},
+    {url = "https://files.pythonhosted.org/packages/87/48/2adbdffb16e8a4c0545df46e65b3f288f81f3c941e9bb41f847d5882e52c/regex-2023.5.4-cp36-cp36m-musllinux_1_1_ppc64le.whl", hash = "sha256:c1155571edd498b6274f969517db6781500fbb24fc91ff740ea5a37c4735b3ba"},
+    {url = "https://files.pythonhosted.org/packages/88/00/60b21a1bd9f905a26b05edba7db9d476c77e1f400c7b8615b8c1eb6421fe/regex-2023.5.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:1ef51012493837263236781ac9598f059dc4e5a4d72627bd3ac85cbd5d1b0ee1"},
+    {url = "https://files.pythonhosted.org/packages/89/a6/163269fca67d5aa0519d5961d1d92c988504441d6119215dc19481adbe3a/regex-2023.5.4-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:037f4be6a240a11a6d3397e932ef5d3ec5855858910792a0ab7d351bd0333533"},
+    {url = "https://files.pythonhosted.org/packages/8a/5f/4b178a1c1e50b668b3ae7da2e1a64ae77331d57dc7eba1a15150de2c9551/regex-2023.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c1fa9651141caaafa0d6048695a4a04bc4bf39c75f250a36b1a05c9588a403a9"},
+    {url = "https://files.pythonhosted.org/packages/8d/b2/9fd4c711b3dc910493aa93ec0fb2b81cb926cb034f29ed76e013a7a8e9e9/regex-2023.5.4-cp38-cp38-win32.whl", hash = "sha256:00f6f26e748c797a041ab6957f4cacc66a7fbd5dc5f627760985f5c5b7de2af6"},
+    {url = "https://files.pythonhosted.org/packages/93/c2/c350802f22f78b55eafd806953dd37e17064a95e135f57aadc6081d94318/regex-2023.5.4-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3d8cc797f87c07372e7d300198e1423c2b7bd35b68f375cc6700e26158940c9a"},
+    {url = "https://files.pythonhosted.org/packages/95/1c/b8628add2fe7f56951a2349d6b91503388fd2141718683da21d0f5c5e307/regex-2023.5.4-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c10b1388106447db0cdb8e340d06fa2d49b822368a049c36928d3c24296c2e37"},
+    {url = "https://files.pythonhosted.org/packages/95/db/9fa301b8abd90b47cd6c90a8d181d76705f94b5403c0220483f7dbefdd2b/regex-2023.5.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:aa92f9ad481108a7e4c5a5234608f7c718f8b67003ce4719a4d2735d82b54167"},
+    {url = "https://files.pythonhosted.org/packages/96/5b/c94cb87614eb47ae4c5f12fcfa17a638ac83a2b8f69832585f4bcc5b8a02/regex-2023.5.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:5d321dd059fd00482537aaba919e29189ea4ab6a03528881267982bb7707f610"},
+    {url = "https://files.pythonhosted.org/packages/96/eb/88b9a00654b962a0080aefb34add4402993406feb4ff18643f195ddfeb75/regex-2023.5.4-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f2bc7249840faacfff6196e5b5ffeb3fdaf078986521a1cda34e9be5607e773b"},
+    {url = "https://files.pythonhosted.org/packages/98/0c/b7ee04449927abe07871a55bb335ab8acc520a73aa79540aa9001457f2fd/regex-2023.5.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ea2d66c1fd898d81b8ce0f95afab9ba0ab522cf08810f11fa28ad958706cd2b2"},
+    {url = "https://files.pythonhosted.org/packages/9d/39/7bb5510155462138ebea3fd47c062ef079bb46bb957cd90f6773787a3190/regex-2023.5.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:2095acff95df0bf6ec3dee672a03d3d78606b4ca419d53fbd606c559cebedf45"},
+    {url = "https://files.pythonhosted.org/packages/a3/0e/170b3720d68baf866f7de484aa694e4dab2e2abc89927a563a7c59082de3/regex-2023.5.4-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:eaff21326bc5d9be0c2f400931d39274105bd5d06650f0b0215392d1b050d404"},
+    {url = "https://files.pythonhosted.org/packages/a4/8c/590b50ea391be247205713441fecb32b2aa050e833b89f2a814b2a7b2807/regex-2023.5.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:91f47522688955cb33190f8354ccaa1cc058d05e73f99afe9ace40db36c159e8"},
+    {url = "https://files.pythonhosted.org/packages/aa/28/324b556d8f5ec4a7d00e54ce362de3b1689697b0f0986073ff49ec9bd173/regex-2023.5.4-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:bda905e040e6c2875a7dde9652a9e0c426aaac6058568cc064f8128b061439ee"},
+    {url = "https://files.pythonhosted.org/packages/ab/e1/cbd88ac5426a97ec5a1f9d1f41094aa6b3d0fa9148bb0259dbd8cb382602/regex-2023.5.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:ff8fef88029d0420315935041db517855ea022889fa8d54959943e39fffebf59"},
+    {url = "https://files.pythonhosted.org/packages/ae/a6/ba2eef76ec8bbeb9f78610591d5c5a71866b01823763193c43b207b6c745/regex-2023.5.4-cp36-cp36m-musllinux_1_1_s390x.whl", hash = "sha256:1d98e4748a60c9902ad504e862756c43cc707404fc3025f82ef5bbe50bee3b9e"},
+    {url = "https://files.pythonhosted.org/packages/af/92/c1b41690de10780e80e878570397c6476ca1e68a612c078acac96a95ccfa/regex-2023.5.4-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:e708e69c4d3bc41df29efb94aadc5578c841b2cd02f8cbb1bcfbf280f2801238"},
+    {url = "https://files.pythonhosted.org/packages/af/b2/641758331548f171fbcddfd6f32f83e049ee93fe20a39725cd54fb7feda9/regex-2023.5.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:99780a0880d3dab2bb6f863492d38ab90ffdc9daf4fbefb505524f6f3a1c9dbe"},
+    {url = "https://files.pythonhosted.org/packages/b0/41/72441fc5e60d41f5c1051a94648f43aff1bef8e467f2963ae38431219c89/regex-2023.5.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4c2ae89c92a04b057b412f88a3359e77600ce966a740e2da212667ce795e1bdc"},
+    {url = "https://files.pythonhosted.org/packages/b0/47/6f06ed9008f35174397204fc56bea2fbcac1d843ab4d15dcf6cfb22b5f4c/regex-2023.5.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:b48820071a49b68ca8734e8b2bd1f26632512154816b261b614e62cc724d9f8a"},
+    {url = "https://files.pythonhosted.org/packages/b0/51/d4f159b33243f468fc4a4e0730ddc7b8edeae614d756eeb517ca1c6e5b41/regex-2023.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:cb22580ce5e2eee138a78df40444151ff51c91acd11be546216a046677c75593"},
+    {url = "https://files.pythonhosted.org/packages/b3/34/031b01104bbb56e85b10ad9a396e5c1fab81b29a748800f63e5abe8798d7/regex-2023.5.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3633a07ffeabc14f3cd531f11794bb603267d86e4109cb811a34aee020622d3f"},
+    {url = "https://files.pythonhosted.org/packages/b4/71/c41e92c996ae338fcedcebf8eb3ea155379ef9acbc96641c40364d51c11a/regex-2023.5.4-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b365b8fa0d5fd0208db5b0e94582edb796dde07d1f99c5a9c1ff6be172c374ee"},
+    {url = "https://files.pythonhosted.org/packages/b6/3b/a2cdd542ae9273816d80510920cd9c82382ae06439f39f6e78a602e5e6f7/regex-2023.5.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:8418b0ee315555ca9786daab00ec8aaf47dfb2698a5be689676e83e88b949f22"},
+    {url = "https://files.pythonhosted.org/packages/b7/bc/6880c51cc766db336f1d8aa2a34bcf7549c439d3da65822cb9923644f195/regex-2023.5.4-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:77b3333a6cd1161b81bcf018a9bdb3cc567074a913aa69b98b9c8c79be28565c"},
+    {url = "https://files.pythonhosted.org/packages/b7/c3/3eec96b9b46ae3c241d607cf297d0e7fa5660878133f563d6dc38387da8d/regex-2023.5.4-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:5f82d4e0725788787216c9ae53116e6e477b2d97f29ec1e5086f5afbab5716b0"},
+    {url = "https://files.pythonhosted.org/packages/c0/7a/0e302d0be5268a6703e90ec9b9b67b2c655f1aad3f7ca90316204e89355e/regex-2023.5.4-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:460672c6ec94997755bd37b00302853b9d85a5a433121c198359958e8c10ced5"},
+    {url = "https://files.pythonhosted.org/packages/c2/87/3371dfa064d1354232089ab6bd2b9d05ce5d2d51785338eb2412ea8b4b63/regex-2023.5.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:5cc67b3562aada6682ae45f2ea40819baa6bffe38155883100f8779c22c8c087"},
+    {url = "https://files.pythonhosted.org/packages/c4/37/3aa71aa11bc21efd618f148caeea0122050ff17a73bf76fee214f77193db/regex-2023.5.4-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:ebf0776fdc7a5e0ac11b6db2d69ac77479411b627a96119ffa4427ba32f3bb66"},
+    {url = "https://files.pythonhosted.org/packages/c5/dd/404aa5be84d68855fd1fd443f32838fa80803d633c21920540c5d9b997e2/regex-2023.5.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b7eb07d60c385aec906b82d48447907a2bbf454d0e9ead62168de111accabaf8"},
+    {url = "https://files.pythonhosted.org/packages/c6/7d/97e89f7c9874f84a880bf477313fefc3c909499243465f28b8fdc26740a5/regex-2023.5.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f576b8dec95456ba0157943a57f5f88c076cf96cc363ef1bf5027c2976fd487a"},
+    {url = "https://files.pythonhosted.org/packages/c7/73/388a37a3181f33b3a416b5d1bc3a13ac3894371214a80257cedc9c1026ff/regex-2023.5.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:0a664857dd9b1076942c4d73c54a031066ee0ae88a438e7a1e0e79c1c5ddf47a"},
+    {url = "https://files.pythonhosted.org/packages/cd/81/bf87ef23e4e11f7daeaa3349ba711122e2bf02ed8b49a6bfef53a33fb5b6/regex-2023.5.4-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f3e20cf2575b1330687d3dd6242f82278b3bdc09a9f36cc7ac4d45b7dd63c1f5"},
+    {url = "https://files.pythonhosted.org/packages/cf/77/7a215137960185b41ddbb1e74b84dedc66b8bc55e8c38c16d0ad87015b37/regex-2023.5.4-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6686256d1d435ed782ff12ef11e074705911a40d3907b986e53ca9a996e88489"},
+    {url = "https://files.pythonhosted.org/packages/d1/28/cb054f5ad66f8e81aedec637bb18be00b87bdac6713a95fdc5d13b91f50d/regex-2023.5.4-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:376fa2ef6a02a004b6fe4ebaa5ba370e7532ec6915efd12e33aa434517f8bbee"},
+    {url = "https://files.pythonhosted.org/packages/d2/2f/deae077e7e23a9810eb5aa2bc82a820e50fe627ea06217f060e736b552ff/regex-2023.5.4-cp36-cp36m-win32.whl", hash = "sha256:8d5bc5035989852a4ae7dacf8dc99db7c4f21c852486777a98b8efe37af4d8d7"},
+    {url = "https://files.pythonhosted.org/packages/e4/13/77cb2583a366c7fea8082396c280a3a1c8021011cd259933f097d77ed9b9/regex-2023.5.4-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:ac402ac165f42f41b3aef9e8a9c6fb204dac31faad65b3b0ae6bff4bc9d0dad2"},
+    {url = "https://files.pythonhosted.org/packages/e4/e6/eac6b94eaf4081ccbe08aaff2e729f4c24b7ddaaffd023c0d8d9693ca8fc/regex-2023.5.4.tar.gz", hash = "sha256:9e1b4b0b4baff934ef3c0ac56578a6b773f7f90ad1db3ff843ee40d83bdae09f"},
+    {url = "https://files.pythonhosted.org/packages/f3/ee/d8bc48c2773afa2c0ac10f31163f5d119703cee146a2a766365391406037/regex-2023.5.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c300461ed8159f61d979971ba51f1acd1e6f9907d86888e9275165e06ea90f06"},
+    {url = "https://files.pythonhosted.org/packages/f7/60/55aad6d2554a71705a209c056ecbf28515044e4d1ca681951f4a6753d4c6/regex-2023.5.4-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3965a9ab13f1bf3e4af021c7dbe9678dd9f8dc5cc9097b3d3cbbf3ad00574b5d"},
+    {url = "https://files.pythonhosted.org/packages/fb/a5/28a78b8bf5c3daba4bc0d12ae8bb7cc454925a6855cfe8c6ef4c9522caf1/regex-2023.5.4-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:861ed1249302664f96b2e968216486a02af0a143e0f3cc6fd92b78f11aa18579"},
+    {url = "https://files.pythonhosted.org/packages/fd/da/071972ad34fac0237532254a9d3ad4b859537486b20b90f492a20d126b73/regex-2023.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:04a825fd9f5931263eccd0cbdbf171a9792fa1bf2642ca62800b57689ca1b660"},
+    {url = "https://files.pythonhosted.org/packages/fe/a7/88cdcaaf6b61f977e927df302fb432925709b896f7087e030eb1f37401a6/regex-2023.5.4-cp37-cp37m-win32.whl", hash = "sha256:06fe9870165d4975a8a3e27a83919b9014b35dd2ee7061a5f2be8e579294cedc"},
 ]
 "requests 2.24.0" = [
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.3.5" = [
     {url = "https://files.pythonhosted.org/packages/39/03/6de23bdd88f5ee7f8b03f94f6e88108f5d7ffe6d207e95cdb06d9aa4cd57/rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
     {url = "https://files.pythonhosted.org/packages/3d/0b/8dd34d20929c4b5e474db2e64426175469c2b7fea5ba71c6d4b3397a9729/rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
 ]
-"ruff 0.0.263" = [
-    {url = "https://files.pythonhosted.org/packages/08/01/e553109ab71bcef7dbf994b7c935f683857cdd7cef8353a76d6fad962014/ruff-0.0.263-py3-none-win_arm64.whl", hash = "sha256:ddf4503595b560bfa5fae92fa2e4cb09ec465ee4cf88cc248f10ad2e956deec3"},
-    {url = "https://files.pythonhosted.org/packages/14/c9/5470c9324095f3b3f603b4f2533e89594ebdd17579f6e1111bb0712aee30/ruff-0.0.263-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:82c41f276106017b6f075dd2f2cc68e1a0b434cc75488f816fc98bd41982628d"},
-    {url = "https://files.pythonhosted.org/packages/2a/4b/bea4dc1790bff48b0f5e1fa9e0b1f6d4cdff4eb76b8aa241e4c9ac73261d/ruff-0.0.263-py3-none-win_amd64.whl", hash = "sha256:9af932f665e177de62e172901704257fd6e5bfabb95893867ff7382a851459d3"},
-    {url = "https://files.pythonhosted.org/packages/2e/8e/084839c7b3f3548f1985cdb6536770dee4dabab8f40d2ca181c1107b549a/ruff-0.0.263-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:15386933dd8e03aafa3186f9e996d6823105492817311338fbcb64d0ecbcd95f"},
-    {url = "https://files.pythonhosted.org/packages/4c/bd/0e66ad872dc598aaead4f9b8cf3e7de07ad97435448be662853dafd6d293/ruff-0.0.263-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ddcee0d91629a4fa4bc9faebf5b94d4615d50d1cd76d1098fa71fbe1c54f4104"},
-    {url = "https://files.pythonhosted.org/packages/5f/c8/8a17037c7a7a604a1eb25332a7b7e425b02c41500c13f7b1ddd8ffd46217/ruff-0.0.263-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:4f75fa1632ea065b8f10678e7b6ae9873f84d5046bdf146990112751e98af42a"},
-    {url = "https://files.pythonhosted.org/packages/61/0f/c3936d988d83bd0d6b705982779a2a254f6f1d9cc5431cb2e01e6d5c461b/ruff-0.0.263-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:04e0b280dd246448564c892bce5607d820ad1f14944f3d535db98692e2a7ac07"},
-    {url = "https://files.pythonhosted.org/packages/64/24/d4bfd6f8e08246d96f5b46f1961f7678767c62aa370a7cfeaa76c6db8c85/ruff-0.0.263-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:c3b7d4b365207f3e4c40d235127091478e595b31e35b6cd57d940920cdfae68b"},
-    {url = "https://files.pythonhosted.org/packages/74/c8/7c61be29a2d454ff1ba9f5f0ac17f3cc3ddb5f3d59219d271e549d94ccb3/ruff-0.0.263-py3-none-musllinux_1_2_i686.whl", hash = "sha256:bed1d3fba306e3f7e13ce226927b84200350e25abd1e754e06ee361c6d41de15"},
-    {url = "https://files.pythonhosted.org/packages/7a/22/8b20958ec2c03ce20b7b335ec20b27875b0890d2ab45871ee0bc7a51eeae/ruff-0.0.263-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:3e9fcee3f81129eabc75da005d839235e32d7d374f2d4c0db0c708dad4703d6e"},
-    {url = "https://files.pythonhosted.org/packages/90/48/ff8008dc66a523fc604954833ca3813bcf3265e2554af9cbeba023079de4/ruff-0.0.263-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebc778d95f29c9917e6e7608b2b67815707e6ab8eb5af9341617beda479c3edf"},
-    {url = "https://files.pythonhosted.org/packages/91/30/2c5c72c3dd7a3a2263675dcb0fd00bac6e2743d9f7e83d646342d6b15683/ruff-0.0.263-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:4010b156f2e9fa6e74b5581098467f6ff68beac48945599b3a9239481e578ab4"},
-    {url = "https://files.pythonhosted.org/packages/aa/17/cc39e9bede6626d6d2497f8034f0292c5c88c4646d95ae816ad077bedf56/ruff-0.0.263-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:7890499c2c3dcb1e60de2a8b4c5f5775b2bfcdff7d3e68e38db5cb2d65b12006"},
-    {url = "https://files.pythonhosted.org/packages/b7/cf/9b6e460cbc5e6c32433b3d95898b2b295f210bd5777e1a0425f076d335bc/ruff-0.0.263.tar.gz", hash = "sha256:1008f211ad8aa1d998517ac5bf3d68fbc68ec516d1da89b6081f25ff2f30b687"},
-    {url = "https://files.pythonhosted.org/packages/dc/30/2a44532db86e557a559284b442111d18ad1b140994f55713e9798c2a891f/ruff-0.0.263-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:981e3c4d773f7ff52479c4fd74a65e408f1e13fa5f889b72214d400cd1299ce4"},
-    {url = "https://files.pythonhosted.org/packages/ec/8e/23588cb311081bed6c1771fddfe811148a5160d2f3a80793713019c23d4b/ruff-0.0.263-py3-none-win32.whl", hash = "sha256:c2b79919ebd93674b93dfc2c843e264bf8e52fbe737467e9b58521775c85f4ad"},
-    {url = "https://files.pythonhosted.org/packages/fd/17/6f6560d8307525839dc11eca7f43a5ab652442b2945c5c31ec2f6261522b/ruff-0.0.263-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:ee6c7a77f142c427fa73e1f5f603fc1a39413a36fe6966ed0fc55e97f6921d9c"},
+"ruff 0.0.264" = [
+    {url = "https://files.pythonhosted.org/packages/1e/0e/375fde351cb0531470ad6b437cb1bbb6ce83cb0f6e01d0fd68680e3cfeff/ruff-0.0.264-py3-none-win32.whl", hash = "sha256:5a8658ebcc37d62f72840cbdf564171c1a2b6831db482b4d917962541a2f4a44"},
+    {url = "https://files.pythonhosted.org/packages/23/dc/51ee0cd6d2c3c8e0ddc6531c7a8909c5df5f5f21d091854e9ff4293a7466/ruff-0.0.264-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:d628de91e2be7a83128526636097d2dd890669a06143f826f6c591d79aeefbc4"},
+    {url = "https://files.pythonhosted.org/packages/31/84/b47957fa69018359dfbc350e28404a78f20a6cf213b580eff737784e3389/ruff-0.0.264-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:cd4f60ffc3eb15802c554a9c8581bf2117c4d3d06fbc57e0ba58f04cb1aaa47f"},
+    {url = "https://files.pythonhosted.org/packages/37/6f/4aeda64a401beecf560381961efd8a01d6d53d1e095b084b77f31e410dca/ruff-0.0.264-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:91c6eb4f979b661a2dd850d9ac803842bb7b66d4926de84f09c787af82590f73"},
+    {url = "https://files.pythonhosted.org/packages/37/f1/c4023c9dc501d7e49fe939fd86a287c02cf044be6f6cece359218c2ea025/ruff-0.0.264-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:71fd865ebacc1083259b3fb7e3eb45235a86e62e21830b8a6b067be0ec54aa2e"},
+    {url = "https://files.pythonhosted.org/packages/57/eb/ec0dd02cfd07b7f725d5ba18edcbe1f1228b89d650eb72f50049c75f1df2/ruff-0.0.264-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:04ec5d75e4bca754cedd20d53e2ba4920d6259e7579abfb2e8e30c3c80e41b17"},
+    {url = "https://files.pythonhosted.org/packages/64/a9/0ab814985bc90c19e7ac8ba53406c8f2f535739fff3a749e83a0573420ae/ruff-0.0.264-py3-none-musllinux_1_2_i686.whl", hash = "sha256:484e395d1984ab9e1e66bd42e7a5192decfee86998d07d36ee50b2fadccc8734"},
+    {url = "https://files.pythonhosted.org/packages/68/1d/f6fbf3b023b0c86c372ebe31907e18a3fc22ee3f6e00ea534e530aa48466/ruff-0.0.264-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4564e0f245eb515c6ed63988c21e9c40bcfd485cd1ec63bdd790f9a81d301f15"},
+    {url = "https://files.pythonhosted.org/packages/6a/18/9809f9c1008a9f0cf1cbfc400b46649f1631eebe4dc6f9421f7178c361f8/ruff-0.0.264-py3-none-win_arm64.whl", hash = "sha256:3e2c38449548e122f2612843a7c04e22b4fd491656955c57b8cb05df11639ad6"},
+    {url = "https://files.pythonhosted.org/packages/78/40/6a33d40d0bd48adce97775ed68b06922c95dba8076bb6db7ab320f6b9002/ruff-0.0.264-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:323ae6c1702b26c96d0fbf939c5959c37e79021f86b70f63634df918bc77f36e"},
+    {url = "https://files.pythonhosted.org/packages/8a/e0/3cc67b6f9b9f20c04f1237a6192b19343309d3c2605930ea2472eb2f81fe/ruff-0.0.264-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18a29ed37bf8cfe6dce8a2db56c313a64c0804095108753621f3c3321e0c9c5f"},
+    {url = "https://files.pythonhosted.org/packages/a3/82/2cb89c8afffb03201cbdd19529ed5b3338705d5c6fb2b76830d3d1955f17/ruff-0.0.264-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:d97ba8db0fb601ffe9ee996ebb97c698e427a2fd4514fefbe7b803111354f783"},
+    {url = "https://files.pythonhosted.org/packages/b2/95/bb0befe3eb5fc7ae4bfde2f4162323bf55136a106fd0685378c35a89e1bb/ruff-0.0.264-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:67326fdc9ac0a1b13e229c6e24e8d115863c52cd710faaaaa588851535281d6c"},
+    {url = "https://files.pythonhosted.org/packages/be/b3/bcf54b0ddf6e0e75ebe7fbe3bb1c7786647f1aac3ed60e128863129b3b4a/ruff-0.0.264-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:ec2fa192c035b8b68cc2b91049c561cd69543e2b8c4d157d9aa7727320bedcca"},
+    {url = "https://files.pythonhosted.org/packages/c2/a9/7c1b194946f1460ffbf26d9d25649c6ec4119982552936b3ce4425b7cae7/ruff-0.0.264-py3-none-win_amd64.whl", hash = "sha256:068a82a29d80848a56e3d9d4308e6e0ca8b2ecdaf5ac342a292545a59b7f2c21"},
+    {url = "https://files.pythonhosted.org/packages/c6/06/3ed1d46e1e2a71d5b88b0087a994642730e5c1396425dd31d017463e0614/ruff-0.0.264.tar.gz", hash = "sha256:8fcd4b693ca1374eb7a5796581c90689f884f98f388740d94f0702fd30f8f78f"},
+    {url = "https://files.pythonhosted.org/packages/fb/60/2f4f5170c58d70e4600d71c91e76b83a25ec31dfd2eb939e0805c1bbe6d2/ruff-0.0.264-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:05ee163a046fc593d150179d23f4af447fb82f3e59cd34e031ea0868c65bb8e8"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
```

### Comparing `xklb-1.26.20/readme.py` & `xklb-1.26.21/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.21/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.21/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/.github/workflows/push.yaml` & `xklb-1.26.21/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/av.py` & `xklb-1.26.21/xklb/av.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import sys
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Dict, Optional
 
 from xklb import subtitle, utils
 from xklb.consts import DBType
 from xklb.utils import combine, log, safe_unpack
 
 
@@ -99,16 +98,16 @@
 
 
 def munge_av_tags(args, media, f) -> Optional[dict]:
     import ffmpeg
 
     try:
         probe = ffmpeg.probe(f, show_chapters=None)
-    except (KeyboardInterrupt, SystemExit):
-        raise SystemExit(130)
+    except (KeyboardInterrupt, SystemExit) as sys_exit:
+        raise SystemExit(130) from sys_exit
     except Exception as e:
         log.error(f"[{f}] Failed reading header. Metadata corruption")
         log.debug(e)
         if args.delete_unplayable:
             utils.trash(f)
         return None
 
@@ -137,15 +136,15 @@
 
     duration = format_.pop("duration", None)
     tags = format_.pop("tags", None)
     if tags:
         upload_date = tags.get("DATE")
         if upload_date:
             try:
-                upload_date = int(datetime.strptime(upload_date, "%Y%m%d").timestamp())
+                upload_date = int(datetime.strptime(upload_date, "%Y%m%d").replace(tzinfo=timezone.utc).timestamp())
             except Exception:
                 upload_date = None
 
         tags = utils.dict_filter_bool(
             {
                 "title": tags.get("title"),
                 "webpath": tags.get("PURL"),
```

### Comparing `xklb-1.26.20/xklb/books.py` & `xklb-1.26.21/xklb/books.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import re, sys
+import re
 from typing import List, Optional
 
 from xklb import utils
 from xklb.utils import combine, log, safe_unpack
 
 REGEX_SENTENCE_ENDS = re.compile(r";|,|\.|\*|\n|\t")
 
 
 def munge_book_tags(media, f) -> Optional[dict]:
     try:
         import textract
     except ModuleNotFoundError:
-        raise ModuleNotFoundError(
+        print(
             "textract is required for text database creation: pip install textract; sudo dnf install libxml2-devel libxslt-devel antiword unrtf poppler-utils tesseract sox-plugins-nonfree sox libjpeg-devel swig",
         )
+        raise
     try:
         tags = textract.process(f)
         tags = REGEX_SENTENCE_ENDS.split(tags.decode())
     except Exception as e:
         log.warning(e)
         log.error(f"[{f}] Failed reading file")
         tags = []
@@ -206,17 +207,18 @@
     return m
 
 
 def extract_image_metadata_chunk(metadata: List[dict]) -> List[dict]:
     try:
         import exiftool
     except ModuleNotFoundError:
-        raise ModuleNotFoundError(
+        print(
             "exiftool and PyExifTool are required for image database creation: sudo dnf install perl-Image-ExifTool && pip install PyExifTool",
         )
+        raise
 
     chunk_paths = [d["path"] for d in metadata]
     with exiftool.ExifToolHelper() as et:
         exif = et.get_metadata(chunk_paths)
 
     exif_enriched = []
     for m, e in zip(metadata, exif):
```

### Comparing `xklb-1.26.20/xklb/consts.py` & `xklb-1.26.21/xklb/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 
 def now():
     return int(datetime.now(tz=timezone.utc).timestamp())
 
 
 TEMP_DIR = gettempdir()
-FAKE_SUBTITLE = os.path.join(TEMP_DIR, "sub.srt")  # https://github.com/skorokithakis/catt/issues/393
-CAST_NOW_PLAYING = os.path.join(TEMP_DIR, "catt_playing")
-DEFAULT_MPV_SOCKET = os.path.join(TEMP_DIR, "mpv_socket")
+FAKE_SUBTITLE = Path(TEMP_DIR) / "sub.srt"  # https://github.com/skorokithakis/catt/issues/393
+CAST_NOW_PLAYING = Path(TEMP_DIR) / "catt_playing"
+DEFAULT_MPV_SOCKET = Path(TEMP_DIR) / "mpv_socket"
 DEFAULT_MPV_WATCH_LATER = str(Path("~/.config/mpv/watch_later/").expanduser().resolve())
-SUB_TEMP_DIR = os.path.join(TEMP_DIR, "library_temp_subtitles")
+SUB_TEMP_DIR = Path(TEMP_DIR) / "library_temp_subtitles"
 BLOCK_THE_CHANNEL = "__BLOCKLIST_ENTRY_"
 
 LOG_INFO = 1
 LOG_DEBUG = 2
 SIMILAR = 1
 SIMILAR_NO_FILTER = 2
 SIMILAR_NO_FILTER_NO_FTS = 2
```

### Comparing `xklb-1.26.20/xklb/db.py` & `xklb-1.26.21/xklb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import sqlite3
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Union
 
 from xklb import consts, utils
 from xklb.utils import log
 
+if TYPE_CHECKING:
+    from sqlite_utils import Database
+
 
 def tracer(sql, params) -> None:
     sql = utils.remove_consecutives(dedent(sql), "\n")
     log.info(f"SQL: {sql} - params: {params}")
 
 
 def connect(args, conn=None, **kwargs):
     from sqlite_utils import Database
 
-    sqlite3.enable_callback_tracebacks(True)
+    sqlite3.enable_callback_tracebacks(True)  # noqa: FBT003
 
     class DB(Database):
         def pop(self, sql: str, params: Optional[Union[Iterable, dict]] = None, ignore_errors=None) -> Optional[Any]:
             if ignore_errors is None:
                 ignore_errors = ["no such table"]
             try:
                 curs = self.execute(sql, params)
@@ -39,18 +42,18 @@
             ignore_errors=None,
         ) -> Optional[Dict]:
             if ignore_errors is None:
                 ignore_errors = ["no such table"]
             try:
                 dg = self.query(sql, params)
                 d = next(dg, None)
-            except sqlite3.OperationalError as exc:
-                if any(e in str(exc) for e in ignore_errors):
+            except sqlite3.OperationalError as e:
+                if any(ignore_error in str(e) for ignore_error in ignore_errors):
                     return None
-                raise exc
+                raise
             return d
 
     if kwargs.get("memory"):
         db = DB(tracer=tracer if args.verbose >= consts.LOG_DEBUG else None, **kwargs)  # type: ignore
         return db
 
     if not Path(args.database).exists() and ":memory:" not in args.database:
@@ -66,15 +69,14 @@
 
 
 def optimize(args) -> None:
     if not hasattr(args, "force"):
         args.force = False
 
     log.info("\nOptimizing database")
-    from sqlite_utils import Database
 
     db: Database = args.db
 
     config = {
         "media": {
             "search_columns": ["path", "title", "tags", "mood", "genre", "description", "artist", "album"],
             "column_order": ["path", "webpath", "id", "ie_key", "playlist_path"],
@@ -109,16 +111,16 @@
 
     for table in config:
         if table not in db.table_names():
             continue
         if args.force:
             try:
                 db[table].disable_fts()  # type: ignore
-            except Exception:
-                pass
+            except Exception as e:
+                log.debug(e)
 
         log.info("Processing table: %s", table)
         table_columns = db[table].columns_dict
         table_config = config.get(table) or {}
         ignore_columns = table_config.get("ignore_columns") or []
         search_columns = table_config.get("search_columns") or []
```

### Comparing `xklb-1.26.20/xklb/dl_config.py` & `xklb-1.26.21/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/dl_extract.py` & `xklb-1.26.21/xklb/dl_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,22 +39,22 @@
         help="Use image downloader",
     )
 
     parser.add_argument(
         "--dl-config",
         "-dl-config",
         nargs=1,
-        action=utils.argparse_dict,
+        action=utils.ArgparseDict,
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
-    parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.argparse_dict, metavar="KEY=VALUE")
-    parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.argparse_dict, metavar="KEY=VALUE")
+    parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
+    parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
 
     parser.add_argument("--prefix", default=os.getcwd(), help=argparse.SUPPRESS)
     parser.add_argument("--ext", default="DEFAULT")
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
     parser.add_argument("--cols", "-cols", "-col", nargs="*", help=argparse.SUPPRESS)
@@ -283,17 +283,17 @@
         if download_already_attempted:
             log.info("[%s]: Already downloaded. Skipping!", m["path"])
             continue
 
         if args.profile in (DBType.audio, DBType.video):
             try:
                 tube_backend.yt(args, m)
-            except Exception as e:
+            except Exception:
                 print("db:", args.database)
-                raise e
+                raise
         else:
             raise NotImplementedError
 
 
 def dl_block(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
@@ -310,15 +310,15 @@
     Use with the all-deleted-playlists flag to delete any previously downloaded files from the playlist uploader
 
         library block dl.db --all-deleted-playlists https://annoyingwebsite/etc/
     """,
     )
 
     if not any([args.playlists, args.all_deleted_playlists]):
-        raise Exception("Specific URLs or --all-deleted-playlists must be supplied")
+        raise RuntimeError("Specific URLs or --all-deleted-playlists must be supplied")
 
     log.info(utils.dict_filter_bool(args.__dict__))
     args.category = consts.BLOCK_THE_CHANNEL
     args.extra_playlist_data = {"time_deleted": consts.APPLICATION_START}
     args.extra_media_data = {"time_deleted": consts.APPLICATION_START}
     for p in args.playlists:
         tube_backend.process_playlist(args, p, tube_backend.tube_opts(args, func_opts={"playlistend": 30}))
```

### Comparing `xklb-1.26.20/xklb/fs_extract.py` & `xklb-1.26.21/xklb/fs_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
         elif args.profile == DBType.video:
             args.database = "video.db"
         elif args.profile == DBType.text:
             args.database = "text.db"
         elif args.profile == DBType.image:
             args.database = "image.db"
         else:
-            raise Exception(f"fs_extract for profile {args.profile} not implemented")
+            msg = f"fs_extract for profile {args.profile}"
+            raise NotImplementedError(msg)
 
     if args.db:
         args.database = args.db
     Path(args.database).touch()
     args.db = db.connect(args)
     if hasattr(args, "paths"):
         args.paths = utils.conform(args.paths)
@@ -151,29 +152,27 @@
     if hasattr(stat, "st_blocks"):
         media = {**media, "sparseness": calculate_sparseness(stat)}
 
     if mp_args.profile == DBType.filesystem:
         media = {**media, "is_dir": Path(f).is_dir()}
 
     if mp_args.profile in (DBType.audio, DBType.video):
-        return av.munge_av_tags(mp_args, media, f)
+        media = av.munge_av_tags(mp_args, media, f)
 
     if mp_args.profile == DBType.text:
         try:
             start = timer()
             if any([mp_args.ocr, mp_args.speech_recognition]):
                 media = books.munge_book_tags_slow(media, f)
             else:
                 media = books.munge_book_tags_fast(media, f)
         except mp_TimeoutError:
             log.warning(f"[{f}]: Timed out trying to read file")
-            return media
         else:
             log.debug(f"[{f}]: {timer()-start}")
-            return media
 
     return media
 
 
 def clean_up_temp_dirs():
     temp_subs_path = Path(consts.SUB_TEMP_DIR)
     if temp_subs_path.exists():
@@ -200,20 +199,23 @@
             scanned_files = [str(p) for p in path.rglob("*")]
         elif args.profile == DBType.audio:
             scanned_files = consts.get_audio_files(path)
         elif args.profile == DBType.video:
             scanned_files = consts.get_video_files(path)
         elif args.profile == DBType.text:
             scanned_files = consts.get_text_files(
-                path, image_recognition=args.ocr, speech_recognition=args.speech_recognition
+                path,
+                image_recognition=args.ocr,
+                speech_recognition=args.speech_recognition,
             )
         elif args.profile == DBType.image:
             scanned_files = consts.get_image_files(path)
         else:
-            raise Exception(f"fs_extract for profile {args.profile} not implemented")
+            msg = f"fs_extract for profile {args.profile}"
+            raise NotImplementedError(msg)
     except FileNotFoundError:
         print(f"[{path}] Not found")
         return []
 
     columns = args.db["media"].columns_dict
     scanned_set = set(scanned_files)
 
@@ -227,15 +229,14 @@
                     and path like '{path}%'
                     {'AND time_downloaded > 0' if 'time_downloaded' in columns else ''}
                 """,
             )
         }
     except Exception as e:
         log.debug(e)
-        pass
     else:
         undeleted_files = list(deleted_set.intersection(scanned_set))
         undeleted_count = player.mark_media_undeleted(args, undeleted_files)
         if undeleted_count > 0:
             print(f"[{path}] Marking", undeleted_count, "metadata records as undeleted")
 
     try:
@@ -336,17 +337,18 @@
 def extractor(args, paths) -> None:
     new_files = 0
     for path in paths:
         new_files += scan_path(args, path)
 
     log.info("Imported %s paths", new_files)
 
-    if args.profile in [DBType.audio, DBType.video, DBType.text]:
-        if not args.db["media"].detect_fts() or new_files > 100000:
-            db.optimize(args)
+    if args.profile in [DBType.audio, DBType.video, DBType.text] and (
+        not args.db["media"].detect_fts() or new_files > 100000
+    ):
+        db.optimize(args)
 
 
 def fs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args = parse_args(
```

### Comparing `xklb-1.26.20/xklb/gui.py` & `xklb-1.26.21/xklb/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
 
 class MrSuperDialogue:
     def __init__(self, path, qty, geom_data=None, true_action="keep", false_action="delete") -> None:
         from tkinter import PhotoImage, Tk
         from tkinter.ttk import Button, Frame, Label, Style
 
-        def raise_error(self, *args):
+        def raise_error(_self, *_args):
             raise  # pylint: disable=misplaced-bare-raise
 
         Tk.report_callback_exception = raise_error
 
         self.root = Tk()
         self.root.title("Library dialogue")
         self.root.wm_attributes("-alpha", 0)
 
         style = Style(self.root)
         style.theme_use("clam")
 
         photo = PhotoImage(file="assets/kotobago.png")
-        self.root.wm_iconphoto(False, photo)
+        self.root.wm_iconphoto(True, photo)  # noqa: FBT003
         self.root.wm_attributes("-topmost", 1)
 
         for keyseq in ("<Escape>", "<Control-c>", "<Control-q>"):
             self.root.bind(keyseq, lambda _ev: self.user_quit())
 
         # menu left
         self.menu_left = Frame(self.root, width=150)
@@ -137,15 +137,15 @@
         # monitors to find the pixel offset within the framebuffer for the window to show up in
         # that monitor but I have some doubts about whether this will work at all as well as
         # the portability of this solution. I cycle through five different monitors throughout
         # the day but I never use more than one simultaneously so I will stop over-optimizing here:
         raise NotImplementedError
 
     @staticmethod
-    def get_monitor_from_coord(coord_x, coord_y):
+    def get_monitor_from_coord(coord_x, coord_y):  # noqa: ANN205; -> Monitor
         import screeninfo
 
         monitors = screeninfo.get_monitors()
 
         for m in reversed(monitors):
             if m.x <= coord_x <= m.width + m.x and m.y <= coord_y <= m.height + m.y:
                 return m
```

### Comparing `xklb-1.26.20/xklb/hn_extract.py` & `xklb-1.26.21/xklb/hn_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     return args
 
 
 def get(url):
     import requests
 
-    r = requests.get(url)
+    r = requests.get(url, timeout=120)
     return r.json()
 
 
 def db_worker(args, input_queue):
     conn = sqlite3.connect(args.database, isolation_level=None)
     db_conn = db.connect(args, conn)
     while True:
@@ -129,17 +129,17 @@
     Fetch oldest stories first:
 
         library hnadd --oldest hn.db
     """,
     )
     try:
         import aiohttp
-    except ModuleNotFoundError as e:
+    except ModuleNotFoundError:
         log.error("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[full]")
-        raise e
+        raise
 
     args.db.enable_wal()
 
     max_item_id = get("https://hacker-news.firebaseio.com/v0/maxitem.json")
     tables = args.db.table_names()
     r = list(
         args.db.query(
```

### Comparing `xklb-1.26.20/xklb/lb.py` & `xklb-1.26.21/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/play_actions.py` & `xklb-1.26.21/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,17 +645,17 @@
         catt_log = player.listen_chromecast(args, m)
     else:
         raise NotImplementedError
 
     if catt_log:
         if catt_log.stderr is None or catt_log.stderr == "":
             if not args.cast_with_local:
-                raise Exception("catt does not exit nonzero? but something might have gone wrong")
+                raise RuntimeError("catt does not exit nonzero? but something might have gone wrong")
         elif "Heartbeat timeout, resetting connection" in catt_log.stderr:
-            raise Exception("Media is possibly partially unwatched")
+            raise RuntimeError("Media is possibly partially unwatched")
 
 
 def is_play_in_order_lvl2(args, media_file) -> bool:
     return any(
         [
             args.play_in_order >= consts.SIMILAR,
             args.action == SC.listen and "audiobook" in media_file.lower(),
@@ -735,19 +735,19 @@
 
     args.player = player.parse(args, m)
 
     start_time = time.time()
     if args.chromecast:
         try:
             chromecast_play(args, m)
-        except Exception as e:
+        except Exception:
             if args.ignore_errors:
                 return
             else:
-                raise e
+                raise
 
     elif args.interdimensional_cable:
         player.socket_play(args, m)
         return
 
     else:
         r = player.local_player(args, m)
```

### Comparing `xklb-1.26.20/xklb/playback.py` & `xklb-1.26.21/xklb/playback.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
 def _now_playing(args) -> dict:
     media = {
-        "catt": Path(consts.CAST_NOW_PLAYING).read_text() if os.path.exists(consts.CAST_NOW_PLAYING) else None,
-        "mpv": args.mpv.command("get_property", "path") if os.path.exists(args.mpv_socket) else None,
+        "catt": Path(consts.CAST_NOW_PLAYING).read_text() if Path(consts.CAST_NOW_PLAYING).exists() else None,
+        "mpv": args.mpv.command("get_property", "path") if Path(args.mpv_socket).exists() else None,
     }
     log.info(media)
     return media
 
 
 def indent_prefix_first(text, prefix, indent="\t"):
     lines = text.splitlines()
```

### Comparing `xklb-1.26.20/xklb/player.py` & `xklb-1.26.21/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import csv, operator, os, platform, re, shutil, socket, subprocess, sys
+import csv, operator, os, platform, re, shutil, socket, subprocess
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 from platform import system
 from random import randrange
 from shlex import join, quote, split
@@ -75,15 +75,15 @@
     mimetype = cmd("xdg-mime", "query", "filetype", media_file).stdout
     default_application = cmd("xdg-mime", "query", "default", mimetype).stdout
     return which(default_application.replace(".desktop", ""))
 
 
 def parse(args, m) -> List[str]:
     player = generic_player(args)
-    mpv = which("mpv.com") or which("mpv")
+    mpv = which("mpv.com") or which("mpv") or "mpv"
 
     if args.override_player:
         player = args.override_player
         args.player_need_sleep = False
 
     elif args.action in (SC.read) and m["path"]:
         player_path = find_xdg_application(m["path"])
@@ -349,20 +349,20 @@
     elif action.startswith("ask_"):
         handle_ask_action(action)
     else:
         raise ValueError("Unrecognized action:", action)
 
 
 def override_sort(sort_expression: str) -> str:
-    def YEAR_MONTH(var):
+    def year_month_sql(var):
         return f"cast(strftime('%Y%m', datetime({var}, 'unixepoch')) as int)"
 
     return (
-        sort_expression.replace("month_created", YEAR_MONTH("time_created"))
-        .replace("month_modified", YEAR_MONTH("time_modified"))
+        sort_expression.replace("month_created", year_month_sql("time_created"))
+        .replace("month_modified", year_month_sql("time_modified"))
         .replace("random", "random()")
         .replace("priority", "ntile(1000) over (order by size) desc, duration")
     )
 
 
 def last_chars(candidate) -> str:
     remove_groups = re.split(r"([\W]+|\s+|Ep\d+|x\d+|\.\d+)", candidate)
@@ -457,48 +457,50 @@
             catt_log = args.cc.play_url(m["path"], resolve=True, block=True)
     return catt_log
 
 
 def listen_chromecast(args, m: dict) -> Optional[subprocess.CompletedProcess]:
     Path(consts.CAST_NOW_PLAYING).write_text(m["path"])
     Path(consts.FAKE_SUBTITLE).touch()
+    catt = which("catt") or "catt"
     if args.cast_with_local:
         cast_process = subprocess.Popen(
-            ["catt", "-d", args.chromecast_device, "cast", "-s", consts.FAKE_SUBTITLE, m["path"]],
+            [catt, "-d", args.chromecast_device, "cast", "-s", consts.FAKE_SUBTITLE, m["path"]],
             **utils.os_bg_kwargs(),
         )
         sleep(0.974)  # imperfect lazy sync; I use keyboard shortcuts to send `set speed` commands to mpv for resync
         # if pyChromecast provides a way to sync accurately that would be very interesting to know; I have not researched it
         cmd_interactive(*args.player, "--", m["path"])
         catt_log = utils.Pclose(cast_process)  # wait for chromecast to stop (you can tell any chromecast to pause)
         sleep(3.0)  # give chromecast some time to breathe
     else:
         if m["path"].startswith("http"):
             catt_log = args.cc.play_url(m["path"], resolve=True, block=True)
         else:  #  local file
-            catt_log = cmd("catt", "-d", args.chromecast_device, "cast", "-s", consts.FAKE_SUBTITLE, m["path"])
+            catt_log = cmd(catt, "-d", args.chromecast_device, "cast", "-s", consts.FAKE_SUBTITLE, m["path"])
 
     return catt_log
 
 
 def socket_play(args, m: dict) -> None:
+    mpv = which("mpv") or "mpv"
     if args.sock is None:
-        subprocess.Popen(["mpv", "--idle", "--input-ipc-server=" + args.mpv_socket])
-        while not os.path.exists(args.mpv_socket):
+        subprocess.Popen([mpv, "--idle", "--input-ipc-server=" + args.mpv_socket])
+        while not Path(args.mpv_socket).exists():
             sleep(0.2)
         args.sock = socket.socket(socket.AF_UNIX)
         args.sock.connect(args.mpv_socket)
 
     start, end = calculate_duration(args, m)
 
     try:
         start = randrange(int(start), int(end - args.interdimensional_cable + 1))
         end = start + args.interdimensional_cable
-    except Exception:
-        pass
+    except Exception as e:
+        log.info(e)
     if end == 0:
         return
 
     play_opts = f"start={start},save-position-on-quit=no"
     if args.action in (SC.listen):
         play_opts += ",video=no,really-quiet=yes"
     elif args.action in (SC.watch):
@@ -550,15 +552,16 @@
 
 def get_display_by_name(displays, screen_name):  # noqa: ANN201; -> List[screeninfo.Monitor]
     for d in displays:
         if d.name == screen_name:
             return [d]
 
     display_names = '", "'.join([d.name for d in displays])
-    raise Exception(f'Display "{screen_name}" not found. I see: "{display_names}"')
+    msg = f'Display "{screen_name}" not found. I see: "{display_names}"'
+    raise ValueError(msg)
 
 
 def is_hstack(args, display) -> bool:
     if args.hstack or args.portrait:
         return True
     elif args.vstack:
         return False
@@ -723,15 +726,15 @@
     if "f" in args.print:
         if args.limit == 1:
             f = media[0]["path"]
             if not Path(f).exists():
                 mark_media_deleted(args, f)
                 raise FileNotFoundError
             utils.pipe_print(quote(f))
-            return None
+            return
         else:
             if not args.cols:
                 args.cols = ["path"]
 
             selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
             virtual_csv = StringIO()
             wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
@@ -742,16 +745,16 @@
             for line in virtual_csv.readlines():
                 if args.moved:
                     utils.pipe_print(line.strip().replace(args.moved[0], "", 1))
                 else:
                     utils.pipe_print(line.strip())
             if args.moved:
                 moved_media(args, list(map(operator.itemgetter("path"), media)), *args.moved)
-                return None
-            return None
+                return
+            return
     else:
         tbl = deepcopy(media)
         utils.col_resize(tbl, "path", 22)
         utils.col_resize(tbl, "title", 11)
 
         utils.col_naturalsize(tbl, "size")
         utils.col_naturalsize(tbl, "avg_size")
@@ -767,17 +770,17 @@
             print(f"{len(media)} media" + (f" (limited to {args.limit})" if args.limit else ""))
 
         duration = sum(m.get("duration") or 0 for m in media)
         if duration > 0:
             duration = human_time(duration)
             if "a" not in args.print:
                 print("Total duration:", duration)
-                return None
-            return None
-        return None
+                return
+            return
+        return
 
 
 def printer(args, query, bindings) -> None:
     media = list(args.db.query(query, bindings))
     try:
         media_printer(args, media)
     except FileNotFoundError:
```

### Comparing `xklb-1.26.20/xklb/praw_extract.py` & `xklb-1.26.21/xklb/praw_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import datetime as dt
 import json
 import sys
 from functools import partial
 from itertools import takewhile
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
 from xklb import consts, db, utils
 from xklb.utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
@@ -30,14 +30,18 @@
 - Linux or Mac OS: ~/.config/praw.ini
 - Windows: %APPDATA%\praw.ini
 
 More details: https://praw.readthedocs.io/en/stable/getting_started/configuration/prawini.html
 """
 
 
+if TYPE_CHECKING:
+    import praw
+
+
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library " + action,
         usage=usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--limit", default=1000, type=int)
@@ -67,15 +71,15 @@
 
     try:
         import praw
 
         args.reddit = praw.Reddit(args.praw_site, config_interpolation="basic")
     except Exception as e:
         print(PRAW_SETUP_INSTRUCTIONS)
-        raise SystemExit(e)
+        raise SystemExit(e) from e
 
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
 """
@@ -105,20 +109,20 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
-def created_since(row: Any, target_sec_utc: Optional[int]) -> bool:
+def created_since(row, target_sec_utc: Optional[int]) -> bool:
     result = (not target_sec_utc) or (row.created_utc >= target_sec_utc)
     return result
 
 
-def legalize(val: Any) -> Any:
+def legalize(val):
     import praw
 
     if isinstance(val, praw.models.reddit.base.RedditBase):  # type: ignore
         return str(val)
     if isinstance(val, praw.models.reddit.poll.PollData):  # type: ignore
         d = val.__dict__
         d.pop("_reddit", None)
@@ -135,15 +139,15 @@
     if prefix == "t1_":
         dct["parent_comment_id"] = dct["parent_clean_id"]
     elif prefix == "t3_":
         dct["parent_post_id"] = dct["parent_clean_id"]
     return dct
 
 
-def saveable(item: Any) -> Dict[str, Any]:
+def saveable(item) -> Dict[str, Any]:
     result = {k: legalize(v) for k, v in item.__dict__.items() if not k.startswith("_")}
     return _parent_ids_interpreted(result)
 
 
 def slim_post_data(d: dict, playlist_path=None) -> dict:
     skip_domains = ["linktr.ee", "twitter.com", "t.me", "patreon", "onlyfans", "fans.ly", "file-upload", "file-link"]
     url = d.get("url")
@@ -241,30 +245,26 @@
         log.info("Getting posts since the dawn of time...")
 
     _takewhile = partial(created_since, target_sec_utc=get_since)
     return _takewhile
 
 
 def redditor_new(args, redditor_dict) -> None:
-    import praw
-
     user_path, user_name = redditor_dict.values()
     user: praw.reddit.Redditor = args.reddit.redditor(user_name)
 
     _takewhile = since_last_created(args, user_path)
     log.info("Getting new posts")
 
     for s in takewhile(_takewhile, user.submissions.new(limit=args.limit)):
         s.time_created = s.created_utc
         save_post(args, saveable(s), user_path)
 
 
 def subreddit_new(args, subreddit_dict) -> None:
-    import praw
-
     subreddit_path, subreddit_name = subreddit_dict.values()
     subreddit: praw.reddit.Subreddit = args.reddit.subreddit(subreddit_name)
 
     _takewhile = since_last_created(args, subreddit_path)
     log.info("Getting new posts")
     for idx, post in enumerate(takewhile(_takewhile, subreddit.new(limit=args.limit))):
         post_dict = saveable(post)
@@ -282,16 +282,14 @@
                 alter=True,
             )
 
         save_post(args, post_dict, subreddit_path)
 
 
 def subreddit_top(args, subreddit_dict) -> None:
-    import praw
-
     subreddit_path, subreddit_name = subreddit_dict.values()
 
     subreddit: praw.reddit.Subreddit = args.reddit.subreddit(subreddit_name)
 
     time_filters = ["all", "year", "month", "week", "day", "hour"]
     if args.lookback in [1, 2]:
         time_filters.reverse()
```

### Comparing `xklb-1.26.20/xklb/stats.py` & `xklb-1.26.21/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/subtitle.py` & `xklb-1.26.21/xklb/subtitle.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Path(SUB_TEMP_DIR).mkdir(parents=True, exist_ok=True)
     temp_srt = tempfile.mktemp(".srt", dir=SUB_TEMP_DIR)
     try:
         ffmpeg.input(path).output(temp_srt).global_args("-nostdin").run(quiet=True)
     except Error as e:
         log.info("Could not convert subtitle")
         log.info(e.stderr.decode())
-        raise UnicodeDecodeError("utf-8", b"Dr. John A. Zoidberg", 1, 2, "Bleh!")
+        raise UnicodeDecodeError("utf-8", b"Dr. John A. Zoidberg", 1, 2, "Bleh!") from e
 
     return temp_srt
 
 
 def read_sub_unsafe(path) -> List[str]:
     import pysubs2
```

### Comparing `xklb-1.26.20/xklb/tabs_actions.py` & `xklb-1.26.21/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/tabs_extract.py` & `xklb-1.26.21/xklb/tabs_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse, sys
 from pathlib import Path
 from typing import List
 
 from xklb import consts, db, player, utils
 from xklb.consts import Frequency
-from xklb.utils import argparse_enum, log, sanitize_url
+from xklb.utils import ArgparseEnum, log, sanitize_url
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabsadd",
         usage=r"""library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--category CATEGORY] [--no-sanitize] DATABASE URLS ...
 
@@ -32,15 +32,15 @@
     )
     parser.add_argument(
         "--frequency",
         "--freqency",
         "-f",
         default=Frequency.Monthly,
         type=Frequency,
-        action=argparse_enum,
+        action=ArgparseEnum,
         help=argparse.SUPPRESS,
     )
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
@@ -72,16 +72,16 @@
         qb = (
             "select path from media where category = ? and path in (" + ",".join(["?"] * len(args.paths)) + ")",
             (args.category, *args.paths),
         )
 
     try:
         existing = {d["path"] for d in args.db.query(*qb)}
-    except Exception:
-        pass
+    except Exception as e:
+        log.debug(e)
     else:
         if existing:
             print(f"Updating frequency for {len(existing)} existing paths")
             player.mark_media_deleted(args, list(existing))
 
     args.paths = utils.conform([path.strip() for path in args.paths])
     return args.paths
```

### Comparing `xklb-1.26.20/xklb/tube_backend.py` & `xklb-1.26.21/xklb/tube_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse, json, sys
 from copy import deepcopy
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 from types import ModuleType
 from typing import Dict, List, Optional, Tuple
 
 from xklb import consts, fs_extract, utils
 from xklb.consts import DBType
 from xklb.dl_config import (
@@ -160,29 +160,31 @@
 
     return any(ie.suitable(url) and ie.IE_NAME != "generic" for ie in is_supported.yt_ies)
 
 
 def is_playlist_known(args, playlist_path) -> bool:
     try:
         known = args.db.execute("select 1 from playlists where path=?", [playlist_path]).fetchone()
-    except Exception:
+    except Exception as e:
+        log.debug(e)
         return False
     if known is None:
         return False
     return True
 
 
 def is_video_known(args, playlist_path, path) -> bool:
     m_columns = args.db["media"].columns_dict
     try:
         known = args.db.execute(
             f"select 1 from media where playlist_path=? and (path=? or {'web' if 'webpath' in m_columns else ''}path=?)",
             [playlist_path, path, path],
         ).fetchone()
-    except Exception:
+    except Exception as e:
+        log.debug(e)
         return False
     if known is None:
         return False
     return True
 
 
 def consolidate(v: dict) -> Optional[dict]:
@@ -193,15 +195,15 @@
         if k.startswith("_") or k in consts.TUBE_IGNORE_KEYS:
             v.pop(k, None)
 
     release_date = v.pop("release_date", None)
     upload_date = v.pop("upload_date", None) or release_date
     if upload_date:
         try:
-            upload_date = int(datetime.strptime(upload_date, "%Y%m%d").timestamp())
+            upload_date = int(datetime.strptime(upload_date, "%Y%m%d").replace(tzinfo=timezone.utc).timestamp())
         except Exception:
             upload_date = None
 
     cv = {}
     cv["path"] = safe_unpack(v.pop("webpage_url", None), v.pop("url", None), v.pop("original_url", None))
     size_bytes = v.pop("filesize_approx", None)
     cv["size"] = 0 if not size_bytes else int(size_bytes)
@@ -487,16 +489,16 @@
         "error": error,
     }
     args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)  # type: ignore
 
     if fs_tags:
         try:
             args.db["media"].delete(webpath)  # from sqlite_utils.db import NotFoundError
-        except Exception:
-            pass
+        except Exception as e:
+            log.debug(e)
 
 
 def yt(args, m) -> None:
     yt_dlp = load_module_level_yt_dlp()
 
     if not m["path"].startswith("http"):
         return
```

### Comparing `xklb-1.26.20/xklb/tube_extract.py` & `xklb-1.26.21/xklb/tube_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
         "--dl-config",
         "-dl-config",
         nargs=1,
-        action=utils.argparse_dict,
+        action=utils.ArgparseDict,
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
```

### Comparing `xklb-1.26.20/xklb/utils.py` & `xklb-1.26.21/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,16 @@
         if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
             sys.excepthook = ultratb.FormattedTB(
                 mode="Context",
                 color_scheme="Neutral",
                 call_pdb=True,
                 debugger_cls=TerminalPdb,
             )
-        else:
-            pass
-    except Exception:
-        pass
+    except Exception as e:
+        log.debug(e)
 
     log_levels = [logging.WARNING, logging.INFO, logging.DEBUG]
     logging.root.handlers = []  # clear any existing handlers
     logging.basicConfig(
         level=log_levels[min(len(log_levels) - 1, args.verbose)],
         format="%(message)s",
         handlers=[RichHandler(show_time=False, show_level=False, show_path=False)],
@@ -170,25 +168,26 @@
             capture_output=True,
             text=True,
             cwd=cwd,
             errors=sys.getfilesystemencodeerrors(),
             **os_bg_kwargs(),
             **kwargs,
         )
-    except UnicodeDecodeError as e:
+    except UnicodeDecodeError:
         print(repr(command))
-        raise e
+        raise
 
     log.debug(r.args)
     r.stdout = print_std(r.stdout)
     r.stderr = print_std(r.stderr)
     if r.returncode != 0:
         log.info("[%s]: ERROR %s", shlex.join(command), r.returncode)
         if strict:
-            raise Exception(f"[{command}] exited {r.returncode}")
+            msg = f"[{command}] exited {r.returncode}"
+            raise RuntimeError(msg)
 
     return r
 
 
 def timeout(minutes) -> None:
     if minutes and float(minutes) > 0:
         seconds = int(float(minutes) * 60)
@@ -239,25 +238,27 @@
 
 
 def cmd_interactive(*command) -> subprocess.CompletedProcess:
     return_code = os.spawnvpe(os.P_WAIT, command[0], command, os.environ)
     return subprocess.CompletedProcess(command, return_code)
 
 
-def Pclose(process) -> subprocess.CompletedProcess:
+def Pclose(process) -> subprocess.CompletedProcess:  # noqa: N802
     try:
         stdout, stderr = process.communicate(input)
     except subprocess.TimeoutExpired as exc:
+        log.debug("subprocess.TimeoutExpired")
         process.kill()
         if platform.system() == "Windows":
             exc.stdout, exc.stderr = process.communicate()
         else:
             process.wait()
         raise
-    except Exception:
+    except Exception as e:
+        log.debug(e)
         process.kill()
         raise
     return_code = process.poll()
     return subprocess.CompletedProcess(process.args, return_code, stdout, stderr)
 
 
 def file_temp_copy(src) -> str:
@@ -659,32 +660,33 @@
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = human_time(tbl[idx][col])
 
     col_resize(tbl, "duration", 6)
     return tbl
 
 
-class argparse_dict(argparse.Action):
+class ArgparseDict(argparse.Action):
     def __call__(self, parser, args, values, option_string=None):
         try:
             d = {}
             k_eq_v = list(flatten([val.split(" ") for val in values]))
             for s in k_eq_v:
                 k, v = s.split("=")
                 if any(sym in v for sym in ("[", "{")):
                     d[k] = literal_eval(v)
                 else:
                     d[k] = v
 
         except ValueError as ex:
-            raise argparse.ArgumentError(self, f'Could not parse argument "{values}" as k1=1 k2=2 format {ex}')
+            msg = f'Could not parse argument "{values}" as k1=1 k2=2 format {ex}'
+            raise argparse.ArgumentError(self, msg) from ex
         setattr(args, self.dest, d)
 
 
-class argparse_enum(argparse.Action):
+class ArgparseEnum(argparse.Action):
     def __init__(self, **kwargs) -> None:
         # Pop off the type value
         enum_type = kwargs.pop("type", None)
 
         # Ensure an Enum subclass is provided
         if enum_type is None:
             raise ValueError("type must be assigned an Enum when using EnumAction")
```

### Comparing `xklb-1.26.20/xklb/scripts/__init__.py` & `xklb-1.26.21/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/bigdirs.py` & `xklb-1.26.21/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/christen.py` & `xklb-1.26.21/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/copy_play_counts.py` & `xklb-1.26.21/xklb/scripts/copy_play_counts.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,50 +31,46 @@
 
     return args
 
 
 def copy_play_count(args, source_db) -> None:
     args.db.attach("src", Path(source_db).resolve())
 
-    modified_row_count = 0
-    with args.db.conn:
-        sql = f"""
-        UPDATE
-            main.media
-        SET play_count = (
-                SELECT
-                    play_count
-                FROM
-                    src.media
-                WHERE
-                    main.media.path = REPLACE(src.media.path, :source_prefix, :target_prefix)
-            ),
-            time_played = (
-                SELECT
-                    time_played
-                FROM
-                    src.media
-                WHERE
-                    main.media.path = REPLACE(src.media.path, :source_prefix, :target_prefix)
+    for col in ["play_count", "time_played"]:
+        modified_row_count = 0
+        with args.db.conn:
+            sql = f"""
+            UPDATE
+                main.media
+            SET
+                {col} = (
+                    SELECT
+                        {col}
+                    FROM
+                        src.media
+                    WHERE
+                        main.media.path = REPLACE(src.media.path, :source_prefix, :target_prefix)
+                )
+            WHERE
+                EXISTS(
+                    SELECT
+                        1
+                    FROM
+                        src.media
+                    WHERE
+                        main.media.path = REPLACE(src.media.path, :source_prefix, :target_prefix)
+                        AND src.media.play_count > 0
+                );
+            """
+            cursor = args.db.conn.execute(
+                sql, {"source_prefix": args.source_prefix, "target_prefix": args.target_prefix}
             )
-        WHERE
-            EXISTS(
-                SELECT
-                    1
-                FROM
-                    src.media
-                WHERE
-                    main.media.path = REPLACE(src.media.path, :source_prefix, :target_prefix)
-                    AND src.media.play_count > 0
-            );
-        """
-        cursor = args.db.conn.execute(sql, {"source_prefix": args.source_prefix, "target_prefix": args.target_prefix})
-        modified_row_count += cursor.rowcount
+            modified_row_count += cursor.rowcount
 
-    log.info("Updated %s rows", modified_row_count)
+        log.info("Updated %s rows (%s)", modified_row_count, col)
 
 
 def copy_play_counts() -> None:
     args = parse_args()
     for s_db in args.source_dbs:
         copy_play_count(args, s_db)
```

### Comparing `xklb-1.26.20/xklb/scripts/dedupe.py` & `xklb-1.26.21/xklb/scripts/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     try:
         import pandas as pd
 
         csv_path = tempfile.mktemp(".csv")
         pd.DataFrame(duplicates).to_csv(csv_path, index=False)
         print("Full list saved to:", csv_path)
     except ModuleNotFoundError:
-        pass
+        log.info("Skipping CSV export because pandas is not installed")
 
     duplicates_size = sum(filter(None, map(operator.itemgetter("duplicate_size"), duplicates)))
     print(f"Approx. space savings: {humanize.naturalsize(duplicates_size // 2)}")
 
     if duplicates and (args.force or utils.confirm("Delete duplicates?")):  # type: ignore
         log.info("Deleting...")
         for d in duplicates:
```

### Comparing `xklb-1.26.20/xklb/scripts/merge_dbs.py` & `xklb-1.26.21/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/merge_online_local.py` & `xklb-1.26.21/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/move_list.py` & `xklb-1.26.21/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/optimize_db.py` & `xklb-1.26.21/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/redownload.py` & `xklb-1.26.21/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/relmv.py` & `xklb-1.26.21/xklb/scripts/relmv.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 utils.cmd_interactive("mv", abspath, target_dir)
             elif e.errno == 39:  # target dir not empty
                 log.info("%s ->m %s", abspath, dest)
                 _relmv(args, abspath.glob("*"), dest)
             elif e.errno == 2:  # FileNotFoundError
                 log.error("%s not found", abspath)
             else:
-                raise e
+                raise
 
 
 def relmv() -> None:
     args = parse_args()
 
     dest = Path(args.dest).expanduser().resolve()
     _relmv(args, args.sources, dest)
```

### Comparing `xklb-1.26.20/xklb/scripts/scatter.py` & `xklb-1.26.21/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.21/xklb/scripts/streaming_tab_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,16 @@
 def streaming_tab_loader() -> None:
     args = parse_args()
 
     try:
         from brotab.api import SingleMediatorAPI
         from brotab.main import create_clients
     except ModuleNotFoundError:
-        raise ModuleNotFoundError(
-            "brotab is required for surfing. Install with pip install brotab or pip install xklb[full]",
-        )
+        print("brotab is required for surfing. Install with pip install brotab or pip install xklb[full]")
+        raise
     else:
         logging.getLogger("brotab").setLevel(log.level)
         args.bt_api = SingleMediatorAPI(create_clients(args.target_hosts))  # type: ignore
 
     tabs_opened = 0
     initial_count = len(list_tabs(args))
     try:
```

### Comparing `xklb-1.26.20/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.21/xklb/scripts/mining/nfb_ca.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def get_page_links(url) -> None:
     from urllib.parse import urlparse
 
     import requests
     from bs4 import BeautifulSoup
 
-    soup = BeautifulSoup(requests.get(url).content, "html.parser")
+    soup = BeautifulSoup(requests.get(url, timeout=120).content, "html.parser")
     film_list = set()
 
     for a in soup.findAll("a", attrs={"href": True}):
         href = a["href"].strip()
         if all([len(href) > 1, href[0] != "#", "javascript:" not in href, "mailto:" not in href, "tel:" not in href]):
             if "/film/" in href:
                 up = urlparse(url)
```

### Comparing `xklb-1.26.20/xklb/scripts/mining/nouns.py` & `xklb-1.26.21/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/mining/pushshift.py` & `xklb-1.26.21/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.26.21/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/xklb/scripts/mining/words.py` & `xklb-1.26.21/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/assets/kotobago.png` & `xklb-1.26.21/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/.gitignore` & `xklb-1.26.21/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/LICENSE` & `xklb-1.26.21/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.20/README.md` & `xklb-1.26.21/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.020)
+    xk media library subcommands (v1.26.021)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.26.20/pyproject.toml` & `xklb-1.26.21/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -83,47 +83,60 @@
 
 [tool.ruff]
 ignore = [
   "ANN001",
   "ANN002",
   "ANN003",
   "ANN101",
+  "ANN204",
   "BLE001",
+  "C901",
   "D100",
   "D101",
   "D102",
   "D103",
   "D104",
+  "D107",
   "D211",
   "D212",
   "E401",
   "E501",
   "EM101",
   "ERA001",
+  "F401",
   "FBT002",
   "I001",
   "N806",
   "PGH003",
   "PGH004",
+  "PLR0913",
+  "PLW0603",
   "PLW2901",
   "PTH109",
   "PTH123",
+  "Q000",
   "RET504",
   "RET505",
   "RET507",
   "RUF001",
+  "RUF100",
   "S101",
   "S311",
   "S324",
+  "S603",
   "S606",
   "SIM103",
   "SIM105",
   "SIM108",
+  "SIM114",
+  "T100",
   "T201",
   "TRY003",
+  "TRY300",
+  "TRY301",
 ]
 line-length = 120
 select = ["ALL"]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 show-fixes = true
```

### Comparing `xklb-1.26.20/PKG-INFO` & `xklb-1.26.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.20
+Version: 1.26.21
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.020)
+    xk media library subcommands (v1.26.021)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

