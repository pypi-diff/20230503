# Comparing `tmp/aiida-shell-0.4.0.tar.gz` & `tmp/aiida-shell-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-shell-0.4.0.tar", last modified: Thu Mar 30 20:03:16 2023, max compression
+gzip compressed data, was "aiida-shell-0.5.0.tar", last modified: Wed May  3 09:34:03 2023, max compression
```

## Comparing `aiida-shell-0.4.0.tar` & `aiida-shell-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
--rw-r--r--   0        0        0     7525 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      448 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/CITATION.cff
--rw-r--r--   0        0        0     1076 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0    14151 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/README.md
--rw-r--r--   0        0        0     2910 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      239 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/__init__.py
--rw-r--r--   0        0        0      127 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/calculations/__init__.py
--rw-r--r--   0        0        0    13794 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/calculations/shell.py
--rw-r--r--   0        0        0      167 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/data/__init__.py
--rw-r--r--   0        0        0     1624 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/data/code.py
--rw-r--r--   0        0        0     5518 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/data/pickled.py
--rw-r--r--   0        0        0      141 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/engine/__init__.py
--rw-r--r--   0        0        0      151 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/engine/launchers/__init__.py
--rw-r--r--   0        0        0     7754 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/engine/launchers/shell_job.py
--rw-r--r--   0        0        0      128 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/parsers/__init__.py
--rw-r--r--   0        0        0     5572 2023-03-30 20:03:12.764696 aiida-shell-0.4.0/src/aiida_shell/parsers/shell.py
--rw-r--r--   0        0        0    15458 1970-01-01 00:00:00.000000 aiida-shell-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0    10653 2023-05-03 09:13:18.263500 aiida-shell-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2023-05-03 09:06:02.308511 aiida-shell-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0     1076 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      728 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/README.md
+-rw-r--r--   0        0        0      638 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1323 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0    15543 2023-05-03 02:58:19.035109 aiida-shell-0.5.0/docs/source/howto.rst
+-rw-r--r--   0        0        0    25440 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/images/logo-column.png
+-rw-r--r--   0        0        0   164551 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/images/logo-column.svg
+-rw-r--r--   0        0        0   167883 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/images/logo-text.svg
+-rw-r--r--   0        0        0      429 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0      590 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     3191 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-05-03 09:08:04.335187 aiida-shell-0.5.0/src/aiida_shell/__init__.py
+-rw-r--r--   0        0        0      127 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/calculations/__init__.py
+-rw-r--r--   0        0        0    13794 2023-04-28 07:05:58.787771 aiida-shell-0.5.0/src/aiida_shell/calculations/shell.py
+-rw-r--r--   0        0        0      167 2023-04-25 15:09:47.689921 aiida-shell-0.5.0/src/aiida_shell/data/__init__.py
+-rw-r--r--   0        0        0     1624 2022-11-07 18:18:08.659450 aiida-shell-0.5.0/src/aiida_shell/data/code.py
+-rw-r--r--   0        0        0     5518 2023-04-25 15:09:47.689921 aiida-shell-0.5.0/src/aiida_shell/data/pickled.py
+-rw-r--r--   0        0        0      141 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/engine/__init__.py
+-rw-r--r--   0        0        0      151 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/engine/launchers/__init__.py
+-rw-r--r--   0        0        0     8654 2023-05-03 02:58:19.035109 aiida-shell-0.5.0/src/aiida_shell/engine/launchers/shell_job.py
+-rw-r--r--   0        0        0      128 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/parsers/__init__.py
+-rw-r--r--   0        0        0     5572 2023-04-25 15:09:47.689921 aiida-shell-0.5.0/src/aiida_shell/parsers/shell.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida-shell-0.5.0/PKG-INFO
```

### Comparing `aiida-shell-0.4.0/LICENSE.txt` & `aiida-shell-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.4.0/README.md` & `aiida-shell-0.5.0/docs/source/howto.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,343 +1,411 @@
-# `aiida-shell`
-[![PyPI version](https://badge.fury.io/py/aiida-shell.svg)](https://badge.fury.io/py/aiida-shell)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-shell.svg)](https://pypi.python.org/pypi/aiida-shell)
-[![CI](https://github.com/sphuber/aiida-shell/workflows/ci/badge.svg)](https://github.com/sphuber/aiida-shell/actions/workflows/ci.yml)
+.. _how-to:
 
-AiiDA plugin that makes running shell commands easy.
-Run any shell executable without writing a dedicated plugin or parser.
 
+=============
+How-to guides
+=============
 
-## Installation
 
-The recommended method of installation is through [`pip`](https://pip.pypa.io/en/stable/):
+Running a shell command
+=======================
 
-    pip install aiida-shell
+The most simple example is to run a shell command without any arguments:
 
-## Requirements
+.. code-block:: python
 
-To use `aiida-shell` a configured AiiDA profile is required.
-Please refer to the [documentation of `aiida-core`](https://aiida.readthedocs.io/projects/aiida-core/en/latest/intro/get_started.html) for detailed instructions.
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job('date')
+    print(results['stdout'].get_content())
 
+Which should print something like ``Thu 17 Mar 2022 10:49:52 PM CET``.
 
-## Examples
 
-### Running a shell command
-The most simple example is to run a shell command without any arguments:
+Running a shell command with arguments
+======================================
+
+To pass arguments to the shell command, pass them as a string to the ``arguments`` keyword:
+
+
+.. code-block:: python
+
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'date',
+        arguments='--iso-8601'
+    )
+    print(results['stdout'].get_content())
+
+which should print something like ``2022-03-17``.
+
+
+Running a shell command with files as arguments
+===============================================
+
+For commands that take arguments that refer to files, pass those files using the ``nodes`` keyword.
+The keyword takes a dictionary of ``SinglefileData`` nodes.
+To specify where on the command line the files should be passed, use placeholder strings in the ``arguments`` keyword.
+
+.. code-block:: python
 
-```python
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job('date')
-print(results['stdout'].get_content())
-```
-Which should print something like `Thu 17 Mar 2022 10:49:52 PM CET`.
-
-### Running a shell command with arguments
-To pass arguments to the shell command, pass them as a list to the `arguments` keyword:
-
-```python
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'date',
-    arguments=['--iso-8601']
-)
-print(results['stdout'].get_content())
-```
-which should print something like `2022-03-17`.
-
-### Running a shell command with files as arguments
-For commands that take arguments that refer to files, pass those files using the `nodes` keyword.
-The keyword takes a dictionary of `SinglefileData` nodes.
-To specify where on the command line the files should be passed, use placeholder strings in the `arguments` keyword.
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'cat',
-    arguments=['{file_a}', '{file_b}'],
-    nodes={
-        'file_a': SinglefileData(StringIO('string a')),
-        'file_b': SinglefileData(StringIO('string b')),
-    }
-)
-print(results['stdout'].get_content())
-```
-which prints `string astring b`.
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'cat',
+        arguments='{file_a} {file_b}',
+        nodes={
+            'file_a': SinglefileData(StringIO('string a')),
+            'file_b': SinglefileData(StringIO('string b')),
+        }
+    )
+    print(results['stdout'].get_content())
+
+which prints ``string astring b``.
 
-### Running a shell command with files as arguments with specific filenames
-The keys in the `nodes` dictionary can only use alphanumeric characters and underscores.
+
+Running a shell command with files as arguments with specific filenames
+=======================================================================
+
+The keys in the ``nodes`` dictionary can only use alphanumeric characters and underscores.
 The keys will be used as the link label of the file in the provenance graph, and as the filename in the temporary directory in which the shell command will be executed.
-Certain commands may require specific filenames, for example including a file extension, e.g., `filename.txt`, but this cannot be used in the `nodes` arguments.
-To specify explicit filenames that should be used in the running directory, make sure that the `filename` of the `SinglefileData` node is defined.
-If the `SinglefileData.filename` was explicitly set when creating the node, that is the filename used to write the input file to the working directory:
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'cat',
-    arguments=['{file_a}'],
-    nodes={
-        'file_a': SinglefileData(StringIO('string a'), filename='filename.txt'),
-    }
-)
-print(results['stdout'].get_content())
-```
-which prints `string a`.
-
-If the filename of the `SinglefileData` cannot be controlled, alternatively explicit filenames can be defined using the `filenames` argument:
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'cat',
-    arguments=['{file_a}'],
-    nodes={
-        'file_a': SinglefileData(StringIO('string a')),
-    },
-    filenames={
-        'file_a': 'filename.txt'
-    }
-)
-print(results['stdout'].get_content())
-```
-which prints `string a`.
-Filenames specified in the `filenames` input will override the filename of the `SinglefileData` nodes.
-Any parent directories in the filepath, for example `some/nested/path` in the filename `some/nested/path/file.txt`, will be automatically created.
-
-The output filename can be anything except for `stdout`, `stderr` and `status`, which are reserved filenames.
-
-### Passing other `Data` types as input
-The `nodes` keyword does not only accept `SinglefileData` nodes, but it accepts also other `Data` types.
-For these node types, the content returned by the `value` property is directly cast to `str`, which is used to replace the corresponding placeholder in the `arguments`.
-So as long as the `Data` type implements this `value` property it should be supported.
+Certain commands may require specific filenames, for example including a file extension, e.g., ``filename.txt``, but this cannot be used in the ``nodes`` arguments.
+To specify explicit filenames that should be used in the running directory, make sure that the ``filename`` of the ``SinglefileData`` node is defined.
+If the ``SinglefileData.filename`` was explicitly set when creating the node, that is the filename used to write the input file to the working directory:
+
+.. code-block:: python
+
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'cat',
+        arguments='{file_a}',
+        nodes={
+            'file_a': SinglefileData(StringIO('string a'), filename='filename.txt'),
+        }
+    )
+    print(results['stdout'].get_content())
+
+which prints ``string a``.
+
+If the filename of the ``SinglefileData`` cannot be controlled, alternatively explicit filenames can be defined using the ``filenames`` argument:
+
+.. code-block:: python
+
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'cat',
+        arguments='{file_a}',
+        nodes={
+            'file_a': SinglefileData(StringIO('string a')),
+        },
+        filenames={
+            'file_a': 'filename.txt'
+        }
+    )
+    print(results['stdout'].get_content())
+
+which prints ``string a``.
+Filenames specified in the ``filenames`` input will override the filename of the ``SinglefileData`` nodes.
+Any parent directories in the filepath, for example ``some/nested/path`` in the filename ``some/nested/path/file.txt``, will be automatically created.
+
+The output filename can be anything except for ``stdout``, ``stderr`` and ``status``, which are reserved filenames.
+
+
+Passing other ``Data`` types as input
+=====================================
+
+The ``nodes`` keyword does not only accept ``SinglefileData`` nodes, but it accepts also other ``Data`` types.
+For these node types, the content returned by the ``value`` property is directly cast to ``str``, which is used to replace the corresponding placeholder in the ``arguments``.
+So as long as the ``Data`` type implements this ``value`` property it should be supported.
 Of course, whether it makes sense for the value of the node to be used directly as a command line argument for the shell job, is up to the user.
-Typical useful examples, are the base types that ship with AiiDA, such as the `Float`, `Int` and `Str` types:
-```python
-from aiida.orm import Float, Int, Str
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'echo',
-    arguments=['{float}', '{int}', '{string}'],
-    nodes={
-        'float': Float(1.0),
-        'int': Int(2),
-        'string': Str('string'),
-    },
-)
-print(results['stdout'].get_content())
-```
-which prints `1.0 2 string`.
-This example is of course contrived, but when combining it with other components of AiiDA, which typically return outputs of these form, they can be used directly as inputs for `launch_shell_job` without having to convert the values.
+Typical useful examples, are the base types that ship with AiiDA, such as the ``Float``, ``Int`` and ``Str`` types:
+
+.. code-block:: python
+
+    from aiida.orm import Float, Int, Str
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'echo',
+        arguments='{float} {int} {string}',
+        nodes={
+            'float': Float(1.0),
+            'int': Int(2),
+            'string': Str('string'),
+        },
+    )
+    print(results['stdout'].get_content())
+
+which prints ``1.0 2 string``.
+This example is of course contrived, but when combining it with other components of AiiDA, which typically return outputs of these form, they can be used directly as inputs for ``launch_shell_job`` without having to convert the values.
 This ensures that provenance is kept.
 
-### Redirecting input file through stdin
+
+Redirecting input file through stdin
+====================================
+
 Certain shell commands require input to be passed through the stdin file descriptor.
 This is normally accomplished as follows:
-```bash
-cat < input.txt
-```
-To reproduce this behaviour, the file that should be redirected through stdin can be defined using the `metadata.option.filename_stdin` input:
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'cat',
-    nodes={
-        'input': SinglefileData(StringIO('string a'))
-    },
-    metadata={'options': {'filename_stdin': 'input'}}
-)
-print(results['stdout'].get_content())
-```
-which prints `string a`.
 
-N.B.: one might be tempted to simply define the `arguments` as `['<', '{input}']`, but this won't work as the `<` symbol will be quoted and will be read as a literal command line argument, not as the redirection symbol.
-This is why passing the `<` in the `arguments` input will result in a validation error.
+.. code-block:: bash
+
+    cat < input.txt
+
+To reproduce this behaviour, the file that should be redirected through stdin can be defined using the ``metadata.option.filename_stdin`` input:
+
+.. code-block:: python
+
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'cat',
+        nodes={
+            'input': SinglefileData(StringIO('string a'))
+        },
+        metadata={'options': {'filename_stdin': 'input'}}
+    )
+    print(results['stdout'].get_content())
+
+which prints ``string a``.
+
+N.B.: one might be tempted to simply define the ``arguments`` as ``'< {input}'``, but this won't work as the ``<`` symbol will be quoted and will be read as a literal command line argument, not as the redirection symbol.
+This is why passing the ``<`` in the ``arguments`` input will result in a validation error.
+
+
+Defining outputs
+================
 
-### Defining outputs
 When the shell command is executed, AiiDA captures by default the content written to the stdout and stderr file descriptors.
-The content is wrapped in a `SinglefileData` node and attached to the `ShellJob` with the `stdout` and `stderr` link labels, respectively.
-Any other output files that need to be captured can be defined using the `outputs` keyword argument.
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'sort',
-    arguments=['{input}', '--output', 'sorted'],
-    nodes={
-        'input': SinglefileData(StringIO('2\n5\n3')),
-    },
-    outputs=['sorted']
-)
-print(results['sorted'].get_content())
-```
-which prints `2\n3\n5`.
+The content is wrapped in a ``SinglefileData`` node and attached to the ``ShellJob`` with the ``stdout`` and ``stderr`` link labels, respectively.
+Any other output files that need to be captured can be defined using the ``outputs`` keyword argument.
+
+.. code-block:: python
+
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'sort',
+        arguments='{input} --output sorted',
+        nodes={
+            'input': SinglefileData(StringIO('2\n5\n3')),
+        },
+        outputs=['sorted']
+    )
+    print(results['sorted'].get_content())
+
+which prints ``2\n3\n5``.
+
+
+Defining output files with globbing
+===================================
 
-### Defining output files with globbing
 When the exact output files that will be generated and need to be captured are not known in advance, one can use globbing.
-Take for example the `split` command, which split a file into multiple files of a certain number of lines.
-By default, each output file will follow the sequence `xa`, `xb`, `xc` etc. augmenting the last character alphabetically.
-These output files can be captured by specifying the `outputs` as `['x*']`:
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'split',
-    arguments=['-l', '1', '{single_file}'],
-    nodes={
-        'single_file': SinglefileData(StringIO('line 0\nline 1\nline 2\n')),
-    },
-    outputs=['x*']
-)
-print(results.keys())
-```
-which prints `dict_keys(['xab', 'xaa', 'xac', 'stderr', 'stdout'])`.
+Take for example the ``split`` command, which split a file into multiple files of a certain number of lines.
+By default, each output file will follow the sequence ``xa``, ``xb``, ``xc`` etc. augmenting the last character alphabetically.
+These output files can be captured by specifying the ``outputs`` as ``['x*']``:
+
+.. code-block:: python
+
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'split',
+        arguments='-l 1 {single_file}',
+        nodes={
+            'single_file': SinglefileData(StringIO('line 0\nline 1\nline 2\n')),
+        },
+        outputs=['x*']
+    )
+    print(results.keys())
+
+which prints ``dict_keys(['xab', 'xaa', 'xac', 'stderr', 'stdout'])``.
 
 ### Defining output folders
 When the command produces a folder with multiple output files, it is also possible to parse this as a single output node, instead of individual outputs for each file.
-If a filepath specified in the `outputs` corresponds to a directory, it is attached as a `FolderData` that contains all its contents, instead of individual `SinglefileData` nodes.
-For example, imagine a compressed tarball `/some/path/archive.tar.gz` that contains the folder `sub_folder` with a number of files in it.
-The following example uncompresses the tarball and captures the uncompressed files in the `sub_folder` directory in the `sub_folder` output node:
-```python
-from io import StringIO
-from aiida.orm import SinglefileData
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'tar',
-    arguments=['-zxvf', '{archive}'],
-    nodes={
-        'archive': SinglefileData('/some/path/archive.tar.gz'),
-    },
-    outputs=['sub_folder']
-)
-print(results.keys())
-```
-which prints `dict_keys(['sub_folder', 'stderr', 'stdout'])`.
+If a filepath specified in the ``outputs`` corresponds to a directory, it is attached as a ``FolderData`` that contains all its contents, instead of individual ``SinglefileData`` nodes.
+For example, imagine a compressed tarball ``/some/path/archive.tar.gz`` that contains the folder ``sub_folder`` with a number of files in it.
+The following example uncompresses the tarball and captures the uncompressed files in the ``sub_folder`` directory in the ``sub_folder`` output node:
+
+.. code-block:: python
+
+    from io import StringIO
+    from aiida.orm import SinglefileData
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'tar',
+        arguments='-zxvf {archive}',
+        nodes={
+            'archive': SinglefileData('/some/path/archive.tar.gz'),
+        },
+        outputs=['sub_folder']
+    )
+    print(results.keys())
+
+which prints ``dict_keys(['sub_folder', 'stderr', 'stdout'])``.
 The contents of the folder can be retrieved from the node as follows:
-```python
-for filename in results['sub_folder'].list_object_names():
-    content = results['sub_folder'].get_object_content(filename)
-    # or, if a file-like object is preferred to stream the content
-    with results['sub_folder'].open(filename) as handle:
-        content = handle.read()
-```
 
-### Defining a specific computer
-By default the shell command ran by `launch_shell_job` will be executed on the localhost, i.e., the computer where AiiDA is running.
+.. code-block:: python
+
+    for filename in results['sub_folder'].list_object_names():
+        content = results['sub_folder'].get_object_content(filename)
+        # or, if a file-like object is preferred to stream the content
+        with results['sub_folder'].open(filename) as handle:
+            content = handle.read()
+
+
+Defining a specific computer
+============================
+
+By default the shell command ran by ``launch_shell_job`` will be executed on the localhost, i.e., the computer where AiiDA is running.
 However, AiiDA also supports running commands on remote computers.
-See the [documentation of `aiida-core`](https://aiida.readthedocs.io/projects/aiida-core/en/latest/howto/run_codes.html#how-to-set-up-a-computer) for instructions to setting up and configuring a remote computer.
-To specify what computer to use for a shell command, pass it as an option to the `metadata` keyword:
-```python
-from aiida.orm import load_computer
-from aiida_shell import launch_shell_job
-results, node = launch_shell_job(
-    'date',
-    metadata={'options': {'computer': load_computer('some-computer')}}
-)
-print(results['stdout'].get_content())
-```
-Here you can use `aiida.orm.load_computer` to load the `Computer` instance from its label, PK or UUID.
+See the `AiiDA's documentation <https://aiida.readthedocs.io/projects/aiida-core/en/latest/howto/run_codes.html#how-to-set-up-a-computer>`_ for instructions to setting up and configuring a remote computer.
+To specify what computer to use for a shell command, pass it as an option to the ``metadata`` keyword:
+
+.. code-block:: python
+
+    from aiida.orm import load_computer
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'date',
+        metadata={'options': {'computer': load_computer('some-computer')}}
+    )
+    print(results['stdout'].get_content())
+
+Here you can use ``aiida.orm.load_computer`` to load the ``Computer`` instance from its label, PK or UUID.
+
+
+Defining a pre-configured code
+==============================
+
+The first argument, ``command``, of ``launch_shell_job`` takes the name of the command to be run as a string.
+Under the hood, this is automatically converted into an :class:`~aiida.orm.nodes.data.code.abstract.AbstractCode`.
+The ``command`` argument also accepts a pre-configured code instance directly:
+
+.. code-block:: python
+
+    from aiida.orm import load_code
+    from aiida_shell import launch_shell_job
+    code = load_code('date@localhost')
+    results, node = launch_shell_job(code)
+
+This approach can be used as an alternative to the previous example where the target computer is specified through the `metadata` argument.
 
-### Running many shell jobs in parallel
-By default the shell command ran by `launch_shell_job` is run blockingly; meaning that the Python interpreter is blocked from doing anything else until the shell command finishes.
+
+Running many shell jobs in parallel
+===================================
+
+By default the shell command ran by ``launch_shell_job`` is run blockingly; meaning that the Python interpreter is blocked from doing anything else until the shell command finishes.
 This becomes inefficient if you need to run many shell commands.
-If the shell commands are independent and can be run in parallel, it is possible to submit the jobs to AiiDA's daemon by setting `submit=True`:
-```python
-from aiida.engine.daemon.client import get_daemon_client
-from aiida_shell import launch_shell_job
+If the shell commands are independent and can be run in parallel, it is possible to submit the jobs to AiiDA's daemon by setting ``submit=True``:
 
-# Make sure the daemon is running
-get_daemon_client().start_daemon()
+.. code-block:: python
 
-nodes = []
+    from aiida.engine.daemon.client import get_daemon_client
+    from aiida_shell import launch_shell_job
 
-for string in ['string_one', 'string_two']:
-    node = launch_shell_job(
-        'echo',
-        arguments=[string],
-        submit=True,
-    )
-    nodes.append(node)
-    print(f'Submitted {node}')
-```
-Instead of returning a tuple of the results and the node, `launch_shell_job` now only returns the `node`.
-The reason is because the function returns immediately after submitting the job to the daemon at which point it isn't necessarily finished yet.
-To check on the status of the submitted jobs, you can use the `verdi process list` command of the CLI that ships with AiiDA.
+    # Make sure the daemon is running
+    get_daemon_client().start_daemon()
+
+    nodes = []
+
+    for arguments in ['string_one', 'string_two']:
+        results, node = launch_shell_job(
+            'echo',
+            arguments=arguments,
+            submit=True,
+        )
+        nodes.append(node)
+        print(f'Submitted {node}')
+
+The results returned by ``launch_shell_job`` will now just be an empty dictionary.
+The reason is because the function returns immediately after submitting the job to the daemon at which point it isn't finished yet and so the results are not yet known.
+To check on the status of the submitted jobs, you can use the ``verdi process list`` command of the CLI that ships with AiiDA.
 Or you can do it programmatically:
-```python
-import time
 
-while True:
-    if all(node.is_terminated for node in nodes):
-        break
-    time.sleep(1)
-
-for node in nodes:
-    if node.is_finished_ok:
-        print(f'{node} finished successfully')
-    else:
-        print(f'{node} failed')
-```
+.. code-block:: python
+
+    import time
+
+    while True:
+        if all(node.is_terminated for node in nodes):
+            break
+        time.sleep(1)
 
-### Custom parsing
-By default, all outputs will be parsed into `SinglefileData` nodes.
+    for node in nodes:
+        if node.is_finished_ok:
+            print(f'{node} finished successfully')
+        else:
+            print(f'{node} failed')
+
+
+Custom output parsing
+=====================
+
+By default, all outputs will be parsed into ``SinglefileData`` nodes.
 While convenient not having to define a parser manually, it can also be quite restrictive.
-One of AiiDA's strong points is that it can store data in JSON form in a relational database, making it queryable, but the content of `SinglefileData` nodes is excluded from this functionality.
+One of AiiDA's strong points is that it can store data in JSON form in a relational database, making it queryable, but the content of ``SinglefileData`` nodes is excluded from this functionality.
+
+The ``parser`` keyword allows to define a "custom" parser, which is a function with the following signature:
+
+.. code-block:: python
+
+    def parser(self, dirpath: pathlib.Path) -> dict[str, Data]:
+        """Parse any output file generated by the shell command and return it as any ``Data`` node."""
 
-The `parser` keyword allows to define a "custom" parser, which is a function with the following signature:
-```python
-def parser(self, dirpath: pathlib.Path) -> dict[str, Data]:
-    """Parse any output file generated by the shell command and return it as any `Data` node."""
-```
 
 The following example shows how a custom parser can be implemented:
-```python
-from aiida_shell import launch_shell_job
 
-def parser(self, dirpath):
-    from aiida.orm import Str
-    return {'string': Str((dirpath / 'stdout').read_text().strip())}
-
-results, node = launch_shell_job(
-    'echo',
-    arguments=['some output'],
-    parser=parser
-)
-print(results['string'].value)
-```
-which prints `some output`.
-
-**Important:** if the output file that is parsed by the custom parser is not any of the files that are retrieved by default, i.e., `stdout`, `stderr`, `status` and the filenames specified in the `outputs` input, it has to be specified in the `metadata.options.additional_retrieve` input:
-
-```python
-from io import StringIO
-from json import dumps
-from aiida_shell import launch_shell_job
-from aiida.orm import SinglefileData
-
-def parser(self, dirpath):
-    """Parse the content of the ``results.json`` file and return as a ``Dict`` node."""
-    import json
-    from aiida.orm import Dict
-    return {'json': Dict(json.load((dirpath / 'results.json').open()))}
-
-results, node = launch_shell_job(
-    'cat',
-    arguments=['{json}'],
-    nodes={'json': SinglefileData(StringIO(dumps({'a': 1})))},
-    parser=parser,
-    metadata={
-        'options': {
-            'output_filename': 'results.json',
-            'additional_retrieve': ['results.json']
-        }
-    }
-)
-print(results['json'].get_dict())
-```
-which prints `{'a': 1}`.
+.. code-block:: python
+
+    from aiida_shell import launch_shell_job
+
+    def parser(self, dirpath):
+        from aiida.orm import Str
+        return {'string': Str((dirpath / 'stdout').read_text().strip())}
+
+    results, node = launch_shell_job(
+        'echo',
+        arguments='some output',
+        parser=parser
+    )
+    print(results['string'].value)
+
+which prints ``some output``.
+
+.. important::
+
+    If the output file that is parsed by the custom parser is not any of the files that are retrieved by default, i.e., ``stdout``, ``stderr``, ``status`` and the filenames specified in the ``outputs`` input, it has to be specified in the ``metadata.options.additional_retrieve`` input:
+
+    .. code-block:: python
+
+        from io import StringIO
+        from json import dumps
+        from aiida_shell import launch_shell_job
+        from aiida.orm import SinglefileData
+
+        def parser(self, dirpath):
+            """Parse the content of the ``results.json`` file and return as a ``Dict`` node."""
+            import json
+            from aiida.orm import Dict
+            return {'json': Dict(json.load((dirpath / 'results.json').open()))}
+
+        results, node = launch_shell_job(
+            'cat',
+            arguments='{json}',
+            nodes={'json': SinglefileData(StringIO(dumps({'a': 1})))},
+            parser=parser,
+            metadata={
+                'options': {
+                    'output_filename': 'results.json',
+                    'additional_retrieve': ['results.json']
+                }
+            }
+        )
+        print(results['json'].get_dict())
+
+    which prints ``{'a': 1}``.
```

### Comparing `aiida-shell-0.4.0/pyproject.toml` & `aiida-shell-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,26 @@
 requires-python = '>=3.8'
 dependencies = [
     'aiida-core~=2.1',
     'dill'
 ]
 
 [project.urls]
-Source = 'https://github.com/sphuber/aiida-shell'
+homepage = 'https://github.com/sphuber/aiida-shell'
+documentation = 'https://aiida-shell.readthedocs.io/'
+tracker = 'https://github.com/sphuber/aiida-shell/issues'
+source = 'https://github.com/sphuber/aiida-shell'
 
 [project.optional-dependencies]
+docs = [
+    'sphinx~=6.1',
+    'sphinx-copybutton~=0.5.0',
+    'sphinx-book-theme~=1.0',
+    'sphinx-click~=4.0',
+]
 pre-commit = [
     'mypy==0.981',
     'pre-commit~=2.17',
     'pylint==2.13.7',
     'pylint-aiida~=0.1.1',
 ]
 tests = [
```

### Comparing `aiida-shell-0.4.0/src/aiida_shell/calculations/shell.py` & `aiida-shell-0.5.0/src/aiida_shell/calculations/shell.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.4.0/src/aiida_shell/data/code.py` & `aiida-shell-0.5.0/src/aiida_shell/data/code.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.4.0/src/aiida_shell/data/pickled.py` & `aiida-shell-0.5.0/src/aiida_shell/data/pickled.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.4.0/src/aiida_shell/engine/launchers/shell_job.py` & `aiida-shell-0.5.0/src/aiida_shell/engine/launchers/shell_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,88 @@
 # -*- coding: utf-8 -*-
 """Convenience wrapper function to simplify the interface to launch a :class:`aiida_shell.ShellJob` job."""
 from __future__ import annotations
 
 import logging
 import pathlib
+import shlex
 import tempfile
 import typing as t
 
-from aiida.common import exceptions
-from aiida.engine import launch
+from aiida.common import exceptions, lang
+from aiida.engine import Process, WorkChain, launch
 from aiida.orm import AbstractCode, Computer, Data, ProcessNode, SinglefileData, load_code, load_computer
 from aiida.parsers import Parser
 
 from aiida_shell import ShellCode, ShellJob
 
 __all__ = ('launch_shell_job',)
 
 LOGGER = logging.getLogger('aiida_shell')
 
 
 def launch_shell_job(  # pylint: disable=too-many-arguments
-    command: str,
-    nodes: dict[str, Data] | None = None,
+    command: str | AbstractCode,
+    nodes: t.Mapping[str, str | pathlib.Path | Data] | None = None,
     filenames: dict[str, str] | None = None,
-    arguments: list[str] | None = None,
+    arguments: list[str] | str | None = None,
     outputs: list[str] | None = None,
     parser: t.Callable[[Parser, pathlib.Path], dict[str, Data]] | None = None,
     metadata: dict[str, t.Any] | None = None,
     submit: bool = False,
-) -> tuple[dict[str, Data], ProcessNode] | ProcessNode:
+) -> tuple[dict[str, Data], ProcessNode]:
     """Launch a :class:`aiida_shell.ShellJob` job for the given command.
 
-    :param command: The shell command to run. Should be the relative command name, e.g., ``date``.
+    :param command: The shell command to run. Should be the relative command name, e.g., ``date``. An ``AbstractCode``
+        instance will be automatically created for this command if it doesn't already exist. Alternatively, a pre-
+        configured ``AbstractCode`` instance can be passed directly.
     :param nodes: A dictionary of ``Data`` nodes whose content is to replace placeholders in the ``arguments`` list.
     :param filenames: Optional dictionary of explicit filenames to use for the ``nodes`` to be written to ``dirpath``.
-    :param arguments: Optional list of command line arguments optionally containing placeholders for input nodes.
+    :param arguments: Optional list of command line arguments optionally containing placeholders for input nodes. The
+        arguments can also be specified as a single string. In this case, it will be split into separate parameters
+        using ``shlex.split``.
     :param outputs: Optional list of relative filenames that should be captured as outputs.
     :param parser: Optional callable that can implement custom parsing logic of produced output files.
     :param metadata: Optional dictionary of metadata inputs to be passed to the ``ShellJob``.
-    :param submit: Boolean, if ``True`` will submit the job to the daemon and return the ``ProcessNode``.
+    :param submit: Boolean, if ``True`` will submit the job to the daemon instead of running in current interpreter.
     :raises TypeError: If the value specified for ``metadata.options.computer`` is not a ``Computer``.
     :raises ValueError: If the absolute path of the command on the computer could not be determined.
     :returns: The tuple of results dictionary and ``ProcessNode``, or just the ``ProcessNode`` if ``submit=True``. The
         results dictionary intentionally doesn't include the ``retrieved`` and ``remote_folder`` outputs as they are
         generated for each ``CalcJob`` and typically are not of interest to a user running ``launch_shell_job``. In
         order to not confuse them, these nodes are omitted, but they can always be accessed through the node.
     """
     computer = (metadata or {}).get('options', {}).pop('computer', None)
-    code = prepare_code(command, computer)
+
+    if isinstance(command, str):
+        code = prepare_code(command, computer)
+    else:
+        lang.type_check(command, AbstractCode)
+        code = command
+
+    if isinstance(arguments, str):
+        arguments = shlex.split(arguments)
+    else:
+        lang.type_check(arguments, list, allow_none=True)
 
     inputs = {
         'code': code,
         'nodes': convert_nodes_single_file_data(nodes or {}),
         'filenames': filenames,
         'arguments': arguments,
         'outputs': outputs,
         'parser': parser,
         'metadata': metadata or {},
     }
 
     if submit:
-        return launch.submit(ShellJob, **inputs)
+        current_process = Process.current()
+        if current_process is not None and isinstance(current_process, WorkChain):
+            return {}, current_process.submit(ShellJob, **inputs)
+        return {}, launch.submit(ShellJob, **inputs)
 
     results, node = launch.run_get_node(ShellJob, **inputs)
 
     return {label: node for label, node in results.items() if label not in ('retrieved', 'remote_folder')}, node
 
 
 def prepare_code(command: str, computer: Computer | None = None) -> AbstractCode:
```

### Comparing `aiida-shell-0.4.0/src/aiida_shell/parsers/shell.py` & `aiida-shell-0.5.0/src/aiida_shell/parsers/shell.py`

 * *Files identical despite different names*

