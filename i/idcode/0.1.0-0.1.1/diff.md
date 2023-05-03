# Comparing `tmp/idcode-0.1.0.tar.gz` & `tmp/idcode-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idcode-0.1.0.tar", max compression
+gzip compressed data, was "idcode-0.1.1.tar", max compression
```

## Comparing `idcode-0.1.0.tar` & `idcode-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-03 14:58:29.726031 idcode-0.1.0/idcode/__init__.py
--rw-r--r--   0        0        0     1572 2023-05-02 11:09:24.479694 idcode-0.1.0/idcode/cli.py
--rw-r--r--   0        0        0     2121 2023-05-01 18:04:12.437129 idcode-0.1.0/idcode/core_values.py
--rw-r--r--   0        0        0    11093 2023-05-02 09:28:06.021797 idcode-0.1.0/idcode/custom_encoding.py
--rw-r--r--   0        0        0     5712 2023-05-02 10:58:09.327876 idcode-0.1.0/idcode/interactive_decoder.py
--rw-r--r--   0        0        0      339 2023-05-02 10:49:07.137334 idcode-0.1.0/idcode/preprocessing.py
--rw-r--r--   0        0        0     1083 2023-05-01 19:53:11.733482 idcode-0.1.0/LICENSE
--rw-r--r--   0        0        0      507 2023-05-03 14:54:04.579641 idcode-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1823 2023-05-02 11:13:36.208454 idcode-0.1.0/README.md
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 idcode-0.1.0/setup.py
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 idcode-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 14:58:29.726031 idcode-0.1.1/idcode/__init__.py
+-rw-r--r--   0        0        0     1572 2023-05-02 11:09:24.479694 idcode-0.1.1/idcode/cli.py
+-rw-r--r--   0        0        0     2121 2023-05-01 18:04:12.437129 idcode-0.1.1/idcode/core_values.py
+-rw-r--r--   0        0        0    11093 2023-05-02 09:28:06.021797 idcode-0.1.1/idcode/custom_encoding.py
+-rw-r--r--   0        0        0     5712 2023-05-02 10:58:09.327876 idcode-0.1.1/idcode/interactive_decoder.py
+-rw-r--r--   0        0        0      339 2023-05-02 10:49:07.137334 idcode-0.1.1/idcode/preprocessing.py
+-rw-r--r--   0        0        0     1083 2023-05-01 19:53:11.733482 idcode-0.1.1/LICENSE
+-rw-r--r--   0        0        0      506 2023-05-03 15:13:42.596598 idcode-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1823 2023-05-02 11:13:36.208454 idcode-0.1.1/README.md
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 idcode-0.1.1/setup.py
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 idcode-0.1.1/PKG-INFO
```

### Comparing `idcode-0.1.0/idcode/cli.py` & `idcode-0.1.1/idcode/cli.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.0/idcode/core_values.py` & `idcode-0.1.1/idcode/core_values.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.0/idcode/custom_encoding.py` & `idcode-0.1.1/idcode/custom_encoding.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.0/idcode/interactive_decoder.py` & `idcode-0.1.1/idcode/interactive_decoder.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.0/LICENSE` & `idcode-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idcode-0.1.0/README.md` & `idcode-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `idcode-0.1.0/setup.py` & `idcode-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['idcode']
 
 package_data = \
 {'': ['*']}
 
 entry_points = \
-{'console_scripts': ['idcode = idcode.main:main']}
+{'console_scripts': ['idcode = idcode.cli:main']}
 
 setup_kwargs = {
     'name': 'idcode',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '交互式检测并解码编码文本。',
     'long_description': '# idcode\n\nidcode 是一个使用 Python 编写的命令行工具，用于交互式检测并解码编码文本。它支持命令行输入和文件输入，可以自动检测编码类型和尝试解码，并提供了一个交互式界面来逐步解码编码文本。\n\n## 支持的编码格式\n\nidcode 支持多种编码格式，包括：\n\n- Base85/Base64/Base32\n- Base94/Base92/Base91/Ascii85/AdobeAscii85/Z85/Base58/Base45/Base36/Base8\n- Binary 编码\n- Hex 编码\n- URL 编码\n- HTML 实体编码\n- Quoted-printable 编码\n- 核心价值观编码\n\n## 安装\n\n要使用 idcode，你需要按照以下步骤进行安装：\n\n1. 克隆或下载此仓库。\n2. 确保你已经安装了 Python 3.6 或更高版本。\n3. 在项目目录中，运行以下命令安装依赖：\n\n```sh\npip install -r requirements.txt\n```\n\n或者，使用 `poetry` 来安装依赖：\n\n```sh\npoetry install\n```\n\n## 用法\n\nidcode 支持交互式输入、命令行输入和文件输入来获取编码文本。\n\n### 交互式输入\n\n当不给出任何命令行参数时，程序会在运行后提示你给出目标文本：\n\n```sh\nidcode\n```\n\n### 命令行输入\n\n要使用命令行输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -t "编码文本"\n```\n\n其中，`-t` 参数用于指定要解码的文本。\n\n### 文件输入\n\n要使用文件输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -f "文件路径"\n```\n\n其中，`-f` 参数用于指定包含编码文本的文件路径。\n\n## 贡献\n\n如果你发现了 bug，或者有改进建议，请随时创建 issue 或者 pull request。我们欢迎任何形式的贡献。\n\n## 许可证\n\nidcode 使用 MIT 许可证。请参阅 LICENSE 文件了解更多详情。',
     'author': 'p0ise',
     'author_email': 'changelf@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/p0ise/idcode',
```

### Comparing `idcode-0.1.0/PKG-INFO` & `idcode-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idcode
-Version: 0.1.0
+Version: 0.1.1
 Summary: 交互式检测并解码编码文本。
 Home-page: https://github.com/p0ise/idcode
 License: MIT
 Author: p0ise
 Author-email: changelf@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

