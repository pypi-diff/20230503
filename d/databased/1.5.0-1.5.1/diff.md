# Comparing `tmp/databased-1.5.0.tar.gz` & `tmp/databased-1.5.1.tar.gz`

## Comparing `databased-1.5.0.tar` & `databased-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 databased-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    34888 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-1.5.0/docs/index.html
--rw-r--r--   0        0        0    60821 2020-02-02 00:00:00.000000 databased-1.5.0/docs/search.js
--rw-r--r--   0        0        0    44509 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/custom_manager.html
--rw-r--r--   0        0        0   406809 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/databased.html
--rw-r--r--   0        0        0   280216 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/dbmanager.html
--rw-r--r--   0        0        0   101086 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/dbparsers.html
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/__init__.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/custom_manager.py
--rw-r--r--   0        0        0    20869 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/databased.py
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/dbmanager.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/dbparsers.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-1.5.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 databased-1.5.0/README.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 databased-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 databased-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 databased-1.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34888 2020-02-02 00:00:00.000000 databased-1.5.1/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-1.5.1/docs/index.html
+-rw-r--r--   0        0        0    60780 2020-02-02 00:00:00.000000 databased-1.5.1/docs/search.js
+-rw-r--r--   0        0        0    44509 2020-02-02 00:00:00.000000 databased-1.5.1/docs/databased/custom_manager.html
+-rw-r--r--   0        0        0   410787 2020-02-02 00:00:00.000000 databased-1.5.1/docs/databased/databased.html
+-rw-r--r--   0        0        0   280216 2020-02-02 00:00:00.000000 databased-1.5.1/docs/databased/dbmanager.html
+-rw-r--r--   0        0        0   101086 2020-02-02 00:00:00.000000 databased-1.5.1/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 databased-1.5.1/src/databased/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 databased-1.5.1/src/databased/custom_manager.py
+-rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 databased-1.5.1/src/databased/databased.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 databased-1.5.1/src/databased/dbmanager.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 databased-1.5.1/src/databased/dbparsers.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 databased-1.5.1/README.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 databased-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 databased-1.5.1/PKG-INFO
```

### Comparing `databased-1.5.0/CHANGELOG.md` & `databased-1.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/docs/databased.html` & `databased-1.5.1/docs/databased.html`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/docs/search.js` & `databased-1.5.1/docs/search.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -711,15 +711,15 @@
         "kind": "class",
         "doc": "<p>Sqli wrapper so queries don't need to be written except table definitions.</p>\n\n<p>Supports saving and reading dates as datetime objects.</p>\n\n<p>Supports using a context manager.</p>\n"
     }, {
         "fullname": "databased.databased.DataBased.__init__",
         "modulename": "databased.databased",
         "qualname": "DataBased.__init__",
         "kind": "function",
-        "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>dbpath</strong>:  String or Path object to database file.\nIf a relative path is given, it will be relative to the\ncurrent working directory. The log file will be saved to the\nsame directory.</p></li>\n<li><p><strong>logger_message_format</strong>:  '{' style format string\nfor the logger object.</p></li>\n</ul>\n",
+        "doc": "<h4 id=\"params\">:params:</h4>\n\n<p><code>dbpath</code>: String or Path object to database file.\nIf a relative path is given, it will be relative to the\ncurrent working directory. The log file will be saved to the\nsame directory.</p>\n\n<p><code>logger_message_format</code>: '{' style format string for the logger object.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">dbpath</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>,</span><span class=\"param\">\t<span class=\"n\">logger_encoding</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;utf-8&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">logger_message_format</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;</span><span class=\"si\">{levelname}</span><span class=\"s1\">|-|</span><span class=\"si\">{asctime}</span><span class=\"s1\">|-|</span><span class=\"si\">{message}</span><span class=\"s1\">&#39;</span></span>)</span>"
     }, {
         "fullname": "databased.databased.DataBased.open",
         "modulename": "databased.databased",
         "qualname": "DataBased.open",
         "kind": "function",
         "doc": "<p>Open connection to db.</p>\n",
@@ -734,39 +734,39 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.query",
         "modulename": "databased.databased",
         "qualname": "DataBased.query",
         "kind": "function",
-        "doc": "<p>Execute an arbitrary query and\nreturn the results.</p>\n",
+        "doc": "<p>Execute an arbitrary query and return the results.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">query_</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.create_tables",
         "modulename": "databased.databased",
         "qualname": "DataBased.create_tables",
         "kind": "function",
-        "doc": "<p>Create tables if they don't exist.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>table_querys</strong>:  Each query should be\nin the form 'tableName(columnDefinitions)'</li>\n</ul>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">table_querys</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[]</span></span><span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Create tables if they don't exist.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong><code>table_defs</code></strong>:  Each definition should be in the form <code>table_name(column_definitions)</code></li>\n</ul>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">table_defs</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[]</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.create_table",
         "modulename": "databased.databased",
         "qualname": "DataBased.create_table",
         "kind": "function",
-        "doc": "<p>Create a table if it doesn't exist.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>table</strong>:  Name of the table to create.</p></li>\n<li><p><strong>column_defs</strong>:  List of column definitions in\nproper Sqlite3 sytax.\ni.e. \"columnName text unique\" or \"columnName int primary key\" etc.</p></li>\n</ul>\n",
+        "doc": "<p>Create a table if it doesn't exist.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>table</code>: Name of the table to create.</p>\n\n<p><code>column_defs</code>: List of column definitions in proper Sqlite3 sytax.\ni.e. <code>\"column_name text unique\"</code> or <code>\"column_name int primary key\"</code> etc.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">column_defs</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.get_table_names",
         "modulename": "databased.databased",
         "qualname": "DataBased.get_table_names",
         "kind": "function",
-        "doc": "<p>Returns a list of table names from database.</p>\n",
+        "doc": "<p>Returns a list of table names from the database.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.get_column_names",
         "modulename": "databased.databased",
         "qualname": "DataBased.get_column_names",
         "kind": "function",
@@ -774,87 +774,87 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.count",
         "modulename": "databased.databased",
         "qualname": "DataBased.count",
         "kind": "function",
-        "doc": "<p>Return number of items in table.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each\ntuple is (columnName, rowValue) or a dictionary where\nkeys are column names and values are row values.\nIf None, all rows from the table will be counted.</p></li>\n<li><p><strong>exact_match</strong>:  If False, the row value for a give column\nin match_criteria will be matched as a substring. Has no effect if\nmatch_criteria is None.</p></li>\n</ul>\n",
+        "doc": "<p>Return number of items in <code>table</code>.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>match_criteria</code>: Can be a list of 2-tuples where each\ntuple is <code>(columnName, rowValue)</code> or a dictionary where\nkeys are column names and values are row values.\nIf <code>None</code>, all rows from the table will be counted.</p>\n\n<p><code>exact_match</code>: If <code>False</code>, the row value for a given column\nin <code>match_criteria</code> will be matched as a substring.\nHas no effect if <code>match_criteria</code> is <code>None</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">match_criteria</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"nb\">dict</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">exact_match</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.add_row",
         "modulename": "databased.databased",
         "qualname": "DataBased.add_row",
         "kind": "function",
-        "doc": "<p>Add row of values to table.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>table</strong>:  The table to insert into.</p></li>\n<li><p><strong>values</strong>:  A tuple of values to be inserted into the table.</p></li>\n<li><p><strong>columns</strong>:  If None, values param is expected to supply\na value for every column in the table. If columns is\nprovided, it should contain the same number of elements as values.</p></li>\n</ul>\n",
+        "doc": "<p>Add a row of values to a table.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>table</code>: The table to insert values into.</p>\n\n<p><code>values</code>: A tuple of values to be inserted into the table.</p>\n\n<p><code>columns</code>: If <code>None</code>, <code>values</code> is expected to supply a value for every column in the table.\nIf <code>columns</code> is provided, it should contain the same number of elements as <code>values</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">values</span><span class=\"p\">:</span> <span class=\"nb\">tuple</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">columns</span><span class=\"p\">:</span> <span class=\"nb\">tuple</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.get_rows",
         "modulename": "databased.databased",
         "qualname": "DataBased.get_rows",
         "kind": "function",
-        "doc": "<p>Returns rows from table as a list of dictionaries\nwhere the key-value pairs of the dictionaries are\ncolumn name: row value.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each\ntuple is (columnName, rowValue) or a dictionary where\nkeys are column names and values are row values.</p></li>\n<li><p><strong>exact_match</strong>:  If False, the rowValue for a give column\nwill be matched as a substring.</p></li>\n<li><p><strong>sort_by_column</strong>:  A column name to sort the results by.\nThis will sort results in Python after retrieving them from the db.\nUse the 'order_by' param to use SQLite engine for ordering.</p></li>\n<li><p><strong>columns_to_return</strong>:  Optional list of column names.\nIf provided, the elements returned by get_rows() will\nonly contain the provided columns. Otherwise every column\nin the row is returned.</p></li>\n<li><p><strong>return_as_dataframe</strong>:  If True,\nthe results will be returned as a pandas.DataFrame object.</p></li>\n<li><p><strong>values_only</strong>:  Return the results as a list of tuples\ninstead of a list of dictionaries that have column names as keys.\nThe results will still be sorted according to sort_by_column if\none is provided.</p></li>\n<li><p><strong>order_by</strong>:  If given, a 'order by {order_by}' clause\nwill be added to the select query.</p></li>\n<li><p><strong>limit</strong>:  If given, a 'limit {limit}' clause will be\nadded to the select query.</p></li>\n</ul>\n",
+        "doc": "<p>Return matching rows from <code>table</code>.</p>\n\n<p>By default, rows will be returned as a list of dictionaries of the form <code>[{\"column_name\": value, ...}, ...]</code></p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>match_criteria</code>: Can be a list of 2-tuples where each\ntuple is <code>(columnName, rowValue)</code> or a dictionary where\nkeys are column names and values are row values.</p>\n\n<p><code>exact_match</code>: If <code>False</code>, the row value for a given column will be matched as a substring.</p>\n\n<p><code>sort_by_column</code>: A column name to sort the results by.\nThis will sort results in Python after retrieving them from the db.\nUse the 'order_by' param to use SQLite engine for ordering.</p>\n\n<p><code>columns_to_return</code>: Optional list of column names.\nIf provided, the elements returned by this function will only contain the provided columns.\nOtherwise every column in the row is returned.</p>\n\n<p><code>return_as_dataframe</code>: Return the results as a <code>pandas.DataFrame</code> object.</p>\n\n<p><code>values_only</code>: Return the results as a list of tuples.</p>\n\n<p><code>order_by</code>: If given, a <code>order by {order_by}</code> clause will be added to the select query.</p>\n\n<p><code>limit</code>: If given, a <code>limit {limit}</code> clause will be added to the select query.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">match_criteria</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"nb\">dict</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">exact_match</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">sort_by_column</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">columns_to_return</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">return_as_dataframe</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">values_only</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">order_by</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">limit</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">dict</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"n\">pandas</span><span class=\"o\">.</span><span class=\"n\">core</span><span class=\"o\">.</span><span class=\"n\">frame</span><span class=\"o\">.</span><span class=\"n\">DataFrame</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.find",
         "modulename": "databased.databased",
         "qualname": "DataBased.find",
         "kind": "function",
-        "doc": "<p>Search for rows that contain query_string as a substring\nof any column.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>table</strong>:  The table to search.</p></li>\n<li><p><strong>query_string</strong>:  The substring to search for in all columns.</p></li>\n<li><p><strong>columns</strong>:  A list of columns to search for query_string.\nIf None, all columns in the table will be searched.</p></li>\n</ul>\n",
+        "doc": "<p>Search for rows that contain <code>query_string</code> as a substring of any column.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>table</code>: The table to search.</p>\n\n<p><code>query_string</code>: The substring to search for in all columns.</p>\n\n<p><code>columns</code>: A list of columns to search for query_string.\nIf None, all columns in the table will be searched.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">query_string</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">columns</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">dict</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.delete",
         "modulename": "databased.databased",
         "qualname": "DataBased.delete",
         "kind": "function",
-        "doc": "<p>Delete records from table.</p>\n\n<p>Returns number of deleted records.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each\ntuple is (columnName, rowValue) or a dictionary where\nkeys are column names and values are row values.</p></li>\n<li><p><strong>exact_match</strong>:  If False, the rowValue for a give column\nwill be matched as a substring.</p></li>\n</ul>\n",
+        "doc": "<p>Delete records from <code>table</code>.</p>\n\n<p>Returns the number of deleted records.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>match_criteria</code>: Can be a list of 2-tuples where each tuple is <code>(column_name, value)</code>\nor a dictionary where keys are column names and values are corresponding values.</p>\n\n<p><code>exact_match</code>: If <code>False</code>, the value for a given column will be matched as a substring.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">match_criteria</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"nb\">dict</span>,</span><span class=\"param\">\t<span class=\"n\">exact_match</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.update",
         "modulename": "databased.databased",
         "qualname": "DataBased.update",
         "kind": "function",
-        "doc": "<p>Update row value for entry matched with match_criteria.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>column_to_update</strong>:  The column to be updated in the matched row.</p></li>\n<li><p><strong>new_value</strong>:  The new value to insert.</p></li>\n<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each\ntuple is (columnName, rowValue) or a dictionary where\nkeys are column names and values are row values.\nIf None, every row will be updated.</p></li>\n</ul>\n\n<p>Returns True if successful, False if not.</p>\n",
+        "doc": "<p>Update the value in <code>column_to_update</code> to <code>new_value</code> for rows matched with <code>match_criteria</code>.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>table</code>: The table to update rows in.</p>\n\n<p><code>column_to_update</code>: The column to be updated in the matched rows.</p>\n\n<p><code>new_value</code>: The new value to insert.</p>\n\n<p><code>match_criteria</code>: Can be a list of 2-tuples where each tuple is <code>(columnName, rowValue)</code>\nor a dictionary where keys are column names and values are corresponding values.\nIf <code>None</code>, every row in <code>table</code> will be updated.</p>\n\n<p>Returns <code>True</code> if successful, <code>False</code> if not.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">column_to_update</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">new_value</span><span class=\"p\">:</span> <span class=\"n\">Any</span>,</span><span class=\"param\">\t<span class=\"n\">match_criteria</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"nb\">dict</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.drop_table",
         "modulename": "databased.databased",
         "qualname": "DataBased.drop_table",
         "kind": "function",
-        "doc": "<p>Drop a table from the database.</p>\n\n<p>Returns True if successful, False if not.</p>\n",
+        "doc": "<p>Drop <code>table</code> from the database.</p>\n\n<p>Returns <code>True</code> if successful, <code>False</code> if not.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.add_column",
         "modulename": "databased.databased",
         "qualname": "DataBased.add_column",
         "kind": "function",
-        "doc": "<p>Add a new column to table.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>column</strong>:  Name of the column to add.</p></li>\n<li><p><strong>_type</strong>:  The data type of the new column.</p></li>\n<li><p><strong>default_value</strong>:  Optional default value for the column.</p></li>\n</ul>\n",
+        "doc": "<p>Add a new column to <code>table</code>.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>column</code>: Name of the column to add.</p>\n\n<p><code>_type</code>: The data type of the new column.</p>\n\n<p><code>default_value</code>: Optional default value for the column.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">table</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">column</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">_type</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">default_value</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.data_to_string",
         "modulename": "databased.databased",
         "qualname": "DataBased.data_to_string",
         "kind": "function",
-        "doc": "<p>Uses tabulate to produce pretty string output\nfrom a list of dictionaries.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>data</strong>:  Assumes all dictionaries in list have the same set of keys.</p></li>\n<li><p><strong>sort_key</strong>:  Optional dictionary key to sort data with.</p></li>\n<li><p><strong>wrap_to_terminal</strong>:  If True, the table width will be wrapped\nto fit within the current terminal window. Set to False\nif the output is going into something like a txt file.</p></li>\n</ul>\n",
+        "doc": "<p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>data</code>: The list of dictionaries to create a grid from.\nAssumes all dictionaries in list have the same set of keys.</p>\n\n<p><code>sort_key</code>: Optional dictionary key to sort data with.</p>\n\n<p><code>wrap_to_terminal</code>: If <code>True</code>, the table width will be wrapped to fit within the current terminal window.\nPass as <code>False</code> if the output is going into something like a <code>.txt</code> file.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">data</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">dict</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">sort_key</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">wrap_to_terminal</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.data_to_string",
         "modulename": "databased.databased",
         "qualname": "data_to_string",
         "kind": "function",
-        "doc": "<p>Use tabulate to produce grid output from a list of dictionaries.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>data</strong>:  Assumes all dictionaries in list have the same set of keys.</p></li>\n<li><p><strong>sort_key</strong>:  Optional dictionary key to sort data with.</p></li>\n<li><p><strong>wrap_to_terminal</strong>:  If True, the column widths will be reduced so the grid fits\nwithin the current terminal window without wrapping. If the column widths have reduced to 1\nand the grid is still too wide, str(data) will be returned.</p></li>\n</ul>\n",
+        "doc": "<p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>data</code>: The list of dictionaries to create a grid from.\nAssumes all dictionaries in list have the same set of keys.</p>\n\n<p><code>sort_key</code>: Optional dictionary key to sort data with.</p>\n\n<p><code>wrap_to_terminal</code>: If <code>True</code>, the table width will be wrapped to fit within the current terminal window.\nPass as <code>False</code> if the output is going into something like a <code>.txt</code> file.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">data</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">dict</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">sort_key</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">wrap_to_terminal</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.dbmanager",
         "modulename": "databased.dbmanager",
         "kind": "module",
         "doc": "<p></p>\n"
@@ -926,17 +926,17 @@
         "modulename": "databased.dbmanager",
         "qualname": "DBManager.do_info",
         "kind": "function",
         "doc": "<p>Print out the names of the database tables, their columns, and the number of rows.\nPass a space-separated list of table names to only print info for those specific tables,\notherwise all tables will be printed.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">arg</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "databased.dbmanager.DBManager.do_find",
+        "fullname": "databased.dbmanager.DBManager.do_show",
         "modulename": "databased.dbmanager",
-        "qualname": "DBManager.do_find",
+        "qualname": "DBManager.do_show",
         "kind": "function",
         "doc": "<p>Find and print rows from the database.\nUse the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.\nUse the -c/--columns flag to limit what columns are printed.\nUse the -o/--order_by flag to order the results.\nUse the -p/--partial_matching flag to enable substring matching on -m/--match_pairs\nPass -h/--help flag for parser help.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.dbmanager.DBManager.do_search",
         "modulename": "databased.dbmanager",
```

### Comparing `databased-1.5.0/docs/databased/custom_manager.html` & `databased-1.5.1/docs/databased/custom_manager.html`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                 <dd id="CustomManager.do_dbpath" class="function"><a href="dbmanager.html#DBManager.do_dbpath">do_dbpath</a></dd>
                 <dd id="CustomManager.do_backup" class="function"><a href="dbmanager.html#DBManager.do_backup">do_backup</a></dd>
                 <dd id="CustomManager.do_size" class="function"><a href="dbmanager.html#DBManager.do_size">do_size</a></dd>
                 <dd id="CustomManager.do_create_table" class="function"><a href="dbmanager.html#DBManager.do_create_table">do_create_table</a></dd>
                 <dd id="CustomManager.do_drop_table" class="function"><a href="dbmanager.html#DBManager.do_drop_table">do_drop_table</a></dd>
                 <dd id="CustomManager.do_add_row" class="function"><a href="dbmanager.html#DBManager.do_add_row">do_add_row</a></dd>
                 <dd id="CustomManager.do_info" class="function"><a href="dbmanager.html#DBManager.do_info">do_info</a></dd>
-                <dd id="CustomManager.do_find" class="function"><a href="dbmanager.html#DBManager.do_find">do_find</a></dd>
+                <dd id="CustomManager.do_show" class="function"><a href="dbmanager.html#DBManager.do_show">do_show</a></dd>
                 <dd id="CustomManager.do_search" class="function"><a href="dbmanager.html#DBManager.do_search">do_search</a></dd>
                 <dd id="CustomManager.do_count" class="function"><a href="dbmanager.html#DBManager.do_count">do_count</a></dd>
                 <dd id="CustomManager.do_query" class="function"><a href="dbmanager.html#DBManager.do_query">do_query</a></dd>
                 <dd id="CustomManager.do_update" class="function"><a href="dbmanager.html#DBManager.do_update">do_update</a></dd>
                 <dd id="CustomManager.do_delete" class="function"><a href="dbmanager.html#DBManager.do_delete">do_delete</a></dd>
                 <dd id="CustomManager.do_flush_log" class="function"><a href="dbmanager.html#DBManager.do_flush_log">do_flush_log</a></dd>
                 <dd id="CustomManager.do_customize" class="function"><a href="dbmanager.html#DBManager.do_customize">do_customize</a></dd>
```

### Comparing `databased-1.5.0/docs/databased/databased.html` & `databased-1.5.1/docs/databased/databased.html`

 * *Files 2% similar despite different names*

```diff
@@ -146,530 +146,543 @@
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="bp">self</span><span class="p">,</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">,</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="p">):</span>
 </span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">        :param dbpath: String or Path object to database file.</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">        same directory.</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">        :param logger_message_format: &#39;{&#39; style format string</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">        for the logger object.&quot;&quot;&quot;</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="p">)</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="p">)</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="p">):</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="sd">&quot;&quot;&quot;:param message_format: &#39;{&#39; style format string&quot;&quot;&quot;</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="p">)</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                <span class="p">)</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>            <span class="p">)</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">        :param table: The table that values were pulled from.</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">        :param values: List of values expected to be the same quantity</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">        `dbpath`: String or Path object to database file.</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">        same directory.</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">        `logger_message_format`: &#39;{&#39; style format string for the logger object.&quot;&quot;&quot;</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="p">)</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1;&quot;</span><span class="p">)</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="p">):</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="sd">&quot;&quot;&quot;:param `message_format`: &#39;{&#39; style format string&quot;&quot;&quot;</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>            <span class="p">)</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>                <span class="p">)</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>            <span class="p">)</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">        `table`: The table that values were pulled from.</span>
 </span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">        :param columns_to_return: An optional list of column names.</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">return</span> <span class="p">{</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="p">}</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        Usage e.g.:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">        `values`: List of values expected to be the same quantity</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">        `columns_to_return`: An optional list of column names.</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="p">{</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="p">}</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        self.cursor.execute(f&#39;select * from {table} where {conditions}&#39;)&quot;&quot;&quot;</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="p">)</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">        Usage e.g.:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">        &gt;&gt;&gt; self.cursor.execute(f&#39;select * from {table} where {conditions};&#39;)&quot;&quot;&quot;</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
 </span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
 </span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
 </span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="p">)</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="p">)</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        :param table_querys: Each query should be</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        :param table: Name of the table to create.</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">        proper Sqlite3 sytax.</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">)</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        match_criteria is None.</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>                <span class="p">)</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="p">):</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="p">)</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>                <span class="p">)</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">        :param table: The table to insert into.</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="sd">        a value for every column in the table. If columns is</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>                    <span class="n">values</span><span class="p">,</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                <span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="p">)</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                <span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">        column name: row value.</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="p">):</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>                    <span class="n">values</span><span class="p">,</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>                <span class="p">)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>                <span class="p">)</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>                <span class="p">)</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
 </span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">        in the row is returned.</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
 </span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">        one is provided.</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
 </span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="sd">        will be added to the select query.</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">        added to the select query.</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>            <span class="k">return</span> <span class="n">results</span>
-</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>
-</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
-</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a><span class="sd">        of any column.</span>
-</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>
-</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a><span class="sd">        :param table: The table to search.</span>
-</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>
-</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
-</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
-</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>                <span class="p">[</span>
-</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a>                    <span class="n">row</span>
-</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a>                    <span class="p">)</span>
-</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a>                <span class="p">]</span>
-</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a>            <span class="p">)</span>
-</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a>        <span class="k">return</span> <span class="n">results</span>
-</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a>
-</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
-</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a>
-</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">        Returns number of deleted records.</span>
-</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a>
-</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a>
-</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>            <span class="p">)</span>
-</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
-</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>
-</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
-</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>
-</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
-</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a>
-</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="sd">        :param new_value: The new value to insert.</span>
-</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a>
-</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="sd">        If None, every row will be updated.</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>
+</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
+</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>
+</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a>
+</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a>
+</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a>
+</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
+</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a>                <span class="p">[</span>
+</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a>                    <span class="n">row</span>
+</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a>                    <span class="p">)</span>
+</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a>                <span class="p">]</span>
+</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>            <span class="p">)</span>
+</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a>
+</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
+</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a>
+</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">        Returns the number of deleted records.</span>
+</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a>
+</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a>
+</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
+</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>
+</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
+</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>            <span class="p">)</span>
+</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
+</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>
+</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
+</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a>
+</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a>
+</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="sd">        `table`: The table to update rows in.</span>
+</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a>
+</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
 </span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a>
-</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
-</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>                <span class="p">)</span>
-</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>                <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
-</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>            <span class="p">)</span>
-</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>            <span class="p">)</span>
-</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a>            <span class="p">)</span>
-</span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a>
-</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
-</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a>
-</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>
-</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>    <span class="p">):</span>
-</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
-</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>
-</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a><span class="sd">        :param column: Name of the column to add.</span>
-</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>
-</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a><span class="sd">        :param _type: The data type of the new column.</span>
-</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>
-</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>                <span class="p">)</span>
-</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a>
-</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
-</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a><span class="sd">        from a list of dictionaries.</span>
-</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>
-</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>
-</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>
-</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
-</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
-</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
-</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="sd">        `new_value`: The new value to insert.</span>
+</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a>
+</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
+</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a>
+</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
+</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a>                <span class="p">)</span>
+</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>                <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
+</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
+</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>            <span class="p">)</span>
+</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a>            <span class="p">)</span>
+</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a>            <span class="p">)</span>
+</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>
+</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>
+</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>
+</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a>    <span class="p">):</span>
+</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
+</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>
+</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>
+</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>
+</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>
+</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>                <span class="p">)</span>
+</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
+</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a>
+</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
 </span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a>
-</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>
-</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>    <span class="sd">&quot;&quot;&quot;Use tabulate to produce grid output from a list of dictionaries.</span>
-</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>
-</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a><span class="sd">    :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a>
-</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">    :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>
-</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a><span class="sd">    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits</span>
-</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a><span class="sd">    within the current terminal window without wrapping. If the column widths have reduced to 1</span>
-</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="sd">    and the grid is still too wide, str(data) will be returned.&quot;&quot;&quot;</span>
-</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>
-</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
-</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
-</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>    <span class="c1"># to see if shrinking is necessary</span>
-</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>        <span class="n">data</span><span class="p">,</span>
-</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>    <span class="p">)</span>
-</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...&quot;</span><span class="p">)</span>
-</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
-</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
-</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
-</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
-</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
-</span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
-</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a>                <span class="p">)</span>
-</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a>                <span class="n">data</span><span class="p">,</span>
-</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>            <span class="p">)</span>
-</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
-</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>    <span class="k">return</span> <span class="n">output</span>
+</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a>
+</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>
+</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a>
+</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a>
+</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>
+</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>
+</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>
+</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>
+</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>
+</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
+</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>
+</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
+</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
+</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a>    <span class="c1"># to see if shrinking is necessary</span>
+</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>        <span class="n">data</span><span class="p">,</span>
+</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a>    <span class="p">)</span>
+</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
+</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;=</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
+</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
+</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
+</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
+</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
+</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>                <span class="p">)</span>
+</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a>                <span class="n">data</span><span class="p">,</span>
+</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a>            <span class="p">)</span>
+</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
+</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a>    <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DataBased">
                             <input id="DataBased-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -691,464 +704,475 @@
 </span><span id="DataBased-34"><a href="#DataBased-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
 </span><span id="DataBased-35"><a href="#DataBased-35"><span class="linenos"> 35</span></a>        <span class="bp">self</span><span class="p">,</span>
 </span><span id="DataBased-36"><a href="#DataBased-36"><span class="linenos"> 36</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">,</span>
 </span><span id="DataBased-37"><a href="#DataBased-37"><span class="linenos"> 37</span></a>        <span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
 </span><span id="DataBased-38"><a href="#DataBased-38"><span class="linenos"> 38</span></a>        <span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
 </span><span id="DataBased-39"><a href="#DataBased-39"><span class="linenos"> 39</span></a>    <span class="p">):</span>
 </span><span id="DataBased-40"><a href="#DataBased-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="DataBased-41"><a href="#DataBased-41"><span class="linenos"> 41</span></a><span class="sd">        :param dbpath: String or Path object to database file.</span>
-</span><span id="DataBased-42"><a href="#DataBased-42"><span class="linenos"> 42</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
-</span><span id="DataBased-43"><a href="#DataBased-43"><span class="linenos"> 43</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
-</span><span id="DataBased-44"><a href="#DataBased-44"><span class="linenos"> 44</span></a><span class="sd">        same directory.</span>
-</span><span id="DataBased-45"><a href="#DataBased-45"><span class="linenos"> 45</span></a>
-</span><span id="DataBased-46"><a href="#DataBased-46"><span class="linenos"> 46</span></a><span class="sd">        :param logger_message_format: &#39;{&#39; style format string</span>
-</span><span id="DataBased-47"><a href="#DataBased-47"><span class="linenos"> 47</span></a><span class="sd">        for the logger object.&quot;&quot;&quot;</span>
-</span><span id="DataBased-48"><a href="#DataBased-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DataBased-49"><a href="#DataBased-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
-</span><span id="DataBased-50"><a href="#DataBased-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="DataBased-51"><a href="#DataBased-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
-</span><span id="DataBased-52"><a href="#DataBased-52"><span class="linenos"> 52</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
-</span><span id="DataBased-53"><a href="#DataBased-53"><span class="linenos"> 53</span></a>        <span class="p">)</span>
-</span><span id="DataBased-54"><a href="#DataBased-54"><span class="linenos"> 54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="DataBased-55"><a href="#DataBased-55"><span class="linenos"> 55</span></a>
-</span><span id="DataBased-56"><a href="#DataBased-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-57"><a href="#DataBased-57"><span class="linenos"> 57</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
-</span><span id="DataBased-58"><a href="#DataBased-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="DataBased-59"><a href="#DataBased-59"><span class="linenos"> 59</span></a>
-</span><span id="DataBased-60"><a href="#DataBased-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
-</span><span id="DataBased-61"><a href="#DataBased-61"><span class="linenos"> 61</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DataBased-62"><a href="#DataBased-62"><span class="linenos"> 62</span></a>
-</span><span id="DataBased-63"><a href="#DataBased-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-64"><a href="#DataBased-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
-</span><span id="DataBased-65"><a href="#DataBased-65"><span class="linenos"> 65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-</span><span id="DataBased-66"><a href="#DataBased-66"><span class="linenos"> 66</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
-</span><span id="DataBased-67"><a href="#DataBased-67"><span class="linenos"> 67</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
-</span><span id="DataBased-68"><a href="#DataBased-68"><span class="linenos"> 68</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
-</span><span id="DataBased-69"><a href="#DataBased-69"><span class="linenos"> 69</span></a>        <span class="p">)</span>
-</span><span id="DataBased-70"><a href="#DataBased-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
-</span><span id="DataBased-71"><a href="#DataBased-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
-</span><span id="DataBased-72"><a href="#DataBased-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-73"><a href="#DataBased-73"><span class="linenos"> 73</span></a>
-</span><span id="DataBased-74"><a href="#DataBased-74"><span class="linenos"> 74</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-75"><a href="#DataBased-75"><span class="linenos"> 75</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
-</span><span id="DataBased-76"><a href="#DataBased-76"><span class="linenos"> 76</span></a>
-</span><span id="DataBased-77"><a href="#DataBased-77"><span class="linenos"> 77</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
-</span><span id="DataBased-78"><a href="#DataBased-78"><span class="linenos"> 78</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
-</span><span id="DataBased-79"><a href="#DataBased-79"><span class="linenos"> 79</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
-</span><span id="DataBased-80"><a href="#DataBased-80"><span class="linenos"> 80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
-</span><span id="DataBased-81"><a href="#DataBased-81"><span class="linenos"> 81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DataBased-82"><a href="#DataBased-82"><span class="linenos"> 82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="DataBased-83"><a href="#DataBased-83"><span class="linenos"> 83</span></a>
-</span><span id="DataBased-84"><a href="#DataBased-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
-</span><span id="DataBased-85"><a href="#DataBased-85"><span class="linenos"> 85</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-86"><a href="#DataBased-86"><span class="linenos"> 86</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="DataBased-87"><a href="#DataBased-87"><span class="linenos"> 87</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
-</span><span id="DataBased-88"><a href="#DataBased-88"><span class="linenos"> 88</span></a>    <span class="p">):</span>
-</span><span id="DataBased-89"><a href="#DataBased-89"><span class="linenos"> 89</span></a>        <span class="sd">&quot;&quot;&quot;:param message_format: &#39;{&#39; style format string&quot;&quot;&quot;</span>
-</span><span id="DataBased-90"><a href="#DataBased-90"><span class="linenos"> 90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
-</span><span id="DataBased-91"><a href="#DataBased-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
-</span><span id="DataBased-92"><a href="#DataBased-92"><span class="linenos"> 92</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
-</span><span id="DataBased-93"><a href="#DataBased-93"><span class="linenos"> 93</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
-</span><span id="DataBased-94"><a href="#DataBased-94"><span class="linenos"> 94</span></a>            <span class="p">)</span>
-</span><span id="DataBased-95"><a href="#DataBased-95"><span class="linenos"> 95</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
-</span><span id="DataBased-96"><a href="#DataBased-96"><span class="linenos"> 96</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
-</span><span id="DataBased-97"><a href="#DataBased-97"><span class="linenos"> 97</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
-</span><span id="DataBased-98"><a href="#DataBased-98"><span class="linenos"> 98</span></a>                <span class="p">)</span>
-</span><span id="DataBased-99"><a href="#DataBased-99"><span class="linenos"> 99</span></a>            <span class="p">)</span>
-</span><span id="DataBased-100"><a href="#DataBased-100"><span class="linenos">100</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
-</span><span id="DataBased-101"><a href="#DataBased-101"><span class="linenos">101</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
-</span><span id="DataBased-102"><a href="#DataBased-102"><span class="linenos">102</span></a>
-</span><span id="DataBased-103"><a href="#DataBased-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
-</span><span id="DataBased-104"><a href="#DataBased-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-105"><a href="#DataBased-105"><span class="linenos">105</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="DataBased-106"><a href="#DataBased-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
-</span><span id="DataBased-107"><a href="#DataBased-107"><span class="linenos">107</span></a>
-</span><span id="DataBased-108"><a href="#DataBased-108"><span class="linenos">108</span></a><span class="sd">        :param table: The table that values were pulled from.</span>
-</span><span id="DataBased-109"><a href="#DataBased-109"><span class="linenos">109</span></a>
-</span><span id="DataBased-110"><a href="#DataBased-110"><span class="linenos">110</span></a><span class="sd">        :param values: List of values expected to be the same quantity</span>
-</span><span id="DataBased-111"><a href="#DataBased-111"><span class="linenos">111</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="DataBased-41"><a href="#DataBased-41"><span class="linenos"> 41</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-42"><a href="#DataBased-42"><span class="linenos"> 42</span></a>
+</span><span id="DataBased-43"><a href="#DataBased-43"><span class="linenos"> 43</span></a><span class="sd">        `dbpath`: String or Path object to database file.</span>
+</span><span id="DataBased-44"><a href="#DataBased-44"><span class="linenos"> 44</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
+</span><span id="DataBased-45"><a href="#DataBased-45"><span class="linenos"> 45</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
+</span><span id="DataBased-46"><a href="#DataBased-46"><span class="linenos"> 46</span></a><span class="sd">        same directory.</span>
+</span><span id="DataBased-47"><a href="#DataBased-47"><span class="linenos"> 47</span></a>
+</span><span id="DataBased-48"><a href="#DataBased-48"><span class="linenos"> 48</span></a><span class="sd">        `logger_message_format`: &#39;{&#39; style format string for the logger object.&quot;&quot;&quot;</span>
+</span><span id="DataBased-49"><a href="#DataBased-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DataBased-50"><a href="#DataBased-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
+</span><span id="DataBased-51"><a href="#DataBased-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="DataBased-52"><a href="#DataBased-52"><span class="linenos"> 52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
+</span><span id="DataBased-53"><a href="#DataBased-53"><span class="linenos"> 53</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
+</span><span id="DataBased-54"><a href="#DataBased-54"><span class="linenos"> 54</span></a>        <span class="p">)</span>
+</span><span id="DataBased-55"><a href="#DataBased-55"><span class="linenos"> 55</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="DataBased-56"><a href="#DataBased-56"><span class="linenos"> 56</span></a>
+</span><span id="DataBased-57"><a href="#DataBased-57"><span class="linenos"> 57</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased-58"><a href="#DataBased-58"><span class="linenos"> 58</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
+</span><span id="DataBased-59"><a href="#DataBased-59"><span class="linenos"> 59</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="DataBased-60"><a href="#DataBased-60"><span class="linenos"> 60</span></a>
+</span><span id="DataBased-61"><a href="#DataBased-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
+</span><span id="DataBased-62"><a href="#DataBased-62"><span class="linenos"> 62</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DataBased-63"><a href="#DataBased-63"><span class="linenos"> 63</span></a>
+</span><span id="DataBased-64"><a href="#DataBased-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased-65"><a href="#DataBased-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
+</span><span id="DataBased-66"><a href="#DataBased-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
+</span><span id="DataBased-67"><a href="#DataBased-67"><span class="linenos"> 67</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
+</span><span id="DataBased-68"><a href="#DataBased-68"><span class="linenos"> 68</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
+</span><span id="DataBased-69"><a href="#DataBased-69"><span class="linenos"> 69</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
+</span><span id="DataBased-70"><a href="#DataBased-70"><span class="linenos"> 70</span></a>        <span class="p">)</span>
+</span><span id="DataBased-71"><a href="#DataBased-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-72"><a href="#DataBased-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
+</span><span id="DataBased-73"><a href="#DataBased-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-74"><a href="#DataBased-74"><span class="linenos"> 74</span></a>
+</span><span id="DataBased-75"><a href="#DataBased-75"><span class="linenos"> 75</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased-76"><a href="#DataBased-76"><span class="linenos"> 76</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
+</span><span id="DataBased-77"><a href="#DataBased-77"><span class="linenos"> 77</span></a>
+</span><span id="DataBased-78"><a href="#DataBased-78"><span class="linenos"> 78</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
+</span><span id="DataBased-79"><a href="#DataBased-79"><span class="linenos"> 79</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
+</span><span id="DataBased-80"><a href="#DataBased-80"><span class="linenos"> 80</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
+</span><span id="DataBased-81"><a href="#DataBased-81"><span class="linenos"> 81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
+</span><span id="DataBased-82"><a href="#DataBased-82"><span class="linenos"> 82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DataBased-83"><a href="#DataBased-83"><span class="linenos"> 83</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="DataBased-84"><a href="#DataBased-84"><span class="linenos"> 84</span></a>
+</span><span id="DataBased-85"><a href="#DataBased-85"><span class="linenos"> 85</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
+</span><span id="DataBased-86"><a href="#DataBased-86"><span class="linenos"> 86</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-87"><a href="#DataBased-87"><span class="linenos"> 87</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="DataBased-88"><a href="#DataBased-88"><span class="linenos"> 88</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
+</span><span id="DataBased-89"><a href="#DataBased-89"><span class="linenos"> 89</span></a>    <span class="p">):</span>
+</span><span id="DataBased-90"><a href="#DataBased-90"><span class="linenos"> 90</span></a>        <span class="sd">&quot;&quot;&quot;:param `message_format`: &#39;{&#39; style format string&quot;&quot;&quot;</span>
+</span><span id="DataBased-91"><a href="#DataBased-91"><span class="linenos"> 91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
+</span><span id="DataBased-92"><a href="#DataBased-92"><span class="linenos"> 92</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
+</span><span id="DataBased-93"><a href="#DataBased-93"><span class="linenos"> 93</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
+</span><span id="DataBased-94"><a href="#DataBased-94"><span class="linenos"> 94</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
+</span><span id="DataBased-95"><a href="#DataBased-95"><span class="linenos"> 95</span></a>            <span class="p">)</span>
+</span><span id="DataBased-96"><a href="#DataBased-96"><span class="linenos"> 96</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
+</span><span id="DataBased-97"><a href="#DataBased-97"><span class="linenos"> 97</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
+</span><span id="DataBased-98"><a href="#DataBased-98"><span class="linenos"> 98</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
+</span><span id="DataBased-99"><a href="#DataBased-99"><span class="linenos"> 99</span></a>                <span class="p">)</span>
+</span><span id="DataBased-100"><a href="#DataBased-100"><span class="linenos">100</span></a>            <span class="p">)</span>
+</span><span id="DataBased-101"><a href="#DataBased-101"><span class="linenos">101</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
+</span><span id="DataBased-102"><a href="#DataBased-102"><span class="linenos">102</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
+</span><span id="DataBased-103"><a href="#DataBased-103"><span class="linenos">103</span></a>
+</span><span id="DataBased-104"><a href="#DataBased-104"><span class="linenos">104</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
+</span><span id="DataBased-105"><a href="#DataBased-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-106"><a href="#DataBased-106"><span class="linenos">106</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="DataBased-107"><a href="#DataBased-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
+</span><span id="DataBased-108"><a href="#DataBased-108"><span class="linenos">108</span></a>
+</span><span id="DataBased-109"><a href="#DataBased-109"><span class="linenos">109</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-110"><a href="#DataBased-110"><span class="linenos">110</span></a>
+</span><span id="DataBased-111"><a href="#DataBased-111"><span class="linenos">111</span></a><span class="sd">        `table`: The table that values were pulled from.</span>
 </span><span id="DataBased-112"><a href="#DataBased-112"><span class="linenos">112</span></a>
-</span><span id="DataBased-113"><a href="#DataBased-113"><span class="linenos">113</span></a><span class="sd">        :param columns_to_return: An optional list of column names.</span>
-</span><span id="DataBased-114"><a href="#DataBased-114"><span class="linenos">114</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
-</span><span id="DataBased-115"><a href="#DataBased-115"><span class="linenos">115</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
-</span><span id="DataBased-116"><a href="#DataBased-116"><span class="linenos">116</span></a>        <span class="k">return</span> <span class="p">{</span>
-</span><span id="DataBased-117"><a href="#DataBased-117"><span class="linenos">117</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
-</span><span id="DataBased-118"><a href="#DataBased-118"><span class="linenos">118</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-119"><a href="#DataBased-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
-</span><span id="DataBased-120"><a href="#DataBased-120"><span class="linenos">120</span></a>        <span class="p">}</span>
-</span><span id="DataBased-121"><a href="#DataBased-121"><span class="linenos">121</span></a>
-</span><span id="DataBased-122"><a href="#DataBased-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
-</span><span id="DataBased-123"><a href="#DataBased-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-124"><a href="#DataBased-124"><span class="linenos">124</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-125"><a href="#DataBased-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
-</span><span id="DataBased-126"><a href="#DataBased-126"><span class="linenos">126</span></a>
-</span><span id="DataBased-127"><a href="#DataBased-127"><span class="linenos">127</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-128"><a href="#DataBased-128"><span class="linenos">128</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-129"><a href="#DataBased-129"><span class="linenos">129</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-130"><a href="#DataBased-130"><span class="linenos">130</span></a>
-</span><span id="DataBased-131"><a href="#DataBased-131"><span class="linenos">131</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased-132"><a href="#DataBased-132"><span class="linenos">132</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased-133"><a href="#DataBased-133"><span class="linenos">133</span></a>
-</span><span id="DataBased-134"><a href="#DataBased-134"><span class="linenos">134</span></a><span class="sd">        Usage e.g.:</span>
+</span><span id="DataBased-113"><a href="#DataBased-113"><span class="linenos">113</span></a><span class="sd">        `values`: List of values expected to be the same quantity</span>
+</span><span id="DataBased-114"><a href="#DataBased-114"><span class="linenos">114</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="DataBased-115"><a href="#DataBased-115"><span class="linenos">115</span></a>
+</span><span id="DataBased-116"><a href="#DataBased-116"><span class="linenos">116</span></a><span class="sd">        `columns_to_return`: An optional list of column names.</span>
+</span><span id="DataBased-117"><a href="#DataBased-117"><span class="linenos">117</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
+</span><span id="DataBased-118"><a href="#DataBased-118"><span class="linenos">118</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
+</span><span id="DataBased-119"><a href="#DataBased-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="p">{</span>
+</span><span id="DataBased-120"><a href="#DataBased-120"><span class="linenos">120</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
+</span><span id="DataBased-121"><a href="#DataBased-121"><span class="linenos">121</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-122"><a href="#DataBased-122"><span class="linenos">122</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
+</span><span id="DataBased-123"><a href="#DataBased-123"><span class="linenos">123</span></a>        <span class="p">}</span>
+</span><span id="DataBased-124"><a href="#DataBased-124"><span class="linenos">124</span></a>
+</span><span id="DataBased-125"><a href="#DataBased-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
+</span><span id="DataBased-126"><a href="#DataBased-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-127"><a href="#DataBased-127"><span class="linenos">127</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-128"><a href="#DataBased-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
+</span><span id="DataBased-129"><a href="#DataBased-129"><span class="linenos">129</span></a>
+</span><span id="DataBased-130"><a href="#DataBased-130"><span class="linenos">130</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-131"><a href="#DataBased-131"><span class="linenos">131</span></a>
+</span><span id="DataBased-132"><a href="#DataBased-132"><span class="linenos">132</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-133"><a href="#DataBased-133"><span class="linenos">133</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased-134"><a href="#DataBased-134"><span class="linenos">134</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="DataBased-135"><a href="#DataBased-135"><span class="linenos">135</span></a>
-</span><span id="DataBased-136"><a href="#DataBased-136"><span class="linenos">136</span></a><span class="sd">        self.cursor.execute(f&#39;select * from {table} where {conditions}&#39;)&quot;&quot;&quot;</span>
-</span><span id="DataBased-137"><a href="#DataBased-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="DataBased-138"><a href="#DataBased-138"><span class="linenos">138</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
-</span><span id="DataBased-139"><a href="#DataBased-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
-</span><span id="DataBased-140"><a href="#DataBased-140"><span class="linenos">140</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DataBased-141"><a href="#DataBased-141"><span class="linenos">141</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
-</span><span id="DataBased-142"><a href="#DataBased-142"><span class="linenos">142</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="DataBased-143"><a href="#DataBased-143"><span class="linenos">143</span></a>            <span class="p">)</span>
-</span><span id="DataBased-144"><a href="#DataBased-144"><span class="linenos">144</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-136"><a href="#DataBased-136"><span class="linenos">136</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="DataBased-137"><a href="#DataBased-137"><span class="linenos">137</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased-138"><a href="#DataBased-138"><span class="linenos">138</span></a>
+</span><span id="DataBased-139"><a href="#DataBased-139"><span class="linenos">139</span></a><span class="sd">        Usage e.g.:</span>
+</span><span id="DataBased-140"><a href="#DataBased-140"><span class="linenos">140</span></a>
+</span><span id="DataBased-141"><a href="#DataBased-141"><span class="linenos">141</span></a><span class="sd">        &gt;&gt;&gt; self.cursor.execute(f&#39;select * from {table} where {conditions};&#39;)&quot;&quot;&quot;</span>
+</span><span id="DataBased-142"><a href="#DataBased-142"><span class="linenos">142</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="DataBased-143"><a href="#DataBased-143"><span class="linenos">143</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
+</span><span id="DataBased-144"><a href="#DataBased-144"><span class="linenos">144</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
 </span><span id="DataBased-145"><a href="#DataBased-145"><span class="linenos">145</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DataBased-146"><a href="#DataBased-146"><span class="linenos">146</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
+</span><span id="DataBased-146"><a href="#DataBased-146"><span class="linenos">146</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
 </span><span id="DataBased-147"><a href="#DataBased-147"><span class="linenos">147</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
 </span><span id="DataBased-148"><a href="#DataBased-148"><span class="linenos">148</span></a>            <span class="p">)</span>
-</span><span id="DataBased-149"><a href="#DataBased-149"><span class="linenos">149</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="DataBased-150"><a href="#DataBased-150"><span class="linenos">150</span></a>
-</span><span id="DataBased-151"><a href="#DataBased-151"><span class="linenos">151</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-152"><a href="#DataBased-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="DataBased-153"><a href="#DataBased-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
-</span><span id="DataBased-154"><a href="#DataBased-154"><span class="linenos">154</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
-</span><span id="DataBased-155"><a href="#DataBased-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="DataBased-156"><a href="#DataBased-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased-157"><a href="#DataBased-157"><span class="linenos">157</span></a>
-</span><span id="DataBased-158"><a href="#DataBased-158"><span class="linenos">158</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-159"><a href="#DataBased-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="DataBased-160"><a href="#DataBased-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased-149"><a href="#DataBased-149"><span class="linenos">149</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-150"><a href="#DataBased-150"><span class="linenos">150</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DataBased-151"><a href="#DataBased-151"><span class="linenos">151</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
+</span><span id="DataBased-152"><a href="#DataBased-152"><span class="linenos">152</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
+</span><span id="DataBased-153"><a href="#DataBased-153"><span class="linenos">153</span></a>            <span class="p">)</span>
+</span><span id="DataBased-154"><a href="#DataBased-154"><span class="linenos">154</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="DataBased-155"><a href="#DataBased-155"><span class="linenos">155</span></a>
+</span><span id="DataBased-156"><a href="#DataBased-156"><span class="linenos">156</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-157"><a href="#DataBased-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="DataBased-158"><a href="#DataBased-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
+</span><span id="DataBased-159"><a href="#DataBased-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="DataBased-160"><a href="#DataBased-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span><span id="DataBased-161"><a href="#DataBased-161"><span class="linenos">161</span></a>
-</span><span id="DataBased-162"><a href="#DataBased-162"><span class="linenos">162</span></a><span class="sd">        :param table_querys: Each query should be</span>
-</span><span id="DataBased-163"><a href="#DataBased-163"><span class="linenos">163</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
-</span><span id="DataBased-164"><a href="#DataBased-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased-165"><a href="#DataBased-165"><span class="linenos">165</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DataBased-166"><a href="#DataBased-166"><span class="linenos">166</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
-</span><span id="DataBased-167"><a href="#DataBased-167"><span class="linenos">167</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased-168"><a href="#DataBased-168"><span class="linenos">168</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-169"><a href="#DataBased-169"><span class="linenos">169</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-170"><a href="#DataBased-170"><span class="linenos">170</span></a>
-</span><span id="DataBased-171"><a href="#DataBased-171"><span class="linenos">171</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-172"><a href="#DataBased-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="DataBased-173"><a href="#DataBased-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="DataBased-174"><a href="#DataBased-174"><span class="linenos">174</span></a>
-</span><span id="DataBased-175"><a href="#DataBased-175"><span class="linenos">175</span></a><span class="sd">        :param table: Name of the table to create.</span>
-</span><span id="DataBased-176"><a href="#DataBased-176"><span class="linenos">176</span></a>
-</span><span id="DataBased-177"><a href="#DataBased-177"><span class="linenos">177</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
-</span><span id="DataBased-178"><a href="#DataBased-178"><span class="linenos">178</span></a><span class="sd">        proper Sqlite3 sytax.</span>
-</span><span id="DataBased-179"><a href="#DataBased-179"><span class="linenos">179</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
-</span><span id="DataBased-180"><a href="#DataBased-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased-181"><a href="#DataBased-181"><span class="linenos">181</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="DataBased-182"><a href="#DataBased-182"><span class="linenos">182</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased-183"><a href="#DataBased-183"><span class="linenos">183</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
-</span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a>
-</span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
-</span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
-</span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>        <span class="p">)</span>
-</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
-</span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>
-</span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
-</span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
-</span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>
-</span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-203"><a href="#DataBased-203"><span class="linenos">203</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
-</span><span id="DataBased-207"><a href="#DataBased-207"><span class="linenos">207</span></a>
-</span><span id="DataBased-208"><a href="#DataBased-208"><span class="linenos">208</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-209"><a href="#DataBased-209"><span class="linenos">209</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-210"><a href="#DataBased-210"><span class="linenos">210</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-211"><a href="#DataBased-211"><span class="linenos">211</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
-</span><span id="DataBased-212"><a href="#DataBased-212"><span class="linenos">212</span></a>
-</span><span id="DataBased-213"><a href="#DataBased-213"><span class="linenos">213</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
-</span><span id="DataBased-214"><a href="#DataBased-214"><span class="linenos">214</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
-</span><span id="DataBased-215"><a href="#DataBased-215"><span class="linenos">215</span></a><span class="sd">        match_criteria is None.</span>
-</span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-219"><a href="#DataBased-219"><span class="linenos">219</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a>                <span class="p">)</span>
-</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>
-</span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
-</span><span id="DataBased-231"><a href="#DataBased-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-232"><a href="#DataBased-232"><span class="linenos">232</span></a>    <span class="p">):</span>
-</span><span id="DataBased-233"><a href="#DataBased-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
+</span><span id="DataBased-162"><a href="#DataBased-162"><span class="linenos">162</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-163"><a href="#DataBased-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="DataBased-164"><a href="#DataBased-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased-165"><a href="#DataBased-165"><span class="linenos">165</span></a>
+</span><span id="DataBased-166"><a href="#DataBased-166"><span class="linenos">166</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
+</span><span id="DataBased-167"><a href="#DataBased-167"><span class="linenos">167</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased-168"><a href="#DataBased-168"><span class="linenos">168</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DataBased-169"><a href="#DataBased-169"><span class="linenos">169</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
+</span><span id="DataBased-170"><a href="#DataBased-170"><span class="linenos">170</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="DataBased-171"><a href="#DataBased-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-172"><a href="#DataBased-172"><span class="linenos">172</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-173"><a href="#DataBased-173"><span class="linenos">173</span></a>
+</span><span id="DataBased-174"><a href="#DataBased-174"><span class="linenos">174</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-175"><a href="#DataBased-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="DataBased-176"><a href="#DataBased-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="DataBased-177"><a href="#DataBased-177"><span class="linenos">177</span></a>
+</span><span id="DataBased-178"><a href="#DataBased-178"><span class="linenos">178</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-179"><a href="#DataBased-179"><span class="linenos">179</span></a>
+</span><span id="DataBased-180"><a href="#DataBased-180"><span class="linenos">180</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="DataBased-181"><a href="#DataBased-181"><span class="linenos">181</span></a>
+</span><span id="DataBased-182"><a href="#DataBased-182"><span class="linenos">182</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
+</span><span id="DataBased-183"><a href="#DataBased-183"><span class="linenos">183</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
+</span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a>
+</span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
+</span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
+</span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>        <span class="p">)</span>
+</span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+</span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>
+</span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>
+</span><span id="DataBased-203"><a href="#DataBased-203"><span class="linenos">203</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-207"><a href="#DataBased-207"><span class="linenos">207</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-208"><a href="#DataBased-208"><span class="linenos">208</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-209"><a href="#DataBased-209"><span class="linenos">209</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-210"><a href="#DataBased-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
+</span><span id="DataBased-211"><a href="#DataBased-211"><span class="linenos">211</span></a>
+</span><span id="DataBased-212"><a href="#DataBased-212"><span class="linenos">212</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-213"><a href="#DataBased-213"><span class="linenos">213</span></a>
+</span><span id="DataBased-214"><a href="#DataBased-214"><span class="linenos">214</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-215"><a href="#DataBased-215"><span class="linenos">215</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
+</span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a>
+</span><span id="DataBased-219"><a href="#DataBased-219"><span class="linenos">219</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
+</span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
+</span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>                <span class="p">)</span>
+</span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-231"><a href="#DataBased-231"><span class="linenos">231</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DataBased-232"><a href="#DataBased-232"><span class="linenos">232</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="DataBased-233"><a href="#DataBased-233"><span class="linenos">233</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span><span id="DataBased-234"><a href="#DataBased-234"><span class="linenos">234</span></a>
-</span><span id="DataBased-235"><a href="#DataBased-235"><span class="linenos">235</span></a><span class="sd">        :param table: The table to insert into.</span>
-</span><span id="DataBased-236"><a href="#DataBased-236"><span class="linenos">236</span></a>
-</span><span id="DataBased-237"><a href="#DataBased-237"><span class="linenos">237</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
-</span><span id="DataBased-238"><a href="#DataBased-238"><span class="linenos">238</span></a>
-</span><span id="DataBased-239"><a href="#DataBased-239"><span class="linenos">239</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
-</span><span id="DataBased-240"><a href="#DataBased-240"><span class="linenos">240</span></a><span class="sd">        a value for every column in the table. If columns is</span>
-</span><span id="DataBased-241"><a href="#DataBased-241"><span class="linenos">241</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
-</span><span id="DataBased-242"><a href="#DataBased-242"><span class="linenos">242</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-243"><a href="#DataBased-243"><span class="linenos">243</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-244"><a href="#DataBased-244"><span class="linenos">244</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-245"><a href="#DataBased-245"><span class="linenos">245</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-246"><a href="#DataBased-246"><span class="linenos">246</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="DataBased-247"><a href="#DataBased-247"><span class="linenos">247</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-248"><a href="#DataBased-248"><span class="linenos">248</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span>
-</span><span id="DataBased-249"><a href="#DataBased-249"><span class="linenos">249</span></a>                    <span class="n">values</span><span class="p">,</span>
-</span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a>                <span class="p">)</span>
-</span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
-</span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a>                <span class="p">)</span>
-</span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="DataBased-260"><a href="#DataBased-260"><span class="linenos">260</span></a>                <span class="p">)</span>
-</span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a>
-</span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-270"><a href="#DataBased-270"><span class="linenos">270</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-271"><a href="#DataBased-271"><span class="linenos">271</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-272"><a href="#DataBased-272"><span class="linenos">272</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased-273"><a href="#DataBased-273"><span class="linenos">273</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased-274"><a href="#DataBased-274"><span class="linenos">274</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-275"><a href="#DataBased-275"><span class="linenos">275</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-276"><a href="#DataBased-276"><span class="linenos">276</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="DataBased-277"><a href="#DataBased-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
-</span><span id="DataBased-278"><a href="#DataBased-278"><span class="linenos">278</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
-</span><span id="DataBased-279"><a href="#DataBased-279"><span class="linenos">279</span></a><span class="sd">        column name: row value.</span>
-</span><span id="DataBased-280"><a href="#DataBased-280"><span class="linenos">280</span></a>
-</span><span id="DataBased-281"><a href="#DataBased-281"><span class="linenos">281</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-282"><a href="#DataBased-282"><span class="linenos">282</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-283"><a href="#DataBased-283"><span class="linenos">283</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-284"><a href="#DataBased-284"><span class="linenos">284</span></a>
-</span><span id="DataBased-285"><a href="#DataBased-285"><span class="linenos">285</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased-286"><a href="#DataBased-286"><span class="linenos">286</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased-235"><a href="#DataBased-235"><span class="linenos">235</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-236"><a href="#DataBased-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="DataBased-237"><a href="#DataBased-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-238"><a href="#DataBased-238"><span class="linenos">238</span></a>    <span class="p">):</span>
+</span><span id="DataBased-239"><a href="#DataBased-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
+</span><span id="DataBased-240"><a href="#DataBased-240"><span class="linenos">240</span></a>
+</span><span id="DataBased-241"><a href="#DataBased-241"><span class="linenos">241</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-242"><a href="#DataBased-242"><span class="linenos">242</span></a>
+</span><span id="DataBased-243"><a href="#DataBased-243"><span class="linenos">243</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased-244"><a href="#DataBased-244"><span class="linenos">244</span></a>
+</span><span id="DataBased-245"><a href="#DataBased-245"><span class="linenos">245</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased-246"><a href="#DataBased-246"><span class="linenos">246</span></a>
+</span><span id="DataBased-247"><a href="#DataBased-247"><span class="linenos">247</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="DataBased-248"><a href="#DataBased-248"><span class="linenos">248</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="DataBased-249"><a href="#DataBased-249"><span class="linenos">249</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a>                    <span class="n">values</span><span class="p">,</span>
+</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a>                <span class="p">)</span>
+</span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-260"><a href="#DataBased-260"><span class="linenos">260</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a>                <span class="p">)</span>
+</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
+</span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>                <span class="p">)</span>
+</span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="DataBased-270"><a href="#DataBased-270"><span class="linenos">270</span></a>
+</span><span id="DataBased-271"><a href="#DataBased-271"><span class="linenos">271</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-272"><a href="#DataBased-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="DataBased-273"><a href="#DataBased-273"><span class="linenos">273</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-274"><a href="#DataBased-274"><span class="linenos">274</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-275"><a href="#DataBased-275"><span class="linenos">275</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-276"><a href="#DataBased-276"><span class="linenos">276</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-277"><a href="#DataBased-277"><span class="linenos">277</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-278"><a href="#DataBased-278"><span class="linenos">278</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-279"><a href="#DataBased-279"><span class="linenos">279</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased-280"><a href="#DataBased-280"><span class="linenos">280</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased-281"><a href="#DataBased-281"><span class="linenos">281</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-282"><a href="#DataBased-282"><span class="linenos">282</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-283"><a href="#DataBased-283"><span class="linenos">283</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="DataBased-284"><a href="#DataBased-284"><span class="linenos">284</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
+</span><span id="DataBased-285"><a href="#DataBased-285"><span class="linenos">285</span></a>
+</span><span id="DataBased-286"><a href="#DataBased-286"><span class="linenos">286</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
 </span><span id="DataBased-287"><a href="#DataBased-287"><span class="linenos">287</span></a>
-</span><span id="DataBased-288"><a href="#DataBased-288"><span class="linenos">288</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
-</span><span id="DataBased-289"><a href="#DataBased-289"><span class="linenos">289</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="DataBased-290"><a href="#DataBased-290"><span class="linenos">290</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
-</span><span id="DataBased-291"><a href="#DataBased-291"><span class="linenos">291</span></a>
-</span><span id="DataBased-292"><a href="#DataBased-292"><span class="linenos">292</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
-</span><span id="DataBased-293"><a href="#DataBased-293"><span class="linenos">293</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
-</span><span id="DataBased-294"><a href="#DataBased-294"><span class="linenos">294</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
-</span><span id="DataBased-295"><a href="#DataBased-295"><span class="linenos">295</span></a><span class="sd">        in the row is returned.</span>
+</span><span id="DataBased-288"><a href="#DataBased-288"><span class="linenos">288</span></a>
+</span><span id="DataBased-289"><a href="#DataBased-289"><span class="linenos">289</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-290"><a href="#DataBased-290"><span class="linenos">290</span></a>
+</span><span id="DataBased-291"><a href="#DataBased-291"><span class="linenos">291</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-292"><a href="#DataBased-292"><span class="linenos">292</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased-293"><a href="#DataBased-293"><span class="linenos">293</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-294"><a href="#DataBased-294"><span class="linenos">294</span></a>
+</span><span id="DataBased-295"><a href="#DataBased-295"><span class="linenos">295</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
 </span><span id="DataBased-296"><a href="#DataBased-296"><span class="linenos">296</span></a>
-</span><span id="DataBased-297"><a href="#DataBased-297"><span class="linenos">297</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
-</span><span id="DataBased-298"><a href="#DataBased-298"><span class="linenos">298</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
-</span><span id="DataBased-299"><a href="#DataBased-299"><span class="linenos">299</span></a>
-</span><span id="DataBased-300"><a href="#DataBased-300"><span class="linenos">300</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
-</span><span id="DataBased-301"><a href="#DataBased-301"><span class="linenos">301</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
-</span><span id="DataBased-302"><a href="#DataBased-302"><span class="linenos">302</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
-</span><span id="DataBased-303"><a href="#DataBased-303"><span class="linenos">303</span></a><span class="sd">        one is provided.</span>
+</span><span id="DataBased-297"><a href="#DataBased-297"><span class="linenos">297</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
+</span><span id="DataBased-298"><a href="#DataBased-298"><span class="linenos">298</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="DataBased-299"><a href="#DataBased-299"><span class="linenos">299</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="DataBased-300"><a href="#DataBased-300"><span class="linenos">300</span></a>
+</span><span id="DataBased-301"><a href="#DataBased-301"><span class="linenos">301</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
+</span><span id="DataBased-302"><a href="#DataBased-302"><span class="linenos">302</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
+</span><span id="DataBased-303"><a href="#DataBased-303"><span class="linenos">303</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
 </span><span id="DataBased-304"><a href="#DataBased-304"><span class="linenos">304</span></a>
-</span><span id="DataBased-305"><a href="#DataBased-305"><span class="linenos">305</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
-</span><span id="DataBased-306"><a href="#DataBased-306"><span class="linenos">306</span></a><span class="sd">        will be added to the select query.</span>
-</span><span id="DataBased-307"><a href="#DataBased-307"><span class="linenos">307</span></a>
-</span><span id="DataBased-308"><a href="#DataBased-308"><span class="linenos">308</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
-</span><span id="DataBased-309"><a href="#DataBased-309"><span class="linenos">309</span></a><span class="sd">        added to the select query.</span>
-</span><span id="DataBased-310"><a href="#DataBased-310"><span class="linenos">310</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-311"><a href="#DataBased-311"><span class="linenos">311</span></a>
-</span><span id="DataBased-312"><a href="#DataBased-312"><span class="linenos">312</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-313"><a href="#DataBased-313"><span class="linenos">313</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased-314"><a href="#DataBased-314"><span class="linenos">314</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-315"><a href="#DataBased-315"><span class="linenos">315</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased-316"><a href="#DataBased-316"><span class="linenos">316</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-317"><a href="#DataBased-317"><span class="linenos">317</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-318"><a href="#DataBased-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="DataBased-319"><a href="#DataBased-319"><span class="linenos">319</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-320"><a href="#DataBased-320"><span class="linenos">320</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="DataBased-321"><a href="#DataBased-321"><span class="linenos">321</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-322"><a href="#DataBased-322"><span class="linenos">322</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased-323"><a href="#DataBased-323"><span class="linenos">323</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased-324"><a href="#DataBased-324"><span class="linenos">324</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased-325"><a href="#DataBased-325"><span class="linenos">325</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="DataBased-326"><a href="#DataBased-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="DataBased-327"><a href="#DataBased-327"><span class="linenos">327</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="DataBased-328"><a href="#DataBased-328"><span class="linenos">328</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="DataBased-329"><a href="#DataBased-329"><span class="linenos">329</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="DataBased-330"><a href="#DataBased-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="DataBased-331"><a href="#DataBased-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DataBased-332"><a href="#DataBased-332"><span class="linenos">332</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-333"><a href="#DataBased-333"><span class="linenos">333</span></a>            <span class="k">return</span> <span class="n">results</span>
-</span><span id="DataBased-334"><a href="#DataBased-334"><span class="linenos">334</span></a>
-</span><span id="DataBased-335"><a href="#DataBased-335"><span class="linenos">335</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-336"><a href="#DataBased-336"><span class="linenos">336</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="DataBased-337"><a href="#DataBased-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-338"><a href="#DataBased-338"><span class="linenos">338</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
-</span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a><span class="sd">        of any column.</span>
-</span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a>
-</span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a><span class="sd">        :param table: The table to search.</span>
-</span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a>
-</span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
-</span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a>
-</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
-</span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DataBased-354"><a href="#DataBased-354"><span class="linenos">354</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-355"><a href="#DataBased-355"><span class="linenos">355</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="DataBased-356"><a href="#DataBased-356"><span class="linenos">356</span></a>                <span class="p">[</span>
-</span><span id="DataBased-357"><a href="#DataBased-357"><span class="linenos">357</span></a>                    <span class="n">row</span>
-</span><span id="DataBased-358"><a href="#DataBased-358"><span class="linenos">358</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DataBased-359"><a href="#DataBased-359"><span class="linenos">359</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="DataBased-360"><a href="#DataBased-360"><span class="linenos">360</span></a>                    <span class="p">)</span>
-</span><span id="DataBased-361"><a href="#DataBased-361"><span class="linenos">361</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="DataBased-362"><a href="#DataBased-362"><span class="linenos">362</span></a>                <span class="p">]</span>
-</span><span id="DataBased-363"><a href="#DataBased-363"><span class="linenos">363</span></a>            <span class="p">)</span>
-</span><span id="DataBased-364"><a href="#DataBased-364"><span class="linenos">364</span></a>        <span class="k">return</span> <span class="n">results</span>
-</span><span id="DataBased-365"><a href="#DataBased-365"><span class="linenos">365</span></a>
-</span><span id="DataBased-366"><a href="#DataBased-366"><span class="linenos">366</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-367"><a href="#DataBased-367"><span class="linenos">367</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="DataBased-368"><a href="#DataBased-368"><span class="linenos">368</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-369"><a href="#DataBased-369"><span class="linenos">369</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-370"><a href="#DataBased-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
-</span><span id="DataBased-371"><a href="#DataBased-371"><span class="linenos">371</span></a>
-</span><span id="DataBased-372"><a href="#DataBased-372"><span class="linenos">372</span></a><span class="sd">        Returns number of deleted records.</span>
-</span><span id="DataBased-373"><a href="#DataBased-373"><span class="linenos">373</span></a>
-</span><span id="DataBased-374"><a href="#DataBased-374"><span class="linenos">374</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-375"><a href="#DataBased-375"><span class="linenos">375</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-376"><a href="#DataBased-376"><span class="linenos">376</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-377"><a href="#DataBased-377"><span class="linenos">377</span></a>
-</span><span id="DataBased-378"><a href="#DataBased-378"><span class="linenos">378</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased-379"><a href="#DataBased-379"><span class="linenos">379</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased-380"><a href="#DataBased-380"><span class="linenos">380</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-381"><a href="#DataBased-381"><span class="linenos">381</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased-382"><a href="#DataBased-382"><span class="linenos">382</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased-383"><a href="#DataBased-383"><span class="linenos">383</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-384"><a href="#DataBased-384"><span class="linenos">384</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-385"><a href="#DataBased-385"><span class="linenos">385</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-386"><a href="#DataBased-386"><span class="linenos">386</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="DataBased-387"><a href="#DataBased-387"><span class="linenos">387</span></a>            <span class="p">)</span>
-</span><span id="DataBased-388"><a href="#DataBased-388"><span class="linenos">388</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
-</span><span id="DataBased-389"><a href="#DataBased-389"><span class="linenos">389</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-390"><a href="#DataBased-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="DataBased-391"><a href="#DataBased-391"><span class="linenos">391</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-392"><a href="#DataBased-392"><span class="linenos">392</span></a>
-</span><span id="DataBased-393"><a href="#DataBased-393"><span class="linenos">393</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-394"><a href="#DataBased-394"><span class="linenos">394</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="DataBased-395"><a href="#DataBased-395"><span class="linenos">395</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-396"><a href="#DataBased-396"><span class="linenos">396</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-397"><a href="#DataBased-397"><span class="linenos">397</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-398"><a href="#DataBased-398"><span class="linenos">398</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="DataBased-399"><a href="#DataBased-399"><span class="linenos">399</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-400"><a href="#DataBased-400"><span class="linenos">400</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased-401"><a href="#DataBased-401"><span class="linenos">401</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
-</span><span id="DataBased-402"><a href="#DataBased-402"><span class="linenos">402</span></a>
-</span><span id="DataBased-403"><a href="#DataBased-403"><span class="linenos">403</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
-</span><span id="DataBased-404"><a href="#DataBased-404"><span class="linenos">404</span></a>
-</span><span id="DataBased-405"><a href="#DataBased-405"><span class="linenos">405</span></a><span class="sd">        :param new_value: The new value to insert.</span>
-</span><span id="DataBased-406"><a href="#DataBased-406"><span class="linenos">406</span></a>
-</span><span id="DataBased-407"><a href="#DataBased-407"><span class="linenos">407</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-408"><a href="#DataBased-408"><span class="linenos">408</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a><span class="sd">        If None, every row will be updated.</span>
+</span><span id="DataBased-305"><a href="#DataBased-305"><span class="linenos">305</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
+</span><span id="DataBased-306"><a href="#DataBased-306"><span class="linenos">306</span></a>
+</span><span id="DataBased-307"><a href="#DataBased-307"><span class="linenos">307</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="DataBased-308"><a href="#DataBased-308"><span class="linenos">308</span></a>
+</span><span id="DataBased-309"><a href="#DataBased-309"><span class="linenos">309</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="DataBased-310"><a href="#DataBased-310"><span class="linenos">310</span></a>
+</span><span id="DataBased-311"><a href="#DataBased-311"><span class="linenos">311</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
+</span><span id="DataBased-312"><a href="#DataBased-312"><span class="linenos">312</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-313"><a href="#DataBased-313"><span class="linenos">313</span></a>
+</span><span id="DataBased-314"><a href="#DataBased-314"><span class="linenos">314</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-315"><a href="#DataBased-315"><span class="linenos">315</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="DataBased-316"><a href="#DataBased-316"><span class="linenos">316</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-317"><a href="#DataBased-317"><span class="linenos">317</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased-318"><a href="#DataBased-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-319"><a href="#DataBased-319"><span class="linenos">319</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-320"><a href="#DataBased-320"><span class="linenos">320</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="DataBased-321"><a href="#DataBased-321"><span class="linenos">321</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-322"><a href="#DataBased-322"><span class="linenos">322</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="DataBased-323"><a href="#DataBased-323"><span class="linenos">323</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-324"><a href="#DataBased-324"><span class="linenos">324</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased-325"><a href="#DataBased-325"><span class="linenos">325</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased-326"><a href="#DataBased-326"><span class="linenos">326</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased-327"><a href="#DataBased-327"><span class="linenos">327</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="DataBased-328"><a href="#DataBased-328"><span class="linenos">328</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="DataBased-329"><a href="#DataBased-329"><span class="linenos">329</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="DataBased-330"><a href="#DataBased-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="DataBased-331"><a href="#DataBased-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="DataBased-332"><a href="#DataBased-332"><span class="linenos">332</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="DataBased-333"><a href="#DataBased-333"><span class="linenos">333</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DataBased-334"><a href="#DataBased-334"><span class="linenos">334</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-335"><a href="#DataBased-335"><span class="linenos">335</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-336"><a href="#DataBased-336"><span class="linenos">336</span></a>
+</span><span id="DataBased-337"><a href="#DataBased-337"><span class="linenos">337</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-338"><a href="#DataBased-338"><span class="linenos">338</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
+</span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a>
+</span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a>
+</span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a>
+</span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a>
+</span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
+</span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="DataBased-354"><a href="#DataBased-354"><span class="linenos">354</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased-355"><a href="#DataBased-355"><span class="linenos">355</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-356"><a href="#DataBased-356"><span class="linenos">356</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DataBased-357"><a href="#DataBased-357"><span class="linenos">357</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-358"><a href="#DataBased-358"><span class="linenos">358</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="DataBased-359"><a href="#DataBased-359"><span class="linenos">359</span></a>                <span class="p">[</span>
+</span><span id="DataBased-360"><a href="#DataBased-360"><span class="linenos">360</span></a>                    <span class="n">row</span>
+</span><span id="DataBased-361"><a href="#DataBased-361"><span class="linenos">361</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DataBased-362"><a href="#DataBased-362"><span class="linenos">362</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="DataBased-363"><a href="#DataBased-363"><span class="linenos">363</span></a>                    <span class="p">)</span>
+</span><span id="DataBased-364"><a href="#DataBased-364"><span class="linenos">364</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="DataBased-365"><a href="#DataBased-365"><span class="linenos">365</span></a>                <span class="p">]</span>
+</span><span id="DataBased-366"><a href="#DataBased-366"><span class="linenos">366</span></a>            <span class="p">)</span>
+</span><span id="DataBased-367"><a href="#DataBased-367"><span class="linenos">367</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-368"><a href="#DataBased-368"><span class="linenos">368</span></a>
+</span><span id="DataBased-369"><a href="#DataBased-369"><span class="linenos">369</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-370"><a href="#DataBased-370"><span class="linenos">370</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="DataBased-371"><a href="#DataBased-371"><span class="linenos">371</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-372"><a href="#DataBased-372"><span class="linenos">372</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-373"><a href="#DataBased-373"><span class="linenos">373</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
+</span><span id="DataBased-374"><a href="#DataBased-374"><span class="linenos">374</span></a>
+</span><span id="DataBased-375"><a href="#DataBased-375"><span class="linenos">375</span></a><span class="sd">        Returns the number of deleted records.</span>
+</span><span id="DataBased-376"><a href="#DataBased-376"><span class="linenos">376</span></a>
+</span><span id="DataBased-377"><a href="#DataBased-377"><span class="linenos">377</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-378"><a href="#DataBased-378"><span class="linenos">378</span></a>
+</span><span id="DataBased-379"><a href="#DataBased-379"><span class="linenos">379</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
+</span><span id="DataBased-380"><a href="#DataBased-380"><span class="linenos">380</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased-381"><a href="#DataBased-381"><span class="linenos">381</span></a>
+</span><span id="DataBased-382"><a href="#DataBased-382"><span class="linenos">382</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
+</span><span id="DataBased-383"><a href="#DataBased-383"><span class="linenos">383</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-384"><a href="#DataBased-384"><span class="linenos">384</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased-385"><a href="#DataBased-385"><span class="linenos">385</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased-386"><a href="#DataBased-386"><span class="linenos">386</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-387"><a href="#DataBased-387"><span class="linenos">387</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-388"><a href="#DataBased-388"><span class="linenos">388</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-389"><a href="#DataBased-389"><span class="linenos">389</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="DataBased-390"><a href="#DataBased-390"><span class="linenos">390</span></a>            <span class="p">)</span>
+</span><span id="DataBased-391"><a href="#DataBased-391"><span class="linenos">391</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
+</span><span id="DataBased-392"><a href="#DataBased-392"><span class="linenos">392</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-393"><a href="#DataBased-393"><span class="linenos">393</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="DataBased-394"><a href="#DataBased-394"><span class="linenos">394</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased-395"><a href="#DataBased-395"><span class="linenos">395</span></a>
+</span><span id="DataBased-396"><a href="#DataBased-396"><span class="linenos">396</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-397"><a href="#DataBased-397"><span class="linenos">397</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="DataBased-398"><a href="#DataBased-398"><span class="linenos">398</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-399"><a href="#DataBased-399"><span class="linenos">399</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-400"><a href="#DataBased-400"><span class="linenos">400</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-401"><a href="#DataBased-401"><span class="linenos">401</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="DataBased-402"><a href="#DataBased-402"><span class="linenos">402</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-403"><a href="#DataBased-403"><span class="linenos">403</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased-404"><a href="#DataBased-404"><span class="linenos">404</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
+</span><span id="DataBased-405"><a href="#DataBased-405"><span class="linenos">405</span></a>
+</span><span id="DataBased-406"><a href="#DataBased-406"><span class="linenos">406</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-407"><a href="#DataBased-407"><span class="linenos">407</span></a>
+</span><span id="DataBased-408"><a href="#DataBased-408"><span class="linenos">408</span></a><span class="sd">        `table`: The table to update rows in.</span>
+</span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a>
+</span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
 </span><span id="DataBased-411"><a href="#DataBased-411"><span class="linenos">411</span></a>
-</span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="DataBased-414"><a href="#DataBased-414"><span class="linenos">414</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
-</span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a>                <span class="p">)</span>
-</span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>                <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
-</span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-424"><a href="#DataBased-424"><span class="linenos">424</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-425"><a href="#DataBased-425"><span class="linenos">425</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-426"><a href="#DataBased-426"><span class="linenos">426</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-427"><a href="#DataBased-427"><span class="linenos">427</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="DataBased-428"><a href="#DataBased-428"><span class="linenos">428</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="DataBased-429"><a href="#DataBased-429"><span class="linenos">429</span></a>            <span class="p">)</span>
-</span><span id="DataBased-430"><a href="#DataBased-430"><span class="linenos">430</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-431"><a href="#DataBased-431"><span class="linenos">431</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased-432"><a href="#DataBased-432"><span class="linenos">432</span></a>            <span class="p">)</span>
-</span><span id="DataBased-433"><a href="#DataBased-433"><span class="linenos">433</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased-434"><a href="#DataBased-434"><span class="linenos">434</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-435"><a href="#DataBased-435"><span class="linenos">435</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased-436"><a href="#DataBased-436"><span class="linenos">436</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased-437"><a href="#DataBased-437"><span class="linenos">437</span></a>            <span class="p">)</span>
-</span><span id="DataBased-438"><a href="#DataBased-438"><span class="linenos">438</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-439"><a href="#DataBased-439"><span class="linenos">439</span></a>
-</span><span id="DataBased-440"><a href="#DataBased-440"><span class="linenos">440</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-441"><a href="#DataBased-441"><span class="linenos">441</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased-442"><a href="#DataBased-442"><span class="linenos">442</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
-</span><span id="DataBased-443"><a href="#DataBased-443"><span class="linenos">443</span></a>
-</span><span id="DataBased-444"><a href="#DataBased-444"><span class="linenos">444</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased-445"><a href="#DataBased-445"><span class="linenos">445</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-446"><a href="#DataBased-446"><span class="linenos">446</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a>
-</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a>    <span class="p">):</span>
-</span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
-</span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>
-</span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a><span class="sd">        :param column: Name of the column to add.</span>
-</span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>
-</span><span id="DataBased-462"><a href="#DataBased-462"><span class="linenos">462</span></a><span class="sd">        :param _type: The data type of the new column.</span>
-</span><span id="DataBased-463"><a href="#DataBased-463"><span class="linenos">463</span></a>
-</span><span id="DataBased-464"><a href="#DataBased-464"><span class="linenos">464</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="DataBased-465"><a href="#DataBased-465"><span class="linenos">465</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-466"><a href="#DataBased-466"><span class="linenos">466</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="DataBased-467"><a href="#DataBased-467"><span class="linenos">467</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-468"><a href="#DataBased-468"><span class="linenos">468</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-469"><a href="#DataBased-469"><span class="linenos">469</span></a>                <span class="p">)</span>
-</span><span id="DataBased-470"><a href="#DataBased-470"><span class="linenos">470</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-471"><a href="#DataBased-471"><span class="linenos">471</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-472"><a href="#DataBased-472"><span class="linenos">472</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-473"><a href="#DataBased-473"><span class="linenos">473</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-474"><a href="#DataBased-474"><span class="linenos">474</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-475"><a href="#DataBased-475"><span class="linenos">475</span></a>
-</span><span id="DataBased-476"><a href="#DataBased-476"><span class="linenos">476</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-480"><a href="#DataBased-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
-</span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a><span class="sd">        from a list of dictionaries.</span>
-</span><span id="DataBased-482"><a href="#DataBased-482"><span class="linenos">482</span></a>
-</span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>
-</span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="DataBased-486"><a href="#DataBased-486"><span class="linenos">486</span></a>
-</span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
-</span><span id="DataBased-488"><a href="#DataBased-488"><span class="linenos">488</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
-</span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
-</span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a><span class="sd">        `new_value`: The new value to insert.</span>
+</span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a>
+</span><span id="DataBased-414"><a href="#DataBased-414"><span class="linenos">414</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
+</span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a>
+</span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-424"><a href="#DataBased-424"><span class="linenos">424</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
+</span><span id="DataBased-425"><a href="#DataBased-425"><span class="linenos">425</span></a>                <span class="p">)</span>
+</span><span id="DataBased-426"><a href="#DataBased-426"><span class="linenos">426</span></a>                <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-427"><a href="#DataBased-427"><span class="linenos">427</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
+</span><span id="DataBased-428"><a href="#DataBased-428"><span class="linenos">428</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-429"><a href="#DataBased-429"><span class="linenos">429</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-430"><a href="#DataBased-430"><span class="linenos">430</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-431"><a href="#DataBased-431"><span class="linenos">431</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased-432"><a href="#DataBased-432"><span class="linenos">432</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-433"><a href="#DataBased-433"><span class="linenos">433</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-434"><a href="#DataBased-434"><span class="linenos">434</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="DataBased-435"><a href="#DataBased-435"><span class="linenos">435</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
+</span><span id="DataBased-436"><a href="#DataBased-436"><span class="linenos">436</span></a>            <span class="p">)</span>
+</span><span id="DataBased-437"><a href="#DataBased-437"><span class="linenos">437</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-438"><a href="#DataBased-438"><span class="linenos">438</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-439"><a href="#DataBased-439"><span class="linenos">439</span></a>            <span class="p">)</span>
+</span><span id="DataBased-440"><a href="#DataBased-440"><span class="linenos">440</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased-441"><a href="#DataBased-441"><span class="linenos">441</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-442"><a href="#DataBased-442"><span class="linenos">442</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="DataBased-443"><a href="#DataBased-443"><span class="linenos">443</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-444"><a href="#DataBased-444"><span class="linenos">444</span></a>            <span class="p">)</span>
+</span><span id="DataBased-445"><a href="#DataBased-445"><span class="linenos">445</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-446"><a href="#DataBased-446"><span class="linenos">446</span></a>
+</span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a>
+</span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a>
+</span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-462"><a href="#DataBased-462"><span class="linenos">462</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="DataBased-463"><a href="#DataBased-463"><span class="linenos">463</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-464"><a href="#DataBased-464"><span class="linenos">464</span></a>    <span class="p">):</span>
+</span><span id="DataBased-465"><a href="#DataBased-465"><span class="linenos">465</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
+</span><span id="DataBased-466"><a href="#DataBased-466"><span class="linenos">466</span></a>
+</span><span id="DataBased-467"><a href="#DataBased-467"><span class="linenos">467</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-468"><a href="#DataBased-468"><span class="linenos">468</span></a>
+</span><span id="DataBased-469"><a href="#DataBased-469"><span class="linenos">469</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="DataBased-470"><a href="#DataBased-470"><span class="linenos">470</span></a>
+</span><span id="DataBased-471"><a href="#DataBased-471"><span class="linenos">471</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="DataBased-472"><a href="#DataBased-472"><span class="linenos">472</span></a>
+</span><span id="DataBased-473"><a href="#DataBased-473"><span class="linenos">473</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="DataBased-474"><a href="#DataBased-474"><span class="linenos">474</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-475"><a href="#DataBased-475"><span class="linenos">475</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="DataBased-476"><a href="#DataBased-476"><span class="linenos">476</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>                <span class="p">)</span>
+</span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
+</span><span id="DataBased-480"><a href="#DataBased-480"><span class="linenos">480</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-482"><a href="#DataBased-482"><span class="linenos">482</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a>
+</span><span id="DataBased-486"><a href="#DataBased-486"><span class="linenos">486</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased-488"><a href="#DataBased-488"><span class="linenos">488</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="DataBased-491"><a href="#DataBased-491"><span class="linenos">491</span></a>
+</span><span id="DataBased-492"><a href="#DataBased-492"><span class="linenos">492</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-493"><a href="#DataBased-493"><span class="linenos">493</span></a>
+</span><span id="DataBased-494"><a href="#DataBased-494"><span class="linenos">494</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="DataBased-495"><a href="#DataBased-495"><span class="linenos">495</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="DataBased-496"><a href="#DataBased-496"><span class="linenos">496</span></a>
+</span><span id="DataBased-497"><a href="#DataBased-497"><span class="linenos">497</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased-498"><a href="#DataBased-498"><span class="linenos">498</span></a>
+</span><span id="DataBased-499"><a href="#DataBased-499"><span class="linenos">499</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="DataBased-500"><a href="#DataBased-500"><span class="linenos">500</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="DataBased-501"><a href="#DataBased-501"><span class="linenos">501</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sqli wrapper so queries don't need to be written except table definitions.</p>
 
 <p>Supports saving and reading dates as datetime objects.</p>
 
@@ -1169,41 +1193,40 @@
             <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.__init__-34"><a href="#DataBased.__init__-34"><span class="linenos">34</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
 </span><span id="DataBased.__init__-35"><a href="#DataBased.__init__-35"><span class="linenos">35</span></a>        <span class="bp">self</span><span class="p">,</span>
 </span><span id="DataBased.__init__-36"><a href="#DataBased.__init__-36"><span class="linenos">36</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">,</span>
 </span><span id="DataBased.__init__-37"><a href="#DataBased.__init__-37"><span class="linenos">37</span></a>        <span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
 </span><span id="DataBased.__init__-38"><a href="#DataBased.__init__-38"><span class="linenos">38</span></a>        <span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
 </span><span id="DataBased.__init__-39"><a href="#DataBased.__init__-39"><span class="linenos">39</span></a>    <span class="p">):</span>
 </span><span id="DataBased.__init__-40"><a href="#DataBased.__init__-40"><span class="linenos">40</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="DataBased.__init__-41"><a href="#DataBased.__init__-41"><span class="linenos">41</span></a><span class="sd">        :param dbpath: String or Path object to database file.</span>
-</span><span id="DataBased.__init__-42"><a href="#DataBased.__init__-42"><span class="linenos">42</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
-</span><span id="DataBased.__init__-43"><a href="#DataBased.__init__-43"><span class="linenos">43</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
-</span><span id="DataBased.__init__-44"><a href="#DataBased.__init__-44"><span class="linenos">44</span></a><span class="sd">        same directory.</span>
-</span><span id="DataBased.__init__-45"><a href="#DataBased.__init__-45"><span class="linenos">45</span></a>
-</span><span id="DataBased.__init__-46"><a href="#DataBased.__init__-46"><span class="linenos">46</span></a><span class="sd">        :param logger_message_format: &#39;{&#39; style format string</span>
-</span><span id="DataBased.__init__-47"><a href="#DataBased.__init__-47"><span class="linenos">47</span></a><span class="sd">        for the logger object.&quot;&quot;&quot;</span>
-</span><span id="DataBased.__init__-48"><a href="#DataBased.__init__-48"><span class="linenos">48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DataBased.__init__-49"><a href="#DataBased.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
-</span><span id="DataBased.__init__-50"><a href="#DataBased.__init__-50"><span class="linenos">50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="DataBased.__init__-51"><a href="#DataBased.__init__-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
-</span><span id="DataBased.__init__-52"><a href="#DataBased.__init__-52"><span class="linenos">52</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
-</span><span id="DataBased.__init__-53"><a href="#DataBased.__init__-53"><span class="linenos">53</span></a>        <span class="p">)</span>
-</span><span id="DataBased.__init__-54"><a href="#DataBased.__init__-54"><span class="linenos">54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="DataBased.__init__-41"><a href="#DataBased.__init__-41"><span class="linenos">41</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.__init__-42"><a href="#DataBased.__init__-42"><span class="linenos">42</span></a>
+</span><span id="DataBased.__init__-43"><a href="#DataBased.__init__-43"><span class="linenos">43</span></a><span class="sd">        `dbpath`: String or Path object to database file.</span>
+</span><span id="DataBased.__init__-44"><a href="#DataBased.__init__-44"><span class="linenos">44</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
+</span><span id="DataBased.__init__-45"><a href="#DataBased.__init__-45"><span class="linenos">45</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
+</span><span id="DataBased.__init__-46"><a href="#DataBased.__init__-46"><span class="linenos">46</span></a><span class="sd">        same directory.</span>
+</span><span id="DataBased.__init__-47"><a href="#DataBased.__init__-47"><span class="linenos">47</span></a>
+</span><span id="DataBased.__init__-48"><a href="#DataBased.__init__-48"><span class="linenos">48</span></a><span class="sd">        `logger_message_format`: &#39;{&#39; style format string for the logger object.&quot;&quot;&quot;</span>
+</span><span id="DataBased.__init__-49"><a href="#DataBased.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DataBased.__init__-50"><a href="#DataBased.__init__-50"><span class="linenos">50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
+</span><span id="DataBased.__init__-51"><a href="#DataBased.__init__-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="DataBased.__init__-52"><a href="#DataBased.__init__-52"><span class="linenos">52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
+</span><span id="DataBased.__init__-53"><a href="#DataBased.__init__-53"><span class="linenos">53</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
+</span><span id="DataBased.__init__-54"><a href="#DataBased.__init__-54"><span class="linenos">54</span></a>        <span class="p">)</span>
+</span><span id="DataBased.__init__-55"><a href="#DataBased.__init__-55"><span class="linenos">55</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
 </span></pre></div>
 
 
-            <div class="docstring"><h6 id="parameters">Parameters</h6>
+            <div class="docstring"><h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>dbpath</strong>:  String or Path object to database file.
+<p><code>dbpath</code>: String or Path object to database file.
 If a relative path is given, it will be relative to the
 current working directory. The log file will be saved to the
-same directory.</p></li>
-<li><p><strong>logger_message_format</strong>:  '{' style format string
-for the logger object.</p></li>
-</ul>
+same directory.</p>
+
+<p><code>logger_message_format</code>: '{' style format string for the logger object.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.open" class="classattr">
                                         <input id="DataBased.open-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1211,24 +1234,24 @@
         <span class="def">def</span>
         <span class="name">open</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.open-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.open"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.open-63"><a href="#DataBased.open-63"><span class="linenos">63</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased.open-64"><a href="#DataBased.open-64"><span class="linenos">64</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
-</span><span id="DataBased.open-65"><a href="#DataBased.open-65"><span class="linenos">65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-</span><span id="DataBased.open-66"><a href="#DataBased.open-66"><span class="linenos">66</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
-</span><span id="DataBased.open-67"><a href="#DataBased.open-67"><span class="linenos">67</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
-</span><span id="DataBased.open-68"><a href="#DataBased.open-68"><span class="linenos">68</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
-</span><span id="DataBased.open-69"><a href="#DataBased.open-69"><span class="linenos">69</span></a>        <span class="p">)</span>
-</span><span id="DataBased.open-70"><a href="#DataBased.open-70"><span class="linenos">70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
-</span><span id="DataBased.open-71"><a href="#DataBased.open-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
-</span><span id="DataBased.open-72"><a href="#DataBased.open-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.open-64"><a href="#DataBased.open-64"><span class="linenos">64</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased.open-65"><a href="#DataBased.open-65"><span class="linenos">65</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
+</span><span id="DataBased.open-66"><a href="#DataBased.open-66"><span class="linenos">66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
+</span><span id="DataBased.open-67"><a href="#DataBased.open-67"><span class="linenos">67</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
+</span><span id="DataBased.open-68"><a href="#DataBased.open-68"><span class="linenos">68</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
+</span><span id="DataBased.open-69"><a href="#DataBased.open-69"><span class="linenos">69</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
+</span><span id="DataBased.open-70"><a href="#DataBased.open-70"><span class="linenos">70</span></a>        <span class="p">)</span>
+</span><span id="DataBased.open-71"><a href="#DataBased.open-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.open-72"><a href="#DataBased.open-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
+</span><span id="DataBased.open-73"><a href="#DataBased.open-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Open connection to db.</p>
 </div>
 
 
@@ -1240,23 +1263,23 @@
         <span class="def">def</span>
         <span class="name">close</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.close-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.close"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.close-74"><a href="#DataBased.close-74"><span class="linenos">74</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased.close-75"><a href="#DataBased.close-75"><span class="linenos">75</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
-</span><span id="DataBased.close-76"><a href="#DataBased.close-76"><span class="linenos">76</span></a>
-</span><span id="DataBased.close-77"><a href="#DataBased.close-77"><span class="linenos">77</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
-</span><span id="DataBased.close-78"><a href="#DataBased.close-78"><span class="linenos">78</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
-</span><span id="DataBased.close-79"><a href="#DataBased.close-79"><span class="linenos">79</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
-</span><span id="DataBased.close-80"><a href="#DataBased.close-80"><span class="linenos">80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
-</span><span id="DataBased.close-81"><a href="#DataBased.close-81"><span class="linenos">81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DataBased.close-82"><a href="#DataBased.close-82"><span class="linenos">82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.close-75"><a href="#DataBased.close-75"><span class="linenos">75</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased.close-76"><a href="#DataBased.close-76"><span class="linenos">76</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
+</span><span id="DataBased.close-77"><a href="#DataBased.close-77"><span class="linenos">77</span></a>
+</span><span id="DataBased.close-78"><a href="#DataBased.close-78"><span class="linenos">78</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
+</span><span id="DataBased.close-79"><a href="#DataBased.close-79"><span class="linenos">79</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
+</span><span id="DataBased.close-80"><a href="#DataBased.close-80"><span class="linenos">80</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
+</span><span id="DataBased.close-81"><a href="#DataBased.close-81"><span class="linenos">81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
+</span><span id="DataBased.close-82"><a href="#DataBased.close-82"><span class="linenos">82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DataBased.close-83"><a href="#DataBased.close-83"><span class="linenos">83</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Save and close connection to db.</p>
 
 <p>Call this as soon as you are done using the database if you have
 multiple threads or processes using the same database.</p>
@@ -1271,62 +1294,58 @@
         <span class="def">def</span>
         <span class="name">query</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">query_</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.query-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.query"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.query-151"><a href="#DataBased.query-151"><span class="linenos">151</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.query-152"><a href="#DataBased.query-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="DataBased.query-153"><a href="#DataBased.query-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
-</span><span id="DataBased.query-154"><a href="#DataBased.query-154"><span class="linenos">154</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
-</span><span id="DataBased.query-155"><a href="#DataBased.query-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="DataBased.query-156"><a href="#DataBased.query-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.query-156"><a href="#DataBased.query-156"><span class="linenos">156</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.query-157"><a href="#DataBased.query-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="DataBased.query-158"><a href="#DataBased.query-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
+</span><span id="DataBased.query-159"><a href="#DataBased.query-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="DataBased.query-160"><a href="#DataBased.query-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Execute an arbitrary query and
-return the results.</p>
+            <div class="docstring"><p>Execute an arbitrary query and return the results.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.create_tables" class="classattr">
                                         <input id="DataBased.create_tables-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_tables</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_tables</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.create_tables-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.create_tables"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_tables-158"><a href="#DataBased.create_tables-158"><span class="linenos">158</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.create_tables-159"><a href="#DataBased.create_tables-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="DataBased.create_tables-160"><a href="#DataBased.create_tables-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
-</span><span id="DataBased.create_tables-161"><a href="#DataBased.create_tables-161"><span class="linenos">161</span></a>
-</span><span id="DataBased.create_tables-162"><a href="#DataBased.create_tables-162"><span class="linenos">162</span></a><span class="sd">        :param table_querys: Each query should be</span>
-</span><span id="DataBased.create_tables-163"><a href="#DataBased.create_tables-163"><span class="linenos">163</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_tables-164"><a href="#DataBased.create_tables-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-165"><a href="#DataBased.create_tables-165"><span class="linenos">165</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DataBased.create_tables-166"><a href="#DataBased.create_tables-166"><span class="linenos">166</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-167"><a href="#DataBased.create_tables-167"><span class="linenos">167</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-168"><a href="#DataBased.create_tables-168"><span class="linenos">168</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.create_tables-169"><a href="#DataBased.create_tables-169"><span class="linenos">169</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_tables-162"><a href="#DataBased.create_tables-162"><span class="linenos">162</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.create_tables-163"><a href="#DataBased.create_tables-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="DataBased.create_tables-164"><a href="#DataBased.create_tables-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased.create_tables-165"><a href="#DataBased.create_tables-165"><span class="linenos">165</span></a>
+</span><span id="DataBased.create_tables-166"><a href="#DataBased.create_tables-166"><span class="linenos">166</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
+</span><span id="DataBased.create_tables-167"><a href="#DataBased.create_tables-167"><span class="linenos">167</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-168"><a href="#DataBased.create_tables-168"><span class="linenos">168</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DataBased.create_tables-169"><a href="#DataBased.create_tables-169"><span class="linenos">169</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-170"><a href="#DataBased.create_tables-170"><span class="linenos">170</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-171"><a href="#DataBased.create_tables-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.create_tables-172"><a href="#DataBased.create_tables-172"><span class="linenos">172</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create tables if they don't exist.</p>
 
 <h6 id="parameters">Parameters</h6>
 
 <ul>
-<li><strong>table_querys</strong>:  Each query should be
-in the form 'tableName(columnDefinitions)'</li>
+<li><strong><code>table_defs</code></strong>:  Each definition should be in the form <code>table_name(column_definitions)</code></li>
 </ul>
 </div>
 
 
                             </div>
                             <div id="DataBased.create_table" class="classattr">
                                         <input id="DataBased.create_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -1335,40 +1354,39 @@
         <span class="def">def</span>
         <span class="name">create_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.create_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.create_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_table-171"><a href="#DataBased.create_table-171"><span class="linenos">171</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.create_table-172"><a href="#DataBased.create_table-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="DataBased.create_table-173"><a href="#DataBased.create_table-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="DataBased.create_table-174"><a href="#DataBased.create_table-174"><span class="linenos">174</span></a>
-</span><span id="DataBased.create_table-175"><a href="#DataBased.create_table-175"><span class="linenos">175</span></a><span class="sd">        :param table: Name of the table to create.</span>
-</span><span id="DataBased.create_table-176"><a href="#DataBased.create_table-176"><span class="linenos">176</span></a>
-</span><span id="DataBased.create_table-177"><a href="#DataBased.create_table-177"><span class="linenos">177</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
-</span><span id="DataBased.create_table-178"><a href="#DataBased.create_table-178"><span class="linenos">178</span></a><span class="sd">        proper Sqlite3 sytax.</span>
-</span><span id="DataBased.create_table-179"><a href="#DataBased.create_table-179"><span class="linenos">179</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_table-180"><a href="#DataBased.create_table-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased.create_table-181"><a href="#DataBased.create_table-181"><span class="linenos">181</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="DataBased.create_table-182"><a href="#DataBased.create_table-182"><span class="linenos">182</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased.create_table-183"><a href="#DataBased.create_table-183"><span class="linenos">183</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_table-174"><a href="#DataBased.create_table-174"><span class="linenos">174</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.create_table-175"><a href="#DataBased.create_table-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="DataBased.create_table-176"><a href="#DataBased.create_table-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="DataBased.create_table-177"><a href="#DataBased.create_table-177"><span class="linenos">177</span></a>
+</span><span id="DataBased.create_table-178"><a href="#DataBased.create_table-178"><span class="linenos">178</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.create_table-179"><a href="#DataBased.create_table-179"><span class="linenos">179</span></a>
+</span><span id="DataBased.create_table-180"><a href="#DataBased.create_table-180"><span class="linenos">180</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="DataBased.create_table-181"><a href="#DataBased.create_table-181"><span class="linenos">181</span></a>
+</span><span id="DataBased.create_table-182"><a href="#DataBased.create_table-182"><span class="linenos">182</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
+</span><span id="DataBased.create_table-183"><a href="#DataBased.create_table-183"><span class="linenos">183</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
+</span><span id="DataBased.create_table-184"><a href="#DataBased.create_table-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="DataBased.create_table-185"><a href="#DataBased.create_table-185"><span class="linenos">185</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="DataBased.create_table-186"><a href="#DataBased.create_table-186"><span class="linenos">186</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased.create_table-187"><a href="#DataBased.create_table-187"><span class="linenos">187</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a table if it doesn't exist.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>table</strong>:  Name of the table to create.</p></li>
-<li><p><strong>column_defs</strong>:  List of column definitions in
-proper Sqlite3 sytax.
-i.e. "columnName text unique" or "columnName int primary key" etc.</p></li>
-</ul>
+<p><code>table</code>: Name of the table to create.</p>
+
+<p><code>column_defs</code>: List of column definitions in proper Sqlite3 sytax.
+i.e. <code>"column_name text unique"</code> or <code>"column_name int primary key"</code> etc.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.get_table_names" class="classattr">
                                         <input id="DataBased.get_table_names-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1376,25 +1394,25 @@
         <span class="def">def</span>
         <span class="name">get_table_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_table_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_table_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_table_names-185"><a href="#DataBased.get_table_names-185"><span class="linenos">185</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_table_names-186"><a href="#DataBased.get_table_names-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased.get_table_names-187"><a href="#DataBased.get_table_names-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_table_names-188"><a href="#DataBased.get_table_names-188"><span class="linenos">188</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.get_table_names-189"><a href="#DataBased.get_table_names-189"><span class="linenos">189</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
-</span><span id="DataBased.get_table_names-190"><a href="#DataBased.get_table_names-190"><span class="linenos">190</span></a>        <span class="p">)</span>
-</span><span id="DataBased.get_table_names-191"><a href="#DataBased.get_table_names-191"><span class="linenos">191</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_table_names-189"><a href="#DataBased.get_table_names-189"><span class="linenos">189</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_table_names-190"><a href="#DataBased.get_table_names-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased.get_table_names-191"><a href="#DataBased.get_table_names-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
+</span><span id="DataBased.get_table_names-192"><a href="#DataBased.get_table_names-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.get_table_names-193"><a href="#DataBased.get_table_names-193"><span class="linenos">193</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
+</span><span id="DataBased.get_table_names-194"><a href="#DataBased.get_table_names-194"><span class="linenos">194</span></a>        <span class="p">)</span>
+</span><span id="DataBased.get_table_names-195"><a href="#DataBased.get_table_names-195"><span class="linenos">195</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns a list of table names from database.</p>
+            <div class="docstring"><p>Returns a list of table names from the database.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.get_column_names" class="classattr">
                                         <input id="DataBased.get_column_names-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1402,19 +1420,19 @@
         <span class="def">def</span>
         <span class="name">get_column_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_column_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_column_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-193"><a href="#DataBased.get_column_names-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_column_names-194"><a href="#DataBased.get_column_names-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased.get_column_names-195"><a href="#DataBased.get_column_names-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_column_names-196"><a href="#DataBased.get_column_names-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
-</span><span id="DataBased.get_column_names-197"><a href="#DataBased.get_column_names-197"><span class="linenos">197</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-197"><a href="#DataBased.get_column_names-197"><span class="linenos">197</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_column_names-198"><a href="#DataBased.get_column_names-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased.get_column_names-199"><a href="#DataBased.get_column_names-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="DataBased.get_column_names-200"><a href="#DataBased.get_column_names-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="DataBased.get_column_names-201"><a href="#DataBased.get_column_names-201"><span class="linenos">201</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a list of column names from a table.</p>
 </div>
 
 
@@ -1426,59 +1444,60 @@
         <span class="def">def</span>
         <span class="name">count</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.count-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.count"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.count-199"><a href="#DataBased.count-199"><span class="linenos">199</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.count-200"><a href="#DataBased.count-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="DataBased.count-201"><a href="#DataBased.count-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.count-202"><a href="#DataBased.count-202"><span class="linenos">202</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.count-203"><a href="#DataBased.count-203"><span class="linenos">203</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.count-204"><a href="#DataBased.count-204"><span class="linenos">204</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.count-205"><a href="#DataBased.count-205"><span class="linenos">205</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.count-206"><a href="#DataBased.count-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
-</span><span id="DataBased.count-207"><a href="#DataBased.count-207"><span class="linenos">207</span></a>
-</span><span id="DataBased.count-208"><a href="#DataBased.count-208"><span class="linenos">208</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.count-209"><a href="#DataBased.count-209"><span class="linenos">209</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.count-210"><a href="#DataBased.count-210"><span class="linenos">210</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.count-211"><a href="#DataBased.count-211"><span class="linenos">211</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
-</span><span id="DataBased.count-212"><a href="#DataBased.count-212"><span class="linenos">212</span></a>
-</span><span id="DataBased.count-213"><a href="#DataBased.count-213"><span class="linenos">213</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
-</span><span id="DataBased.count-214"><a href="#DataBased.count-214"><span class="linenos">214</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
-</span><span id="DataBased.count-215"><a href="#DataBased.count-215"><span class="linenos">215</span></a><span class="sd">        match_criteria is None.</span>
-</span><span id="DataBased.count-216"><a href="#DataBased.count-216"><span class="linenos">216</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.count-217"><a href="#DataBased.count-217"><span class="linenos">217</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.count-218"><a href="#DataBased.count-218"><span class="linenos">218</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.count-219"><a href="#DataBased.count-219"><span class="linenos">219</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.count-220"><a href="#DataBased.count-220"><span class="linenos">220</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.count-221"><a href="#DataBased.count-221"><span class="linenos">221</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.count-222"><a href="#DataBased.count-222"><span class="linenos">222</span></a>                <span class="p">)</span>
-</span><span id="DataBased.count-223"><a href="#DataBased.count-223"><span class="linenos">223</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.count-224"><a href="#DataBased.count-224"><span class="linenos">224</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.count-225"><a href="#DataBased.count-225"><span class="linenos">225</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DataBased.count-226"><a href="#DataBased.count-226"><span class="linenos">226</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="DataBased.count-227"><a href="#DataBased.count-227"><span class="linenos">227</span></a>            <span class="k">return</span> <span class="mi">0</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.count-203"><a href="#DataBased.count-203"><span class="linenos">203</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.count-204"><a href="#DataBased.count-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="DataBased.count-205"><a href="#DataBased.count-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.count-206"><a href="#DataBased.count-206"><span class="linenos">206</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.count-207"><a href="#DataBased.count-207"><span class="linenos">207</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.count-208"><a href="#DataBased.count-208"><span class="linenos">208</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.count-209"><a href="#DataBased.count-209"><span class="linenos">209</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.count-210"><a href="#DataBased.count-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
+</span><span id="DataBased.count-211"><a href="#DataBased.count-211"><span class="linenos">211</span></a>
+</span><span id="DataBased.count-212"><a href="#DataBased.count-212"><span class="linenos">212</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.count-213"><a href="#DataBased.count-213"><span class="linenos">213</span></a>
+</span><span id="DataBased.count-214"><a href="#DataBased.count-214"><span class="linenos">214</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.count-215"><a href="#DataBased.count-215"><span class="linenos">215</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased.count-216"><a href="#DataBased.count-216"><span class="linenos">216</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.count-217"><a href="#DataBased.count-217"><span class="linenos">217</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
+</span><span id="DataBased.count-218"><a href="#DataBased.count-218"><span class="linenos">218</span></a>
+</span><span id="DataBased.count-219"><a href="#DataBased.count-219"><span class="linenos">219</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="DataBased.count-220"><a href="#DataBased.count-220"><span class="linenos">220</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
+</span><span id="DataBased.count-221"><a href="#DataBased.count-221"><span class="linenos">221</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
+</span><span id="DataBased.count-222"><a href="#DataBased.count-222"><span class="linenos">222</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.count-223"><a href="#DataBased.count-223"><span class="linenos">223</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.count-224"><a href="#DataBased.count-224"><span class="linenos">224</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.count-225"><a href="#DataBased.count-225"><span class="linenos">225</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.count-226"><a href="#DataBased.count-226"><span class="linenos">226</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.count-227"><a href="#DataBased.count-227"><span class="linenos">227</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.count-228"><a href="#DataBased.count-228"><span class="linenos">228</span></a>                <span class="p">)</span>
+</span><span id="DataBased.count-229"><a href="#DataBased.count-229"><span class="linenos">229</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.count-230"><a href="#DataBased.count-230"><span class="linenos">230</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.count-231"><a href="#DataBased.count-231"><span class="linenos">231</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DataBased.count-232"><a href="#DataBased.count-232"><span class="linenos">232</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="DataBased.count-233"><a href="#DataBased.count-233"><span class="linenos">233</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Return number of items in table.</p>
+            <div class="docstring"><p>Return number of items in <code>table</code>.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each
-tuple is (columnName, rowValue) or a dictionary where
+<p><code>match_criteria</code>: Can be a list of 2-tuples where each
+tuple is <code>(columnName, rowValue)</code> or a dictionary where
 keys are column names and values are row values.
-If None, all rows from the table will be counted.</p></li>
-<li><p><strong>exact_match</strong>:  If False, the row value for a give column
-in match_criteria will be matched as a substring. Has no effect if
-match_criteria is None.</p></li>
-</ul>
+If <code>None</code>, all rows from the table will be counted.</p>
+
+<p><code>exact_match</code>: If <code>False</code>, the row value for a given column
+in <code>match_criteria</code> will be matched as a substring.
+Has no effect if <code>match_criteria</code> is <code>None</code>.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.add_row" class="classattr">
                                         <input id="DataBased.add_row-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1486,62 +1505,62 @@
         <span class="def">def</span>
         <span class="name">add_row</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.add_row-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_row"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_row-229"><a href="#DataBased.add_row-229"><span class="linenos">229</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_row-230"><a href="#DataBased.add_row-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
-</span><span id="DataBased.add_row-231"><a href="#DataBased.add_row-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.add_row-232"><a href="#DataBased.add_row-232"><span class="linenos">232</span></a>    <span class="p">):</span>
-</span><span id="DataBased.add_row-233"><a href="#DataBased.add_row-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
-</span><span id="DataBased.add_row-234"><a href="#DataBased.add_row-234"><span class="linenos">234</span></a>
-</span><span id="DataBased.add_row-235"><a href="#DataBased.add_row-235"><span class="linenos">235</span></a><span class="sd">        :param table: The table to insert into.</span>
-</span><span id="DataBased.add_row-236"><a href="#DataBased.add_row-236"><span class="linenos">236</span></a>
-</span><span id="DataBased.add_row-237"><a href="#DataBased.add_row-237"><span class="linenos">237</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
-</span><span id="DataBased.add_row-238"><a href="#DataBased.add_row-238"><span class="linenos">238</span></a>
-</span><span id="DataBased.add_row-239"><a href="#DataBased.add_row-239"><span class="linenos">239</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
-</span><span id="DataBased.add_row-240"><a href="#DataBased.add_row-240"><span class="linenos">240</span></a><span class="sd">        a value for every column in the table. If columns is</span>
-</span><span id="DataBased.add_row-241"><a href="#DataBased.add_row-241"><span class="linenos">241</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_row-242"><a href="#DataBased.add_row-242"><span class="linenos">242</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased.add_row-243"><a href="#DataBased.add_row-243"><span class="linenos">243</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased.add_row-244"><a href="#DataBased.add_row-244"><span class="linenos">244</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.add_row-245"><a href="#DataBased.add_row-245"><span class="linenos">245</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.add_row-246"><a href="#DataBased.add_row-246"><span class="linenos">246</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="DataBased.add_row-247"><a href="#DataBased.add_row-247"><span class="linenos">247</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-248"><a href="#DataBased.add_row-248"><span class="linenos">248</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span>
-</span><span id="DataBased.add_row-249"><a href="#DataBased.add_row-249"><span class="linenos">249</span></a>                    <span class="n">values</span><span class="p">,</span>
-</span><span id="DataBased.add_row-250"><a href="#DataBased.add_row-250"><span class="linenos">250</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-251"><a href="#DataBased.add_row-251"><span class="linenos">251</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_row-252"><a href="#DataBased.add_row-252"><span class="linenos">252</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-253"><a href="#DataBased.add_row-253"><span class="linenos">253</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
-</span><span id="DataBased.add_row-254"><a href="#DataBased.add_row-254"><span class="linenos">254</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-255"><a href="#DataBased.add_row-255"><span class="linenos">255</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_row-256"><a href="#DataBased.add_row-256"><span class="linenos">256</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_row-257"><a href="#DataBased.add_row-257"><span class="linenos">257</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="DataBased.add_row-258"><a href="#DataBased.add_row-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="DataBased.add_row-259"><a href="#DataBased.add_row-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="DataBased.add_row-260"><a href="#DataBased.add_row-260"><span class="linenos">260</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-261"><a href="#DataBased.add_row-261"><span class="linenos">261</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_row-262"><a href="#DataBased.add_row-262"><span class="linenos">262</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_row-235"><a href="#DataBased.add_row-235"><span class="linenos">235</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_row-236"><a href="#DataBased.add_row-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="DataBased.add_row-237"><a href="#DataBased.add_row-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_row-238"><a href="#DataBased.add_row-238"><span class="linenos">238</span></a>    <span class="p">):</span>
+</span><span id="DataBased.add_row-239"><a href="#DataBased.add_row-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
+</span><span id="DataBased.add_row-240"><a href="#DataBased.add_row-240"><span class="linenos">240</span></a>
+</span><span id="DataBased.add_row-241"><a href="#DataBased.add_row-241"><span class="linenos">241</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.add_row-242"><a href="#DataBased.add_row-242"><span class="linenos">242</span></a>
+</span><span id="DataBased.add_row-243"><a href="#DataBased.add_row-243"><span class="linenos">243</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased.add_row-244"><a href="#DataBased.add_row-244"><span class="linenos">244</span></a>
+</span><span id="DataBased.add_row-245"><a href="#DataBased.add_row-245"><span class="linenos">245</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased.add_row-246"><a href="#DataBased.add_row-246"><span class="linenos">246</span></a>
+</span><span id="DataBased.add_row-247"><a href="#DataBased.add_row-247"><span class="linenos">247</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="DataBased.add_row-248"><a href="#DataBased.add_row-248"><span class="linenos">248</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_row-249"><a href="#DataBased.add_row-249"><span class="linenos">249</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased.add_row-250"><a href="#DataBased.add_row-250"><span class="linenos">250</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased.add_row-251"><a href="#DataBased.add_row-251"><span class="linenos">251</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.add_row-252"><a href="#DataBased.add_row-252"><span class="linenos">252</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.add_row-253"><a href="#DataBased.add_row-253"><span class="linenos">253</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="DataBased.add_row-254"><a href="#DataBased.add_row-254"><span class="linenos">254</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_row-255"><a href="#DataBased.add_row-255"><span class="linenos">255</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="DataBased.add_row-256"><a href="#DataBased.add_row-256"><span class="linenos">256</span></a>                    <span class="n">values</span><span class="p">,</span>
+</span><span id="DataBased.add_row-257"><a href="#DataBased.add_row-257"><span class="linenos">257</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-258"><a href="#DataBased.add_row-258"><span class="linenos">258</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_row-259"><a href="#DataBased.add_row-259"><span class="linenos">259</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_row-260"><a href="#DataBased.add_row-260"><span class="linenos">260</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased.add_row-261"><a href="#DataBased.add_row-261"><span class="linenos">261</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-262"><a href="#DataBased.add_row-262"><span class="linenos">262</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_row-263"><a href="#DataBased.add_row-263"><span class="linenos">263</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_row-264"><a href="#DataBased.add_row-264"><span class="linenos">264</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="DataBased.add_row-265"><a href="#DataBased.add_row-265"><span class="linenos">265</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="DataBased.add_row-266"><a href="#DataBased.add_row-266"><span class="linenos">266</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
+</span><span id="DataBased.add_row-267"><a href="#DataBased.add_row-267"><span class="linenos">267</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-268"><a href="#DataBased.add_row-268"><span class="linenos">268</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_row-269"><a href="#DataBased.add_row-269"><span class="linenos">269</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Add row of values to table.</p>
+            <div class="docstring"><p>Add a row of values to a table.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>table</strong>:  The table to insert into.</p></li>
-<li><p><strong>values</strong>:  A tuple of values to be inserted into the table.</p></li>
-<li><p><strong>columns</strong>:  If None, values param is expected to supply
-a value for every column in the table. If columns is
-provided, it should contain the same number of elements as values.</p></li>
-</ul>
+<p><code>table</code>: The table to insert values into.</p>
+
+<p><code>values</code>: A tuple of values to be inserted into the table.</p>
+
+<p><code>columns</code>: If <code>None</code>, <code>values</code> is expected to supply a value for every column in the table.
+If <code>columns</code> is provided, it should contain the same number of elements as <code>values</code>.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.get_rows" class="classattr">
                                         <input id="DataBased.get_rows-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1549,117 +1568,109 @@
         <span class="def">def</span>
         <span class="name">get_rows</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">core</span><span class="o">.</span><span class="n">frame</span><span class="o">.</span><span class="n">DataFrame</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_rows-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_rows"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_rows-264"><a href="#DataBased.get_rows-264"><span class="linenos">264</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_rows-265"><a href="#DataBased.get_rows-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="DataBased.get_rows-266"><a href="#DataBased.get_rows-266"><span class="linenos">266</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-267"><a href="#DataBased.get_rows-267"><span class="linenos">267</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-268"><a href="#DataBased.get_rows-268"><span class="linenos">268</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-269"><a href="#DataBased.get_rows-269"><span class="linenos">269</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-270"><a href="#DataBased.get_rows-270"><span class="linenos">270</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-271"><a href="#DataBased.get_rows-271"><span class="linenos">271</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-272"><a href="#DataBased.get_rows-272"><span class="linenos">272</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-273"><a href="#DataBased.get_rows-273"><span class="linenos">273</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-274"><a href="#DataBased.get_rows-274"><span class="linenos">274</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-275"><a href="#DataBased.get_rows-275"><span class="linenos">275</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-276"><a href="#DataBased.get_rows-276"><span class="linenos">276</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-277"><a href="#DataBased.get_rows-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
-</span><span id="DataBased.get_rows-278"><a href="#DataBased.get_rows-278"><span class="linenos">278</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
-</span><span id="DataBased.get_rows-279"><a href="#DataBased.get_rows-279"><span class="linenos">279</span></a><span class="sd">        column name: row value.</span>
-</span><span id="DataBased.get_rows-280"><a href="#DataBased.get_rows-280"><span class="linenos">280</span></a>
-</span><span id="DataBased.get_rows-281"><a href="#DataBased.get_rows-281"><span class="linenos">281</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.get_rows-282"><a href="#DataBased.get_rows-282"><span class="linenos">282</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.get_rows-283"><a href="#DataBased.get_rows-283"><span class="linenos">283</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.get_rows-284"><a href="#DataBased.get_rows-284"><span class="linenos">284</span></a>
-</span><span id="DataBased.get_rows-285"><a href="#DataBased.get_rows-285"><span class="linenos">285</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased.get_rows-286"><a href="#DataBased.get_rows-286"><span class="linenos">286</span></a><span class="sd">        will be matched as a substring.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_rows-271"><a href="#DataBased.get_rows-271"><span class="linenos">271</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_rows-272"><a href="#DataBased.get_rows-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="DataBased.get_rows-273"><a href="#DataBased.get_rows-273"><span class="linenos">273</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-274"><a href="#DataBased.get_rows-274"><span class="linenos">274</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-275"><a href="#DataBased.get_rows-275"><span class="linenos">275</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-276"><a href="#DataBased.get_rows-276"><span class="linenos">276</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-277"><a href="#DataBased.get_rows-277"><span class="linenos">277</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-278"><a href="#DataBased.get_rows-278"><span class="linenos">278</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-279"><a href="#DataBased.get_rows-279"><span class="linenos">279</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-280"><a href="#DataBased.get_rows-280"><span class="linenos">280</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-281"><a href="#DataBased.get_rows-281"><span class="linenos">281</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-282"><a href="#DataBased.get_rows-282"><span class="linenos">282</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-283"><a href="#DataBased.get_rows-283"><span class="linenos">283</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-284"><a href="#DataBased.get_rows-284"><span class="linenos">284</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
+</span><span id="DataBased.get_rows-285"><a href="#DataBased.get_rows-285"><span class="linenos">285</span></a>
+</span><span id="DataBased.get_rows-286"><a href="#DataBased.get_rows-286"><span class="linenos">286</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
 </span><span id="DataBased.get_rows-287"><a href="#DataBased.get_rows-287"><span class="linenos">287</span></a>
-</span><span id="DataBased.get_rows-288"><a href="#DataBased.get_rows-288"><span class="linenos">288</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
-</span><span id="DataBased.get_rows-289"><a href="#DataBased.get_rows-289"><span class="linenos">289</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="DataBased.get_rows-290"><a href="#DataBased.get_rows-290"><span class="linenos">290</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
-</span><span id="DataBased.get_rows-291"><a href="#DataBased.get_rows-291"><span class="linenos">291</span></a>
-</span><span id="DataBased.get_rows-292"><a href="#DataBased.get_rows-292"><span class="linenos">292</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
-</span><span id="DataBased.get_rows-293"><a href="#DataBased.get_rows-293"><span class="linenos">293</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
-</span><span id="DataBased.get_rows-294"><a href="#DataBased.get_rows-294"><span class="linenos">294</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
-</span><span id="DataBased.get_rows-295"><a href="#DataBased.get_rows-295"><span class="linenos">295</span></a><span class="sd">        in the row is returned.</span>
+</span><span id="DataBased.get_rows-288"><a href="#DataBased.get_rows-288"><span class="linenos">288</span></a>
+</span><span id="DataBased.get_rows-289"><a href="#DataBased.get_rows-289"><span class="linenos">289</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.get_rows-290"><a href="#DataBased.get_rows-290"><span class="linenos">290</span></a>
+</span><span id="DataBased.get_rows-291"><a href="#DataBased.get_rows-291"><span class="linenos">291</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.get_rows-292"><a href="#DataBased.get_rows-292"><span class="linenos">292</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased.get_rows-293"><a href="#DataBased.get_rows-293"><span class="linenos">293</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.get_rows-294"><a href="#DataBased.get_rows-294"><span class="linenos">294</span></a>
+</span><span id="DataBased.get_rows-295"><a href="#DataBased.get_rows-295"><span class="linenos">295</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
 </span><span id="DataBased.get_rows-296"><a href="#DataBased.get_rows-296"><span class="linenos">296</span></a>
-</span><span id="DataBased.get_rows-297"><a href="#DataBased.get_rows-297"><span class="linenos">297</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
-</span><span id="DataBased.get_rows-298"><a href="#DataBased.get_rows-298"><span class="linenos">298</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
-</span><span id="DataBased.get_rows-299"><a href="#DataBased.get_rows-299"><span class="linenos">299</span></a>
-</span><span id="DataBased.get_rows-300"><a href="#DataBased.get_rows-300"><span class="linenos">300</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
-</span><span id="DataBased.get_rows-301"><a href="#DataBased.get_rows-301"><span class="linenos">301</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
-</span><span id="DataBased.get_rows-302"><a href="#DataBased.get_rows-302"><span class="linenos">302</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
-</span><span id="DataBased.get_rows-303"><a href="#DataBased.get_rows-303"><span class="linenos">303</span></a><span class="sd">        one is provided.</span>
+</span><span id="DataBased.get_rows-297"><a href="#DataBased.get_rows-297"><span class="linenos">297</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
+</span><span id="DataBased.get_rows-298"><a href="#DataBased.get_rows-298"><span class="linenos">298</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="DataBased.get_rows-299"><a href="#DataBased.get_rows-299"><span class="linenos">299</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="DataBased.get_rows-300"><a href="#DataBased.get_rows-300"><span class="linenos">300</span></a>
+</span><span id="DataBased.get_rows-301"><a href="#DataBased.get_rows-301"><span class="linenos">301</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
+</span><span id="DataBased.get_rows-302"><a href="#DataBased.get_rows-302"><span class="linenos">302</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
+</span><span id="DataBased.get_rows-303"><a href="#DataBased.get_rows-303"><span class="linenos">303</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
 </span><span id="DataBased.get_rows-304"><a href="#DataBased.get_rows-304"><span class="linenos">304</span></a>
-</span><span id="DataBased.get_rows-305"><a href="#DataBased.get_rows-305"><span class="linenos">305</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
-</span><span id="DataBased.get_rows-306"><a href="#DataBased.get_rows-306"><span class="linenos">306</span></a><span class="sd">        will be added to the select query.</span>
-</span><span id="DataBased.get_rows-307"><a href="#DataBased.get_rows-307"><span class="linenos">307</span></a>
-</span><span id="DataBased.get_rows-308"><a href="#DataBased.get_rows-308"><span class="linenos">308</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
-</span><span id="DataBased.get_rows-309"><a href="#DataBased.get_rows-309"><span class="linenos">309</span></a><span class="sd">        added to the select query.</span>
-</span><span id="DataBased.get_rows-310"><a href="#DataBased.get_rows-310"><span class="linenos">310</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.get_rows-311"><a href="#DataBased.get_rows-311"><span class="linenos">311</span></a>
-</span><span id="DataBased.get_rows-312"><a href="#DataBased.get_rows-312"><span class="linenos">312</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-313"><a href="#DataBased.get_rows-313"><span class="linenos">313</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-314"><a href="#DataBased.get_rows-314"><span class="linenos">314</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-315"><a href="#DataBased.get_rows-315"><span class="linenos">315</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased.get_rows-316"><a href="#DataBased.get_rows-316"><span class="linenos">316</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-317"><a href="#DataBased.get_rows-317"><span class="linenos">317</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-318"><a href="#DataBased.get_rows-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-319"><a href="#DataBased.get_rows-319"><span class="linenos">319</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-320"><a href="#DataBased.get_rows-320"><span class="linenos">320</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-321"><a href="#DataBased.get_rows-321"><span class="linenos">321</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-322"><a href="#DataBased.get_rows-322"><span class="linenos">322</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased.get_rows-323"><a href="#DataBased.get_rows-323"><span class="linenos">323</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased.get_rows-324"><a href="#DataBased.get_rows-324"><span class="linenos">324</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased.get_rows-325"><a href="#DataBased.get_rows-325"><span class="linenos">325</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-326"><a href="#DataBased.get_rows-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-327"><a href="#DataBased.get_rows-327"><span class="linenos">327</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="DataBased.get_rows-328"><a href="#DataBased.get_rows-328"><span class="linenos">328</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-329"><a href="#DataBased.get_rows-329"><span class="linenos">329</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="DataBased.get_rows-330"><a href="#DataBased.get_rows-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-331"><a href="#DataBased.get_rows-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-332"><a href="#DataBased.get_rows-332"><span class="linenos">332</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-333"><a href="#DataBased.get_rows-333"><span class="linenos">333</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased.get_rows-305"><a href="#DataBased.get_rows-305"><span class="linenos">305</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
+</span><span id="DataBased.get_rows-306"><a href="#DataBased.get_rows-306"><span class="linenos">306</span></a>
+</span><span id="DataBased.get_rows-307"><a href="#DataBased.get_rows-307"><span class="linenos">307</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="DataBased.get_rows-308"><a href="#DataBased.get_rows-308"><span class="linenos">308</span></a>
+</span><span id="DataBased.get_rows-309"><a href="#DataBased.get_rows-309"><span class="linenos">309</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="DataBased.get_rows-310"><a href="#DataBased.get_rows-310"><span class="linenos">310</span></a>
+</span><span id="DataBased.get_rows-311"><a href="#DataBased.get_rows-311"><span class="linenos">311</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
+</span><span id="DataBased.get_rows-312"><a href="#DataBased.get_rows-312"><span class="linenos">312</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.get_rows-313"><a href="#DataBased.get_rows-313"><span class="linenos">313</span></a>
+</span><span id="DataBased.get_rows-314"><a href="#DataBased.get_rows-314"><span class="linenos">314</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-315"><a href="#DataBased.get_rows-315"><span class="linenos">315</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-316"><a href="#DataBased.get_rows-316"><span class="linenos">316</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-317"><a href="#DataBased.get_rows-317"><span class="linenos">317</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased.get_rows-318"><a href="#DataBased.get_rows-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-319"><a href="#DataBased.get_rows-319"><span class="linenos">319</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-320"><a href="#DataBased.get_rows-320"><span class="linenos">320</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-321"><a href="#DataBased.get_rows-321"><span class="linenos">321</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-322"><a href="#DataBased.get_rows-322"><span class="linenos">322</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-323"><a href="#DataBased.get_rows-323"><span class="linenos">323</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-324"><a href="#DataBased.get_rows-324"><span class="linenos">324</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased.get_rows-325"><a href="#DataBased.get_rows-325"><span class="linenos">325</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased.get_rows-326"><a href="#DataBased.get_rows-326"><span class="linenos">326</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased.get_rows-327"><a href="#DataBased.get_rows-327"><span class="linenos">327</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-328"><a href="#DataBased.get_rows-328"><span class="linenos">328</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-329"><a href="#DataBased.get_rows-329"><span class="linenos">329</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="DataBased.get_rows-330"><a href="#DataBased.get_rows-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-331"><a href="#DataBased.get_rows-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="DataBased.get_rows-332"><a href="#DataBased.get_rows-332"><span class="linenos">332</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-333"><a href="#DataBased.get_rows-333"><span class="linenos">333</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-334"><a href="#DataBased.get_rows-334"><span class="linenos">334</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-335"><a href="#DataBased.get_rows-335"><span class="linenos">335</span></a>            <span class="k">return</span> <span class="n">results</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns rows from table as a list of dictionaries
-where the key-value pairs of the dictionaries are
-column name: row value.</p>
+            <div class="docstring"><p>Return matching rows from <code>table</code>.</p>
 
-<h6 id="parameters">Parameters</h6>
+<p>By default, rows will be returned as a list of dictionaries of the form <code>[{"column_name": value, ...}, ...]</code></p>
 
-<ul>
-<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each
-tuple is (columnName, rowValue) or a dictionary where
-keys are column names and values are row values.</p></li>
-<li><p><strong>exact_match</strong>:  If False, the rowValue for a give column
-will be matched as a substring.</p></li>
-<li><p><strong>sort_by_column</strong>:  A column name to sort the results by.
+<h4 id="params">:params:</h4>
+
+<p><code>match_criteria</code>: Can be a list of 2-tuples where each
+tuple is <code>(columnName, rowValue)</code> or a dictionary where
+keys are column names and values are row values.</p>
+
+<p><code>exact_match</code>: If <code>False</code>, the row value for a given column will be matched as a substring.</p>
+
+<p><code>sort_by_column</code>: A column name to sort the results by.
 This will sort results in Python after retrieving them from the db.
-Use the 'order_by' param to use SQLite engine for ordering.</p></li>
-<li><p><strong>columns_to_return</strong>:  Optional list of column names.
-If provided, the elements returned by get_rows() will
-only contain the provided columns. Otherwise every column
-in the row is returned.</p></li>
-<li><p><strong>return_as_dataframe</strong>:  If True,
-the results will be returned as a pandas.DataFrame object.</p></li>
-<li><p><strong>values_only</strong>:  Return the results as a list of tuples
-instead of a list of dictionaries that have column names as keys.
-The results will still be sorted according to sort_by_column if
-one is provided.</p></li>
-<li><p><strong>order_by</strong>:  If given, a 'order by {order_by}' clause
-will be added to the select query.</p></li>
-<li><p><strong>limit</strong>:  If given, a 'limit {limit}' clause will be
-added to the select query.</p></li>
-</ul>
+Use the 'order_by' param to use SQLite engine for ordering.</p>
+
+<p><code>columns_to_return</code>: Optional list of column names.
+If provided, the elements returned by this function will only contain the provided columns.
+Otherwise every column in the row is returned.</p>
+
+<p><code>return_as_dataframe</code>: Return the results as a <code>pandas.DataFrame</code> object.</p>
+
+<p><code>values_only</code>: Return the results as a list of tuples.</p>
+
+<p><code>order_by</code>: If given, a <code>order by {order_by}</code> clause will be added to the select query.</p>
+
+<p><code>limit</code>: If given, a <code>limit {limit}</code> clause will be added to the select query.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.find" class="classattr">
                                         <input id="DataBased.find-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1667,58 +1678,58 @@
         <span class="def">def</span>
         <span class="name">find</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.find-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.find"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.find-335"><a href="#DataBased.find-335"><span class="linenos">335</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.find-336"><a href="#DataBased.find-336"><span class="linenos">336</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="DataBased.find-337"><a href="#DataBased.find-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.find-338"><a href="#DataBased.find-338"><span class="linenos">338</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="DataBased.find-339"><a href="#DataBased.find-339"><span class="linenos">339</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
-</span><span id="DataBased.find-340"><a href="#DataBased.find-340"><span class="linenos">340</span></a><span class="sd">        of any column.</span>
-</span><span id="DataBased.find-341"><a href="#DataBased.find-341"><span class="linenos">341</span></a>
-</span><span id="DataBased.find-342"><a href="#DataBased.find-342"><span class="linenos">342</span></a><span class="sd">        :param table: The table to search.</span>
-</span><span id="DataBased.find-343"><a href="#DataBased.find-343"><span class="linenos">343</span></a>
-</span><span id="DataBased.find-344"><a href="#DataBased.find-344"><span class="linenos">344</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
-</span><span id="DataBased.find-345"><a href="#DataBased.find-345"><span class="linenos">345</span></a>
-</span><span id="DataBased.find-346"><a href="#DataBased.find-346"><span class="linenos">346</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
-</span><span id="DataBased.find-347"><a href="#DataBased.find-347"><span class="linenos">347</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="DataBased.find-348"><a href="#DataBased.find-348"><span class="linenos">348</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.find-349"><a href="#DataBased.find-349"><span class="linenos">349</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.find-350"><a href="#DataBased.find-350"><span class="linenos">350</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="DataBased.find-351"><a href="#DataBased.find-351"><span class="linenos">351</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased.find-352"><a href="#DataBased.find-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.find-353"><a href="#DataBased.find-353"><span class="linenos">353</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DataBased.find-354"><a href="#DataBased.find-354"><span class="linenos">354</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.find-355"><a href="#DataBased.find-355"><span class="linenos">355</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="DataBased.find-356"><a href="#DataBased.find-356"><span class="linenos">356</span></a>                <span class="p">[</span>
-</span><span id="DataBased.find-357"><a href="#DataBased.find-357"><span class="linenos">357</span></a>                    <span class="n">row</span>
-</span><span id="DataBased.find-358"><a href="#DataBased.find-358"><span class="linenos">358</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DataBased.find-359"><a href="#DataBased.find-359"><span class="linenos">359</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="DataBased.find-360"><a href="#DataBased.find-360"><span class="linenos">360</span></a>                    <span class="p">)</span>
-</span><span id="DataBased.find-361"><a href="#DataBased.find-361"><span class="linenos">361</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="DataBased.find-362"><a href="#DataBased.find-362"><span class="linenos">362</span></a>                <span class="p">]</span>
-</span><span id="DataBased.find-363"><a href="#DataBased.find-363"><span class="linenos">363</span></a>            <span class="p">)</span>
-</span><span id="DataBased.find-364"><a href="#DataBased.find-364"><span class="linenos">364</span></a>        <span class="k">return</span> <span class="n">results</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.find-337"><a href="#DataBased.find-337"><span class="linenos">337</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.find-338"><a href="#DataBased.find-338"><span class="linenos">338</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="DataBased.find-339"><a href="#DataBased.find-339"><span class="linenos">339</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.find-340"><a href="#DataBased.find-340"><span class="linenos">340</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="DataBased.find-341"><a href="#DataBased.find-341"><span class="linenos">341</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
+</span><span id="DataBased.find-342"><a href="#DataBased.find-342"><span class="linenos">342</span></a>
+</span><span id="DataBased.find-343"><a href="#DataBased.find-343"><span class="linenos">343</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.find-344"><a href="#DataBased.find-344"><span class="linenos">344</span></a>
+</span><span id="DataBased.find-345"><a href="#DataBased.find-345"><span class="linenos">345</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="DataBased.find-346"><a href="#DataBased.find-346"><span class="linenos">346</span></a>
+</span><span id="DataBased.find-347"><a href="#DataBased.find-347"><span class="linenos">347</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="DataBased.find-348"><a href="#DataBased.find-348"><span class="linenos">348</span></a>
+</span><span id="DataBased.find-349"><a href="#DataBased.find-349"><span class="linenos">349</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
+</span><span id="DataBased.find-350"><a href="#DataBased.find-350"><span class="linenos">350</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="DataBased.find-351"><a href="#DataBased.find-351"><span class="linenos">351</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.find-352"><a href="#DataBased.find-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.find-353"><a href="#DataBased.find-353"><span class="linenos">353</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="DataBased.find-354"><a href="#DataBased.find-354"><span class="linenos">354</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased.find-355"><a href="#DataBased.find-355"><span class="linenos">355</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.find-356"><a href="#DataBased.find-356"><span class="linenos">356</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DataBased.find-357"><a href="#DataBased.find-357"><span class="linenos">357</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.find-358"><a href="#DataBased.find-358"><span class="linenos">358</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="DataBased.find-359"><a href="#DataBased.find-359"><span class="linenos">359</span></a>                <span class="p">[</span>
+</span><span id="DataBased.find-360"><a href="#DataBased.find-360"><span class="linenos">360</span></a>                    <span class="n">row</span>
+</span><span id="DataBased.find-361"><a href="#DataBased.find-361"><span class="linenos">361</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DataBased.find-362"><a href="#DataBased.find-362"><span class="linenos">362</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="DataBased.find-363"><a href="#DataBased.find-363"><span class="linenos">363</span></a>                    <span class="p">)</span>
+</span><span id="DataBased.find-364"><a href="#DataBased.find-364"><span class="linenos">364</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="DataBased.find-365"><a href="#DataBased.find-365"><span class="linenos">365</span></a>                <span class="p">]</span>
+</span><span id="DataBased.find-366"><a href="#DataBased.find-366"><span class="linenos">366</span></a>            <span class="p">)</span>
+</span><span id="DataBased.find-367"><a href="#DataBased.find-367"><span class="linenos">367</span></a>        <span class="k">return</span> <span class="n">results</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Search for rows that contain query_string as a substring
-of any column.</p>
+            <div class="docstring"><p>Search for rows that contain <code>query_string</code> as a substring of any column.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>table</strong>:  The table to search.</p></li>
-<li><p><strong>query_string</strong>:  The substring to search for in all columns.</p></li>
-<li><p><strong>columns</strong>:  A list of columns to search for query_string.
-If None, all columns in the table will be searched.</p></li>
-</ul>
+<p><code>table</code>: The table to search.</p>
+
+<p><code>query_string</code>: The substring to search for in all columns.</p>
+
+<p><code>columns</code>: A list of columns to search for query_string.
+If None, all columns in the table will be searched.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.delete" class="classattr">
                                         <input id="DataBased.delete-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1726,56 +1737,53 @@
         <span class="def">def</span>
         <span class="name">delete</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.delete-366"><a href="#DataBased.delete-366"><span class="linenos">366</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.delete-367"><a href="#DataBased.delete-367"><span class="linenos">367</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="DataBased.delete-368"><a href="#DataBased.delete-368"><span class="linenos">368</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.delete-369"><a href="#DataBased.delete-369"><span class="linenos">369</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.delete-370"><a href="#DataBased.delete-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
-</span><span id="DataBased.delete-371"><a href="#DataBased.delete-371"><span class="linenos">371</span></a>
-</span><span id="DataBased.delete-372"><a href="#DataBased.delete-372"><span class="linenos">372</span></a><span class="sd">        Returns number of deleted records.</span>
-</span><span id="DataBased.delete-373"><a href="#DataBased.delete-373"><span class="linenos">373</span></a>
-</span><span id="DataBased.delete-374"><a href="#DataBased.delete-374"><span class="linenos">374</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.delete-375"><a href="#DataBased.delete-375"><span class="linenos">375</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.delete-376"><a href="#DataBased.delete-376"><span class="linenos">376</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.delete-377"><a href="#DataBased.delete-377"><span class="linenos">377</span></a>
-</span><span id="DataBased.delete-378"><a href="#DataBased.delete-378"><span class="linenos">378</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased.delete-379"><a href="#DataBased.delete-379"><span class="linenos">379</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased.delete-380"><a href="#DataBased.delete-380"><span class="linenos">380</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.delete-381"><a href="#DataBased.delete-381"><span class="linenos">381</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased.delete-382"><a href="#DataBased.delete-382"><span class="linenos">382</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased.delete-383"><a href="#DataBased.delete-383"><span class="linenos">383</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.delete-384"><a href="#DataBased.delete-384"><span class="linenos">384</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.delete-385"><a href="#DataBased.delete-385"><span class="linenos">385</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.delete-386"><a href="#DataBased.delete-386"><span class="linenos">386</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="DataBased.delete-387"><a href="#DataBased.delete-387"><span class="linenos">387</span></a>            <span class="p">)</span>
-</span><span id="DataBased.delete-388"><a href="#DataBased.delete-388"><span class="linenos">388</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
-</span><span id="DataBased.delete-389"><a href="#DataBased.delete-389"><span class="linenos">389</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.delete-390"><a href="#DataBased.delete-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="DataBased.delete-391"><a href="#DataBased.delete-391"><span class="linenos">391</span></a>            <span class="k">return</span> <span class="mi">0</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.delete-369"><a href="#DataBased.delete-369"><span class="linenos">369</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.delete-370"><a href="#DataBased.delete-370"><span class="linenos">370</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="DataBased.delete-371"><a href="#DataBased.delete-371"><span class="linenos">371</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.delete-372"><a href="#DataBased.delete-372"><span class="linenos">372</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.delete-373"><a href="#DataBased.delete-373"><span class="linenos">373</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
+</span><span id="DataBased.delete-374"><a href="#DataBased.delete-374"><span class="linenos">374</span></a>
+</span><span id="DataBased.delete-375"><a href="#DataBased.delete-375"><span class="linenos">375</span></a><span class="sd">        Returns the number of deleted records.</span>
+</span><span id="DataBased.delete-376"><a href="#DataBased.delete-376"><span class="linenos">376</span></a>
+</span><span id="DataBased.delete-377"><a href="#DataBased.delete-377"><span class="linenos">377</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.delete-378"><a href="#DataBased.delete-378"><span class="linenos">378</span></a>
+</span><span id="DataBased.delete-379"><a href="#DataBased.delete-379"><span class="linenos">379</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
+</span><span id="DataBased.delete-380"><a href="#DataBased.delete-380"><span class="linenos">380</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased.delete-381"><a href="#DataBased.delete-381"><span class="linenos">381</span></a>
+</span><span id="DataBased.delete-382"><a href="#DataBased.delete-382"><span class="linenos">382</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
+</span><span id="DataBased.delete-383"><a href="#DataBased.delete-383"><span class="linenos">383</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.delete-384"><a href="#DataBased.delete-384"><span class="linenos">384</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased.delete-385"><a href="#DataBased.delete-385"><span class="linenos">385</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased.delete-386"><a href="#DataBased.delete-386"><span class="linenos">386</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.delete-387"><a href="#DataBased.delete-387"><span class="linenos">387</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.delete-388"><a href="#DataBased.delete-388"><span class="linenos">388</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.delete-389"><a href="#DataBased.delete-389"><span class="linenos">389</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="DataBased.delete-390"><a href="#DataBased.delete-390"><span class="linenos">390</span></a>            <span class="p">)</span>
+</span><span id="DataBased.delete-391"><a href="#DataBased.delete-391"><span class="linenos">391</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
+</span><span id="DataBased.delete-392"><a href="#DataBased.delete-392"><span class="linenos">392</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.delete-393"><a href="#DataBased.delete-393"><span class="linenos">393</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="DataBased.delete-394"><a href="#DataBased.delete-394"><span class="linenos">394</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Delete records from table.</p>
+            <div class="docstring"><p>Delete records from <code>table</code>.</p>
 
-<p>Returns number of deleted records.</p>
+<p>Returns the number of deleted records.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each
-tuple is (columnName, rowValue) or a dictionary where
-keys are column names and values are row values.</p></li>
-<li><p><strong>exact_match</strong>:  If False, the rowValue for a give column
-will be matched as a substring.</p></li>
-</ul>
+<p><code>match_criteria</code>: Can be a list of 2-tuples where each tuple is <code>(column_name, value)</code>
+or a dictionary where keys are column names and values are corresponding values.</p>
+
+<p><code>exact_match</code>: If <code>False</code>, the value for a given column will be matched as a substring.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.update" class="classattr">
                                         <input id="DataBased.update-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1783,77 +1791,82 @@
         <span class="def">def</span>
         <span class="name">update</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.update-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.update"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.update-393"><a href="#DataBased.update-393"><span class="linenos">393</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.update-394"><a href="#DataBased.update-394"><span class="linenos">394</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="DataBased.update-395"><a href="#DataBased.update-395"><span class="linenos">395</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.update-396"><a href="#DataBased.update-396"><span class="linenos">396</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.update-397"><a href="#DataBased.update-397"><span class="linenos">397</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.update-398"><a href="#DataBased.update-398"><span class="linenos">398</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="DataBased.update-399"><a href="#DataBased.update-399"><span class="linenos">399</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.update-400"><a href="#DataBased.update-400"><span class="linenos">400</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased.update-401"><a href="#DataBased.update-401"><span class="linenos">401</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
-</span><span id="DataBased.update-402"><a href="#DataBased.update-402"><span class="linenos">402</span></a>
-</span><span id="DataBased.update-403"><a href="#DataBased.update-403"><span class="linenos">403</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
-</span><span id="DataBased.update-404"><a href="#DataBased.update-404"><span class="linenos">404</span></a>
-</span><span id="DataBased.update-405"><a href="#DataBased.update-405"><span class="linenos">405</span></a><span class="sd">        :param new_value: The new value to insert.</span>
-</span><span id="DataBased.update-406"><a href="#DataBased.update-406"><span class="linenos">406</span></a>
-</span><span id="DataBased.update-407"><a href="#DataBased.update-407"><span class="linenos">407</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.update-408"><a href="#DataBased.update-408"><span class="linenos">408</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.update-409"><a href="#DataBased.update-409"><span class="linenos">409</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.update-410"><a href="#DataBased.update-410"><span class="linenos">410</span></a><span class="sd">        If None, every row will be updated.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.update-396"><a href="#DataBased.update-396"><span class="linenos">396</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.update-397"><a href="#DataBased.update-397"><span class="linenos">397</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="DataBased.update-398"><a href="#DataBased.update-398"><span class="linenos">398</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.update-399"><a href="#DataBased.update-399"><span class="linenos">399</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.update-400"><a href="#DataBased.update-400"><span class="linenos">400</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.update-401"><a href="#DataBased.update-401"><span class="linenos">401</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="DataBased.update-402"><a href="#DataBased.update-402"><span class="linenos">402</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.update-403"><a href="#DataBased.update-403"><span class="linenos">403</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased.update-404"><a href="#DataBased.update-404"><span class="linenos">404</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
+</span><span id="DataBased.update-405"><a href="#DataBased.update-405"><span class="linenos">405</span></a>
+</span><span id="DataBased.update-406"><a href="#DataBased.update-406"><span class="linenos">406</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.update-407"><a href="#DataBased.update-407"><span class="linenos">407</span></a>
+</span><span id="DataBased.update-408"><a href="#DataBased.update-408"><span class="linenos">408</span></a><span class="sd">        `table`: The table to update rows in.</span>
+</span><span id="DataBased.update-409"><a href="#DataBased.update-409"><span class="linenos">409</span></a>
+</span><span id="DataBased.update-410"><a href="#DataBased.update-410"><span class="linenos">410</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
 </span><span id="DataBased.update-411"><a href="#DataBased.update-411"><span class="linenos">411</span></a>
-</span><span id="DataBased.update-412"><a href="#DataBased.update-412"><span class="linenos">412</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased.update-413"><a href="#DataBased.update-413"><span class="linenos">413</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="DataBased.update-414"><a href="#DataBased.update-414"><span class="linenos">414</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="DataBased.update-415"><a href="#DataBased.update-415"><span class="linenos">415</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.update-416"><a href="#DataBased.update-416"><span class="linenos">416</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased.update-417"><a href="#DataBased.update-417"><span class="linenos">417</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.update-418"><a href="#DataBased.update-418"><span class="linenos">418</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
-</span><span id="DataBased.update-419"><a href="#DataBased.update-419"><span class="linenos">419</span></a>                <span class="p">)</span>
-</span><span id="DataBased.update-420"><a href="#DataBased.update-420"><span class="linenos">420</span></a>                <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased.update-421"><a href="#DataBased.update-421"><span class="linenos">421</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
-</span><span id="DataBased.update-422"><a href="#DataBased.update-422"><span class="linenos">422</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.update-423"><a href="#DataBased.update-423"><span class="linenos">423</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.update-424"><a href="#DataBased.update-424"><span class="linenos">424</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.update-425"><a href="#DataBased.update-425"><span class="linenos">425</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.update-426"><a href="#DataBased.update-426"><span class="linenos">426</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.update-427"><a href="#DataBased.update-427"><span class="linenos">427</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="DataBased.update-428"><a href="#DataBased.update-428"><span class="linenos">428</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="DataBased.update-429"><a href="#DataBased.update-429"><span class="linenos">429</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-430"><a href="#DataBased.update-430"><span class="linenos">430</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.update-431"><a href="#DataBased.update-431"><span class="linenos">431</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased.update-432"><a href="#DataBased.update-432"><span class="linenos">432</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-433"><a href="#DataBased.update-433"><span class="linenos">433</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased.update-434"><a href="#DataBased.update-434"><span class="linenos">434</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.update-435"><a href="#DataBased.update-435"><span class="linenos">435</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased.update-436"><a href="#DataBased.update-436"><span class="linenos">436</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased.update-437"><a href="#DataBased.update-437"><span class="linenos">437</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-438"><a href="#DataBased.update-438"><span class="linenos">438</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased.update-412"><a href="#DataBased.update-412"><span class="linenos">412</span></a><span class="sd">        `new_value`: The new value to insert.</span>
+</span><span id="DataBased.update-413"><a href="#DataBased.update-413"><span class="linenos">413</span></a>
+</span><span id="DataBased.update-414"><a href="#DataBased.update-414"><span class="linenos">414</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
+</span><span id="DataBased.update-415"><a href="#DataBased.update-415"><span class="linenos">415</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased.update-416"><a href="#DataBased.update-416"><span class="linenos">416</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="DataBased.update-417"><a href="#DataBased.update-417"><span class="linenos">417</span></a>
+</span><span id="DataBased.update-418"><a href="#DataBased.update-418"><span class="linenos">418</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased.update-419"><a href="#DataBased.update-419"><span class="linenos">419</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased.update-420"><a href="#DataBased.update-420"><span class="linenos">420</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="DataBased.update-421"><a href="#DataBased.update-421"><span class="linenos">421</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.update-422"><a href="#DataBased.update-422"><span class="linenos">422</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased.update-423"><a href="#DataBased.update-423"><span class="linenos">423</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.update-424"><a href="#DataBased.update-424"><span class="linenos">424</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
+</span><span id="DataBased.update-425"><a href="#DataBased.update-425"><span class="linenos">425</span></a>                <span class="p">)</span>
+</span><span id="DataBased.update-426"><a href="#DataBased.update-426"><span class="linenos">426</span></a>                <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased.update-427"><a href="#DataBased.update-427"><span class="linenos">427</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
+</span><span id="DataBased.update-428"><a href="#DataBased.update-428"><span class="linenos">428</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.update-429"><a href="#DataBased.update-429"><span class="linenos">429</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.update-430"><a href="#DataBased.update-430"><span class="linenos">430</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.update-431"><a href="#DataBased.update-431"><span class="linenos">431</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased.update-432"><a href="#DataBased.update-432"><span class="linenos">432</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.update-433"><a href="#DataBased.update-433"><span class="linenos">433</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.update-434"><a href="#DataBased.update-434"><span class="linenos">434</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="DataBased.update-435"><a href="#DataBased.update-435"><span class="linenos">435</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
+</span><span id="DataBased.update-436"><a href="#DataBased.update-436"><span class="linenos">436</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-437"><a href="#DataBased.update-437"><span class="linenos">437</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.update-438"><a href="#DataBased.update-438"><span class="linenos">438</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.update-439"><a href="#DataBased.update-439"><span class="linenos">439</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-440"><a href="#DataBased.update-440"><span class="linenos">440</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased.update-441"><a href="#DataBased.update-441"><span class="linenos">441</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.update-442"><a href="#DataBased.update-442"><span class="linenos">442</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="DataBased.update-443"><a href="#DataBased.update-443"><span class="linenos">443</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.update-444"><a href="#DataBased.update-444"><span class="linenos">444</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-445"><a href="#DataBased.update-445"><span class="linenos">445</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Update row value for entry matched with match_criteria.</p>
+            <div class="docstring"><p>Update the value in <code>column_to_update</code> to <code>new_value</code> for rows matched with <code>match_criteria</code>.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>column_to_update</strong>:  The column to be updated in the matched row.</p></li>
-<li><p><strong>new_value</strong>:  The new value to insert.</p></li>
-<li><p><strong>match_criteria</strong>:  Can be a list of 2-tuples where each
-tuple is (columnName, rowValue) or a dictionary where
-keys are column names and values are row values.
-If None, every row will be updated.</p></li>
-</ul>
+<p><code>table</code>: The table to update rows in.</p>
+
+<p><code>column_to_update</code>: The column to be updated in the matched rows.</p>
 
-<p>Returns True if successful, False if not.</p>
+<p><code>new_value</code>: The new value to insert.</p>
+
+<p><code>match_criteria</code>: Can be a list of 2-tuples where each tuple is <code>(columnName, rowValue)</code>
+or a dictionary where keys are column names and values are corresponding values.
+If <code>None</code>, every row in <code>table</code> will be updated.</p>
+
+<p>Returns <code>True</code> if successful, <code>False</code> if not.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.drop_table" class="classattr">
                                         <input id="DataBased.drop_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1861,33 +1874,33 @@
         <span class="def">def</span>
         <span class="name">drop_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.drop_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.drop_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-440"><a href="#DataBased.drop_table-440"><span class="linenos">440</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.drop_table-441"><a href="#DataBased.drop_table-441"><span class="linenos">441</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-442"><a href="#DataBased.drop_table-442"><span class="linenos">442</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
-</span><span id="DataBased.drop_table-443"><a href="#DataBased.drop_table-443"><span class="linenos">443</span></a>
-</span><span id="DataBased.drop_table-444"><a href="#DataBased.drop_table-444"><span class="linenos">444</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased.drop_table-445"><a href="#DataBased.drop_table-445"><span class="linenos">445</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-446"><a href="#DataBased.drop_table-446"><span class="linenos">446</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-447"><a href="#DataBased.drop_table-447"><span class="linenos">447</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-448"><a href="#DataBased.drop_table-448"><span class="linenos">448</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased.drop_table-449"><a href="#DataBased.drop_table-449"><span class="linenos">449</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-450"><a href="#DataBased.drop_table-450"><span class="linenos">450</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-451"><a href="#DataBased.drop_table-451"><span class="linenos">451</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-452"><a href="#DataBased.drop_table-452"><span class="linenos">452</span></a>            <span class="k">return</span> <span class="kc">False</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-447"><a href="#DataBased.drop_table-447"><span class="linenos">447</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.drop_table-448"><a href="#DataBased.drop_table-448"><span class="linenos">448</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-449"><a href="#DataBased.drop_table-449"><span class="linenos">449</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="DataBased.drop_table-450"><a href="#DataBased.drop_table-450"><span class="linenos">450</span></a>
+</span><span id="DataBased.drop_table-451"><a href="#DataBased.drop_table-451"><span class="linenos">451</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased.drop_table-452"><a href="#DataBased.drop_table-452"><span class="linenos">452</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-453"><a href="#DataBased.drop_table-453"><span class="linenos">453</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-454"><a href="#DataBased.drop_table-454"><span class="linenos">454</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-455"><a href="#DataBased.drop_table-455"><span class="linenos">455</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased.drop_table-456"><a href="#DataBased.drop_table-456"><span class="linenos">456</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-457"><a href="#DataBased.drop_table-457"><span class="linenos">457</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-458"><a href="#DataBased.drop_table-458"><span class="linenos">458</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-459"><a href="#DataBased.drop_table-459"><span class="linenos">459</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Drop a table from the database.</p>
+            <div class="docstring"><p>Drop <code>table</code> from the database.</p>
 
-<p>Returns True if successful, False if not.</p>
+<p>Returns <code>True</code> if successful, <code>False</code> if not.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.add_column" class="classattr">
                                         <input id="DataBased.add_column-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1895,47 +1908,50 @@
         <span class="def">def</span>
         <span class="name">add_column</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">_type</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.add_column-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_column"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_column-454"><a href="#DataBased.add_column-454"><span class="linenos">454</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_column-455"><a href="#DataBased.add_column-455"><span class="linenos">455</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="DataBased.add_column-456"><a href="#DataBased.add_column-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.add_column-457"><a href="#DataBased.add_column-457"><span class="linenos">457</span></a>    <span class="p">):</span>
-</span><span id="DataBased.add_column-458"><a href="#DataBased.add_column-458"><span class="linenos">458</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
-</span><span id="DataBased.add_column-459"><a href="#DataBased.add_column-459"><span class="linenos">459</span></a>
-</span><span id="DataBased.add_column-460"><a href="#DataBased.add_column-460"><span class="linenos">460</span></a><span class="sd">        :param column: Name of the column to add.</span>
-</span><span id="DataBased.add_column-461"><a href="#DataBased.add_column-461"><span class="linenos">461</span></a>
-</span><span id="DataBased.add_column-462"><a href="#DataBased.add_column-462"><span class="linenos">462</span></a><span class="sd">        :param _type: The data type of the new column.</span>
-</span><span id="DataBased.add_column-463"><a href="#DataBased.add_column-463"><span class="linenos">463</span></a>
-</span><span id="DataBased.add_column-464"><a href="#DataBased.add_column-464"><span class="linenos">464</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_column-465"><a href="#DataBased.add_column-465"><span class="linenos">465</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.add_column-466"><a href="#DataBased.add_column-466"><span class="linenos">466</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="DataBased.add_column-467"><a href="#DataBased.add_column-467"><span class="linenos">467</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_column-468"><a href="#DataBased.add_column-468"><span class="linenos">468</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.add_column-469"><a href="#DataBased.add_column-469"><span class="linenos">469</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_column-470"><a href="#DataBased.add_column-470"><span class="linenos">470</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_column-471"><a href="#DataBased.add_column-471"><span class="linenos">471</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-472"><a href="#DataBased.add_column-472"><span class="linenos">472</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-473"><a href="#DataBased.add_column-473"><span class="linenos">473</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_column-474"><a href="#DataBased.add_column-474"><span class="linenos">474</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_column-461"><a href="#DataBased.add_column-461"><span class="linenos">461</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_column-462"><a href="#DataBased.add_column-462"><span class="linenos">462</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="DataBased.add_column-463"><a href="#DataBased.add_column-463"><span class="linenos">463</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_column-464"><a href="#DataBased.add_column-464"><span class="linenos">464</span></a>    <span class="p">):</span>
+</span><span id="DataBased.add_column-465"><a href="#DataBased.add_column-465"><span class="linenos">465</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
+</span><span id="DataBased.add_column-466"><a href="#DataBased.add_column-466"><span class="linenos">466</span></a>
+</span><span id="DataBased.add_column-467"><a href="#DataBased.add_column-467"><span class="linenos">467</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.add_column-468"><a href="#DataBased.add_column-468"><span class="linenos">468</span></a>
+</span><span id="DataBased.add_column-469"><a href="#DataBased.add_column-469"><span class="linenos">469</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="DataBased.add_column-470"><a href="#DataBased.add_column-470"><span class="linenos">470</span></a>
+</span><span id="DataBased.add_column-471"><a href="#DataBased.add_column-471"><span class="linenos">471</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="DataBased.add_column-472"><a href="#DataBased.add_column-472"><span class="linenos">472</span></a>
+</span><span id="DataBased.add_column-473"><a href="#DataBased.add_column-473"><span class="linenos">473</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_column-474"><a href="#DataBased.add_column-474"><span class="linenos">474</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.add_column-475"><a href="#DataBased.add_column-475"><span class="linenos">475</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="DataBased.add_column-476"><a href="#DataBased.add_column-476"><span class="linenos">476</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_column-477"><a href="#DataBased.add_column-477"><span class="linenos">477</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.add_column-478"><a href="#DataBased.add_column-478"><span class="linenos">478</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_column-479"><a href="#DataBased.add_column-479"><span class="linenos">479</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
+</span><span id="DataBased.add_column-480"><a href="#DataBased.add_column-480"><span class="linenos">480</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_column-481"><a href="#DataBased.add_column-481"><span class="linenos">481</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-482"><a href="#DataBased.add_column-482"><span class="linenos">482</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-483"><a href="#DataBased.add_column-483"><span class="linenos">483</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_column-484"><a href="#DataBased.add_column-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Add a new column to table.</p>
+            <div class="docstring"><p>Add a new column to <code>table</code>.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>column</strong>:  Name of the column to add.</p></li>
-<li><p><strong>_type</strong>:  The data type of the new column.</p></li>
-<li><p><strong>default_value</strong>:  Optional default value for the column.</p></li>
-</ul>
+<p><code>column</code>: Name of the column to add.</p>
+
+<p><code>_type</code>: The data type of the new column.</p>
+
+<p><code>default_value</code>: Optional default value for the column.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.data_to_string" class="classattr">
                                         <input id="DataBased.data_to_string-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1944,44 +1960,44 @@
         <span class="def">def</span>
         <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-476"><a href="#DataBased.data_to_string-476"><span class="linenos">476</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased.data_to_string-477"><a href="#DataBased.data_to_string-477"><span class="linenos">477</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased.data_to_string-478"><a href="#DataBased.data_to_string-478"><span class="linenos">478</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.data_to_string-479"><a href="#DataBased.data_to_string-479"><span class="linenos">479</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.data_to_string-480"><a href="#DataBased.data_to_string-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
-</span><span id="DataBased.data_to_string-481"><a href="#DataBased.data_to_string-481"><span class="linenos">481</span></a><span class="sd">        from a list of dictionaries.</span>
-</span><span id="DataBased.data_to_string-482"><a href="#DataBased.data_to_string-482"><span class="linenos">482</span></a>
-</span><span id="DataBased.data_to_string-483"><a href="#DataBased.data_to_string-483"><span class="linenos">483</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased.data_to_string-484"><a href="#DataBased.data_to_string-484"><span class="linenos">484</span></a>
-</span><span id="DataBased.data_to_string-485"><a href="#DataBased.data_to_string-485"><span class="linenos">485</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="DataBased.data_to_string-486"><a href="#DataBased.data_to_string-486"><span class="linenos">486</span></a>
-</span><span id="DataBased.data_to_string-487"><a href="#DataBased.data_to_string-487"><span class="linenos">487</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
-</span><span id="DataBased.data_to_string-488"><a href="#DataBased.data_to_string-488"><span class="linenos">488</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
-</span><span id="DataBased.data_to_string-489"><a href="#DataBased.data_to_string-489"><span class="linenos">489</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
-</span><span id="DataBased.data_to_string-490"><a href="#DataBased.data_to_string-490"><span class="linenos">490</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-486"><a href="#DataBased.data_to_string-486"><span class="linenos">486</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased.data_to_string-487"><a href="#DataBased.data_to_string-487"><span class="linenos">487</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased.data_to_string-488"><a href="#DataBased.data_to_string-488"><span class="linenos">488</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.data_to_string-489"><a href="#DataBased.data_to_string-489"><span class="linenos">489</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.data_to_string-490"><a href="#DataBased.data_to_string-490"><span class="linenos">490</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="DataBased.data_to_string-491"><a href="#DataBased.data_to_string-491"><span class="linenos">491</span></a>
+</span><span id="DataBased.data_to_string-492"><a href="#DataBased.data_to_string-492"><span class="linenos">492</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.data_to_string-493"><a href="#DataBased.data_to_string-493"><span class="linenos">493</span></a>
+</span><span id="DataBased.data_to_string-494"><a href="#DataBased.data_to_string-494"><span class="linenos">494</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="DataBased.data_to_string-495"><a href="#DataBased.data_to_string-495"><span class="linenos">495</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="DataBased.data_to_string-496"><a href="#DataBased.data_to_string-496"><span class="linenos">496</span></a>
+</span><span id="DataBased.data_to_string-497"><a href="#DataBased.data_to_string-497"><span class="linenos">497</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased.data_to_string-498"><a href="#DataBased.data_to_string-498"><span class="linenos">498</span></a>
+</span><span id="DataBased.data_to_string-499"><a href="#DataBased.data_to_string-499"><span class="linenos">499</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="DataBased.data_to_string-500"><a href="#DataBased.data_to_string-500"><span class="linenos">500</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="DataBased.data_to_string-501"><a href="#DataBased.data_to_string-501"><span class="linenos">501</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Uses tabulate to produce pretty string output
-from a list of dictionaries.</p>
+            <div class="docstring"><p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>data</strong>:  Assumes all dictionaries in list have the same set of keys.</p></li>
-<li><p><strong>sort_key</strong>:  Optional dictionary key to sort data with.</p></li>
-<li><p><strong>wrap_to_terminal</strong>:  If True, the table width will be wrapped
-to fit within the current terminal window. Set to False
-if the output is going into something like a txt file.</p></li>
-</ul>
+<p><code>data</code>: The list of dictionaries to create a grid from.
+Assumes all dictionaries in list have the same set of keys.</p>
+
+<p><code>sort_key</code>: Optional dictionary key to sort data with.</p>
+
+<p><code>wrap_to_terminal</code>: If <code>True</code>, the table width will be wrapped to fit within the current terminal window.
+Pass as <code>False</code> if the output is going into something like a <code>.txt</code> file.</p>
 </div>
 
 
                             </div>
                 </section>
                 <section id="data_to_string">
                             <input id="data_to_string-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -1990,92 +2006,94 @@
         <span class="def">def</span>
         <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-493"><a href="#data_to_string-493"><span class="linenos">493</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="data_to_string-494"><a href="#data_to_string-494"><span class="linenos">494</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-495"><a href="#data_to_string-495"><span class="linenos">495</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="data_to_string-496"><a href="#data_to_string-496"><span class="linenos">496</span></a>    <span class="sd">&quot;&quot;&quot;Use tabulate to produce grid output from a list of dictionaries.</span>
-</span><span id="data_to_string-497"><a href="#data_to_string-497"><span class="linenos">497</span></a>
-</span><span id="data_to_string-498"><a href="#data_to_string-498"><span class="linenos">498</span></a><span class="sd">    :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="data_to_string-499"><a href="#data_to_string-499"><span class="linenos">499</span></a>
-</span><span id="data_to_string-500"><a href="#data_to_string-500"><span class="linenos">500</span></a><span class="sd">    :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="data_to_string-501"><a href="#data_to_string-501"><span class="linenos">501</span></a>
-</span><span id="data_to_string-502"><a href="#data_to_string-502"><span class="linenos">502</span></a><span class="sd">    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits</span>
-</span><span id="data_to_string-503"><a href="#data_to_string-503"><span class="linenos">503</span></a><span class="sd">    within the current terminal window without wrapping. If the column widths have reduced to 1</span>
-</span><span id="data_to_string-504"><a href="#data_to_string-504"><span class="linenos">504</span></a><span class="sd">    and the grid is still too wide, str(data) will be returned.&quot;&quot;&quot;</span>
-</span><span id="data_to_string-505"><a href="#data_to_string-505"><span class="linenos">505</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="data_to_string-506"><a href="#data_to_string-506"><span class="linenos">506</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="data_to_string-507"><a href="#data_to_string-507"><span class="linenos">507</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="data_to_string-508"><a href="#data_to_string-508"><span class="linenos">508</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="data_to_string-509"><a href="#data_to_string-509"><span class="linenos">509</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="data_to_string-510"><a href="#data_to_string-510"><span class="linenos">510</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="data_to_string-511"><a href="#data_to_string-511"><span class="linenos">511</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="data_to_string-512"><a href="#data_to_string-512"><span class="linenos">512</span></a>
-</span><span id="data_to_string-513"><a href="#data_to_string-513"><span class="linenos">513</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-514"><a href="#data_to_string-514"><span class="linenos">514</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="data_to_string-515"><a href="#data_to_string-515"><span class="linenos">515</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
-</span><span id="data_to_string-516"><a href="#data_to_string-516"><span class="linenos">516</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
-</span><span id="data_to_string-517"><a href="#data_to_string-517"><span class="linenos">517</span></a>    <span class="c1"># to see if shrinking is necessary</span>
-</span><span id="data_to_string-518"><a href="#data_to_string-518"><span class="linenos">518</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="data_to_string-519"><a href="#data_to_string-519"><span class="linenos">519</span></a>        <span class="n">data</span><span class="p">,</span>
-</span><span id="data_to_string-520"><a href="#data_to_string-520"><span class="linenos">520</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-521"><a href="#data_to_string-521"><span class="linenos">521</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="data_to_string-522"><a href="#data_to_string-522"><span class="linenos">522</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-523"><a href="#data_to_string-523"><span class="linenos">523</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="data_to_string-524"><a href="#data_to_string-524"><span class="linenos">524</span></a>    <span class="p">)</span>
-</span><span id="data_to_string-525"><a href="#data_to_string-525"><span class="linenos">525</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-526"><a href="#data_to_string-526"><span class="linenos">526</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-527"><a href="#data_to_string-527"><span class="linenos">527</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="data_to_string-528"><a href="#data_to_string-528"><span class="linenos">528</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="data_to_string-529"><a href="#data_to_string-529"><span class="linenos">529</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-530"><a href="#data_to_string-530"><span class="linenos">530</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="data_to_string-531"><a href="#data_to_string-531"><span class="linenos">531</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
-</span><span id="data_to_string-532"><a href="#data_to_string-532"><span class="linenos">532</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="data_to_string-533"><a href="#data_to_string-533"><span class="linenos">533</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-534"><a href="#data_to_string-534"><span class="linenos">534</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="data_to_string-535"><a href="#data_to_string-535"><span class="linenos">535</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
-</span><span id="data_to_string-536"><a href="#data_to_string-536"><span class="linenos">536</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-537"><a href="#data_to_string-537"><span class="linenos">537</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
-</span><span id="data_to_string-538"><a href="#data_to_string-538"><span class="linenos">538</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="data_to_string-539"><a href="#data_to_string-539"><span class="linenos">539</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
-</span><span id="data_to_string-540"><a href="#data_to_string-540"><span class="linenos">540</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
-</span><span id="data_to_string-541"><a href="#data_to_string-541"><span class="linenos">541</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
-</span><span id="data_to_string-542"><a href="#data_to_string-542"><span class="linenos">542</span></a>                <span class="p">)</span>
-</span><span id="data_to_string-543"><a href="#data_to_string-543"><span class="linenos">543</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="data_to_string-544"><a href="#data_to_string-544"><span class="linenos">544</span></a>                <span class="n">data</span><span class="p">,</span>
-</span><span id="data_to_string-545"><a href="#data_to_string-545"><span class="linenos">545</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-546"><a href="#data_to_string-546"><span class="linenos">546</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="data_to_string-547"><a href="#data_to_string-547"><span class="linenos">547</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-548"><a href="#data_to_string-548"><span class="linenos">548</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="data_to_string-549"><a href="#data_to_string-549"><span class="linenos">549</span></a>            <span class="p">)</span>
-</span><span id="data_to_string-550"><a href="#data_to_string-550"><span class="linenos">550</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-551"><a href="#data_to_string-551"><span class="linenos">551</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-552"><a href="#data_to_string-552"><span class="linenos">552</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="data_to_string-553"><a href="#data_to_string-553"><span class="linenos">553</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="data_to_string-554"><a href="#data_to_string-554"><span class="linenos">554</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-555"><a href="#data_to_string-555"><span class="linenos">555</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="data_to_string-556"><a href="#data_to_string-556"><span class="linenos">556</span></a>    <span class="k">return</span> <span class="n">output</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-504"><a href="#data_to_string-504"><span class="linenos">504</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="data_to_string-505"><a href="#data_to_string-505"><span class="linenos">505</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-506"><a href="#data_to_string-506"><span class="linenos">506</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="data_to_string-507"><a href="#data_to_string-507"><span class="linenos">507</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="data_to_string-508"><a href="#data_to_string-508"><span class="linenos">508</span></a>
+</span><span id="data_to_string-509"><a href="#data_to_string-509"><span class="linenos">509</span></a><span class="sd">    #### :params:</span>
+</span><span id="data_to_string-510"><a href="#data_to_string-510"><span class="linenos">510</span></a>
+</span><span id="data_to_string-511"><a href="#data_to_string-511"><span class="linenos">511</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="data_to_string-512"><a href="#data_to_string-512"><span class="linenos">512</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="data_to_string-513"><a href="#data_to_string-513"><span class="linenos">513</span></a>
+</span><span id="data_to_string-514"><a href="#data_to_string-514"><span class="linenos">514</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="data_to_string-515"><a href="#data_to_string-515"><span class="linenos">515</span></a>
+</span><span id="data_to_string-516"><a href="#data_to_string-516"><span class="linenos">516</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="data_to_string-517"><a href="#data_to_string-517"><span class="linenos">517</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="data_to_string-518"><a href="#data_to_string-518"><span class="linenos">518</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="data_to_string-519"><a href="#data_to_string-519"><span class="linenos">519</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="data_to_string-520"><a href="#data_to_string-520"><span class="linenos">520</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="data_to_string-521"><a href="#data_to_string-521"><span class="linenos">521</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="data_to_string-522"><a href="#data_to_string-522"><span class="linenos">522</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="data_to_string-523"><a href="#data_to_string-523"><span class="linenos">523</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="data_to_string-524"><a href="#data_to_string-524"><span class="linenos">524</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
+</span><span id="data_to_string-525"><a href="#data_to_string-525"><span class="linenos">525</span></a>
+</span><span id="data_to_string-526"><a href="#data_to_string-526"><span class="linenos">526</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-527"><a href="#data_to_string-527"><span class="linenos">527</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="data_to_string-528"><a href="#data_to_string-528"><span class="linenos">528</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
+</span><span id="data_to_string-529"><a href="#data_to_string-529"><span class="linenos">529</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
+</span><span id="data_to_string-530"><a href="#data_to_string-530"><span class="linenos">530</span></a>    <span class="c1"># to see if shrinking is necessary</span>
+</span><span id="data_to_string-531"><a href="#data_to_string-531"><span class="linenos">531</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="data_to_string-532"><a href="#data_to_string-532"><span class="linenos">532</span></a>        <span class="n">data</span><span class="p">,</span>
+</span><span id="data_to_string-533"><a href="#data_to_string-533"><span class="linenos">533</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-534"><a href="#data_to_string-534"><span class="linenos">534</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="data_to_string-535"><a href="#data_to_string-535"><span class="linenos">535</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-536"><a href="#data_to_string-536"><span class="linenos">536</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="data_to_string-537"><a href="#data_to_string-537"><span class="linenos">537</span></a>    <span class="p">)</span>
+</span><span id="data_to_string-538"><a href="#data_to_string-538"><span class="linenos">538</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-539"><a href="#data_to_string-539"><span class="linenos">539</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-540"><a href="#data_to_string-540"><span class="linenos">540</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="data_to_string-541"><a href="#data_to_string-541"><span class="linenos">541</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="data_to_string-542"><a href="#data_to_string-542"><span class="linenos">542</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-543"><a href="#data_to_string-543"><span class="linenos">543</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="data_to_string-544"><a href="#data_to_string-544"><span class="linenos">544</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
+</span><span id="data_to_string-545"><a href="#data_to_string-545"><span class="linenos">545</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="data_to_string-546"><a href="#data_to_string-546"><span class="linenos">546</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;=</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-547"><a href="#data_to_string-547"><span class="linenos">547</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="data_to_string-548"><a href="#data_to_string-548"><span class="linenos">548</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
+</span><span id="data_to_string-549"><a href="#data_to_string-549"><span class="linenos">549</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-550"><a href="#data_to_string-550"><span class="linenos">550</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
+</span><span id="data_to_string-551"><a href="#data_to_string-551"><span class="linenos">551</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="data_to_string-552"><a href="#data_to_string-552"><span class="linenos">552</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
+</span><span id="data_to_string-553"><a href="#data_to_string-553"><span class="linenos">553</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
+</span><span id="data_to_string-554"><a href="#data_to_string-554"><span class="linenos">554</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
+</span><span id="data_to_string-555"><a href="#data_to_string-555"><span class="linenos">555</span></a>                <span class="p">)</span>
+</span><span id="data_to_string-556"><a href="#data_to_string-556"><span class="linenos">556</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="data_to_string-557"><a href="#data_to_string-557"><span class="linenos">557</span></a>                <span class="n">data</span><span class="p">,</span>
+</span><span id="data_to_string-558"><a href="#data_to_string-558"><span class="linenos">558</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-559"><a href="#data_to_string-559"><span class="linenos">559</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="data_to_string-560"><a href="#data_to_string-560"><span class="linenos">560</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-561"><a href="#data_to_string-561"><span class="linenos">561</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="data_to_string-562"><a href="#data_to_string-562"><span class="linenos">562</span></a>            <span class="p">)</span>
+</span><span id="data_to_string-563"><a href="#data_to_string-563"><span class="linenos">563</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-564"><a href="#data_to_string-564"><span class="linenos">564</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-565"><a href="#data_to_string-565"><span class="linenos">565</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="data_to_string-566"><a href="#data_to_string-566"><span class="linenos">566</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="data_to_string-567"><a href="#data_to_string-567"><span class="linenos">567</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-568"><a href="#data_to_string-568"><span class="linenos">568</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="data_to_string-569"><a href="#data_to_string-569"><span class="linenos">569</span></a>    <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Use tabulate to produce grid output from a list of dictionaries.</p>
+            <div class="docstring"><p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>data</strong>:  Assumes all dictionaries in list have the same set of keys.</p></li>
-<li><p><strong>sort_key</strong>:  Optional dictionary key to sort data with.</p></li>
-<li><p><strong>wrap_to_terminal</strong>:  If True, the column widths will be reduced so the grid fits
-within the current terminal window without wrapping. If the column widths have reduced to 1
-and the grid is still too wide, str(data) will be returned.</p></li>
-</ul>
+<p><code>data</code>: The list of dictionaries to create a grid from.
+Assumes all dictionaries in list have the same set of keys.</p>
+
+<p><code>sort_key</code>: Optional dictionary key to sort data with.</p>
+
+<p><code>wrap_to_terminal</code>: If <code>True</code>, the table width will be wrapped to fit within the current terminal window.
+Pass as <code>False</code> if the output is going into something like a <code>.txt</code> file.</p>
 </div>
 
 
                 </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -62,587 +62,23 @@
 _33    def __init__(
 _34        self,
 _35        dbpath: str | Pathier,
 _36        logger_encoding: str = "utf-8",
 _37        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
 _38    ):
 _39        """
-_40        :param dbpath: String or Path object to database file.
-_41        If a relative path is given, it will be relative to the
-_42        current working directory. The log file will be saved to the
-_43        same directory.
-_44
-_45        :param logger_message_format: '{' style format string
-_46        for the logger object."""
-_47        self.dbpath = Pathier(dbpath)
-_48        self.dbname = Pathier(dbpath).name
-_49        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
-_50        self._logger_init(
-_51            encoding=logger_encoding, message_format=logger_message_format
-_52        )
-_53        self.connection_open = False
-_54
-_55    def __enter__(self):
-_56        self.open()
-_57        return self
-_58
-_59    def __exit__(self, exception_type, exception_value,
-exception_traceback):
-_60        self.close()
-_61
-_62    def open(self):
-_63        """Open connection to db."""
-_64        self.connection = sqlite3.connect(
-_65            self.dbpath,
-_66            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-_67            timeout=10,
-_68        )
-_69        self.connection.execute("pragma foreign_keys = 1")
-_70        self.cursor = self.connection.cursor()
-_71        self.connection_open = True
-_72
-_73    def close(self):
-_74        """Save and close connection to db.
-_75
-_76        Call this as soon as you are done using the database if you have
-_77        multiple threads or processes using the same database."""
-_78        if self.connection_open:
-_79            self.connection.commit()
-_80            self.connection.close()
-_81            self.connection_open = False
-_82
-_83    def _logger_init(
-_84        self,
-_85        message_format: str = "{levelname}|-|{asctime}|-|{message}",
-_86        encoding: str = "utf-8",
-_87    ):
-_88        """:param message_format: '{' style format string"""
-_89        self.logger = logging.getLogger(self.dbname)
-_90        if not self.logger.hasHandlers():
-_91            handler = logging.FileHandler(
-_92                str(self.dbpath).replace(".", "") + ".log",
-encoding=encoding
-_93            )
-_94            handler.setFormatter(
-_95                logging.Formatter(
-_96                    message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S
-%p"
-_97                )
-_98            )
-_99            self.logger.addHandler(handler)
-100            self.logger.setLevel(logging.INFO)
-101
-102    def _get_dict(
-103        self, table: str, values: list, columns_to_return: list[str] | None
-= None
-104    ) -> dict:
-105        """Converts the values of a row into a dictionary with column names
-as keys.
-106
-107        :param table: The table that values were pulled from.
-108
-109        :param values: List of values expected to be the same quantity
-110        and in the same order as the column names of table.
-111
-112        :param columns_to_return: An optional list of column names.
-113        If given, only these columns will be included in the returned
-dictionary.
-114        Otherwise all columns and values are returned."""
-115        return {
-116            column: value
-117            for column, value in zip(self.get_column_names(table), values)
-118            if not columns_to_return or column in columns_to_return
-119        }
-120
-121    def _get_conditions(
-122        self, match_criteria: list[tuple] | dict, exact_match: bool = True
-123    ) -> str:
-124        """Builds and returns the conditional portion of a query.
-125
-126        :param match_criteria: Can be a list of 2-tuples where each
-127        tuple is (columnName, rowValue) or a dictionary where
-128        keys are column names and values are row values.
-129
-130        :param exact_match: If False, the rowValue for a give column
-131        will be matched as a substring.
-132
-133        Usage e.g.:
-134
-135        self.cursor.execute(f'select * from {table} where {conditions}')"""
-136        if type(match_criteria) == dict:
-137            match_criteria = [(k, v) for k, v in match_criteria.items()]
-138        if exact_match:
-139            conditions = " and ".join(
-140                f'"{column_row[0]}" = "{column_row[1]}"'
-141                for column_row in match_criteria
-142            )
-143        else:
-144            conditions = " and ".join(
-145                f'"{column_row[0]}" like "%{column_row[1]}%"'
-146                for column_row in match_criteria
-147            )
-148        return f"({conditions})"
-149
-150    @_connect
-151    def query(self, query_) -> list[Any]:
-152        """Execute an arbitrary query and
-153        return the results."""
-154        self.cursor.execute(query_)
-155        return self.cursor.fetchall()
-156
-157    @_connect
-158    def create_tables(self, table_querys: list[str] = []):
-159        """Create tables if they don't exist.
-160
-161        :param table_querys: Each query should be
-162        in the form 'tableName(columnDefinitions)'"""
-163        if len(table_querys) > 0:
-164            table_names = self.get_table_names()
-165            for table in table_querys:
-166                if table.split("(")[0].strip() not in table_names:
-167                    self.cursor.execute(f"create table {table}")
-168                    self.logger.info(f'{table.split("(")[0]} table
-created.')
-169
-170    @_connect
-171    def create_table(self, table: str, column_defs: list[str]):
-172        """Create a table if it doesn't exist.
-173
-174        :param table: Name of the table to create.
-175
-176        :param column_defs: List of column definitions in
-177        proper Sqlite3 sytax.
-178        i.e. "columnName text unique" or "columnName int primary key"
-etc."""
-179        if table not in self.get_table_names():
-180            query = f"create table {table}({', '.join(column_defs)})"
-181            self.cursor.execute(query)
-182            self.logger.info(f"'{table}' table created.")
-183
-184    @_connect
-185    def get_table_names(self) -> list[str]:
-186        """Returns a list of table names from database."""
-187        self.cursor.execute(
-188            'select name from sqlite_Schema where type = "table" and name
-not like "sqlite_%"'
-189        )
-190        return [result[0] for result in self.cursor.fetchall()]
-191
-192    @_connect
-193    def get_column_names(self, table: str) -> list[str]:
-194        """Return a list of column names from a table."""
-195        self.cursor.execute(f"select * from {table} where 1=0")
-196        return [description[0] for description in self.cursor.description]
-197
-198    @_connect
-199    def count(
-200        self,
-201        table: str,
-202        match_criteria: list[tuple] | dict | None = None,
-203        exact_match: bool = True,
-204    ) -> int:
-205        """Return number of items in table.
-206
-207        :param match_criteria: Can be a list of 2-tuples where each
-208        tuple is (columnName, rowValue) or a dictionary where
-209        keys are column names and values are row values.
-210        If None, all rows from the table will be counted.
-211
-212        :param exact_match: If False, the row value for a give column
-213        in match_criteria will be matched as a substring. Has no effect if
-214        match_criteria is None.
-215        """
-216        query = f"select count(_rowid_) from {table}"
-217        try:
-218            if match_criteria:
-219                self.cursor.execute(
-220                    f"{query} where {self._get_conditions(match_criteria,
-exact_match)}"
-221                )
-222            else:
-223                self.cursor.execute(f"{query}")
-224            return self.cursor.fetchone()[0]
-225        except:
-226            return 0
-227
-228    @_connect
-229    def add_row(
-230        self, table: str, values: tuple[Any], columns: tuple[str] | None =
-None
-231    ):
-232        """Add row of values to table.
-233
-234        :param table: The table to insert into.
-235
-236        :param values: A tuple of values to be inserted into the table.
-237
-238        :param columns: If None, values param is expected to supply
-239        a value for every column in the table. If columns is
-240        provided, it should contain the same number of elements as
-values."""
-241        parameterizer = ", ".join("?" for _ in values)
-242        logger_values = ", ".join(str(value) for value in values)
-243        try:
-244            if columns:
-245                columns_query = ", ".join(column for column in columns)
-246                self.cursor.execute(
-247                    f"insert into {table} ({columns_query}) values(
-{parameterizer})",
-248                    values,
-249                )
-250            else:
-251                self.cursor.execute(
-252                    f"insert into {table} values({parameterizer})", values
-253                )
-254            self.logger.info(f'Added "{logger_values}" to {table} table.')
-255        except Exception as e:
-256            if "constraint" not in str(e).lower():
-257                self.logger.exception(
-258                    f'Error adding "{logger_values}" to {table} table.'
-259                )
-260            else:
-261                self.logger.debug(str(e))
-262
-263    @_connect
-264    def get_rows(
-265        self,
-266        table: str,
-267        match_criteria: list[tuple] | dict | None = None,
-268        exact_match: bool = True,
-269        sort_by_column: str | None = None,
-270        columns_to_return: list[str] | None = None,
-271        return_as_dataframe: bool = False,
-272        values_only: bool = False,
-273        order_by: str | None = None,
-274        limit: str | int | None = None,
-275    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-276        """Returns rows from table as a list of dictionaries
-277        where the key-value pairs of the dictionaries are
-278        column name: row value.
-279
-280        :param match_criteria: Can be a list of 2-tuples where each
-281        tuple is (columnName, rowValue) or a dictionary where
-282        keys are column names and values are row values.
-283
-284        :param exact_match: If False, the rowValue for a give column
-285        will be matched as a substring.
-286
-287        :param sort_by_column: A column name to sort the results by.
-288        This will sort results in Python after retrieving them from the db.
-289        Use the 'order_by' param to use SQLite engine for ordering.
-290
-291        :param columns_to_return: Optional list of column names.
-292        If provided, the elements returned by get_rows() will
-293        only contain the provided columns. Otherwise every column
-294        in the row is returned.
-295
-296        :param return_as_dataframe: If True,
-297        the results will be returned as a pandas.DataFrame object.
-298
-299        :param values_only: Return the results as a list of tuples
-300        instead of a list of dictionaries that have column names as keys.
-301        The results will still be sorted according to sort_by_column if
-302        one is provided.
-303
-304        :param order_by: If given, a 'order by {order_by}' clause
-305        will be added to the select query.
-306
-307        :param limit: If given, a 'limit {limit}' clause will be
-308        added to the select query.
-309        """
-310
-311        if type(columns_to_return) is str:
-312            columns_to_return = [columns_to_return]
-313        query = f"select * from {table}"
-314        matches = []
-315        if match_criteria:
-316            query += f" where {self._get_conditions(match_criteria,
-exact_match)}"
-317        if order_by:
-318            query += f" order by {order_by}"
-319        if limit:
-320            query += f" limit {limit}"
-321        query += ";"
-322        self.cursor.execute(query)
-323        matches = self.cursor.fetchall()
-324        results = [self._get_dict(table, match, columns_to_return) for match
-in matches]
-325        if sort_by_column:
-326            results = sorted(results, key=lambda x: x[sort_by_column])
-327        if return_as_dataframe:
-328            return pandas.DataFrame(results)
-329        if values_only:
-330            return [tuple(row.values()) for row in results]
-331        else:
-332            return results
-333
-334    @_connect
-335    def find(
-336        self, table: str, query_string: str, columns: list[str] | None =
-None
-337    ) -> list[dict]:
-338        """Search for rows that contain query_string as a substring
-339        of any column.
-340
-341        :param table: The table to search.
-342
-343        :param query_string: The substring to search for in all columns.
-344
-345        :param columns: A list of columns to search for query_string.
-346        If None, all columns in the table will be searched.
-347        """
-348        if type(columns) is str:
-349            columns = [columns]
-350        results = []
-351        if not columns:
-352            columns = self.get_column_names(table)
-353        for column in columns:
-354            results.extend(
-355                [
-356                    row
-357                    for row in self.get_rows(
-358                        table, [(column, query_string)], exact_match=False
-359                    )
-360                    if row not in results
-361                ]
-362            )
-363        return results
-364
-365    @_connect
-366    def delete(
-367        self, table: str, match_criteria: list[tuple] | dict, exact_match:
-bool = True
-368    ) -> int:
-369        """Delete records from table.
-370
-371        Returns number of deleted records.
-372
-373        :param match_criteria: Can be a list of 2-tuples where each
-374        tuple is (columnName, rowValue) or a dictionary where
-375        keys are column names and values are row values.
-376
-377        :param exact_match: If False, the rowValue for a give column
-378        will be matched as a substring.
-379        """
-380        num_matches = self.count(table, match_criteria, exact_match)
-381        conditions = self._get_conditions(match_criteria, exact_match)
-382        try:
-383            self.cursor.execute(f"delete from {table} where {conditions}")
-384            self.logger.info(
-385                f'Deleted {num_matches} from "{table}" where {conditions}".'
-386            )
-387            return num_matches
-388        except Exception as e:
-389            self.logger.debug(f'Error deleting from "{table}" where
-{conditions}.\n{e}')
-390            return 0
-391
-392    @_connect
-393    def update(
-394        self,
-395        table: str,
-396        column_to_update: str,
-397        new_value: Any,
-398        match_criteria: list[tuple] | dict | None = None,
-399    ) -> bool:
-400        """Update row value for entry matched with match_criteria.
-401
-402        :param column_to_update: The column to be updated in the matched
-row.
-403
-404        :param new_value: The new value to insert.
-405
-406        :param match_criteria: Can be a list of 2-tuples where each
-407        tuple is (columnName, rowValue) or a dictionary where
-408        keys are column names and values are row values.
-409        If None, every row will be updated.
-410
-411        Returns True if successful, False if not."""
-412        query = f"update {table} set {column_to_update} = ?"
-413        conditions = ""
-414        if match_criteria:
-415            if self.count(table, match_criteria) == 0:
-416                self.logger.info(
-417                    f"Couldn't find matching records in {table} table to
-update to '{new_value}'"
-418                )
-419                return False
-420            conditions = self._get_conditions(match_criteria)
-421            query += f" where {conditions}"
-422        else:
-423            conditions = None
-424        try:
-425            self.cursor.execute(
-426                query,
-427                (new_value,),
-428            )
-429            self.logger.info(
-430                f'Updated "{column_to_update}" in "{table}" table to "
-{new_value}" where {conditions}'
-431            )
-432            return True
-433        except Exception as e:
-434            self.logger.error(
-435                f'Failed to update "{column_to_update}" in "{table}" table
-to "{new_value}" where {conditions}"\n{e}'
-436            )
-437            return False
-438
-439    @_connect
-440    def drop_table(self, table: str) -> bool:
-441        """Drop a table from the database.
-442
-443        Returns True if successful, False if not."""
-444        try:
-445            self.cursor.execute(f"drop Table {table}")
-446            self.logger.info(f'Dropped table "{table}"')
-447            return True
-448        except Exception as e:
-449            print(e)
-450            self.logger.error(f'Failed to drop table "{table}"')
-451            return False
-452
-453    @_connect
-454    def add_column(
-455        self, table: str, column: str, _type: str, default_value: str | None
-= None
-456    ):
-457        """Add a new column to table.
-458
-459        :param column: Name of the column to add.
-460
-461        :param _type: The data type of the new column.
-462
-463        :param default_value: Optional default value for the column."""
-464        try:
-465            if default_value:
-466                self.cursor.execute(
-467                    f"alter table {table} add column {column} {_type}
-default {default_value}"
-468                )
-469            else:
-470                self.cursor.execute(f"alter table {table} add column
-{column} {_type}")
-471            self.logger.info(f'Added column "{column}" to "{table}" table.')
-472        except Exception as e:
-473            self.logger.error(f'Failed to add column "{column}" to "{table}"
-table.')
-474
-475    @staticmethod
-476    def data_to_string(
-477        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
-bool = True
-478    ) -> str:
-479        """Uses tabulate to produce pretty string output
-480        from a list of dictionaries.
-481
-482        :param data: Assumes all dictionaries in list have the same set of
-keys.
-483
-484        :param sort_key: Optional dictionary key to sort data with.
-485
-486        :param wrap_to_terminal: If True, the table width will be wrapped
-487        to fit within the current terminal window. Set to False
-488        if the output is going into something like a txt file."""
-489        return data_to_string(data, sort_key, wrap_to_terminal)
-490
-491
-492def data_to_string(
-493    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
-True
-494) -> str:
-495    """Use tabulate to produce grid output from a list of dictionaries.
-496
-497    :param data: Assumes all dictionaries in list have the same set of keys.
-498
-499    :param sort_key: Optional dictionary key to sort data with.
-500
-501    :param wrap_to_terminal: If True, the column widths will be reduced so
-the grid fits
-502    within the current terminal window without wrapping. If the column
-widths have reduced to 1
-503    and the grid is still too wide, str(data) will be returned."""
-504    if len(data) == 0:
-505        return ""
-506    if sort_key:
-507        data = sorted(data, key=lambda d: d[sort_key])
-508    for i, d in enumerate(data):
-509        for k in d:
-510            data[i][k] = str(data[i][k])
-511
-512    too_wide = True
-513    terminal_width = os.get_terminal_size().columns
-514    max_col_widths = terminal_width
-515    # Make an output with effectively unrestricted column widths
-516    # to see if shrinking is necessary
-517    output = tabulate(
-518        data,
-519        headers="keys",
-520        disable_numparse=True,
-521        tablefmt="grid",
-522        maxcolwidths=max_col_widths,
-523    )
-524    current_width = output.index("\n")
-525    if current_width < terminal_width:
-526        too_wide = False
-527    if wrap_to_terminal and too_wide:
-528        print("Resizing grid to fit within the terminal...")
-529        previous_col_widths = max_col_widths
-530        acceptable_width = terminal_width - 10
-531        while too_wide and max_col_widths > 1:
-532            if current_width > terminal_width:
-533                previous_col_widths = max_col_widths
-534                max_col_widths = int(max_col_widths * 0.5)
-535            elif current_width < terminal_width:
-536                # Without lowering acceptable_width, this condition will
-cause infinite loop
-537                if max_col_widths == previous_col_widths - 1:
-538                    acceptable_width -= 10
-539                max_col_widths = int(
-540                    max_col_widths + (0.5 * (previous_col_widths -
-max_col_widths))
-541                )
-542            output = tabulate(
-543                data,
-544                headers="keys",
-545                disable_numparse=True,
-546                tablefmt="grid",
-547                maxcolwidths=max_col_widths,
-548            )
-549            current_width = output.index("\n")
-550            if acceptable_width < current_width < terminal_width:
-551                too_wide = False
-552        if too_wide:
-553            print("Couldn't resize grid to fit within the terminal.")
-554            return str(data)
-555    return output
-  ⁰
-class DataBased: View Source
-_27class DataBased:
-_28    """Sqli wrapper so queries don't need to be written except table
-definitions.
-_29
-_30    Supports saving and reading dates as datetime objects.
-_31
-_32    Supports using a context manager."""
-_33
-_34    def __init__(
-_35        self,
-_36        dbpath: str | Pathier,
-_37        logger_encoding: str = "utf-8",
-_38        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
-_39    ):
-_40        """
-_41        :param dbpath: String or Path object to database file.
-_42        If a relative path is given, it will be relative to the
-_43        current working directory. The log file will be saved to the
-_44        same directory.
-_45
-_46        :param logger_message_format: '{' style format string
-_47        for the logger object."""
+_40        #### :params:
+_41
+_42        `dbpath`: String or Path object to database file.
+_43        If a relative path is given, it will be relative to the
+_44        current working directory. The log file will be saved to the
+_45        same directory.
+_46
+_47        `logger_message_format`: '{' style format string for the logger
+object."""
 _48        self.dbpath = Pathier(dbpath)
 _49        self.dbname = Pathier(dbpath).name
 _50        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
 _51        self._logger_init(
 _52            encoding=logger_encoding, message_format=logger_message_format
 _53        )
 _54        self.connection_open = False
@@ -658,15 +94,15 @@
 _63    def open(self):
 _64        """Open connection to db."""
 _65        self.connection = sqlite3.connect(
 _66            self.dbpath,
 _67            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
 _68            timeout=10,
 _69        )
-_70        self.connection.execute("pragma foreign_keys = 1")
+_70        self.connection.execute("pragma foreign_keys = 1;")
 _71        self.cursor = self.connection.cursor()
 _72        self.connection_open = True
 _73
 _74    def close(self):
 _75        """Save and close connection to db.
 _76
 _77        Call this as soon as you are done using the database if you have
@@ -677,15 +113,15 @@
 _82            self.connection_open = False
 _83
 _84    def _logger_init(
 _85        self,
 _86        message_format: str = "{levelname}|-|{asctime}|-|{message}",
 _87        encoding: str = "utf-8",
 _88    ):
-_89        """:param message_format: '{' style format string"""
+_89        """:param `message_format`: '{' style format string"""
 _90        self.logger = logging.getLogger(self.dbname)
 _91        if not self.logger.hasHandlers():
 _92            handler = logging.FileHandler(
 _93                str(self.dbpath).replace(".", "") + ".log",
 encoding=encoding
 _94            )
 _95            handler.setFormatter(
@@ -700,420 +136,1045 @@
 103    def _get_dict(
 104        self, table: str, values: list, columns_to_return: list[str] | None
 = None
 105    ) -> dict:
 106        """Converts the values of a row into a dictionary with column names
 as keys.
 107
-108        :param table: The table that values were pulled from.
+108        #### :params:
 109
-110        :param values: List of values expected to be the same quantity
-111        and in the same order as the column names of table.
-112
-113        :param columns_to_return: An optional list of column names.
-114        If given, only these columns will be included in the returned
+110        `table`: The table that values were pulled from.
+111
+112        `values`: List of values expected to be the same quantity
+113        and in the same order as the column names of table.
+114
+115        `columns_to_return`: An optional list of column names.
+116        If given, only these columns will be included in the returned
 dictionary.
-115        Otherwise all columns and values are returned."""
-116        return {
-117            column: value
-118            for column, value in zip(self.get_column_names(table), values)
-119            if not columns_to_return or column in columns_to_return
-120        }
-121
-122    def _get_conditions(
-123        self, match_criteria: list[tuple] | dict, exact_match: bool = True
-124    ) -> str:
-125        """Builds and returns the conditional portion of a query.
-126
-127        :param match_criteria: Can be a list of 2-tuples where each
-128        tuple is (columnName, rowValue) or a dictionary where
-129        keys are column names and values are row values.
+117        Otherwise all columns and values are returned."""
+118        return {
+119            column: value
+120            for column, value in zip(self.get_column_names(table), values)
+121            if not columns_to_return or column in columns_to_return
+122        }
+123
+124    def _get_conditions(
+125        self, match_criteria: list[tuple] | dict, exact_match: bool = True
+126    ) -> str:
+127        """Builds and returns the conditional portion of a query.
+128
+129        #### :params:
 130
-131        :param exact_match: If False, the rowValue for a give column
-132        will be matched as a substring.
-133
-134        Usage e.g.:
-135
-136        self.cursor.execute(f'select * from {table} where {conditions}')"""
-137        if type(match_criteria) == dict:
-138            match_criteria = [(k, v) for k, v in match_criteria.items()]
-139        if exact_match:
-140            conditions = " and ".join(
-141                f'"{column_row[0]}" = "{column_row[1]}"'
-142                for column_row in match_criteria
-143            )
-144        else:
-145            conditions = " and ".join(
-146                f'"{column_row[0]}" like "%{column_row[1]}%"'
-147                for column_row in match_criteria
-148            )
-149        return f"({conditions})"
-150
-151    @_connect
-152    def query(self, query_) -> list[Any]:
-153        """Execute an arbitrary query and
-154        return the results."""
-155        self.cursor.execute(query_)
-156        return self.cursor.fetchall()
-157
-158    @_connect
-159    def create_tables(self, table_querys: list[str] = []):
-160        """Create tables if they don't exist.
-161
-162        :param table_querys: Each query should be
-163        in the form 'tableName(columnDefinitions)'"""
-164        if len(table_querys) > 0:
-165            table_names = self.get_table_names()
-166            for table in table_querys:
-167                if table.split("(")[0].strip() not in table_names:
-168                    self.cursor.execute(f"create table {table}")
-169                    self.logger.info(f'{table.split("(")[0]} table
+131        `match_criteria`: Can be a list of 2-tuples where each
+132        tuple is `(columnName, rowValue)` or a dictionary where
+133        keys are column names and values are row values.
+134
+135        `exact_match`: If `False`, the row value for a given column
+136        will be matched as a substring.
+137
+138        Usage e.g.:
+139
+140        >>> self.cursor.execute(f'select * from {table} where
+{conditions};')"""
+141        if type(match_criteria) == dict:
+142            match_criteria = [(k, v) for k, v in match_criteria.items()]
+143        if exact_match:
+144            conditions = " and ".join(
+145                f'"{column_row[0]}" = "{column_row[1]}"'
+146                for column_row in match_criteria
+147            )
+148        else:
+149            conditions = " and ".join(
+150                f'"{column_row[0]}" like "%{column_row[1]}%"'
+151                for column_row in match_criteria
+152            )
+153        return f"({conditions})"
+154
+155    @_connect
+156    def query(self, query_) -> list[Any]:
+157        """Execute an arbitrary query and return the results."""
+158        self.cursor.execute(query_)
+159        return self.cursor.fetchall()
+160
+161    @_connect
+162    def create_tables(self, table_defs: list[str] = []):
+163        """Create tables if they don't exist.
+164
+165        :param `table_defs`: Each definition should be in the form
+`table_name(column_definitions)`"""
+166        if len(table_defs) > 0:
+167            table_names = self.get_table_names()
+168            for table in table_defs:
+169                if table.split("(")[0].strip() not in table_names:
+170                    self.cursor.execute(f"create table {table};")
+171                    self.logger.info(f'{table.split("(")[0]} table
 created.')
-170
-171    @_connect
-172    def create_table(self, table: str, column_defs: list[str]):
-173        """Create a table if it doesn't exist.
-174
-175        :param table: Name of the table to create.
+172
+173    @_connect
+174    def create_table(self, table: str, column_defs: list[str]):
+175        """Create a table if it doesn't exist.
 176
-177        :param column_defs: List of column definitions in
-178        proper Sqlite3 sytax.
-179        i.e. "columnName text unique" or "columnName int primary key"
+177        #### :params:
+178
+179        `table`: Name of the table to create.
+180
+181        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+182        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
-180        if table not in self.get_table_names():
-181            query = f"create table {table}({', '.join(column_defs)})"
-182            self.cursor.execute(query)
-183            self.logger.info(f"'{table}' table created.")
-184
-185    @_connect
-186    def get_table_names(self) -> list[str]:
-187        """Returns a list of table names from database."""
-188        self.cursor.execute(
-189            'select name from sqlite_Schema where type = "table" and name
-not like "sqlite_%"'
-190        )
-191        return [result[0] for result in self.cursor.fetchall()]
-192
-193    @_connect
-194    def get_column_names(self, table: str) -> list[str]:
-195        """Return a list of column names from a table."""
-196        self.cursor.execute(f"select * from {table} where 1=0")
-197        return [description[0] for description in self.cursor.description]
-198
-199    @_connect
-200    def count(
-201        self,
-202        table: str,
-203        match_criteria: list[tuple] | dict | None = None,
-204        exact_match: bool = True,
-205    ) -> int:
-206        """Return number of items in table.
-207
-208        :param match_criteria: Can be a list of 2-tuples where each
-209        tuple is (columnName, rowValue) or a dictionary where
-210        keys are column names and values are row values.
-211        If None, all rows from the table will be counted.
+183        if table not in self.get_table_names():
+184            query = f"create table {table}({', '.join(column_defs)});"
+185            self.cursor.execute(query)
+186            self.logger.info(f"'{table}' table created.")
+187
+188    @_connect
+189    def get_table_names(self) -> list[str]:
+190        """Returns a list of table names from the database."""
+191        self.cursor.execute(
+192            'select name from sqlite_Schema where type = "table" and name
+not like "sqlite_%";'
+193        )
+194        return [result[0] for result in self.cursor.fetchall()]
+195
+196    @_connect
+197    def get_column_names(self, table: str) -> list[str]:
+198        """Return a list of column names from a table."""
+199        self.cursor.execute(f"select * from {table} where 1=0")
+200        return [description[0] for description in self.cursor.description]
+201
+202    @_connect
+203    def count(
+204        self,
+205        table: str,
+206        match_criteria: list[tuple] | dict | None = None,
+207        exact_match: bool = True,
+208    ) -> int:
+209        """Return number of items in `table`.
+210
+211        #### :params:
 212
-213        :param exact_match: If False, the row value for a give column
-214        in match_criteria will be matched as a substring. Has no effect if
-215        match_criteria is None.
-216        """
-217        query = f"select count(_rowid_) from {table}"
-218        try:
-219            if match_criteria:
-220                self.cursor.execute(
-221                    f"{query} where {self._get_conditions(match_criteria,
-exact_match)}"
-222                )
-223            else:
-224                self.cursor.execute(f"{query}")
-225            return self.cursor.fetchone()[0]
-226        except:
-227            return 0
-228
-229    @_connect
-230    def add_row(
-231        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+213        `match_criteria`: Can be a list of 2-tuples where each
+214        tuple is `(columnName, rowValue)` or a dictionary where
+215        keys are column names and values are row values.
+216        If `None`, all rows from the table will be counted.
+217
+218        `exact_match`: If `False`, the row value for a given column
+219        in `match_criteria` will be matched as a substring.
+220        Has no effect if `match_criteria` is `None`.
+221        """
+222        query = f"select count(_rowid_) from {table}"
+223        try:
+224            if match_criteria:
+225                self.cursor.execute(
+226                    f"{query} where {self._get_conditions(match_criteria,
+exact_match)};"
+227                )
+228            else:
+229                self.cursor.execute(f"{query}")
+230            return self.cursor.fetchone()[0]
+231        except:
+232            return 0
+233
+234    @_connect
+235    def add_row(
+236        self, table: str, values: tuple[Any], columns: tuple[str] | None =
 None
-232    ):
-233        """Add row of values to table.
-234
-235        :param table: The table to insert into.
-236
-237        :param values: A tuple of values to be inserted into the table.
-238
-239        :param columns: If None, values param is expected to supply
-240        a value for every column in the table. If columns is
-241        provided, it should contain the same number of elements as
-values."""
-242        parameterizer = ", ".join("?" for _ in values)
-243        logger_values = ", ".join(str(value) for value in values)
-244        try:
-245            if columns:
-246                columns_query = ", ".join(column for column in columns)
-247                self.cursor.execute(
-248                    f"insert into {table} ({columns_query}) values(
-{parameterizer})",
-249                    values,
-250                )
-251            else:
-252                self.cursor.execute(
-253                    f"insert into {table} values({parameterizer})", values
-254                )
-255            self.logger.info(f'Added "{logger_values}" to {table} table.')
-256        except Exception as e:
-257            if "constraint" not in str(e).lower():
-258                self.logger.exception(
-259                    f'Error adding "{logger_values}" to {table} table.'
+237    ):
+238        """Add a row of values to a table.
+239
+240        #### :params:
+241
+242        `table`: The table to insert values into.
+243
+244        `values`: A tuple of values to be inserted into the table.
+245
+246        `columns`: If `None`, `values` is expected to supply a value for
+every column in the table.
+247        If `columns` is provided, it should contain the same number of
+elements as `values`."""
+248        parameterizer = ", ".join("?" for _ in values)
+249        logger_values = ", ".join(str(value) for value in values)
+250        try:
+251            if columns:
+252                columns_query = ", ".join(column for column in columns)
+253                self.cursor.execute(
+254                    f"insert into {table} ({columns_query}) values(
+{parameterizer});",
+255                    values,
+256                )
+257            else:
+258                self.cursor.execute(
+259                    f"insert into {table} values({parameterizer});", values
 260                )
-261            else:
-262                self.logger.debug(str(e))
-263
-264    @_connect
-265    def get_rows(
-266        self,
-267        table: str,
-268        match_criteria: list[tuple] | dict | None = None,
-269        exact_match: bool = True,
-270        sort_by_column: str | None = None,
-271        columns_to_return: list[str] | None = None,
-272        return_as_dataframe: bool = False,
-273        values_only: bool = False,
-274        order_by: str | None = None,
-275        limit: str | int | None = None,
-276    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-277        """Returns rows from table as a list of dictionaries
-278        where the key-value pairs of the dictionaries are
-279        column name: row value.
-280
-281        :param match_criteria: Can be a list of 2-tuples where each
-282        tuple is (columnName, rowValue) or a dictionary where
-283        keys are column names and values are row values.
+261            self.logger.info(f'Added "{logger_values}" to {table} table.')
+262        except Exception as e:
+263            if "constraint" not in str(e).lower():
+264                self.logger.exception(
+265                    f'Error adding "{logger_values}" to {table} table.'
+266                )
+267            else:
+268                self.logger.debug(str(e))
+269
+270    @_connect
+271    def get_rows(
+272        self,
+273        table: str,
+274        match_criteria: list[tuple] | dict | None = None,
+275        exact_match: bool = True,
+276        sort_by_column: str | None = None,
+277        columns_to_return: list[str] | None = None,
+278        return_as_dataframe: bool = False,
+279        values_only: bool = False,
+280        order_by: str | None = None,
+281        limit: str | int | None = None,
+282    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+283        """Return matching rows from `table`.
 284
-285        :param exact_match: If False, the rowValue for a give column
-286        will be matched as a substring.
+285        By default, rows will be returned as a list of dictionaries of the
+form `[{"column_name": value, ...}, ...]`
+286
 287
-288        :param sort_by_column: A column name to sort the results by.
-289        This will sort results in Python after retrieving them from the db.
-290        Use the 'order_by' param to use SQLite engine for ordering.
-291
-292        :param columns_to_return: Optional list of column names.
-293        If provided, the elements returned by get_rows() will
-294        only contain the provided columns. Otherwise every column
-295        in the row is returned.
-296
-297        :param return_as_dataframe: If True,
-298        the results will be returned as a pandas.DataFrame object.
+288        #### :params:
+289
+290        `match_criteria`: Can be a list of 2-tuples where each
+291        tuple is `(columnName, rowValue)` or a dictionary where
+292        keys are column names and values are row values.
+293
+294        `exact_match`: If `False`, the row value for a given column will be
+matched as a substring.
+295
+296        `sort_by_column`: A column name to sort the results by.
+297        This will sort results in Python after retrieving them from the db.
+298        Use the 'order_by' param to use SQLite engine for ordering.
 299
-300        :param values_only: Return the results as a list of tuples
-301        instead of a list of dictionaries that have column names as keys.
-302        The results will still be sorted according to sort_by_column if
-303        one is provided.
-304
-305        :param order_by: If given, a 'order by {order_by}' clause
-306        will be added to the select query.
+300        `columns_to_return`: Optional list of column names.
+301        If provided, the elements returned by this function will only
+contain the provided columns.
+302        Otherwise every column in the row is returned.
+303
+304        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
+object.
+305
+306        `values_only`: Return the results as a list of tuples.
 307
-308        :param limit: If given, a 'limit {limit}' clause will be
-309        added to the select query.
-310        """
-311
-312        if type(columns_to_return) is str:
-313            columns_to_return = [columns_to_return]
-314        query = f"select * from {table}"
-315        matches = []
-316        if match_criteria:
-317            query += f" where {self._get_conditions(match_criteria,
+308        `order_by`: If given, a `order by {order_by}` clause will be added
+to the select query.
+309
+310        `limit`: If given, a `limit {limit}` clause will be added to the
+select query.
+311        """
+312
+313        if type(columns_to_return) is str:
+314            columns_to_return = [columns_to_return]
+315        query = f"select * from {table}"
+316        matches = []
+317        if match_criteria:
+318            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-318        if order_by:
-319            query += f" order by {order_by}"
-320        if limit:
-321            query += f" limit {limit}"
-322        query += ";"
-323        self.cursor.execute(query)
-324        matches = self.cursor.fetchall()
-325        results = [self._get_dict(table, match, columns_to_return) for match
+319        if order_by:
+320            query += f" order by {order_by}"
+321        if limit:
+322            query += f" limit {limit}"
+323        query += ";"
+324        self.cursor.execute(query)
+325        matches = self.cursor.fetchall()
+326        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-326        if sort_by_column:
-327            results = sorted(results, key=lambda x: x[sort_by_column])
-328        if return_as_dataframe:
-329            return pandas.DataFrame(results)
-330        if values_only:
-331            return [tuple(row.values()) for row in results]
-332        else:
-333            return results
-334
-335    @_connect
-336    def find(
-337        self, table: str, query_string: str, columns: list[str] | None =
+327        if sort_by_column:
+328            results = sorted(results, key=lambda x: x[sort_by_column])
+329        if return_as_dataframe:
+330            return pandas.DataFrame(results)
+331        if values_only:
+332            return [tuple(row.values()) for row in results]
+333        else:
+334            return results
+335
+336    @_connect
+337    def find(
+338        self, table: str, query_string: str, columns: list[str] | None =
 None
-338    ) -> list[dict]:
-339        """Search for rows that contain query_string as a substring
-340        of any column.
+339    ) -> list[dict]:
+340        """Search for rows that contain `query_string` as a substring of any
+column.
 341
-342        :param table: The table to search.
+342        #### :params:
 343
-344        :param query_string: The substring to search for in all columns.
+344        `table`: The table to search.
 345
-346        :param columns: A list of columns to search for query_string.
-347        If None, all columns in the table will be searched.
-348        """
-349        if type(columns) is str:
-350            columns = [columns]
-351        results = []
-352        if not columns:
-353            columns = self.get_column_names(table)
-354        for column in columns:
-355            results.extend(
-356                [
-357                    row
-358                    for row in self.get_rows(
-359                        table, [(column, query_string)], exact_match=False
-360                    )
-361                    if row not in results
-362                ]
-363            )
-364        return results
-365
-366    @_connect
-367    def delete(
-368        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+346        `query_string`: The substring to search for in all columns.
+347
+348        `columns`: A list of columns to search for query_string.
+349        If None, all columns in the table will be searched.
+350        """
+351        if type(columns) is str:
+352            columns = [columns]
+353        results = []
+354        if not columns:
+355            columns = self.get_column_names(table)
+356        for column in columns:
+357            results.extend(
+358                [
+359                    row
+360                    for row in self.get_rows(
+361                        table, [(column, query_string)], exact_match=False
+362                    )
+363                    if row not in results
+364                ]
+365            )
+366        return results
+367
+368    @_connect
+369    def delete(
+370        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-369    ) -> int:
-370        """Delete records from table.
-371
-372        Returns number of deleted records.
+371    ) -> int:
+372        """Delete records from `table`.
 373
-374        :param match_criteria: Can be a list of 2-tuples where each
-375        tuple is (columnName, rowValue) or a dictionary where
-376        keys are column names and values are row values.
+374        Returns the number of deleted records.
+375
+376        #### :params:
 377
-378        :param exact_match: If False, the rowValue for a give column
-379        will be matched as a substring.
-380        """
-381        num_matches = self.count(table, match_criteria, exact_match)
-382        conditions = self._get_conditions(match_criteria, exact_match)
-383        try:
-384            self.cursor.execute(f"delete from {table} where {conditions}")
-385            self.logger.info(
-386                f'Deleted {num_matches} from "{table}" where {conditions}".'
-387            )
-388            return num_matches
-389        except Exception as e:
-390            self.logger.debug(f'Error deleting from "{table}" where
+378        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+(column_name, value)`
+379        or a dictionary where keys are column names and values are
+corresponding values.
+380
+381        `exact_match`: If `False`, the value for a given column will be
+matched as a substring.
+382        """
+383        num_matches = self.count(table, match_criteria, exact_match)
+384        conditions = self._get_conditions(match_criteria, exact_match)
+385        try:
+386            self.cursor.execute(f"delete from {table} where {conditions};")
+387            self.logger.info(
+388                f'Deleted {num_matches} from "{table}" where {conditions}".'
+389            )
+390            return num_matches
+391        except Exception as e:
+392            self.logger.debug(f'Error deleting from "{table}" where
 {conditions}.\n{e}')
-391            return 0
-392
-393    @_connect
-394    def update(
-395        self,
-396        table: str,
-397        column_to_update: str,
-398        new_value: Any,
-399        match_criteria: list[tuple] | dict | None = None,
-400    ) -> bool:
-401        """Update row value for entry matched with match_criteria.
-402
-403        :param column_to_update: The column to be updated in the matched
-row.
+393            return 0
+394
+395    @_connect
+396    def update(
+397        self,
+398        table: str,
+399        column_to_update: str,
+400        new_value: Any,
+401        match_criteria: list[tuple] | dict | None = None,
+402    ) -> bool:
+403        """Update the value in `column_to_update` to `new_value` for rows
+matched with `match_criteria`.
 404
-405        :param new_value: The new value to insert.
+405        #### :params:
 406
-407        :param match_criteria: Can be a list of 2-tuples where each
-408        tuple is (columnName, rowValue) or a dictionary where
-409        keys are column names and values are row values.
-410        If None, every row will be updated.
+407        `table`: The table to update rows in.
+408
+409        `column_to_update`: The column to be updated in the matched rows.
+410
+411        `new_value`: The new value to insert.
+412
+413        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+(columnName, rowValue)`
+414        or a dictionary where keys are column names and values are
+corresponding values.
+415        If `None`, every row in `table` will be updated.
+416
+417        Returns `True` if successful, `False` if not."""
+418        query = f"update {table} set {column_to_update} = ?"
+419        conditions = ""
+420        if match_criteria:
+421            if self.count(table, match_criteria) == 0:
+422                self.logger.info(
+423                    f"Couldn't find matching records in {table} table to
+update to '{new_value}'"
+424                )
+425                return False
+426            conditions = self._get_conditions(match_criteria)
+427            query += f" where {conditions}"
+428        else:
+429            conditions = None
+430        query += ";"
+431        try:
+432            self.cursor.execute(
+433                query,
+434                (new_value,),
+435            )
+436            self.logger.info(
+437                f'Updated "{column_to_update}" in "{table}" table to "
+{new_value}" where {conditions}'
+438            )
+439            return True
+440        except Exception as e:
+441            self.logger.error(
+442                f'Failed to update "{column_to_update}" in "{table}" table
+to "{new_value}" where {conditions}"\n{e}'
+443            )
+444            return False
+445
+446    @_connect
+447    def drop_table(self, table: str) -> bool:
+448        """Drop `table` from the database.
+449
+450        Returns `True` if successful, `False` if not."""
+451        try:
+452            self.cursor.execute(f"drop Table {table};")
+453            self.logger.info(f'Dropped table "{table}"')
+454            return True
+455        except Exception as e:
+456            print(e)
+457            self.logger.error(f'Failed to drop table "{table}"')
+458            return False
+459
+460    @_connect
+461    def add_column(
+462        self, table: str, column: str, _type: str, default_value: str | None
+= None
+463    ):
+464        """Add a new column to `table`.
+465
+466        #### :params:
+467
+468        `column`: Name of the column to add.
+469
+470        `_type`: The data type of the new column.
+471
+472        `default_value`: Optional default value for the column."""
+473        try:
+474            if default_value:
+475                self.cursor.execute(
+476                    f"alter table {table} add column {column} {_type}
+default {default_value};"
+477                )
+478                self.update(table, column, default_value)
+479            else:
+480                self.cursor.execute(f"alter table {table} add column
+{column} {_type};")
+481            self.logger.info(f'Added column "{column}" to "{table}" table.')
+482        except Exception as e:
+483            self.logger.error(f'Failed to add column "{column}" to "{table}"
+table.')
+484
+485    @staticmethod
+486    def data_to_string(
+487        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+bool = True
+488    ) -> str:
+489        """Uses tabulate to produce pretty string output from a list of
+dictionaries.
+490
+491        #### :params:
+492
+493        `data`: The list of dictionaries to create a grid from.
+494        Assumes all dictionaries in list have the same set of keys.
+495
+496        `sort_key`: Optional dictionary key to sort data with.
+497
+498        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+fit within the current terminal window.
+499        Pass as `False` if the output is going into something like a `.txt`
+file."""
+500        return data_to_string(data, sort_key, wrap_to_terminal)
+501
+502
+503def data_to_string(
+504    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+True
+505) -> str:
+506    """Uses tabulate to produce pretty string output from a list of
+dictionaries.
+507
+508    #### :params:
+509
+510    `data`: The list of dictionaries to create a grid from.
+511    Assumes all dictionaries in list have the same set of keys.
+512
+513    `sort_key`: Optional dictionary key to sort data with.
+514
+515    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
+within the current terminal window.
+516    Pass as `False` if the output is going into something like a `.txt`
+file."""
+517    if len(data) == 0:
+518        return ""
+519    if sort_key:
+520        data = sorted(data, key=lambda d: d[sort_key])
+521    for i, d in enumerate(data):
+522        for k in d:
+523            data[i][k] = str(data[i][k])
+524
+525    too_wide = True
+526    terminal_width = os.get_terminal_size().columns
+527    max_col_widths = terminal_width
+528    # Make an output with effectively unrestricted column widths
+529    # to see if shrinking is necessary
+530    output = tabulate(
+531        data,
+532        headers="keys",
+533        disable_numparse=True,
+534        tablefmt="grid",
+535        maxcolwidths=max_col_widths,
+536    )
+537    current_width = output.index("\n")
+538    if current_width < terminal_width:
+539        too_wide = False
+540    if wrap_to_terminal and too_wide:
+541        print("Resizing grid to fit within the terminal...\n")
+542        previous_col_widths = max_col_widths
+543        acceptable_width = terminal_width - 10
+544        while too_wide and max_col_widths > 1:
+545            if current_width >= terminal_width:
+546                previous_col_widths = max_col_widths
+547                max_col_widths = int(max_col_widths * 0.5)
+548            elif current_width < terminal_width:
+549                # Without lowering acceptable_width, this condition will
+cause infinite loop
+550                if max_col_widths == previous_col_widths - 1:
+551                    acceptable_width -= 10
+552                max_col_widths = int(
+553                    max_col_widths + (0.5 * (previous_col_widths -
+max_col_widths))
+554                )
+555            output = tabulate(
+556                data,
+557                headers="keys",
+558                disable_numparse=True,
+559                tablefmt="grid",
+560                maxcolwidths=max_col_widths,
+561            )
+562            current_width = output.index("\n")
+563            if acceptable_width < current_width < terminal_width:
+564                too_wide = False
+565        if too_wide:
+566            print("Couldn't resize grid to fit within the terminal.")
+567            return str(data)
+568    return output
+  ⁰
+class DataBased: View Source
+_27class DataBased:
+_28    """Sqli wrapper so queries don't need to be written except table
+definitions.
+_29
+_30    Supports saving and reading dates as datetime objects.
+_31
+_32    Supports using a context manager."""
+_33
+_34    def __init__(
+_35        self,
+_36        dbpath: str | Pathier,
+_37        logger_encoding: str = "utf-8",
+_38        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
+_39    ):
+_40        """
+_41        #### :params:
+_42
+_43        `dbpath`: String or Path object to database file.
+_44        If a relative path is given, it will be relative to the
+_45        current working directory. The log file will be saved to the
+_46        same directory.
+_47
+_48        `logger_message_format`: '{' style format string for the logger
+object."""
+_49        self.dbpath = Pathier(dbpath)
+_50        self.dbname = Pathier(dbpath).name
+_51        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
+_52        self._logger_init(
+_53            encoding=logger_encoding, message_format=logger_message_format
+_54        )
+_55        self.connection_open = False
+_56
+_57    def __enter__(self):
+_58        self.open()
+_59        return self
+_60
+_61    def __exit__(self, exception_type, exception_value,
+exception_traceback):
+_62        self.close()
+_63
+_64    def open(self):
+_65        """Open connection to db."""
+_66        self.connection = sqlite3.connect(
+_67            self.dbpath,
+_68            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
+_69            timeout=10,
+_70        )
+_71        self.connection.execute("pragma foreign_keys = 1;")
+_72        self.cursor = self.connection.cursor()
+_73        self.connection_open = True
+_74
+_75    def close(self):
+_76        """Save and close connection to db.
+_77
+_78        Call this as soon as you are done using the database if you have
+_79        multiple threads or processes using the same database."""
+_80        if self.connection_open:
+_81            self.connection.commit()
+_82            self.connection.close()
+_83            self.connection_open = False
+_84
+_85    def _logger_init(
+_86        self,
+_87        message_format: str = "{levelname}|-|{asctime}|-|{message}",
+_88        encoding: str = "utf-8",
+_89    ):
+_90        """:param `message_format`: '{' style format string"""
+_91        self.logger = logging.getLogger(self.dbname)
+_92        if not self.logger.hasHandlers():
+_93            handler = logging.FileHandler(
+_94                str(self.dbpath).replace(".", "") + ".log",
+encoding=encoding
+_95            )
+_96            handler.setFormatter(
+_97                logging.Formatter(
+_98                    message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S
+%p"
+_99                )
+100            )
+101            self.logger.addHandler(handler)
+102            self.logger.setLevel(logging.INFO)
+103
+104    def _get_dict(
+105        self, table: str, values: list, columns_to_return: list[str] | None
+= None
+106    ) -> dict:
+107        """Converts the values of a row into a dictionary with column names
+as keys.
+108
+109        #### :params:
+110
+111        `table`: The table that values were pulled from.
+112
+113        `values`: List of values expected to be the same quantity
+114        and in the same order as the column names of table.
+115
+116        `columns_to_return`: An optional list of column names.
+117        If given, only these columns will be included in the returned
+dictionary.
+118        Otherwise all columns and values are returned."""
+119        return {
+120            column: value
+121            for column, value in zip(self.get_column_names(table), values)
+122            if not columns_to_return or column in columns_to_return
+123        }
+124
+125    def _get_conditions(
+126        self, match_criteria: list[tuple] | dict, exact_match: bool = True
+127    ) -> str:
+128        """Builds and returns the conditional portion of a query.
+129
+130        #### :params:
+131
+132        `match_criteria`: Can be a list of 2-tuples where each
+133        tuple is `(columnName, rowValue)` or a dictionary where
+134        keys are column names and values are row values.
+135
+136        `exact_match`: If `False`, the row value for a given column
+137        will be matched as a substring.
+138
+139        Usage e.g.:
+140
+141        >>> self.cursor.execute(f'select * from {table} where
+{conditions};')"""
+142        if type(match_criteria) == dict:
+143            match_criteria = [(k, v) for k, v in match_criteria.items()]
+144        if exact_match:
+145            conditions = " and ".join(
+146                f'"{column_row[0]}" = "{column_row[1]}"'
+147                for column_row in match_criteria
+148            )
+149        else:
+150            conditions = " and ".join(
+151                f'"{column_row[0]}" like "%{column_row[1]}%"'
+152                for column_row in match_criteria
+153            )
+154        return f"({conditions})"
+155
+156    @_connect
+157    def query(self, query_) -> list[Any]:
+158        """Execute an arbitrary query and return the results."""
+159        self.cursor.execute(query_)
+160        return self.cursor.fetchall()
+161
+162    @_connect
+163    def create_tables(self, table_defs: list[str] = []):
+164        """Create tables if they don't exist.
+165
+166        :param `table_defs`: Each definition should be in the form
+`table_name(column_definitions)`"""
+167        if len(table_defs) > 0:
+168            table_names = self.get_table_names()
+169            for table in table_defs:
+170                if table.split("(")[0].strip() not in table_names:
+171                    self.cursor.execute(f"create table {table};")
+172                    self.logger.info(f'{table.split("(")[0]} table
+created.')
+173
+174    @_connect
+175    def create_table(self, table: str, column_defs: list[str]):
+176        """Create a table if it doesn't exist.
+177
+178        #### :params:
+179
+180        `table`: Name of the table to create.
+181
+182        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+183        i.e. `"column_name text unique"` or `"column_name int primary key"`
+etc."""
+184        if table not in self.get_table_names():
+185            query = f"create table {table}({', '.join(column_defs)});"
+186            self.cursor.execute(query)
+187            self.logger.info(f"'{table}' table created.")
+188
+189    @_connect
+190    def get_table_names(self) -> list[str]:
+191        """Returns a list of table names from the database."""
+192        self.cursor.execute(
+193            'select name from sqlite_Schema where type = "table" and name
+not like "sqlite_%";'
+194        )
+195        return [result[0] for result in self.cursor.fetchall()]
+196
+197    @_connect
+198    def get_column_names(self, table: str) -> list[str]:
+199        """Return a list of column names from a table."""
+200        self.cursor.execute(f"select * from {table} where 1=0")
+201        return [description[0] for description in self.cursor.description]
+202
+203    @_connect
+204    def count(
+205        self,
+206        table: str,
+207        match_criteria: list[tuple] | dict | None = None,
+208        exact_match: bool = True,
+209    ) -> int:
+210        """Return number of items in `table`.
+211
+212        #### :params:
+213
+214        `match_criteria`: Can be a list of 2-tuples where each
+215        tuple is `(columnName, rowValue)` or a dictionary where
+216        keys are column names and values are row values.
+217        If `None`, all rows from the table will be counted.
+218
+219        `exact_match`: If `False`, the row value for a given column
+220        in `match_criteria` will be matched as a substring.
+221        Has no effect if `match_criteria` is `None`.
+222        """
+223        query = f"select count(_rowid_) from {table}"
+224        try:
+225            if match_criteria:
+226                self.cursor.execute(
+227                    f"{query} where {self._get_conditions(match_criteria,
+exact_match)};"
+228                )
+229            else:
+230                self.cursor.execute(f"{query}")
+231            return self.cursor.fetchone()[0]
+232        except:
+233            return 0
+234
+235    @_connect
+236    def add_row(
+237        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+None
+238    ):
+239        """Add a row of values to a table.
+240
+241        #### :params:
+242
+243        `table`: The table to insert values into.
+244
+245        `values`: A tuple of values to be inserted into the table.
+246
+247        `columns`: If `None`, `values` is expected to supply a value for
+every column in the table.
+248        If `columns` is provided, it should contain the same number of
+elements as `values`."""
+249        parameterizer = ", ".join("?" for _ in values)
+250        logger_values = ", ".join(str(value) for value in values)
+251        try:
+252            if columns:
+253                columns_query = ", ".join(column for column in columns)
+254                self.cursor.execute(
+255                    f"insert into {table} ({columns_query}) values(
+{parameterizer});",
+256                    values,
+257                )
+258            else:
+259                self.cursor.execute(
+260                    f"insert into {table} values({parameterizer});", values
+261                )
+262            self.logger.info(f'Added "{logger_values}" to {table} table.')
+263        except Exception as e:
+264            if "constraint" not in str(e).lower():
+265                self.logger.exception(
+266                    f'Error adding "{logger_values}" to {table} table.'
+267                )
+268            else:
+269                self.logger.debug(str(e))
+270
+271    @_connect
+272    def get_rows(
+273        self,
+274        table: str,
+275        match_criteria: list[tuple] | dict | None = None,
+276        exact_match: bool = True,
+277        sort_by_column: str | None = None,
+278        columns_to_return: list[str] | None = None,
+279        return_as_dataframe: bool = False,
+280        values_only: bool = False,
+281        order_by: str | None = None,
+282        limit: str | int | None = None,
+283    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+284        """Return matching rows from `table`.
+285
+286        By default, rows will be returned as a list of dictionaries of the
+form `[{"column_name": value, ...}, ...]`
+287
+288
+289        #### :params:
+290
+291        `match_criteria`: Can be a list of 2-tuples where each
+292        tuple is `(columnName, rowValue)` or a dictionary where
+293        keys are column names and values are row values.
+294
+295        `exact_match`: If `False`, the row value for a given column will be
+matched as a substring.
+296
+297        `sort_by_column`: A column name to sort the results by.
+298        This will sort results in Python after retrieving them from the db.
+299        Use the 'order_by' param to use SQLite engine for ordering.
+300
+301        `columns_to_return`: Optional list of column names.
+302        If provided, the elements returned by this function will only
+contain the provided columns.
+303        Otherwise every column in the row is returned.
+304
+305        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
+object.
+306
+307        `values_only`: Return the results as a list of tuples.
+308
+309        `order_by`: If given, a `order by {order_by}` clause will be added
+to the select query.
+310
+311        `limit`: If given, a `limit {limit}` clause will be added to the
+select query.
+312        """
+313
+314        if type(columns_to_return) is str:
+315            columns_to_return = [columns_to_return]
+316        query = f"select * from {table}"
+317        matches = []
+318        if match_criteria:
+319            query += f" where {self._get_conditions(match_criteria,
+exact_match)}"
+320        if order_by:
+321            query += f" order by {order_by}"
+322        if limit:
+323            query += f" limit {limit}"
+324        query += ";"
+325        self.cursor.execute(query)
+326        matches = self.cursor.fetchall()
+327        results = [self._get_dict(table, match, columns_to_return) for match
+in matches]
+328        if sort_by_column:
+329            results = sorted(results, key=lambda x: x[sort_by_column])
+330        if return_as_dataframe:
+331            return pandas.DataFrame(results)
+332        if values_only:
+333            return [tuple(row.values()) for row in results]
+334        else:
+335            return results
+336
+337    @_connect
+338    def find(
+339        self, table: str, query_string: str, columns: list[str] | None =
+None
+340    ) -> list[dict]:
+341        """Search for rows that contain `query_string` as a substring of any
+column.
+342
+343        #### :params:
+344
+345        `table`: The table to search.
+346
+347        `query_string`: The substring to search for in all columns.
+348
+349        `columns`: A list of columns to search for query_string.
+350        If None, all columns in the table will be searched.
+351        """
+352        if type(columns) is str:
+353            columns = [columns]
+354        results = []
+355        if not columns:
+356            columns = self.get_column_names(table)
+357        for column in columns:
+358            results.extend(
+359                [
+360                    row
+361                    for row in self.get_rows(
+362                        table, [(column, query_string)], exact_match=False
+363                    )
+364                    if row not in results
+365                ]
+366            )
+367        return results
+368
+369    @_connect
+370    def delete(
+371        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+bool = True
+372    ) -> int:
+373        """Delete records from `table`.
+374
+375        Returns the number of deleted records.
+376
+377        #### :params:
+378
+379        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+(column_name, value)`
+380        or a dictionary where keys are column names and values are
+corresponding values.
+381
+382        `exact_match`: If `False`, the value for a given column will be
+matched as a substring.
+383        """
+384        num_matches = self.count(table, match_criteria, exact_match)
+385        conditions = self._get_conditions(match_criteria, exact_match)
+386        try:
+387            self.cursor.execute(f"delete from {table} where {conditions};")
+388            self.logger.info(
+389                f'Deleted {num_matches} from "{table}" where {conditions}".'
+390            )
+391            return num_matches
+392        except Exception as e:
+393            self.logger.debug(f'Error deleting from "{table}" where
+{conditions}.\n{e}')
+394            return 0
+395
+396    @_connect
+397    def update(
+398        self,
+399        table: str,
+400        column_to_update: str,
+401        new_value: Any,
+402        match_criteria: list[tuple] | dict | None = None,
+403    ) -> bool:
+404        """Update the value in `column_to_update` to `new_value` for rows
+matched with `match_criteria`.
+405
+406        #### :params:
+407
+408        `table`: The table to update rows in.
+409
+410        `column_to_update`: The column to be updated in the matched rows.
 411
-412        Returns True if successful, False if not."""
-413        query = f"update {table} set {column_to_update} = ?"
-414        conditions = ""
-415        if match_criteria:
-416            if self.count(table, match_criteria) == 0:
-417                self.logger.info(
-418                    f"Couldn't find matching records in {table} table to
+412        `new_value`: The new value to insert.
+413
+414        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+(columnName, rowValue)`
+415        or a dictionary where keys are column names and values are
+corresponding values.
+416        If `None`, every row in `table` will be updated.
+417
+418        Returns `True` if successful, `False` if not."""
+419        query = f"update {table} set {column_to_update} = ?"
+420        conditions = ""
+421        if match_criteria:
+422            if self.count(table, match_criteria) == 0:
+423                self.logger.info(
+424                    f"Couldn't find matching records in {table} table to
 update to '{new_value}'"
-419                )
-420                return False
-421            conditions = self._get_conditions(match_criteria)
-422            query += f" where {conditions}"
-423        else:
-424            conditions = None
-425        try:
-426            self.cursor.execute(
-427                query,
-428                (new_value,),
-429            )
-430            self.logger.info(
-431                f'Updated "{column_to_update}" in "{table}" table to "
+425                )
+426                return False
+427            conditions = self._get_conditions(match_criteria)
+428            query += f" where {conditions}"
+429        else:
+430            conditions = None
+431        query += ";"
+432        try:
+433            self.cursor.execute(
+434                query,
+435                (new_value,),
+436            )
+437            self.logger.info(
+438                f'Updated "{column_to_update}" in "{table}" table to "
 {new_value}" where {conditions}'
-432            )
-433            return True
-434        except Exception as e:
-435            self.logger.error(
-436                f'Failed to update "{column_to_update}" in "{table}" table
+439            )
+440            return True
+441        except Exception as e:
+442            self.logger.error(
+443                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-437            )
-438            return False
-439
-440    @_connect
-441    def drop_table(self, table: str) -> bool:
-442        """Drop a table from the database.
-443
-444        Returns True if successful, False if not."""
-445        try:
-446            self.cursor.execute(f"drop Table {table}")
-447            self.logger.info(f'Dropped table "{table}"')
-448            return True
-449        except Exception as e:
-450            print(e)
-451            self.logger.error(f'Failed to drop table "{table}"')
-452            return False
-453
-454    @_connect
-455    def add_column(
-456        self, table: str, column: str, _type: str, default_value: str | None
+444            )
+445            return False
+446
+447    @_connect
+448    def drop_table(self, table: str) -> bool:
+449        """Drop `table` from the database.
+450
+451        Returns `True` if successful, `False` if not."""
+452        try:
+453            self.cursor.execute(f"drop Table {table};")
+454            self.logger.info(f'Dropped table "{table}"')
+455            return True
+456        except Exception as e:
+457            print(e)
+458            self.logger.error(f'Failed to drop table "{table}"')
+459            return False
+460
+461    @_connect
+462    def add_column(
+463        self, table: str, column: str, _type: str, default_value: str | None
 = None
-457    ):
-458        """Add a new column to table.
-459
-460        :param column: Name of the column to add.
-461
-462        :param _type: The data type of the new column.
-463
-464        :param default_value: Optional default value for the column."""
-465        try:
-466            if default_value:
-467                self.cursor.execute(
-468                    f"alter table {table} add column {column} {_type}
-default {default_value}"
-469                )
-470            else:
-471                self.cursor.execute(f"alter table {table} add column
-{column} {_type}")
-472            self.logger.info(f'Added column "{column}" to "{table}" table.')
-473        except Exception as e:
-474            self.logger.error(f'Failed to add column "{column}" to "{table}"
+464    ):
+465        """Add a new column to `table`.
+466
+467        #### :params:
+468
+469        `column`: Name of the column to add.
+470
+471        `_type`: The data type of the new column.
+472
+473        `default_value`: Optional default value for the column."""
+474        try:
+475            if default_value:
+476                self.cursor.execute(
+477                    f"alter table {table} add column {column} {_type}
+default {default_value};"
+478                )
+479                self.update(table, column, default_value)
+480            else:
+481                self.cursor.execute(f"alter table {table} add column
+{column} {_type};")
+482            self.logger.info(f'Added column "{column}" to "{table}" table.')
+483        except Exception as e:
+484            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
-475
-476    @staticmethod
-477    def data_to_string(
-478        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+485
+486    @staticmethod
+487    def data_to_string(
+488        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-479    ) -> str:
-480        """Uses tabulate to produce pretty string output
-481        from a list of dictionaries.
-482
-483        :param data: Assumes all dictionaries in list have the same set of
-keys.
-484
-485        :param sort_key: Optional dictionary key to sort data with.
-486
-487        :param wrap_to_terminal: If True, the table width will be wrapped
-488        to fit within the current terminal window. Set to False
-489        if the output is going into something like a txt file."""
-490        return data_to_string(data, sort_key, wrap_to_terminal)
+489    ) -> str:
+490        """Uses tabulate to produce pretty string output from a list of
+dictionaries.
+491
+492        #### :params:
+493
+494        `data`: The list of dictionaries to create a grid from.
+495        Assumes all dictionaries in list have the same set of keys.
+496
+497        `sort_key`: Optional dictionary key to sort data with.
+498
+499        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+fit within the current terminal window.
+500        Pass as `False` if the output is going into something like a `.txt`
+file."""
+501        return data_to_string(data, sort_key, wrap_to_terminal)
 Sqli wrapper so queries don't need to be written except table definitions.
 Supports saving and reading dates as datetime objects.
 Supports using a context manager.
 ⁰
 DataBased(
 dbpath: str | pathier.pathier.Pathier,
 logger_encoding: str = 'utf-8',
@@ -1121,639 +1182,666 @@
 34    def __init__(
 35        self,
 36        dbpath: str | Pathier,
 37        logger_encoding: str = "utf-8",
 38        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
 39    ):
 40        """
-41        :param dbpath: String or Path object to database file.
-42        If a relative path is given, it will be relative to the
-43        current working directory. The log file will be saved to the
-44        same directory.
-45
-46        :param logger_message_format: '{' style format string
-47        for the logger object."""
-48        self.dbpath = Pathier(dbpath)
-49        self.dbname = Pathier(dbpath).name
-50        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
-51        self._logger_init(
-52            encoding=logger_encoding, message_format=logger_message_format
-53        )
-54        self.connection_open = False
-* Parameters *
-    * dbpath: String or Path object to database file. If a relative path is
-      given, it will be relative to the current working directory. The log file
-      will be saved to the same directory.
-    * logger_message_format: '{' style format string for the logger object.
+41        #### :params:
+42
+43        `dbpath`: String or Path object to database file.
+44        If a relative path is given, it will be relative to the
+45        current working directory. The log file will be saved to the
+46        same directory.
+47
+48        `logger_message_format`: '{' style format string for the logger
+object."""
+49        self.dbpath = Pathier(dbpath)
+50        self.dbname = Pathier(dbpath).name
+51        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
+52        self._logger_init(
+53            encoding=logger_encoding, message_format=logger_message_format
+54        )
+55        self.connection_open = False
+*** :params: ***
+dbpath: String or Path object to database file. If a relative path is given, it
+will be relative to the current working directory. The log file will be saved
+to the same directory.
+logger_message_format: '{' style format string for the logger object.
 ⁰
 def open(self): View Source
-63    def open(self):
-64        """Open connection to db."""
-65        self.connection = sqlite3.connect(
-66            self.dbpath,
-67            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-68            timeout=10,
-69        )
-70        self.connection.execute("pragma foreign_keys = 1")
-71        self.cursor = self.connection.cursor()
-72        self.connection_open = True
+64    def open(self):
+65        """Open connection to db."""
+66        self.connection = sqlite3.connect(
+67            self.dbpath,
+68            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
+69            timeout=10,
+70        )
+71        self.connection.execute("pragma foreign_keys = 1;")
+72        self.cursor = self.connection.cursor()
+73        self.connection_open = True
 Open connection to db.
 ⁰
 def close(self): View Source
-74    def close(self):
-75        """Save and close connection to db.
-76
-77        Call this as soon as you are done using the database if you have
-78        multiple threads or processes using the same database."""
-79        if self.connection_open:
-80            self.connection.commit()
-81            self.connection.close()
-82            self.connection_open = False
+75    def close(self):
+76        """Save and close connection to db.
+77
+78        Call this as soon as you are done using the database if you have
+79        multiple threads or processes using the same database."""
+80        if self.connection_open:
+81            self.connection.commit()
+82            self.connection.close()
+83            self.connection_open = False
 Save and close connection to db.
 Call this as soon as you are done using the database if you have multiple
 threads or processes using the same database.
 ⁰
 def query(self, query_) -> list[typing.Any]: View Source
-151    @_connect
-152    def query(self, query_) -> list[Any]:
-153        """Execute an arbitrary query and
-154        return the results."""
-155        self.cursor.execute(query_)
-156        return self.cursor.fetchall()
+156    @_connect
+157    def query(self, query_) -> list[Any]:
+158        """Execute an arbitrary query and return the results."""
+159        self.cursor.execute(query_)
+160        return self.cursor.fetchall()
 Execute an arbitrary query and return the results.
 ⁰
-def create_tables(self, table_querys: list[str] = []): View Source
-158    @_connect
-159    def create_tables(self, table_querys: list[str] = []):
-160        """Create tables if they don't exist.
-161
-162        :param table_querys: Each query should be
-163        in the form 'tableName(columnDefinitions)'"""
-164        if len(table_querys) > 0:
-165            table_names = self.get_table_names()
-166            for table in table_querys:
-167                if table.split("(")[0].strip() not in table_names:
-168                    self.cursor.execute(f"create table {table}")
-169                    self.logger.info(f'{table.split("(")[0]} table
+def create_tables(self, table_defs: list[str] = []): View Source
+162    @_connect
+163    def create_tables(self, table_defs: list[str] = []):
+164        """Create tables if they don't exist.
+165
+166        :param `table_defs`: Each definition should be in the form
+`table_name(column_definitions)`"""
+167        if len(table_defs) > 0:
+168            table_names = self.get_table_names()
+169            for table in table_defs:
+170                if table.split("(")[0].strip() not in table_names:
+171                    self.cursor.execute(f"create table {table};")
+172                    self.logger.info(f'{table.split("(")[0]} table
 created.')
 Create tables if they don't exist.
 * Parameters *
-    * table_querys: Each query should be in the form 'tableName
-      (columnDefinitions)'
+    * table_defs: Each definition should be in the form table_name
+      (column_definitions)
 ⁰
 def create_table(self, table: str, column_defs: list[str]): View Source
-171    @_connect
-172    def create_table(self, table: str, column_defs: list[str]):
-173        """Create a table if it doesn't exist.
-174
-175        :param table: Name of the table to create.
-176
-177        :param column_defs: List of column definitions in
-178        proper Sqlite3 sytax.
-179        i.e. "columnName text unique" or "columnName int primary key"
+174    @_connect
+175    def create_table(self, table: str, column_defs: list[str]):
+176        """Create a table if it doesn't exist.
+177
+178        #### :params:
+179
+180        `table`: Name of the table to create.
+181
+182        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+183        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
-180        if table not in self.get_table_names():
-181            query = f"create table {table}({', '.join(column_defs)})"
-182            self.cursor.execute(query)
-183            self.logger.info(f"'{table}' table created.")
+184        if table not in self.get_table_names():
+185            query = f"create table {table}({', '.join(column_defs)});"
+186            self.cursor.execute(query)
+187            self.logger.info(f"'{table}' table created.")
 Create a table if it doesn't exist.
-* Parameters *
-    * table: Name of the table to create.
-    * column_defs: List of column definitions in proper Sqlite3 sytax. i.e.
-      "columnName text unique" or "columnName int primary key" etc.
+*** :params: ***
+table: Name of the table to create.
+column_defs: List of column definitions in proper Sqlite3 sytax. i.e.
+"column_name text unique" or "column_name int primary key" etc.
 ⁰
 def get_table_names(self) -> list[str]: View Source
-185    @_connect
-186    def get_table_names(self) -> list[str]:
-187        """Returns a list of table names from database."""
-188        self.cursor.execute(
-189            'select name from sqlite_Schema where type = "table" and name
-not like "sqlite_%"'
-190        )
-191        return [result[0] for result in self.cursor.fetchall()]
-Returns a list of table names from database.
+189    @_connect
+190    def get_table_names(self) -> list[str]:
+191        """Returns a list of table names from the database."""
+192        self.cursor.execute(
+193            'select name from sqlite_Schema where type = "table" and name
+not like "sqlite_%";'
+194        )
+195        return [result[0] for result in self.cursor.fetchall()]
+Returns a list of table names from the database.
 ⁰
 def get_column_names(self, table: str) -> list[str]: View Source
-193    @_connect
-194    def get_column_names(self, table: str) -> list[str]:
-195        """Return a list of column names from a table."""
-196        self.cursor.execute(f"select * from {table} where 1=0")
-197        return [description[0] for description in self.cursor.description]
+197    @_connect
+198    def get_column_names(self, table: str) -> list[str]:
+199        """Return a list of column names from a table."""
+200        self.cursor.execute(f"select * from {table} where 1=0")
+201        return [description[0] for description in self.cursor.description]
 Return a list of column names from a table.
 ⁰
 def count(
 self,
 table: str,
 match_criteria: list[tuple] | dict | None = None,
 exact_match: bool = True) -> int: View Source
-199    @_connect
-200    def count(
-201        self,
-202        table: str,
-203        match_criteria: list[tuple] | dict | None = None,
-204        exact_match: bool = True,
-205    ) -> int:
-206        """Return number of items in table.
-207
-208        :param match_criteria: Can be a list of 2-tuples where each
-209        tuple is (columnName, rowValue) or a dictionary where
-210        keys are column names and values are row values.
-211        If None, all rows from the table will be counted.
-212
-213        :param exact_match: If False, the row value for a give column
-214        in match_criteria will be matched as a substring. Has no effect if
-215        match_criteria is None.
-216        """
-217        query = f"select count(_rowid_) from {table}"
-218        try:
-219            if match_criteria:
-220                self.cursor.execute(
-221                    f"{query} where {self._get_conditions(match_criteria,
-exact_match)}"
-222                )
-223            else:
-224                self.cursor.execute(f"{query}")
-225            return self.cursor.fetchone()[0]
-226        except:
-227            return 0
+203    @_connect
+204    def count(
+205        self,
+206        table: str,
+207        match_criteria: list[tuple] | dict | None = None,
+208        exact_match: bool = True,
+209    ) -> int:
+210        """Return number of items in `table`.
+211
+212        #### :params:
+213
+214        `match_criteria`: Can be a list of 2-tuples where each
+215        tuple is `(columnName, rowValue)` or a dictionary where
+216        keys are column names and values are row values.
+217        If `None`, all rows from the table will be counted.
+218
+219        `exact_match`: If `False`, the row value for a given column
+220        in `match_criteria` will be matched as a substring.
+221        Has no effect if `match_criteria` is `None`.
+222        """
+223        query = f"select count(_rowid_) from {table}"
+224        try:
+225            if match_criteria:
+226                self.cursor.execute(
+227                    f"{query} where {self._get_conditions(match_criteria,
+exact_match)};"
+228                )
+229            else:
+230                self.cursor.execute(f"{query}")
+231            return self.cursor.fetchone()[0]
+232        except:
+233            return 0
 Return number of items in table.
-* Parameters *
-    * match_criteria: Can be a list of 2-tuples where each tuple is
-      (columnName, rowValue) or a dictionary where keys are column names and
-      values are row values. If None, all rows from the table will be counted.
-    * exact_match: If False, the row value for a give column in match_criteria
-      will be matched as a substring. Has no effect if match_criteria is None.
+*** :params: ***
+match_criteria: Can be a list of 2-tuples where each tuple is (columnName,
+rowValue) or a dictionary where keys are column names and values are row
+values. If None, all rows from the table will be counted.
+exact_match: If False, the row value for a given column in match_criteria will
+be matched as a substring. Has no effect if match_criteria is None.
 ⁰
 def add_row(
 self,
 table: str,
 values: tuple[typing.Any],
 columns: tuple[str] | None = None): View Source
-229    @_connect
-230    def add_row(
-231        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+235    @_connect
+236    def add_row(
+237        self, table: str, values: tuple[Any], columns: tuple[str] | None =
 None
-232    ):
-233        """Add row of values to table.
-234
-235        :param table: The table to insert into.
-236
-237        :param values: A tuple of values to be inserted into the table.
-238
-239        :param columns: If None, values param is expected to supply
-240        a value for every column in the table. If columns is
-241        provided, it should contain the same number of elements as
-values."""
-242        parameterizer = ", ".join("?" for _ in values)
-243        logger_values = ", ".join(str(value) for value in values)
-244        try:
-245            if columns:
-246                columns_query = ", ".join(column for column in columns)
-247                self.cursor.execute(
-248                    f"insert into {table} ({columns_query}) values(
-{parameterizer})",
-249                    values,
-250                )
-251            else:
-252                self.cursor.execute(
-253                    f"insert into {table} values({parameterizer})", values
-254                )
-255            self.logger.info(f'Added "{logger_values}" to {table} table.')
-256        except Exception as e:
-257            if "constraint" not in str(e).lower():
-258                self.logger.exception(
-259                    f'Error adding "{logger_values}" to {table} table.'
-260                )
-261            else:
-262                self.logger.debug(str(e))
-Add row of values to table.
-* Parameters *
-    * table: The table to insert into.
-    * values: A tuple of values to be inserted into the table.
-    * columns: If None, values param is expected to supply a value for every
-      column in the table. If columns is provided, it should contain the same
-      number of elements as values.
+238    ):
+239        """Add a row of values to a table.
+240
+241        #### :params:
+242
+243        `table`: The table to insert values into.
+244
+245        `values`: A tuple of values to be inserted into the table.
+246
+247        `columns`: If `None`, `values` is expected to supply a value for
+every column in the table.
+248        If `columns` is provided, it should contain the same number of
+elements as `values`."""
+249        parameterizer = ", ".join("?" for _ in values)
+250        logger_values = ", ".join(str(value) for value in values)
+251        try:
+252            if columns:
+253                columns_query = ", ".join(column for column in columns)
+254                self.cursor.execute(
+255                    f"insert into {table} ({columns_query}) values(
+{parameterizer});",
+256                    values,
+257                )
+258            else:
+259                self.cursor.execute(
+260                    f"insert into {table} values({parameterizer});", values
+261                )
+262            self.logger.info(f'Added "{logger_values}" to {table} table.')
+263        except Exception as e:
+264            if "constraint" not in str(e).lower():
+265                self.logger.exception(
+266                    f'Error adding "{logger_values}" to {table} table.'
+267                )
+268            else:
+269                self.logger.debug(str(e))
+Add a row of values to a table.
+*** :params: ***
+table: The table to insert values into.
+values: A tuple of values to be inserted into the table.
+columns: If None, values is expected to supply a value for every column in the
+table. If columns is provided, it should contain the same number of elements as
+values.
 ⁰
 def get_rows(
 self,
 table: str,
 match_criteria: list[tuple] | dict | None = None,
 exact_match: bool = True,
 sort_by_column: str | None = None,
 columns_to_return: list[str] | None = None,
 return_as_dataframe: bool = False,
 values_only: bool = False,
 order_by: str | None = None,
 limit: str | int | None = None) -> list[dict] | list[tuple] |
 pandas.core.frame.DataFrame: View Source
-264    @_connect
-265    def get_rows(
-266        self,
-267        table: str,
-268        match_criteria: list[tuple] | dict | None = None,
-269        exact_match: bool = True,
-270        sort_by_column: str | None = None,
-271        columns_to_return: list[str] | None = None,
-272        return_as_dataframe: bool = False,
-273        values_only: bool = False,
-274        order_by: str | None = None,
-275        limit: str | int | None = None,
-276    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-277        """Returns rows from table as a list of dictionaries
-278        where the key-value pairs of the dictionaries are
-279        column name: row value.
-280
-281        :param match_criteria: Can be a list of 2-tuples where each
-282        tuple is (columnName, rowValue) or a dictionary where
-283        keys are column names and values are row values.
-284
-285        :param exact_match: If False, the rowValue for a give column
-286        will be matched as a substring.
+271    @_connect
+272    def get_rows(
+273        self,
+274        table: str,
+275        match_criteria: list[tuple] | dict | None = None,
+276        exact_match: bool = True,
+277        sort_by_column: str | None = None,
+278        columns_to_return: list[str] | None = None,
+279        return_as_dataframe: bool = False,
+280        values_only: bool = False,
+281        order_by: str | None = None,
+282        limit: str | int | None = None,
+283    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+284        """Return matching rows from `table`.
+285
+286        By default, rows will be returned as a list of dictionaries of the
+form `[{"column_name": value, ...}, ...]`
 287
-288        :param sort_by_column: A column name to sort the results by.
-289        This will sort results in Python after retrieving them from the db.
-290        Use the 'order_by' param to use SQLite engine for ordering.
-291
-292        :param columns_to_return: Optional list of column names.
-293        If provided, the elements returned by get_rows() will
-294        only contain the provided columns. Otherwise every column
-295        in the row is returned.
+288
+289        #### :params:
+290
+291        `match_criteria`: Can be a list of 2-tuples where each
+292        tuple is `(columnName, rowValue)` or a dictionary where
+293        keys are column names and values are row values.
+294
+295        `exact_match`: If `False`, the row value for a given column will be
+matched as a substring.
 296
-297        :param return_as_dataframe: If True,
-298        the results will be returned as a pandas.DataFrame object.
-299
-300        :param values_only: Return the results as a list of tuples
-301        instead of a list of dictionaries that have column names as keys.
-302        The results will still be sorted according to sort_by_column if
-303        one is provided.
+297        `sort_by_column`: A column name to sort the results by.
+298        This will sort results in Python after retrieving them from the db.
+299        Use the 'order_by' param to use SQLite engine for ordering.
+300
+301        `columns_to_return`: Optional list of column names.
+302        If provided, the elements returned by this function will only
+contain the provided columns.
+303        Otherwise every column in the row is returned.
 304
-305        :param order_by: If given, a 'order by {order_by}' clause
-306        will be added to the select query.
-307
-308        :param limit: If given, a 'limit {limit}' clause will be
-309        added to the select query.
-310        """
-311
-312        if type(columns_to_return) is str:
-313            columns_to_return = [columns_to_return]
-314        query = f"select * from {table}"
-315        matches = []
-316        if match_criteria:
-317            query += f" where {self._get_conditions(match_criteria,
+305        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
+object.
+306
+307        `values_only`: Return the results as a list of tuples.
+308
+309        `order_by`: If given, a `order by {order_by}` clause will be added
+to the select query.
+310
+311        `limit`: If given, a `limit {limit}` clause will be added to the
+select query.
+312        """
+313
+314        if type(columns_to_return) is str:
+315            columns_to_return = [columns_to_return]
+316        query = f"select * from {table}"
+317        matches = []
+318        if match_criteria:
+319            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-318        if order_by:
-319            query += f" order by {order_by}"
-320        if limit:
-321            query += f" limit {limit}"
-322        query += ";"
-323        self.cursor.execute(query)
-324        matches = self.cursor.fetchall()
-325        results = [self._get_dict(table, match, columns_to_return) for match
+320        if order_by:
+321            query += f" order by {order_by}"
+322        if limit:
+323            query += f" limit {limit}"
+324        query += ";"
+325        self.cursor.execute(query)
+326        matches = self.cursor.fetchall()
+327        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-326        if sort_by_column:
-327            results = sorted(results, key=lambda x: x[sort_by_column])
-328        if return_as_dataframe:
-329            return pandas.DataFrame(results)
-330        if values_only:
-331            return [tuple(row.values()) for row in results]
-332        else:
-333            return results
-Returns rows from table as a list of dictionaries where the key-value pairs of
-the dictionaries are column name: row value.
-* Parameters *
-    * match_criteria: Can be a list of 2-tuples where each tuple is
-      (columnName, rowValue) or a dictionary where keys are column names and
-      values are row values.
-    * exact_match: If False, the rowValue for a give column will be matched as
-      a substring.
-    * sort_by_column: A column name to sort the results by. This will sort
-      results in Python after retrieving them from the db. Use the 'order_by'
-      param to use SQLite engine for ordering.
-    * columns_to_return: Optional list of column names. If provided, the
-      elements returned by get_rows() will only contain the provided columns.
-      Otherwise every column in the row is returned.
-    * return_as_dataframe: If True, the results will be returned as a
-      pandas.DataFrame object.
-    * values_only: Return the results as a list of tuples instead of a list of
-      dictionaries that have column names as keys. The results will still be
-      sorted according to sort_by_column if one is provided.
-    * order_by: If given, a 'order by {order_by}' clause will be added to the
-      select query.
-    * limit: If given, a 'limit {limit}' clause will be added to the select
-      query.
+328        if sort_by_column:
+329            results = sorted(results, key=lambda x: x[sort_by_column])
+330        if return_as_dataframe:
+331            return pandas.DataFrame(results)
+332        if values_only:
+333            return [tuple(row.values()) for row in results]
+334        else:
+335            return results
+Return matching rows from table.
+By default, rows will be returned as a list of dictionaries of the form [
+{"column_name": value, ...}, ...]
+*** :params: ***
+match_criteria: Can be a list of 2-tuples where each tuple is (columnName,
+rowValue) or a dictionary where keys are column names and values are row
+values.
+exact_match: If False, the row value for a given column will be matched as a
+substring.
+sort_by_column: A column name to sort the results by. This will sort results in
+Python after retrieving them from the db. Use the 'order_by' param to use
+SQLite engine for ordering.
+columns_to_return: Optional list of column names. If provided, the elements
+returned by this function will only contain the provided columns. Otherwise
+every column in the row is returned.
+return_as_dataframe: Return the results as a pandas.DataFrame object.
+values_only: Return the results as a list of tuples.
+order_by: If given, a order by {order_by} clause will be added to the select
+query.
+limit: If given, a limit {limit} clause will be added to the select query.
 ⁰
 def find(
 self,
 table: str,
 query_string: str,
 columns: list[str] | None = None) -> list[dict]: View Source
-335    @_connect
-336    def find(
-337        self, table: str, query_string: str, columns: list[str] | None =
+337    @_connect
+338    def find(
+339        self, table: str, query_string: str, columns: list[str] | None =
 None
-338    ) -> list[dict]:
-339        """Search for rows that contain query_string as a substring
-340        of any column.
-341
-342        :param table: The table to search.
-343
-344        :param query_string: The substring to search for in all columns.
-345
-346        :param columns: A list of columns to search for query_string.
-347        If None, all columns in the table will be searched.
-348        """
-349        if type(columns) is str:
-350            columns = [columns]
-351        results = []
-352        if not columns:
-353            columns = self.get_column_names(table)
-354        for column in columns:
-355            results.extend(
-356                [
-357                    row
-358                    for row in self.get_rows(
-359                        table, [(column, query_string)], exact_match=False
-360                    )
-361                    if row not in results
-362                ]
-363            )
-364        return results
+340    ) -> list[dict]:
+341        """Search for rows that contain `query_string` as a substring of any
+column.
+342
+343        #### :params:
+344
+345        `table`: The table to search.
+346
+347        `query_string`: The substring to search for in all columns.
+348
+349        `columns`: A list of columns to search for query_string.
+350        If None, all columns in the table will be searched.
+351        """
+352        if type(columns) is str:
+353            columns = [columns]
+354        results = []
+355        if not columns:
+356            columns = self.get_column_names(table)
+357        for column in columns:
+358            results.extend(
+359                [
+360                    row
+361                    for row in self.get_rows(
+362                        table, [(column, query_string)], exact_match=False
+363                    )
+364                    if row not in results
+365                ]
+366            )
+367        return results
 Search for rows that contain query_string as a substring of any column.
-* Parameters *
-    * table: The table to search.
-    * query_string: The substring to search for in all columns.
-    * columns: A list of columns to search for query_string. If None, all
-      columns in the table will be searched.
+*** :params: ***
+table: The table to search.
+query_string: The substring to search for in all columns.
+columns: A list of columns to search for query_string. If None, all columns in
+the table will be searched.
 ⁰
 def delete(
 self,
 table: str,
 match_criteria: list[tuple] | dict,
 exact_match: bool = True) -> int: View Source
-366    @_connect
-367    def delete(
-368        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+369    @_connect
+370    def delete(
+371        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-369    ) -> int:
-370        """Delete records from table.
-371
-372        Returns number of deleted records.
-373
-374        :param match_criteria: Can be a list of 2-tuples where each
-375        tuple is (columnName, rowValue) or a dictionary where
-376        keys are column names and values are row values.
-377
-378        :param exact_match: If False, the rowValue for a give column
-379        will be matched as a substring.
-380        """
-381        num_matches = self.count(table, match_criteria, exact_match)
-382        conditions = self._get_conditions(match_criteria, exact_match)
-383        try:
-384            self.cursor.execute(f"delete from {table} where {conditions}")
-385            self.logger.info(
-386                f'Deleted {num_matches} from "{table}" where {conditions}".'
-387            )
-388            return num_matches
-389        except Exception as e:
-390            self.logger.debug(f'Error deleting from "{table}" where
+372    ) -> int:
+373        """Delete records from `table`.
+374
+375        Returns the number of deleted records.
+376
+377        #### :params:
+378
+379        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+(column_name, value)`
+380        or a dictionary where keys are column names and values are
+corresponding values.
+381
+382        `exact_match`: If `False`, the value for a given column will be
+matched as a substring.
+383        """
+384        num_matches = self.count(table, match_criteria, exact_match)
+385        conditions = self._get_conditions(match_criteria, exact_match)
+386        try:
+387            self.cursor.execute(f"delete from {table} where {conditions};")
+388            self.logger.info(
+389                f'Deleted {num_matches} from "{table}" where {conditions}".'
+390            )
+391            return num_matches
+392        except Exception as e:
+393            self.logger.debug(f'Error deleting from "{table}" where
 {conditions}.\n{e}')
-391            return 0
+394            return 0
 Delete records from table.
-Returns number of deleted records.
-* Parameters *
-    * match_criteria: Can be a list of 2-tuples where each tuple is
-      (columnName, rowValue) or a dictionary where keys are column names and
-      values are row values.
-    * exact_match: If False, the rowValue for a give column will be matched as
-      a substring.
+Returns the number of deleted records.
+*** :params: ***
+match_criteria: Can be a list of 2-tuples where each tuple is (column_name,
+value) or a dictionary where keys are column names and values are corresponding
+values.
+exact_match: If False, the value for a given column will be matched as a
+substring.
 ⁰
 def update(
 self,
 table: str,
 column_to_update: str,
 new_value: Any,
 match_criteria: list[tuple] | dict | None = None) -> bool: View Source
-393    @_connect
-394    def update(
-395        self,
-396        table: str,
-397        column_to_update: str,
-398        new_value: Any,
-399        match_criteria: list[tuple] | dict | None = None,
-400    ) -> bool:
-401        """Update row value for entry matched with match_criteria.
-402
-403        :param column_to_update: The column to be updated in the matched
-row.
-404
-405        :param new_value: The new value to insert.
-406
-407        :param match_criteria: Can be a list of 2-tuples where each
-408        tuple is (columnName, rowValue) or a dictionary where
-409        keys are column names and values are row values.
-410        If None, every row will be updated.
+396    @_connect
+397    def update(
+398        self,
+399        table: str,
+400        column_to_update: str,
+401        new_value: Any,
+402        match_criteria: list[tuple] | dict | None = None,
+403    ) -> bool:
+404        """Update the value in `column_to_update` to `new_value` for rows
+matched with `match_criteria`.
+405
+406        #### :params:
+407
+408        `table`: The table to update rows in.
+409
+410        `column_to_update`: The column to be updated in the matched rows.
 411
-412        Returns True if successful, False if not."""
-413        query = f"update {table} set {column_to_update} = ?"
-414        conditions = ""
-415        if match_criteria:
-416            if self.count(table, match_criteria) == 0:
-417                self.logger.info(
-418                    f"Couldn't find matching records in {table} table to
+412        `new_value`: The new value to insert.
+413
+414        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+(columnName, rowValue)`
+415        or a dictionary where keys are column names and values are
+corresponding values.
+416        If `None`, every row in `table` will be updated.
+417
+418        Returns `True` if successful, `False` if not."""
+419        query = f"update {table} set {column_to_update} = ?"
+420        conditions = ""
+421        if match_criteria:
+422            if self.count(table, match_criteria) == 0:
+423                self.logger.info(
+424                    f"Couldn't find matching records in {table} table to
 update to '{new_value}'"
-419                )
-420                return False
-421            conditions = self._get_conditions(match_criteria)
-422            query += f" where {conditions}"
-423        else:
-424            conditions = None
-425        try:
-426            self.cursor.execute(
-427                query,
-428                (new_value,),
-429            )
-430            self.logger.info(
-431                f'Updated "{column_to_update}" in "{table}" table to "
+425                )
+426                return False
+427            conditions = self._get_conditions(match_criteria)
+428            query += f" where {conditions}"
+429        else:
+430            conditions = None
+431        query += ";"
+432        try:
+433            self.cursor.execute(
+434                query,
+435                (new_value,),
+436            )
+437            self.logger.info(
+438                f'Updated "{column_to_update}" in "{table}" table to "
 {new_value}" where {conditions}'
-432            )
-433            return True
-434        except Exception as e:
-435            self.logger.error(
-436                f'Failed to update "{column_to_update}" in "{table}" table
+439            )
+440            return True
+441        except Exception as e:
+442            self.logger.error(
+443                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-437            )
-438            return False
-Update row value for entry matched with match_criteria.
-* Parameters *
-    * column_to_update: The column to be updated in the matched row.
-    * new_value: The new value to insert.
-    * match_criteria: Can be a list of 2-tuples where each tuple is
-      (columnName, rowValue) or a dictionary where keys are column names and
-      values are row values. If None, every row will be updated.
+444            )
+445            return False
+Update the value in column_to_update to new_value for rows matched with
+match_criteria.
+*** :params: ***
+table: The table to update rows in.
+column_to_update: The column to be updated in the matched rows.
+new_value: The new value to insert.
+match_criteria: Can be a list of 2-tuples where each tuple is (columnName,
+rowValue) or a dictionary where keys are column names and values are
+corresponding values. If None, every row in table will be updated.
 Returns True if successful, False if not.
 ⁰
 def drop_table(self, table: str) -> bool: View Source
-440    @_connect
-441    def drop_table(self, table: str) -> bool:
-442        """Drop a table from the database.
-443
-444        Returns True if successful, False if not."""
-445        try:
-446            self.cursor.execute(f"drop Table {table}")
-447            self.logger.info(f'Dropped table "{table}"')
-448            return True
-449        except Exception as e:
-450            print(e)
-451            self.logger.error(f'Failed to drop table "{table}"')
-452            return False
-Drop a table from the database.
+447    @_connect
+448    def drop_table(self, table: str) -> bool:
+449        """Drop `table` from the database.
+450
+451        Returns `True` if successful, `False` if not."""
+452        try:
+453            self.cursor.execute(f"drop Table {table};")
+454            self.logger.info(f'Dropped table "{table}"')
+455            return True
+456        except Exception as e:
+457            print(e)
+458            self.logger.error(f'Failed to drop table "{table}"')
+459            return False
+Drop table from the database.
 Returns True if successful, False if not.
 ⁰
 def add_column(
 self,
 table: str,
 column: str,
 _type: str,
 default_value: str | None = None): View Source
-454    @_connect
-455    def add_column(
-456        self, table: str, column: str, _type: str, default_value: str | None
+461    @_connect
+462    def add_column(
+463        self, table: str, column: str, _type: str, default_value: str | None
 = None
-457    ):
-458        """Add a new column to table.
-459
-460        :param column: Name of the column to add.
-461
-462        :param _type: The data type of the new column.
-463
-464        :param default_value: Optional default value for the column."""
-465        try:
-466            if default_value:
-467                self.cursor.execute(
-468                    f"alter table {table} add column {column} {_type}
-default {default_value}"
-469                )
-470            else:
-471                self.cursor.execute(f"alter table {table} add column
-{column} {_type}")
-472            self.logger.info(f'Added column "{column}" to "{table}" table.')
-473        except Exception as e:
-474            self.logger.error(f'Failed to add column "{column}" to "{table}"
+464    ):
+465        """Add a new column to `table`.
+466
+467        #### :params:
+468
+469        `column`: Name of the column to add.
+470
+471        `_type`: The data type of the new column.
+472
+473        `default_value`: Optional default value for the column."""
+474        try:
+475            if default_value:
+476                self.cursor.execute(
+477                    f"alter table {table} add column {column} {_type}
+default {default_value};"
+478                )
+479                self.update(table, column, default_value)
+480            else:
+481                self.cursor.execute(f"alter table {table} add column
+{column} {_type};")
+482            self.logger.info(f'Added column "{column}" to "{table}" table.')
+483        except Exception as e:
+484            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
 Add a new column to table.
-* Parameters *
-    * column: Name of the column to add.
-    * _type: The data type of the new column.
-    * default_value: Optional default value for the column.
+*** :params: ***
+column: Name of the column to add.
+_type: The data type of the new column.
+default_value: Optional default value for the column.
 ⁰
 @staticmethod
 def data_to_string(
 data: list[dict],
 sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-476    @staticmethod
-477    def data_to_string(
-478        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+486    @staticmethod
+487    def data_to_string(
+488        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-479    ) -> str:
-480        """Uses tabulate to produce pretty string output
-481        from a list of dictionaries.
-482
-483        :param data: Assumes all dictionaries in list have the same set of
-keys.
-484
-485        :param sort_key: Optional dictionary key to sort data with.
-486
-487        :param wrap_to_terminal: If True, the table width will be wrapped
-488        to fit within the current terminal window. Set to False
-489        if the output is going into something like a txt file."""
-490        return data_to_string(data, sort_key, wrap_to_terminal)
+489    ) -> str:
+490        """Uses tabulate to produce pretty string output from a list of
+dictionaries.
+491
+492        #### :params:
+493
+494        `data`: The list of dictionaries to create a grid from.
+495        Assumes all dictionaries in list have the same set of keys.
+496
+497        `sort_key`: Optional dictionary key to sort data with.
+498
+499        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+fit within the current terminal window.
+500        Pass as `False` if the output is going into something like a `.txt`
+file."""
+501        return data_to_string(data, sort_key, wrap_to_terminal)
 Uses tabulate to produce pretty string output from a list of dictionaries.
-* Parameters *
-    * data: Assumes all dictionaries in list have the same set of keys.
-    * sort_key: Optional dictionary key to sort data with.
-    * wrap_to_terminal: If True, the table width will be wrapped to fit within
-      the current terminal window. Set to False if the output is going into
-      something like a txt file.
+*** :params: ***
+data: The list of dictionaries to create a grid from. Assumes all dictionaries
+in list have the same set of keys.
+sort_key: Optional dictionary key to sort data with.
+wrap_to_terminal: If True, the table width will be wrapped to fit within the
+current terminal window. Pass as False if the output is going into something
+like a .txt file.
   ⁰
 def data_to_string(
 data: list[dict],
 sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-493def data_to_string(
-494    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+504def data_to_string(
+505    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
 True
-495) -> str:
-496    """Use tabulate to produce grid output from a list of dictionaries.
-497
-498    :param data: Assumes all dictionaries in list have the same set of keys.
-499
-500    :param sort_key: Optional dictionary key to sort data with.
-501
-502    :param wrap_to_terminal: If True, the column widths will be reduced so
-the grid fits
-503    within the current terminal window without wrapping. If the column
-widths have reduced to 1
-504    and the grid is still too wide, str(data) will be returned."""
-505    if len(data) == 0:
-506        return ""
-507    if sort_key:
-508        data = sorted(data, key=lambda d: d[sort_key])
-509    for i, d in enumerate(data):
-510        for k in d:
-511            data[i][k] = str(data[i][k])
-512
-513    too_wide = True
-514    terminal_width = os.get_terminal_size().columns
-515    max_col_widths = terminal_width
-516    # Make an output with effectively unrestricted column widths
-517    # to see if shrinking is necessary
-518    output = tabulate(
-519        data,
-520        headers="keys",
-521        disable_numparse=True,
-522        tablefmt="grid",
-523        maxcolwidths=max_col_widths,
-524    )
-525    current_width = output.index("\n")
-526    if current_width < terminal_width:
-527        too_wide = False
-528    if wrap_to_terminal and too_wide:
-529        print("Resizing grid to fit within the terminal...")
-530        previous_col_widths = max_col_widths
-531        acceptable_width = terminal_width - 10
-532        while too_wide and max_col_widths > 1:
-533            if current_width > terminal_width:
-534                previous_col_widths = max_col_widths
-535                max_col_widths = int(max_col_widths * 0.5)
-536            elif current_width < terminal_width:
-537                # Without lowering acceptable_width, this condition will
+506) -> str:
+507    """Uses tabulate to produce pretty string output from a list of
+dictionaries.
+508
+509    #### :params:
+510
+511    `data`: The list of dictionaries to create a grid from.
+512    Assumes all dictionaries in list have the same set of keys.
+513
+514    `sort_key`: Optional dictionary key to sort data with.
+515
+516    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
+within the current terminal window.
+517    Pass as `False` if the output is going into something like a `.txt`
+file."""
+518    if len(data) == 0:
+519        return ""
+520    if sort_key:
+521        data = sorted(data, key=lambda d: d[sort_key])
+522    for i, d in enumerate(data):
+523        for k in d:
+524            data[i][k] = str(data[i][k])
+525
+526    too_wide = True
+527    terminal_width = os.get_terminal_size().columns
+528    max_col_widths = terminal_width
+529    # Make an output with effectively unrestricted column widths
+530    # to see if shrinking is necessary
+531    output = tabulate(
+532        data,
+533        headers="keys",
+534        disable_numparse=True,
+535        tablefmt="grid",
+536        maxcolwidths=max_col_widths,
+537    )
+538    current_width = output.index("\n")
+539    if current_width < terminal_width:
+540        too_wide = False
+541    if wrap_to_terminal and too_wide:
+542        print("Resizing grid to fit within the terminal...\n")
+543        previous_col_widths = max_col_widths
+544        acceptable_width = terminal_width - 10
+545        while too_wide and max_col_widths > 1:
+546            if current_width >= terminal_width:
+547                previous_col_widths = max_col_widths
+548                max_col_widths = int(max_col_widths * 0.5)
+549            elif current_width < terminal_width:
+550                # Without lowering acceptable_width, this condition will
 cause infinite loop
-538                if max_col_widths == previous_col_widths - 1:
-539                    acceptable_width -= 10
-540                max_col_widths = int(
-541                    max_col_widths + (0.5 * (previous_col_widths -
+551                if max_col_widths == previous_col_widths - 1:
+552                    acceptable_width -= 10
+553                max_col_widths = int(
+554                    max_col_widths + (0.5 * (previous_col_widths -
 max_col_widths))
-542                )
-543            output = tabulate(
-544                data,
-545                headers="keys",
-546                disable_numparse=True,
-547                tablefmt="grid",
-548                maxcolwidths=max_col_widths,
-549            )
-550            current_width = output.index("\n")
-551            if acceptable_width < current_width < terminal_width:
-552                too_wide = False
-553        if too_wide:
-554            print("Couldn't resize grid to fit within the terminal.")
-555            return str(data)
-556    return output
-Use tabulate to produce grid output from a list of dictionaries.
-* Parameters *
-    * data: Assumes all dictionaries in list have the same set of keys.
-    * sort_key: Optional dictionary key to sort data with.
-    * wrap_to_terminal: If True, the column widths will be reduced so the grid
-      fits within the current terminal window without wrapping. If the column
-      widths have reduced to 1 and the grid is still too wide, str(data) will
-      be returned.
+555                )
+556            output = tabulate(
+557                data,
+558                headers="keys",
+559                disable_numparse=True,
+560                tablefmt="grid",
+561                maxcolwidths=max_col_widths,
+562            )
+563            current_width = output.index("\n")
+564            if acceptable_width < current_width < terminal_width:
+565                too_wide = False
+566        if too_wide:
+567            print("Couldn't resize grid to fit within the terminal.")
+568            return str(data)
+569    return output
+Uses tabulate to produce pretty string output from a list of dictionaries.
+*** :params: ***
+data: The list of dictionaries to create a grid from. Assumes all dictionaries
+in list have the same set of keys.
+sort_key: Optional dictionary key to sort data with.
+wrap_to_terminal: If True, the table width will be wrapped to fit within the
+current terminal window. Pass as False if the output is going into something
+like a .txt file.
```

### Comparing `databased-1.5.0/docs/databased/dbmanager.html` & `databased-1.5.1/docs/databased/dbmanager.html`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                         <li>
                                 <a class="function" href="#DBManager.do_add_row">do_add_row</a>
                         </li>
                         <li>
                                 <a class="function" href="#DBManager.do_info">do_info</a>
                         </li>
                         <li>
-                                <a class="function" href="#DBManager.do_find">do_find</a>
+                                <a class="function" href="#DBManager.do_show">do_show</a>
                         </li>
                         <li>
                                 <a class="function" href="#DBManager.do_search">do_search</a>
                         </li>
                         <li>
                                 <a class="function" href="#DBManager.do_count">do_count</a>
                         </li>
@@ -183,15 +183,15 @@
 </span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">),</span>
 </span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>                <span class="p">}</span>
 </span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
 </span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>            <span class="p">]</span>
 </span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
 </span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="k">def</span> <span class="nf">do_find</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
 </span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
 </span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
 </span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
 </span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
 </span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
 </span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
@@ -459,15 +459,15 @@
 </span><span id="DBManager-71"><a href="#DBManager-71"><span class="linenos"> 71</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">),</span>
 </span><span id="DBManager-72"><a href="#DBManager-72"><span class="linenos"> 72</span></a>                <span class="p">}</span>
 </span><span id="DBManager-73"><a href="#DBManager-73"><span class="linenos"> 73</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
 </span><span id="DBManager-74"><a href="#DBManager-74"><span class="linenos"> 74</span></a>            <span class="p">]</span>
 </span><span id="DBManager-75"><a href="#DBManager-75"><span class="linenos"> 75</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
 </span><span id="DBManager-76"><a href="#DBManager-76"><span class="linenos"> 76</span></a>
 </span><span id="DBManager-77"><a href="#DBManager-77"><span class="linenos"> 77</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBManager-78"><a href="#DBManager-78"><span class="linenos"> 78</span></a>    <span class="k">def</span> <span class="nf">do_find</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBManager-78"><a href="#DBManager-78"><span class="linenos"> 78</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
 </span><span id="DBManager-79"><a href="#DBManager-79"><span class="linenos"> 79</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
 </span><span id="DBManager-80"><a href="#DBManager-80"><span class="linenos"> 80</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
 </span><span id="DBManager-81"><a href="#DBManager-81"><span class="linenos"> 81</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
 </span><span id="DBManager-82"><a href="#DBManager-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
 </span><span id="DBManager-83"><a href="#DBManager-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
 </span><span id="DBManager-84"><a href="#DBManager-84"><span class="linenos"> 84</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
 </span><span id="DBManager-85"><a href="#DBManager-85"><span class="linenos"> 85</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
@@ -865,56 +865,56 @@
             <div class="docstring"><p>Print out the names of the database tables, their columns, and the number of rows.
 Pass a space-separated list of table names to only print info for those specific tables,
 otherwise all tables will be printed.</p>
 </div>
 
 
                             </div>
-                            <div id="DBManager.do_find" class="classattr">
-                                        <input id="DBManager.do_find-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="DBManager.do_show" class="classattr">
+                                        <input id="DBManager.do_show-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@argshell.with_parser(dbparsers.get_lookup_parser, [dbparsers.convert_match_pairs])</div>
 
         <span class="def">def</span>
-        <span class="name">do_find</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
+        <span class="name">do_show</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
-                <label class="view-source-button" for="DBManager.do_find-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="DBManager.do_show-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#DBManager.do_find"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBManager.do_find-77"><a href="#DBManager.do_find-77"><span class="linenos"> 77</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBManager.do_find-78"><a href="#DBManager.do_find-78"><span class="linenos"> 78</span></a>    <span class="k">def</span> <span class="nf">do_find</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBManager.do_find-79"><a href="#DBManager.do_find-79"><span class="linenos"> 79</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
-</span><span id="DBManager.do_find-80"><a href="#DBManager.do_find-80"><span class="linenos"> 80</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
-</span><span id="DBManager.do_find-81"><a href="#DBManager.do_find-81"><span class="linenos"> 81</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
-</span><span id="DBManager.do_find-82"><a href="#DBManager.do_find-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
-</span><span id="DBManager.do_find-83"><a href="#DBManager.do_find-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
-</span><span id="DBManager.do_find-84"><a href="#DBManager.do_find-84"><span class="linenos"> 84</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBManager.do_find-85"><a href="#DBManager.do_find-85"><span class="linenos"> 85</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
-</span><span id="DBManager.do_find-86"><a href="#DBManager.do_find-86"><span class="linenos"> 86</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DBManager.do_find-87"><a href="#DBManager.do_find-87"><span class="linenos"> 87</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DBManager.do_find-88"><a href="#DBManager.do_find-88"><span class="linenos"> 88</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBManager.do_find-89"><a href="#DBManager.do_find-89"><span class="linenos"> 89</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBManager.do_find-90"><a href="#DBManager.do_find-90"><span class="linenos"> 90</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBManager.do_find-91"><a href="#DBManager.do_find-91"><span class="linenos"> 91</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DBManager.do_find-92"><a href="#DBManager.do_find-92"><span class="linenos"> 92</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBManager.do_find-93"><a href="#DBManager.do_find-93"><span class="linenos"> 93</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBManager.do_find-94"><a href="#DBManager.do_find-94"><span class="linenos"> 94</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
-</span><span id="DBManager.do_find-95"><a href="#DBManager.do_find-95"><span class="linenos"> 95</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
-</span><span id="DBManager.do_find-96"><a href="#DBManager.do_find-96"><span class="linenos"> 96</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
-</span><span id="DBManager.do_find-97"><a href="#DBManager.do_find-97"><span class="linenos"> 97</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBManager.do_find-98"><a href="#DBManager.do_find-98"><span class="linenos"> 98</span></a>                <span class="p">)</span>
-</span><span id="DBManager.do_find-99"><a href="#DBManager.do_find-99"><span class="linenos"> 99</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DBManager.do_find-100"><a href="#DBManager.do_find-100"><span class="linenos">100</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
-</span><span id="DBManager.do_find-101"><a href="#DBManager.do_find-101"><span class="linenos">101</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="DBManager.do_find-102"><a href="#DBManager.do_find-102"><span class="linenos">102</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBManager.do_find-103"><a href="#DBManager.do_find-103"><span class="linenos">103</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBManager.do_find-104"><a href="#DBManager.do_find-104"><span class="linenos">104</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
-</span><span id="DBManager.do_find-105"><a href="#DBManager.do_find-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBManager.do_find-106"><a href="#DBManager.do_find-106"><span class="linenos">106</span></a>                <span class="nb">print</span><span class="p">()</span>
+    <a class="headerlink" href="#DBManager.do_show"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBManager.do_show-77"><a href="#DBManager.do_show-77"><span class="linenos"> 77</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBManager.do_show-78"><a href="#DBManager.do_show-78"><span class="linenos"> 78</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBManager.do_show-79"><a href="#DBManager.do_show-79"><span class="linenos"> 79</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
+</span><span id="DBManager.do_show-80"><a href="#DBManager.do_show-80"><span class="linenos"> 80</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
+</span><span id="DBManager.do_show-81"><a href="#DBManager.do_show-81"><span class="linenos"> 81</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
+</span><span id="DBManager.do_show-82"><a href="#DBManager.do_show-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
+</span><span id="DBManager.do_show-83"><a href="#DBManager.do_show-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
+</span><span id="DBManager.do_show-84"><a href="#DBManager.do_show-84"><span class="linenos"> 84</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBManager.do_show-85"><a href="#DBManager.do_show-85"><span class="linenos"> 85</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
+</span><span id="DBManager.do_show-86"><a href="#DBManager.do_show-86"><span class="linenos"> 86</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DBManager.do_show-87"><a href="#DBManager.do_show-87"><span class="linenos"> 87</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DBManager.do_show-88"><a href="#DBManager.do_show-88"><span class="linenos"> 88</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBManager.do_show-89"><a href="#DBManager.do_show-89"><span class="linenos"> 89</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBManager.do_show-90"><a href="#DBManager.do_show-90"><span class="linenos"> 90</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBManager.do_show-91"><a href="#DBManager.do_show-91"><span class="linenos"> 91</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DBManager.do_show-92"><a href="#DBManager.do_show-92"><span class="linenos"> 92</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBManager.do_show-93"><a href="#DBManager.do_show-93"><span class="linenos"> 93</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBManager.do_show-94"><a href="#DBManager.do_show-94"><span class="linenos"> 94</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
+</span><span id="DBManager.do_show-95"><a href="#DBManager.do_show-95"><span class="linenos"> 95</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
+</span><span id="DBManager.do_show-96"><a href="#DBManager.do_show-96"><span class="linenos"> 96</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
+</span><span id="DBManager.do_show-97"><a href="#DBManager.do_show-97"><span class="linenos"> 97</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBManager.do_show-98"><a href="#DBManager.do_show-98"><span class="linenos"> 98</span></a>                <span class="p">)</span>
+</span><span id="DBManager.do_show-99"><a href="#DBManager.do_show-99"><span class="linenos"> 99</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DBManager.do_show-100"><a href="#DBManager.do_show-100"><span class="linenos">100</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="DBManager.do_show-101"><a href="#DBManager.do_show-101"><span class="linenos">101</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="DBManager.do_show-102"><a href="#DBManager.do_show-102"><span class="linenos">102</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBManager.do_show-103"><a href="#DBManager.do_show-103"><span class="linenos">103</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBManager.do_show-104"><a href="#DBManager.do_show-104"><span class="linenos">104</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
+</span><span id="DBManager.do_show-105"><a href="#DBManager.do_show-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBManager.do_show-106"><a href="#DBManager.do_show-106"><span class="linenos">106</span></a>                <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Find and print rows from the database.
 Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.
 Use the -c/--columns flag to limit what columns are printed.
 Use the -o/--order_by flag to order the results.
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
           o do_dbpath
           o do_backup
           o do_size
           o do_create_table
           o do_drop_table
           o do_add_row
           o do_info
-          o do_find
+          o do_show
           o do_search
           o do_count
           o do_query
           o do_update
           o do_delete
           o do_flush_log
           o do_customize
@@ -101,15 +101,15 @@
 _71                }
 _72                for table in tables
 _73            ]
 _74        print(DataBased.data_to_string(info))
 _75
 _76    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-_77    def do_find(self, args: argshell.Namespace):
+_77    def do_show(self, args: argshell.Namespace):
 _78        """Find and print rows from the database.
 _79        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
 the search.
 _80        Use the -c/--columns flag to limit what columns are printed.
 _81        Use the -o/--order_by flag to order the results.
 _82        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs
@@ -395,15 +395,15 @@
 _72                }
 _73                for table in tables
 _74            ]
 _75        print(DataBased.data_to_string(info))
 _76
 _77    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-_78    def do_find(self, args: argshell.Namespace):
+_78    def do_show(self, args: argshell.Namespace):
 _79        """Find and print rows from the database.
 _80        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
 the search.
 _81        Use the -c/--columns flag to limit what columns are printed.
 _82        Use the -o/--order_by flag to order the results.
 _83        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs
@@ -701,18 +701,18 @@
 75        print(DataBased.data_to_string(info))
 Print out the names of the database tables, their columns, and the number of
 rows. Pass a space-separated list of table names to only print info for those
 specific tables, otherwise all tables will be printed.
 ⁰
 @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-def do_find(self, args: argshell.argshell.Namespace): View Source
+def do_show(self, args: argshell.argshell.Namespace): View Source
 _77    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-_78    def do_find(self, args: argshell.Namespace):
+_78    def do_show(self, args: argshell.Namespace):
 _79        """Find and print rows from the database.
 _80        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
 the search.
 _81        Use the -c/--columns flag to limit what columns are printed.
 _82        Use the -o/--order_by flag to order the results.
 _83        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs
```

### Comparing `databased-1.5.0/docs/databased/dbparsers.html` & `databased-1.5.1/docs/databased/dbparsers.html`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/src/databased/custom_manager.py` & `databased-1.5.1/src/databased/custom_manager.py`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/src/databased/databased.py` & `databased-1.5.1/src/databased/databased.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,21 +33,22 @@
     def __init__(
         self,
         dbpath: str | Pathier,
         logger_encoding: str = "utf-8",
         logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
     ):
         """
-        :param dbpath: String or Path object to database file.
+        #### :params:
+
+        `dbpath`: String or Path object to database file.
         If a relative path is given, it will be relative to the
         current working directory. The log file will be saved to the
         same directory.
 
-        :param logger_message_format: '{' style format string
-        for the logger object."""
+        `logger_message_format`: '{' style format string for the logger object."""
         self.dbpath = Pathier(dbpath)
         self.dbname = Pathier(dbpath).name
         self.dbpath.parent.mkdir(parents=True, exist_ok=True)
         self._logger_init(
             encoding=logger_encoding, message_format=logger_message_format
         )
         self.connection_open = False
@@ -62,15 +63,15 @@
     def open(self):
         """Open connection to db."""
         self.connection = sqlite3.connect(
             self.dbpath,
             detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
             timeout=10,
         )
-        self.connection.execute("pragma foreign_keys = 1")
+        self.connection.execute("pragma foreign_keys = 1;")
         self.cursor = self.connection.cursor()
         self.connection_open = True
 
     def close(self):
         """Save and close connection to db.
 
         Call this as soon as you are done using the database if you have
@@ -81,15 +82,15 @@
             self.connection_open = False
 
     def _logger_init(
         self,
         message_format: str = "{levelname}|-|{asctime}|-|{message}",
         encoding: str = "utf-8",
     ):
-        """:param message_format: '{' style format string"""
+        """:param `message_format`: '{' style format string"""
         self.logger = logging.getLogger(self.dbname)
         if not self.logger.hasHandlers():
             handler = logging.FileHandler(
                 str(self.dbpath).replace(".", "") + ".log", encoding=encoding
             )
             handler.setFormatter(
                 logging.Formatter(
@@ -100,43 +101,47 @@
             self.logger.setLevel(logging.INFO)
 
     def _get_dict(
         self, table: str, values: list, columns_to_return: list[str] | None = None
     ) -> dict:
         """Converts the values of a row into a dictionary with column names as keys.
 
-        :param table: The table that values were pulled from.
+        #### :params:
+
+        `table`: The table that values were pulled from.
 
-        :param values: List of values expected to be the same quantity
+        `values`: List of values expected to be the same quantity
         and in the same order as the column names of table.
 
-        :param columns_to_return: An optional list of column names.
+        `columns_to_return`: An optional list of column names.
         If given, only these columns will be included in the returned dictionary.
         Otherwise all columns and values are returned."""
         return {
             column: value
             for column, value in zip(self.get_column_names(table), values)
             if not columns_to_return or column in columns_to_return
         }
 
     def _get_conditions(
         self, match_criteria: list[tuple] | dict, exact_match: bool = True
     ) -> str:
         """Builds and returns the conditional portion of a query.
 
-        :param match_criteria: Can be a list of 2-tuples where each
-        tuple is (columnName, rowValue) or a dictionary where
+        #### :params:
+
+        `match_criteria`: Can be a list of 2-tuples where each
+        tuple is `(columnName, rowValue)` or a dictionary where
         keys are column names and values are row values.
 
-        :param exact_match: If False, the rowValue for a give column
+        `exact_match`: If `False`, the row value for a given column
         will be matched as a substring.
 
         Usage e.g.:
 
-        self.cursor.execute(f'select * from {table} where {conditions}')"""
+        >>> self.cursor.execute(f'select * from {table} where {conditions};')"""
         if type(match_criteria) == dict:
             match_criteria = [(k, v) for k, v in match_criteria.items()]
         if exact_match:
             conditions = " and ".join(
                 f'"{column_row[0]}" = "{column_row[1]}"'
                 for column_row in match_criteria
             )
@@ -145,51 +150,50 @@
                 f'"{column_row[0]}" like "%{column_row[1]}%"'
                 for column_row in match_criteria
             )
         return f"({conditions})"
 
     @_connect
     def query(self, query_) -> list[Any]:
-        """Execute an arbitrary query and
-        return the results."""
+        """Execute an arbitrary query and return the results."""
         self.cursor.execute(query_)
         return self.cursor.fetchall()
 
     @_connect
-    def create_tables(self, table_querys: list[str] = []):
+    def create_tables(self, table_defs: list[str] = []):
         """Create tables if they don't exist.
 
-        :param table_querys: Each query should be
-        in the form 'tableName(columnDefinitions)'"""
-        if len(table_querys) > 0:
+        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`"""
+        if len(table_defs) > 0:
             table_names = self.get_table_names()
-            for table in table_querys:
+            for table in table_defs:
                 if table.split("(")[0].strip() not in table_names:
-                    self.cursor.execute(f"create table {table}")
+                    self.cursor.execute(f"create table {table};")
                     self.logger.info(f'{table.split("(")[0]} table created.')
 
     @_connect
     def create_table(self, table: str, column_defs: list[str]):
         """Create a table if it doesn't exist.
 
-        :param table: Name of the table to create.
+        #### :params:
 
-        :param column_defs: List of column definitions in
-        proper Sqlite3 sytax.
-        i.e. "columnName text unique" or "columnName int primary key" etc."""
+        `table`: Name of the table to create.
+
+        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+        i.e. `"column_name text unique"` or `"column_name int primary key"` etc."""
         if table not in self.get_table_names():
-            query = f"create table {table}({', '.join(column_defs)})"
+            query = f"create table {table}({', '.join(column_defs)});"
             self.cursor.execute(query)
             self.logger.info(f"'{table}' table created.")
 
     @_connect
     def get_table_names(self) -> list[str]:
-        """Returns a list of table names from database."""
+        """Returns a list of table names from the database."""
         self.cursor.execute(
-            'select name from sqlite_Schema where type = "table" and name not like "sqlite_%"'
+            'select name from sqlite_Schema where type = "table" and name not like "sqlite_%";'
         )
         return [result[0] for result in self.cursor.fetchall()]
 
     @_connect
     def get_column_names(self, table: str) -> list[str]:
         """Return a list of column names from a table."""
         self.cursor.execute(f"select * from {table} where 1=0")
@@ -198,62 +202,65 @@
     @_connect
     def count(
         self,
         table: str,
         match_criteria: list[tuple] | dict | None = None,
         exact_match: bool = True,
     ) -> int:
-        """Return number of items in table.
+        """Return number of items in `table`.
+
+        #### :params:
 
-        :param match_criteria: Can be a list of 2-tuples where each
-        tuple is (columnName, rowValue) or a dictionary where
+        `match_criteria`: Can be a list of 2-tuples where each
+        tuple is `(columnName, rowValue)` or a dictionary where
         keys are column names and values are row values.
-        If None, all rows from the table will be counted.
+        If `None`, all rows from the table will be counted.
 
-        :param exact_match: If False, the row value for a give column
-        in match_criteria will be matched as a substring. Has no effect if
-        match_criteria is None.
+        `exact_match`: If `False`, the row value for a given column
+        in `match_criteria` will be matched as a substring.
+        Has no effect if `match_criteria` is `None`.
         """
         query = f"select count(_rowid_) from {table}"
         try:
             if match_criteria:
                 self.cursor.execute(
-                    f"{query} where {self._get_conditions(match_criteria, exact_match)}"
+                    f"{query} where {self._get_conditions(match_criteria, exact_match)};"
                 )
             else:
                 self.cursor.execute(f"{query}")
             return self.cursor.fetchone()[0]
         except:
             return 0
 
     @_connect
     def add_row(
         self, table: str, values: tuple[Any], columns: tuple[str] | None = None
     ):
-        """Add row of values to table.
+        """Add a row of values to a table.
+
+        #### :params:
 
-        :param table: The table to insert into.
+        `table`: The table to insert values into.
 
-        :param values: A tuple of values to be inserted into the table.
+        `values`: A tuple of values to be inserted into the table.
 
-        :param columns: If None, values param is expected to supply
-        a value for every column in the table. If columns is
-        provided, it should contain the same number of elements as values."""
+        `columns`: If `None`, `values` is expected to supply a value for every column in the table.
+        If `columns` is provided, it should contain the same number of elements as `values`."""
         parameterizer = ", ".join("?" for _ in values)
         logger_values = ", ".join(str(value) for value in values)
         try:
             if columns:
                 columns_query = ", ".join(column for column in columns)
                 self.cursor.execute(
-                    f"insert into {table} ({columns_query}) values({parameterizer})",
+                    f"insert into {table} ({columns_query}) values({parameterizer});",
                     values,
                 )
             else:
                 self.cursor.execute(
-                    f"insert into {table} values({parameterizer})", values
+                    f"insert into {table} values({parameterizer});", values
                 )
             self.logger.info(f'Added "{logger_values}" to {table} table.')
         except Exception as e:
             if "constraint" not in str(e).lower():
                 self.logger.exception(
                     f'Error adding "{logger_values}" to {table} table.'
                 )
@@ -269,47 +276,42 @@
         sort_by_column: str | None = None,
         columns_to_return: list[str] | None = None,
         return_as_dataframe: bool = False,
         values_only: bool = False,
         order_by: str | None = None,
         limit: str | int | None = None,
     ) -> list[dict] | list[tuple] | pandas.DataFrame:
-        """Returns rows from table as a list of dictionaries
-        where the key-value pairs of the dictionaries are
-        column name: row value.
+        """Return matching rows from `table`.
 
-        :param match_criteria: Can be a list of 2-tuples where each
-        tuple is (columnName, rowValue) or a dictionary where
+        By default, rows will be returned as a list of dictionaries of the form `[{"column_name": value, ...}, ...]`
+
+
+        #### :params:
+
+        `match_criteria`: Can be a list of 2-tuples where each
+        tuple is `(columnName, rowValue)` or a dictionary where
         keys are column names and values are row values.
 
-        :param exact_match: If False, the rowValue for a give column
-        will be matched as a substring.
+        `exact_match`: If `False`, the row value for a given column will be matched as a substring.
 
-        :param sort_by_column: A column name to sort the results by.
+        `sort_by_column`: A column name to sort the results by.
         This will sort results in Python after retrieving them from the db.
         Use the 'order_by' param to use SQLite engine for ordering.
 
-        :param columns_to_return: Optional list of column names.
-        If provided, the elements returned by get_rows() will
-        only contain the provided columns. Otherwise every column
-        in the row is returned.
-
-        :param return_as_dataframe: If True,
-        the results will be returned as a pandas.DataFrame object.
-
-        :param values_only: Return the results as a list of tuples
-        instead of a list of dictionaries that have column names as keys.
-        The results will still be sorted according to sort_by_column if
-        one is provided.
+        `columns_to_return`: Optional list of column names.
+        If provided, the elements returned by this function will only contain the provided columns.
+        Otherwise every column in the row is returned.
+
+        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.
+
+        `values_only`: Return the results as a list of tuples.
 
-        :param order_by: If given, a 'order by {order_by}' clause
-        will be added to the select query.
+        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.
 
-        :param limit: If given, a 'limit {limit}' clause will be
-        added to the select query.
+        `limit`: If given, a `limit {limit}` clause will be added to the select query.
         """
 
         if type(columns_to_return) is str:
             columns_to_return = [columns_to_return]
         query = f"select * from {table}"
         matches = []
         if match_criteria:
@@ -331,22 +333,23 @@
         else:
             return results
 
     @_connect
     def find(
         self, table: str, query_string: str, columns: list[str] | None = None
     ) -> list[dict]:
-        """Search for rows that contain query_string as a substring
-        of any column.
+        """Search for rows that contain `query_string` as a substring of any column.
 
-        :param table: The table to search.
+        #### :params:
 
-        :param query_string: The substring to search for in all columns.
+        `table`: The table to search.
 
-        :param columns: A list of columns to search for query_string.
+        `query_string`: The substring to search for in all columns.
+
+        `columns`: A list of columns to search for query_string.
         If None, all columns in the table will be searched.
         """
         if type(columns) is str:
             columns = [columns]
         results = []
         if not columns:
             columns = self.get_column_names(table)
@@ -362,29 +365,29 @@
             )
         return results
 
     @_connect
     def delete(
         self, table: str, match_criteria: list[tuple] | dict, exact_match: bool = True
     ) -> int:
-        """Delete records from table.
+        """Delete records from `table`.
 
-        Returns number of deleted records.
+        Returns the number of deleted records.
 
-        :param match_criteria: Can be a list of 2-tuples where each
-        tuple is (columnName, rowValue) or a dictionary where
-        keys are column names and values are row values.
+        #### :params:
 
-        :param exact_match: If False, the rowValue for a give column
-        will be matched as a substring.
+        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`
+        or a dictionary where keys are column names and values are corresponding values.
+
+        `exact_match`: If `False`, the value for a given column will be matched as a substring.
         """
         num_matches = self.count(table, match_criteria, exact_match)
         conditions = self._get_conditions(match_criteria, exact_match)
         try:
-            self.cursor.execute(f"delete from {table} where {conditions}")
+            self.cursor.execute(f"delete from {table} where {conditions};")
             self.logger.info(
                 f'Deleted {num_matches} from "{table}" where {conditions}".'
             )
             return num_matches
         except Exception as e:
             self.logger.debug(f'Error deleting from "{table}" where {conditions}.\n{e}')
             return 0
@@ -393,38 +396,42 @@
     def update(
         self,
         table: str,
         column_to_update: str,
         new_value: Any,
         match_criteria: list[tuple] | dict | None = None,
     ) -> bool:
-        """Update row value for entry matched with match_criteria.
+        """Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.
 
-        :param column_to_update: The column to be updated in the matched row.
+        #### :params:
 
-        :param new_value: The new value to insert.
+        `table`: The table to update rows in.
 
-        :param match_criteria: Can be a list of 2-tuples where each
-        tuple is (columnName, rowValue) or a dictionary where
-        keys are column names and values are row values.
-        If None, every row will be updated.
+        `column_to_update`: The column to be updated in the matched rows.
+
+        `new_value`: The new value to insert.
 
-        Returns True if successful, False if not."""
+        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`
+        or a dictionary where keys are column names and values are corresponding values.
+        If `None`, every row in `table` will be updated.
+
+        Returns `True` if successful, `False` if not."""
         query = f"update {table} set {column_to_update} = ?"
         conditions = ""
         if match_criteria:
             if self.count(table, match_criteria) == 0:
                 self.logger.info(
                     f"Couldn't find matching records in {table} table to update to '{new_value}'"
                 )
                 return False
             conditions = self._get_conditions(match_criteria)
             query += f" where {conditions}"
         else:
             conditions = None
+        query += ";"
         try:
             self.cursor.execute(
                 query,
                 (new_value,),
             )
             self.logger.info(
                 f'Updated "{column_to_update}" in "{table}" table to "{new_value}" where {conditions}'
@@ -434,77 +441,83 @@
             self.logger.error(
                 f'Failed to update "{column_to_update}" in "{table}" table to "{new_value}" where {conditions}"\n{e}'
             )
             return False
 
     @_connect
     def drop_table(self, table: str) -> bool:
-        """Drop a table from the database.
+        """Drop `table` from the database.
 
-        Returns True if successful, False if not."""
+        Returns `True` if successful, `False` if not."""
         try:
-            self.cursor.execute(f"drop Table {table}")
+            self.cursor.execute(f"drop Table {table};")
             self.logger.info(f'Dropped table "{table}"')
             return True
         except Exception as e:
             print(e)
             self.logger.error(f'Failed to drop table "{table}"')
             return False
 
     @_connect
     def add_column(
         self, table: str, column: str, _type: str, default_value: str | None = None
     ):
-        """Add a new column to table.
+        """Add a new column to `table`.
+
+        #### :params:
 
-        :param column: Name of the column to add.
+        `column`: Name of the column to add.
 
-        :param _type: The data type of the new column.
+        `_type`: The data type of the new column.
 
-        :param default_value: Optional default value for the column."""
+        `default_value`: Optional default value for the column."""
         try:
             if default_value:
                 self.cursor.execute(
-                    f"alter table {table} add column {column} {_type} default {default_value}"
+                    f"alter table {table} add column {column} {_type} default {default_value};"
                 )
+                self.update(table, column, default_value)
             else:
-                self.cursor.execute(f"alter table {table} add column {column} {_type}")
+                self.cursor.execute(f"alter table {table} add column {column} {_type};")
             self.logger.info(f'Added column "{column}" to "{table}" table.')
         except Exception as e:
             self.logger.error(f'Failed to add column "{column}" to "{table}" table.')
 
     @staticmethod
     def data_to_string(
         data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool = True
     ) -> str:
-        """Uses tabulate to produce pretty string output
-        from a list of dictionaries.
+        """Uses tabulate to produce pretty string output from a list of dictionaries.
 
-        :param data: Assumes all dictionaries in list have the same set of keys.
+        #### :params:
 
-        :param sort_key: Optional dictionary key to sort data with.
+        `data`: The list of dictionaries to create a grid from.
+        Assumes all dictionaries in list have the same set of keys.
 
-        :param wrap_to_terminal: If True, the table width will be wrapped
-        to fit within the current terminal window. Set to False
-        if the output is going into something like a txt file."""
+        `sort_key`: Optional dictionary key to sort data with.
+
+        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.
+        Pass as `False` if the output is going into something like a `.txt` file."""
         return data_to_string(data, sort_key, wrap_to_terminal)
 
 
 def data_to_string(
     data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool = True
 ) -> str:
-    """Use tabulate to produce grid output from a list of dictionaries.
+    """Uses tabulate to produce pretty string output from a list of dictionaries.
+
+    #### :params:
 
-    :param data: Assumes all dictionaries in list have the same set of keys.
+    `data`: The list of dictionaries to create a grid from.
+    Assumes all dictionaries in list have the same set of keys.
 
-    :param sort_key: Optional dictionary key to sort data with.
+    `sort_key`: Optional dictionary key to sort data with.
 
-    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits
-    within the current terminal window without wrapping. If the column widths have reduced to 1
-    and the grid is still too wide, str(data) will be returned."""
+    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.
+    Pass as `False` if the output is going into something like a `.txt` file."""
     if len(data) == 0:
         return ""
     if sort_key:
         data = sorted(data, key=lambda d: d[sort_key])
     for i, d in enumerate(data):
         for k in d:
             data[i][k] = str(data[i][k])
@@ -521,19 +534,19 @@
         tablefmt="grid",
         maxcolwidths=max_col_widths,
     )
     current_width = output.index("\n")
     if current_width < terminal_width:
         too_wide = False
     if wrap_to_terminal and too_wide:
-        print("Resizing grid to fit within the terminal...")
+        print("Resizing grid to fit within the terminal...\n")
         previous_col_widths = max_col_widths
         acceptable_width = terminal_width - 10
         while too_wide and max_col_widths > 1:
-            if current_width > terminal_width:
+            if current_width >= terminal_width:
                 previous_col_widths = max_col_widths
                 max_col_widths = int(max_col_widths * 0.5)
             elif current_width < terminal_width:
                 # Without lowering acceptable_width, this condition will cause infinite loop
                 if max_col_widths == previous_col_widths - 1:
                     acceptable_width -= 10
                 max_col_widths = int(
```

### Comparing `databased-1.5.0/src/databased/dbmanager.py` & `databased-1.5.1/src/databased/dbmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                     "Number of Rows": db.count(table),
                 }
                 for table in tables
             ]
         print(DataBased.data_to_string(info))
 
     @argshell.with_parser(dbparsers.get_lookup_parser, [dbparsers.convert_match_pairs])
-    def do_find(self, args: argshell.Namespace):
+    def do_show(self, args: argshell.Namespace):
         """Find and print rows from the database.
         Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.
         Use the -c/--columns flag to limit what columns are printed.
         Use the -o/--order_by flag to order the results.
         Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs
         Pass -h/--help flag for parser help."""
         print("Finding records... ")
```

### Comparing `databased-1.5.0/src/databased/dbparsers.py` & `databased-1.5.1/src/databased/dbparsers.py`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/LICENSE.txt` & `databased-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/README.md` & `databased-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `databased-1.5.0/pyproject.toml` & `databased-1.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
 authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "1.5.0"
+version = "1.5.1"
 requires-python = ">=3.10"
 dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier"]
 readme = "README.md"
 keywords = [
     "database",
     "sqlite",
     "sqlite3"
```

### Comparing `databased-1.5.0/PKG-INFO` & `databased-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 1.5.0
+Version: 1.5.1
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
```

