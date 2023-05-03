# Comparing `tmp/docformatter-1.6.4.tar.gz` & `tmp/docformatter-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.6.4.tar", max compression
+gzip compressed data, was "docformatter-1.6.5.tar", max compression
```

## Comparing `docformatter-1.6.4.tar` & `docformatter-1.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.4/LICENSE
--rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.4/README.rst
--rw-r--r--   0        0        0     5881 2023-04-26 13:06:31.058027 docformatter-1.6.4/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.4/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     2555 2023-04-12 22:55:21.294454 docformatter-1.6.4/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-04-26 13:06:31.058027 docformatter-1.6.4/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    11411 2023-04-12 22:55:21.304454 docformatter-1.6.4/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.4/src/docformatter/encode.py
--rw-r--r--   0        0        0    20933 2023-04-25 02:19:20.744420 docformatter-1.6.4/src/docformatter/format.py
--rw-r--r--   0        0        0     5967 2023-04-25 02:19:20.744420 docformatter-1.6.4/src/docformatter/strings.py
--rw-r--r--   0        0        0    15048 2023-04-26 03:57:38.348349 docformatter-1.6.4/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4572 2023-04-12 22:55:21.329455 docformatter-1.6.4/src/docformatter/util.py
--rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.4/setup.py
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.5/LICENSE
+-rw-r--r--   0        0        0     6593 2023-05-03 00:53:18.139711 docformatter-1.6.5/README.rst
+-rw-r--r--   0        0        0     5851 2023-05-03 17:53:43.941376 docformatter-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.5/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6095 2023-05-03 00:52:57.971387 docformatter-1.6.5/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-05-03 17:53:43.942376 docformatter-1.6.5/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    12789 2023-05-03 00:52:57.971387 docformatter-1.6.5/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.5/src/docformatter/encode.py
+-rw-r--r--   0        0        0    20851 2023-05-03 17:45:12.943363 docformatter-1.6.5/src/docformatter/format.py
+-rw-r--r--   0        0        0     6611 2023-05-02 23:18:37.457940 docformatter-1.6.5/src/docformatter/strings.py
+-rw-r--r--   0        0        0    15048 2023-05-03 17:40:52.745753 docformatter-1.6.5/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.6.5/src/docformatter/util.py
+-rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 docformatter-1.6.5/setup.py
+-rw-r--r--   0        0        0     8254 1970-01-01 00:00:00.000000 docformatter-1.6.5/PKG-INFO
```

### Comparing `docformatter-1.6.4/LICENSE` & `docformatter-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.4/README.rst` & `docformatter-1.6.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings
 
 .. |VERSION| image:: https://img.shields.io/pypi/v/docformatter
 .. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter
 .. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter
 .. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter
 .. |DD| image:: https://img.shields.io/pypi/dd/docformatter
+.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases
 
 +----------------+----------------------------------------------------------+
 | **Code**       + |BLACK| |ISORT|                                          +
 +----------------+----------------------------------------------------------+
 | **Docstrings** + |SELF| |NUMPSTYLE|                                       +
 +----------------+----------------------------------------------------------+
-| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT|                             +
+| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +
 +----------------+----------------------------------------------------------+
 | **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +
 +----------------+----------------------------------------------------------+
 
 Formats docstrings to follow `PEP 257`_.
 
 .. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/
```

### Comparing `docformatter-1.6.4/pyproject.toml` & `docformatter-1.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.6.4"
+version = "1.6.5"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
@@ -88,16 +88,15 @@
     "too-many-boolean-expressions",
     "too-many-locals",
     "too-many-return-statements",
     "useless-object-inheritance",
 ]
 
 [tool.docformatter]
-wrap-summaries = 79
-wrap-descriptions = 72
+black = true
 non-strict = false
 
 [tool.pydocstyle]
 convention = "pep257"
 
 [tool.pytest.ini_options]
 markers = [
```

### Comparing `docformatter-1.6.4/src/docformatter/__init__.py` & `docformatter-1.6.5/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.4/src/docformatter/__pkginfo__.py` & `docformatter-1.6.5/src/docformatter/__pkginfo__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.6.4"
+__version__ = "1.6.5"
```

### Comparing `docformatter-1.6.4/src/docformatter/configuration.py` & `docformatter-1.6.5/src/docformatter/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,28 +124,67 @@
             "-e",
             "--exclude",
             nargs="*",
             default=self.flargs_dct.get("exclude", None),
             help="in recursive mode, exclude directories and files by names",
         )
         self.parser.add_argument(
+            "-n",
+            "--non-cap",
+            action="store",
+            nargs="*",
+            default=self.flargs_dct.get("non-cap", None),
+            help="list of words not to capitalize "
+            "when they appear as the "
+            "first word in the summary",
+        )
+        self.parser.add_argument(
+            "--black",
+            action="store_true",
+            default=self.flargs_dct.get("black", "false").lower() == "true",
+            help="make formatting compatible with standard black options "
+            "(default: False)",
+        )
+
+        self.args = self.parser.parse_known_args(self.args_lst[1:])[0]
+
+        # Default black line length is 88 so use this when not specified
+        # otherwise use PEP-8 defaults
+        if self.args.black:
+            _default_wrap_summaries = 88
+            _default_wrap_descriptions = 88
+            _default_pre_summary_space = "true"
+        else:
+            _default_wrap_summaries = 79
+            _default_wrap_descriptions = 72
+            _default_pre_summary_space = "false"
+
+        self.parser.add_argument(
             "--wrap-summaries",
-            default=int(self.flargs_dct.get("wrap-summaries", 79)),
+            default=int(
+                self.flargs_dct.get("wrap-summaries", _default_wrap_summaries)
+            ),
             type=int,
             metavar="length",
             help="wrap long summary lines at this length; "
-            "set to 0 to disable wrapping (default: 79)",
+            "set to 0 to disable wrapping (default: 79, 88 with --black "
+            "option)",
         )
         self.parser.add_argument(
             "--wrap-descriptions",
-            default=int(self.flargs_dct.get("wrap-descriptions", 72)),
+            default=int(
+                self.flargs_dct.get(
+                    "wrap-descriptions", _default_wrap_descriptions
+                )
+            ),
             type=int,
             metavar="length",
             help="wrap descriptions at this length; "
-            "set to 0 to disable wrapping (default: 72)",
+            "set to 0 to disable wrapping (default: 72, 88 with --black "
+            "option)",
         )
         self.parser.add_argument(
             "--force-wrap",
             action="store_true",
             default=self.flargs_dct.get("force-wrap", "false").lower()
             == "true",
             help="force descriptions to be wrapped even if it may "
@@ -174,15 +213,17 @@
             == "true",
             help="add a newline before the summary of a multi-line docstring "
             "(default: False)",
         )
         self.parser.add_argument(
             "--pre-summary-space",
             action="store_true",
-            default=self.flargs_dct.get("pre-summary-space", "false").lower()
+            default=self.flargs_dct.get(
+                "pre-summary-space", _default_pre_summary_space
+            ).lower()
             == "true",
             help="add a space after the opening triple quotes "
             "(default: False)",
         )
         self.parser.add_argument(
             "--make-summary-multi-line",
             action="store_true",
@@ -245,14 +286,15 @@
         self.parser.add_argument(
             "files",
             nargs="+",
             help="files to format or '-' for standard in",
         )
 
         self.args = self.parser.parse_args(self.args_lst[1:])
+
         if self.args.line_range:
             if self.args.line_range[0] <= 0:
                 self.parser.error("--range must be positive numbers")
             if self.args.line_range[0] > self.args.line_range[1]:
                 self.parser.error(
                     "First value of --range should be less than or equal "
                     "to the second"
```

### Comparing `docformatter-1.6.4/src/docformatter/encode.py` & `docformatter-1.6.5/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.4/src/docformatter/format.py` & `docformatter-1.6.5/src/docformatter/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,121 @@
 import docformatter.strings as _strings
 import docformatter.syntax as _syntax
 import docformatter.util as _util
 
 unicode = str
 
 
+def _do_remove_blank_lines_after_definitions(
+    modified_tokens,
+):
+    """Remove blank lines between definitions and docstrings.
+
+    Blank lines between class, method, function, and variable
+    definitions and the docstring will be removed.
+
+    Parameters
+    ----------
+    modified_tokens: list
+        The list of tokens created from the docstring.
+
+    Returns
+    -------
+    modified_tokens: list
+        The list of tokens with any blank lines following a variable
+        definition removed.
+    """
+    for _idx, _token in enumerate(modified_tokens):
+        if _token[0] == 3:
+            j = 1
+
+            # Remove newline between variable definition and docstring
+            # unless it's separating a docstring from:
+            #     * A previous docstring.
+            #     * The file's shebang.
+            #     * The import section.
+            while (
+                modified_tokens[_idx - j][4] == "\n"
+                and not (
+                    modified_tokens[_idx - j - 1][4].strip().endswith('"""')
+                )
+                and not modified_tokens[_idx - j - 1][4].startswith("#!/")
+                and "import" not in modified_tokens[_idx - j - 1][4]
+            ):
+                modified_tokens.pop(_idx - j)
+                j += 1
+
+            # Remove newline between class, method, and function
+            # definitions and docstring.
+            j = 2
+            while modified_tokens[_idx - j][4] == "\n" and modified_tokens[
+                _idx - j - 2
+            ][4].strip().startswith(("def", "class")):
+                modified_tokens.pop(_idx - j)
+                j += 1
+
+    return modified_tokens
+
+
+def _do_remove_blank_lines_after_docstring(modified_tokens):
+    """Remove blank lines between docstring and first Python statement.
+
+    Parameters
+    ----------
+    modified_tokens: list
+        The list of tokens created from the docstring.
+
+    Returns
+    -------
+    modified_tokens: list
+        The list of tokens with any blank lines following a docstring
+        removed.
+    """
+    # Remove all newlines between docstring and first Python
+    # statement as long as it's not a stub function.
+    for _idx, _token in enumerate(modified_tokens):
+        j = 1
+        _num_blank_lines = 0
+        while modified_tokens[_idx - j][4] == "\n":
+            j += 1
+            _num_blank_lines += 1
+
+        with contextlib.suppress(IndexError):
+            _is_definition = (
+                _token[4].lstrip().startswith(("class ", "def ", "@"))
+            )
+            _is_docstring = (
+                modified_tokens[_idx - 2][4].strip().endswith('"""')
+            )
+            _after_definition = (
+                modified_tokens[_idx - _num_blank_lines - 4][4]
+                .lstrip()
+                .startswith(("class", "def", "@"))
+            )
+            _after_docstring = modified_tokens[_idx - 5][4].strip().endswith(
+                '"""'
+            ) or modified_tokens[_idx - 5][4].strip().startswith('"""')
+            _comment_follows = re.search(
+                r"\"\"\" *#", modified_tokens[_idx - 4][4]
+            )
+
+            if (
+                _token[0] == 1
+                and not _is_definition
+                and not _is_docstring
+                and not _comment_follows
+                and _after_definition
+                and _after_docstring
+            ):
+                for j in range(_num_blank_lines):
+                    modified_tokens.pop(_idx - j - 1)
+
+    return modified_tokens
+
+
 class FormatResult:
     """Possible exit codes."""
 
     ok = 0
     error = 1
     interrupted = 2
     check_failed = 3
@@ -311,18 +418,18 @@
                     only_comments_so_far = False
 
                 previous_token_type = token_type
                 modified_tokens.append(
                     (token_type, token_string, start, end, line)
                 )
 
-            modified_tokens = self._do_remove_blank_lines_after_definitions(
+            modified_tokens = _do_remove_blank_lines_after_definitions(
                 modified_tokens
             )
-            modified_tokens = self._do_remove_blank_lines_after_docstring(
+            modified_tokens = _do_remove_blank_lines_after_docstring(
                 modified_tokens
             )
 
             return untokenize.untokenize(modified_tokens)
         except tokenize.TokenError:
             return source
 
@@ -342,17 +449,22 @@
 
         Returns
         -------
         docstring_formatted: str
             The docstring formatted according the various options.
         """
         contents, open_quote = self._do_strip_docstring(docstring)
-        open_quote = (
-            f"{open_quote} " if self.args.pre_summary_space else open_quote
-        )
+
+        if (
+            self.args.black
+            and contents.startswith('"')
+            or not self.args.black
+            and self.args.pre_summary_space
+        ):
+            open_quote = f"{open_quote} "
 
         # Skip if there are nested triple double quotes
         if contents.count(self.QUOTE_TYPES[0]):
             return docstring
 
         # Do not modify things that start with doctests.
         if contents.lstrip().startswith(">>>"):
@@ -426,23 +538,25 @@
         formatted_docstring : str
             The formatted docstring.
         """
         if self.args.make_summary_multi_line:
             beginning = f"{open_quote}\n{indentation}"
             ending = f'\n{indentation}"""'
             summary_wrapped = _syntax.wrap_summary(
-                _strings.normalize_summary(contents),
+                _strings.normalize_summary(contents, self.args.non_cap),
                 wrap_length=self.args.wrap_summaries,
                 initial_indent=indentation,
                 subsequent_indent=indentation,
             ).strip()
             return f"{beginning}{summary_wrapped}{ending}"
         else:
             summary_wrapped = _syntax.wrap_summary(
-                open_quote + _strings.normalize_summary(contents) + '"""',
+                open_quote
+                + _strings.normalize_summary(contents, self.args.non_cap)
+                + '"""',
                 wrap_length=self.args.wrap_summaries,
                 initial_indent=indentation,
                 subsequent_indent=indentation,
             ).strip()
             if self.args.close_quotes_on_newline and "\n" in summary_wrapped:
                 summary_wrapped = (
                     f"{summary_wrapped[:-3]}"
@@ -484,15 +598,15 @@
             if self.args.pre_summary_newline
             else 3 * " " + indentation
         )
         pre_summary = (
             "\n" + indentation if self.args.pre_summary_newline else ""
         )
         summary = _syntax.wrap_summary(
-            _strings.normalize_summary(summary),
+            _strings.normalize_summary(summary, self.args.non_cap),
             wrap_length=self.args.wrap_summaries,
             initial_indent=initial_indent,
             subsequent_indent=indentation,
         ).lstrip()
         description = _syntax.wrap_description(
             description,
             indentation=indentation,
@@ -504,119 +618,14 @@
         return f'''\
 {open_quote}{pre_summary}{summary}
 
 {description}{post_description}
 {indentation}"""\
 '''
 
-    @staticmethod
-    def _do_remove_blank_lines_after_definitions(modified_tokens):
-        """Remove blank lines between definitions and docstrings.
-
-        Blank lines between class, method, function, and variable
-        definitions and the docstring will be removed.
-
-        Parameters
-        ----------
-        modified_tokens: list
-            The list of tokens created from the docstring.
-
-        Returns
-        -------
-        modified_tokens: list
-            The list of tokens with any blank lines following a variable
-            definition removed.
-        """
-        for _idx, _token in enumerate(modified_tokens):
-            if _token[0] == 3:
-                j = 1
-
-                # Remove newline between variable definition and docstring
-                # unless is separating docstring from:
-                #     * A previous docstring.
-                #     * The file's shebang.
-                while (
-                    modified_tokens[_idx - j][4] == "\n"
-                    and not (
-                        modified_tokens[_idx - j - 1][4]
-                        .strip()
-                        .endswith('"""')
-                    )
-                    and not modified_tokens[_idx - j - 1][4].startswith("#!/")
-                ):
-                    modified_tokens.pop(_idx - j)
-                    j += 1
-
-                # Remove newline between class, method, and function
-                # definitions and docstring.
-                j = 2
-                while modified_tokens[_idx - j][4] == "\n" and modified_tokens[
-                    _idx - j - 2
-                ][4].strip().startswith(("def", "class")):
-                    modified_tokens.pop(_idx - j)
-                    j += 1
-
-        return modified_tokens
-
-    @staticmethod
-    def _do_remove_blank_lines_after_docstring(modified_tokens):
-        """Remove blank lines between docstring and first Python statement.
-
-        Parameters
-        ----------
-        modified_tokens: list
-            The list of tokens created from the docstring.
-
-        Returns
-        -------
-        modified_tokens: list
-            The list of tokens with any blank lines following a docstring
-            removed.
-        """
-        # Remove all newlines between docstring and first Python
-        # statement as long as it's not a stub function.
-        for _idx, _token in enumerate(modified_tokens):
-            with contextlib.suppress(IndexError):
-                _is_definition = (
-                    _token[4].lstrip().startswith(("class ", "def ", "@"))
-                )
-                _is_docstring = (
-                    modified_tokens[_idx - 2][4].strip().endswith('"""')
-                )
-                _after_definition = (
-                    modified_tokens[_idx - 6][4]
-                    .lstrip()
-                    .startswith(("class", "def", "@"))
-                )
-                _after_docstring = modified_tokens[_idx - 5][
-                    4
-                ].strip().endswith('"""') or modified_tokens[_idx - 5][
-                    4
-                ].strip().startswith(
-                    '"""'
-                )
-                _comment_follows = re.search(
-                    r"\"\"\" *#", modified_tokens[_idx - 4][4]
-                )
-
-                if (
-                    _token[0] == 1
-                    and not _is_definition
-                    and not _is_docstring
-                    and not _comment_follows
-                    and _after_definition
-                    and _after_docstring
-                ):
-                    j = 1
-                    while modified_tokens[_idx - j][4] == "\n":
-                        modified_tokens.pop(_idx - j)
-                        j += 1
-
-        return modified_tokens
-
     def _do_strip_docstring(self, docstring: str) -> Tuple[str, str]:
         """Return contents of docstring and opening quote type.
 
         Strips the docstring of its triple quotes, trailing white space,
         and line returns.  Determines type of docstring quote (either string,
         raw, or unicode) and returns the opening quotes, including the type
         identifier, with single quotes replaced by double quotes.
```

### Comparing `docformatter-1.6.4/src/docformatter/strings.py` & `docformatter-1.6.5/src/docformatter/strings.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """This module provides docformatter string functions."""
 
 
-import contextlib
 # Standard Library Imports
+import contextlib
 import re
+from typing import List
 
 
 def find_shortest_indentation(lines):
     """Determine the shortest indentation in a list of lines.
 
     Parameters
     ----------
@@ -95,33 +96,57 @@
     """Return fixed line endings.
 
     All lines will be modified to use the most common line ending.
     """
     return "".join([normalize_line(line, newline) for line in lines])
 
 
-def normalize_summary(summary: str) -> str:
-    """Return normalized docstring summary."""
+def normalize_summary(summary: str, noncap: List[str] = None) -> str:
+    """Return normalized docstring summary.
+
+    A normalized docstring summary will have the first word capitalized and
+    a period at the end.
+
+    Parameters
+    ----------
+    summary : str
+        The summary string.
+    noncap : list
+        A user-provided list of words not to capitalize when they appear as
+        the first word in the summary.
+
+    Returns
+    -------
+    summary : str
+        The normalized summary string.
+    """
+    if noncap is None:
+        noncap = []
+
     # Remove trailing whitespace
     summary = summary.rstrip()
 
     # Add period at end of sentence.
     if (
         summary
         and (summary[-1].isalnum() or summary[-1] in ['"', "'"])
         and (not summary.startswith("#"))
     ):
         summary += "."
 
     with contextlib.suppress(IndexError):
         # Look for underscores, periods in the first word, this would typically
         # indicate the first word is a variable name, file name, or some other
-        # non-standard English word.  If none of these exist capitalize the
+        # non-standard English word.  The search the list of user-defined
+        # words not to capitalize.  If none of these exist capitalize the
         # first word of the summary.
-        if all(char not in summary.split(" ", 1)[0] for char in ["_", "."]):
+        if (
+            all(char not in summary.split(" ", 1)[0] for char in ["_", "."])
+            and summary.split(" ", 1)[0] not in noncap
+        ):
             summary = summary[0].upper() + summary[1:]
 
     return summary
 
 
 def split_first_sentence(text):
     """Split text into first sentence and the rest.
```

### Comparing `docformatter-1.6.4/src/docformatter/syntax.py` & `docformatter-1.6.5/src/docformatter/syntax.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.4/src/docformatter/util.py` & `docformatter-1.6.5/src/docformatter/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     Parameters
         - sources: iterable with paths as strings.
         - recursive: drill down directories if True.
         - exclude: string based on which directories and files are excluded.
 
     Return: yields paths to found files.
     """
+
     def not_hidden(name):
         """Return True if file 'name' isn't .hidden."""
         return not name.startswith(".")
 
     def is_excluded(name, exclude):
         """Return True if file 'name' is excluded."""
         return (
```

### Comparing `docformatter-1.6.4/setup.py` & `docformatter-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 {'tomli': ['tomli>=2.0.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['docformatter = docformatter.__main__:main']}
 
 setup_kwargs = {
     'name': 'docformatter',
-    'version': '1.6.4',
+    'version': '1.6.5',
     'description': 'Formats docstrings to follow PEP 257',
-    'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT|                             +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
+    'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
     'author': 'Steven Myint',
     'author_email': 'None',
     'maintainer': 'Doyle Rowland',
     'maintainer_email': 'doyle.rowland@reliaqual.com',
     'url': 'https://github.com/PyCQA/docformatter',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `docformatter-1.6.4/PKG-INFO` & `docformatter-1.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.6.4
+Version: 1.6.5
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
@@ -61,21 +61,22 @@
     :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings
 
 .. |VERSION| image:: https://img.shields.io/pypi/v/docformatter
 .. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter
 .. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter
 .. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter
 .. |DD| image:: https://img.shields.io/pypi/dd/docformatter
+.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases
 
 +----------------+----------------------------------------------------------+
 | **Code**       + |BLACK| |ISORT|                                          +
 +----------------+----------------------------------------------------------+
 | **Docstrings** + |SELF| |NUMPSTYLE|                                       +
 +----------------+----------------------------------------------------------+
-| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT|                             +
+| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +
 +----------------+----------------------------------------------------------+
 | **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +
 +----------------+----------------------------------------------------------+
 
 Formats docstrings to follow `PEP 257`_.
 
 .. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/
```

