# Comparing `tmp/whoisdomain-1.20230424.7.tar.gz` & `tmp/whoisdomain-1.20230503.1.tar.gz`

## Comparing `whoisdomain-1.20230424.7.tar` & `whoisdomain-1.20230503.1.tar`

### file list

```diff
@@ -1,206 +1,13 @@
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Historical.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/MANIFEST.in
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/license
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pypi-test.sh
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pypi.sh
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pyproject.toml-template
--rwxr-xr-x   0        0        0     2472 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test.py
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test.sh
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test2.py
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test_adjust.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.github/workflows/lint.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/getopt.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/getopt.meta.json
--rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test.meta.json
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test2.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test2.meta.json
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test_adjust.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test_adjust.meta.json
--rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
--rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_1_query.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
--rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
--rw-r--r--   0        0        0    12064 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
--rw-r--r--   0        0        0    17214 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/__init__.data.json
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/__init__.meta.json
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/exceptions.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
--rw-r--r--   0        0        0    19586 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/main.data.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/main.meta.json
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
--rw-r--r--   0        0        0    14355 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/whoisdomain.data.json
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/whoisdomain.meta.json
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/DONE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/TODO
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/analize_patterns.py
--rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/compare_known_tld.py
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/convert_to_dict.sh
--rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/makeTestdataAll.sh
--rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/test.py
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/test.sh
--rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/test3.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/testExtend.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/bin/find_input_no_output.sh
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/failed-parsing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/invalid-tld.txt
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/new-test.txt
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/ok-domains.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/private-reg.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/unknown-dateformat.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/docs/index.html
--rwxr-xr-x   0        0        0     1733 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/make_testdata.sh
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.com/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.com/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.com/output
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.net/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.net/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.net/output
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.org/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.org/nameservers
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.org/output
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/hello.xyz/input
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/hello.xyz/nameservers
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/hello.xyz/output
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.jp/input
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.jp/nameservers
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.jp/output
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.uk/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.uk/nameservers
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.uk/output
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com/input
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com/nameservers
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com/output
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com.tr/input
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com.tr/nameservers
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com.tr/output
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.jp/input
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.jp/nameservers
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.jp/output
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.kr/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.kr/nameservers
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.kr/output
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/xs4all.nl/input
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/xs4all.nl/nameservers
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/xs4all.nl/output
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_1_query.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    16746 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/main.py
--rw-r--r--   0        0        0   104916 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.gitignore
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.hgignore
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/README.md
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pyproject.toml
--rw-r--r--   0        0        0     8388 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/PKG-INFO
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    17812 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/main.py
+-rw-r--r--   0        0        0   104916 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/version.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/.gitignore
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/pyproject.toml
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/PKG-INFO
```

### Comparing `whoisdomain-1.20230424.7/pyproject.toml-template` & `whoisdomain-1.20230503.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,39 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build]
+only-packages = true
+
+include = [
+    "whoisdomain/*.py",
+]
+
+exclude = [
+    "/Old/*",
+    "/lib/*",
+    "/etc/*",
+    "/bin/*",
+    "/testdata/*",
+    "Makefile",
+    ".gitignore",
+    "/.gitignore",
+]
 
 [project]
 name = "whoisdomain"
-version = "@VERSION@.@YYYYMMDD@.@SEQ@"
+version = "1.20230503.1"
+
 authors = [
   { name="DannyCork"},
 ]
 
 maintainers = [
-  { name="Maarten Boot", email="mboot.github@gmail.com" },
+  { name="Maarten Boot", email="130295084+mboot-github@users.noreply.github.com" },
 ]
 
 description = "Python package for retrieving WHOIS information of domains."
 readme = "README.md"
 requires-python = ">=3.6"
 
 license = "MIT"
@@ -46,12 +64,13 @@
     "cctld",
     "registrar",
 ]
 
 [project.scripts]
 whoisdomain = 'whoisdomain.main:main'
 
+
 [project.urls]
 "Bug Tracker" = "https://github.com/mboot-github/WhoisDomain/issues"
 "Home Page" = "https://github.com/mboot-github/WhoisDomain/"
 "Repository" = "https://github.com/mboot-github/WhoisDomain/"
```

### Comparing `whoisdomain-1.20230424.7/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230503.1/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230424.7/whoisdomain/_1_query.py` & `whoisdomain-1.20230503.1/whoisdomain/_1_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     cache_age: int = CACHE_MAX_AGE,
     slow_down: int = 0,
     ignore_returncode: bool = False,
     server: Optional[str] = None,
     verbose: bool = False,
     timeout: Optional[float] = None,
     wh: str = "whois",
+    simplistic: bool = False,
 ) -> str:
     k = ".".join(dl)
 
     if cache_file:
         if verbose:
             print(f"using cache file: {cache_file}", file=sys.stderr)
         cache_load(cache_file)
@@ -72,14 +73,15 @@
             _do_whois_query(
                 dl=dl,
                 ignore_returncode=ignore_returncode,
                 server=server,
                 verbose=verbose,
                 timeout=timeout,
                 wh=wh,
+                simplistic=simplistic,
             ),
         )
 
         if cache_file:
             cache_save(cache_file)
 
     return CACHE[k][1]
@@ -162,14 +164,15 @@
 def _do_whois_query(
     dl: List[str],
     ignore_returncode: bool,
     server: Optional[str] = None,
     verbose: bool = False,
     timeout: Optional[float] = None,
     wh: str = "whois",
+    simplistic: bool = False,
 ) -> str:
     # if getenv[TEST_WHOIS_PYTON] fake whois by reading static data from a file
     # this wasy we can actually implemnt a test run with known data in and expected data out
     if os.getenv("TEST_WHOIS_PYTHON"):
         return testWhoisPythonFromStaticTestData(dl, ignore_returncode, server, verbose)
 
     cmd = makeWhoisCommandToRun(dl=dl, server=server, verbose=verbose, wh=wh)
@@ -199,10 +202,13 @@
         # network error, "fgets: Connection reset by peer" fix, ignore
         if "fgets: Connection reset by peer" in r:
             return r.replace("fgets: Connection reset by peer", "")
         # connect: Connection refused
         elif "connect: Connection refused" in r:
             return r.replace("connect: Connection refused", "")
 
+        if simplistic:
+            return r
+
         raise WhoisCommandFailed(r)
 
     return r
```

### Comparing `whoisdomain-1.20230424.7/whoisdomain/_2_parse.py` & `whoisdomain-1.20230503.1/whoisdomain/_2_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,15 @@
 
 def do_parse(
     whois_str: str,
     tld: str,
     dl: List[str],
     verbose: bool = False,
     with_cleanup_results: bool = False,
+    simplistic: bool = False,
 ) -> Optional[Dict[str, Any]]:
 
     whois_str = cleanupWhoisResponse(
         whois_str=whois_str,
         verbose=verbose,
         with_cleanup_results=with_cleanup_results,
     )
```

### Comparing `whoisdomain-1.20230424.7/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230503.1/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230424.7/whoisdomain/__init__.py` & `whoisdomain-1.20230503.1/whoisdomain/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import os
 from functools import wraps
 from typing import (
     cast,
     Optional,
     List,
     Dict,
     Tuple,
@@ -41,28 +42,44 @@
     UnknownDateFormat,
     WhoisCommandFailed,
     WhoisPrivateRegistry,
     WhoisQuotaExceeded,
     WhoisCommandTimeout,
 )
 
+from .version import (
+    VERSION,
+)
+
 __all__ = [
     "UnknownTld",
     "FailedParsingWhoisOutput",
     "UnknownDateFormat",
     "WhoisCommandFailed",
     "WhoisPrivateRegistry",
     "WhoisQuotaExceeded",
     "WhoisCommandTimeout",
     "cleanupWhoisResponse",
     "validTlds",
     "TLD_RE",
     "get_last_raw_whois_data",
+    "VERSION",
+    "getVersion",
 ]
 
+WHOISDOMAIN: str = ""
+if os.getenv("WHOISDOMAIN"):
+    WHOISDOMAIN = str(os.getenv("WHOISDOMAIN"))
+
+WD = WHOISDOMAIN.upper().split(":")
+
+SIMPLISTIC = False
+if "SIMPISTIC" in WD:
+    SIMPLISTIC = True
+
 CACHE_FILE = None
 SLOW_DOWN = 0
 
 LastWhois: Dict[str, Any] = {
     "Try": [],
 }
 
@@ -173,26 +190,28 @@
     tld: str,
     dl: List[str],
     ignore_returncode: bool = False,
     slow_down: int = 0,
     server: Optional[str] = None,
     verbose: bool = False,
     wh: str = "whois",
+    simplistic: bool = False,
 ) -> Optional[Domain]:
     include_raw_whois_text = True
 
     # we will not hunt for possible valid first level domains as we have no actual feedback
 
     whois_str = do_query(
         dl=dl,
         slow_down=slow_down,
         ignore_returncode=ignore_returncode,
         server=server,
         verbose=verbose,
         wh=wh,
+        simplistic=simplistic,
     )
 
     # we will only return minimal data
     data = {
         "tld": tld,
         "domain_name": [],
     }
@@ -229,14 +248,15 @@
     verbose: bool = False,
     with_cleanup_results: bool = False,
     internationalized: bool = False,
     include_raw_whois_text: bool = False,
     return_raw_text_for_unsupported_tld: bool = False,
     timeout: Optional[float] = None,
     cmd: str = "whois",
+    simplistic: bool = False,
 ) -> Optional[Domain]:
     """
     force=True          Don't use cache.
     cache_file=<path>   Use file to store cache not only memory.
     cache_age=172800    Cache expiration time for given domain, in seconds
     slow_down=0         Time [s] it will wait after you query WHOIS database.
                         This is useful when there is a limit to the number of requests at a time.
@@ -247,16 +267,17 @@
     internationalized:  if true convert with internationalizedDomainNameToPunyCode().
     ignore_returncode:  if true and the whois command fails with code 1, still process the data returned as normal.
     verbose:            if true, print relevant information on steps taken to standard error
     include_raw_whois_text:
                         if reqested the full response is also returned.
     return_raw_text_for_unsupported_tld:
                         if the tld is unsupported, just try it anyway but return only the raw text.
-    timeout:
-                        timeout in seconds for the whois command to return a result.
+    timeout:            timeout in seconds for the whois command to return a result.
+    cmd:                explicitly specify the path to the whois you want to use.
+    simplistic:         when simplistic is True we return None for most exceptions and dont pass info why we have no data.
     """
     global LastWhois
     LastWhois["Try"] = []  # init on start of query
 
     wh: str = cmd  # make it compatible with python-whois-extended
 
     assert isinstance(domain, str), Exception("`domain` - must be <str>")
@@ -271,23 +292,25 @@
         return None
 
     dl = cast(List[str], dl)
     thisTld = _validateWeKnowTheToplevelDomain(
         tld,
         return_raw_text_for_unsupported_tld,
     )  # may raise UnknownTld
+
     if thisTld is None:
         return _doUnsupportedTldAnyway(
             tld,
             dl,
             ignore_returncode=ignore_returncode,
             slow_down=slow_down,
             server=server,
             verbose=verbose,
             wh=wh,
+            simplistic=simplistic,
         )
 
     _verifyPrivateREgistry(thisTld)  # may raise WhoisPrivateRegistry
     server = _doServerHintsForThisTld(tld, thisTld, server, verbose)
 
     slow_down = slow_down or SLOW_DOWN
     slow_down = _doSlowdownHintForThisTld(tld, thisTld, slow_down, verbose)
@@ -306,28 +329,31 @@
             cache_file=cache_file,
             cache_age=cache_age,
             slow_down=slow_down,
             ignore_returncode=ignore_returncode,
             server=server,
             verbose=verbose,
             timeout=timeout,
+            simplistic=simplistic,
         )
+
         tryMe = {
             "Domain": ".".join(dl),
             "rawData": whois_str,
             "server": server,
         }
         LastWhois["Try"].append(tryMe)
 
         data = do_parse(
             whois_str=whois_str,
             tld=tld,
             dl=dl,
             verbose=verbose,
             with_cleanup_results=with_cleanup_results,
+            simplistic=simplistic,
         )
 
         # do we have a result and does it have a domain name
         if data and data["domain_name"][0]:
             return Domain(
                 data=data,
                 whois_str=whois_str,
@@ -345,7 +371,11 @@
         return None
 
     return None
 
 
 # Add get function to support return result in dictionary form
 get = _result2dict(query)
+
+
+def getVersion() -> str:
+    return VERSION
```

### Comparing `whoisdomain-1.20230424.7/whoisdomain/exceptions.py` & `whoisdomain-1.20230503.1/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230424.7/whoisdomain/main.py` & `whoisdomain-1.20230503.1/whoisdomain/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/python3
 
 import os
 import re
 import getopt
 import sys
+import json
+
 from typing import (
     Optional,
     Tuple,
     Any,
     List,
     Dict,
 )
 
 import whoisdomain as whois  # to be compatible with dannycork
 
+# if we are not running as test2.py run in a simplistic way
+SIMPLISTIC: bool = False
 
+PrintJson: bool = False
 Verbose: bool = False
 PrintGetRawWhoisResult: bool = False
 Ruleset: bool = False
 
 Failures: Dict[str, Any] = {}
 IgnoreReturncode: bool = False
 
@@ -181,16 +186,17 @@
                 cr = " [CR] " if "\r" in lines else ""  # \r is present in this section
                 print(f"# --- {k} Section: {n} {cr}{tab}{ws}")
                 n += 1
                 print(lines)
 
 
 def prepItem(d: str) -> None:
-    print("")
-    print(f"test domain: <<<<<<<<<< {d} >>>>>>>>>>>>>>>>>>>>")
+    if PrintJson is False:
+        print("")
+        print(f"test domain: <<<<<<<<<< {d} >>>>>>>>>>>>>>>>>>>>")
 
 
 def xType(x: Any) -> str:
     s = f"{type(x)}"
     return s.split("'")[1]
 
 
@@ -205,14 +211,15 @@
     w = whois.query(
         d,
         ignore_returncode=IgnoreReturncode,
         verbose=Verbose,
         internationalized=True,
         include_raw_whois_text=PrintGetRawWhoisResult,
         timeout=timout,
+        simplistic=SIMPLISTIC,
     )
 
     if w is None:
         print("None")
         print("\n", whois.get_last_raw_whois_data())
         return
 
@@ -221,20 +228,34 @@
     # some strings are return as '' when empty (status)
     # statuses can be a array of one empty string if no data
 
     # not all values are always present it mainly depends on whet we see in the output of whois
     # if we return not None: the elements that ars always there ars domain_name , tld, dnssec
 
     wd = w.__dict__
+    if PrintJson is True:
+        for f in ["creation_date", "expiration_date", "last_updated"]:
+            if f in wd:
+                wd[f] = f"{wd[f]}"
+        print(json.dumps(wd))
+        return
+
     for k, v in wd.items():
-        ss = "%-18s %-17s "
-        if isinstance(v, str):
-            print((ss + "'%s'") % (k, xType(v), v))
+        if SIMPLISTIC:
+            ss = "%-18s "
+            if isinstance(v, str):
+                print((ss + "'%s'") % (k, v))
+            else:
+                print((ss + "%s") % (k, v))
         else:
-            print((ss + "%s") % (k, xType(v), v))
+            ss = "%-18s %-17s "
+            if isinstance(v, str):
+                print((ss + "'%s'") % (k, xType(v), v))
+            else:
+                print((ss + "%s") % (k, xType(v), v))
 
     # print("\n", whois.get_last_raw_whois_data())
 
 
 def errorItem(d: str, e: Any, what: str = "Generic") -> None:
     if what not in Failures:
         Failures[what] = {}
@@ -354,65 +375,78 @@
 
 def usage() -> None:
     name = os.path.basename(sys.argv[0])
 
     print(
         f"""
 {name}
-    [ -v | --verbose ]
-        # set verbose to True, this will be forwarded to whois.query
+    [ -h | --usage ]
+        print this text and exit
 
-    [ -I | --IgnoreReturncode ]
-        # sets the IgnoreReturncode to True, this will be forwarded to whois.query
+    [ -V | --Version ]
+        print the build version string
+        and exit
 
-    [ -a | --all]
-        # test all existing tld currently supported,
+    [ -S | --SupportedTld ]
+        print all known top level domains
+        and exit
 
-    [ -d <domain> | --domain = <domain> " ]
-        # only analyze the given domains
-        # the option can be repeated to specify more then one domain
+    [ -a | --all]
+        test all existing tld currently supported
+        and exit
 
     [ -f <filename> | --file = <filename> " ]
-        # use the named file to test all domains (one domain per line)
-        # lines starting with # or empty lines are skipped, anything after the domain is ignored
-        # the option can be repeated to specify more then one file
+        use the named file to test all domains (one domain per line)
+        lines starting with # or empty lines are skipped, anything after the domain is ignored
+        the option can be repeated to specify more then one file
+        exits after processing all the files
 
     [ -D <directory> | --Directory = <directory> " ]
-        # use the named directory, ald use all files ending in .txt as files containing domains
-        # files are processed as in the -f option so comments and empty lines are skipped
-        # the option can be repeated to specify more then one directory
+        use the named directory, ald use all files ending in .txt as files containing domains
+        files are processed as in the -f option so comments and empty lines are skipped
+        the option can be repeated to specify more then one directory
+        exits after processing all the dirs
 
-    [ -p | --print ]
-    also print text containing the raw output of whois
+    [ -d <domain> | --domain = <domain> " ]
+        only analyze the given domains
+        the option can be repeated to specify more domain's
 
-    [ -R | --Ruleset ]
-    dump the ruleset for the tld and exit
+    [ -v | --verbose ]
+        set verbose to True,
+        verbose output will be printed on stderr only
 
-    [ -S | --SupportedTld ]
-    print all supported top level domains we know and exit
+    [ -j | --json ]
+        print each result as json
 
-    [ -C <file> | --Cleanup <file> ]
-    read the input file specified and run the same cleanup as in whois.query , then exit
+    [ -I | --IgnoreReturncode ]
+        sets the IgnoreReturncode to True,
 
-    # options are exclusive and without any options the {name} program does nothing
+    [ -p | --print ]
+        also print text containing the raw output of the cli whois
 
-    # test one specific file with verbose and IgnoreReturncode
-    example: {name} -v -I -f tests/ok-domains.txt 2>2 >out
+    [ -R | --Ruleset ]
+        dump the ruleset for the requested tld and exit
+        should be combined with -d to specify tld's
 
-    # test one specific directory with verbose and IgnoreReturncode
-    example: {name} -v -I -D tests 2>2 >out
+    [ -C <file> | --Cleanup <file> ]
+        read the input file specified and run the same cleanup as in whois.query,
+        then exit
 
     # test two domains with verbose and IgnoreReturncode
-    example: {name} -v -I -d meta.org -d meta.com 2>2 >out
+    example: {name} -v -I -d meta.org -d meta.com
 
     # test all supported tld's with verbose and IgnoreReturncode
-    example: {name} -v -I -a 2>2 >out
+    example: {name} -v -I -a
+
+    # test one specific file with verbose and IgnoreReturncode
+    example: {name} -v -I -f tests/ok-domains.txt
+
+    # test one specific directory with verbose and IgnoreReturncode
+    example: {name} -v -I -D tests
 
-    # test nothing
-    example: {name} -v -I 2>2 >out
 """
     )
 
     """
     TODO
     --all --reg <re>
         from all tld a regex match sub selection
@@ -428,28 +462,42 @@
         print("\n# ========================")
         for i in sorted(Failures.keys()):
             for j in sorted(Failures[i].keys()):
                 print(i, j, Failures[i][j])
 
 
 def main() -> None:
+    global PrintJson
     global Verbose
     global IgnoreReturncode
     global PrintGetRawWhoisResult
     global Ruleset
+    global SIMPLISTIC
+
+    name: str = os.path.basename(sys.argv[0])
+    if name == "test2.py":
+        SIMPLISTIC = False
+    else:
+        SIMPLISTIC = True
+
+    if 0:
+        print(name, SIMPLISTIC)
+        exit(0)
 
     try:
         opts, args = getopt.getopt(
             sys.argv[1:],
-            "RSpvIhaf:d:D:r:H:C:",
+            "jRSpvVIhaf:d:D:r:H:C:",
             [
+                "json",
                 "Ruleset",
                 "SupportedTld",
                 "print",
                 "verbose",
+                "Version",
                 "IgnoreReturncode",
                 "all",
                 "file=",
                 "Directory=",
                 "domain=",
                 "reg=",
                 "having=",
@@ -478,14 +526,18 @@
 
     for opt, arg in opts:
         if opt in ("-S", "SupportedTld"):
             for tld in sorted(whois.validTlds()):
                 print(tld)
             sys.exit(0)
 
+        if opt in ("-V", "Version"):
+            print(whois.getVersion())
+            sys.exit(0)
+
         if opt == "-h":
             usage()
             sys.exit(0)
 
         if opt in ("-a", "--all"):
             testAllTld = True
 
@@ -499,14 +551,17 @@
 
         if opt in ("-v", "--verbose"):
             Verbose = True
 
         if opt in ("-p", "--print"):
             PrintGetRawWhoisResult = True
 
+        if opt in ("-j", "--json"):
+            PrintJson = True
+
         if opt in ("-R", "--Ruleset"):
             Ruleset = True
 
         if opt in ("-D", "--Directory"):
             directory = arg
             isDir = os.path.isdir(directory)
             if isDir is False:
@@ -547,42 +602,38 @@
         sys.exit(0)
 
     if testAllTld:
         print("## ===== TEST CURRENT TLD's")
         allMetaTld = makeMetaAllCurrentTld(allHaving, allRegex)
         testDomains(allMetaTld)
         showFailures()
-        return
+        sys.exit(0)
 
     if len(dirs):
         fileData = {}
-        print("## ===== TEST DIRECTORIES")
         for dName in dirs:
             getTestFilesAll(dName, fileData)
         for testFile in fileData:
-            print(f"## ===== TEST FILE: {testFile}")
             testDomains(fileData[testFile])
         showFailures()
-        return
+        sys.exit(0)
 
     if len(files):
         fileData = {}
-        print("## ===== TEST FILES")
         for testFile in files:
             getTestFileOne(testFile, fileData)
         for testFile in fileData:
-            print(f"## ===== TEST FILE: {testFile}")
             testDomains(fileData[testFile])
         showFailures()
-        return
+        sys.exit(0)
 
     if len(domains):
         testDomains(domains)
         showFailures()
-        return
+        sys.exit(0)
 
     usage()
     sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `whoisdomain-1.20230424.7/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230503.1/whoisdomain/tld_regexpr.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230424.7/.gitignore` & `whoisdomain-1.20230503.1/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230424.7/README.md` & `whoisdomain-1.20230503.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # whoisdomain
 
+* https://pypi.org/project/whoisdomain/
+
 A Python package for retrieving WHOIS information of DOMAIN'S ONLY.
 
 This package will not support querying ip CIDR ranges or AS information
 
 This is a copy of the original DanyCork 'whois'.
 
 I will start versioning at 1.x.x where the second item will be YYYYMMDD,
@@ -21,27 +23,28 @@
  * raise a exception on Quota ecceeded type responses
  * raise a exception on PrivateRegistry tld's where we know the tld and know we don't know anything
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
  * the module is now 'mypy --strict' clean
  * the module now also exports a cli command domainwhois
+ * both the module and the cli now support showing the version with lib:whois.getVersion() or cli:whoisdomain -V
 
 ## Dependencies
-  * please install also the command line "whois" of your distribution
-  * this library parses the output of the "whois" cli command of your operating system
+  * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
 ## Usage example
 
 Install the cli `whois` of your operating system if it is not present already,
 e.g 'apt install whois' or 'yum install whois'
 
 ```
+# fedora 37
 sudo yum install whois
-$pip install whoisdomain
+pip install whoisdomain
 python
 >>> import whoisdomain as whois
 >>> d = whois.query('google.com')
 >>> print(d.__dict__)
 {'name': 'google.com', 'tld': 'com', 'registrar': 'MarkMonitor, Inc.', 'registrant_country': 'US', 'creation_date': datetime.datetime(1997, 9, 15, 9, 0), 'expiration_date': datetime.datetime(2028, 9, 13, 9, 0), 'last_updated': datetime.datetime(2019, 9, 9, 17, 39, 4), 'status': 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'statuses': ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)'], 'dnssec': False, 'name_servers': ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com'], 'registrant': 'Google LLC', 'emails': ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']}
 >>> print (d.expiration_date)
 2028-09-13 09:00:00
@@ -49,17 +52,20 @@
 >>> print(d.name)
 google.com
 
 >>> print (d.creation_date)
 1997-09-15 09:00:00
 ```
 
-# example test2.py
+# whoisdomain
 ```
-./test2.py -d google.com
+# fedora 37
+sudo yum install whois
+pip3 install whoisdomain
+whoisdomain -d google.com
 
 test domain: <<<<<<<<<< google.com >>>>>>>>>>>>>>>>>>>>
 name               str               'google.com'
 tld                str               'com'
 registrar          str               'MarkMonitor, Inc.'
 registrant_country str               'US'
 creation_date      datetime.datetime 1997-09-15 09:00:00
@@ -73,75 +79,83 @@
 emails             list              ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
 
  ```
 
 A short intro into the cli whoisdomain command
 ```
 whoisdomain
-    [ -v | --verbose ]
-        # set verbose to True, this will be forwarded to whois.query
+    [ -h | --usage ]
+        print this text and exit
 
-    [ -I | --IgnoreReturncode ]
-        # sets the IgnoreReturncode to True, this will be forwarded to whois.query
+    [ -V | --Version ]
+        print the build version string
+        and exit
 
-    [ -a | --all]
-        # test all existing tld currently supported,
+    [ -S | --SupportedTld ]
+        print all known top level domains
+        and exit
 
-    [ -d <domain> | --domain = <domain> " ]
-        # only analyze the given domains
-        # the option can be repeated to specify more then one domain
+    [ -a | --all]
+        test all existing tld currently supported
+        and exit
 
     [ -f <filename> | --file = <filename> " ]
-        # use the named file to test all domains (one domain per line)
-        # lines starting with # or empty lines are skipped, anything after the domain is ignored
-        # the option can be repeated to specify more then one file
+        use the named file to test all domains (one domain per line)
+        lines starting with # or empty lines are skipped, anything after the domain is ignored
+        the option can be repeated to specify more then one file
+        exits after processing all the files
 
     [ -D <directory> | --Directory = <directory> " ]
-        # use the named directory, ald use all files ending in .txt as files containing domains
-        # files are processed as in the -f option so comments and empty lines are skipped
-        # the option can be repeated to specify more then one directory
+        use the named directory, ald use all files ending in .txt as files containing domains
+        files are processed as in the -f option so comments and empty lines are skipped
+        the option can be repeated to specify more then one directory
+        exits after processing all the dirs
 
-    [ -p | --print ]
-    also print text containing the raw output of whois
-
-    [ -R | --Ruleset ]
-    dump the ruleset for the tld and exit
+    [ -d <domain> | --domain = <domain> " ]
+        only analyze the given domains
+        the option can be repeated to specify more domain's
 
-    [ -S | --SupportedTld ]
-    print all supported top level domains we know and exit
+    [ -v | --verbose ]
+        set verbose to True,
+        verbose output will be printed on stderr only
 
-    [ -C <file> | --Cleanup <file> ]
-    read the input file specified and run the same cleanup as in whois.query , then exit
+    [ -I | --IgnoreReturncode ]
+        sets the IgnoreReturncode to True,
 
-    # options are exclusive and without any options the whoisdomain program does nothing
+    [ -p | --print ]
+        also print text containing the raw output of the cli whois
 
-    # test one specific file with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -f tests/ok-domains.txt 2>2 >out
+    [ -R | --Ruleset ]
+        dump the ruleset for the requested tld and exit
+        should be combined with -d to specify tld's
 
-    # test one specific directory with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -D tests 2>2 >out
+    [ -C <file> | --Cleanup <file> ]
+        read the input file specified and run the same cleanup as in whois.query,
+        then exit
 
     # test two domains with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -d meta.org -d meta.com 2>2 >out
+    example: whoisdomain -v -I -d meta.org -d meta.com
 
     # test all supported tld's with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -a 2>2 >out
+    example: whoisdomain -v -I -a
 
-    # test nothing
-    example: whoisdomain -v -I 2>2 >out
+    # test one specific file with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -f tests/ok-domains.txt
 
+    # test one specific directory with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -D tests
 ```
 
 ## ccTLD & TLD support
 see the file: ./whoisdomain/tld_regexpr.py
-or call whoisdomain.validTlds()
+or call lib:whoisdomain.validTlds() or cli:whoisdomain -S
 
 ## Support
  * Python 3.x is supported for x >= 6
  * Python 2.x IS NOT supported.
 
 ## Author's
   * this is a rename copy of original work done in: https://github.com/DannyCork/python-whois
   * the project is also related to the project: https://github.com/gen1us2k/python-whois
   * both seem derived from a older google.code site: https://code.google.com/archive/p/python-whois
-  * aside from the original authors, many others already contributed to the repositories
+  * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
```

### Comparing `whoisdomain-1.20230424.7/PKG-INFO` & `whoisdomain-1.20230503.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230424.7
+Version: 1.20230503.1
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
-Maintainer-email: Maarten Boot <mboot.github@gmail.com>
+Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
 Keywords: Python,cctld,domain,expiration,registrar,tld,whois
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -22,14 +22,16 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # whoisdomain
 
+* https://pypi.org/project/whoisdomain/
+
 A Python package for retrieving WHOIS information of DOMAIN'S ONLY.
 
 This package will not support querying ip CIDR ranges or AS information
 
 This is a copy of the original DanyCork 'whois'.
 
 I will start versioning at 1.x.x where the second item will be YYYYMMDD,
@@ -47,27 +49,28 @@
  * raise a exception on Quota ecceeded type responses
  * raise a exception on PrivateRegistry tld's where we know the tld and know we don't know anything
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
  * the module is now 'mypy --strict' clean
  * the module now also exports a cli command domainwhois
+ * both the module and the cli now support showing the version with lib:whois.getVersion() or cli:whoisdomain -V
 
 ## Dependencies
-  * please install also the command line "whois" of your distribution
-  * this library parses the output of the "whois" cli command of your operating system
+  * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
 ## Usage example
 
 Install the cli `whois` of your operating system if it is not present already,
 e.g 'apt install whois' or 'yum install whois'
 
 ```
+# fedora 37
 sudo yum install whois
-$pip install whoisdomain
+pip install whoisdomain
 python
 >>> import whoisdomain as whois
 >>> d = whois.query('google.com')
 >>> print(d.__dict__)
 {'name': 'google.com', 'tld': 'com', 'registrar': 'MarkMonitor, Inc.', 'registrant_country': 'US', 'creation_date': datetime.datetime(1997, 9, 15, 9, 0), 'expiration_date': datetime.datetime(2028, 9, 13, 9, 0), 'last_updated': datetime.datetime(2019, 9, 9, 17, 39, 4), 'status': 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'statuses': ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)'], 'dnssec': False, 'name_servers': ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com'], 'registrant': 'Google LLC', 'emails': ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']}
 >>> print (d.expiration_date)
 2028-09-13 09:00:00
@@ -75,17 +78,20 @@
 >>> print(d.name)
 google.com
 
 >>> print (d.creation_date)
 1997-09-15 09:00:00
 ```
 
-# example test2.py
+# whoisdomain
 ```
-./test2.py -d google.com
+# fedora 37
+sudo yum install whois
+pip3 install whoisdomain
+whoisdomain -d google.com
 
 test domain: <<<<<<<<<< google.com >>>>>>>>>>>>>>>>>>>>
 name               str               'google.com'
 tld                str               'com'
 registrar          str               'MarkMonitor, Inc.'
 registrant_country str               'US'
 creation_date      datetime.datetime 1997-09-15 09:00:00
@@ -99,75 +105,83 @@
 emails             list              ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
 
  ```
 
 A short intro into the cli whoisdomain command
 ```
 whoisdomain
-    [ -v | --verbose ]
-        # set verbose to True, this will be forwarded to whois.query
+    [ -h | --usage ]
+        print this text and exit
 
-    [ -I | --IgnoreReturncode ]
-        # sets the IgnoreReturncode to True, this will be forwarded to whois.query
+    [ -V | --Version ]
+        print the build version string
+        and exit
 
-    [ -a | --all]
-        # test all existing tld currently supported,
+    [ -S | --SupportedTld ]
+        print all known top level domains
+        and exit
 
-    [ -d <domain> | --domain = <domain> " ]
-        # only analyze the given domains
-        # the option can be repeated to specify more then one domain
+    [ -a | --all]
+        test all existing tld currently supported
+        and exit
 
     [ -f <filename> | --file = <filename> " ]
-        # use the named file to test all domains (one domain per line)
-        # lines starting with # or empty lines are skipped, anything after the domain is ignored
-        # the option can be repeated to specify more then one file
+        use the named file to test all domains (one domain per line)
+        lines starting with # or empty lines are skipped, anything after the domain is ignored
+        the option can be repeated to specify more then one file
+        exits after processing all the files
 
     [ -D <directory> | --Directory = <directory> " ]
-        # use the named directory, ald use all files ending in .txt as files containing domains
-        # files are processed as in the -f option so comments and empty lines are skipped
-        # the option can be repeated to specify more then one directory
+        use the named directory, ald use all files ending in .txt as files containing domains
+        files are processed as in the -f option so comments and empty lines are skipped
+        the option can be repeated to specify more then one directory
+        exits after processing all the dirs
 
-    [ -p | --print ]
-    also print text containing the raw output of whois
-
-    [ -R | --Ruleset ]
-    dump the ruleset for the tld and exit
+    [ -d <domain> | --domain = <domain> " ]
+        only analyze the given domains
+        the option can be repeated to specify more domain's
 
-    [ -S | --SupportedTld ]
-    print all supported top level domains we know and exit
+    [ -v | --verbose ]
+        set verbose to True,
+        verbose output will be printed on stderr only
 
-    [ -C <file> | --Cleanup <file> ]
-    read the input file specified and run the same cleanup as in whois.query , then exit
+    [ -I | --IgnoreReturncode ]
+        sets the IgnoreReturncode to True,
 
-    # options are exclusive and without any options the whoisdomain program does nothing
+    [ -p | --print ]
+        also print text containing the raw output of the cli whois
 
-    # test one specific file with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -f tests/ok-domains.txt 2>2 >out
+    [ -R | --Ruleset ]
+        dump the ruleset for the requested tld and exit
+        should be combined with -d to specify tld's
 
-    # test one specific directory with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -D tests 2>2 >out
+    [ -C <file> | --Cleanup <file> ]
+        read the input file specified and run the same cleanup as in whois.query,
+        then exit
 
     # test two domains with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -d meta.org -d meta.com 2>2 >out
+    example: whoisdomain -v -I -d meta.org -d meta.com
 
     # test all supported tld's with verbose and IgnoreReturncode
-    example: whoisdomain -v -I -a 2>2 >out
+    example: whoisdomain -v -I -a
 
-    # test nothing
-    example: whoisdomain -v -I 2>2 >out
+    # test one specific file with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -f tests/ok-domains.txt
 
+    # test one specific directory with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -D tests
 ```
 
 ## ccTLD & TLD support
 see the file: ./whoisdomain/tld_regexpr.py
-or call whoisdomain.validTlds()
+or call lib:whoisdomain.validTlds() or cli:whoisdomain -S
 
 ## Support
  * Python 3.x is supported for x >= 6
  * Python 2.x IS NOT supported.
 
 ## Author's
   * this is a rename copy of original work done in: https://github.com/DannyCork/python-whois
   * the project is also related to the project: https://github.com/gen1us2k/python-whois
   * both seem derived from a older google.code site: https://code.google.com/archive/p/python-whois
-  * aside from the original authors, many others already contributed to the repositories
+  * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
```

