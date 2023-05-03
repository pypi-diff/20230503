# Comparing `tmp/drb-2.1.3.tar.gz` & `tmp/drb-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-2.1.3.tar", last modified: Thu Mar 23 13:29:06 2023, max compression
+gzip compressed data, was "drb-2.1.4.tar", last modified: Wed May  3 12:14:31 2023, max compression
```

## Comparing `drb-2.1.3.tar` & `drb-2.1.4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.084036 drb-2.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-23 09:38:20.000000 drb-2.1.3/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-11-29 12:51:50.000000 drb-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10378 2023-03-23 13:29:06.084036 drb-2.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10007 2022-01-31 14:39:35.000000 drb-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.024035 drb-2.1.3/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.088036 drb-2.1.3/drb/core/
--rw-rw-rw-   0 root         (0) root         (0)      440 2022-11-29 12:51:50.000000 drb-2.1.3/drb/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-23 13:29:06.088036 drb-2.1.3/drb/core/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-01-23 09:38:20.000000 drb-2.1.3/drb/core/cortex_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2022-11-29 12:51:50.000000 drb-2.1.3/drb/core/events.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2023-03-08 16:35:51.000000 drb-2.1.3/drb/core/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2783 2023-03-08 16:35:51.000000 drb-2.1.3/drb/core/item.py
--rw-rw-rw-   0 root         (0) root         (0)    14860 2023-03-23 12:42:47.000000 drb-2.1.3/drb/core/node.py
--rw-rw-rw-   0 root         (0) root         (0)     9956 2023-03-08 16:35:51.000000 drb-2.1.3/drb/core/path.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2022-11-29 12:51:50.000000 drb-2.1.3/drb/core/predicate.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2022-11-29 12:51:50.000000 drb-2.1.3/drb/core/signature.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.024035 drb-2.1.3/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.044035 drb-2.1.3/drb/drivers/file/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-08 16:35:51.000000 drb-2.1.3/drb/drivers/file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4409 2023-03-23 12:42:47.000000 drb-2.1.3/drb/drivers/file/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.044035 drb-2.1.3/drb/drivers/xml/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-23 09:38:20.000000 drb-2.1.3/drb/drivers/xml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-01-23 09:38:20.000000 drb-2.1.3/drb/drivers/xml/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     7234 2023-03-15 13:58:11.000000 drb-2.1.3/drb/drivers/xml/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.048035 drb-2.1.3/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-01-23 09:38:20.000000 drb-2.1.3/drb/exceptions/core.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-01-23 09:38:20.000000 drb-2.1.3/drb/exceptions/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.024035 drb-2.1.3/drb/keyring/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.048035 drb-2.1.3/drb/keyring/bitwarden/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-01-23 09:38:20.000000 drb-2.1.3/drb/keyring/bitwarden/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-03-02 15:39:38.000000 drb-2.1.3/drb/keyring/bitwarden/bitwarden.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.056036 drb-2.1.3/drb/nodes/
--rw-rw-rw-   0 root         (0) root         (0)     7255 2023-03-15 13:58:12.000000 drb-2.1.3/drb/nodes/abstract_node.py
--rw-rw-rw-   0 root         (0) root         (0)     8125 2023-03-08 16:35:51.000000 drb-2.1.3/drb/nodes/logical_node.py
--rw-rw-rw-   0 root         (0) root         (0)    13171 2023-03-15 13:58:12.000000 drb-2.1.3/drb/nodes/mutable_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3277 2023-03-08 16:35:51.000000 drb-2.1.3/drb/nodes/url_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.060036 drb-2.1.3/drb/signatures/
--rw-rw-rw-   0 root         (0) root         (0)     6868 2022-11-29 12:51:50.000000 drb-2.1.3/drb/signatures/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.060036 drb-2.1.3/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.068036 drb-2.1.3/drb/topics/dao/
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/dao/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6624 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/dao/manager_dao.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/dao/topic_dao.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/dao/topic_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/dao/xml_dao.py
--rw-rw-rw-   0 root         (0) root         (0)     8789 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/dao/yaml_dao.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.068036 drb-2.1.3/drb/topics/file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-03-23 13:28:21.000000 drb-2.1.3/drb/topics/file/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)    13635 2023-03-17 13:56:33.000000 drb-2.1.3/drb/topics/resolver.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.068036 drb-2.1.3/drb/topics/xml/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-23 09:38:20.000000 drb-2.1.3/drb/topics/xml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-23 13:28:21.000000 drb-2.1.3/drb/topics/xml/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.072036 drb-2.1.3/drb/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-14 10:20:32.000000 drb-2.1.3/drb/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-11-29 12:51:50.000000 drb-2.1.3/drb/utils/drb_python_script.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2022-11-29 12:51:50.000000 drb-2.1.3/drb/utils/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-03-08 16:35:51.000000 drb-2.1.3/drb/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.032035 drb-2.1.3/drb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10378 2023-03-23 13:29:06.000000 drb-2.1.3/drb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1625 2023-03-23 13:29:06.000000 drb-2.1.3/drb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 13:29:06.000000 drb-2.1.3/drb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      517 2023-03-23 13:29:06.000000 drb-2.1.3/drb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 13:29:05.000000 drb-2.1.3/drb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-03-23 13:29:06.000000 drb-2.1.3/drb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-23 13:29:06.000000 drb-2.1.3/drb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-08 16:35:52.000000 drb-2.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-03-08 16:35:52.000000 drb-2.1.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-03-23 13:29:06.088036 drb-2.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-08 16:35:52.000000 drb-2.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 13:29:06.084036 drb-2.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-03-23 12:42:47.000000 drb-2.1.3/tests/test_abstract_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3544 2022-11-29 12:51:50.000000 drb-2.1.3/tests/test_drb_node_list.py
--rw-rw-rw-   0 root         (0) root         (0)     1468 2022-11-29 12:51:50.000000 drb-2.1.3/tests/test_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     6925 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_factory_resolver.py
--rw-rw-rw-   0 root         (0) root         (0)     6874 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_keyring_bitwarden.py
--rw-rw-rw-   0 root         (0) root         (0)    23074 2022-11-29 12:51:50.000000 drb-2.1.3/tests/test_logical_node.py
--rw-rw-rw-   0 root         (0) root         (0)     5213 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_manager_dao.py
--rw-rw-rw-   0 root         (0) root         (0)    15747 2023-03-02 15:39:38.000000 drb-2.1.3/tests/test_path.py
--rw-rw-rw-   0 root         (0) root         (0)     6697 2022-11-29 12:51:50.000000 drb-2.1.3/tests/test_signatures.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_topic.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-03-02 15:39:38.000000 drb-2.1.3/tests/test_url_node.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_xml_dao.py
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-01-23 09:38:21.000000 drb-2.1.3/tests/test_yaml_dao.py
--rw-rw-rw-   0 root         (0) root         (0)    70144 2022-10-19 07:59:20.000000 drb-2.1.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:31.099683 drb-2.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-23 09:38:20.000000 drb-2.1.4/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-11-29 12:51:50.000000 drb-2.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10378 2023-05-03 12:14:31.099683 drb-2.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10007 2022-01-31 14:39:35.000000 drb-2.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.911680 drb-2.1.4/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:31.103684 drb-2.1.4/drb/core/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-03 12:14:31.103684 drb-2.1.4/drb/core/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-01-23 09:38:20.000000 drb-2.1.4/drb/core/cortex_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2023-03-08 16:35:51.000000 drb-2.1.4/drb/core/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-03-08 16:35:51.000000 drb-2.1.4/drb/core/item.py
+-rw-rw-rw-   0 root         (0) root         (0)    14860 2023-03-23 12:42:47.000000 drb-2.1.4/drb/core/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     9956 2023-03-08 16:35:51.000000 drb-2.1.4/drb/core/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/predicate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/signature.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.907680 drb-2.1.4/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.935681 drb-2.1.4/drb/drivers/file/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-08 16:35:51.000000 drb-2.1.4/drb/drivers/file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4467 2023-05-02 15:56:43.000000 drb-2.1.4/drb/drivers/file/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.939681 drb-2.1.4/drb/drivers/xml/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-23 09:38:20.000000 drb-2.1.4/drb/drivers/xml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-01-23 09:38:20.000000 drb-2.1.4/drb/drivers/xml/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7022 2023-05-02 15:56:44.000000 drb-2.1.4/drb/drivers/xml/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.939681 drb-2.1.4/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-01-23 09:38:20.000000 drb-2.1.4/drb/exceptions/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-01-23 09:38:20.000000 drb-2.1.4/drb/exceptions/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.911680 drb-2.1.4/drb/keyring/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.943681 drb-2.1.4/drb/keyring/bitwarden/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-01-23 09:38:20.000000 drb-2.1.4/drb/keyring/bitwarden/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-03-02 15:39:38.000000 drb-2.1.4/drb/keyring/bitwarden/bitwarden.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.947681 drb-2.1.4/drb/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)     7255 2023-03-15 13:58:12.000000 drb-2.1.4/drb/nodes/abstract_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     8125 2023-03-08 16:35:51.000000 drb-2.1.4/drb/nodes/logical_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13171 2023-03-15 13:58:12.000000 drb-2.1.4/drb/nodes/mutable_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-03-08 16:35:51.000000 drb-2.1.4/drb/nodes/url_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.947681 drb-2.1.4/drb/signatures/
+-rw-rw-rw-   0 root         (0) root         (0)     6868 2022-11-29 12:51:50.000000 drb-2.1.4/drb/signatures/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.951681 drb-2.1.4/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.963681 drb-2.1.4/drb/topics/dao/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6624 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/manager_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/topic_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/topic_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/xml_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     8789 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/yaml_dao.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.963681 drb-2.1.4/drb/topics/file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-03 12:13:36.000000 drb-2.1.4/drb/topics/file/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13635 2023-03-17 13:56:33.000000 drb-2.1.4/drb/topics/resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.963681 drb-2.1.4/drb/topics/xml/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/xml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-03 12:13:36.000000 drb-2.1.4/drb/topics/xml/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.967681 drb-2.1.4/drb/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-14 10:20:32.000000 drb-2.1.4/drb/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-11-29 12:51:50.000000 drb-2.1.4/drb/utils/drb_python_script.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2022-11-29 12:51:50.000000 drb-2.1.4/drb/utils/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-03-08 16:35:51.000000 drb-2.1.4/drb/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.923681 drb-2.1.4/drb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10378 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-08 16:35:52.000000 drb-2.1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-03-08 16:35:52.000000 drb-2.1.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-03 12:14:31.103684 drb-2.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-08 16:35:52.000000 drb-2.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:31.099683 drb-2.1.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-03-23 12:42:47.000000 drb-2.1.4/tests/test_abstract_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_drb_node_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6925 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_factory_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6874 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_keyring_bitwarden.py
+-rw-rw-rw-   0 root         (0) root         (0)    23074 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_logical_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5213 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_manager_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)    15747 2023-03-02 15:39:38.000000 drb-2.1.4/tests/test_path.py
+-rw-rw-rw-   0 root         (0) root         (0)     6697 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_signatures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_topic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-03-02 15:39:38.000000 drb-2.1.4/tests/test_url_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_xml_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_yaml_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)    70144 2022-10-19 07:59:20.000000 drb-2.1.4/versioneer.py
```

### Comparing `drb-2.1.3/LICENCE.txt` & `drb-2.1.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/PKG-INFO` & `drb-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb
-Version: 2.1.3
+Version: 2.1.4
 Summary: Data Request Broker
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
```

### Comparing `drb-2.1.3/README.md` & `drb-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/events.py` & `drb-2.1.4/drb/core/events.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/factory.py` & `drb-2.1.4/drb/core/factory.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/item.py` & `drb-2.1.4/drb/core/item.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/node.py` & `drb-2.1.4/drb/core/node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/path.py` & `drb-2.1.4/drb/core/path.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/predicate.py` & `drb-2.1.4/drb/core/predicate.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/core/signature.py` & `drb-2.1.4/drb/core/signature.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/drivers/file/file.py` & `drb-2.1.4/drb/drivers/file/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             self._path = path
         else:
             if platform.uname()[0] == 'Windows':
                 path = pathlib.Path(path).as_posix()
             self._path = ParsedPath(os.path.abspath(path))
         self.parent: DrbNode = parent
         self.__init_attr()
-        self._available_impl.append(io.RawIOBase)
+        self._available_impl = [io.FileIO, io.BufferedReader]
         self.name = self._path.filename
         self._children: List[DrbNode] = None
 
     @property
     def path(self) -> ParsedPath:
         return self._path
 
@@ -94,18 +94,19 @@
                 sorted_child_names = sorted(os.listdir(self.path.path))
                 for filename in sorted_child_names:
                     child = DrbFileNode(self.path / filename, parent=self)
                     self._children.append(child)
         return self._children
 
     def get_impl(self, impl: type, **kwargs) -> Any:
-        if issubclass(impl, io.RawIOBase):
-            return impl_stream(self.path.path)
-        if issubclass(impl, io.BufferedIOBase):
-            return impl_buffered_stream(self.path.path)
+        if self.has_impl(impl):
+            if issubclass(io.FileIO, impl):
+                return impl_stream(self.path.path)
+            if issubclass(io.BufferedReader, impl):
+                return impl_buffered_stream(self.path.path)
         raise DrbNotImplementationException(
             f'no {impl} implementation found')
 
     def close(self) -> None:
         """
         Not use in this implementation.
```

### Comparing `drb-2.1.3/drb/drivers/xml/factory.py` & `drb-2.1.4/drb/drivers/xml/factory.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/drivers/xml/node.py` & `drb-2.1.4/drb/drivers/xml/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,49 +136,39 @@
     Parameters:
         node (DrbNode): the base node of this node.
         source(Union[BufferedIOBase, RawIOBase, IO]): The xml data.
     """
     def __init__(self, node: DrbNode, source: Union[BufferedIOBase, IO]):
         super().__init__()
         self.__base_node = node
+        self.name = node.name
+        self.namespace_uri = node.namespace_uri
+        self.value = node.value
+        self.parent = node.parent
         self.__source = source
         self.__xml_node = XmlNode(parse(source).getroot(), node)
         if isinstance(source, IOBase):
             self.__source.close()
+        for n, ns in node.attribute_names():
+            self @= (n, ns, node @ (n, ns))
 
-    @property
-    def name(self) -> str:
-        return self.__base_node.name
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return self.__base_node.namespace_uri
+    def __setitem__(self, key, value):
+        raise NotImplementedError
 
-    @property
-    def value(self) -> Optional[Any]:
-        return self.__base_node.value
+    def __delitem__(self, key):
+        raise NotImplementedError
 
     @property
     def path(self) -> ParsedPath:
         return self.__base_node.path
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self.__base_node.parent
-
     def impl_capabilities(self) -> List[type]:
         return self.__base_node.impl_capabilities()
 
     @property
-    @deprecated(version='2.1.0',
-                reason='Usage of the @ operator is recommended')
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self.__base_node.attributes
-
-    @property
     @deprecated(version='2.1.0', reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
         return [self.__xml_node]
 
     def has_child(self, name: str = None, namespace: str = None) -> bool:
         if name is None and namespace is None:
             return True
```

### Comparing `drb-2.1.3/drb/keyring/bitwarden/bitwarden.py` & `drb-2.1.4/drb/keyring/bitwarden/bitwarden.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/nodes/abstract_node.py` & `drb-2.1.4/drb/nodes/abstract_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/nodes/logical_node.py` & `drb-2.1.4/drb/nodes/logical_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/nodes/mutable_node.py` & `drb-2.1.4/drb/nodes/mutable_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/nodes/url_node.py` & `drb-2.1.4/drb/nodes/url_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/signatures/core.py` & `drb-2.1.4/drb/signatures/core.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/dao/manager_dao.py` & `drb-2.1.4/drb/topics/dao/manager_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/dao/topic_dao.py` & `drb-2.1.4/drb/topics/dao/topic_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/dao/topic_schema.yml` & `drb-2.1.4/drb/topics/dao/topic_schema.yml`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/dao/xml_dao.py` & `drb-2.1.4/drb/topics/dao/xml_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/dao/yaml_dao.py` & `drb-2.1.4/drb/topics/dao/yaml_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/resolver.py` & `drb-2.1.4/drb/topics/resolver.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/topics/topic.py` & `drb-2.1.4/drb/topics/topic.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/utils/drb_python_script.py` & `drb-2.1.4/drb/utils/drb_python_script.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/utils/plugins.py` & `drb-2.1.4/drb/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb/utils/utils.py` & `drb-2.1.4/drb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb.egg-info/PKG-INFO` & `drb-2.1.4/drb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb
-Version: 2.1.3
+Version: 2.1.4
 Summary: Data Request Broker
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
```

### Comparing `drb-2.1.3/drb.egg-info/SOURCES.txt` & `drb-2.1.4/drb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/drb.egg-info/entry_points.txt` & `drb-2.1.4/drb.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/setup.cfg` & `drb-2.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_abstract_node.py` & `drb-2.1.4/tests/test_abstract_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_drb_node_list.py` & `drb-2.1.4/tests/test_drb_node_list.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_event.py` & `drb-2.1.4/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_factory.py` & `drb-2.1.4/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_factory_resolver.py` & `drb-2.1.4/tests/test_factory_resolver.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_keyring_bitwarden.py` & `drb-2.1.4/tests/test_keyring_bitwarden.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_logical_node.py` & `drb-2.1.4/tests/test_logical_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_manager_dao.py` & `drb-2.1.4/tests/test_manager_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_path.py` & `drb-2.1.4/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_signatures.py` & `drb-2.1.4/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_topic.py` & `drb-2.1.4/tests/test_topic.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_url_node.py` & `drb-2.1.4/tests/test_url_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_xml_dao.py` & `drb-2.1.4/tests/test_xml_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/tests/test_yaml_dao.py` & `drb-2.1.4/tests/test_yaml_dao.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.3/versioneer.py` & `drb-2.1.4/versioneer.py`

 * *Files identical despite different names*

