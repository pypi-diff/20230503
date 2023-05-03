# Comparing `tmp/types-Markdown-3.4.2.7.tar.gz` & `tmp/types-Markdown-3.4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Markdown-3.4.2.7.tar", last modified: Tue Apr  4 12:29:21 2023, max compression
+gzip compressed data, was "types-Markdown-3.4.2.8.tar", last modified: Wed May  3 12:29:47 2023, max compression
```

## Comparing `types-Markdown-3.4.2.7.tar` & `types-Markdown-3.4.2.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:29:21.265724 types-Markdown-3.4.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-04 12:29:18.000000 types-Markdown-3.4.2.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 12:29:18.000000 types-Markdown-3.4.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-04 12:29:21.265724 types-Markdown-3.4.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:29:21.265724 types-Markdown-3.4.2.7/markdown-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-04 12:29:18.000000 types-Markdown-3.4.2.7/markdown-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/__meta__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/blockparser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/blockprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:29:21.265724 types-Markdown-3.4.2.7/markdown-stubs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/abbr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/admonition.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/attr_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/codehilite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/def_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/extra.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/fenced_code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/footnotes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/legacy_attrs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/legacy_em.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/md_in_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/meta.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/nl2br.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/sane_lists.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/smarty.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/toc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/extensions/wikilinks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/inlinepatterns.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/postprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/preprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/serializers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/treeprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-04 12:29:07.000000 types-Markdown-3.4.2.7/markdown-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:29:21.265724 types-Markdown-3.4.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-04 12:29:18.000000 types-Markdown-3.4.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:29:21.265724 types-Markdown-3.4.2.7/types_Markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-04 12:29:21.000000 types-Markdown-3.4.2.7/types_Markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-04 12:29:21.000000 types-Markdown-3.4.2.7/types_Markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:29:21.000000 types-Markdown-3.4.2.7/types_Markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 12:29:21.000000 types-Markdown-3.4.2.7/types_Markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.400845 types-Markdown-3.4.2.8/markdown-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/markdown-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/__meta__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/blockparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/blockprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/markdown-stubs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/abbr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/admonition.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/attr_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/codehilite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/def_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/extra.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/fenced_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/footnotes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/legacy_attrs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/legacy_em.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/md_in_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/meta.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/nl2br.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/sane_lists.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/smarty.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/toc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/wikilinks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/inlinepatterns.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/postprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/preprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/serializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/treeprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/types_Markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/top_level.txt
```

### Comparing `types-Markdown-3.4.2.7/CHANGELOG.md` & `types-Markdown-3.4.2.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.4.2.8 (2023-05-03)
+
+Add Markdown.ESCAPED_CHARS to Markdown stubs (#10134)
+
 ## 3.4.2.7 (2023-04-04)
 
 Various improvements to `Markdown` stubs (#10008)
 
 ## 3.4.2.6 (2023-03-27)
 
 Add defaults for third-party stubs M-O (#9956)
```

### Comparing `types-Markdown-3.4.2.7/PKG-INFO` & `types-Markdown-3.4.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Markdown
-Version: 3.4.2.7
+Version: 3.4.2.8
 Summary: Typing stubs for Markdown
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Markdown.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Markdown`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Markdown. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fe9eb630eedfc588c57cee51807c505c072c1348`.
+This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
```

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/blockparser.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/blockparser.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/blockprocessors.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/blockprocessors.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/core.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/core.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     htmlStash: HtmlStash
     output_formats: ClassVar[dict[Literal["xhtml", "html"], Callable[[Element], str]]]
     output_format: Literal["xhtml", "html"]
     serializer: Callable[[Element], str]
     tab_length: int
     block_level_elements: list[str]
     registeredExtensions: list[Extension]
+    ESCAPED_CHARS: list[str]
     def __init__(
         self,
         *,
         extensions: Sequence[str | Extension] | None = ...,
         extension_configs: Mapping[str, Mapping[str, Any]] | None = ...,
         output_format: Literal["xhtml", "html"] | None = ...,
         tab_length: int | None = ...,
```

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/extensions/__init__.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/extensions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/extensions/codehilite.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/extensions/codehilite.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/extensions/footnotes.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/extensions/footnotes.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/extensions/smarty.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/extensions/smarty.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/extensions/toc.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/extensions/toc.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/inlinepatterns.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/inlinepatterns.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/treeprocessors.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/treeprocessors.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/markdown-stubs/util.pyi` & `types-Markdown-3.4.2.8/markdown-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.7/setup.py` & `types-Markdown-3.4.2.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Markdown`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Markdown. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fe9eb630eedfc588c57cee51807c505c072c1348`.
+This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.4.2.7",
+      version="3.4.2.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Markdown.md",
```

### Comparing `types-Markdown-3.4.2.7/types_Markdown.egg-info/PKG-INFO` & `types-Markdown-3.4.2.8/types_Markdown.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Markdown
-Version: 3.4.2.7
+Version: 3.4.2.8
 Summary: Typing stubs for Markdown
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Markdown.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Markdown`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Markdown. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fe9eb630eedfc588c57cee51807c505c072c1348`.
+This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
```

### Comparing `types-Markdown-3.4.2.7/types_Markdown.egg-info/SOURCES.txt` & `types-Markdown-3.4.2.8/types_Markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

