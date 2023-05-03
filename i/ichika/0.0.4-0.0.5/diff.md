# Comparing `tmp/ichika-0.0.4.tar.gz` & `tmp/ichika-0.0.5.tar.gz`

## Comparing `ichika-0.0.4.tar` & `ichika-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 ichika-0.0.4/local_dependencies/pyo3-repr/Cargo.toml
--rw-r--r--   0     1001      123     4649 2023-03-17 14:49:27.000000 ichika-0.0.4/local_dependencies/pyo3-repr/src/lib.rs
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 ichika-0.0.4/Cargo.toml
--rw-r--r--   0     1001      123     1639 2023-03-17 14:49:27.000000 ichika-0.0.4/README.md
--rw-r--r--   0     1001      123     2216 2023-03-17 14:49:27.000000 ichika-0.0.4/pyproject.toml
--rw-r--r--   0     1001      123      122 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/__init__.py
--rw-r--r--   0     1001      123     1686 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/client.py
--rw-r--r--   0     1001      123     7614 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/core/__init__.pyi
--rw-r--r--   0     1001      123     1037 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/core/events/__init__.pyi
--rw-r--r--   0     1001      123      409 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/core/events/structs.pyi
--rw-r--r--   0     1001      123      266 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/exceptions.py
--rw-r--r--   0     1001      123     3999 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/login/__init__.py
--rw-r--r--   0     1001      123     3788 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/login/password.py
--rw-r--r--   0     1001      123     4085 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/login/qrcode/__init__.py
--rw-r--r--   0     1001      123      249 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/login/qrcode/render/__init__.py
--rw-r--r--   0     1001      123      794 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/login/qrcode/render/dense1x2.py
--rw-r--r--   0     1001      123      940 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/message/__init__.py
--rw-r--r--   0     1001      123      290 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/message/_sealed.py
--rw-r--r--   0     1001      123     7548 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/message/elements.py
--rw-r--r--   0     1001      123     1462 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/message/serializer.py
--rw-r--r--   0     1001      123        0 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/scripts/__init__.py
--rw-r--r--   0     1001      123     1227 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/scripts/device/__init__.py
--rw-r--r--   0     1001      123     1903 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/scripts/device/converter.py
--rw-r--r--   0     1001      123     5163 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/scripts/device/data.json
--rw-r--r--   0     1001      123     2305 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/scripts/device/generator.py
--rw-r--r--   0     1001      123      437 2023-03-17 14:49:27.000000 ichika-0.0.4/python/ichika/utils.py
--rw-r--r--   0     1001      123     4961 2023-03-17 14:49:27.000000 ichika-0.0.4/src/client/cached.rs
--rw-r--r--   0     1001      123     2947 2023-03-17 14:49:27.000000 ichika-0.0.4/src/client/friend.rs
--rw-r--r--   0     1001      123     2592 2023-03-17 14:49:27.000000 ichika-0.0.4/src/client/group.rs
--rw-r--r--   0     1001      123    17475 2023-03-17 14:49:27.000000 ichika-0.0.4/src/client/mod.rs
--rw-r--r--   0     1001      123     1534 2023-03-17 14:49:27.000000 ichika-0.0.4/src/client/structs.rs
--rw-r--r--   0     1001      123     7448 2023-03-17 14:49:27.000000 ichika-0.0.4/src/events/converter.rs
--rw-r--r--   0     1001      123     3462 2023-03-17 14:49:27.000000 ichika-0.0.4/src/events/mod.rs
--rw-r--r--   0     1001      123     1250 2023-03-17 14:49:27.000000 ichika-0.0.4/src/events/structs.rs
--rw-r--r--   0     1001      123      805 2023-03-17 14:49:27.000000 ichika-0.0.4/src/exc.rs
--rw-r--r--   0     1001      123     2739 2023-03-17 14:49:27.000000 ichika-0.0.4/src/lib.rs
--rw-r--r--   0     1001      123    17342 2023-03-17 14:49:27.000000 ichika-0.0.4/src/login.rs
--rw-r--r--   0     1001      123     6554 2023-03-17 14:49:27.000000 ichika-0.0.4/src/loguru.rs
--rw-r--r--   0     1001      123     6506 2023-03-17 14:49:27.000000 ichika-0.0.4/src/message/convert.rs
--rw-r--r--   0     1001      123     1667 2023-03-17 14:49:27.000000 ichika-0.0.4/src/message/elements.rs
--rw-r--r--   0     1001      123       35 2023-03-17 14:49:27.000000 ichika-0.0.4/src/message/mod.rs
--rw-r--r--   0     1001      123     4277 2023-03-17 14:49:27.000000 ichika-0.0.4/src/utils.rs
--rw-r--r--   0     1001      123    53035 2023-03-17 14:49:27.000000 ichika-0.0.4/Cargo.lock
--rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 ichika-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      253 1970-01-01 00:00:00.000000 ichika-0.0.5/local_dependencies/pyo3-repr/Cargo.toml
+-rw-r--r--   0     1001      123     4379 2023-05-03 10:21:17.000000 ichika-0.0.5/local_dependencies/pyo3-repr/src/lib.rs
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 ichika-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      123     2004 2023-05-03 10:21:17.000000 ichika-0.0.5/README.md
+-rw-r--r--   0     1001      123     3028 2023-05-03 10:21:17.000000 ichika-0.0.5/pyproject.toml
+-rw-r--r--   0     1001      123      231 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/__init__.py
+-rw-r--r--   0     1001      123     1052 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/build_info.py
+-rw-r--r--   0     1001      123     7580 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/client.py
+-rw-r--r--   0     1001      123    19567 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/core.pyi
+-rw-r--r--   0     1001      123     4138 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/event_defs.py
+-rw-r--r--   0     1001      123      266 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/exceptions.py
+-rw-r--r--   0     1001      123     5086 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/graia/__init__.py
+-rw-r--r--   0     1001      123     6990 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/graia/event.py
+-rw-r--r--   0     1001      123     4303 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/login/__init__.py
+-rw-r--r--   0     1001      123     3864 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/login/password.py
+-rw-r--r--   0     1001      123     4115 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/login/qrcode/__init__.py
+-rw-r--r--   0     1001      123      249 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/login/qrcode/render/__init__.py
+-rw-r--r--   0     1001      123      794 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/login/qrcode/render/dense1x2.py
+-rw-r--r--   0     1001      123     1016 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/message/__init__.py
+-rw-r--r--   0     1001      123      290 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/message/_sealed.py
+-rw-r--r--   0     1001      123    13312 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/message/elements.py
+-rw-r--r--   0     1001      123     1913 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/message/serializer.py
+-rw-r--r--   0     1001      123        0 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/scripts/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/scripts/device/__init__.py
+-rw-r--r--   0     1001      123     1903 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/scripts/device/converter.py
+-rw-r--r--   0     1001      123     5163 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/scripts/device/data.json
+-rw-r--r--   0     1001      123     2305 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/scripts/device/generator.py
+-rw-r--r--   0     1001      123     1934 2023-05-03 10:21:17.000000 ichika-0.0.5/python/ichika/utils.py
+-rw-r--r--   0     1001      123     1036 2023-05-03 10:21:17.000000 ichika-0.0.5/src/build_info.rs
+-rw-r--r--   0     1001      123     4961 2023-05-03 10:21:17.000000 ichika-0.0.5/src/client/cached.rs
+-rw-r--r--   0     1001      123     2995 2023-05-03 10:21:17.000000 ichika-0.0.5/src/client/friend.rs
+-rw-r--r--   0     1001      123     2640 2023-05-03 10:21:17.000000 ichika-0.0.5/src/client/group.rs
+-rw-r--r--   0     1001      123     1926 2023-05-03 10:21:17.000000 ichika-0.0.5/src/client/http.rs
+-rw-r--r--   0     1001      123    24702 2023-05-03 10:21:17.000000 ichika-0.0.5/src/client/mod.rs
+-rw-r--r--   0     1001      123     8028 2023-05-03 10:21:17.000000 ichika-0.0.5/src/client/structs.rs
+-rw-r--r--   0     1001      123    12659 2023-05-03 10:21:17.000000 ichika-0.0.5/src/events/converter.rs
+-rw-r--r--   0     1001      123     3897 2023-05-03 10:21:17.000000 ichika-0.0.5/src/events/mod.rs
+-rw-r--r--   0     1001      123     2035 2023-05-03 10:21:17.000000 ichika-0.0.5/src/exc.rs
+-rw-r--r--   0     1001      123     1509 2023-05-03 10:21:17.000000 ichika-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      123     1918 2023-05-03 10:21:17.000000 ichika-0.0.5/src/login/connector.rs
+-rw-r--r--   0     1001      123    17476 2023-05-03 10:21:17.000000 ichika-0.0.5/src/login/mod.rs
+-rw-r--r--   0     1001      123     6514 2023-05-03 10:21:17.000000 ichika-0.0.5/src/loguru.rs
+-rw-r--r--   0     1001      123     9823 2023-05-03 10:21:17.000000 ichika-0.0.5/src/message/convert.rs
+-rw-r--r--   0     1001      123     1667 2023-05-03 10:21:17.000000 ichika-0.0.5/src/message/elements.rs
+-rw-r--r--   0     1001      123       35 2023-05-03 10:21:17.000000 ichika-0.0.5/src/message/mod.rs
+-rw-r--r--   0     1001      123     5393 2023-05-03 10:21:17.000000 ichika-0.0.5/src/utils.rs
+-rw-r--r--   0     1001      123    55974 2023-05-03 10:21:17.000000 ichika-0.0.5/Cargo.lock
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 ichika-0.0.5/PKG-INFO
```

### Comparing `ichika-0.0.4/local_dependencies/pyo3-repr/src/lib.rs` & `ichika-0.0.5/local_dependencies/pyo3-repr/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -94,40 +94,38 @@
 }
 
 fn gen_named_impl(ident: String, fields: &FieldsNamed) -> MacroResult {
     let mut core_stream = pm2::TokenStream::new();
     core_stream.extend(quote!(
         f.debug_struct(#ident)
     ));
-    'field_iter: for f in fields.named.iter() {
+    for f in fields.named.iter() {
         let field_name_ident = f.ident.as_ref().unwrap();
         let field_name_literal = field_name_ident.to_string();
         let mut py_convert = is_py_ptr(&f.ty);
         for attr in f.attrs.iter() {
-            if let Ok(syn::Meta::List(syn::MetaList { ref nested, .. })) = attr.parse_meta() {
-                for arg in nested.iter() {
-                    if let syn::NestedMeta::Meta(meta) = arg
-                    && let syn::Meta::Path(pth) = meta
-                    && let Some(ident) = pth.get_ident() {
-                        match ident.to_string().as_str() {
-                            "skip" => continue 'field_iter,
-                            "py" => {
-                                py_convert = true;
-                            }
-                            "debug" => {
-                                py_convert = false;
-                            }
-                            _ => return Err(syn::Error::new_spanned(arg, "Unexpected arg")),
-                        }
+            attr.parse_nested_meta(|meta| {
+                let ident = meta.path.get_ident().ok_or_else(|| {
+                    syn::Error::new_spanned(
+                        meta.path.clone(),
+                        "py_repr only supports bare ident as arg.",
+                    )
+                })?;
+                match ident.to_string().as_str() {
+                    "skip" => return Ok(()),
+                    "py" => {
+                        py_convert = true;
                     }
-                    else{
-                        return Err(syn::Error::new_spanned(arg, "py_repr only supports bare ident as arg."))
+                    "debug" => {
+                        py_convert = false;
                     }
+                    _ => return Err(syn::Error::new_spanned(ident, "Unexpected option")),
                 }
-            }
+                Ok(())
+            })?;
         }
         if py_convert {
             core_stream.extend(quote!(
                 .field(#field_name_literal, self.#field_name_ident.as_ref(py))
             ));
         } else {
             core_stream.extend(quote!(
```

### Comparing `ichika-0.0.4/README.md` & `ichika-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,32 @@
 [![PyPI](https://img.shields.io/pypi/v/ichika)](https://github.com/BlueGlassBlock/ichika/blob/master/CHANGELOG.md)
 [![Python Version](https://img.shields.io/pypi/pyversions/ichika)](https://pypi.org/project/ichika)
 [![License](https://img.shields.io/github/license/BlueGlassBlock/Ichika)](https://github.com/BlueGlassBlock/Ichika/blob/master/LICENSE)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
+[![Deploy Docs](https://github.com/BlueGlassBlock/Ichika/actions/workflows/deploy-docs.yml/badge.svg)](https://github.comBlueGlassBlock/Ichika/actions/workflows/deploy-docs.yml/badge.svg)
 [![Run CI](https://github.com/BlueGlassBlock/Ichika/actions/workflows/ci.yml/badge.svg)](https://github.com/BlueGlassBlock/Ichika/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/BlueGlassBlock/Ichika/master.svg)](https://results.pre-commit.ci/latest/github/BlueGlassBlock/Ichika/master)
 
 </div>
 
+## 示例
+
+请参阅 [example.py](./example.py)，它包含了一个识别指定指令并发送图片的简单示例。
+
+<!-- start docs-include -->
+
 ## 鸣谢
 
 - [AWR](https://github.com/wybxc/awr): Ichika 的前身和部分代码来源
 - [ricq](https://github.com/lz1998/ricq): 使用 Rust 实现的高性能 QQ 协议 移植于 [OICQ](https://github.com/takayama-lily/oicq)
 - [mirai](https://github.com/mamoe/mirai): 高效率 QQ 机器人支持库
 - [PyO3](https://github.com/PyO3/PyO3): Python 解释器的 Rust 绑定
 - [GraiaProject](https://github.com/GraiaProject): 用于 Bot 开发的一系列高效, 现代化, 充分可扩展的工具链
 
 ## 许可证
 
 `Ichika` 使用 [`GNU AGPL-3.0`](https://choosealicense.com/licenses/agpl-3.0/) 作为许可证，这意味着你需要遵守相应的规则。
+
+<!-- end docs-include -->
```

### Comparing `ichika-0.0.4/pyproject.toml` & `ichika-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -16,35 +16,36 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 
 dependencies = [
     "loguru~=0.6.0",
-    "graia-broadcast>=0.19.0",
-    "creart-graia>=0.1.5",
     "dacite>=1.6.0",
     "graia-amnesia>=0.7.0",
     "aiohttp>=3.8.3",
 ]
 
 dynamic = ["version"]
-
 [project.optional-dependencies]
-kayaku = [
-    "kayaku>=0.5.0",
+graia = [
+    "graia-broadcast>=0.19.2",
+    "launart>=0.6.3",
+    "creart>=0.2.2",
+    "creart-graia>=0.1.5",
+    "graiax-shortcut>=0.2.1",
 ]
 
-
 [build-system]
-requires = ["maturin>=0.13,<0.14"]
+requires = ["maturin>=0.14.16,<0.15"]
 build-backend = "maturin"
 
 [tool.maturin]
 python-source = "python"
+module-name = "ichika.core"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 py_version = 38
@@ -89,7 +90,41 @@
 name = "修复"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
 name = "其他"
 showcontent = true
+
+[tool.pdm]
+[tool.pdm.dev-dependencies]
+lint = [
+    "black>=23.1.0",
+    "isort>=5.12.0",
+    "pre-commit>=3.2.1",
+]
+release = [
+    "towncrier>=22.12.0",
+    "maturin>=0.14.16",
+    "tomlkit>=0.11.6",
+    "actions-toolkit>=0.1.15",
+]
+docs = [
+    "mkdocs-material~=9.1",
+    "mkdocstrings[python]~=0.21",
+    "mkdocs-exclude~=1.0",
+    "mkdocs-gen-files~=0.4",
+    "mkdocs-section-index~=0.3",
+    "mkdocs-literate-nav~=0.6",
+    "markdown-exec[ansi]>=1.4.0",
+    "mkdocs-include-markdown-plugin>=3.9.1",
+]
+dev = [
+    "maturin>=0.14.16",
+    "pip>=23.0.1",
+    "graia-saya>=0.0.17",
+    "graiax-shortcut>=0.2.1",
+]
+[tool.pdm.scripts]
+develop.cmd = "maturin develop"
+build-docs.cmd = "mkdocs build"
+view-docs.cmd = "mkdocs serve"
```

### Comparing `ichika-0.0.4/python/ichika/login/__init__.py` & `ichika-0.0.5/python/ichika/login/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 from __future__ import annotations
 
 import json
 import os
 from asyncio import Queue
 from enum import Enum
 from pathlib import Path
-from typing import Literal, Optional, Union, overload
+from typing import Literal, Optional, Sequence, Union, overload
 
 from loguru import logger as log
 
 import ichika.core as _core
 from ichika.client import Client
 
 from .password import PasswordLoginCallbacks as PasswordLoginCallbacks
 from .qrcode import QRCodeLoginCallbacks as QRCodeLoginCallbacks
 
 
-class Protocol(str, Enum):
-    IPad = "IPad"
-    AndroidPhone = "AndroidPhone"
-    AndroidWatch = "AndroidWatch"
-    MacOS = "MacOS"
-    QiDian = "QiDian"
-
-
 class BaseLoginCredentialStore:
-    def get_token(self, uin: int, protocol: Protocol) -> Optional[bytes]:
+    def get_token(self, uin: int, protocol: str) -> Optional[bytes]:
         pass
 
-    def write_token(self, uin: int, protocol: Protocol, token: bytes) -> None:
+    def write_token(self, uin: int, protocol: str, token: bytes) -> None:
         pass
 
-    def get_device(self, uin: int, protocol: Protocol) -> dict:
+    def get_device(self, uin: int, protocol: str) -> dict:
         from dataclasses import asdict
         from random import Random
 
         from ichika.scripts.device.generator import generate
 
         return asdict(generate(Random(hash(protocol) ^ uin)))
 
@@ -48,15 +40,15 @@
         self.path.mkdir(parents=True, exist_ok=True)
 
     def uin_path(self, uin: int) -> Path:
         path = self.path / str(uin)
         path.mkdir(parents=True, exist_ok=True)
         return path
 
-    def get_device(self, uin: int, protocol: Protocol) -> dict:
+    def get_device(self, uin: int, protocol: str) -> dict:
         ricq_device = self.uin_path(uin) / "ricq_device.json"
         if ricq_device.exists():
             log.info("发现 `ricq_device.json`, 读取")
             return json.loads(ricq_device.read_text("utf-8"))
 
         other_device = self.uin_path(uin) / "device.json"
         if other_device.exists():
@@ -69,66 +61,84 @@
         else:
             log.info("未发现 `device.json`, 正在生成")
             device_content = super().get_device(uin, protocol)
 
         ricq_device.write_text(json.dumps(device_content, indent=4), "utf-8")
         return device_content
 
-    def get_token(self, uin: int, protocol: Protocol) -> Optional[bytes]:
-        token = self.uin_path(uin) / f"token-{protocol.value}.bin"
+    def get_token(self, uin: int, protocol: str) -> Optional[bytes]:
+        token = self.uin_path(uin) / f"token-{protocol}.bin"
         return token.read_bytes() if token.exists() else None
 
-    def write_token(self, uin: int, protocol: Protocol, token: bytes) -> None:
-        token_path = self.uin_path(uin) / f"token-{protocol.value}.bin"
+    def write_token(self, uin: int, protocol: str, token: bytes) -> None:
+        token_path = self.uin_path(uin) / f"token-{protocol}.bin"
         token_path.write_bytes(token)
 
 
 @overload
 async def login_password(
     uin: int,
     password: str,
     /,
-    protocol: Protocol,
+    protocol: str,
     store: BaseLoginCredentialStore,
-    queues: list[Queue],
-    callbacks: PasswordLoginCallbacks = ...,
+    event_callbacks: Sequence[_core.EventCallback],
+    login_callbacks: PasswordLoginCallbacks | None = None,
     use_sms: bool = ...,
 ) -> Client:
     ...
 
 
 @overload
 async def login_password(
     uin: int,
     password_md5: bytes,
     /,
-    protocol: Protocol,
+    protocol: str,
+    store: BaseLoginCredentialStore,
+    event_callbacks: Sequence[_core.EventCallback],
+    login_callbacks: PasswordLoginCallbacks | None = None,
+    use_sms: bool = ...,
+) -> Client:
+    ...
+
+
+@overload
+async def login_password(
+    uin: int,
+    credential: str | bytes,
+    /,
+    protocol: str,
     store: BaseLoginCredentialStore,
-    queues: list[Queue],
-    callbacks: PasswordLoginCallbacks = ...,
+    event_callbacks: Sequence[_core.EventCallback],
+    login_callbacks: PasswordLoginCallbacks | None = None,
     use_sms: bool = ...,
 ) -> Client:
     ...
 
 
 async def login_password(
     uin: int,
-    credential: Union[str, bytes],
+    credential: str | bytes,
     /,
-    protocol: Protocol,
+    protocol: str,
     store: BaseLoginCredentialStore,
-    queues: list[Queue],
-    callbacks: PasswordLoginCallbacks = PasswordLoginCallbacks.default(),
+    event_callbacks: Sequence[_core.EventCallback],
+    login_callbacks: PasswordLoginCallbacks | None = None,
     use_sms: bool = True,
 ) -> Client:
-    return await _core.password_login(uin, credential, use_sms, protocol, store, queues, callbacks)
+    return await _core.password_login(
+        uin, credential, use_sms, protocol, store, event_callbacks, login_callbacks or PasswordLoginCallbacks.default()
+    )
 
 
 async def login_qrcode(
     uin: int,
     /,
-    protocol: Literal[Protocol.AndroidWatch, Protocol.MacOS],
+    protocol: Literal["AndroidWatch"],
     store: BaseLoginCredentialStore,
-    queues: list[Queue],
-    callbacks: QRCodeLoginCallbacks = QRCodeLoginCallbacks.default(),
+    event_callbacks: Sequence[_core.EventCallback],
+    login_callbacks: QRCodeLoginCallbacks | None = None,
 ) -> Client:
-    return await _core.qrcode_login(uin, protocol, store, queues, callbacks)
+    return await _core.qrcode_login(
+        uin, protocol, store, event_callbacks, login_callbacks or QRCodeLoginCallbacks.default()
+    )
```

### Comparing `ichika-0.0.4/python/ichika/login/password.py` & `ichika-0.0.5/python/ichika/login/password.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from enum import auto
 from typing import Any, Callable, Literal, NoReturn, Optional, overload
 from typing_extensions import Self
 
 from loguru import logger as log
 
-from ichika.utils import AutoEnum
-from ichika.utils import Decor as Decor
+from ichika.utils import AsyncFn, AutoEnum, Decor
 
 
 class PasswordLoginState(str, AutoEnum):
     Success = auto()
     AccountFrozen = auto()
     TooManySMSRequest = auto()
     DeviceLockLogin = auto()
@@ -23,52 +22,52 @@
 
 class PasswordLoginCallbacks:
     def __init__(self, callbacks: dict[PasswordLoginState, Callable] | None = None):
         self.callbacks: dict[PasswordLoginState, Optional[Callable]] = {state: None for state in PasswordLoginState}
         self.callbacks.update(callbacks or {})
 
     @overload
-    def set_handle(self, state: Literal[PasswordLoginState.DeviceLocked]) -> Decor[Callable[[str, str], Any]]:
+    def set_handle(self, state: Literal[PasswordLoginState.DeviceLocked]) -> Decor[AsyncFn[[str, str], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[PasswordLoginState.RequestSMS]) -> Decor[Callable[[str, str], str]]:
+    def set_handle(self, state: Literal[PasswordLoginState.RequestSMS]) -> Decor[AsyncFn[[str, str], str]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[PasswordLoginState.NeedCaptcha]) -> Decor[Callable[[str], str]]:
+    def set_handle(self, state: Literal[PasswordLoginState.NeedCaptcha]) -> Decor[AsyncFn[[str], str]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[PasswordLoginState.Success]) -> Decor[Callable[[], Any]]:
+    def set_handle(self, state: Literal[PasswordLoginState.Success]) -> Decor[AsyncFn[[], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[PasswordLoginState.DeviceLockLogin]) -> Decor[Callable[[], Any]]:
+    def set_handle(self, state: Literal[PasswordLoginState.DeviceLockLogin]) -> Decor[AsyncFn[[], Any]]:
         ...
 
     @overload
     def set_handle(
         self,
         state: Literal[PasswordLoginState.AccountFrozen],
-    ) -> Decor[Callable[[], NoReturn]]:
+    ) -> Decor[AsyncFn[[], NoReturn]]:
         ...
 
     @overload
     def set_handle(
         self,
         state: Literal[PasswordLoginState.TooManySMSRequest],
-    ) -> Decor[Callable[[], NoReturn]]:
+    ) -> Decor[AsyncFn[[], NoReturn]]:
         ...
 
     @overload
     def set_handle(
         self,
         state: Literal[PasswordLoginState.UnknownStatus],
-    ) -> Decor[Callable[[str, int], NoReturn]]:
+    ) -> Decor[AsyncFn[[str, int], NoReturn]]:
         ...
 
     def set_handle(self, state) -> Decor[Callable]:
         def register_callback(func: Callable) -> Callable:
             self.callbacks[state] = func
             return func
 
@@ -79,41 +78,47 @@
 
     @classmethod
     def default(cls) -> Self:
         cbs = cls({})
         S = PasswordLoginState
 
         @cbs.set_handle(S.NeedCaptcha)
-        def _(url: str):
+        async def _(url: str):
             log.warning(f"请完成滑块验证，URL: {url}")
             return input("完成后请输入 ticket >").strip(" ")
 
         @cbs.set_handle(S.DeviceLocked)
-        def _(message: str, url: str):
+        async def _(message: str, url: str):
             log.warning(message)
             log.warning(f"请完成设备锁验证，URL: {url}")
             input("请在完成后回车")
 
         @cbs.set_handle(S.RequestSMS)
-        def _(message: str, phone_number: str) -> str:
+        async def _(message: str, phone_number: str) -> str:
             log.warning(message)
             log.warning(f"已发送短信验证码至 {phone_number}")
             return input("请输入收到的短信验证码 >").strip(" ")
 
         @cbs.set_handle(S.AccountFrozen)
-        def _() -> NoReturn:
+        async def _() -> NoReturn:
             msg = "无法登录：账号被冻结"
             raise RuntimeError(msg)
 
         @cbs.set_handle(S.TooManySMSRequest)
-        def _() -> NoReturn:
+        async def _() -> NoReturn:
             msg = "短信请求次数过多，请稍后再试"
             raise RuntimeError(msg)
 
         @cbs.set_handle(S.UnknownStatus)
-        def _(message: str, code: int) -> NoReturn:
+        async def _(message: str, code: int) -> NoReturn:
             msg = f"未知错误（代码 {code}）：{message}"
             raise RuntimeError(msg)
 
-        cbs.set_handle(S.Success)(lambda: log.success("登录成功"))
-        cbs.set_handle(S.DeviceLockLogin)(lambda: log.info("尝试设备锁登录"))
+        @cbs.set_handle(S.Success)
+        async def _() -> None:
+            log.success("登录成功")
+
+        @cbs.set_handle(S.DeviceLockLogin)
+        async def _() -> None:
+            log.info("尝试设备锁登录")
+
         return cbs
```

### Comparing `ichika-0.0.4/python/ichika/login/qrcode/__init__.py` & `ichika-0.0.5/python/ichika/login/qrcode/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from enum import auto
 from typing import Any, Callable, Literal, Optional, overload
 from typing_extensions import Self
 
 from loguru import logger as log
 
-from ichika.utils import AutoEnum, Decor, P, Ref
+from ichika.utils import AsyncFn, AutoEnum, Decor, P, Ref
 
 from .render import Dense1x2 as Dense1x2
 from .render import QRCodeRenderer as QRCodeRenderer
 
 
 class QRCodeLoginState(str, AutoEnum):
     WaitingForScan = auto()
@@ -25,39 +25,39 @@
 class QRCodeLoginCallbacks:
     def __init__(self, callbacks: dict[QRCodeLoginState, Callable] | None = None, interval: float = 5.0):
         self.callbacks: dict[QRCodeLoginState, Optional[Callable]] = {state: None for state in QRCodeLoginState}
         self.callbacks.update(callbacks or {})
         self.interval: float = interval
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.WaitingForScan]) -> Decor[Callable[[], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.WaitingForScan]) -> Decor[AsyncFn[[], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.WaitingForConfirm]) -> Decor[Callable[[], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.WaitingForConfirm]) -> Decor[AsyncFn[[], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.Canceled]) -> Decor[Callable[[], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.Canceled]) -> Decor[AsyncFn[[], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.Timeout]) -> Decor[Callable[[], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.Timeout]) -> Decor[AsyncFn[[], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.Success]) -> Decor[Callable[[int], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.Success]) -> Decor[AsyncFn[[int], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.UINMismatch]) -> Decor[Callable[[int, int], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.UINMismatch]) -> Decor[AsyncFn[[int, int], Any]]:
         ...
 
     @overload
-    def set_handle(self, state: Literal[QRCodeLoginState.DisplayQRCode]) -> Decor[Callable[[list[list[bool]]], Any]]:
+    def set_handle(self, state: Literal[QRCodeLoginState.DisplayQRCode]) -> Decor[AsyncFn[[list[list[bool]]], Any]]:
         ...
 
     def set_handle(self, state) -> Decor[Callable]:
         def register_callback(func: Callable) -> Callable:
             self.callbacks[state] = func
             return func
 
@@ -69,20 +69,20 @@
     @classmethod
     def default(cls, qrcode_printer: QRCodeRenderer = Dense1x2(), interval: float = 5.0, merge: bool = True) -> Self:
         cbs = QRCodeLoginCallbacks(interval=interval)
         S = QRCodeLoginState
 
         last_state: Ref[Optional[S]] = Ref(None)
 
-        def wrap(state: S) -> Decor[Callable[P, None]]:
-            def receiver(func: Callable[P, None]) -> Callable[P, None]:
+        def wrap(state: S) -> Callable[[Callable[P, None]], AsyncFn[P, None]]:
+            def receiver(func: Callable[P, None]) -> AsyncFn[P, None]:
                 import functools
 
                 @functools.wraps(func)
-                def wrapper(*args: P.args, **kwargs: P.kwargs) -> None:
+                async def wrapper(*args: P.args, **kwargs: P.kwargs) -> None:
                     if last_state.ref == state and merge:
                         return
                     last_state.ref = state
                     return func(*args, **kwargs)
 
                 return wrapper
```

### Comparing `ichika-0.0.4/python/ichika/login/qrcode/render/dense1x2.py` & `ichika-0.0.5/python/ichika/login/qrcode/render/dense1x2.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/python/ichika/message/__init__.py` & `ichika-0.0.5/python/ichika/message/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 from typing import Any
 
 from graia.amnesia.message import MessageChain
 from graia.amnesia.message.element import Element, Unknown
+from loguru import logger
 
-from .elements import TYPE_MAP
-from .serializer import SERIALIZE_INV
+from .elements import _DESERIALIZE_INV
+from .serializer import _SERIALIZE_INV
 
 
-def deserialize_message(elements: list[dict[str, Any]]) -> MessageChain:
+def _deserialize_message(elements: list[dict[str, Any]]) -> MessageChain:
     elem_seq: list[Element] = []
     for e_data in elements:
-        cls = TYPE_MAP.get(e_data.pop("type"), None)
+        cls = _DESERIALIZE_INV.get(e_data.pop("type"), None)
         if cls is None:
-            print(e_data)
+            logger.warning(f"未知元素: {e_data!r}")
             elem_seq.append(Unknown("Unknown", e_data))
         else:
             elem_seq.append(cls(**e_data))
     return MessageChain(elem_seq)
 
 
-def serialize_message(chain: MessageChain) -> list[dict[str, Any]]:
+def _serialize_message(chain: MessageChain) -> list[dict[str, Any]]:
     res: list[dict[str, Any]] = []
     for elem in chain:
-        if serializer := SERIALIZE_INV.get(elem.__class__):
+        if serializer := _SERIALIZE_INV.get(elem.__class__):
             res.append(serializer(elem))
         else:
-            raise TypeError(f"无法发送元素 {elem!r}")
+            raise TypeError(f"无法转换元素 {elem!r}")
     return res
```

### Comparing `ichika-0.0.4/python/ichika/message/serializer.py` & `ichika-0.0.5/python/ichika/message/serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,53 +10,61 @@
 from .elements import (
     At,
     AtAll,
     Dice,
     Face,
     FingerGuessing,
     FlashImage,
+    ForwardCard,
     Image,
+    LightApp,
     MarketFace,
+    Reply,
+    RichMessage,
 )
 
-SERIALIZE_INV: dict[type, Callable[[Any], dict[str, Any]]] = {}
+_SERIALIZE_INV: dict[type, Callable[[Any], dict[str, Any]]] = {}
 
 Elem_T = TypeVar("Elem_T", bound=Element)
 
 
 def _serialize(
     elem_type: type[Elem_T],
 ) -> Decor[Callable[[Elem_T], dict[str, Any]]]:
     def func_register(func: Callable[[Elem_T], dict[str, Any]]) -> Callable[[Elem_T], dict[str, Any]]:
         @functools.wraps(func)
         def wrapper(elem: Elem_T) -> dict[str, Any]:
             res = func(elem)
             res.setdefault("type", elem.__class__.__name__)
             return res
 
-        SERIALIZE_INV[elem_type] = wrapper
+        _SERIALIZE_INV[elem_type] = wrapper
         return func
 
     return func_register
 
 
+_serialize(Reply)(lambda t: {"seq": t.seq, "sender": t.sender, "time": int(t.time.timestamp()), "content": t.content})
 _serialize(Text)(lambda t: {"text": t.text})
 _serialize(AtAll)(lambda _: {})
 _serialize(At)(lambda t: {"target": t.target})
 _serialize(Dice)(lambda t: {"value": t.value})
 _serialize(FingerGuessing)(lambda t: {"choice": t.choice.name})
 _serialize(Face)(lambda t: {"index": t.index})
 _serialize(MarketFace)(lambda t: {"raw": t.raw})
+_serialize(LightApp)(lambda t: {"content": t.content})
+_serialize(RichMessage)(lambda t: {"service_id": t.service_id, "content": t.content})
+_serialize(ForwardCard)(lambda t: {"service_id": 35, "content": t.content})
 
 
 @_serialize(Image)
-def _(i: Image):
-    if i.raw is None:
+def _serialize_image(elem: Image):
+    if elem.raw is None:
         raise ValueError
-    return {"raw": i.raw}
+    return {"raw": elem.raw}
 
 
 @_serialize(FlashImage)
-def _(i: FlashImage):
-    if i.raw is None:
+def _serialize_flash_image(elem: FlashImage):
+    if elem.raw is None:
         raise ValueError
-    return {"raw": i.raw}
+    return {"raw": elem.raw}
```

### Comparing `ichika-0.0.4/python/ichika/scripts/device/__init__.py` & `ichika-0.0.5/python/ichika/scripts/device/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/python/ichika/scripts/device/converter.py` & `ichika-0.0.5/python/ichika/scripts/device/converter.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/python/ichika/scripts/device/data.json` & `ichika-0.0.5/python/ichika/scripts/device/data.json`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/python/ichika/scripts/device/generator.py` & `ichika-0.0.5/python/ichika/scripts/device/generator.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/src/client/cached.rs` & `ichika-0.0.5/src/client/cached.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/src/client/friend.rs` & `ichika-0.0.5/src/client/friend.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use pyo3::prelude::*;
 use pyo3::types::*;
 use pyo3_repr::PyRepr;
 use ricq::structs::{FriendGroupInfo, FriendInfo};
 use ricq_core::command::friendlist::FriendListResponse;
 
-#[pyclass(get_all)]
+#[pyclass(get_all, module = "ichika.core")]
 #[derive(PyRepr, Clone)]
 pub struct Friend {
     pub uin: i64,
     pub nick: String,
     pub remark: String,
     pub face_id: i16,
     pub group_id: u8,
@@ -24,15 +24,15 @@
             remark: info.remark,
             face_id: info.face_id,
             group_id: info.group_id,
         }
     }
 }
 
-#[pyclass(get_all)]
+#[pyclass(get_all, module = "ichika.core")]
 #[derive(PyRepr, Clone)]
 pub struct FriendGroup {
     pub group_id: u8,
     pub name: String,
     pub total_count: i32,
     pub online_count: i32,
     pub seq_id: u8,
```

### Comparing `ichika-0.0.4/src/client/group.rs` & `ichika-0.0.5/src/client/group.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use pyo3::prelude::*;
 use pyo3_repr::PyRepr;
 use ricq::structs::{GroupInfo, GroupMemberInfo};
-#[pyclass(get_all)]
+#[pyclass(get_all, module = "ichika.core")]
 #[derive(PyRepr, Clone)]
 pub struct Group {
     pub uin: i64,
     pub name: String,
     pub memo: String,
     pub owner_uin: i64,
     pub create_time: u32,
@@ -49,15 +49,15 @@
             global_mute_timestamp: shut_up_timestamp,
             mute_timestamp: my_shut_up_timestamp,
             last_msg_seq, // TODO: maybe `Option`?
         }
     }
 }
 
-#[pyclass(get_all)]
+#[pyclass(get_all, module = "ichika.core")]
 #[derive(PyRepr, Clone)]
 pub struct Member {
     pub group_uin: i64,
     pub uin: i64,
     pub gender: u8,
     pub nickname: String,
     pub card_name: String,
```

### Comparing `ichika-0.0.4/src/client/mod.rs` & `ichika-0.0.5/src/client/mod.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 mod cached;
 pub mod friend;
 pub mod group;
+mod http;
 pub mod structs;
 use std::sync::Arc;
 use std::time::Duration;
 
-pub use cached::cache;
+pub use cached::{cache, ClientCache};
 use group::Group;
+use http::get_rust_client;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::*;
 use ricq::msg::elem::RQElem;
-use ricq::structs::{ProfileDetailUpdate, Status};
+use ricq::structs::{ForwardMessage, FriendAudio, GroupAudio, ProfileDetailUpdate, Status};
 use structs::*;
 use tokio::task::JoinHandle;
 
 use crate::login::{reconnect, TokenRW};
-use crate::message::convert::{deserialize_message_chain, serialize_element};
-use crate::utils::{py_future, py_none, py_use, AsPython};
-#[pyclass(subclass)]
+use crate::message::convert::{
+    deserialize_message_chain,
+    render_forward,
+    serialize_audio_dict,
+    serialize_element,
+    serialize_forward,
+};
+use crate::message::elements::SealedAudio;
+use crate::utils::{py_future, py_none, py_try, py_use, AsPython};
+
+#[pyclass(subclass, weakref, module = "ichika.core")]
 pub struct PlumbingClient {
     client: Arc<ricq::client::Client>,
     alive: Option<JoinHandle<()>>,
     #[pyo3(get)]
     uin: i64,
     token_rw: TokenRW,
 }
@@ -57,15 +67,17 @@
         let client = self.client.clone();
         let token_rw = self.token_rw.clone();
         let alive = self.alive.take();
         let uin = self.uin;
         py_future(py, async move {
             if let Some(mut alive) = alive {
                 loop {
-                    alive.await?;
+                    alive
+                        .await
+                        .map_err(|e| Box::new(e) as Box<dyn std::error::Error>)?;
 
                     // 断线重连
                     if let Some(handle) = reconnect(&client, &token_rw).await? {
                         alive = handle;
                     } else {
                         break;
                     }
@@ -82,14 +94,17 @@
             .online
             .load(std::sync::atomic::Ordering::Acquire)
     }
 
     pub fn stop<'py>(&self, py: Python<'py>) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         py_future(py, async move {
+            client
+                .update_online_status(ricq::structs::OnlineStatus::Offline)
+                .await?;
             client.stop(ricq::client::NetworkStatus::Stop);
             Ok(())
         })
     }
 
     pub fn get_account_info<'py>(&self, py: Python<'py>) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
@@ -175,14 +190,31 @@
     ) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         py_future(py, async move {
             client.update_online_status(Status::from(status)).await?;
             Ok(())
         })
     }
+
+    pub fn image_ocr<'py>(
+        &self,
+        py: Python<'py>,
+        url: String,
+        md5: String,
+        weight: i32,
+        height: i32,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        py_future(py, async move {
+            let resp = client
+                .image_ocr(url, md5, weight * height, weight, height)
+                .await?;
+            Ok(OCRResult::from(resp).obj())
+        })
+    }
 }
 
 #[pymethods]
 impl PlumbingClient {
     pub fn get_friend_list<'py>(&self, py: Python<'py>) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         py_future(py, async move {
@@ -466,75 +498,205 @@
         uin: i64,
         data: Py<PyBytes>,
     ) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         py_future(py, async move {
             let data: Vec<u8> = py_use(|py| data.as_bytes(py).into());
             let image = client.upload_friend_image(uin, &data).await?;
-            Ok(py_use(|py| {
-                serialize_element(py, RQElem::FriendImage(image)).into_py(py)
-            }))
+            Ok(py_try(|py| {
+                Ok(serialize_element(py, RQElem::FriendImage(image))?.into_py(py))
+            })?)
         })
     }
 
-    pub fn send_friend_message<'py>(
+    pub fn upload_friend_audio<'py>(
         &self,
         py: Python<'py>,
         uin: i64,
-        chain: &'py PyList,
+        data: Py<PyBytes>,
     ) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
-        let chain = deserialize_message_chain(chain)?;
         py_future(py, async move {
-            let ricq::structs::MessageReceipt { seqs, rands, time } =
-                client.send_friend_message(uin, chain).await?;
-            Ok(Python::with_gil(|py| RawMessageReceipt {
-                seqs: PyTuple::new(py, seqs).into_py(py),
-                rands: PyTuple::new(py, rands).into_py(py),
-                time,
-                kind: "friend".into(),
-                target: uin,
-            }))
+            let data: Vec<u8> = py_use(|py| data.as_bytes(py).into());
+            let audio = client
+                .upload_friend_audio(uin, &data, std::time::Duration::from_secs(0))
+                .await?;
+            let client_uin = client.uin().await;
+            let url = client
+                .get_friend_audio_url(client_uin, audio.clone())
+                .await?;
+            Ok(py_try(|py| {
+                Ok(serialize_audio_dict(py, url, &audio.0)?.obj())
+            })?)
         })
     }
 
     pub fn upload_group_image<'py>(
         &self,
         py: Python<'py>,
         uin: i64,
         data: Py<PyBytes>,
     ) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         py_future(py, async move {
             let data: Vec<u8> = py_use(|py| data.as_bytes(py).into());
             let image = client.upload_group_image(uin, &data).await?;
-            Ok(py_use(|py| {
-                serialize_element(py, RQElem::GroupImage(image)).into_py(py)
-            }))
+            Ok(py_try(|py| {
+                Ok(serialize_element(py, RQElem::GroupImage(image))?.into_py(py))
+            })?)
+        })
+    }
+
+    pub fn upload_group_audio<'py>(
+        &self,
+        py: Python<'py>,
+        uin: i64,
+        data: Py<PyBytes>,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        py_future(py, async move {
+            let data: Vec<u8> = py_use(|py| data.as_bytes(py).into());
+            let audio = client.upload_group_audio(uin, &data, 1).await?;
+            let url = client.get_group_audio_url(uin, audio.clone()).await?;
+            Ok(py_try(|py| {
+                Ok(serialize_audio_dict(py, url, &audio.0)?.obj())
+            })?)
+        })
+    }
+
+    pub fn send_friend_audio<'py>(
+        &self,
+        py: Python<'py>,
+        uin: i64,
+        audio: PyObject,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        let ptt = audio.extract::<SealedAudio>(py)?.inner;
+        py_future(py, async move {
+            let receipt = client.send_friend_audio(uin, FriendAudio(ptt)).await?;
+            Ok(RawMessageReceipt::new(receipt, "friend", uin)?)
+        })
+    }
+
+    pub fn send_group_audio<'py>(
+        &self,
+        py: Python<'py>,
+        uin: i64,
+        audio: PyObject,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        let ptt = audio.extract::<SealedAudio>(py)?.inner;
+        py_future(py, async move {
+            let receipt = client.send_group_audio(uin, GroupAudio(ptt)).await?;
+            Ok(RawMessageReceipt::new(receipt, "group", uin)?)
+        })
+    }
+
+    pub fn send_friend_music_share<'py>(
+        &self,
+        py: Python<'py>,
+        uin: i64,
+        share: MusicShareParam,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        let (music_share, music_version) = share.try_into()?;
+        py_future(py, async move {
+            client
+                .send_friend_music_share(uin, music_share, music_version)
+                .await?;
+            Ok(RawMessageReceipt::empty("group", uin)?)
+        })
+    }
+
+    pub fn send_group_music_share<'py>(
+        &self,
+        py: Python<'py>,
+        uin: i64,
+        share: MusicShareParam,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        let (music_share, music_version) = share.try_into()?;
+        py_future(py, async move {
+            client
+                .send_group_music_share(uin, music_share, music_version)
+                .await?;
+            // TODO: Immediate listen hook
+            // LINK: https://github.com/Mrs4s/MiraiGo/blob/f8d9841755b579f7c95ed918d23b767e3854553a/client/richmsg.go#L71
+            Ok(RawMessageReceipt::empty("group", uin)?)
+        })
+    }
+
+    pub fn upload_forward_msg<'py>(
+        &self,
+        py: Python<'py>,
+        group_uin: i64,
+        msgs: Vec<PyForwardMessage>,
+    ) -> PyResult<&'py PyAny> {
+        use ricq_core::command::multi_msg::gen_forward_preview;
+
+        let client = self.client.clone();
+        let msgs: Vec<ForwardMessage> = msgs.into_iter().map(|v| v.try_into()).try_collect()?;
+        let preview = gen_forward_preview(&msgs);
+        let summary = format!("查看 {} 条转发消息", msgs.len());
+        let file_name: String = "MultiMsg".into();
+
+        py_future(py, async move {
+            let res_id = client.upload_msgs(group_uin, msgs, false).await?;
+            let content = render_forward(&file_name, &res_id, &preview, &summary);
+            Ok((res_id, file_name, content))
+        })
+    }
+
+    pub fn download_forward_msg<'py>(
+        &self,
+        py: Python<'py>,
+        downloader: &'py PyAny,
+        res_id: String,
+    ) -> PyResult<&'py PyAny> {
+        let mut http_client = get_rust_client(py, downloader)?;
+        let client = self.client.clone();
+
+        py_future(py, async move {
+            let msgs = client.download_msgs(res_id, &mut http_client).await?;
+            Ok(py_try(|py| {
+                msgs.into_iter()
+                    .map(|msg| serialize_forward(py, msg).map(|ok| ok.into_py(py)))
+                    .try_collect::<Vec<PyObject>>()
+            })?)
+        })
+    }
+}
+
+#[pymethods]
+impl PlumbingClient {
+    pub fn send_friend_message<'py>(
+        &self,
+        py: Python<'py>,
+        uin: i64,
+        chain: &'py PyList,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        let chain = deserialize_message_chain(chain)?;
+        py_future(py, async move {
+            let receipt = client.send_friend_message(uin, chain).await?;
+            Ok(RawMessageReceipt::new(receipt, "friend", uin)?)
         })
     }
 
     pub fn send_group_message<'py>(
         &self,
         py: Python<'py>,
         uin: i64,
         chain: &'py PyList,
     ) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         let chain = deserialize_message_chain(chain)?;
         py_future(py, async move {
-            let ricq::structs::MessageReceipt { seqs, rands, time } =
-                client.send_group_message(uin, chain).await?;
-            Ok(Python::with_gil(|py| RawMessageReceipt {
-                seqs: PyTuple::new(py, seqs).into_py(py),
-                rands: PyTuple::new(py, rands).into_py(py),
-                time,
-                kind: "group".into(),
-                target: uin,
-            }))
+            let receipt = client.send_group_message(uin, chain).await?;
+            Ok(RawMessageReceipt::new(receipt, "group", uin)?)
         })
     }
 
     pub fn recall_friend_message<'py>(
         &self,
         py: Python<'py>,
         uin: i64,
@@ -577,9 +739,89 @@
     ) -> PyResult<&'py PyAny> {
         let client = self.client.clone();
         py_future(py, async move {
             client.operate_group_essence(uin, seq, rand, flag).await?;
             Ok(())
         })
     }
-    // TODO: Send audio
+}
+
+#[pymethods]
+impl PlumbingClient {
+    #[allow(clippy::too_many_arguments, reason = "Necessary")]
+    pub fn process_join_group_request<'py>(
+        &self,
+        py: Python<'py>,
+        seq: i64,
+        request_uin: i64,
+        group_uin: i64,
+        accept: bool,
+        block: bool,
+        message: String,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        py_future(py, async move {
+            client
+                .solve_group_system_message(
+                    seq,
+                    request_uin,
+                    group_uin,
+                    false,
+                    false,
+                    accept,
+                    block,
+                    message,
+                )
+                .await?;
+            Ok(())
+        })
+    }
+
+    pub fn process_group_invitation<'py>(
+        &self,
+        py: Python<'py>,
+        seq: i64,
+        invitor_uin: i64,
+        group_uin: i64,
+        accept: bool,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        py_future(py, async move {
+            client
+                .solve_group_system_message(
+                    seq,
+                    invitor_uin,
+                    group_uin,
+                    false,
+                    false,
+                    accept,
+                    false,
+                    "".to_string(),
+                )
+                .await?;
+            Ok(())
+        })
+    }
+
+    pub fn process_new_friend_request<'py>(
+        &self,
+        py: Python<'py>,
+        seq: i64,
+        request_uin: i64,
+        accept: bool,
+    ) -> PyResult<&'py PyAny> {
+        let client = self.client.clone();
+        py_future(py, async move {
+            client
+                .solve_friend_system_message(seq, request_uin, accept)
+                .await?;
+            Ok(())
+        })
+    }
+}
+
+impl Drop for PlumbingClient {
+    fn drop(&mut self) {
+        let uin = self.uin;
+        tracing::info!("{} 的 Rust 客户端已被成功回收", uin);
+    }
 }
```

### Comparing `ichika-0.0.4/src/login.rs` & `ichika-0.0.5/src/login/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
+mod connector;
+
 use std::sync::Arc;
 
+use connector::IchikaConnector;
 use pyo3::exceptions::*;
 use pyo3::prelude::*;
 use pyo3::types::*;
-use pyo3_asyncio::TaskLocals;
+use pyo3_asyncio::{into_future_with_locals, TaskLocals};
 use pythonize::depythonize;
-use ricq::client::{Client, Connector, DefaultConnector, NetworkStatus, Token};
+use ricq::client::{Client, Connector, NetworkStatus, Token};
 use ricq::ext::common::after_login;
-use ricq::version::get_version;
+use ricq::version::Version;
 use ricq::{
     Device,
     LoginDeviceLocked,
     LoginNeedCaptcha,
     LoginResponse,
     LoginSuccess,
     LoginUnknownStatus,
-    Protocol,
     QRCodeState,
 };
 use tokio::task::JoinHandle;
 
 use crate::events::PyHandler;
 use crate::exc::MapPyErr;
-use crate::utils::{partial, py_bytes, py_future, py_try, py_use};
+use crate::utils::{partial, py_bytes, py_client_refs, py_future, py_try, py_use};
 use crate::{exc, import_call, PyRet};
-
 async fn prepare_client(
     device: Device,
-    protocol: Protocol,
+    app_ver: Version,
     handler: PyHandler,
 ) -> PyResult<(Arc<Client>, JoinHandle<()>)> {
-    let client = Arc::new(Client::new(device, get_version(protocol), handler));
+    let client = Arc::new(Client::new(device, app_ver, handler));
     let alive = tokio::spawn({
         let client = client.clone();
         // 连接最快的服务器
-        let stream = DefaultConnector
+        let stream = IchikaConnector
             .connect(&client)
             .await
             .map_err(|e| PyIOError::new_err(e.to_string()))?;
 
         #[allow(
             clippy::redundant_async_block,
             reason = "FP: rust-lang/rust-clippy#10482"
@@ -56,25 +57,14 @@
 pub enum PasswordCredential {
     #[pyo3(transparent, annotation = "str")]
     String(Py<PyString>),
     #[pyo3(transparent, annotation = "bytes")]
     MD5(Py<PyBytes>),
 }
 
-fn protocol_from_str(protocol: &str) -> PyResult<Protocol> {
-    match protocol {
-        "IPad" => Ok(Protocol::IPad),
-        "AndroidPhone" => Ok(Protocol::AndroidPhone),
-        "AndroidWatch" => Ok(Protocol::AndroidWatch),
-        "MacOS" => Ok(Protocol::MacOS),
-        "QiDian" => Ok(Protocol::QiDian),
-        _ => Err(exc::LoginError::new_err("未知协议")),
-    }
-}
-
 #[derive(Debug, Clone)]
 pub struct TokenRW {
     get_token: PyObject,
     write_token: PyObject,
 }
 
 impl TokenRW {
@@ -129,51 +119,60 @@
         Ok(false)
     }
 }
 
 fn parse_login_args<'py>(
     py: Python<'py>,
     uin: i64,
-    protocol: &'py PyAny,
+    protocol: String,
     store: &'py PyAny,
     queues: &'py PyList,
-) -> PyResult<(Protocol, PyHandler, Device, TokenRW)> {
-    let handler = PyHandler::new(
-        queues.into_py(py),
-        TaskLocals::with_running_loop(py)?, // Necessary since retrieving task locals at handling time is already insufficient
-    );
+) -> PyResult<(Version, PyHandler, Device, TokenRW, TaskLocals)> {
+    let task_locals = TaskLocals::with_running_loop(py)?; // Necessary since retrieving task locals at handling time is already insufficient
+    let handler = PyHandler::new(queues.into_py(py), task_locals.clone(), uin);
 
-    let get_token = partial(py).call1((store.getattr("get_token")?, uin, protocol))?;
-    let write_token = partial(py).call1((store.getattr("write_token")?, uin, protocol))?;
+    let get_token = partial(py).call1((store.getattr("get_token")?, uin, &protocol))?;
+    let write_token = partial(py).call1((store.getattr("write_token")?, uin, &protocol))?;
 
-    let device = store.getattr("get_device")?.call1((uin, protocol))?; // JSON
+    let device = store.getattr("get_device")?.call1((uin, &protocol))?; // JSON
     let device: Device = depythonize(device)
         .map_err(|e| exc::LoginError::new_err(format!("无法解析传入的设备信息: {e:?}")))?;
 
-    // Extract Protocol
-    let protocol = protocol.getattr("value")?.extract::<String>()?;
-    let protocol = protocol_from_str(&protocol)?;
-
     Ok((
-        protocol,
+        ricq::version::get_version(
+            ricq::Protocol::try_from(protocol.as_ref())
+                .map_err(|_| PyValueError::new_err(format!("无法找到协议 {protocol}")))?,
+        ),
         handler,
         device,
         TokenRW {
             get_token: get_token.into_py(py),
             write_token: write_token.into_py(py),
         },
+        task_locals,
     ))
 }
 
-fn call_state(py: Python, getter: &PyObject, name: &str, args: impl IntoPy<Py<PyTuple>>) -> PyRet {
-    let handler = getter.as_ref(py).call1((name,))?;
-    if handler.is_none() {
-        return Ok(py.None()); // return None
+async fn invoke_cb(
+    locals: &TaskLocals,
+    getter: &PyObject,
+    name: &str,
+    args: impl IntoPy<Py<PyTuple>>,
+) -> PyRet {
+    let (obj, is_none) = py_try(|py| {
+        let handler = getter.as_ref(py).call1((name,))?;
+        if handler.is_none() {
+            return Ok((py.None(), true)); // return None
+        }
+        Ok((handler.call1(args)?.into_py(py), false))
+    })?;
+    if is_none {
+        return Ok(obj);
     }
-    Ok(handler.call1(args)?.into_py(py))
+    py_use(|py| into_future_with_locals(locals, obj.as_ref(py)))?.await
 }
 
 pub async fn reconnect(
     client: &Arc<Client>,
     token_rw: &TokenRW,
 ) -> PyResult<Option<JoinHandle<()>>> {
     crate::utils::py_retry(
@@ -188,15 +187,15 @@
 
             tracing::error!("客户端连接中断，将在 10 秒后重连");
             tokio::time::sleep(std::time::Duration::from_secs(10)).await;
 
             let alive = tokio::spawn({
                 let client = client.clone();
                 // 连接最快的服务器
-                let stream = DefaultConnector.connect(&client).await?;
+                let stream = IchikaConnector.connect(&client).await?;
 
                 #[allow(
                     clippy::redundant_async_block,
                     reason = "FP: rust-lang/rust-clippy#10482"
                 )]
                 async move {
                     client.start(stream).await;
@@ -237,154 +236,166 @@
             client
                 .password_md5_login(uin, &py_use(|py| bytes.as_ref(py).as_bytes().to_owned()))
                 .await
         }
     }
 }
 async fn handle_device_lock(
+    locals: &TaskLocals,
     data: &LoginDeviceLocked,
     uin: i64,
     client: &Client,
     credential: &PasswordCredential,
     handle_getter: PyObject,
     sms: bool,
 ) -> PyResult<LoginResponse> {
     let sms_phone = data.sms_phone.as_ref();
     let message = data
         .message
         .as_ref()
         .map_or_else(|| "请解锁设备锁进行验证", |msg| msg.as_str());
-    let verify_url = data.verify_url.as_ref().map_or(
-        Err(exc::RICQError::new_err("无法获取验证地址")),
+    let verify_url = data.verify_url.as_ref().map_or_else(
+        || Err(exc::RICQError::new_err("无法获取验证地址")),
         |url| Ok(url.clone()),
     )?;
     tracing::info!("{:?}", data.clone());
     if let Some(sms_phone) = sms_phone
         && sms
         && let Ok(rsp) = client.request_sms().await {
             if !matches!(rsp, LoginResponse::DeviceLocked(_)) {
                 return Ok(rsp);
             }
 
-            let sms_code = py_try(|py| {
-                let res = call_state(py, &handle_getter, "RequestSMS", (message,sms_phone))?;
-                let res = res.as_ref(py);
-                if !res.is_none() {
-                    return Ok(Some(res.extract::<String>()?));
-                }
-                Ok(None)
-            })?;
+            let res = invoke_cb(locals, &handle_getter, "RequestSMS", (message, sms_phone)).await?;
+            let sms_code = py_try(|py| res.extract::<Option<String>>(py))?;
 
             if let Some(sms_code) = sms_code {
                 return client
                 .submit_sms_code(&sms_code)
                 .await
                 .py_res();
             }
         }
-    py_try(|py| call_state(py, &handle_getter, "DeviceLocked", (message, verify_url)))?;
+    invoke_cb(
+        locals,
+        &handle_getter,
+        "DeviceLocked",
+        (message, verify_url),
+    )
+    .await?;
     make_password_login_req(uin, client, credential)
         .await
         .py_res()
 }
 
 async fn password_login_process(
+    locals: &TaskLocals,
     client: &Client,
     uin: i64,
     credential: PasswordCredential,
     sms: bool,
     handle_getter: PyObject,
 ) -> PyResult<()> {
     let mut resp: LoginResponse = make_password_login_req(uin, client, &credential)
         .await
         .py_res()?;
 
     loop {
         match resp {
             LoginResponse::Success(LoginSuccess { .. }) => {
-                py_try(|py| call_state(py, &handle_getter, "Success", ()))?;
+                invoke_cb(locals, &handle_getter, "Success", ()).await?;
                 break;
             }
             LoginResponse::DeviceLocked(data) => {
-                resp =
-                    handle_device_lock(&data, uin, client, &credential, handle_getter.clone(), sms)
-                        .await?;
+                resp = handle_device_lock(
+                    locals,
+                    &data,
+                    uin,
+                    client,
+                    &credential,
+                    handle_getter.clone(),
+                    sms,
+                )
+                .await?;
             }
             LoginResponse::NeedCaptcha(LoginNeedCaptcha { ref verify_url, .. }) => {
-                let verify_url = verify_url.as_ref().map_or(
-                    Err(exc::RICQError::new_err("无法获取验证地址")),
+                let verify_url = verify_url.as_ref().map_or_else(
+                    || Err(exc::RICQError::new_err("无法获取验证地址")),
                     |url| Ok(url.clone()),
                 )?;
-                let ticket = py_try(|py| {
-                    Ok(
-                        call_state(py, &handle_getter, "NeedCaptcha", (verify_url,))?
-                            .downcast::<PyString>(py)?
-                            .to_string(),
-                    )
-                })?;
+                let ticket =
+                    invoke_cb(locals, &handle_getter, "NeedCaptcha", (verify_url,)).await?;
+                let ticket = py_try(|py| ticket.extract::<String>(py))?;
                 resp = client.submit_ticket(&ticket).await.py_res()?;
             }
             LoginResponse::DeviceLockLogin { .. } => {
-                py_try(|py| call_state(py, &handle_getter, "DeviceLockLogin", ()))?;
+                invoke_cb(locals, &handle_getter, "DeviceLockLogin", ()).await?;
                 resp = client.device_lock_login().await.py_res()?;
             }
             LoginResponse::AccountFrozen => {
-                py_try(|py| call_state(py, &handle_getter, "AccountFrozen", ()))?;
+                invoke_cb(locals, &handle_getter, "AccountFrozen", ()).await?;
                 break;
             }
             LoginResponse::TooManySMSRequest => {
-                py_try(|py| call_state(py, &handle_getter, "TooManySMSRequest", ()))?;
+                invoke_cb(locals, &handle_getter, "TooManySMSRequest", ()).await?;
                 break;
             }
             LoginResponse::UnknownStatus(LoginUnknownStatus {
                 ref status,
                 ref message,
                 ..
             }) => {
                 let (status, message) = (*status, message.clone());
-                py_try(|py| call_state(py, &handle_getter, "UnknownStatus", (message, status)))?;
+                invoke_cb(locals, &handle_getter, "UnknownStatus", (message, status)).await?;
                 break;
             }
         }
     }
 
     Ok(())
 }
 
 async fn post_login(client: Arc<Client>, alive: JoinHandle<()>, token_rw: TokenRW) -> PyRet {
     after_login(&client).await;
     token_rw.set(&client).await?;
+    let uin = client.uin().await;
     let init = crate::client::ClientInitializer {
-        uin: client.uin().await,
+        uin,
         client,
         alive: Arc::new(std::sync::Mutex::new(Some(alive))),
         token_rw,
     };
-    py_try(|py| Ok(import_call!(py, "ichika.client" => "Client" => init)?.into_py(py)))
+    py_try(|py| {
+        let client = import_call!(py, "ichika.client" => "Client" => init)?.into_py(py);
+        py_client_refs(py).set_item(uin, client.clone_ref(py))?;
+        Ok(client)
+    })
 }
 
 #[pyfunction]
 #[allow(clippy::too_many_arguments, reason = "Required for Python binding")]
 pub fn password_login<'py>(
     py: Python<'py>,
     uin: i64,
     credential: PasswordCredential,
     use_sms: bool,
-    protocol: &'py PyAny,
+    protocol: String,
     store: &'py PyAny,
     queues: &'py PyList,       // List[asyncio.Queue[Event]]
     login_callbacks: PyObject, // PasswordLoginCallbacks
 ) -> PyResult<&'py PyAny> {
-    let (protocol, handler, device, token_rw) = parse_login_args(py, uin, protocol, store, queues)?;
+    let (protocol, handler, device, token_rw, locals) =
+        parse_login_args(py, uin, protocol, store, queues)?;
     py_future(py, async move {
         let (client, alive) = prepare_client(device, protocol.clone(), handler).await?;
         if !token_rw.try_login(&client).await? {
             tracing::info!("正在使用密码登录 {}", uin);
             let handle_getter: PyObject = py_try(|py| login_callbacks.getattr(py, "get_handle"))?;
-            password_login_process(&client, uin, credential, use_sms, handle_getter).await?;
+            password_login_process(&locals, &client, uin, credential, use_sms, handle_getter)
+                .await?;
         }
 
         Ok(post_login(client, alive, token_rw).await?)
     })
 }
 
 fn parse_qrcode(qrcode: &bytes::Bytes) -> PyResult<Vec<Vec<bool>>> {
@@ -418,86 +429,88 @@
                 })
                 .collect()
         })
         .collect())
 }
 
 async fn qrcode_login_process(
+    locals: &TaskLocals,
     client: &Client,
     decl_uin: i64,
     handle_getter: PyObject,
     interval: f64,
 ) -> PyResult<()> {
     let mut resp = client.fetch_qrcode().await.py_res()?;
     let mut image_sig = bytes::Bytes::new();
 
     loop {
         use tokio::time::{sleep_until, Duration, Instant};
         let st_time = Instant::now();
         match resp {
             QRCodeState::WaitingForScan => {
-                py_try(|py| call_state(py, &handle_getter, "WaitingForScan", ()))?;
+                invoke_cb(locals, &handle_getter, "WaitingForScan", ()).await?;
             }
             QRCodeState::WaitingForConfirm => {
-                py_try(|py| call_state(py, &handle_getter, "WaitingForConfirm", ()))?;
+                invoke_cb(locals, &handle_getter, "WaitingForConfirm", ()).await?;
             }
             QRCodeState::Canceled => {
-                py_try(|py| call_state(py, &handle_getter, "Canceled", ()))?;
+                invoke_cb(locals, &handle_getter, "Canceled", ()).await?;
                 resp = client.fetch_qrcode().await.py_res()?;
                 continue;
             }
             QRCodeState::Timeout => {
-                py_try(|py| call_state(py, &handle_getter, "Timeout", ()))?;
+                invoke_cb(locals, &handle_getter, "Timeout", ()).await?;
                 resp = client.fetch_qrcode().await.py_res()?;
                 continue;
             }
             QRCodeState::ImageFetch(ricq::QRCodeImageFetch {
                 ref sig,
                 ref image_data,
             }) => {
                 image_sig = sig.clone();
                 let qrcode_data = parse_qrcode(image_data)?;
-                py_try(|py| call_state(py, &handle_getter, "DisplayQRCode", (qrcode_data,)))?;
+                invoke_cb(locals, &handle_getter, "DisplayQRCode", (qrcode_data,)).await?;
             }
             QRCodeState::Confirmed(ricq::QRCodeConfirmed { uin, .. }) => {
                 if uin == decl_uin {
-                    py_try(|py| call_state(py, &handle_getter, "Success", (uin,)))?;
+                    invoke_cb(locals, &handle_getter, "Success", (uin,)).await?;
                     break;
                 }
-                py_try(|py| call_state(py, &handle_getter, "UINMismatch", (decl_uin, uin)))?;
+                invoke_cb(locals, &handle_getter, "UINMismatch", (decl_uin, uin)).await?;
                 resp = client.fetch_qrcode().await.py_res()?;
                 continue;
             }
         }
         sleep_until(st_time + Duration::from_secs_f64(interval)).await;
         resp = client.query_qrcode_result(&image_sig).await.py_res()?;
     }
     Ok(())
 }
 
 #[pyfunction]
 pub fn qrcode_login<'py>(
     py: Python<'py>,
     uin: i64,
-    protocol: &'py PyAny,
+    protocol: String,
     store: &'py PyAny,
     queues: &'py PyList,       // List[asyncio.Queue[Event]]
     login_callbacks: PyObject, // QRCodeLoginCallbacks
 ) -> PyResult<&'py PyAny> {
-    let (protocol, handler, device, token_rw) = parse_login_args(py, uin, protocol, store, queues)?;
+    let (protocol, handler, device, token_rw, locals) =
+        parse_login_args(py, uin, protocol, store, queues)?;
     py_future(py, async move {
         let (client, alive) = prepare_client(device, protocol.clone(), handler).await?;
         if !token_rw.try_login(&client).await? {
             tracing::info!("正在使用二维码登录 {}", uin);
             let interval: f64 = py_try(|py| {
                 login_callbacks
                     .as_ref(py)
                     .getattr("interval")?
                     .extract::<f64>()
             })?;
             let handle_getter: PyObject = py_try(|py| login_callbacks.getattr(py, "get_handle"))?;
-            qrcode_login_process(&client, uin, handle_getter, interval).await?;
+            qrcode_login_process(&locals, &client, uin, handle_getter, interval).await?;
         }
 
         Ok(post_login(client, alive, token_rw).await?)
     })
 }
```

### Comparing `ichika-0.0.4/src/loguru.rs` & `ichika-0.0.5/src/loguru.rs`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 impl LoguruLayer {
     /// 创建一个新的 `LoguruLayer` 对象。
     pub(crate) fn new() -> PyResult<Self> {
         let log_fn = Python::with_gil(|py| -> PyResult<PyObject> {
             let loguru = py.import("loguru")?;
             let logger = loguru.getattr("logger")?;
-            // let logger = logger.call_method("opt", (), kwargs!(py, "depth" => -1))?;
             let log_fn = logger.getattr("log")?;
             Ok(log_fn.into())
         })?;
         Ok(LoguruLayer { log_fn })
     }
 }
 
@@ -129,23 +128,23 @@
             write!(self.0, "{value:?}").unwrap();
         } else {
             write!(self.0, "{}={value:?}", field.name()).unwrap();
         }
     }
 }
 
-#[pyclass(get_all)]
+#[pyclass(get_all, module = "ichika.core")]
 #[derive(PyRepr, Clone)]
 pub struct FakePyFrame {
     f_globals: Py<PyDict>,
     f_code: Py<FakePyCode>,
     f_lineno: u32,
 }
 
-#[pyclass(get_all)]
+#[pyclass(get_all, module = "ichika.core")]
 #[derive(PyRepr, Clone)]
 pub struct FakePyCode {
     co_filename: Py<PyString>,
     co_name: Py<PyString>,
 }
 
 impl FakePyFrame {
```

### Comparing `ichika-0.0.4/src/message/elements.rs` & `ichika-0.0.5/src/message/elements.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.4/src/utils.rs` & `ichika-0.0.5/src/utils.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-use anyhow::Result;
 use futures_util::Future;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 
 // use pyo3::types::*;
 
 /// 获取 Python 的 None。
@@ -38,20 +37,25 @@
                 dict.set_item($name, $value).expect("Failed to set_item on dict");
             )*
             dict
         }
     };
 }
 
-/// 等价于 `Some(py_dict!(..))`，用于指定 kwargs。
 #[macro_export]
 #[doc(hidden)]
-macro_rules! kwargs {
-    ($py:expr, $($name:expr => $value:expr),*) => {
-        Some($crate::py_dict!($py, $($name => $value),*))
+macro_rules! dict {
+    {$py:expr, $($name:ident : $value:expr),* $(,)?} => {
+        {
+            let dict = ::pyo3::types::PyDict::new($py);
+            $(
+                dict.set_item(stringify!($name), $value)?;
+            )*
+            dict
+        }
     };
 }
 
 #[macro_export]
 macro_rules! import_call {
     ($py:expr, $module:expr => $attr:expr => $arg:expr) => {
         $py.import(::pyo3::intern!($py, $module))?
@@ -79,18 +83,18 @@
         }
     };
 }
 
 /// 将 [`tokio`] 的 Future 包装为 Python 的 Future。
 pub fn py_future<F, T>(py: Python, future: F) -> PyResult<&PyAny>
 where
-    F: Future<Output = Result<T, anyhow::Error>> + Send + 'static,
+    F: Future<Output = Result<T, crate::exc::Error>> + Send + 'static,
     T: IntoPy<PyObject>,
 {
-    pyo3_asyncio::tokio::future_into_py(py, async move { Ok(future.await?) })
+    pyo3_asyncio::tokio::future_into_py(py, async move { future.await.map_err(|e| e.into()) })
 }
 
 /// 自动重试直到得到 `Ok(..)`。
 pub async fn py_retry<F, T, D>(
     mut max_count: usize,
     mut f: impl FnMut() -> F,
     mut on_retry: impl FnMut(PyErr, usize) -> D,
@@ -159,14 +163,53 @@
         )
         .expect($reason)
         .into()
     }
 }
 
 static_py_fn!(
-    datetime_from_ts,
+    _datetime_from_ts,
     __DT_CELL,
     "datetime",
     ["datetime", "fromtimestamp"]
 );
 
+pub fn datetime_from_ts(py: Python<'_>, time: impl IntoPy<PyObject>) -> PyResult<&PyAny> {
+    call_static_py!(_datetime_from_ts, py, (time))
+}
+
+static_py_fn!(
+    _timedelta_from_secs,
+    __TDELTA_CELL,
+    "datetime",
+    ["timedelta"]
+);
+
+pub fn timedelta_from_secs(py: Python<'_>, delta: impl IntoPy<PyObject>) -> PyResult<&PyAny> {
+    _timedelta_from_secs(py).call((), Some(dict!(py, seconds: delta.into_py(py))))
+}
+
 static_py_fn!(partial, __PARTIAL_CELL, "functools", ["partial"]);
+
+static_py_fn!(
+    py_client_refs,
+    __CLIENT_WEAKREFS_CELL,
+    "ichika.client",
+    ["CLIENT_REFS"]
+);
+
+#[macro_export]
+macro_rules! dict_obj {
+    {$py:ident ! $($key:ident : $val:expr),* $(,)?} => {
+        ::pyo3::Python::with_gil(|$py| -> ::pyo3::PyResult<_> {
+            let dict = ::pyo3::types::PyDict::new($py);
+            $(
+                let _val: ::pyo3::PyObject = $val.into_py($py);
+                dict.set_item(stringify!($key), _val)?;
+            )*
+            Ok(dict.into_py($py))
+        })
+    };
+    {$($key:ident : $val:expr),* $(,)?} => {
+        dict_obj!(py ! $($key : $val),*)
+    }
+}
```

### Comparing `ichika-0.0.4/Cargo.lock` & `ichika-0.0.5/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 
 [[package]]
 name = "async-trait"
-version = "0.1.66"
+version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b84f9ebcc6c1f5b8cb160f6990096a5c127f423fcb6e1ccc46c370cbdfb75dfc"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -151,17 +151,17 @@
 name = "checked_int_cast"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17cc5e6b5ab06331c33589842070416baa137e8b0eb912b008cfd4a78ada7919"
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "iana-time-zone",
  "num-integer",
  "num-traits",
  "winapi",
 ]
 
@@ -185,32 +185,32 @@
 name = "const-oid"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4c78c047431fee22c1a7bb92e00ad095a02a983affe4d8a72e2a2c62c1b94f3"
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -261,64 +261,64 @@
  "rand_core",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.1.26"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
+checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
 dependencies = [
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a140f260e6f3f79013b8bfc65e7ce630c9ab4388c6a89c71e07226f49487b72"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da6383f459341ea689374bf0a42979739dc421874f112ff26f829b8040b8e613"
+checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90201c1a650e95ccff1c8c0bb5a343213bdd317c6e600a93075bca2eff54ec97"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b75aed41bb2e6367cae39e6326ef817a851db13c13e4f3263714ca3cfb8de56"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "der"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6919815d73839e7ad218de758883aae3a257ba6759ce7a9992501efbb53d705c"
@@ -330,15 +330,15 @@
 name = "derivative"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
@@ -359,59 +359,68 @@
  "sec1",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "exr"
-version = "1.5.3"
+version = "1.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8af5ef47e2ed89d23d0ecbc1b681b30390069de70260937877514377fc24feb"
+checksum = "bdd2162b720141a91a054640662d3edce3d50a944a50ffca5313cd951abb35b4"
 dependencies = [
  "bit_field",
  "flume",
  "half",
  "lebe",
- "miniz_oxide",
+ "miniz_oxide 0.6.2",
+ "rayon-core",
  "smallvec",
- "threadpool",
  "zune-inflate",
 ]
 
 [[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "fdeflate"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+dependencies = [
+ "simd-adler32",
+]
+
+[[package]]
 name = "ff"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "131655483be284720a17d74ff97592b8e76576dc25563148601df2d7c9080924"
 dependencies = [
  "rand_core",
  "subtle",
@@ -426,15 +435,15 @@
 [[package]]
 name = "flate2"
 version = "1.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
 dependencies = [
  "crc32fast",
- "miniz_oxide",
+ "miniz_oxide 0.6.2",
 ]
 
 [[package]]
 name = "flume"
 version = "0.10.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
@@ -453,88 +462,88 @@
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e2792b0ff0340399d58445b88fd9770e3489eff258a4cbc1523418f12abf84"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8de0a35a6ab97ec8869e32a2473f4b1324459e14c29275d14b10cb1fd19b50e"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -549,15 +558,15 @@
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc2c7625b2fc250dd90b63f7887a6bb0f7ec1d714c8278415bea2669ef20820e"
 dependencies = [
  "g2poly",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "g2p"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc36d9bdc3d2da057775a9f4fa7d7b09edab3e0eda7a92cc353358fa63b8519e"
@@ -570,51 +579,51 @@
 name = "g2poly"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af6a86e750338603ea2c14b1c0bfe58cd61f87ca67a0021d9334996024608e12"
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghost"
-version = "0.1.8"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69e0cd8a998937e25c6ba7cc276b96ec5cc3f4dc4ab5de9ede4fb152bdd5c5eb"
+checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "gif"
-version = "0.11.4"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3edd93c6756b4dfaf2709eafcc345ba2636565295c198a9cfbf75fa5e3e00b06"
+checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
 dependencies = [
  "color_quant",
  "weezl",
 ]
 
 [[package]]
 name = "group"
@@ -666,58 +675,62 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "ichika"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
- "anyhow",
  "async-trait",
  "built",
  "bytes",
  "futures-util",
  "hex",
- "image 0.24.5",
+ "image 0.24.6",
  "once_cell",
  "pyo3",
  "pyo3-asyncio",
- "pyo3-built",
  "pyo3-repr",
  "pythonize",
  "qrcode",
  "ricq",
  "ricq-core",
  "rqrr",
  "serde",
@@ -751,36 +764,36 @@
  "num-iter",
  "num-rational 0.3.2",
  "num-traits",
 ]
 
 [[package]]
 name = "image"
-version = "0.24.5"
+version = "0.24.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69b7ea949b537b0fd0af141fff8c77690f2ce96f4f41f042ccb6c69c6c965945"
+checksum = "527909aa81e20ac3a44803521443a765550f09b5130c2c2fa1ea59c2f8f50a3a"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
  "exr",
  "gif",
  "jpeg-decoder",
  "num-rational 0.4.1",
  "num-traits",
  "png",
- "scoped_threadpool",
+ "qoi",
  "tiff",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
@@ -795,30 +808,31 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "inventory"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "498ae1c9c329c7972b917506239b557a60386839192f1cf0ca034f345b65db99"
+checksum = "7741301a6d6a9b28ce77c0fb77a4eb116b6bc8f3bef09923f7743d059c4157d3"
 dependencies = [
  "ctor",
  "ghost",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.6"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfa919a82ea574332e2de6e74b4c36e74d41982b335080fa59d4ef31be20fdf3"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -846,15 +860,15 @@
 name = "jcers_proc"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c886d02037458dd4436cb66948ae2e50502f876250fc026fe52c45f4150da454"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
@@ -881,32 +895,32 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "link-cplusplus"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "d59d8c75012853d2e872fb56bc8a2e53718e2cafe1a4c823143141c6d90c322f"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -959,14 +973,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+ "simd-adler32",
+]
+
+[[package]]
 name = "mio"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
@@ -1053,15 +1077,15 @@
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1097,15 +1121,15 @@
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
@@ -1135,15 +1159,15 @@
 name = "pin-project-internal"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1152,35 +1176,36 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "png"
-version = "0.17.7"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d708eaf860a19b19ce538740d2b4bdeeb8337fa53f7738455e706623ad5c638"
+checksum = "aaeebc51f9e7d2c150d3f3bfeb667f2aa985db5ef1e3d212847bdedb488beeaa"
 dependencies = [
  "bitflags",
  "crc32fast",
+ "fdeflate",
  "flate2",
- "miniz_oxide",
+ "miniz_oxide 0.7.1",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
 version = "0.9.0"
@@ -1217,32 +1242,32 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9cc1a3263e07e0bf68e96268f37665207b49560d98739662cdfaae215c720fe"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "prost-types"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "534b7a0e836e3c482d2693070f982e39e7611da9695d4d1f5a4b186b51faef0a"
 dependencies = [
  "bytes",
  "prost",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
@@ -1264,95 +1289,98 @@
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
-name = "pyo3-built"
-version = "0.4.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be6d574e0f8cab2cdd1eeeb640cbf845c974519fa9e9b62fa9c08ecece0ca5de"
-
-[[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-repr"
 version = "0.1.0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "pythonize"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a0e1bbcd2a3856284bf4f4ef09ccb1157e9467847792754556f153ea3fe6b42"
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
+name = "qoi"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
+dependencies = [
+ "bytemuck",
+]
+
+[[package]]
 name = "qrcode"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16d2f1455f3630c6e5107b4f2b94e74d76dea80736de0981fd27644216cff57f"
 dependencies = [
  "checked_int_cast",
  "image 0.23.14",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1411,57 +1439,66 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "ricq"
 version = "0.1.20"
-source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=sms_phone_resolve#8c32150ffe12fbb430dfb76ce885e4f3e9f670cc"
+source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=ichika-snapshot#637203cbd700626905cb089fc38bd056769abe9c"
 dependencies = [
  "async-trait",
  "bytes",
  "cached",
  "derivative",
  "flate2",
  "futures-util",
- "image 0.24.5",
+ "image 0.24.6",
  "jcers",
  "md5",
  "prost",
  "rand",
  "ricq-core",
  "serde",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "ricq-core"
 version = "0.1.20"
-source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=sms_phone_resolve#8c32150ffe12fbb430dfb76ce885e4f3e9f670cc"
+source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=ichika-snapshot#637203cbd700626905cb089fc38bd056769abe9c"
 dependencies = [
  "byteorder",
  "bytes",
  "derivative",
  "flate2",
  "generic-array",
  "jcers",
@@ -1478,45 +1515,39 @@
 [[package]]
 name = "rqrr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4a8b87d1f9f69bb1a6c77e20fd303f9617b2b68dcff87cd9bcbfff2ced4b8a0b"
 dependencies = [
  "g2p",
- "image 0.24.5",
+ "image 0.24.6",
  "lru",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.9"
+version = "0.37.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd5c6ff11fecd55b40746d1995a02f2eb375bf8c00d192d521ee09f42bef37bc"
+checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
-name = "scoped_threadpool"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d51f5df5af43ab3f1360b429fa5e0152ac5ce8c0bd6485cae490332e96846a8"
-
-[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "scratch"
@@ -1534,46 +1565,46 @@
  "generic-array",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58bc9567378fc7690d6b2addae4e60ac2eeea07becb2c64b9f218b53865cba2a"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.156"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "314b5b092c0ade17c00142951e50ced110ec27cea304b1037c6969246c2469a4"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.156"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7e29c4601e36bcec74a223228dce795f4cd3616341a4af93520ca1a837c087d"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1583,17 +1614,17 @@
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "simd-adler32"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14a5df39617d7c8558154693a1bb8157a4aab8179209540cc0b10e5dc24e0b18"
+checksum = "238abfbb77c1915110ad968465608b68e869e0772622c9656714e73e5a1a522f"
 
 [[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
@@ -1614,17 +1645,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "spin"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dccf47db1b41fa1573ed27ccf5e08e3ca771cb994f776668c5ebda893b248fc"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
@@ -1639,81 +1670,83 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5ab016db510546d856297882807df8da66a16fb8c4101cb8b30054b0d5b2d9c"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5420d42e90af0c38c3290abcca25b9b3bdf379fc9f55c528f53a269d9c9a267e"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
-name = "threadpool"
-version = "1.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
-dependencies = [
- "num_cpus",
-]
-
-[[package]]
 name = "tiff"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7449334f9ff2baf290d55d73983a7d6fa15e01198faef72af07e2a8db851e471"
 dependencies = [
  "flate2",
  "jpeg-decoder",
@@ -1733,55 +1766,55 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.12"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fb52b74f05dbf495a8fba459fdc331812b96aa086d9eb78101fa0d4569c3313"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -1794,33 +1827,32 @@
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "cf9cf6a813d3f40c88b0b6b6f29a5c95c6cdbf97c1f9cc53fb820200f5ad814d"
 dependencies = [
- "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
@@ -1838,17 +1870,17 @@
  "lazy_static",
  "log",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "nu-ansi-term",
  "sharded-slab",
  "smallvec",
  "thread_local",
  "tracing-core",
  "tracing-log",
@@ -1858,17 +1890,17 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.11"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524b68aca1d05e03fdf03fcdce2c6c94b6daf6d16861ddaa7e4f2b6638a9052c"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
@@ -1945,15 +1977,15 @@
 checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1967,15 +1999,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
@@ -2027,101 +2059,161 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 
 [[package]]
 name = "zune-inflate"
-version = "0.2.51"
+version = "0.2.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a01728b79fb9b7e28a8c11f715e1cd8dc2cda7416a007d66cac55cebb3a8ac6b"
+checksum = "440a08fd59c6442e4b846ea9b10386c38307eae728b216e1ab2c305d1c9daaf8"
 dependencies = [
  "simd-adler32",
 ]
```

### Comparing `ichika-0.0.4/PKG-INFO` & `ichika-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: ichika
-Version: 0.0.4
+Version: 0.0.5
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru~=0.6.0
-Requires-Dist: graia-broadcast>=0.19.0
-Requires-Dist: creart-graia>=0.1.5
 Requires-Dist: dacite>=1.6.0
 Requires-Dist: graia-amnesia>=0.7.0
 Requires-Dist: aiohttp>=3.8.3
-Requires-Dist: kayaku>=0.5.0; extra == 'kayaku'
-Provides-Extra: kayaku
+Requires-Dist: graia-broadcast>=0.19.2; extra == 'graia'
+Requires-Dist: launart>=0.6.3; extra == 'graia'
+Requires-Dist: creart>=0.2.2; extra == 'graia'
+Requires-Dist: creart-graia>=0.1.5; extra == 'graia'
+Requires-Dist: graiax-shortcut>=0.2.1; extra == 'graia'
+Provides-Extra: graia
 License-File: LICENSE
 Summary: 基于 RICQ 的轻量级 Python QQ 自动化框架。
 Keywords: graia,bot,qq,framework,ricq,ichika
 Author: BlueGlassBlock <blueglassblock@outlook.com>
 Author-email: BlueGlassBlock <blueglassblock@outlook.com>
 License: AGPL-3.0
 Requires-Python: >=3.8
@@ -37,24 +39,33 @@
 [![PyPI](https://img.shields.io/pypi/v/ichika)](https://github.com/BlueGlassBlock/ichika/blob/master/CHANGELOG.md)
 [![Python Version](https://img.shields.io/pypi/pyversions/ichika)](https://pypi.org/project/ichika)
 [![License](https://img.shields.io/github/license/BlueGlassBlock/Ichika)](https://github.com/BlueGlassBlock/Ichika/blob/master/LICENSE)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
+[![Deploy Docs](https://github.com/BlueGlassBlock/Ichika/actions/workflows/deploy-docs.yml/badge.svg)](https://github.comBlueGlassBlock/Ichika/actions/workflows/deploy-docs.yml/badge.svg)
 [![Run CI](https://github.com/BlueGlassBlock/Ichika/actions/workflows/ci.yml/badge.svg)](https://github.com/BlueGlassBlock/Ichika/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/BlueGlassBlock/Ichika/master.svg)](https://results.pre-commit.ci/latest/github/BlueGlassBlock/Ichika/master)
 
 </div>
 
+## 示例
+
+请参阅 [example.py](./example.py)，它包含了一个识别指定指令并发送图片的简单示例。
+
+<!-- start docs-include -->
+
 ## 鸣谢
 
 - [AWR](https://github.com/wybxc/awr): Ichika 的前身和部分代码来源
 - [ricq](https://github.com/lz1998/ricq): 使用 Rust 实现的高性能 QQ 协议 移植于 [OICQ](https://github.com/takayama-lily/oicq)
 - [mirai](https://github.com/mamoe/mirai): 高效率 QQ 机器人支持库
 - [PyO3](https://github.com/PyO3/PyO3): Python 解释器的 Rust 绑定
 - [GraiaProject](https://github.com/GraiaProject): 用于 Bot 开发的一系列高效, 现代化, 充分可扩展的工具链
 
 ## 许可证
 
 `Ichika` 使用 [`GNU AGPL-3.0`](https://choosealicense.com/licenses/agpl-3.0/) 作为许可证，这意味着你需要遵守相应的规则。
 
+<!-- end docs-include -->
+
```

